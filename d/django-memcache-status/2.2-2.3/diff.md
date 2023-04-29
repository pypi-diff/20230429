# Comparing `tmp/django-memcache-status-2.2.tar.gz` & `tmp/django-memcache-status-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-memcache-status-2.2.tar", last modified: Wed Feb  5 08:49:16 2020, max compression
+gzip compressed data, was "django-memcache-status-2.3.tar", last modified: Sat Apr 29 11:37:04 2023, max compression
```

## Comparing `django-memcache-status-2.2.tar` & `django-memcache-status-2.3.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-02-05 08:49:16.000000 django-memcache-status-2.2/
--rw-r--r--   0 martin     (501) staff       (20)     8257 2020-02-05 08:49:16.000000 django-memcache-status-2.2/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)     1103 2019-11-24 16:00:47.000000 django-memcache-status-2.2/LICENSE
--rw-r--r--   0 martin     (501) staff       (20)      200 2019-11-24 16:00:47.000000 django-memcache-status-2.2/MANIFEST.in
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-02-05 08:49:16.000000 django-memcache-status-2.2/django_memcache_status.egg-info/
--rw-r--r--   0 martin     (501) staff       (20)     8257 2020-02-05 08:49:16.000000 django-memcache-status-2.2/django_memcache_status.egg-info/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)        1 2019-11-24 16:10:13.000000 django-memcache-status-2.2/django_memcache_status.egg-info/not-zip-safe
--rw-r--r--   0 martin     (501) staff       (20)      913 2020-02-05 08:49:16.000000 django-memcache-status-2.2/django_memcache_status.egg-info/SOURCES.txt
--rw-r--r--   0 martin     (501) staff       (20)       17 2020-02-05 08:49:16.000000 django-memcache-status-2.2/django_memcache_status.egg-info/requires.txt
--rw-r--r--   0 martin     (501) staff       (20)       16 2020-02-05 08:49:16.000000 django-memcache-status-2.2/django_memcache_status.egg-info/top_level.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2020-02-05 08:49:16.000000 django-memcache-status-2.2/django_memcache_status.egg-info/dependency_links.txt
--rw-r--r--   0 martin     (501) staff       (20)      820 2020-02-05 08:39:59.000000 django-memcache-status-2.2/Pipfile
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-02-05 08:49:16.000000 django-memcache-status-2.2/memcache_status/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-02-05 08:49:16.000000 django-memcache-status-2.2/memcache_status/templatetags/
--rw-r--r--   0 martin     (501) staff       (20)        0 2019-11-24 16:00:47.000000 django-memcache-status-2.2/memcache_status/templatetags/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     2495 2019-11-24 16:00:47.000000 django-memcache-status-2.2/memcache_status/templatetags/memcache_status_tags.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-02-05 08:49:16.000000 django-memcache-status-2.2/memcache_status/tests/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-02-05 08:49:16.000000 django-memcache-status-2.2/memcache_status/tests/testapp/
--rw-r--r--   0 martin     (501) staff       (20)      127 2019-11-24 16:00:47.000000 django-memcache-status-2.2/memcache_status/tests/testapp/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     1629 2019-11-24 16:00:47.000000 django-memcache-status-2.2/memcache_status/tests/testapp/apps.py
--rw-r--r--   0 martin     (501) staff       (20)     3327 2019-11-24 16:00:47.000000 django-memcache-status-2.2/memcache_status/tests/testapp/settings.py
--rw-r--r--   0 martin     (501) staff       (20)      733 2019-11-24 16:00:47.000000 django-memcache-status-2.2/memcache_status/tests/testapp/urls.py
--rw-r--r--   0 martin     (501) staff       (20)       62 2019-11-24 16:00:47.000000 django-memcache-status-2.2/memcache_status/tests/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     2827 2019-11-24 17:17:01.000000 django-memcache-status-2.2/memcache_status/tests/tests.py
--rw-r--r--   0 martin     (501) staff       (20)      106 2019-11-24 16:00:47.000000 django-memcache-status-2.2/memcache_status/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)      573 2019-11-24 16:00:47.000000 django-memcache-status-2.2/memcache_status/apps.py
--rw-r--r--   0 martin     (501) staff       (20)      937 2019-11-24 16:00:47.000000 django-memcache-status-2.2/memcache_status/utils.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-02-05 08:49:16.000000 django-memcache-status-2.2/memcache_status/static/
--rw-r--r--   0 martin     (501) staff       (20)      771 2019-11-24 16:00:47.000000 django-memcache-status-2.2/memcache_status/static/memcache_status.css
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-02-05 08:49:16.000000 django-memcache-status-2.2/memcache_status/templates/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2020-02-05 08:49:16.000000 django-memcache-status-2.2/memcache_status/templates/memcache_status/
--rw-r--r--   0 martin     (501) staff       (20)      440 2019-11-24 16:19:55.000000 django-memcache-status-2.2/memcache_status/templates/memcache_status/admin_index.html
--rw-r--r--   0 martin     (501) staff       (20)     2757 2019-11-24 16:00:47.000000 django-memcache-status-2.2/memcache_status/templates/memcache_status/memcache_status.html
--rw-r--r--   0 martin     (501) staff       (20)       59 2019-11-24 16:00:47.000000 django-memcache-status-2.2/setup.py
--rw-r--r--   0 martin     (501) staff       (20)     1635 2020-02-05 08:30:44.000000 django-memcache-status-2.2/tox.ini
--rw-r--r--   0 martin     (501) staff       (20)     1621 2020-02-05 08:49:16.000000 django-memcache-status-2.2/setup.cfg
--rw-r--r--   0 martin     (501) staff       (20)     5929 2020-02-05 08:37:45.000000 django-memcache-status-2.2/README.rst
--rw-r--r--   0 martin     (501) staff       (20)    21541 2020-02-05 08:39:59.000000 django-memcache-status-2.2/Pipfile.lock
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-29 11:37:04.684343 django-memcache-status-2.3/
+-rw-r--r--   0 martin     (501) staff       (20)     1103 2023-04-28 22:23:09.000000 django-memcache-status-2.3/LICENSE
+-rw-r--r--   0 martin     (501) staff       (20)      223 2023-04-28 23:03:46.000000 django-memcache-status-2.3/MANIFEST.in
+-rw-r--r--   0 martin     (501) staff       (20)     6534 2023-04-29 11:37:04.684441 django-memcache-status-2.3/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)      606 2023-04-29 11:00:26.000000 django-memcache-status-2.3/Pipfile
+-rw-r--r--   0 martin     (501) staff       (20)    19813 2023-04-29 11:00:37.000000 django-memcache-status-2.3/Pipfile.lock
+-rw-r--r--   0 martin     (501) staff       (20)     5604 2023-04-29 11:35:17.000000 django-memcache-status-2.3/README.rst
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-29 11:37:04.682070 django-memcache-status-2.3/django_memcache_status.egg-info/
+-rw-r--r--   0 martin     (501) staff       (20)     6534 2023-04-29 11:37:04.000000 django-memcache-status-2.3/django_memcache_status.egg-info/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)      928 2023-04-29 11:37:04.000000 django-memcache-status-2.3/django_memcache_status.egg-info/SOURCES.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2023-04-29 11:37:04.000000 django-memcache-status-2.3/django_memcache_status.egg-info/dependency_links.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2023-04-28 22:23:26.000000 django-memcache-status-2.3/django_memcache_status.egg-info/not-zip-safe
+-rw-r--r--   0 martin     (501) staff       (20)       12 2023-04-29 11:37:04.000000 django-memcache-status-2.3/django_memcache_status.egg-info/requires.txt
+-rw-r--r--   0 martin     (501) staff       (20)       16 2023-04-29 11:37:04.000000 django-memcache-status-2.3/django_memcache_status.egg-info/top_level.txt
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-29 11:37:04.682485 django-memcache-status-2.3/memcache_status/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2023-04-28 22:34:53.000000 django-memcache-status-2.3/memcache_status/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)      589 2023-04-28 22:41:53.000000 django-memcache-status-2.3/memcache_status/apps.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-29 11:37:04.682639 django-memcache-status-2.3/memcache_status/static/
+-rw-r--r--   0 martin     (501) staff       (20)      771 2023-04-28 22:23:09.000000 django-memcache-status-2.3/memcache_status/static/memcache_status.css
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-29 11:37:04.679121 django-memcache-status-2.3/memcache_status/templates/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-29 11:37:04.683056 django-memcache-status-2.3/memcache_status/templates/memcache_status/
+-rw-r--r--   0 martin     (501) staff       (20)      440 2023-04-28 22:23:09.000000 django-memcache-status-2.3/memcache_status/templates/memcache_status/admin_index.html
+-rw-r--r--   0 martin     (501) staff       (20)     2764 2023-04-29 11:28:38.000000 django-memcache-status-2.3/memcache_status/templates/memcache_status/memcache_status.html
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-29 11:37:04.683345 django-memcache-status-2.3/memcache_status/templatetags/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2023-04-28 22:23:09.000000 django-memcache-status-2.3/memcache_status/templatetags/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     2823 2023-04-29 11:28:20.000000 django-memcache-status-2.3/memcache_status/templatetags/memcache_status_tags.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-29 11:37:04.683641 django-memcache-status-2.3/memcache_status/tests/
+-rw-r--r--   0 martin     (501) staff       (20)       47 2023-04-29 11:12:19.000000 django-memcache-status-2.3/memcache_status/tests/__init__.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-29 11:37:04.684211 django-memcache-status-2.3/memcache_status/tests/testapp/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2023-04-28 22:34:52.000000 django-memcache-status-2.3/memcache_status/tests/testapp/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     1604 2023-04-29 06:24:35.000000 django-memcache-status-2.3/memcache_status/tests/testapp/apps.py
+-rw-r--r--   0 martin     (501) staff       (20)     3058 2023-04-29 11:17:01.000000 django-memcache-status-2.3/memcache_status/tests/testapp/settings.py
+-rw-r--r--   0 martin     (501) staff       (20)      498 2023-04-29 11:14:14.000000 django-memcache-status-2.3/memcache_status/tests/testapp/urls.py
+-rw-r--r--   0 martin     (501) staff       (20)     3031 2023-04-29 11:13:39.000000 django-memcache-status-2.3/memcache_status/tests/tests.py
+-rw-r--r--   0 martin     (501) staff       (20)     1016 2023-04-29 11:08:11.000000 django-memcache-status-2.3/memcache_status/utils.py
+-rw-r--r--   0 martin     (501) staff       (20)     1653 2023-04-29 11:12:01.000000 django-memcache-status-2.3/pyproject.toml
+-rw-r--r--   0 martin     (501) staff       (20)      981 2023-04-29 11:37:04.684763 django-memcache-status-2.3/setup.cfg
+-rw-r--r--   0 martin     (501) staff       (20)       59 2023-04-28 22:23:09.000000 django-memcache-status-2.3/setup.py
+-rw-r--r--   0 martin     (501) staff       (20)      908 2023-04-29 11:05:26.000000 django-memcache-status-2.3/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-memcache-status-2.2/PKG-INFO` & `django-memcache-status-2.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,192 +1,197 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: django-memcache-status
-Version: 2.2
-Summary: A django application that displays the load and other statistics about your memcached instances in the admin.
+Version: 2.3
+Summary: "A django application that displays the load and other statistics about your memcached instances in the admin."
 Home-page: https://github.com/bartTC/django-memcache-status
 Author: Martin Mahner
 Author-email: martin@mahner.org
 License: MIT
-Description: .. image:: https://img.shields.io/pypi/v/django-memcache-status.svg
-            :target: https://pypi.org/project/django-memcache-status/
-        
-        .. image:: https://travis-ci.org/bartTC/django-memcache-status.svg?branch=master
-            :target: https://travis-ci.org/bartTC/django-memcache-status
-        
-        .. image:: https://api.codacy.com/project/badge/Coverage/1d7d0306c4d14fb9817017d7d23237fe
-            :target: https://www.codacy.com/app/bartTC/django-memcache-status
-        
-        .. image:: https://api.codacy.com/project/badge/Grade/1d7d0306c4d14fb9817017d7d23237fe
-            :target: https://www.codacy.com/app/bartTC/django-memcache-status
-        
-        -----
-        
-        ======================
-        django-memcache-status
-        ======================
-        
-        This app displays the current load and some statistics for your memcached_
-        instances in the index view of your Django admin section.
-        
-        Currently these memcached bindings are tested:
-        
-        ========================================================= ================================
-        Backend                                                   Support
-        ========================================================= ================================
-        `python-memcached`_ with vanilla Django                   ✅ Works fine with >= v1.57
-        pylibmc with `django-pylibmc`_                            ✅ Works fine
-        pymemcache with `django-pymemcache`_                      ❎ Does not provide stats
-        ========================================================= ================================
-        
-        Other bindings may provide statistics too.
-        
-        .. _memcached: http://www.danga.com/memcached/
-        .. _python-memcached: https://pypi.org/project/python-memcached/
-        .. _django-pylibmc: https://pypi.org/project/django-pylibmc/
-        .. _django-pymemcache: https://pypi.org/project/django-pymemcache/
-        
-        Installation
-        ============
-        
-        First add ``memcache_status`` to your ``INSTALLED_APPS`` list.
-        
-        ::
-        
-            INSTALLED_APPS = [
-                # ...
-                'memcache_status',
-            ]
-        
-        Then you have two options:
-        
-        1) The quickest way is to replace your Django Admin index page with the one
-           provided by django-memcache-status. This will show the memcache stats in the
-           top left column. This was the regular behavior of django-memcache-status
-           prior to version 2.0.
-        
-           Place this in any ``admin.py`` file of your project::
-        
-            from django.contrib import admin
-            admin.site.index_template = 'memcache_status/admin_index.html'
-        
-        
-        2) If you need to manually place the stats, simply add the CSS file and include
-           the memcache-status template anywhere you like::
-        
-            <link rel="stylesheet" href="{% static "memcache_status.css" %}"/>
-            {% include "memcache_status/memcache_status.html" %}
-        
-        
-        Local Development
-        =================
-        
-        Install the package using Pipenv and run the tests::
-        
-            $ pipenv install --dev
-            $ pipenv run test
-        
-        You can test against a matrix of Python and Django versions using tox::
-        
-            $ tox
-        
-        Once run you will see a coverage report in `/tmp/coverage_report/django-memcache-status`.
-        
-        You can run a local runserver with the test application to see the
-        admin::
-        
-            $ pipenv run django-admin.py migrate
-            $ pipenv run django-admin.py createsuperuser
-            $ pipenv run django-admin.py runserver
-        
-        To test a specific cache backend define it in the env variable::
-        
-            $ TEST_CACHE_BACKEND=django-pylibmc pipenv run django-admin.py runserver
-        
-        
-        .. note:: If you're testing pylibmc on OS X and you get an error like
-            ``'libmemcached/memcached.h' file not found``, install pylibmc manually,
-            then run the installation again::
-        
-            $ brew install libmemcached
-            $ pipenv run pip install pylibmc --install-option="--with-libmemcached=/usr/local/Cellar/libmemcached/1.0.18_2/"
-            $ pipenv install --dev
-        
-        ----
-        
-        Changelog
-        =========
-        
-        **v2.2 (2020-02-05):**
-        
-        - Compatibility and tests for Django 2.2 and 3.0, and Python 3.8.
-        - Use pytest for testing. 
-        
-        **v2.1 (2019-03-21):**
-        
-        - Removed some deprecated django-debug-toolbar and pre-Django 1.11
-          related workarounds.
-        - More comprehensive unittests across all backends and it's relation
-          with django-debug-toolbar.
-        
-        **v2.0 (2019-03-16):**
-        
-        - Compatibility and tests for Django 1.11 → 2.1 and Python 2.7 → 3.7.
-        - Full code cleanup and update to latest standards.
-        - Tested against a variety of memcache bindings.
-        - Pipenv support for local development and testing.
-        - *[Backwards Incompatible]* memcache-status no longer automatically overwrites
-          the admin index template to add the stats. Instead you have the option to
-          either  manually display the stats anywhere you like using a template include,
-          or use the contributed memcache-status admin index page that overwrites the
-          vanilla Django template and adds statistics to the top left admin index page.
-          This was the regular behavior of django-memcache-status prior to version 2.0.
-        
-        **v1.3 (2016-10-13):**
-        
-        - Django 1.10 compatibility and test integration. Python 3 compatibility.
-        
-        **v1.2 (2009-11-06):**
-        
-        - Unittests, General code cleanup to support Django 1.8+ features such as
-        - AppConfig, Django-Debugtoolbar support, Python3 Support, Compatibility tests
-        - with latest supported Django versions (currently Django 1.8 and 1.9) but the
-        - package is likely working with Django 1.4+.
-        
-        **v1.1 (2009-06-29):**
-        
-        - Added support for Django's multiple cache backend setting. Kudos to Luke
-          Granger-Brown for the implementation.
-        - This version is compatible with Django v1.3 and up.
-        
-        **v1.0 (2009-04-30):**
-        
-        - Initial Release.
-        - This version is compatible up to Django v1.2.
-        
-        ----
-        
-        Screenshots
-        ===========
-        
-        .. image:: https://user-images.githubusercontent.com/1896/54476030-f0dd3080-47f8-11e9-8399-b11f3bf15ebc.png
-           :target: https://user-images.githubusercontent.com/1896/54476030-f0dd3080-47f8-11e9-8399-b11f3bf15ebc.png
-           :align: left
-           :height: 200px
-        
-        .. image:: https://user-images.githubusercontent.com/1896/54476031-f470b780-47f8-11e9-842f-95d880563a53.png
-           :target: https://user-images.githubusercontent.com/1896/54476031-f470b780-47f8-11e9-842f-95d880563a53.png
-           :height: 300px
 Keywords: django,cache,memcache,memcached,statistics
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Requires-Python: >=2.7
+Requires-Python: >=3.8
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/v/django-memcache-status.svg
+    :target: https://pypi.org/project/django-memcache-status/
+
+-----
+
+======================
+django-memcache-status
+======================
+
+This app displays the current load and some statistics for your memcached_
+instances in the index view of your Django admin section.
+
+Currently these memcached bindings are tested:
+
+========================================================= ================================
+Backend                                                   Support
+========================================================= ================================
+``django.core.cache.backends.memcached.PyLibMCCache``      ✅ Works fine
+``django.core.cache.backends.memcached.PyMemcacheCache``   ❎ Does not provide stats
+========================================================= ================================
+
+Other bindings may provide statistics too.
+
+.. _memcached: http://www.danga.com/memcached/
+
+Compatibility Matrix:
+=====================
+
+========= === === ==== ====
+Py/Dj     3.8 3.9 3.10 3.11
+========= === === ==== ====
+3.2 (LTS)  ✓   ✓   ✓    ✓
+4.0        ✓   ✓   ✓    ✓
+4.1        ✓   ✓   ✓    ✓
+4.2 (LTS)  ✓   ✓   ✓    ✓
+========= === === ==== ====
+
+
+Installation
+============
+
+First add ``memcache_status`` to your ``INSTALLED_APPS`` list.
+
+::
+
+    INSTALLED_APPS = [
+        # ...
+        'memcache_status',
+    ]
+
+Then you have two options:
+
+1) The quickest way is to replace your Django Admin index page with the one
+   provided by django-memcache-status. This will show the memcache stats in the
+   top left column. This was the regular behavior of django-memcache-status
+   prior to version 2.0.
+
+   Place this in any ``admin.py`` file of your project::
+
+    from django.contrib import admin
+    admin.site.index_template = 'memcache_status/admin_index.html'
+
+
+2) If you need to manually place the stats, simply add the CSS file and include
+   the memcache-status template anywhere you like::
+
+    <link rel="stylesheet" href="{% static "memcache_status.css" %}"/>
+    {% include "memcache_status/memcache_status.html" %}
+
+
+Local Development
+=================
+
+Install the package using Pipenv and run the tests::
+
+    $ pipenv install --dev
+    $ pipenv run test
+
+You can test against a matrix of Python and Django versions using tox::
+
+    $ tox
+
+Once run you will see a coverage report in `/tmp/coverage_report/django-memcache-status`.
+
+You can run a local runserver with the test application to see the
+admin::
+
+    $ pipenv run django-admin.py migrate
+    $ pipenv run django-admin.py createsuperuser
+    $ pipenv run django-admin.py runserver
+
+To test a specific cache backend define it in the env variable::
+
+    $ TEST_CACHE_BACKEND=django-pylibmc pipenv run django-admin.py runserver
+
+
+.. note:: If you're testing pylibmc on OS X and you get an error like
+    ``'libmemcached/memcached.h' file not found``, install pylibmc manually,
+    then run the installation again::
+
+    $ brew install libmemcached
+    $ pipenv run pip install pylibmc --install-option="--with-libmemcached=/usr/local/Cellar/libmemcached/1.0.18_2/"
+    $ pipenv install --dev
+
+----
+
+Changelog
+=========
+
+**v2.3 (2023-04-30):**
+
+- Compatibility and tests for Django 3.2 to 4.2, and Python 3.11.
+- Dropped support for Django 2.2.
+
+**v2.2 (2020-02-05):**
+
+- Compatibility and tests for Django 2.2 and 3.0, and Python 3.8.
+- Use pytest for testing.
+
+**v2.1 (2019-03-21):**
+
+- Removed some deprecated django-debug-toolbar and pre-Django 1.11
+  related workarounds.
+- More comprehensive unittests across all backends and it's relation
+  with django-debug-toolbar.
+
+**v2.0 (2019-03-16):**
+
+- Compatibility and tests for Django 1.11 → 2.1 and Python 2.7 → 3.7.
+- Full code cleanup and update to latest standards.
+- Tested against a variety of memcache bindings.
+- Pipenv support for local development and testing.
+- *[Backwards Incompatible]* memcache-status no longer automatically overwrites
+  the admin index template to add the stats. Instead you have the option to
+  either  manually display the stats anywhere you like using a template include,
+  or use the contributed memcache-status admin index page that overwrites the
+  vanilla Django template and adds statistics to the top left admin index page.
+  This was the regular behavior of django-memcache-status prior to version 2.0.
+
+**v1.3 (2016-10-13):**
+
+- Django 1.10 compatibility and test integration. Python 3 compatibility.
+
+**v1.2 (2009-11-06):**
+
+- Unittests, General code cleanup to support Django 1.8+ features such as
+- AppConfig, Django-Debugtoolbar support, Python3 Support, Compatibility tests
+- with latest supported Django versions (currently Django 1.8 and 1.9) but the
+- package is likely working with Django 1.4+.
+
+**v1.1 (2009-06-29):**
+
+- Added support for Django's multiple cache backend setting. Kudos to Luke
+  Granger-Brown for the implementation.
+- This version is compatible with Django v1.3 and up.
+
+**v1.0 (2009-04-30):**
+
+- Initial Release.
+- This version is compatible up to Django v1.2.
+
+----
+
+Screenshots
+===========
+
+.. image:: https://user-images.githubusercontent.com/1896/54476030-f0dd3080-47f8-11e9-8399-b11f3bf15ebc.png
+   :target: https://user-images.githubusercontent.com/1896/54476030-f0dd3080-47f8-11e9-8399-b11f3bf15ebc.png
+   :align: left
+   :height: 200px
+
+.. image:: https://user-images.githubusercontent.com/1896/54476031-f470b780-47f8-11e9-842f-95d880563a53.png
+   :target: https://user-images.githubusercontent.com/1896/54476031-f470b780-47f8-11e9-842f-95d880563a53.png
+   :height: 300px
```

### Comparing `django-memcache-status-2.2/LICENSE` & `django-memcache-status-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-memcache-status-2.2/django_memcache_status.egg-info/PKG-INFO` & `django-memcache-status-2.3/django_memcache_status.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,192 +1,197 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: django-memcache-status
-Version: 2.2
-Summary: A django application that displays the load and other statistics about your memcached instances in the admin.
+Version: 2.3
+Summary: "A django application that displays the load and other statistics about your memcached instances in the admin."
 Home-page: https://github.com/bartTC/django-memcache-status
 Author: Martin Mahner
 Author-email: martin@mahner.org
 License: MIT
-Description: .. image:: https://img.shields.io/pypi/v/django-memcache-status.svg
-            :target: https://pypi.org/project/django-memcache-status/
-        
-        .. image:: https://travis-ci.org/bartTC/django-memcache-status.svg?branch=master
-            :target: https://travis-ci.org/bartTC/django-memcache-status
-        
-        .. image:: https://api.codacy.com/project/badge/Coverage/1d7d0306c4d14fb9817017d7d23237fe
-            :target: https://www.codacy.com/app/bartTC/django-memcache-status
-        
-        .. image:: https://api.codacy.com/project/badge/Grade/1d7d0306c4d14fb9817017d7d23237fe
-            :target: https://www.codacy.com/app/bartTC/django-memcache-status
-        
-        -----
-        
-        ======================
-        django-memcache-status
-        ======================
-        
-        This app displays the current load and some statistics for your memcached_
-        instances in the index view of your Django admin section.
-        
-        Currently these memcached bindings are tested:
-        
-        ========================================================= ================================
-        Backend                                                   Support
-        ========================================================= ================================
-        `python-memcached`_ with vanilla Django                   ✅ Works fine with >= v1.57
-        pylibmc with `django-pylibmc`_                            ✅ Works fine
-        pymemcache with `django-pymemcache`_                      ❎ Does not provide stats
-        ========================================================= ================================
-        
-        Other bindings may provide statistics too.
-        
-        .. _memcached: http://www.danga.com/memcached/
-        .. _python-memcached: https://pypi.org/project/python-memcached/
-        .. _django-pylibmc: https://pypi.org/project/django-pylibmc/
-        .. _django-pymemcache: https://pypi.org/project/django-pymemcache/
-        
-        Installation
-        ============
-        
-        First add ``memcache_status`` to your ``INSTALLED_APPS`` list.
-        
-        ::
-        
-            INSTALLED_APPS = [
-                # ...
-                'memcache_status',
-            ]
-        
-        Then you have two options:
-        
-        1) The quickest way is to replace your Django Admin index page with the one
-           provided by django-memcache-status. This will show the memcache stats in the
-           top left column. This was the regular behavior of django-memcache-status
-           prior to version 2.0.
-        
-           Place this in any ``admin.py`` file of your project::
-        
-            from django.contrib import admin
-            admin.site.index_template = 'memcache_status/admin_index.html'
-        
-        
-        2) If you need to manually place the stats, simply add the CSS file and include
-           the memcache-status template anywhere you like::
-        
-            <link rel="stylesheet" href="{% static "memcache_status.css" %}"/>
-            {% include "memcache_status/memcache_status.html" %}
-        
-        
-        Local Development
-        =================
-        
-        Install the package using Pipenv and run the tests::
-        
-            $ pipenv install --dev
-            $ pipenv run test
-        
-        You can test against a matrix of Python and Django versions using tox::
-        
-            $ tox
-        
-        Once run you will see a coverage report in `/tmp/coverage_report/django-memcache-status`.
-        
-        You can run a local runserver with the test application to see the
-        admin::
-        
-            $ pipenv run django-admin.py migrate
-            $ pipenv run django-admin.py createsuperuser
-            $ pipenv run django-admin.py runserver
-        
-        To test a specific cache backend define it in the env variable::
-        
-            $ TEST_CACHE_BACKEND=django-pylibmc pipenv run django-admin.py runserver
-        
-        
-        .. note:: If you're testing pylibmc on OS X and you get an error like
-            ``'libmemcached/memcached.h' file not found``, install pylibmc manually,
-            then run the installation again::
-        
-            $ brew install libmemcached
-            $ pipenv run pip install pylibmc --install-option="--with-libmemcached=/usr/local/Cellar/libmemcached/1.0.18_2/"
-            $ pipenv install --dev
-        
-        ----
-        
-        Changelog
-        =========
-        
-        **v2.2 (2020-02-05):**
-        
-        - Compatibility and tests for Django 2.2 and 3.0, and Python 3.8.
-        - Use pytest for testing. 
-        
-        **v2.1 (2019-03-21):**
-        
-        - Removed some deprecated django-debug-toolbar and pre-Django 1.11
-          related workarounds.
-        - More comprehensive unittests across all backends and it's relation
-          with django-debug-toolbar.
-        
-        **v2.0 (2019-03-16):**
-        
-        - Compatibility and tests for Django 1.11 → 2.1 and Python 2.7 → 3.7.
-        - Full code cleanup and update to latest standards.
-        - Tested against a variety of memcache bindings.
-        - Pipenv support for local development and testing.
-        - *[Backwards Incompatible]* memcache-status no longer automatically overwrites
-          the admin index template to add the stats. Instead you have the option to
-          either  manually display the stats anywhere you like using a template include,
-          or use the contributed memcache-status admin index page that overwrites the
-          vanilla Django template and adds statistics to the top left admin index page.
-          This was the regular behavior of django-memcache-status prior to version 2.0.
-        
-        **v1.3 (2016-10-13):**
-        
-        - Django 1.10 compatibility and test integration. Python 3 compatibility.
-        
-        **v1.2 (2009-11-06):**
-        
-        - Unittests, General code cleanup to support Django 1.8+ features such as
-        - AppConfig, Django-Debugtoolbar support, Python3 Support, Compatibility tests
-        - with latest supported Django versions (currently Django 1.8 and 1.9) but the
-        - package is likely working with Django 1.4+.
-        
-        **v1.1 (2009-06-29):**
-        
-        - Added support for Django's multiple cache backend setting. Kudos to Luke
-          Granger-Brown for the implementation.
-        - This version is compatible with Django v1.3 and up.
-        
-        **v1.0 (2009-04-30):**
-        
-        - Initial Release.
-        - This version is compatible up to Django v1.2.
-        
-        ----
-        
-        Screenshots
-        ===========
-        
-        .. image:: https://user-images.githubusercontent.com/1896/54476030-f0dd3080-47f8-11e9-8399-b11f3bf15ebc.png
-           :target: https://user-images.githubusercontent.com/1896/54476030-f0dd3080-47f8-11e9-8399-b11f3bf15ebc.png
-           :align: left
-           :height: 200px
-        
-        .. image:: https://user-images.githubusercontent.com/1896/54476031-f470b780-47f8-11e9-842f-95d880563a53.png
-           :target: https://user-images.githubusercontent.com/1896/54476031-f470b780-47f8-11e9-842f-95d880563a53.png
-           :height: 300px
 Keywords: django,cache,memcache,memcached,statistics
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Requires-Python: >=2.7
+Requires-Python: >=3.8
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/v/django-memcache-status.svg
+    :target: https://pypi.org/project/django-memcache-status/
+
+-----
+
+======================
+django-memcache-status
+======================
+
+This app displays the current load and some statistics for your memcached_
+instances in the index view of your Django admin section.
+
+Currently these memcached bindings are tested:
+
+========================================================= ================================
+Backend                                                   Support
+========================================================= ================================
+``django.core.cache.backends.memcached.PyLibMCCache``      ✅ Works fine
+``django.core.cache.backends.memcached.PyMemcacheCache``   ❎ Does not provide stats
+========================================================= ================================
+
+Other bindings may provide statistics too.
+
+.. _memcached: http://www.danga.com/memcached/
+
+Compatibility Matrix:
+=====================
+
+========= === === ==== ====
+Py/Dj     3.8 3.9 3.10 3.11
+========= === === ==== ====
+3.2 (LTS)  ✓   ✓   ✓    ✓
+4.0        ✓   ✓   ✓    ✓
+4.1        ✓   ✓   ✓    ✓
+4.2 (LTS)  ✓   ✓   ✓    ✓
+========= === === ==== ====
+
+
+Installation
+============
+
+First add ``memcache_status`` to your ``INSTALLED_APPS`` list.
+
+::
+
+    INSTALLED_APPS = [
+        # ...
+        'memcache_status',
+    ]
+
+Then you have two options:
+
+1) The quickest way is to replace your Django Admin index page with the one
+   provided by django-memcache-status. This will show the memcache stats in the
+   top left column. This was the regular behavior of django-memcache-status
+   prior to version 2.0.
+
+   Place this in any ``admin.py`` file of your project::
+
+    from django.contrib import admin
+    admin.site.index_template = 'memcache_status/admin_index.html'
+
+
+2) If you need to manually place the stats, simply add the CSS file and include
+   the memcache-status template anywhere you like::
+
+    <link rel="stylesheet" href="{% static "memcache_status.css" %}"/>
+    {% include "memcache_status/memcache_status.html" %}
+
+
+Local Development
+=================
+
+Install the package using Pipenv and run the tests::
+
+    $ pipenv install --dev
+    $ pipenv run test
+
+You can test against a matrix of Python and Django versions using tox::
+
+    $ tox
+
+Once run you will see a coverage report in `/tmp/coverage_report/django-memcache-status`.
+
+You can run a local runserver with the test application to see the
+admin::
+
+    $ pipenv run django-admin.py migrate
+    $ pipenv run django-admin.py createsuperuser
+    $ pipenv run django-admin.py runserver
+
+To test a specific cache backend define it in the env variable::
+
+    $ TEST_CACHE_BACKEND=django-pylibmc pipenv run django-admin.py runserver
+
+
+.. note:: If you're testing pylibmc on OS X and you get an error like
+    ``'libmemcached/memcached.h' file not found``, install pylibmc manually,
+    then run the installation again::
+
+    $ brew install libmemcached
+    $ pipenv run pip install pylibmc --install-option="--with-libmemcached=/usr/local/Cellar/libmemcached/1.0.18_2/"
+    $ pipenv install --dev
+
+----
+
+Changelog
+=========
+
+**v2.3 (2023-04-30):**
+
+- Compatibility and tests for Django 3.2 to 4.2, and Python 3.11.
+- Dropped support for Django 2.2.
+
+**v2.2 (2020-02-05):**
+
+- Compatibility and tests for Django 2.2 and 3.0, and Python 3.8.
+- Use pytest for testing.
+
+**v2.1 (2019-03-21):**
+
+- Removed some deprecated django-debug-toolbar and pre-Django 1.11
+  related workarounds.
+- More comprehensive unittests across all backends and it's relation
+  with django-debug-toolbar.
+
+**v2.0 (2019-03-16):**
+
+- Compatibility and tests for Django 1.11 → 2.1 and Python 2.7 → 3.7.
+- Full code cleanup and update to latest standards.
+- Tested against a variety of memcache bindings.
+- Pipenv support for local development and testing.
+- *[Backwards Incompatible]* memcache-status no longer automatically overwrites
+  the admin index template to add the stats. Instead you have the option to
+  either  manually display the stats anywhere you like using a template include,
+  or use the contributed memcache-status admin index page that overwrites the
+  vanilla Django template and adds statistics to the top left admin index page.
+  This was the regular behavior of django-memcache-status prior to version 2.0.
+
+**v1.3 (2016-10-13):**
+
+- Django 1.10 compatibility and test integration. Python 3 compatibility.
+
+**v1.2 (2009-11-06):**
+
+- Unittests, General code cleanup to support Django 1.8+ features such as
+- AppConfig, Django-Debugtoolbar support, Python3 Support, Compatibility tests
+- with latest supported Django versions (currently Django 1.8 and 1.9) but the
+- package is likely working with Django 1.4+.
+
+**v1.1 (2009-06-29):**
+
+- Added support for Django's multiple cache backend setting. Kudos to Luke
+  Granger-Brown for the implementation.
+- This version is compatible with Django v1.3 and up.
+
+**v1.0 (2009-04-30):**
+
+- Initial Release.
+- This version is compatible up to Django v1.2.
+
+----
+
+Screenshots
+===========
+
+.. image:: https://user-images.githubusercontent.com/1896/54476030-f0dd3080-47f8-11e9-8399-b11f3bf15ebc.png
+   :target: https://user-images.githubusercontent.com/1896/54476030-f0dd3080-47f8-11e9-8399-b11f3bf15ebc.png
+   :align: left
+   :height: 200px
+
+.. image:: https://user-images.githubusercontent.com/1896/54476031-f470b780-47f8-11e9-842f-95d880563a53.png
+   :target: https://user-images.githubusercontent.com/1896/54476031-f470b780-47f8-11e9-842f-95d880563a53.png
+   :height: 300px
```

### Comparing `django-memcache-status-2.2/django_memcache_status.egg-info/SOURCES.txt` & `django-memcache-status-2.3/django_memcache_status.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 Pipfile
 Pipfile.lock
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 django_memcache_status.egg-info/PKG-INFO
 django_memcache_status.egg-info/SOURCES.txt
 django_memcache_status.egg-info/dependency_links.txt
 django_memcache_status.egg-info/not-zip-safe
```

### Comparing `django-memcache-status-2.2/memcache_status/templatetags/memcache_status_tags.py` & `django-memcache-status-2.3/memcache_status/templatetags/memcache_status_tags.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,86 +1,90 @@
-from __future__ import unicode_literals
+from __future__ import annotations
 
 import logging
 from datetime import datetime
 
 from django import template
 from django.apps import apps
+from django.template import Context
 
 from memcache_status.utils import get_cache_stats
 
 logger = logging.getLogger(__name__)
 register = template.Library()
 
 
 @register.simple_tag(takes_context=True)
-def memcache_status(context):
+def memcache_status(context: Context) -> list:
     request = context.request
-    config = apps.get_app_config('memcache_status')
+    config = apps.get_app_config("memcache_status")
 
     if not config.show_cache_stats(request):
-        logger.debug('Cache stats not shown because user has no permission.')
+        logger.debug("Cache stats not shown because user has no permission.")
         return []
 
     return get_cache_stats()
 
 
-class PrettyValue(object):
+class PrettyValue:
     """
     Helper class that reformats the value. Looks for a method named
     ``format_<key>_value`` and returns that value. Returns the value
     as is, if no format method is found.
     """
-
-    def format(self, key, value):
+    def decode(self, value: bytes | str) -> str:
         try:
-            func = getattr(self, 'format_%s_value' % key.lower())
-            return func(value)
+            return value.decode()
         except AttributeError:
-            return value
+            return str(value)
+
+    def format(self, key: str, value: bytes) -> str:
+        if hasattr(self, f"format_{key.lower()}_value"):
+            return getattr(self, f"format_{key.lower()}_value")(value)
+        return self.decode(value)
 
-    def format_limit_maxbytes_value(self, value):
-        return "%s (%s)" % (value, self.human_bytes(value))
+    def format_limit_maxbytes_value(self, value: bytes) -> str:
+        return f"{self.decode(value)} ({self.human_bytes(value)})"
 
-    def format_bytes_read_value(self, value):
-        return "%s (%s)" % (value, self.human_bytes(value))
+    def format_bytes_read_value(self, value:bytes)->str:
+        return f"{self.decode(value)} ({self.human_bytes(value)})"
 
-    def format_bytes_written_value(self, value):
-        return "%s (%s)" % (value, self.human_bytes(value))
+    def format_bytes_written_value(self, value:bytes)->str:
+        return f"{self.decode(value)} ({self.human_bytes(value)})"
 
-    def format_uptime_value(self, value):
+    def format_uptime_value(self, value:str)->str:
         return self.fract_timestamp(int(value))
 
-    def format_time_value(self, value):
-        return datetime.fromtimestamp(int(value)).strftime('%x %X')
+    def format_time_value(self, value:str) ->str:
+        return datetime.fromtimestamp(int(value)).strftime("%x %X")
 
-    def fract_timestamp(self, s):
+    def fract_timestamp(self, s:int) -> str:
         years, s = divmod(s, 31556952)
         min_, s = divmod(s, 60)
         h, min_ = divmod(min_, 60)
         d, h = divmod(h, 24)
-        return '%sy, %sd, %sh, %sm, %ss' % (years, d, h, min_, s)
+        return f"{years}y, {d}d, {h}h, {min_}m, {s}s"
 
-    def human_bytes(self, bytes_):
+    def human_bytes(self, bytes_:bytes) -> str:
         bytes_ = float(bytes_)
         if bytes_ >= 1073741824:
             gigabytes_ = bytes_ / 1073741824
-            size = '%.2fGB' % gigabytes_
+            size = "%.2fGB" % gigabytes_
         elif bytes_ >= 1048576:
             megabytes_ = bytes_ / 1048576
-            size = '%.2fMB' % megabytes_
+            size = "%.2fMB" % megabytes_
         elif bytes_ >= 1024:
             kilobytes_ = bytes_ / 1024
-            size = '%.2fKB' % kilobytes_
+            size = "%.2fKB" % kilobytes_
         else:
-            size = '%.2fB' % bytes_
+            size = "%.2fB" % bytes_
         return size
 
 
 @register.filter
-def memcache_status_pretty_name(name):
-    return ' '.join([word.capitalize() for word in name.split('_')])
+def memcache_status_pretty_name(name: str) -> str:
+    return " ".join([word.capitalize() for word in name.split("_")])
 
 
 @register.filter
-def  memcache_status_pretty_value(value, key):
+def memcache_status_pretty_value(value: str, key: str) -> str:
     return PrettyValue().format(key, value)
```

### Comparing `django-memcache-status-2.2/memcache_status/tests/testapp/apps.py` & `django-memcache-status-2.3/memcache_status/tests/testapp/apps.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,45 @@
-from __future__ import unicode_literals
+from __future__ import annotations
 
 from django.apps import AppConfig
 
 lorem = """
-Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod 
-tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At 
-vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, 
-no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit 
-amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut 
-labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam 
-et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata 
+Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod
+tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At
+vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren,
+no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit
+amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut
+labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam
+et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata
 sanctus est Lorem ipsum dolor sit amet.
 """
 
 
 class MemcacheStatusTestAppConfig(AppConfig):
-    name = 'memcache_status.tests.testapp'
+    name = "memcache_status.tests.testapp"
     verbose_name = "MemcacheStatus Testapp"
 
-    def ready(self):
+    def ready(self) -> None:
         """
         Add some arbitraty data to the cache to have _some_ statistics.
         """
         from django.contrib import admin
-        admin.site.index_template = 'memcache_status/admin_index.html'
+
+        admin.site.index_template = "memcache_status/admin_index.html"
 
         from django.core.cache import cache
 
         # Set 100 items. Generate 200 GET Hits. Generate 50 DELETE hits.
         for i in range(1, 100):
-            key = 'TEST_VALUE_{0}'.format(i)
+            key = f"TEST_VALUE_{i}"
             cache.set(key, lorem)
             cache.get(key)
             cache.get(key)
             if i % 2 == 0:
                 cache.delete(key)
 
         # Generate 100 GET misses and 50 DELETE misses.
         for i in range(100, 200):
-            key = 'TEST_VALUE_{0}'.format(i)
+            key = f"TEST_VALUE_{i}"
             cache.get(key)
             if i % 2 == 0:
                 cache.delete(key)
-
-
-
-
```

### Comparing `django-memcache-status-2.2/memcache_status/tests/testapp/settings.py` & `django-memcache-status-2.3/memcache_status/tests/testapp/settings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,111 +1,102 @@
 import os
+import pathlib
 import sys
 
 DEBUG = True
 
-TESTAPP_DIR = os.path.abspath(os.path.dirname(__file__))
+TESTAPP_DIR = pathlib.Path(__file__).parent.resolve()
 
-SECRET_KEY = 'testsecretkey'
+SECRET_KEY = "testsecretkey"  # noqa: S105 Possible hardcoded password
 
-ALLOWED_HOSTS = ['*']
+ALLOWED_HOSTS = ["*"]
 
-EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
+USE_TZ = True
+
+EMAIL_BACKEND = "django.core.mail.backends.console.EmailBackend"
 
 DATABASES = {
-    'default': {
-        'ENGINE': 'django.db.backends.sqlite3',
-        'NAME': os.path.join(TESTAPP_DIR, 'testdb.sqlite'),
-    }
+    "default": {
+        "ENGINE": "django.db.backends.sqlite3",
+        "NAME": TESTAPP_DIR / "testdb.sqlite",
+    },
 }
 
 # Cache backends to test based on ENV variabe below.
 CACHE_BACKENDS_TO_TEST = {
-    'python-memcached': {
-        'BACKEND': 'django.core.cache.backends.memcached.MemcachedCache',
-        'LOCATION': '127.0.0.1:11211',
-
+    "django-pylibmc": {
+        "BACKEND": "django.core.cache.backends.memcached.PyLibMCCache",
+        "LOCATION": "127.0.0.1:11211",
         # Flag only used for the unittests. It indicates whether its expected
         # that this backend provides stats or not.
-        'TEST_PROVIDES_STATS': True,
+        "TEST_PROVIDES_STATS": True,
     },
-
-    'django-pylibmc': {
-        'BACKEND': 'django.core.cache.backends.memcached.PyLibMCCache',
-        'LOCATION': '127.0.0.1:11211',
-
+    "django-pymemcache": {
+        "BACKEND": "django.core.cache.backends.memcached.PyMemcacheCache",
+        "LOCATION": "127.0.0.1:11211",
         # Flag only used for the unittests. It indicates whether its expected
         # that this backend provides stats or not.
-        'TEST_PROVIDES_STATS': True,
-    },
-
-    'django-pymemcache': {
-        'BACKEND': 'djpymemcache.backend.PyMemcacheCache',
-        'LOCATION': '127.0.0.1:11211',
-
-        # Flag only used for the unittests. It indicates whether its expected
-        # that this backend provides stats or not.
-        'TEST_PROVIDES_STATS': False,
+        "TEST_PROVIDES_STATS": False,
     },
 }
 
-CACHE_LABEL = os.environ.get('TEST_CACHE_BACKEND', 'python-memcached')
-if CACHE_LABEL not in CACHE_BACKENDS_TO_TEST:
-    sys.stderr.write('\nCache backend % is not defined in the settings\n' % CACHE_LABEL)
-    exit(1)
+CACHE_LABEL = os.environ.get("TEST_CACHE_BACKEND")
+if not CACHE_LABEL or CACHE_LABEL not in CACHE_BACKENDS_TO_TEST:
+    sys.stderr.write(f"\nCache backend '{CACHE_LABEL}' is not defined in the settings\n")
+    sys.exit(1)
 
 
-sys.stdout.write('Testing cache backend: %s\n' % CACHE_LABEL)
-CACHES = {'default': CACHE_BACKENDS_TO_TEST[CACHE_LABEL]}
+sys.stdout.write("Testing cache backend: %s\n" % CACHE_LABEL)
+CACHES = {"default": CACHE_BACKENDS_TO_TEST[CACHE_LABEL]}
 
 
-STATIC_ROOT = os.path.join(TESTAPP_DIR, '.static')
-MEDIA_ROOT = os.path.join(TESTAPP_DIR, '.uploads')
+STATIC_ROOT = TESTAPP_DIR / ".static"
+MEDIA_ROOT = TESTAPP_DIR / ".uploads"
 
-STATIC_URL = '/static/'
-MEDIA_URL = '/uploads/'
+STATIC_URL = "/static/"
+MEDIA_URL = "/uploads/"
 
-ROOT_URLCONF = 'memcache_status.tests.testapp.urls'
+ROOT_URLCONF = "memcache_status.tests.testapp.urls"
 
 INSTALLED_APPS = [
-    'memcache_status',
-    'memcache_status.tests.testapp',
-    'django.contrib.admin',
-    'django.contrib.auth',
-    'django.contrib.contenttypes',
-    'django.contrib.sessions',
-    'django.contrib.messages',
-    'django.contrib.staticfiles',
+    "memcache_status",
+    "memcache_status.tests.testapp",
+    "django.contrib.admin",
+    "django.contrib.auth",
+    "django.contrib.contenttypes",
+    "django.contrib.sessions",
+    "django.contrib.messages",
+    "django.contrib.staticfiles",
 ]
 
 MIDDLEWARE = [
-    'django.contrib.sessions.middleware.SessionMiddleware',
-    'django.contrib.auth.middleware.AuthenticationMiddleware',
-    'django.contrib.messages.middleware.MessageMiddleware',
+    "django.contrib.sessions.middleware.SessionMiddleware",
+    "django.contrib.auth.middleware.AuthenticationMiddleware",
+    "django.contrib.messages.middleware.MessageMiddleware",
 ]
 
 TEMPLATES = [
     {
-        'BACKEND': 'django.template.backends.django.DjangoTemplates',
-        'DIRS': [],
-        'APP_DIRS': True,
-        'OPTIONS': {
-            'context_processors': [
-                'django.template.context_processors.debug',
-                'django.template.context_processors.request',
-                'django.template.context_processors.i18n',
-                'django.contrib.auth.context_processors.auth',
-                'django.contrib.messages.context_processors.messages',
-            ]
+        "BACKEND": "django.template.backends.django.DjangoTemplates",
+        "DIRS": [],
+        "APP_DIRS": True,
+        "OPTIONS": {
+            "context_processors": [
+                "django.template.context_processors.debug",
+                "django.template.context_processors.request",
+                "django.template.context_processors.i18n",
+                "django.contrib.auth.context_processors.auth",
+                "django.contrib.messages.context_processors.messages",
+            ],
         },
-    }
+    },
 ]
 
-if os.getenv('TEST_WITH_DEBUGTOOLBAR', False) == 'on':
-    sys.stdout.write('Testing with django-debug-toolbar support.\n')
-    INSTALLED_APPS.insert(0, 'debug_toolbar')
-    MIDDLEWARE.append('debug_toolbar.middleware.DebugToolbarMiddleware')
+if os.getenv("TEST_WITH_DEBUGTOOLBAR", "off") == "on":
+    sys.stdout.write("Testing with django-debug-toolbar support.\n")
+    INSTALLED_APPS.insert(0, "debug_toolbar")
+    MIDDLEWARE.append("debug_toolbar.middleware.DebugToolbarMiddleware")
 
     # Make sure debug toolbar is always visible, even in Unittests.
     DEBUG_TOOLBAR_CONFIG = {
-        'SHOW_TOOLBAR_CALLBACK': lambda request: True
+        "SHOW_TOOLBAR_CALLBACK": lambda _: True,
     }
```

### Comparing `django-memcache-status-2.2/memcache_status/tests/tests.py` & `django-memcache-status-2.3/memcache_status/tests/tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,80 +1,89 @@
-from __future__ import unicode_literals
-
 import os
 
 from django.test import TestCase
 
 
 class MemcacheStatusSanityTests(TestCase):
-    def setUp(self):
+    def setUp(self) -> None:
         from django.contrib.auth.models import User
 
         self.user = User.objects.create_superuser(
-            'test', 'test@test.com', 'password'
+            "test",
+            "test@test.com",
+            "password",
+        )
+        self.client.login(
+            username=self.user.username,
+            password="password",  # noqa: S106 Possible hardcoded password
         )
-        self.client.login(username=self.user.username, password='password')
 
-    def test_admin_accessible(self):
+    def test_admin_accessible(self) -> None:
         """
         First simple check to make sure the /admin/ page is accessible at
         all and we don't hit any 500 error e.g. with the cache or
         with debug toolbar.
         """
-        response = self.client.get('/admin/')
+        response = self.client.get("/admin/")
         self.assertEqual(200, response.status_code)
 
-    def test_cache_stats_included(self):
+    def test_cache_stats_included(self) -> None:
         """
         Make sure that the memcache-status template is rendered within
         the admin index page. This makes sure that at least one cache
         backend provided stats and none of them fail.
         """
         # Not all backends we test do provide stats. In that case
         # memcache-status wont render at all, so we can skip the test.
         # The check whether the backend breaks or not is done above.
         from django.conf import settings
-        if settings.CACHES['default']['TEST_PROVIDES_STATS'] is False:
-            self.skipTest('cache backend does not provide stats')
 
-        response = self.client.get('/admin/')
+        if settings.CACHES["default"]["TEST_PROVIDES_STATS"] is False:
+            self.skipTest("cache backend does not provide stats")
+
+        response = self.client.get("/admin/")
         self.assertIn(
             '<div class="cache-stats">',
             str(response.content),
             '`div class="cache-stats"` tag not found in HTML',
         )
 
-    def test_debugtoolbar_visible(self):
+    def test_debugtoolbar_visible(self) -> None:
         """
         This checks that the debug toolbar is visible. We had some race
         conditions with the debug toolbar and it's cache panel in the past.
         """
-        if os.getenv('TEST_WITH_DEBUGTOOLBAR', False) != 'on':
-            self.skipTest('debug-toolbar is disabled, no need to test.')
+        if os.getenv("TEST_WITH_DEBUGTOOLBAR", "off") != "on":
+            self.skipTest("debug-toolbar is disabled, no need to test.")
 
-        response = self.client.get('/admin/')
+        response = self.client.get("/admin/")
         self.assertIn(
             'id="djDebug"',
             str(response.content),
             '`id="djDebug"` tag not found in HTML',
         )
 
 
 class MemcacheStatusPermissionsTests(TestCase):
-    def test_non_superuser_cant_see_stats(self):
+    def test_non_superuser_cant_see_stats(self) -> None:
         """
         Onlu users with is_superuser permission can see memcache stats
         by default.
         :return:
         """
         from django.contrib.auth.models import User
 
         self.user = User.objects.create_user(
-            'test', 'test@test.com', 'password'
+            "test",
+            "test@test.com",
+            "password",
+        )
+        self.client.login(
+            username=self.user.username,
+            password="password",  # noqa: S106 Possible hardcoded password
         )
-        self.client.login(username=self.user.username, password='password')
-        response = self.client.get('/admin/')
+        response = self.client.get("/admin/")
         self.assertNotIn(
             '<div class="cache-stats">',
             str(response.content),
             '`div class="cache-stats"` FOUND in HTML but should be forbidden',
         )
```

### Comparing `django-memcache-status-2.2/memcache_status/apps.py` & `django-memcache-status-2.3/memcache_status/apps.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from __future__ import unicode_literals
-
 from django.apps import AppConfig
+from django.http import HttpRequest
 
 
 class MemcacheStatusConfig(AppConfig):
-    name = 'memcache_status'
+    name = "memcache_status"
     verbose_name = "MemcacheStatus"
 
-    def show_cache_stats(self, request):
+    def show_cache_stats(self, request: HttpRequest) -> bool:
         """
         Memcache stats are only displayed to Users with `is_superuser`
         permission. You can overwrite this behavior using your custom
         AppConfig.
 
         :param request: Django View Request
         :return bool: Whether to show cache stats for the current request/user.
```

### Comparing `django-memcache-status-2.2/memcache_status/utils.py` & `django-memcache-status-2.3/memcache_status/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from __future__ import unicode_literals
-
 import logging
 
-import six
 from django.conf import settings
 from django.core.cache import caches
 
 logger = logging.getLogger(__name__)
 
 
-def get_cache_stats():
+def get_cache_stats() -> list:
     """
     Returns a list of dictionaries of all cache servers and their stats,
     if they provide stats.
     """
     cache_stats = []
-    for name, _ in six.iteritems(settings.CACHES):
+    for name, _ in settings.CACHES.items():
         cache_backend = caches[name]
 
         try:
             cache_backend_stats = cache_backend._cache.get_stats()
         except AttributeError:  # this backend doesn't provide stats
-            logger.info(
-                'The memcached backend "{0}" does not support or '
-                'provide stats.'.format(name)
-            )
-            continue
+            try:
+                cache_backend_stats = cache_backend._cache.stats()
+            except AttributeError:
+                logger.info(
+                    'The memcached backend "%s" does not support or provide stats.',
+                    name,
+                )
+                continue
 
         for address, stats in cache_backend_stats:
             cache_stats.append(
-                {'name': name, 'address': address, 'stats': stats}
+                {"name": name, "address": address, "stats": stats},
             )
     return cache_stats
```

### Comparing `django-memcache-status-2.2/memcache_status/static/memcache_status.css` & `django-memcache-status-2.3/memcache_status/static/memcache_status.css`

 * *Files identical despite different names*

### Comparing `django-memcache-status-2.2/memcache_status/templates/memcache_status/memcache_status.html` & `django-memcache-status-2.3/memcache_status/templates/memcache_status/memcache_status.html`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
       <table>
 
         <caption>
           <a href="#" class="section"
              data-for-panel="cache-panel-{{ forloop.counter }}">
             <strong>{{ server.name }}</strong>
             &mdash;
-            {{ server.address }}
+            {{ server.address.decode }}
             &mdash;
             {% widthratio server.stats.bytes server.stats.limit_maxbytes 100 %}%
             load</a>
         </caption>
 
         <thead>
         <tr>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 {% load memcache_status_tags %} {% load i18n %} {% memcache_status as
 memcache_status %} {% if memcache_status %}
 **** Memcache Status: ****
 {% for server in memcache_status %}
- {{_server.name_}}_—_{{_server.address_}}_—_{%_widthratio_server.stats.bytes
-                   server.stats.limit_maxbytes_100_%}%_load
+       {{_server.name_}}_—_{{_server.address.decode_}}_—_{%_widthratio
+         server.stats.bytes_server.stats.limit_maxbytes_100_%}%_load
 {% trans "Miss Ratio" %}              {% widthratio server.stats.get_misses
                                       server.stats.cmd_get 100 %}%
 {% trans "Avg GET by item" %}         {% widthratio server.stats.cmd_get
                                       server.stats.total_items 1 %}
                                       {% widthratio server.stats.cmd_get
 {% trans "Avg GET by seconds/minutes" server.stats.uptime 1 %}/{% widthratio
 %}                                    server.stats.cmd_get server.stats.uptime
```

### Comparing `django-memcache-status-2.2/README.rst` & `django-memcache-status-2.3/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 .. image:: https://img.shields.io/pypi/v/django-memcache-status.svg
     :target: https://pypi.org/project/django-memcache-status/
 
-.. image:: https://travis-ci.org/bartTC/django-memcache-status.svg?branch=master
-    :target: https://travis-ci.org/bartTC/django-memcache-status
-
-.. image:: https://api.codacy.com/project/badge/Coverage/1d7d0306c4d14fb9817017d7d23237fe
-    :target: https://www.codacy.com/app/bartTC/django-memcache-status
-
-.. image:: https://api.codacy.com/project/badge/Grade/1d7d0306c4d14fb9817017d7d23237fe
-    :target: https://www.codacy.com/app/bartTC/django-memcache-status
-
 -----
 
 ======================
 django-memcache-status
 ======================
 
 This app displays the current load and some statistics for your memcached_
 instances in the index view of your Django admin section.
 
 Currently these memcached bindings are tested:
 
 ========================================================= ================================
 Backend                                                   Support
 ========================================================= ================================
-`python-memcached`_ with vanilla Django                   ✅ Works fine with >= v1.57
-pylibmc with `django-pylibmc`_                            ✅ Works fine
-pymemcache with `django-pymemcache`_                      ❎ Does not provide stats
+``django.core.cache.backends.memcached.PyLibMCCache``      ✅ Works fine
+``django.core.cache.backends.memcached.PyMemcacheCache``   ❎ Does not provide stats
 ========================================================= ================================
 
 Other bindings may provide statistics too.
 
 .. _memcached: http://www.danga.com/memcached/
-.. _python-memcached: https://pypi.org/project/python-memcached/
-.. _django-pylibmc: https://pypi.org/project/django-pylibmc/
-.. _django-pymemcache: https://pypi.org/project/django-pymemcache/
+
+Compatibility Matrix:
+=====================
+
+========= === === ==== ====
+Py/Dj     3.8 3.9 3.10 3.11
+========= === === ==== ====
+3.2 (LTS)  ✓   ✓   ✓    ✓
+4.0        ✓   ✓   ✓    ✓
+4.1        ✓   ✓   ✓    ✓
+4.2 (LTS)  ✓   ✓   ✓    ✓
+========= === === ==== ====
+
 
 Installation
 ============
 
 First add ``memcache_status`` to your ``INSTALLED_APPS`` list.
 
 ::
@@ -103,18 +103,23 @@
     $ pipenv install --dev
 
 ----
 
 Changelog
 =========
 
+**v2.3 (2023-04-30):**
+
+- Compatibility and tests for Django 3.2 to 4.2, and Python 3.11.
+- Dropped support for Django 2.2.
+
 **v2.2 (2020-02-05):**
 
 - Compatibility and tests for Django 2.2 and 3.0, and Python 3.8.
-- Use pytest for testing. 
+- Use pytest for testing.
 
 **v2.1 (2019-03-21):**
 
 - Removed some deprecated django-debug-toolbar and pre-Django 1.11
   related workarounds.
 - More comprehensive unittests across all backends and it's relation
   with django-debug-toolbar.
```

### Comparing `django-memcache-status-2.2/Pipfile.lock` & `django-memcache-status-2.3/Pipfile.lock`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8323506289308176%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'6beaadcf38779078318c397bc7737816c553b5a7cec6ac35e254cfed41aec623'}}",*

 * * "'default'": "{'asgiref': {'hashes': "*

 * *              "['sha256:71e68008da809b957b7ee4b43dbccff33d1b23519fb8344e33f049897077afac', "*

 * *              "'sha256:9567dfe7bd8d3c8c892227827c41cce860b368104c3431da67a0c5a65a949506'], "*

 * *              '\'version\': \'==3.6.0\', \'markers\': "python_version >= \'3.7\'"}, \'django\': '*

 * *              "{'hashes': "*

 * *              "['sha256:ad33ed68db9398f5d […]*

```diff
@@ -1,44 +1,46 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "aabbe49654cfafceecbf53b49ad48b2372113c3230e3f49330aabcee97f5d131"
+            "sha256": "6beaadcf38779078318c397bc7737816c553b5a7cec6ac35e254cfed41aec623"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "asgiref": {
             "hashes": [
-                "sha256:7e06d934a7718bf3975acbf87780ba678957b87c7adc056f13b6215d610695a0",
-                "sha256:ea448f92fc35a0ef4b1508f53a04c4670255a3f33d22a81c8fc9c872036adbe5"
+                "sha256:71e68008da809b957b7ee4b43dbccff33d1b23519fb8344e33f049897077afac",
+                "sha256:9567dfe7bd8d3c8c892227827c41cce860b368104c3431da67a0c5a65a949506"
             ],
-            "version": "==3.2.3"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.6.0"
         },
         "django": {
             "hashes": [
-                "sha256:0a1efde1b685a6c30999ba00902f23613cf5db864c5a1532d2edf3eda7896a37",
-                "sha256:bd7e7dd0c3065e356f150fb03d1620e98e947d8c0ce913826d43bd468e020bed"
+                "sha256:ad33ed68db9398f5dfb33282704925bce044bef4261cd4fb59e4e7f9ae505a78",
+                "sha256:c36e2ab12824e2ac36afa8b2515a70c53c7742f0d6eaefa7311ec379558db997"
             ],
-            "version": "==3.0rc1"
+            "markers": "python_version >= '3.8'",
+            "version": "==4.2"
         },
         "django-debug-toolbar": {
             "hashes": [
-                "sha256:24c157bc6c0e1648e0a6587511ecb1b007a00a354ce716950bff2de12693e7a8",
-                "sha256:77cfba1d6e91b9bc3d36dc7dc74a9bb80be351948db5f880f2562a0cbf20b6c5"
+                "sha256:89619f6e0ea1057dca47bfc429ed99b237ef70074dabc065a7faa5f00e1459cf",
+                "sha256:bad339d68520652ddc1580c76f136fcbc3e020fd5ed96510a89a02ec81bb3fb1"
             ],
             "index": "pypi",
-            "version": "==2.1"
+            "version": "==4.0.0"
         },
         "django-memcache-status": {
             "editable": true,
             "path": "."
         },
         "django-pylibmc": {
             "hashes": [
@@ -46,425 +48,372 @@
                 "sha256:9cffdee703aaf9ebc029d9dbdee8abdd0723564b95e4b2ac59e4a668b8e58f93"
             ],
             "index": "pypi",
             "version": "==0.6.1"
         },
         "django-pymemcache": {
             "hashes": [
-                "sha256:9b520fb7ba7b0e3ddb418e91b4a3303e27beb92d1f3cdc9d0cc1e1285c52a59c",
-                "sha256:b8a41bee53809ac3df89c1dfc9eb9bc390b807367854912feac04691d428529d"
+                "sha256:53734eed5940350569f5cd90644dfe97755bb08f42c97d72bb149ab0c667dbdc",
+                "sha256:e2a9185dff1fc77c11c462f21cc4d8353683e354b85409639eaf77c9b373ffd8"
             ],
             "index": "pypi",
-            "version": "==0.2.0"
+            "version": "==1.0.0"
         },
         "pylibmc": {
             "hashes": [
-                "sha256:01a7e2e3fa9fcd7a791c7818a80a07e7a381aee988a5d810a1c1e6f7a9a288fd",
-                "sha256:6fff384e3c30af029bbac87f88b3fab14ae87b50103d389341d9b3e633349a3f",
-                "sha256:8a8dd406487d419d58c6d944efd91e8189b360a0c4d9e8c6ebe3990d646ae7e9",
-                "sha256:c749b4251c1137837d00542b62992b96cd2aed639877407f66291120dd6de2ff",
-                "sha256:e6c0c452336db0868d0de521d48872c2a359b1233b974c6b32c36ce68abc4820"
+                "sha256:218125aca214d62e6f69e4f8022bd795fbcb3643ad783f5f5ff33c23a1731c73",
+                "sha256:3c35816082848723455071670770d89b5a531d40e9063fe4e942ea456f86da49",
+                "sha256:4f46b5aa0364bca5e02000f5d62eb408d834a20722ffaf7dae20f75e7d009e6c",
+                "sha256:5251df82535411d8dc08c01141b8e6e61004f0a3ee50db3aa48ffa00e928cebb",
+                "sha256:7660c561e5415f4be01ff4791c1b035359c1d76fed012e18eee907c2d3249deb",
+                "sha256:7b93e381dec1520a3fec922765e04679ac553d2f3fda830a5faa7cdc527280a2",
+                "sha256:9d2ff6d702eb5ae502e29d97772dc85c749d596c6cb8c82a5d18f175fd4eabcc",
+                "sha256:9f4516a14b2beff6062d1d240c00098227ca5478c00afba7e8b329415b0d4d67",
+                "sha256:a6cce1d7705952eb30a3aca9ea3f054040cbee53c668d4e1e29144110da113bc",
+                "sha256:a7baf4b78720f8b72839b3642b374754cb77cf57dab465a70ed1764d943e19d5",
+                "sha256:b34c1e4021b9a395950be19ea9d98f02bea0e3a88be26dbaa7e8ac4416e1232b",
+                "sha256:b649eb7fdd774290b2da73334456eb01e0d66e3d3685acd88ae6bf456a227dc6",
+                "sha256:c6c4bdd8790aede67a464a32df842cacb562f77b0415a8c7823421f5c07524c6",
+                "sha256:cd61f1ff46aa1ca6b0b3dac17a727cd29ac019e85db868c5523c491eef4459d7",
+                "sha256:db8c0f0467182a2a3e8d625b5c60c296f971dd2ee179e865b0262bd44528d676",
+                "sha256:dd98054a571bd450200a61a12b9ada3424678d17a25456bbf9a6100470401e52",
+                "sha256:e589b7e70dec4daf0da1216789713c753d85611d70cfcd32574161cc75b1527e",
+                "sha256:e847cdc78d82964236599ff5b312bc97fde3d10f4b93c9ee17dc33b7cf3c032a",
+                "sha256:e9ef3dc70ee2dfd0981bdf3a383a044bc591de7e445296a64a24f10a560e8b4f",
+                "sha256:eefa46115537abad65fbe2e032acd1b3463d9bf9e335af4b0916df4e4d3206e0",
+                "sha256:f2574f390a2ec89b52a84bccca3ae57c21a4bb4d0e72df210d0d66783eee7f98",
+                "sha256:f2aeff000de7d918806876dfa4880d21b72089f9809ad0b8e7dff26501367ec6",
+                "sha256:f536d73632007358796654ab088d65c55a1a4368a85cfd7c956d2100e2cd8d89"
             ],
             "index": "pypi",
-            "version": "==1.6.1"
+            "version": "==1.6.3"
         },
         "pymemcache": {
             "hashes": [
-                "sha256:3b177743d2bc680a80e74835d080121f7338c35551fbc4cea9bcda9aa841d9f7",
-                "sha256:bb1fa46b5c6ed74d72586e2da4b58db96d0b0ff062b2c45e88d45be9be154801"
+                "sha256:27bf9bd1bbc1e20f83633208620d56de50f14185055e49504f4f5e94e94aff94",
+                "sha256:f507bc20e0dc8d562f8df9d872107a278df049fa496805c1431b926f3ddd0eab"
             ],
             "index": "pypi",
-            "version": "==2.2.2"
+            "version": "==4.0.0"
         },
         "python-memcached": {
             "hashes": [
                 "sha256:4dac64916871bd3550263323fc2ce18e1e439080a2d5670c594cf3118d99b594",
                 "sha256:a2e28637be13ee0bf1a8b6843e7490f9456fd3f2a4cb60471733c7b5d5557e4f"
             ],
             "index": "pypi",
             "version": "==1.59"
         },
-        "pytz": {
-            "hashes": [
-                "sha256:1c557d7d0e871de1f5ccd5833f60fb2550652da6be2693c1e02300743d21500d",
-                "sha256:b02c06db6cf09c12dd25137e563b31700d3b80fcc4ad23abb7a315f2789819be"
-            ],
-            "version": "==2019.3"
-        },
         "six": {
             "hashes": [
-                "sha256:1f1b7d42e254082a9db6279deae68afb421ceba6158efa6131de7b3003ee93fd",
-                "sha256:30f610279e8b2578cab6db20741130331735c781b56053c59c4076da27f06b66"
+                "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
+                "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
-            "version": "==1.13.0"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==1.16.0"
         },
         "sqlparse": {
             "hashes": [
-                "sha256:40afe6b8d4b1117e7dff5504d7a8ce07d9a1b15aeeade8a2d10f130a834f8177",
-                "sha256:7c3dca29c022744e95b547e867cee89f4fce4373f3549ccd8797d8eb52cdb873"
+                "sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3",
+                "sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c"
             ],
-            "version": "==0.3.0"
+            "markers": "python_version >= '3.5'",
+            "version": "==0.4.4"
         }
     },
     "develop": {
-        "appdirs": {
-            "hashes": [
-                "sha256:9e5896d1372858f8dd3344faf4e5014d21849c756c8d5701f78f8a103b372d92",
-                "sha256:d8b24664561d0d34ddfaec54636d502d7cea6e29c3eaf68f3df6180863e2166e"
-            ],
-            "version": "==1.4.3"
-        },
         "appnope": {
             "hashes": [
-                "sha256:5b26757dc6f79a3b7dc9fab95359328d5747fcb2409d331ea66d0272b90ab2a0",
-                "sha256:8b995ffe925347a2138d7ac0fe77155e4311a0ea6d6da4f5128fe4b3cbe5ed71"
+                "sha256:02bd91c4de869fbb1e1c50aafc4098827a7a54ab2f39d9dcba6c9547ed920e24",
+                "sha256:265a455292d0bd8a72453494fa24df5a11eb18373a60c7c0430889f22548605e"
             ],
             "markers": "sys_platform == 'darwin'",
-            "version": "==0.1.0"
+            "version": "==0.1.3"
         },
-        "attrs": {
+        "asttokens": {
             "hashes": [
-                "sha256:08a96c641c3a74e44eb59afb61a24f2cb9f4d7188748e76ba4bb5edfa3cb7d1c",
-                "sha256:f7b7ce16570fe9965acd6d30101a28f62fb4a7f9e926b3bbc9b61f8b04247e72"
+                "sha256:4622110b2a6f30b77e1473affaa97e711bc2f07d3f10848420ff1898edbe94f3",
+                "sha256:6b0ac9e93fb0335014d382b8fa9b3afa7df546984258005da0b9e7095b3deb1c"
             ],
-            "version": "==19.3.0"
+            "version": "==2.2.1"
         },
         "backcall": {
             "hashes": [
-                "sha256:38ecd85be2c1e78f77fd91700c76e14667dc21e2713b63876c0eb901196e01e4",
-                "sha256:bbbf4b1e5cd2bdb08f915895b51081c041bac22394fdfcfdfbe9f14b77c08bf2"
+                "sha256:5cbdbf27be5e7cfadb448baf0aa95508f91f2bbc6c6437cd9cd06e2a4c215e1e",
+                "sha256:fbbce6a29f263178a1f7915c1940bde0ec2b2a967566fe1c65c1dfb7422bd255"
             ],
-            "version": "==0.1.0"
+            "version": "==0.2.0"
         },
         "black": {
             "hashes": [
-                "sha256:1b30e59be925fafc1ee4565e5e08abef6b03fe455102883820fe5ee2e4734e0b",
-                "sha256:c2edb73a08e9e0e6f65a0e6af18b059b8b1cdd5bef997d7a0b181df93dc81539"
+                "sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5",
+                "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915",
+                "sha256:11c410f71b876f961d1de77b9699ad19f939094c3a677323f43d7a29855fe326",
+                "sha256:1c7b8d606e728a41ea1ccbd7264677e494e87cf630e399262ced92d4a8dac940",
+                "sha256:1d06691f1eb8de91cd1b322f21e3bfc9efe0c7ca1f0e1eb1db44ea367dff656b",
+                "sha256:3238f2aacf827d18d26db07524e44741233ae09a584273aa059066d644ca7b30",
+                "sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c",
+                "sha256:35d1381d7a22cc5b2be2f72c7dfdae4072a3336060635718cc7e1ede24221d6c",
+                "sha256:3a150542a204124ed00683f0db1f5cf1c2aaaa9cc3495b7a3b5976fb136090ab",
+                "sha256:48f9d345675bb7fbc3dd85821b12487e1b9a75242028adad0333ce36ed2a6d27",
+                "sha256:50cb33cac881766a5cd9913e10ff75b1e8eb71babf4c7104f2e9c52da1fb7de2",
+                "sha256:562bd3a70495facf56814293149e51aa1be9931567474993c7942ff7d3533961",
+                "sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9",
+                "sha256:6b39abdfb402002b8a7d030ccc85cf5afff64ee90fa4c5aebc531e3ad0175ddb",
+                "sha256:6f3c333ea1dd6771b2d3777482429864f8e258899f6ff05826c3a4fcc5ce3f70",
+                "sha256:714290490c18fb0126baa0fca0a54ee795f7502b44177e1ce7624ba1c00f2331",
+                "sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2",
+                "sha256:92c543f6854c28a3c7f39f4d9b7694f9a6eb9d3c5e2ece488c327b6e7ea9b266",
+                "sha256:a6f6886c9869d4daae2d1715ce34a19bbc4b95006d20ed785ca00fa03cba312d",
+                "sha256:a8a968125d0a6a404842fa1bf0b349a568634f856aa08ffaff40ae0dfa52e7c6",
+                "sha256:c7ab5790333c448903c4b721b59c0d80b11fe5e9803d8703e84dcb8da56fec1b",
+                "sha256:e114420bf26b90d4b9daa597351337762b63039752bdf72bf361364c1aa05925",
+                "sha256:e198cf27888ad6f4ff331ca1c48ffc038848ea9f031a3b40ba36aced7e22f2c8",
+                "sha256:ec751418022185b0c1bb7d7736e6933d40bbb14c14a0abcf9123d1b159f98dd4",
+                "sha256:f0bd2f4a58d6666500542b26354978218a9babcdc972722f4bf90779524515f3"
             ],
             "index": "pypi",
-            "version": "==19.10b0"
-        },
-        "certifi": {
-            "hashes": [
-                "sha256:e4f3620cfea4f83eedc95b24abd9cd56f3c4b146dd0177e83a21b4eb49e21e50",
-                "sha256:fd7c7c74727ddcf00e9acd26bba8da604ffec95bf1c2144e67aff7a8b50e6cef"
-            ],
-            "version": "==2019.9.11"
-        },
-        "chardet": {
-            "hashes": [
-                "sha256:84ab92ed1c4d4f16916e05906b6b75a6c0fb5db821cc65e70cbd64a3e2a5eaae",
-                "sha256:fc323ffcaeaed0e0a02bf4d117757b98aed530d9ed4531e3e15460124c106691"
-            ],
-            "version": "==3.0.4"
+            "version": "==23.3.0"
         },
         "click": {
             "hashes": [
-                "sha256:2335065e6395b9e67ca716de5f7526736bfa6ceead690adf616d925bdc622b13",
-                "sha256:5b94b49521f6456670fdb30cd82a4eca9412788a93fa6dd6df72c94d5a8ff2d7"
+                "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
+                "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
-            "version": "==7.0"
-        },
-        "codacy-coverage": {
-            "hashes": [
-                "sha256:b94651934745c638a980ad8d67494077e60f71e19e29aad1c275b66e0a070cbc",
-                "sha256:d8a1ce56b0dd156d6b1de14fa6217d32ec86097902f08a17ff2f95ba27264474"
-            ],
-            "index": "pypi",
-            "version": "==1.3.11"
-        },
-        "coverage": {
-            "hashes": [
-                "sha256:2358e685d0253125da42a48396038d4c7b4cd1448c00bbc4bda0cb8c43c2a870",
-                "sha256:25017cf384eeed2e6caf72efd3ec4124e32a8b7a4387600499104387975400c7",
-                "sha256:2e2de9423ff8b14303a97eafddd16c479fbcc9a0b8b0be3b7c3843a3e0cf6d69",
-                "sha256:324ed908e4e40a6e2451056fe502470ad4e79495cb7a03ecab94e6309c3e117e",
-                "sha256:34f865a0cf6255b694a46e4383a7131c61ea72c5b4c4f81d20e522fb1e440b4b",
-                "sha256:3a2bcc464b60a18f1f7167b95b2773ede93bf3722bfa59e0802717f652b6cc25",
-                "sha256:48d70865266d649b6602e2ba94820d7972ef470d3b72a8fd41a3d17321feed3a",
-                "sha256:50cf23523ab3a724c6905d3b60f87fa8250d9bae3995e09f49f63effa2b54f15",
-                "sha256:54c84a68abd8c4c5b71878b35eb85321df41f3d144c78181867d5b026ec74994",
-                "sha256:5b59d661ee7f3200aedd7b71882b7927ea7ed522df75e3853f316a79ad872a2e",
-                "sha256:5ffb39624bc573177888a21fb301ccee46838c600b27d58c3e9dae495f44d34a",
-                "sha256:699b3072b7f0e69ed175a88fa8b2ec7eefc4f34d490c54ed9a52feff21a15fdc",
-                "sha256:79ef4a2bb862110bd585174e551a783bee5c3aa461734a2ac7429193be357589",
-                "sha256:8210a6f93c4a8c6d460b402e20e38399529b99200c3318542faf6a520c9b6a5c",
-                "sha256:8d30c10cfd0a6fdf0a2d5023de00ef7b329cd6ead2310c9e53eab79c209acb70",
-                "sha256:97ac79ff28f2cda6ac00a803ee582b965951755f61ab43377482bfba450b619a",
-                "sha256:9fe4aacacff9028ed167db108bf013510654f148d83c4857fed61d2ce0588bf2",
-                "sha256:a5b6395d5957d638f8b1870561607e3c39b1a236ea6cff9eafe5b9bb1db913f2",
-                "sha256:ab32c5fad6905986a7e34e3acf01180a69bb60c2aa7331815b46e51c776a1943",
-                "sha256:ad67f0cfdfecbd49b9da46a7e488e6dc32a69388740b85c36a4ef4b33082cbad",
-                "sha256:aedad67c30326a1af324f45833a40b97180664912deb29942459ddbe9fa0ce19",
-                "sha256:b077cd0e70f41366ac1f9d09275258fa1906758a5d4f31cacc18b10dfcf90784",
-                "sha256:b8ea210810d3c14aec7561f8fe0d3eec582d1088100aaa0bb8153d53d867d20f",
-                "sha256:bf572722326ce6704e863447a070039a827072b7179352570859be899b9e6551",
-                "sha256:c0df57e189dacd2606cae6386acf127d01d85b2bf49acd9a65543b5d6c359ddc",
-                "sha256:d523e75f2a8a0b4a6a8be1287c0e0e3a561b8832b05ddd987d4cd7c62f3ad3bc",
-                "sha256:e10593c60c5f0bfd8b241bf9f27ef2191a3005b73dde8ada0424f642543a1e59",
-                "sha256:e9128444c83bc260aea988bf1ca6278a33ba730955bf94720468c656b61353eb",
-                "sha256:f7162f2e3711f3a08a8a741f92e1f63afd58d0713177979f2cf9723dd50161cf"
-            ],
-            "index": "pypi",
-            "version": "==5.0b1"
+            "markers": "python_version >= '3.7'",
+            "version": "==8.1.3"
         },
         "decorator": {
             "hashes": [
-                "sha256:54c38050039232e1db4ad7375cfce6748d7b41c29e95a081c8a6d2c30364a2ce",
-                "sha256:5d19b92a3c8f7f101c8dd86afd86b0f061a8ce4540ab8cd401fa2542756bce6d"
+                "sha256:637996211036b6385ef91435e4fae22989472f9d571faba8927ba8253acbc330",
+                "sha256:b8c3f85900b9dc423225913c5aace94729fe1fa9763b38939a95226f02d37186"
             ],
-            "version": "==4.4.1"
+            "markers": "python_version >= '3.11'",
+            "version": "==5.1.1"
         },
-        "idna": {
+        "executing": {
             "hashes": [
-                "sha256:c357b3f628cf53ae2c4c05627ecc484553142ca23264e593d327bcde5e9c3407",
-                "sha256:ea8b7f6188e6fa117537c3df7da9fc686d485087abf6ac197f9c46432f7e4a3c"
+                "sha256:0314a69e37426e3608aada02473b4161d4caf5a4b244d1d0c48072b8fee7bacc",
+                "sha256:19da64c18d2d851112f09c287f8d3dbbdf725ab0e569077efb6cdcbd3497c107"
             ],
-            "version": "==2.8"
+            "version": "==1.2.0"
         },
-        "importlib-metadata": {
+        "iniconfig": {
             "hashes": [
-                "sha256:aa18d7378b00b40847790e7c27e11673d7fed219354109d0e7b9e5b25dc3ad26",
-                "sha256:d5f18a79777f3aa179c145737780282e27b508fc8fd688cb17c7a813e8bd39af"
+                "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
+                "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
-            "markers": "python_version < '3.8'",
-            "version": "==0.23"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.0"
         },
         "ipdb": {
             "hashes": [
-                "sha256:473fdd798a099765f093231a8b1fabfa95b0b682fce12de0c74b61a4b4d8ee57"
+                "sha256:45529994741c4ab6d2388bfa5d7b725c2cf7fe9deffabdb8a6113aa5ed449ed4",
+                "sha256:e3ac6018ef05126d442af680aad863006ec19d02290561ac88b8b1c0b0cfc726"
             ],
             "index": "pypi",
-            "version": "==0.12.2"
+            "version": "==0.13.13"
         },
         "ipython": {
             "hashes": [
-                "sha256:dfd303b270b7b5232b3d08bd30ec6fd685d8a58cabd54055e3d69d8f029f7280",
-                "sha256:ed7ebe1cba899c1c3ccad6f7f1c2d2369464cc77dba8eebc65e2043e19cda995"
+                "sha256:1c80d08f04144a1994cda25569eab07fbdc4989bd8d8793e3a4ff643065ccb51",
+                "sha256:9c8487ac18f330c8a683fc50ab6d7bc0fcf9ef1d7a9f6ce7926938261067b81f"
             ],
-            "version": "==7.9.0"
-        },
-        "ipython-genutils": {
-            "hashes": [
-                "sha256:72dd37233799e619666c9f639a9da83c34013a73e8bbc79a7a6348d93c61fab8",
-                "sha256:eb2e116e75ecef9d4d228fdc66af54269afa26ab4463042e33785b887c628ba8"
-            ],
-            "version": "==0.2.0"
+            "markers": "python_version >= '3.11'",
+            "version": "==8.13.1"
         },
-        "isort": {
+        "jedi": {
             "hashes": [
-                "sha256:54da7e92468955c4fceacd0c86bd0ec997b0e1ee80d97f67c35a78b719dccab1",
-                "sha256:6e811fcb295968434526407adb8796944f1988c5b65e8139058f2014cbe100fd"
+                "sha256:203c1fd9d969ab8f2119ec0a3342e0b49910045abe6af0a3ae83a5764d54639e",
+                "sha256:bae794c30d07f6d910d32a7048af09b5a39ed740918da923c6b780790ebac612"
             ],
-            "index": "pypi",
-            "version": "==4.3.21"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.18.2"
         },
-        "jedi": {
+        "matplotlib-inline": {
             "hashes": [
-                "sha256:786b6c3d80e2f06fd77162a07fed81b8baa22dde5d62896a790a331d6ac21a27",
-                "sha256:ba859c74fa3c966a22f2aeebe1b74ee27e2a462f56d3f5f7ca4a59af61bfe42e"
+                "sha256:f1f41aab5328aa5aaea9b16d083b128102f8712542f819fe7e6a420ff581b311",
+                "sha256:f887e5f10ba98e8d2b150ddcf4702c1e5f8b3a20005eb0f74bfdbd360ee6f304"
             ],
-            "version": "==0.15.1"
+            "markers": "python_version >= '3.5'",
+            "version": "==0.1.6"
         },
-        "more-itertools": {
+        "mypy-extensions": {
             "hashes": [
-                "sha256:409cd48d4db7052af495b09dec721011634af3753ae1ef92d2b32f73a745f832",
-                "sha256:92b8c4b06dac4f0611c0729b2f2ede52b2e1bac1ab48f089c7ddc12e26bb60c4"
+                "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
+                "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
-            "version": "==7.2.0"
+            "markers": "python_version >= '3.5'",
+            "version": "==1.0.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:28b924174df7a2fa32c1953825ff29c61e2f5e082343165438812f00d3a7fc47",
-                "sha256:d9551545c6d761f3def1677baf08ab2a3ca17c56879e70fecba2fc4dde4ed108"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
-            "version": "==19.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==23.1"
         },
         "parso": {
             "hashes": [
-                "sha256:63854233e1fadb5da97f2744b6b24346d2750b85965e7e399bec1620232797dc",
-                "sha256:666b0ee4a7a1220f65d367617f2cd3ffddff3e205f3f16a0284df30e774c2a9c"
+                "sha256:8c07be290bb59f03588915921e29e8a50002acaf2cdc5fa0e0114f91709fafa0",
+                "sha256:c001d4636cd3aecdaf33cbb40aebb59b094be2a74c556778ef5576c175e19e75"
             ],
-            "version": "==0.5.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.8.3"
         },
         "pathspec": {
             "hashes": [
-                "sha256:e285ccc8b0785beadd4c18e5708b12bb8fcf529a1e61215b3feff1d1e559ea5c"
+                "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687",
+                "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"
             ],
-            "version": "==0.6.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.1"
         },
         "pexpect": {
             "hashes": [
-                "sha256:2094eefdfcf37a1fdbfb9aa090862c1a4878e5c7e0e7e7088bdb511c558e5cd1",
-                "sha256:9e2c1fd0e6ee3a49b28f95d4b33bc389c89b20af6a1255906e90ff1262ce62eb"
+                "sha256:0b48a55dcb3c05f3329815901ea4fc1537514d6ba867a152b581d69ae3710937",
+                "sha256:fc65a43959d153d0114afe13997d439c22823a27cefceb5ff35c2178c6784c0c"
             ],
             "markers": "sys_platform != 'win32'",
-            "version": "==4.7.0"
+            "version": "==4.8.0"
         },
         "pickleshare": {
             "hashes": [
                 "sha256:87683d47965c1da65cdacaf31c8441d12b8044cdec9aca500cd78fc2c683afca",
                 "sha256:9649af414d74d4df115d5d718f82acb59c9d418196b7b4290ed47a12ce62df56"
             ],
             "version": "==0.7.5"
         },
+        "platformdirs": {
+            "hashes": [
+                "sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4",
+                "sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==3.5.0"
+        },
         "pluggy": {
             "hashes": [
-                "sha256:15b2acde666561e1298d71b523007ed7364de07029219b604cf808bfa1c765b0",
-                "sha256:966c145cd83c96502c3c3868f50408687b38434af77734af1e9ca461a4081d2d"
+                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
+                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
-            "version": "==0.13.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==1.0.0"
         },
         "prompt-toolkit": {
             "hashes": [
-                "sha256:46642344ce457641f28fc9d1c9ca939b63dadf8df128b86f1b9860e59c73a5e4",
-                "sha256:e7f8af9e3d70f514373bf41aa51bc33af12a6db3f71461ea47fea985defb2c31",
-                "sha256:f15af68f66e664eaa559d4ac8a928111eebd5feda0c11738b5998045224829db"
+                "sha256:23ac5d50538a9a38c8bde05fecb47d0b403ecd0662857a86f886f798563d5b9b",
+                "sha256:45ea77a2f7c60418850331366c81cf6b5b9cf4c7fd34616f733c5427e6abbb1f"
             ],
-            "version": "==2.0.10"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.0.38"
         },
         "ptyprocess": {
             "hashes": [
-                "sha256:923f299cc5ad920c68f2bc0bc98b75b9f838b93b599941a6b63ddbc2476394c0",
-                "sha256:d7cc528d76e76342423ca640335bd3633420dc1366f258cb31d05e865ef5ca1f"
+                "sha256:4b41f3967fce3af57cc7e94b888626c18bf37a083e3651ca8feeb66d492fef35",
+                "sha256:5c5d0a3b48ceee0b48485e0c26037c0acd7d29765ca3fbb5cb3831d347423220"
             ],
-            "version": "==0.6.0"
+            "version": "==0.7.0"
         },
-        "py": {
+        "pure-eval": {
             "hashes": [
-                "sha256:64f65755aee5b381cea27766a3a147c3f15b9b6b9ac88676de66ba2ae36793fa",
-                "sha256:dc639b046a6e2cff5bbe40194ad65936d6ba360b52b3c3fe1d08a82dd50b5e53"
+                "sha256:01eaab343580944bc56080ebe0a674b39ec44a945e6d09ba7db3cb8cec289350",
+                "sha256:2b45320af6dfaa1750f543d714b6d1c520a1688dec6fd24d339063ce0aaa9ac3"
             ],
-            "version": "==1.8.0"
+            "version": "==0.2.2"
         },
         "pygments": {
             "hashes": [
-                "sha256:71e430bc85c88a430f000ac1d9b331d2407f681d6f6aec95e8bcfbc3df5b0127",
-                "sha256:881c4c157e45f30af185c1ffe8d549d48ac9127433f2c380c24b84572ad66297"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
-            "version": "==2.4.2"
-        },
-        "pyparsing": {
-            "hashes": [
-                "sha256:20f995ecd72f2a1f4bf6b072b63b22e2eb457836601e76d6e5dfcd75436acc1f",
-                "sha256:4ca62001be367f01bd3e92ecbb79070272a9d4964dce6a48a82ff0b8bc7e683a"
-            ],
-            "version": "==2.4.5"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.1"
         },
         "pytest": {
             "hashes": [
-                "sha256:1897d74f60a5d8be02e06d708b41bf2445da2ee777066bd68edf14474fc201eb",
-                "sha256:f6a567e20c04259d41adce9a360bd8991e6aa29dd9695c5e6bd25a9779272673"
-            ],
-            "index": "pypi",
-            "version": "==5.3.0"
-        },
-        "pytest-cov": {
-            "hashes": [
-                "sha256:cc6742d8bac45070217169f5f72ceee1e0e55b0221f54bcf24845972d3a47f2b",
-                "sha256:cdbdef4f870408ebdbfeb44e63e07eb18bb4619fae852f6e760645fa36172626"
+                "sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362",
+                "sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3"
             ],
             "index": "pypi",
-            "version": "==2.8.1"
+            "version": "==7.3.1"
         },
         "pytest-django": {
             "hashes": [
-                "sha256:17592f06d51c2ef4b7a0fb24aa32c8b6998506a03c8439606cb96db160106659",
-                "sha256:ef3d15b35ed7e46293475e6f282e71a53bcd8c6f87bdc5d5e7ad0f4d49352127"
+                "sha256:c60834861933773109334fe5a53e83d1ef4828f2203a1d6a0fa9972f4f75ab3e",
+                "sha256:d9076f759bb7c36939dbdd5ae6633c18edfc2902d1a69fdbefd2426b970ce6c2"
             ],
             "index": "pypi",
-            "version": "==3.7.0"
+            "version": "==4.5.2"
         },
-        "regex": {
+        "ruff": {
             "hashes": [
-                "sha256:15454b37c5a278f46f7aa2d9339bda450c300617ca2fca6558d05d870245edc7",
-                "sha256:1ad40708c255943a227e778b022c6497c129ad614bb7a2a2f916e12e8a359ee7",
-                "sha256:5e00f65cc507d13ab4dfa92c1232d004fa202c1d43a32a13940ab8a5afe2fb96",
-                "sha256:604dc563a02a74d70ae1f55208ddc9bfb6d9f470f6d1a5054c4bd5ae58744ab1",
-                "sha256:720e34a539a76a1fedcebe4397290604cc2bdf6f81eca44adb9fb2ea071c0c69",
-                "sha256:7caf47e4a9ac6ef08cabd3442cc4ca3386db141fb3c8b2a7e202d0470028e910",
-                "sha256:7faf534c1841c09d8fefa60ccde7b9903c9b528853ecf41628689793290ca143",
-                "sha256:b4e0406d822aa4993ac45072a584d57aa4931cf8288b5455bbf30c1d59dbad59",
-                "sha256:c31eaf28c6fe75ea329add0022efeed249e37861c19681960f99bbc7db981fb2",
-                "sha256:c7393597191fc2043c744db021643549061e12abe0b3ff5c429d806de7b93b66",
-                "sha256:d2b302f8cdd82c8f48e9de749d1d17f85ce9a0f082880b9a4859f66b07037dc6",
-                "sha256:e3d8dd0ec0ea280cf89026b0898971f5750a7bd92cb62c51af5a52abd020054a",
-                "sha256:ec032cbfed59bd5a4b8eab943c310acfaaa81394e14f44454ad5c9eba4f24a74"
+                "sha256:04e0b280dd246448564c892bce5607d820ad1f14944f3d535db98692e2a7ac07",
+                "sha256:1008f211ad8aa1d998517ac5bf3d68fbc68ec516d1da89b6081f25ff2f30b687",
+                "sha256:15386933dd8e03aafa3186f9e996d6823105492817311338fbcb64d0ecbcd95f",
+                "sha256:3e9fcee3f81129eabc75da005d839235e32d7d374f2d4c0db0c708dad4703d6e",
+                "sha256:4010b156f2e9fa6e74b5581098467f6ff68beac48945599b3a9239481e578ab4",
+                "sha256:4f75fa1632ea065b8f10678e7b6ae9873f84d5046bdf146990112751e98af42a",
+                "sha256:7890499c2c3dcb1e60de2a8b4c5f5775b2bfcdff7d3e68e38db5cb2d65b12006",
+                "sha256:82c41f276106017b6f075dd2f2cc68e1a0b434cc75488f816fc98bd41982628d",
+                "sha256:981e3c4d773f7ff52479c4fd74a65e408f1e13fa5f889b72214d400cd1299ce4",
+                "sha256:9af932f665e177de62e172901704257fd6e5bfabb95893867ff7382a851459d3",
+                "sha256:bed1d3fba306e3f7e13ce226927b84200350e25abd1e754e06ee361c6d41de15",
+                "sha256:c2b79919ebd93674b93dfc2c843e264bf8e52fbe737467e9b58521775c85f4ad",
+                "sha256:c3b7d4b365207f3e4c40d235127091478e595b31e35b6cd57d940920cdfae68b",
+                "sha256:ddcee0d91629a4fa4bc9faebf5b94d4615d50d1cd76d1098fa71fbe1c54f4104",
+                "sha256:ddf4503595b560bfa5fae92fa2e4cb09ec465ee4cf88cc248f10ad2e956deec3",
+                "sha256:ebc778d95f29c9917e6e7608b2b67815707e6ab8eb5af9341617beda479c3edf",
+                "sha256:ee6c7a77f142c427fa73e1f5f603fc1a39413a36fe6966ed0fc55e97f6921d9c"
             ],
-            "version": "==2019.11.1"
+            "index": "pypi",
+            "version": "==0.0.263"
         },
-        "requests": {
+        "setuptools": {
             "hashes": [
-                "sha256:11e007a8a2aa0323f5a921e9e6a2d7e4e67d9877e85773fba9ba6419025cbeb4",
-                "sha256:9cf5292fcd0f598c671cfc1e0d7d1a7f13bb8085e9a590f48c010551dc6c4b31"
+                "sha256:23aaf86b85ca52ceb801d32703f12d77517b2556af839621c641fca11287952b",
+                "sha256:f104fa03692a2602fa0fec6c6a9e63b6c8a968de13e17c026957dd1f53d80990"
             ],
-            "version": "==2.22.0"
+            "index": "pypi",
+            "version": "==67.7.2"
         },
         "six": {
             "hashes": [
-                "sha256:1f1b7d42e254082a9db6279deae68afb421ceba6158efa6131de7b3003ee93fd",
-                "sha256:30f610279e8b2578cab6db20741130331735c781b56053c59c4076da27f06b66"
+                "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
+                "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
-            "version": "==1.13.0"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==1.16.0"
         },
-        "toml": {
+        "stack-data": {
             "hashes": [
-                "sha256:229f81c57791a41d65e399fc06bf0848bab550a9dfd5ed66df18ce5f05e73d5c",
-                "sha256:235682dd292d5899d361a811df37e04a8828a5b1da3115886b73cf81ebc9100e"
+                "sha256:32d2dd0376772d01b6cb9fc996f3c8b57a357089dec328ed4b6553d037eaf815",
+                "sha256:cbb2a53eb64e5785878201a97ed7c7b94883f48b87bfb0bbe8b623c74679e4a8"
             ],
-            "version": "==0.10.0"
+            "version": "==0.6.2"
         },
         "traitlets": {
             "hashes": [
-                "sha256:70b4c6a1d9019d7b4f6846832288f86998aa3b9207c6821f3578a6a6a467fe44",
-                "sha256:d023ee369ddd2763310e4c3eae1ff649689440d4ae59d7485eb4cfbbe3e359f7"
+                "sha256:9e6ec080259b9a5940c797d58b613b5e31441c2257b87c2e795c5228ae80d2d8",
+                "sha256:f6cde21a9c68cf756af02035f72d5a723bf607e862e7be33ece505abf4a3bad9"
             ],
-            "version": "==4.3.3"
-        },
-        "typed-ast": {
-            "hashes": [
-                "sha256:1170afa46a3799e18b4c977777ce137bb53c7485379d9706af8a59f2ea1aa161",
-                "sha256:18511a0b3e7922276346bcb47e2ef9f38fb90fd31cb9223eed42c85d1312344e",
-                "sha256:262c247a82d005e43b5b7f69aff746370538e176131c32dda9cb0f324d27141e",
-                "sha256:2b907eb046d049bcd9892e3076c7a6456c93a25bebfe554e931620c90e6a25b0",
-                "sha256:354c16e5babd09f5cb0ee000d54cfa38401d8b8891eefa878ac772f827181a3c",
-                "sha256:48e5b1e71f25cfdef98b013263a88d7145879fbb2d5185f2a0c79fa7ebbeae47",
-                "sha256:4e0b70c6fc4d010f8107726af5fd37921b666f5b31d9331f0bd24ad9a088e631",
-                "sha256:630968c5cdee51a11c05a30453f8cd65e0cc1d2ad0d9192819df9978984529f4",
-                "sha256:66480f95b8167c9c5c5c87f32cf437d585937970f3fc24386f313a4c97b44e34",
-                "sha256:71211d26ffd12d63a83e079ff258ac9d56a1376a25bc80b1cdcdf601b855b90b",
-                "sha256:7954560051331d003b4e2b3eb822d9dd2e376fa4f6d98fee32f452f52dd6ebb2",
-                "sha256:838997f4310012cf2e1ad3803bce2f3402e9ffb71ded61b5ee22617b3a7f6b6e",
-                "sha256:95bd11af7eafc16e829af2d3df510cecfd4387f6453355188342c3e79a2ec87a",
-                "sha256:bc6c7d3fa1325a0c6613512a093bc2a2a15aeec350451cbdf9e1d4bffe3e3233",
-                "sha256:cc34a6f5b426748a507dd5d1de4c1978f2eb5626d51326e43280941206c209e1",
-                "sha256:d755f03c1e4a51e9b24d899561fec4ccaf51f210d52abdf8c07ee2849b212a36",
-                "sha256:d7c45933b1bdfaf9f36c579671fec15d25b06c8398f113dab64c18ed1adda01d",
-                "sha256:d896919306dd0aa22d0132f62a1b78d11aaf4c9fc5b3410d3c666b818191630a",
-                "sha256:fdc1c9bbf79510b76408840e009ed65958feba92a88833cdceecff93ae8fff66",
-                "sha256:ffde2fbfad571af120fcbfbbc61c72469e72f550d676c3342492a9dfdefb8f12"
-            ],
-            "version": "==1.4.0"
-        },
-        "urllib3": {
-            "hashes": [
-                "sha256:a8a318824cc77d1fd4b2bec2ded92646630d7fe8619497b142c84a9e6f5a7293",
-                "sha256:f3c5fd51747d450d4dcf6f923c81f78f811aab8205fda64b0aba34a4e48b0745"
-            ],
-            "version": "==1.25.7"
+            "markers": "python_version >= '3.7'",
+            "version": "==5.9.0"
         },
         "wcwidth": {
             "hashes": [
-                "sha256:3df37372226d6e63e1b1e1eda15c594bca98a22d33a23832a90998faa96bc65e",
-                "sha256:f4ebe71925af7b40a864553f761ed559b43544f8f71746c2d756c7fe788ade7c"
+                "sha256:795b138f6875577cd91bba52baf9e445cd5118fd32723b460e30a0af30ea230e",
+                "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"
             ],
-            "version": "==0.1.7"
+            "version": "==0.2.6"
         },
-        "zipp": {
+        "wheel": {
             "hashes": [
-                "sha256:3718b1cbcd963c7d4c5511a8240812904164b7f381b647143a89d3b98f9bcd8e",
-                "sha256:f06903e9f1f43b12d371004b4ac7b06ab39a44adc747266928ae6debfa7b3335"
+                "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873",
+                "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"
             ],
-            "version": "==0.6.0"
+            "index": "pypi",
+            "version": "==0.40.0"
         }
     }
 }
```


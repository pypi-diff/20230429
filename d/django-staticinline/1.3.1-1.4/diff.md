# Comparing `tmp/django-staticinline-1.3.1.tar.gz` & `tmp/django-staticinline-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-staticinline-1.3.1.tar", last modified: Wed Aug 15 17:33:09 2018, max compression
+gzip compressed data, was "django-staticinline-1.4.tar", last modified: Sat Apr 29 15:25:59 2023, max compression
```

## Comparing `django-staticinline-1.3.1.tar` & `django-staticinline-1.4.tar`

### file list

```diff
@@ -1,50 +1,40 @@
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-08-15 17:33:09.000000 django-staticinline-1.3.1/
--rw-r--r--   0 martin     (501) staff       (20)     4300 2018-08-15 17:33:09.000000 django-staticinline-1.3.1/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)      111 2018-08-14 11:55:12.000000 django-staticinline-1.3.1/MANIFEST.in
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-08-15 17:33:09.000000 django-staticinline-1.3.1/django_staticinline.egg-info/
--rw-r--r--   0 martin     (501) staff       (20)     4300 2018-08-15 17:33:08.000000 django-staticinline-1.3.1/django_staticinline.egg-info/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)        1 2018-08-09 08:43:01.000000 django-staticinline-1.3.1/django_staticinline.egg-info/not-zip-safe
--rw-r--r--   0 martin     (501) staff       (20)     1601 2018-08-15 17:33:09.000000 django-staticinline-1.3.1/django_staticinline.egg-info/SOURCES.txt
--rw-r--r--   0 martin     (501) staff       (20)       79 2018-08-15 17:33:08.000000 django-staticinline-1.3.1/django_staticinline.egg-info/requires.txt
--rw-r--r--   0 martin     (501) staff       (20)       13 2018-08-15 17:33:08.000000 django-staticinline-1.3.1/django_staticinline.egg-info/top_level.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2018-08-15 17:33:08.000000 django-staticinline-1.3.1/django_staticinline.egg-info/dependency_links.txt
--rw-r--r--   0 martin     (501) staff       (20)      401 2018-08-15 17:09:01.000000 django-staticinline-1.3.1/Pipfile
--rw-r--r--   0 martin     (501) staff       (20)       59 2018-08-09 08:36:33.000000 django-staticinline-1.3.1/setup.py
--rw-r--r--   0 martin     (501) staff       (20)     1138 2018-08-15 17:11:45.000000 django-staticinline-1.3.1/tox.ini
--rw-r--r--   0 martin     (501) staff       (20)     1218 2018-08-15 17:33:09.000000 django-staticinline-1.3.1/setup.cfg
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-08-15 17:33:09.000000 django-staticinline-1.3.1/staticinline/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-08-15 17:33:09.000000 django-staticinline-1.3.1/staticinline/templatetags/
--rw-r--r--   0 martin     (501) staff       (20)        0 2018-08-09 08:36:33.000000 django-staticinline-1.3.1/staticinline/templatetags/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     3422 2018-08-15 17:27:59.000000 django-staticinline-1.3.1/staticinline/templatetags/staticinline.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-08-15 17:33:09.000000 django-staticinline-1.3.1/staticinline/tests/
--rw-r--r--   0 martin     (501) staff       (20)     2132 2018-08-14 11:55:12.000000 django-staticinline-1.3.1/staticinline/tests/test_read_data.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-08-15 17:33:09.000000 django-staticinline-1.3.1/staticinline/tests/testapp/
--rw-r--r--   0 martin     (501) staff       (20)     1638 2018-08-15 07:57:23.000000 django-staticinline-1.3.1/staticinline/tests/testapp/apps.pyc
--rw-r--r--   0 martin     (501) staff       (20)     2046 2018-08-15 10:35:15.000000 django-staticinline-1.3.1/staticinline/tests/testapp/settings.pyc
--rw-r--r--   0 martin     (501) staff       (20)        0 2018-08-09 08:36:33.000000 django-staticinline-1.3.1/staticinline/tests/testapp/__init__.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-08-15 17:33:09.000000 django-staticinline-1.3.1/staticinline/tests/testapp/__pycache__/
--rw-r--r--   0 martin     (501) staff       (20)     1767 2018-08-15 10:35:25.000000 django-staticinline-1.3.1/staticinline/tests/testapp/__pycache__/settings.cpython-35.pyc
--rw-r--r--   0 martin     (501) staff       (20)     1795 2018-08-15 10:35:18.000000 django-staticinline-1.3.1/staticinline/tests/testapp/__pycache__/settings.cpython-34.pyc
--rw-r--r--   0 martin     (501) staff       (20)     1659 2018-08-15 10:35:31.000000 django-staticinline-1.3.1/staticinline/tests/testapp/__pycache__/settings.cpython-36.pyc
--rw-r--r--   0 martin     (501) staff       (20)     1658 2018-08-15 10:35:38.000000 django-staticinline-1.3.1/staticinline/tests/testapp/__pycache__/settings.cpython-37.pyc
--rw-r--r--   0 martin     (501) staff       (20)     1379 2018-08-15 07:58:43.000000 django-staticinline-1.3.1/staticinline/tests/testapp/__pycache__/apps.cpython-36.pyc
--rw-r--r--   0 martin     (501) staff       (20)     1383 2018-08-15 07:59:15.000000 django-staticinline-1.3.1/staticinline/tests/testapp/__pycache__/apps.cpython-37.pyc
--rw-r--r--   0 martin     (501) staff       (20)     1414 2018-08-15 07:58:11.000000 django-staticinline-1.3.1/staticinline/tests/testapp/__pycache__/apps.cpython-35.pyc
--rw-r--r--   0 martin     (501) staff       (20)     1416 2018-08-15 07:57:39.000000 django-staticinline-1.3.1/staticinline/tests/testapp/__pycache__/apps.cpython-34.pyc
--rw-r--r--   0 martin     (501) staff       (20)      165 2018-08-09 08:43:04.000000 django-staticinline-1.3.1/staticinline/tests/testapp/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 martin     (501) staff       (20)      169 2018-08-09 10:09:22.000000 django-staticinline-1.3.1/staticinline/tests/testapp/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 martin     (501) staff       (20)      165 2018-08-09 10:08:27.000000 django-staticinline-1.3.1/staticinline/tests/testapp/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 martin     (501) staff       (20)      165 2018-08-09 10:07:51.000000 django-staticinline-1.3.1/staticinline/tests/testapp/__pycache__/__init__.cpython-34.pyc
--rw-r--r--   0 martin     (501) staff       (20)      879 2018-08-14 11:55:12.000000 django-staticinline-1.3.1/staticinline/tests/testapp/apps.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-08-15 17:33:09.000000 django-staticinline-1.3.1/staticinline/tests/testapp/static/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-08-15 17:33:09.000000 django-staticinline-1.3.1/staticinline/tests/testapp/static/testapp/
--rw-r--r--   0 martin     (501) staff       (20)       14 2018-08-09 08:36:33.000000 django-staticinline-1.3.1/staticinline/tests/testapp/static/testapp/myfile.js
--rw-r--r--   0 martin     (501) staff       (20)     1910 2018-08-15 10:29:09.000000 django-staticinline-1.3.1/staticinline/tests/testapp/settings.py
--rw-r--r--   0 martin     (501) staff       (20)      169 2018-08-09 10:07:34.000000 django-staticinline-1.3.1/staticinline/tests/testapp/__init__.pyc
--rw-r--r--   0 martin     (501) staff       (20)       63 2018-08-14 11:55:12.000000 django-staticinline-1.3.1/staticinline/tests/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     7747 2018-08-15 10:29:09.000000 django-staticinline-1.3.1/staticinline/tests/test_templatetag.py
--rw-r--r--   0 martin     (501) staff       (20)        0 2018-08-09 08:36:33.000000 django-staticinline-1.3.1/staticinline/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     3045 2018-08-15 17:32:11.000000 django-staticinline-1.3.1/staticinline/apps.py
--rw-r--r--   0 martin     (501) staff       (20)      880 2018-08-14 11:55:12.000000 django-staticinline-1.3.1/staticinline/main.py
--rw-r--r--   0 martin     (501) staff       (20)     2025 2018-08-15 17:08:56.000000 django-staticinline-1.3.1/README.rst
--rw-r--r--   0 martin     (501) staff       (20)    21236 2018-08-15 17:13:11.000000 django-staticinline-1.3.1/Pipfile.lock
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-29 15:25:59.112493 django-staticinline-1.4/
+-rw-r--r--   0 martin     (501) staff       (20)      816 2023-04-29 15:08:52.000000 django-staticinline-1.4/CHANGELOG.rst
+-rw-r--r--   0 martin     (501) staff       (20)      134 2023-04-29 15:24:57.000000 django-staticinline-1.4/MANIFEST.in
+-rw-r--r--   0 martin     (501) staff       (20)     3738 2023-04-29 15:25:59.112560 django-staticinline-1.4/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)      522 2023-04-29 15:16:31.000000 django-staticinline-1.4/Pipfile
+-rw-r--r--   0 martin     (501) staff       (20)    41053 2023-04-29 15:00:46.000000 django-staticinline-1.4/Pipfile.lock
+-rw-r--r--   0 martin     (501) staff       (20)     2092 2023-04-29 15:12:40.000000 django-staticinline-1.4/README.rst
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-29 15:25:59.110368 django-staticinline-1.4/django_staticinline.egg-info/
+-rw-r--r--   0 martin     (501) staff       (20)     3738 2023-04-29 15:25:59.000000 django-staticinline-1.4/django_staticinline.egg-info/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)      959 2023-04-29 15:25:59.000000 django-staticinline-1.4/django_staticinline.egg-info/SOURCES.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2023-04-29 15:25:59.000000 django-staticinline-1.4/django_staticinline.egg-info/dependency_links.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2023-04-29 15:00:27.000000 django-staticinline-1.4/django_staticinline.egg-info/not-zip-safe
+-rw-r--r--   0 martin     (501) staff       (20)       12 2023-04-29 15:25:59.000000 django-staticinline-1.4/django_staticinline.egg-info/requires.txt
+-rw-r--r--   0 martin     (501) staff       (20)       13 2023-04-29 15:25:59.000000 django-staticinline-1.4/django_staticinline.egg-info/top_level.txt
+-rw-r--r--   0 martin     (501) staff       (20)     2199 2023-04-29 15:17:13.000000 django-staticinline-1.4/pyproject.toml
+-rw-r--r--   0 martin     (501) staff       (20)      916 2023-04-29 15:25:59.112802 django-staticinline-1.4/setup.cfg
+-rwxr-xr-x   0 martin     (501) staff       (20)       60 2023-04-29 15:18:28.000000 django-staticinline-1.4/setup.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-29 15:25:59.110900 django-staticinline-1.4/staticinline/
+-rw-r--r--   0 martin     (501) staff       (20)       64 2023-04-29 14:59:30.000000 django-staticinline-1.4/staticinline/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     3016 2023-04-29 15:19:10.000000 django-staticinline-1.4/staticinline/apps.py
+-rw-r--r--   0 martin     (501) staff       (20)      882 2023-04-29 14:59:30.000000 django-staticinline-1.4/staticinline/main.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-29 15:25:59.111159 django-staticinline-1.4/staticinline/templatetags/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2023-04-29 14:59:30.000000 django-staticinline-1.4/staticinline/templatetags/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     3447 2023-04-29 15:23:21.000000 django-staticinline-1.4/staticinline/templatetags/staticinline.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-29 15:25:59.111548 django-staticinline-1.4/staticinline/tests/
+-rw-r--r--   0 martin     (501) staff       (20)       63 2023-04-29 14:59:30.000000 django-staticinline-1.4/staticinline/tests/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     2118 2023-04-29 14:59:30.000000 django-staticinline-1.4/staticinline/tests/test_read_data.py
+-rw-r--r--   0 martin     (501) staff       (20)     7706 2023-04-29 15:21:03.000000 django-staticinline-1.4/staticinline/tests/test_templatetag.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-29 15:25:59.111901 django-staticinline-1.4/staticinline/tests/testapp/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2023-04-29 14:59:30.000000 django-staticinline-1.4/staticinline/tests/testapp/__init__.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-29 15:25:59.112262 django-staticinline-1.4/staticinline/tests/testapp/__pycache__/
+-rw-r--r--   0 martin     (501) staff       (20)      173 2023-04-29 15:05:18.000000 django-staticinline-1.4/staticinline/tests/testapp/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 martin     (501) staff       (20)     1385 2023-04-29 15:05:18.000000 django-staticinline-1.4/staticinline/tests/testapp/__pycache__/apps.cpython-39.pyc
+-rw-r--r--   0 martin     (501) staff       (20)     1668 2023-04-29 15:05:18.000000 django-staticinline-1.4/staticinline/tests/testapp/__pycache__/settings.cpython-39.pyc
+-rw-r--r--   0 martin     (501) staff       (20)      810 2023-04-29 15:17:26.000000 django-staticinline-1.4/staticinline/tests/testapp/apps.py
+-rw-r--r--   0 martin     (501) staff       (20)     2083 2023-04-29 15:21:03.000000 django-staticinline-1.4/staticinline/tests/testapp/settings.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-29 15:25:59.108221 django-staticinline-1.4/staticinline/tests/testapp/static/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-29 15:25:59.112386 django-staticinline-1.4/staticinline/tests/testapp/static/testapp/
+-rw-r--r--   0 martin     (501) staff       (20)       14 2023-04-29 14:59:30.000000 django-staticinline-1.4/staticinline/tests/testapp/static/testapp/myfile.js
+-rw-r--r--   0 martin     (501) staff       (20)      537 2023-04-29 15:10:15.000000 django-staticinline-1.4/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-staticinline-1.3.1/staticinline/templatetags/staticinline.py` & `django-staticinline-1.4/staticinline/templatetags/staticinline.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from __future__ import absolute_import
-
 from logging import getLogger
 
 from django.apps import apps
 from django.conf import settings
 from django.core.cache import cache as cache_backend
 from django.core.exceptions import ImproperlyConfigured
 from django.template.defaulttags import register
 
 from staticinline.main import read_static_file
 
 logger = getLogger(__file__)
-config = apps.get_app_config('staticinline')
+config = apps.get_app_config("staticinline")
 
 
 @register.simple_tag()
 def staticinline(path, encode=None, cache=False, cache_timeout=None):
     """
     Similar to Django's native `static` templatetag, but this includes
     the file directly in the template, rather than a link to it.
@@ -28,74 +26,76 @@
     <script>{% staticinline "myfile.js" %}</script>
 
     Becomes::
 
         <style type="text/css">body{ color: red; }</style>
         <script>alert("Hello World");</script>
 
-    Raises a ValueError if the the file does not exist, and
-    DEBUG is enabled.
+    Raises a ValueError if the file does not exist, and DEBUG is enabled.
 
     :param str path: Filename of the file to include.
+    :param str encode: Custom encoder function to run on data.
     :param bool cache: Whether to cache the response.
     :param int cache_timeout: The cache timeout for this particular file.
         If not set, AppConfig.cache_timeout is used.
-    :return: Returns the the file content *or* ``''`` (empty string) if the
+    :return: Returns the file content *or* ``''`` (empty string) if the
         file was not found, and ``DEBUG`` is ``False``.
     :rtype: str
     :raises ValueError: if the file is not found and ``DEBUG`` is ``True``
     """
     cache_key = None
     cache_timeout = cache_timeout or config.cache_timeout
 
     # Retrieve from cache if set
     if cache:
         cache_key = config.build_cache_key(path, encode)
         cached_obj = cache_backend.get(cache_key)
-        logger.debug('Cache enabled, cache key: %s', cache_key)
+        logger.debug("Cache enabled, cache key: %s", cache_key)
 
         if cached_obj:
-            logger.debug('Object found in cache')
+            logger.debug("Object found in cache")
             return config.data_response(cached_obj)
 
     try:
-        data = read_static_file(path, mode='rb' if encode else 'r')
+        data = read_static_file(path, mode="rb" if encode else "r")
     except ValueError:
         if settings.DEBUG:
             raise
-        return ''
+        return ""
 
     # If we don't encode the file further, we can return it right away.
     if not encode:
         if cache:
             cache_backend.set(cache_key, data, cache_timeout)
-            logger.debug('Object set in cache, cache key: %s', cache_key)
+            logger.debug("Object set in cache, cache key: %s", cache_key)
         return config.data_response(data)
 
     encoder_registry = config.get_encoder()
 
     if encode not in encoder_registry:
         raise ImproperlyConfigured(
-            '"{0}" is not a registered encoder. Valid values are: {1}'.format(
-                encode, ', '.join(encoder_registry.keys())
-            )
+            '"{}" is not a registered encoder. Valid values are: {}'.format(
+                encode,
+                ", ".join(encoder_registry.keys()),
+            ),
         )
     try:
         response = encoder_registry[encode](data, path)
         if cache:
-            logger.debug('Object encoded and set in cache, cache key: %s', cache_key)
+            logger.debug("Object encoded and set in cache, cache key: %s", cache_key)
             timeout = cache_timeout or config.cache_timeout
             cache_backend.set(cache_key, response, timeout)
         return config.data_response(response)
 
     # Anything could go wrong since we don't control the encoding
     # list itself. In case of an error raise that exception, unless
     # DEBUG mode is off. Then, same as above, return an empty string.
     except Exception as e:
-        logger.error(
+        logger.exception(
             'Error encoding to data format %s in static file "%s".',
-            encode, path)
-        logger.exception(e)
+            encode,
+            path,
+        )
         if settings.DEBUG:
             raise e
 
-    return ''
+    return ""
```

### Comparing `django-staticinline-1.3.1/staticinline/tests/test_read_data.py` & `django-staticinline-1.4/staticinline/tests/test_read_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,59 +6,57 @@
 from django.test import override_settings
 from django.test.testcases import TestCase
 
 from staticinline.main import read_static_file
 
 
 class ReadDataTests(TestCase):
-
     def setUp(self):
         # Django 1.8 won't create the STATIC_ROOT directory itself
         if not os.path.exists(settings.STATIC_ROOT):
             os.makedirs(settings.STATIC_ROOT)
 
     def tearDown(self):
         # Manually delete the collectstatic directory after every test
         # so we can be sure, all tests start from scratch.
         shutil.rmtree(settings.STATIC_ROOT)
 
     def test_read(self):
         """
         File is not read from the app's static dir when DEBUG is off.
         """
-        self.assertRaises(ValueError, read_static_file, 'testapp/myfile.js')
+        self.assertRaises(ValueError, read_static_file, "testapp/myfile.js")
 
     @override_settings(DEBUG=True)
     def test_missing_debug(self):
         """
         An exception is raised if the included file is not found in any
         static dirs.
         """
-        self.assertRaises(
-            ValueError, read_static_file, 'testapp/doesnotexist.js')
+        self.assertRaises(ValueError, read_static_file, "testapp/doesnotexist.js")
 
     @override_settings(DEBUG=True)
     def test_read_debug(self):
         """
         File is read from the app's static dir when DEBUG is on.
         """
-        data = read_static_file('testapp/myfile.js')
-        self.assertEqual(data, 'HelloWorld();\n')
+        data = read_static_file("testapp/myfile.js")
+        self.assertEqual(data, "HelloWorld();\n")
 
     def test_collectstatic(self):
         """
         Files is read from STATIC_ROOT when DEBUG is off.
         """
-        call_command('collectstatic', '-c', interactive=False)
-        data = read_static_file('testapp/myfile.js')
-        self.assertEqual(data, 'HelloWorld();\n')
+        call_command("collectstatic", "-c", interactive=False)
+        data = read_static_file("testapp/myfile.js")
+        self.assertEqual(data, "HelloWorld();\n")
 
     @override_settings(DEBUG=True)
     def test_collectstatic_extraneous_debug(self):
         """
         Extraneous files in STATIC_ROOT are not read when DEBUG is on.
         """
-        call_command('collectstatic', '-c', interactive=False)
-        path = 'testapp/unexpected.bat'
-        with open(os.path.join(settings.STATIC_ROOT, path), 'w') as f:
-            f.write('@echo off')
+        call_command("collectstatic", "-c", interactive=False)
+        path = "testapp/unexpected.bat"
+        with open(os.path.join(settings.STATIC_ROOT, path), "w") as f:
+            f.write("@echo off")
         self.assertRaises(ValueError, read_static_file, path)
```

### Comparing `django-staticinline-1.3.1/staticinline/tests/testapp/__pycache__/settings.cpython-36.pyc` & `django-staticinline-1.4/staticinline/tests/testapp/__pycache__/settings.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,105 @@
-00000000: 330d 0d0a 7500 745b 7607 0000 e300 0000  3...u.t[v.......
-00000010: 0000 0000 0000 0000 0009 0000 0040 0000  .............@..
-00000020: 0073 ba00 0000 6400 6401 6c00 5a01 6400  .s....d.d.l.Z.d.
-00000030: 6401 6c02 5a02 6402 5a03 6403 5a04 6404  d.l.Z.d.Z.d.Z.d.
-00000040: 6405 6406 6407 9c02 6901 5a05 6404 6408  d.d.d...i.Z.d.d.
-00000050: 6409 640a 9c02 6901 5a06 640b 6700 6402  d.d...i.Z.d.g.d.
-00000060: 640c 640d 640e 640f 6410 6704 6901 6411  d.d.d.d.d.g.i.d.
-00000070: 9c04 6701 5a07 6412 6413 6414 6703 5a08  ..g.Z.d.d.d.g.Z.
-00000080: 6426 5a09 6509 5a0a 6416 5a0b 6417 5a0c  d&Z.e.Z.d.Z.d.Z.
-00000090: 6418 6419 6702 5a0d 6501 6a0e 6a0f 641a  d.d.g.Z.e.j.j.d.
-000000a0: 641b 641c 641d 641e 6901 6901 641c 641f  d.d.d.d.i.i.d.d.
-000000b0: 641c 6420 9c02 6901 6421 6502 6a10 6a11  d.d ..i.d!e.j.j.
-000000c0: 6422 6423 8302 6a12 8300 641c 6701 6424  d"d#..j...d.g.d$
-000000d0: 9c02 6901 6425 9c05 8301 0100 6401 5300  ..i.d%......d.S.
-000000e0: 2927 e900 0000 004e 547a 2573 7570 6572  )'.....NTz%super
-000000f0: 2d73 6563 7265 742d 7374 6174 6963 696e  -secret-staticin
-00000100: 6c69 6e65 2d74 6573 7469 6e67 2d6b 6579  line-testing-key
-00000110: da07 6465 6661 756c 747a 1a64 6a61 6e67  ..defaultz.djang
-00000120: 6f2e 6462 2e62 6163 6b65 6e64 732e 7371  o.db.backends.sq
-00000130: 6c69 7465 337a 083a 6d65 6d6f 7279 3a29  lite3z.:memory:)
-00000140: 02da 0645 4e47 494e 45da 044e 414d 457a  ...ENGINE..NAMEz
-00000150: 2d64 6a61 6e67 6f2e 636f 7265 2e63 6163  -django.core.cac
-00000160: 6865 2e62 6163 6b65 6e64 732e 6c6f 636d  he.backends.locm
-00000170: 656d 2e4c 6f63 4d65 6d43 6163 6865 7a10  em.LocMemCachez.
-00000180: 756e 6971 7565 2d73 6e6f 7766 6c61 6b65  unique-snowflake
-00000190: 2902 da07 4241 434b 454e 44da 084c 4f43  )...BACKEND..LOC
-000001a0: 4154 494f 4e7a 2f64 6a61 6e67 6f2e 7465  ATIONz/django.te
-000001b0: 6d70 6c61 7465 2e62 6163 6b65 6e64 732e  mplate.backends.
-000001c0: 646a 616e 676f 2e44 6a61 6e67 6f54 656d  django.DjangoTem
-000001d0: 706c 6174 6573 da12 636f 6e74 6578 745f  plates..context_
-000001e0: 7072 6f63 6573 736f 7273 7a28 646a 616e  processorsz(djan
-000001f0: 676f 2e74 656d 706c 6174 652e 636f 6e74  go.template.cont
-00000200: 6578 745f 7072 6f63 6573 736f 7273 2e64  ext_processors.d
-00000210: 6562 7567 7a2a 646a 616e 676f 2e74 656d  ebugz*django.tem
-00000220: 706c 6174 652e 636f 6e74 6578 745f 7072  plate.context_pr
-00000230: 6f63 6573 736f 7273 2e72 6571 7565 7374  ocessors.request
-00000240: 7a2b 646a 616e 676f 2e63 6f6e 7472 6962  z+django.contrib
-00000250: 2e61 7574 682e 636f 6e74 6578 745f 7072  .auth.context_pr
-00000260: 6f63 6573 736f 7273 2e61 7574 687a 3364  ocessors.authz3d
-00000270: 6a61 6e67 6f2e 636f 6e74 7269 622e 6d65  jango.contrib.me
-00000280: 7373 6167 6573 2e63 6f6e 7465 7874 5f70  ssages.context_p
-00000290: 726f 6365 7373 6f72 732e 6d65 7373 6167  rocessors.messag
-000002a0: 6573 2904 7205 0000 00da 0444 4952 53da  es).r......DIRS.
-000002b0: 0841 5050 5f44 4952 53da 074f 5054 494f  .APP_DIRS..OPTIO
-000002c0: 4e53 7a3f 7374 6174 6963 696e 6c69 6e65  NSz?staticinline
-000002d0: 2e74 6573 7473 2e74 6573 7461 7070 2e61  .tests.testapp.a
-000002e0: 7070 732e 4375 7374 6f6d 697a 6564 5374  pps.CustomizedSt
-000002f0: 6174 6963 496e 6c69 6e65 4170 7043 6f6e  aticInlineAppCon
-00000300: 6669 677a 1a73 7461 7469 6369 6e6c 696e  figz.staticinlin
-00000310: 652e 7465 7374 732e 7465 7374 6170 707a  e.tests.testappz
-00000320: 1a64 6a61 6e67 6f2e 636f 6e74 7269 622e  .django.contrib.
-00000330: 7374 6174 6963 6669 6c65 73fa 2964 6a61  staticfiles.)dja
-00000340: 6e67 6f2e 6d69 6464 6c65 7761 7265 2e63  ngo.middleware.c
-00000350: 6f6d 6d6f 6e2e 436f 6d6d 6f6e 4d69 6464  ommon.CommonMidd
-00000360: 6c65 7761 7265 7a23 2f74 6d70 2f74 6573  lewarez#/tmp/tes
-00000370: 742d 7374 6174 6963 696e 6c69 6e65 2d73  t-staticinline-s
-00000380: 7461 7469 632d 726f 6f74 2f7a 082f 7374  tatic-root/z./st
-00000390: 6174 6963 2f7a 3364 6a61 6e67 6f2e 636f  atic/z3django.co
-000003a0: 6e74 7269 622e 7374 6174 6963 6669 6c65  ntrib.staticfile
-000003b0: 732e 6669 6e64 6572 732e 4669 6c65 5379  s.finders.FileSy
-000003c0: 7374 656d 4669 6e64 6572 7a37 646a 616e  stemFinderz7djan
-000003d0: 676f 2e63 6f6e 7472 6962 2e73 7461 7469  go.contrib.stati
-000003e0: 6366 696c 6573 2e66 696e 6465 7273 2e41  cfiles.finders.A
-000003f0: 7070 4469 7265 6374 6f72 6965 7346 696e  ppDirectoriesFin
-00000400: 6465 72e9 0100 0000 465a 0763 6f6e 736f  der.....FZ.conso
-00000410: 6c65 da06 666f 726d 6174 7a33 2528 6173  le..formatz3%(as
-00000420: 6374 696d 6529 7320 2528 6e61 6d65 292d  ctime)s %(name)-
-00000430: 3132 7320 2528 6c65 7665 6c6e 616d 6529  12s %(levelname)
-00000440: 2d38 7320 2528 6d65 7373 6167 6529 737a  -8s %(message)sz
-00000450: 156c 6f67 6769 6e67 2e53 7472 6561 6d48  .logging.StreamH
-00000460: 616e 646c 6572 2902 da05 636c 6173 73da  andler)...class.
-00000470: 0966 6f72 6d61 7474 6572 da00 5a09 4c4f  .formatter..Z.LO
-00000480: 475f 4c45 5645 4cda 0545 5252 4f52 2902  G_LEVEL..ERROR).
-00000490: da05 6c65 7665 6cda 0868 616e 646c 6572  ..level..handler
-000004a0: 7329 05da 0776 6572 7369 6f6e 5a18 6469  s)...versionZ.di
-000004b0: 7361 626c 655f 6578 6973 7469 6e67 5f6c  sable_existing_l
-000004c0: 6f67 6765 7273 5a0a 666f 726d 6174 7465  oggersZ.formatte
-000004d0: 7273 7213 0000 005a 076c 6f67 6765 7273  rsr....Z.loggers
-000004e0: 2901 720b 0000 0029 135a 0e6c 6f67 6769  ).r....).Z.loggi
-000004f0: 6e67 2e63 6f6e 6669 67da 076c 6f67 6769  ng.config..loggi
-00000500: 6e67 da02 6f73 da05 4445 4255 47da 0a53  ng..os..DEBUG..S
-00000510: 4543 5245 545f 4b45 59da 0944 4154 4142  ECRET_KEY..DATAB
-00000520: 4153 4553 da06 4341 4348 4553 da09 5445  ASES..CACHES..TE
-00000530: 4d50 4c41 5445 53da 0e49 4e53 5441 4c4c  MPLATES..INSTALL
-00000540: 4544 5f41 5050 53da 124d 4944 444c 4557  ED_APPS..MIDDLEW
-00000550: 4152 455f 434c 4153 5345 53da 0a4d 4944  ARE_CLASSES..MID
-00000560: 444c 4557 4152 45da 0b53 5441 5449 435f  DLEWARE..STATIC_
-00000570: 524f 4f54 da0a 5354 4154 4943 5f55 524c  ROOT..STATIC_URL
-00000580: da13 5354 4154 4943 4649 4c45 535f 4649  ..STATICFILES_FI
-00000590: 4e44 4552 53da 0663 6f6e 6669 675a 0a64  NDERS..configZ.d
-000005a0: 6963 7443 6f6e 6669 67da 0765 6e76 6972  ictConfig..envir
-000005b0: 6f6e da03 6765 74da 0575 7070 6572 a900  on..get..upper..
-000005c0: 7226 0000 0072 2600 0000 fa52 2f55 7365  r&...r&....R/Use
-000005d0: 7273 2f6d 6172 7469 6e2f 576f 726b 7370  rs/martin/Worksp
-000005e0: 6163 652f 646a 616e 676f 2d73 7461 7469  ace/django-stati
-000005f0: 6369 6e6c 696e 652f 7374 6174 6963 696e  cinline/staticin
-00000600: 6c69 6e65 2f74 6573 7473 2f74 6573 7461  line/tests/testa
-00000610: 7070 2f73 6574 7469 6e67 732e 7079 da08  pp/settings.py..
-00000620: 3c6d 6f64 756c 653e 0100 0000 734a 0000  <module>....sJ..
-00000630: 0008 0108 0304 0204 0302 0102 010a 0502  ................
-00000640: 0102 010a 0602 0102 0102 0202 0102 0102  ................
-00000650: 0102 010e 0702 0102 0106 0404 0204 0204  ................
-00000660: 0104 0402 0106 0306 0102 0102 0202 0108  ................
-00000670: 0402 0102 0108 0402 0110 01              ...........
+00000000: 610d 0d0a 0000 0000 d230 4d64 8307 0000  a........0Md....
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 000b 0000 0040 0000 0073 b400 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6402  d.l.Z.d.d.l.Z.d.
+00000040: 5a03 6403 5a04 6404 6405 6406 6407 9c02  Z.d.Z.d.d.d.d...
+00000050: 6901 5a05 6404 6408 6409 640a 9c02 6901  i.Z.d.d.d.d...i.
+00000060: 5a06 640b 6700 6402 640c 6700 640d a201  Z.d.g.d.d.g.d...
+00000070: 6901 640e 9c04 6701 5a07 6700 640f a201  i.d...g.Z.g.d...
+00000080: 5a08 6410 5a09 6509 5a0a 6411 5a0b 6412  Z.d.Z.e.Z.d.Z.d.
+00000090: 5a0c 6413 6414 6702 5a0d 6501 6a0e a00f  Z.d.d.g.Z.e.j...
+000000a0: 6415 6416 6417 6418 6419 6901 6901 6417  d.d.d.d.d.i.i.d.
+000000b0: 641a 6417 641b 9c02 6901 641c 6502 6a10  d.d.d...i.d.e.j.
+000000c0: a011 641d 641e a102 a012 a100 6417 6701  ..d.d.......d.g.
+000000d0: 641f 9c02 6901 6420 9c05 a101 0100 6401  d...i.d ......d.
+000000e0: 5300 2921 e900 0000 004e 547a 2573 7570  S.)!.....NTz%sup
+000000f0: 6572 2d73 6563 7265 742d 7374 6174 6963  er-secret-static
+00000100: 696e 6c69 6e65 2d74 6573 7469 6e67 2d6b  inline-testing-k
+00000110: 6579 da07 6465 6661 756c 747a 1a64 6a61  ey..defaultz.dja
+00000120: 6e67 6f2e 6462 2e62 6163 6b65 6e64 732e  ngo.db.backends.
+00000130: 7371 6c69 7465 337a 083a 6d65 6d6f 7279  sqlite3z.:memory
+00000140: 3a29 02da 0645 4e47 494e 45da 044e 414d  :)...ENGINE..NAM
+00000150: 457a 2d64 6a61 6e67 6f2e 636f 7265 2e63  Ez-django.core.c
+00000160: 6163 6865 2e62 6163 6b65 6e64 732e 6c6f  ache.backends.lo
+00000170: 636d 656d 2e4c 6f63 4d65 6d43 6163 6865  cmem.LocMemCache
+00000180: 7a10 756e 6971 7565 2d73 6e6f 7766 6c61  z.unique-snowfla
+00000190: 6b65 2902 da07 4241 434b 454e 44da 084c  ke)...BACKEND..L
+000001a0: 4f43 4154 494f 4e7a 2f64 6a61 6e67 6f2e  OCATIONz/django.
+000001b0: 7465 6d70 6c61 7465 2e62 6163 6b65 6e64  template.backend
+000001c0: 732e 646a 616e 676f 2e44 6a61 6e67 6f54  s.django.DjangoT
+000001d0: 656d 706c 6174 6573 5a12 636f 6e74 6578  emplatesZ.contex
+000001e0: 745f 7072 6f63 6573 736f 7273 2904 7a28  t_processors).z(
+000001f0: 646a 616e 676f 2e74 656d 706c 6174 652e  django.template.
+00000200: 636f 6e74 6578 745f 7072 6f63 6573 736f  context_processo
+00000210: 7273 2e64 6562 7567 7a2a 646a 616e 676f  rs.debugz*django
+00000220: 2e74 656d 706c 6174 652e 636f 6e74 6578  .template.contex
+00000230: 745f 7072 6f63 6573 736f 7273 2e72 6571  t_processors.req
+00000240: 7565 7374 7a2b 646a 616e 676f 2e63 6f6e  uestz+django.con
+00000250: 7472 6962 2e61 7574 682e 636f 6e74 6578  trib.auth.contex
+00000260: 745f 7072 6f63 6573 736f 7273 2e61 7574  t_processors.aut
+00000270: 687a 3364 6a61 6e67 6f2e 636f 6e74 7269  hz3django.contri
+00000280: 622e 6d65 7373 6167 6573 2e63 6f6e 7465  b.messages.conte
+00000290: 7874 5f70 726f 6365 7373 6f72 732e 6d65  xt_processors.me
+000002a0: 7373 6167 6573 2904 7205 0000 005a 0444  ssages).r....Z.D
+000002b0: 4952 53da 0841 5050 5f44 4952 53da 074f  IRS..APP_DIRS..O
+000002c0: 5054 494f 4e53 2903 7a3f 7374 6174 6963  PTIONS).z?static
+000002d0: 696e 6c69 6e65 2e74 6573 7473 2e74 6573  inline.tests.tes
+000002e0: 7461 7070 2e61 7070 732e 4375 7374 6f6d  tapp.apps.Custom
+000002f0: 697a 6564 5374 6174 6963 496e 6c69 6e65  izedStaticInline
+00000300: 4170 7043 6f6e 6669 677a 1a73 7461 7469  AppConfigz.stati
+00000310: 6369 6e6c 696e 652e 7465 7374 732e 7465  cinline.tests.te
+00000320: 7374 6170 707a 1a64 6a61 6e67 6f2e 636f  stappz.django.co
+00000330: 6e74 7269 622e 7374 6174 6963 6669 6c65  ntrib.staticfile
+00000340: 7329 017a 2964 6a61 6e67 6f2e 6d69 6464  s).z)django.midd
+00000350: 6c65 7761 7265 2e63 6f6d 6d6f 6e2e 436f  leware.common.Co
+00000360: 6d6d 6f6e 4d69 6464 6c65 7761 7265 7a23  mmonMiddlewarez#
+00000370: 2f74 6d70 2f74 6573 742d 7374 6174 6963  /tmp/test-static
+00000380: 696e 6c69 6e65 2d73 7461 7469 632d 726f  inline-static-ro
+00000390: 6f74 2f7a 082f 7374 6174 6963 2f7a 3364  ot/z./static/z3d
+000003a0: 6a61 6e67 6f2e 636f 6e74 7269 622e 7374  jango.contrib.st
+000003b0: 6174 6963 6669 6c65 732e 6669 6e64 6572  aticfiles.finder
+000003c0: 732e 4669 6c65 5379 7374 656d 4669 6e64  s.FileSystemFind
+000003d0: 6572 7a37 646a 616e 676f 2e63 6f6e 7472  erz7django.contr
+000003e0: 6962 2e73 7461 7469 6366 696c 6573 2e66  ib.staticfiles.f
+000003f0: 696e 6465 7273 2e41 7070 4469 7265 6374  inders.AppDirect
+00000400: 6f72 6965 7346 696e 6465 72e9 0100 0000  oriesFinder.....
+00000410: 465a 0763 6f6e 736f 6c65 da06 666f 726d  FZ.console..form
+00000420: 6174 7a33 2528 6173 6374 696d 6529 7320  atz3%(asctime)s 
+00000430: 2528 6e61 6d65 292d 3132 7320 2528 6c65  %(name)-12s %(le
+00000440: 7665 6c6e 616d 6529 2d38 7320 2528 6d65  velname)-8s %(me
+00000450: 7373 6167 6529 737a 156c 6f67 6769 6e67  ssage)sz.logging
+00000460: 2e53 7472 6561 6d48 616e 646c 6572 2902  .StreamHandler).
+00000470: da05 636c 6173 73da 0966 6f72 6d61 7474  ..class..formatt
+00000480: 6572 da00 5a09 4c4f 475f 4c45 5645 4cda  er..Z.LOG_LEVEL.
+00000490: 0545 5252 4f52 2902 da05 6c65 7665 6cda  .ERROR)...level.
+000004a0: 0868 616e 646c 6572 7329 05da 0776 6572  .handlers)...ver
+000004b0: 7369 6f6e 5a18 6469 7361 626c 655f 6578  sionZ.disable_ex
+000004c0: 6973 7469 6e67 5f6c 6f67 6765 7273 5a0a  isting_loggersZ.
+000004d0: 666f 726d 6174 7465 7273 7210 0000 005a  formattersr....Z
+000004e0: 076c 6f67 6765 7273 2913 5a0e 6c6f 6767  .loggers).Z.logg
+000004f0: 696e 672e 636f 6e66 6967 da07 6c6f 6767  ing.config..logg
+00000500: 696e 67da 026f 73da 0544 4542 5547 da0a  ing..os..DEBUG..
+00000510: 5345 4352 4554 5f4b 4559 da09 4441 5441  SECRET_KEY..DATA
+00000520: 4241 5345 53da 0643 4143 4845 53da 0954  BASES..CACHES..T
+00000530: 454d 504c 4154 4553 da0e 494e 5354 414c  EMPLATES..INSTAL
+00000540: 4c45 445f 4150 5053 5a12 4d49 4444 4c45  LED_APPSZ.MIDDLE
+00000550: 5741 5245 5f43 4c41 5353 4553 da0a 4d49  WARE_CLASSES..MI
+00000560: 4444 4c45 5741 5245 da0b 5354 4154 4943  DDLEWARE..STATIC
+00000570: 5f52 4f4f 54da 0a53 5441 5449 435f 5552  _ROOT..STATIC_UR
+00000580: 4cda 1353 5441 5449 4346 494c 4553 5f46  L..STATICFILES_F
+00000590: 494e 4445 5253 da06 636f 6e66 6967 5a0a  INDERS..configZ.
+000005a0: 6469 6374 436f 6e66 6967 da07 656e 7669  dictConfig..envi
+000005b0: 726f 6eda 0367 6574 da05 7570 7065 72a9  ron..get..upper.
+000005c0: 0072 2200 0000 7222 0000 00fa 522f 5573  .r"...r"....R/Us
+000005d0: 6572 732f 6d61 7274 696e 2f57 6f72 6b73  ers/martin/Works
+000005e0: 7061 6365 2f64 6a61 6e67 6f2d 7374 6174  pace/django-stat
+000005f0: 6963 696e 6c69 6e65 2f73 7461 7469 6369  icinline/statici
+00000600: 6e6c 696e 652f 7465 7374 732f 7465 7374  nline/tests/test
+00000610: 6170 702f 7365 7474 696e 6773 2e70 79da  app/settings.py.
+00000620: 083c 6d6f 6475 6c65 3e01 0000 0073 5200  .<module>....sR.
+00000630: 0000 0801 0802 0402 0402 0e03 0201 0201  ................
+00000640: 02fe 04ff 0409 0201 0201 0202 08ff 02fc  ................
+00000650: 04ff 0410 0806 0401 0402 0401 0404 0201  ................
+00000660: 02fe 0405 0602 0201 0202 08ff 0204 0201  ................
+00000670: 0201 02fe 04ff 0207 0201 1001 04fe 04ff  ................
+00000680: 02f4 04ff                                ....
```

### Comparing `django-staticinline-1.3.1/staticinline/tests/testapp/__pycache__/apps.cpython-36.pyc` & `django-staticinline-1.4/staticinline/tests/testapp/__pycache__/apps.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-00000000: 330d 0d0a 20c3 725b 6f03 0000 e300 0000  3... .r[o.......
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2400 0000 6400 5a00 6401 6402 6c01  .s$...d.Z.d.d.l.
-00000030: 6d02 5a02 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
-00000040: 6502 8303 5a03 6405 5300 2906 7a60 0a43  e...Z.d.S.).z`.C
-00000050: 7573 746f 6d20 6170 7020 636f 6e66 6967  ustom app config
-00000060: 2066 6f72 2073 7461 7469 6369 6e6c 696e   for staticinlin
-00000070: 6520 746f 2064 656d 6f6e 7374 7261 7465  e to demonstrate
-00000080: 2061 6e64 2074 6573 740a 7468 6520 2763   and test.the 'c
-00000090: 7573 746f 6d20 656e 636f 6465 7227 2066  ustom encoder' f
-000000a0: 756e 6374 696f 6e61 6c69 7479 2e0a e900  unctionality....
-000000b0: 0000 0029 01da 1553 7461 7469 6349 6e6c  ...)...StaticInl
-000000c0: 696e 6541 7070 436f 6e66 6967 6300 0000  ineAppConfigc...
-000000d0: 0000 0000 0000 0000 0003 0000 0000 0000  ................
-000000e0: 0073 3000 0000 6500 5a01 6400 5a02 6401  .s0...e.Z.d.Z.d.
-000000f0: 5a03 8700 6601 6402 6403 8408 5a04 6404  Z...f.d.d...Z.d.
-00000100: 6405 8400 5a05 6406 6407 8400 5a06 8700  d...Z.d.d...Z...
-00000110: 0400 5a07 5300 2908 da1f 4375 7374 6f6d  ..Z.S.)...Custom
-00000120: 697a 6564 5374 6174 6963 496e 6c69 6e65  izedStaticInline
-00000130: 4170 7043 6f6e 6669 677a 400a 2020 2020  AppConfigz@.    
-00000140: 4164 6420 6120 6375 7374 6f6d 2065 6e63  Add a custom enc
-00000150: 6f64 6572 2074 6f20 7468 6520 6c69 7374  oder to the list
-00000160: 2074 6f20 7465 7374 2074 6861 7420 6265   to test that be
-00000170: 6861 7669 6f72 0a20 2020 2063 0100 0000  havior.    c....
-00000180: 0000 0000 0200 0000 0400 0000 0300 0000  ................
-00000190: 7326 0000 0074 0074 017c 0083 026a 0283  s&...t.t.|...j..
-000001a0: 007d 017c 016a 037c 006a 047c 006a 0564  .}.|.j.|.j.|.j.d
-000001b0: 019c 0283 0101 007c 0153 0029 024e 2902  .......|.S.).N).
-000001c0: da09 7570 7065 7263 6173 65da 0662 726f  ..uppercase..bro
-000001d0: 6b65 6e29 06da 0573 7570 6572 7203 0000  ken)...superr...
-000001e0: 00da 0b67 6574 5f65 6e63 6f64 6572 da06  ...get_encoder..
-000001f0: 7570 6461 7465 7204 0000 0072 0500 0000  updater....r....
-00000200: 2902 da04 7365 6c66 da07 656e 636f 6465  )...self..encode
-00000210: 7229 01da 095f 5f63 6c61 7373 5f5f a900  r)...__class__..
-00000220: fa4e 2f55 7365 7273 2f6d 6172 7469 6e2f  .N/Users/martin/
-00000230: 576f 726b 7370 6163 652f 646a 616e 676f  Workspace/django
-00000240: 2d73 7461 7469 6369 6e6c 696e 652f 7374  -staticinline/st
-00000250: 6174 6963 696e 6c69 6e65 2f74 6573 7473  aticinline/tests
-00000260: 2f74 6573 7461 7070 2f61 7070 732e 7079  /testapp/apps.py
-00000270: 7207 0000 000d 0000 0073 0a00 0000 0001  r........s......
-00000280: 0e01 0401 0401 0c02 7a2b 4375 7374 6f6d  ........z+Custom
-00000290: 697a 6564 5374 6174 6963 496e 6c69 6e65  izedStaticInline
-000002a0: 4170 7043 6f6e 6669 672e 6765 745f 656e  AppConfig.get_en
-000002b0: 636f 6465 7263 0300 0000 0000 0000 0300  coderc..........
-000002c0: 0000 0200 0000 4300 0000 7310 0000 007c  ......C...s....|
-000002d0: 016a 007c 006a 0183 016a 0283 0053 0029  .j.|.j...j...S.)
-000002e0: 017a 4d0a 2020 2020 2020 2020 5361 6d70  .zM.        Samp
-000002f0: 6c65 2065 6e63 6f64 6572 2074 6861 7420  le encoder that 
-00000300: 7475 726e 7320 7468 6520 696e 636f 6d69  turns the incomi
-00000310: 6e67 2074 6578 7420 6461 7461 2075 7070  ng text data upp
-00000320: 6572 6361 7365 2e0a 2020 2020 2020 2020  ercase..        
-00000330: 2903 da06 6465 636f 6465 5a17 656e 636f  )...decodeZ.enco
-00000340: 6465 725f 7265 7370 6f6e 7365 5f66 6f72  der_response_for
-00000350: 6d61 74da 0575 7070 6572 2903 7209 0000  mat..upper).r...
-00000360: 00da 0464 6174 61da 0470 6174 6872 0c00  ...data..pathr..
-00000370: 0000 720c 0000 0072 0d00 0000 7204 0000  ..r....r....r...
-00000380: 0015 0000 0073 0200 0000 0004 7a29 4375  .....s......z)Cu
-00000390: 7374 6f6d 697a 6564 5374 6174 6963 496e  stomizedStaticIn
-000003a0: 6c69 6e65 4170 7043 6f6e 6669 672e 7570  lineAppConfig.up
-000003b0: 7065 7263 6173 6563 0300 0000 0000 0000  percasec........
-000003c0: 0300 0000 0200 0000 4300 0000 7308 0000  ........C...s...
-000003d0: 0064 0164 021b 0053 0029 037a 510a 2020  .d.d...S.).zQ.  
-000003e0: 2020 2020 2020 5468 6973 2069 6e74 656e        This inten
-000003f0: 7469 6f6e 616c 6c79 2072 6169 7365 7320  tionally raises 
-00000400: 616e 2045 7863 6570 7469 6f6e 2074 6f20  an Exception to 
-00000410: 7465 7374 2065 7272 6f72 2072 6570 6f72  test error repor
-00000420: 7469 6e67 2e0a 2020 2020 2020 2020 e901  ting..        ..
-00000430: 0000 0072 0100 0000 720c 0000 0029 0372  ...r....r....).r
-00000440: 0900 0000 7210 0000 0072 1100 0000 720c  ....r....r....r.
-00000450: 0000 0072 0c00 0000 720d 0000 0072 0500  ...r....r....r..
-00000460: 0000 1b00 0000 7302 0000 0000 047a 2643  ......s......z&C
-00000470: 7573 746f 6d69 7a65 6453 7461 7469 6349  ustomizedStaticI
-00000480: 6e6c 696e 6541 7070 436f 6e66 6967 2e62  nlineAppConfig.b
-00000490: 726f 6b65 6e29 08da 085f 5f6e 616d 655f  roken)...__name_
-000004a0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-000004b0: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
-000004c0: 6f63 5f5f 7207 0000 0072 0400 0000 7205  oc__r....r....r.
-000004d0: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-000004e0: 5f5f 720c 0000 0072 0c00 0000 2901 720b  __r....r....).r.
-000004f0: 0000 0072 0d00 0000 7203 0000 0009 0000  ...r....r.......
-00000500: 0073 0800 0000 0803 0401 0c08 0806 7203  .s............r.
-00000510: 0000 004e 2904 7216 0000 005a 1173 7461  ...N).r....Z.sta
-00000520: 7469 6369 6e6c 696e 652e 6170 7073 7202  ticinline.appsr.
-00000530: 0000 0072 0300 0000 720c 0000 0072 0c00  ...r....r....r..
-00000540: 0000 720c 0000 0072 0d00 0000 da08 3c6d  ..r....r......<m
-00000550: 6f64 756c 653e 0400 0000 7304 0000 0004  odule>....s.....
-00000560: 020c 03                                  ...
+00000000: 610d 0d0a 0000 0000 d230 4d64 4f03 0000  a........0MdO...
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 0004 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
+00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 4700  Z.d.d.l.m.Z...G.
+00000040: 6403 6404 8400 6404 6502 8303 5a03 6405  d.d...d.e...Z.d.
+00000050: 5300 2906 7a60 0a43 7573 746f 6d20 6170  S.).z`.Custom ap
+00000060: 7020 636f 6e66 6967 2066 6f72 2073 7461  p config for sta
+00000070: 7469 6369 6e6c 696e 6520 746f 2064 656d  ticinline to dem
+00000080: 6f6e 7374 7261 7465 2061 6e64 2074 6573  onstrate and tes
+00000090: 740a 7468 6520 2763 7573 746f 6d20 656e  t.the 'custom en
+000000a0: 636f 6465 7227 2066 756e 6374 696f 6e61  coder' functiona
+000000b0: 6c69 7479 2e0a e900 0000 0029 01da 1553  lity.......)...S
+000000c0: 7461 7469 6349 6e6c 696e 6541 7070 436f  taticInlineAppCo
+000000d0: 6e66 6967 6300 0000 0000 0000 0000 0000  nfigc...........
+000000e0: 0000 0000 0003 0000 0000 0000 0073 3000  .............s0.
+000000f0: 0000 6500 5a01 6400 5a02 6401 5a03 8700  ..e.Z.d.Z.d.Z...
+00000100: 6601 6402 6403 8408 5a04 6404 6405 8400  f.d.d...Z.d.d...
+00000110: 5a05 6406 6407 8400 5a06 8700 0400 5a07  Z.d.d...Z.....Z.
+00000120: 5300 2908 da1f 4375 7374 6f6d 697a 6564  S.)...Customized
+00000130: 5374 6174 6963 496e 6c69 6e65 4170 7043  StaticInlineAppC
+00000140: 6f6e 6669 677a 400a 2020 2020 4164 6420  onfigz@.    Add 
+00000150: 6120 6375 7374 6f6d 2065 6e63 6f64 6572  a custom encoder
+00000160: 2074 6f20 7468 6520 6c69 7374 2074 6f20   to the list to 
+00000170: 7465 7374 2074 6861 7420 6265 6861 7669  test that behavi
+00000180: 6f72 0a20 2020 2063 0100 0000 0000 0000  or.    c........
+00000190: 0000 0000 0200 0000 0500 0000 0300 0000  ................
+000001a0: 7326 0000 0074 0074 017c 0083 02a0 02a1  s&...t.t.|......
+000001b0: 007d 017c 01a0 037c 006a 047c 006a 0564  .}.|...|.j.|.j.d
+000001c0: 019c 02a1 0101 007c 0153 0029 024e 2902  .......|.S.).N).
+000001d0: da09 7570 7065 7263 6173 65da 0662 726f  ..uppercase..bro
+000001e0: 6b65 6e29 06da 0573 7570 6572 7203 0000  ken)...superr...
+000001f0: 00da 0b67 6574 5f65 6e63 6f64 6572 da06  ...get_encoder..
+00000200: 7570 6461 7465 7204 0000 0072 0500 0000  updater....r....
+00000210: 2902 da04 7365 6c66 da07 656e 636f 6465  )...self..encode
+00000220: 72a9 01da 095f 5f63 6c61 7373 5f5f a900  r....__class__..
+00000230: fa4e 2f55 7365 7273 2f6d 6172 7469 6e2f  .N/Users/martin/
+00000240: 576f 726b 7370 6163 652f 646a 616e 676f  Workspace/django
+00000250: 2d73 7461 7469 6369 6e6c 696e 652f 7374  -staticinline/st
+00000260: 6174 6963 696e 6c69 6e65 2f74 6573 7473  aticinline/tests
+00000270: 2f74 6573 7461 7070 2f61 7070 732e 7079  /testapp/apps.py
+00000280: 7207 0000 000e 0000 0073 0600 0000 0001  r........s......
+00000290: 0e01 1401 7a2b 4375 7374 6f6d 697a 6564  ....z+Customized
+000002a0: 5374 6174 6963 496e 6c69 6e65 4170 7043  StaticInlineAppC
+000002b0: 6f6e 6669 672e 6765 745f 656e 636f 6465  onfig.get_encode
+000002c0: 7263 0300 0000 0000 0000 0000 0000 0300  rc..............
+000002d0: 0000 0300 0000 4300 0000 7310 0000 007c  ......C...s....|
+000002e0: 01a0 007c 006a 01a1 01a0 02a1 0053 0029  ...|.j.......S.)
+000002f0: 017a 4d0a 2020 2020 2020 2020 5361 6d70  .zM.        Samp
+00000300: 6c65 2065 6e63 6f64 6572 2074 6861 7420  le encoder that 
+00000310: 7475 726e 7320 7468 6520 696e 636f 6d69  turns the incomi
+00000320: 6e67 2074 6578 7420 6461 7461 2075 7070  ng text data upp
+00000330: 6572 6361 7365 2e0a 2020 2020 2020 2020  ercase..        
+00000340: 2903 da06 6465 636f 6465 5a17 656e 636f  )...decodeZ.enco
+00000350: 6465 725f 7265 7370 6f6e 7365 5f66 6f72  der_response_for
+00000360: 6d61 74da 0575 7070 6572 a903 7209 0000  mat..upper..r...
+00000370: 00da 0464 6174 61da 0470 6174 6872 0d00  ...data..pathr..
+00000380: 0000 720d 0000 0072 0e00 0000 7204 0000  ..r....r....r...
+00000390: 0013 0000 0073 0200 0000 0004 7a29 4375  .....s......z)Cu
+000003a0: 7374 6f6d 697a 6564 5374 6174 6963 496e  stomizedStaticIn
+000003b0: 6c69 6e65 4170 7043 6f6e 6669 672e 7570  lineAppConfig.up
+000003c0: 7065 7263 6173 6563 0300 0000 0000 0000  percasec........
+000003d0: 0000 0000 0300 0000 0200 0000 4300 0000  ............C...
+000003e0: 7308 0000 0064 0164 021b 0053 0029 037a  s....d.d...S.).z
+000003f0: 510a 2020 2020 2020 2020 5468 6973 2069  Q.        This i
+00000400: 6e74 656e 7469 6f6e 616c 6c79 2072 6169  ntentionally rai
+00000410: 7365 7320 616e 2045 7863 6570 7469 6f6e  ses an Exception
+00000420: 2074 6f20 7465 7374 2065 7272 6f72 2072   to test error r
+00000430: 6570 6f72 7469 6e67 2e0a 2020 2020 2020  eporting..      
+00000440: 2020 e901 0000 0072 0100 0000 720d 0000    .....r....r...
+00000450: 0072 1100 0000 720d 0000 0072 0d00 0000  .r....r....r....
+00000460: 720e 0000 0072 0500 0000 1900 0000 7302  r....r........s.
+00000470: 0000 0000 047a 2643 7573 746f 6d69 7a65  .....z&Customize
+00000480: 6453 7461 7469 6349 6e6c 696e 6541 7070  dStaticInlineApp
+00000490: 436f 6e66 6967 2e62 726f 6b65 6e29 08da  Config.broken)..
+000004a0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+000004b0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000004c0: 655f 5fda 075f 5f64 6f63 5f5f 7207 0000  e__..__doc__r...
+000004d0: 0072 0400 0000 7205 0000 00da 0d5f 5f63  .r....r......__c
+000004e0: 6c61 7373 6365 6c6c 5f5f 720d 0000 0072  lasscell__r....r
+000004f0: 0d00 0000 720b 0000 0072 0e00 0000 7203  ....r....r....r.
+00000500: 0000 0009 0000 0073 0800 0000 0801 0404  .......s........
+00000510: 0c05 0806 7203 0000 004e 2904 7218 0000  ....r....N).r...
+00000520: 005a 1173 7461 7469 6369 6e6c 696e 652e  .Z.staticinline.
+00000530: 6170 7073 7202 0000 0072 0300 0000 720d  appsr....r....r.
+00000540: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00000550: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000560: 7304 0000 0004 050c 03                   s........
```

### Comparing `django-staticinline-1.3.1/staticinline/tests/testapp/apps.py` & `django-staticinline-1.4/staticinline/tests/testapp/apps.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,26 +6,24 @@
 from staticinline.apps import StaticInlineAppConfig
 
 
 class CustomizedStaticInlineAppConfig(StaticInlineAppConfig):
     """
     Add a custom encoder to the list to test that behavior
     """
+
     def get_encoder(self):
-        encoder = super(CustomizedStaticInlineAppConfig, self).get_encoder()
-        encoder.update({
-            'uppercase': self.uppercase,
-            'broken': self.broken,
-        })
+        encoder = super().get_encoder()
+        encoder.update({"uppercase": self.uppercase, "broken": self.broken})
         return encoder
 
     def uppercase(self, data, path):
         """
         Sample encoder that turns the incoming text data uppercase.
         """
         return data.decode(self.encoder_response_format).upper()
 
     def broken(self, data, path):
         """
         This intentionally raises an Exception to test error reporting.
         """
-        return 1/0
+        return 1 / 0
```

### Comparing `django-staticinline-1.3.1/staticinline/tests/test_templatetag.py` & `django-staticinline-1.4/staticinline/tests/test_templatetag.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,207 +1,203 @@
+from unittest import mock
+
+from django.core.cache import cache
 from django.core.exceptions import ImproperlyConfigured
 from django.template import Template
 from django.template.context import Context
 from django.test import override_settings
 from django.test.testcases import TestCase
-from django.core.cache import cache
 
 from staticinline.templatetags import staticinline
 
-try:
-    from unittest import mock
-except ImportError:
-    import mock
-
 
 def render(source, **context):
     return Template(source).render(Context(context))
 
 
 class StaticInlineTests(TestCase):
-    template = (
-        '{% load staticinline %}' '<script>{% staticinline "somefile" %}</script>'
-    )
+    template = '{% load staticinline %}<script>{% staticinline "somefile" %}</script>'
 
     def test_found(self):
         """
         Static file is are correctly included inline the template.
         """
-        with mock.patch.object(staticinline, 'read_static_file') as reader:
+        with mock.patch.object(staticinline, "read_static_file") as reader:
             reader.return_value = 'alert("hi")'
             rendered = render(self.template)
             self.assertEqual(rendered, '<script>alert("hi")</script>')
 
     def test_file_missing(self):
         """
         An empty string is returned if the inlined file is missing and
         DEBUG is off.
         """
-        with mock.patch.object(staticinline, 'read_static_file') as reader:
-            reader.side_effect = ValueError('Not found')
+        with mock.patch.object(staticinline, "read_static_file") as reader:
+            reader.side_effect = ValueError("Not found")
             rendered = render(self.template)
-            self.assertEqual(rendered, '<script></script>')
+            self.assertEqual(rendered, "<script></script>")
 
     @override_settings(DEBUG=True)
     def test_file_missing_debug(self):
         """
         An error raised from read_static_file if the inlined file is
         missing and DEBUG is on.
         """
-        with mock.patch.object(staticinline, 'read_static_file') as reader:
-            reader.side_effect = ValueError('Not found')
+        with mock.patch.object(staticinline, "read_static_file") as reader:
+            reader.side_effect = ValueError("Not found")
             self.assertRaises(ValueError, render, self.template)
 
 
 class CachedStaticInlineTests(TestCase):
     template_cached = (
-        '{% load staticinline %}'
+        "{% load staticinline %}"
         '<script>{% staticinline "somefile" cache=True cache_timeout=60 %}</script>'
     )
     template_cached_encoder = (
-        '{% load staticinline %}'
+        "{% load staticinline %}"
         '{% staticinline "some-other-file" encode="base64" cache=True cache_timeout=60 %}'
     )
 
     def tearDown(self):
         cache.clear()
 
     def test_cache(self):
         """
         Static file is are correctly included inline the template.
         """
         # Call once to set in cache
-        with mock.patch.object(staticinline, 'read_static_file') as reader:
+        with mock.patch.object(staticinline, "read_static_file") as reader:
             reader.return_value = 'alert("hi")'
             rendered = render(self.template_cached)
             self.assertEqual(rendered, '<script>alert("hi")</script>')
 
         # Call again to test cache retrieval
-        with mock.patch.object(staticinline, 'read_static_file') as reader:
+        with mock.patch.object(staticinline, "read_static_file") as reader:
             reader.return_value = 'alert("hi")'
             rendered = render(self.template_cached)
             self.assertEqual(rendered, '<script>alert("hi")</script>')
 
     def test_cache_encoder(self):
         """
         Static file is are correctly included inline the template.
         """
         # Call once to set in cache
-        with mock.patch.object(staticinline, 'read_static_file') as reader:
-            reader.return_value = b'it is bytestring data'
+        with mock.patch.object(staticinline, "read_static_file") as reader:
+            reader.return_value = b"it is bytestring data"
             rendered = render(self.template_cached_encoder)
-            self.assertEqual(rendered, 'aXQgaXMgYnl0ZXN0cmluZyBkYXRh')
+            self.assertEqual(rendered, "aXQgaXMgYnl0ZXN0cmluZyBkYXRh")
 
         # Call again to test cache retrieval
-        with mock.patch.object(staticinline, 'read_static_file') as reader:
-            reader.return_value = b'it is bytestring data'
+        with mock.patch.object(staticinline, "read_static_file") as reader:
+            reader.return_value = b"it is bytestring data"
             rendered = render(self.template_cached_encoder)
-            self.assertEqual(rendered, 'aXQgaXMgYnl0ZXN0cmluZyBkYXRh')
+            self.assertEqual(rendered, "aXQgaXMgYnl0ZXN0cmluZyBkYXRh")
 
 
 class EncoderTests(TestCase):
     def test_unregistered(self):
         """
         Using an unregistered encoder will raise ImproperlyConfigured.
         """
         template = (
-            '{% load staticinline %}'
+            "{% load staticinline %}"
             '{% staticinline "somefile" encode="doesnotexist" %}'
         )
-        with mock.patch.object(staticinline, 'read_static_file') as reader:
+        with mock.patch.object(staticinline, "read_static_file") as reader:
             reader.return_value = 'alert("hi")'
             self.assertRaises(ImproperlyConfigured, render, template)
 
     def test_error(self):
         """
         If the encoder raises any exception, return an empty string when
         DEBUG is off.
         """
-        with mock.patch.object(staticinline, 'read_static_file') as reader:
-            reader.return_value = b'it is bytestring data'
+        with mock.patch.object(staticinline, "read_static_file") as reader:
+            reader.return_value = b"it is bytestring data"
             rendered = render(
-                '{% load staticinline %}'
-                'My Key: {% staticinline "somefile" encode="broken" %}'
+                "{% load staticinline %}"
+                'My Key: {% staticinline "somefile" encode="broken" %}',
             )
-            self.assertEqual(rendered, 'My Key: ')
+            self.assertEqual(rendered, "My Key: ")
 
     @override_settings(DEBUG=True)
     def test_error_debug(self):
         """
         If the encoder raises any exception, the exception is raised
         when DEBUG is on.
         """
-        with mock.patch.object(staticinline, 'read_static_file') as reader:
-            reader.return_value = b'it is bytestring data'
+        with mock.patch.object(staticinline, "read_static_file") as reader:
+            reader.return_value = b"it is bytestring data"
             template = (
-                '{% load staticinline %}'
+                "{% load staticinline %}"
                 'My Key: {% staticinline "somefile" encode="broken" %}'
             )
             self.assertRaises(ZeroDivisionError, render, template)
 
     def test_custom(self):
         """
         Custom encoders can be used in a separate appconfig.
         In testapp/apps.py, the 'uppercase' encoder is added.
         """
-        with mock.patch.object(staticinline, 'read_static_file') as reader:
-            reader.return_value = b'shouting'
+        with mock.patch.object(staticinline, "read_static_file") as reader:
+            reader.return_value = b"shouting"
             rendered = render(
-                '{% load staticinline %}'
-                '{% staticinline "somefile" encode="uppercase" %}'
+                "{% load staticinline %}"
+                '{% staticinline "somefile" encode="uppercase" %}',
             )
-            self.assertEqual(rendered, 'SHOUTING')
+            self.assertEqual(rendered, "SHOUTING")
 
     def test_base64(self):
         """
         The 'base64' encoder is shipped with this application.
         """
-        with mock.patch.object(staticinline, 'read_static_file') as reader:
-            reader.return_value = b'it is bytestring data'
+        with mock.patch.object(staticinline, "read_static_file") as reader:
+            reader.return_value = b"it is bytestring data"
             rendered = render(
-                '{% load staticinline %}'
-                'My Key: {% staticinline "somefile" encode="base64" %}'
+                "{% load staticinline %}"
+                'My Key: {% staticinline "somefile" encode="base64" %}',
             )
-            self.assertEqual(rendered, 'My Key: aXQgaXMgYnl0ZXN0cmluZyBkYXRh')
+            self.assertEqual(rendered, "My Key: aXQgaXMgYnl0ZXN0cmluZyBkYXRh")
 
     @override_settings(DEBUG=True)
     def test_data(self):
         """
         The 'data' URI encoder is shipped with this application.
         """
-        with mock.patch.object(staticinline, 'read_static_file') as reader:
-            reader.return_value = b'png content'
+        with mock.patch.object(staticinline, "read_static_file") as reader:
+            reader.return_value = b"png content"
             rendered = render(
-                '{% load staticinline %}'
-                '<img src="{% staticinline "a.png" encode="data" %}">'
+                "{% load staticinline %}"
+                '<img src="{% staticinline "a.png" encode="data" %}">',
             )
             self.assertEqual(
-                rendered, '<img src="data:image/png;base64,cG5nIGNvbnRlbnQ=">'
+                rendered,
+                '<img src="data:image/png;base64,cG5nIGNvbnRlbnQ=">',
             )
 
     @override_settings(DEBUG=True)
     def test_data_unknown_mimetype(self):
         """
         The data URI still works if no mimetype can be guessed.
         """
-        with mock.patch.object(staticinline, 'read_static_file') as reader:
-            reader.return_value = b'png content'
+        with mock.patch.object(staticinline, "read_static_file") as reader:
+            reader.return_value = b"png content"
             rendered = render(
-                '{% load staticinline %}'
-                '<img src="{% staticinline "somefile" encode="data" %}">'
+                "{% load staticinline %}"
+                '<img src="{% staticinline "somefile" encode="data" %}">',
             )
             self.assertEqual(rendered, '<img src="data:;base64,cG5nIGNvbnRlbnQ=">')
 
     def test_sri(self):
         """
         The 'base64' encoder is shipped with this application.
         """
-        with mock.patch.object(staticinline, 'read_static_file') as reader:
+        with mock.patch.object(staticinline, "read_static_file") as reader:
             reader.return_value = b'alert("hi")'
             rendered = render(
-                '{% load staticinline %}'
-                'integrity="{% staticinline "somefile" encode="sri" %}"'
+                "{% load staticinline %}"
+                'integrity="{% staticinline "somefile" encode="sri" %}"',
             )
             self.assertEqual(
                 rendered,
                 'integrity="sha256-fdu2bQSeIdU5fvNNkRCjiwUEOOb+NLZDyGNVShZ1vCM="',
             )
```

### Comparing `django-staticinline-1.3.1/staticinline/apps.py` & `django-staticinline-1.4/staticinline/apps.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import mimetypes
 import base64
 import hashlib
+import mimetypes
 
 from django.apps import AppConfig
 from django.utils.safestring import mark_safe
 
 
 class StaticInlineAppConfig(AppConfig):
-    name = 'staticinline'
-    verbose_name = 'Static Inline Files'
-    encoder_response_format = 'utf-8'
+    name = "staticinline"
+    verbose_name = "Static Inline Files"
+    encoder_response_format = "utf-8"
 
     # Default cache timeout if not specified individually in the template tag
     # with the ``cache_timeout`` argument.
     cache_timeout = 60 * 60
 
     def build_cache_key(self, path, encode=None):
-        s = '{0}{1}'.format(path, encode or '')
-        return 'staticinline-{0}'.format(hashlib.sha1(s.encode()).hexdigest())
+        s = "{}{}".format(path, encode or "")
+        return f"staticinline-{hashlib.sha1(s.encode()).hexdigest()}"  # noqa: S324 Probable use of insecure hash functions
 
     def data_response(self, data):
         """
         This method transforms the data right before its written in the
         template. This is applied to all files, while 'encoder' are set
         individually per file.
 
@@ -37,17 +37,17 @@
         template tag. Example::
 
             {% staticinline "myfile.gif" encode="base64" %}
 
         This can be manually extended by providing a custom AppConfig.
         """
         return {
-            'base64': self.encode_base64,
-            'data': self.encode_data_uri,
-            'sri': self.encode_sri,
+            "base64": self.encode_base64,
+            "data": self.encode_data_uri,
+            "sri": self.encode_sri,
         }
 
     def encode_base64(self, data, path):
         """
         Encodes with standard Base64.
 
         :param bytes data: Input data to encode.
@@ -62,18 +62,15 @@
         Convert to the data URI scheme.
 
         :param bytes data: Input data to encode.
         :return: data URI string.
         :rtype: str
         """
         mimetype = mimetypes.guess_type(path)[0]
-        if mimetype is None:
-            prefix = 'data:;base64,'
-        else:
-            prefix = 'data:{0};base64,'.format(mimetype)
+        prefix = "data:;base64," if mimetype is None else f"data:{mimetype};base64,"
         return prefix + self.encode_base64(data, data)
 
     def encode_sri(self, data, path):
         """
         Adds Subresource Integrity encoder to staticinline. Read more:
 
         https://developer.mozilla.org/en-US/docs/Web/Security/Subresource_Integrity
@@ -89,10 +86,10 @@
             integrity="{% staticinline "base.css" encode="sri" %}"
             crossorigin="anonymous"/>
 
         :param bytes data: File content to build the SRI hash of.
         :return: sha256 hash
         :rtype: str
         """
-        hash = hashlib.sha256(data).digest()
-        hash_base64 = base64.b64encode(hash).decode()
-        return 'sha256-{}'.format(hash_base64)
+        h = hashlib.sha256(data).digest()
+        h_base64 = base64.b64encode(h).decode()
+        return f"sha256-{h_base64}"
```

### Comparing `django-staticinline-1.3.1/staticinline/main.py` & `django-staticinline-1.4/staticinline/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from django.conf import settings
 from django.contrib.staticfiles.finders import find
 from django.contrib.staticfiles.storage import staticfiles_storage
 
 logger = getLogger(__file__)
 
 
-def read_static_file(path, mode='r'):
+def read_static_file(path, mode="r"):
     """
     Return the contents of a static file.
     """
     if settings.DEBUG:
         # Lookup file in using Django's static finder, e.g. when in
         # local development mode.
         filename = find(path)
@@ -19,9 +19,9 @@
             return open(filename, mode=mode).read()
     elif staticfiles_storage.exists(path):
         # Look up file in collectstatic target directory (regular
         # deployment).
         return staticfiles_storage.open(path, mode=mode).read()
 
     message = 'Unable to include inline static file "%s", file not found.'
-    logger.error(message, path)
+    logger.warning(message, path)
     raise ValueError(message % path)
```


# Comparing `tmp/django-bulk-signals-0.3.0.tar.gz` & `tmp/django-bulk-signals-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bulk-signals-0.3.0.tar", last modified: Fri Apr 28 11:51:32 2023, max compression
+gzip compressed data, was "django-bulk-signals-0.4.0.tar", last modified: Sat Apr 29 19:36:03 2023, max compression
```

## Comparing `django-bulk-signals-0.3.0.tar` & `django-bulk-signals-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:51:32.715282 django-bulk-signals-0.3.0/
--rw-r--r--   0 root         (0) root         (0)     1253 2023-04-28 11:51:29.000000 django-bulk-signals-0.3.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1063 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       33 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2468 2023-04-28 11:51:32.715282 django-bulk-signals-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1324 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:51:32.711282 django-bulk-signals-0.3.0/bulk_signals/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 11:51:29.000000 django-bulk-signals-0.3.0/bulk_signals/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2294 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/bulk_signals/apps.py
--rw-r--r--   0 root         (0) root         (0)      203 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/bulk_signals/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:51:32.711282 django-bulk-signals-0.3.0/bulk_signals/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/bulk_signals/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      194 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/bulk_signals/tests/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:51:32.711282 django-bulk-signals-0.3.0/bulk_signals/tests/migrations/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/bulk_signals/tests/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/bulk_signals/tests/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      887 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/bulk_signals/tests/models.py
--rw-r--r--   0 root         (0) root         (0)      298 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/bulk_signals/tests/settings.py
--rw-r--r--   0 root         (0) root         (0)     3512 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/bulk_signals/tests/tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:51:32.715282 django-bulk-signals-0.3.0/django_bulk_signals.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2468 2023-04-28 11:51:32.000000 django-bulk-signals-0.3.0/django_bulk_signals.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-04-28 11:51:32.000000 django-bulk-signals-0.3.0/django_bulk_signals.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 11:51:32.000000 django-bulk-signals-0.3.0/django_bulk_signals.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-28 11:51:32.000000 django-bulk-signals-0.3.0/django_bulk_signals.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 11:51:32.000000 django-bulk-signals-0.3.0/django_bulk_signals.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      593 2023-04-28 11:51:32.715282 django-bulk-signals-0.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2346 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:36:03.402312 django-bulk-signals-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-04-29 19:36:01.000000 django-bulk-signals-0.4.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-04-29 19:36:00.000000 django-bulk-signals-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-29 19:36:00.000000 django-bulk-signals-0.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2707 2023-04-29 19:36:03.402312 django-bulk-signals-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-04-29 19:36:00.000000 django-bulk-signals-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:36:03.402312 django-bulk-signals-0.4.0/bulk_signals/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-29 19:36:01.000000 django-bulk-signals-0.4.0/bulk_signals/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2992 2023-04-29 19:36:00.000000 django-bulk-signals-0.4.0/bulk_signals/apps.py
+-rw-r--r--   0 root         (0) root         (0)      203 2023-04-29 19:36:00.000000 django-bulk-signals-0.4.0/bulk_signals/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:36:03.402312 django-bulk-signals-0.4.0/bulk_signals/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 19:36:00.000000 django-bulk-signals-0.4.0/bulk_signals/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      194 2023-04-29 19:36:00.000000 django-bulk-signals-0.4.0/bulk_signals/tests/apps.py
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-29 19:36:00.000000 django-bulk-signals-0.4.0/bulk_signals/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:36:03.402312 django-bulk-signals-0.4.0/bulk_signals/tests/migrations/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-29 19:36:00.000000 django-bulk-signals-0.4.0/bulk_signals/tests/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 19:36:00.000000 django-bulk-signals-0.4.0/bulk_signals/tests/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      887 2023-04-29 19:36:00.000000 django-bulk-signals-0.4.0/bulk_signals/tests/models.py
+-rw-r--r--   0 root         (0) root         (0)      298 2023-04-29 19:36:00.000000 django-bulk-signals-0.4.0/bulk_signals/tests/settings.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2023-04-29 19:36:00.000000 django-bulk-signals-0.4.0/bulk_signals/tests/test_skip.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2023-04-29 19:36:00.000000 django-bulk-signals-0.4.0/bulk_signals/tests/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 19:36:03.402312 django-bulk-signals-0.4.0/django_bulk_signals.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2707 2023-04-29 19:36:03.000000 django-bulk-signals-0.4.0/django_bulk_signals.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      642 2023-04-29 19:36:03.000000 django-bulk-signals-0.4.0/django_bulk_signals.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 19:36:03.000000 django-bulk-signals-0.4.0/django_bulk_signals.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-29 19:36:03.000000 django-bulk-signals-0.4.0/django_bulk_signals.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-29 19:36:03.000000 django-bulk-signals-0.4.0/django_bulk_signals.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      593 2023-04-29 19:36:03.402312 django-bulk-signals-0.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-04-29 19:36:00.000000 django-bulk-signals-0.4.0/setup.py
```

### Comparing `django-bulk-signals-0.3.0/CHANGELOG.md` & `django-bulk-signals-0.4.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.4.0 (2023-04-29)
+### Feature
+* Signals can be skipped by a keyword argument ([`894e0ec`](https://github.com/awmath/django-bulk-signals/commit/894e0ec69e4f73290085b0e9c0141a0bef19cf3d))
+
 ## v0.3.0 (2023-04-28)
 ### Feature
 * Post query update signal now passed the update count ([`e2424c9`](https://github.com/awmath/django-bulk-signals/commit/e2424c9a6033aab0164e94ff32c6699658291555))
 
 ## v0.2.1 (2022-12-07)
 ### Fix
 * Added missing tests module ([`9d4581c`](https://github.com/awmath/django-bulk-signals/commit/9d4581cbd0bc5a6f6d212e1ca796a1349dad2f79))
```

### Comparing `django-bulk-signals-0.3.0/LICENSE` & `django-bulk-signals-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-bulk-signals-0.3.0/PKG-INFO` & `django-bulk-signals-0.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bulk-signals
-Version: 0.3.0
+Version: 0.4.0
 Summary: A product aggregation function to a postgres database and makes it available with django
 Home-page: https://github.com/awmath/django-bulk-signals
 Download-URL: https://github.com/awmath/django-bulk-signals
 Author: Axel Wegener
 Author-email: pypi@sparse-space.de
 License: MIT
 Keywords: django
@@ -48,15 +48,18 @@
 ```
 Import signals and connect.The signals are connected the same way as in Django itself.
 To see them in action use the following snippet:
 ```
 from django.dispatch import receiver
 from bulk_signals import signals
 
-@receiver(signals.post_bulk_update, signals.post_bulk_update, signals.post_query_update)
+@receiver(signals.pre_bulk_update, signals.post_bulk_update, signals.post_query_update)
 def debug(*args, **kwargs):
     print(args)
     print(kwargs)
 ```
 
+You can skip the signals on a single execution by using the `skip_signal=True` keyword argument.
+Which keyword should be used for skipping is configurable via the `BULK_SIGNALS_SKIP_KEY="skip_signal"` configuration in the django settings.
+
 # TODO
 -  test against different database backends
```

### Comparing `django-bulk-signals-0.3.0/README.md` & `django-bulk-signals-0.4.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -19,15 +19,18 @@
 ```
 Import signals and connect.The signals are connected the same way as in Django itself.
 To see them in action use the following snippet:
 ```
 from django.dispatch import receiver
 from bulk_signals import signals
 
-@receiver(signals.post_bulk_update, signals.post_bulk_update, signals.post_query_update)
+@receiver(signals.pre_bulk_update, signals.post_bulk_update, signals.post_query_update)
 def debug(*args, **kwargs):
     print(args)
     print(kwargs)
 ```
 
+You can skip the signals on a single execution by using the `skip_signal=True` keyword argument.
+Which keyword should be used for skipping is configurable via the `BULK_SIGNALS_SKIP_KEY="skip_signal"` configuration in the django settings.
+
 # TODO
 -  test against different database backends
```

### Comparing `django-bulk-signals-0.3.0/bulk_signals/apps.py` & `django-bulk-signals-0.4.0/bulk_signals/apps.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,53 @@
 from django.apps import AppConfig, apps
+from django.conf import settings
 
 from bulk_signals import signals
 
 
+def skip_signal(kwargs):
+    skip_key = getattr(settings, "BULK_SIGNALS_SKIP_KEY", "skip_signal")
+    return kwargs.pop(skip_key, False) is True
+
+
 class BulkSignalsConfig(AppConfig):
     default_auto_field = "django.db.models.BigAutoField"
     name = "bulk_signals"
 
     def ready(self):
         # monkey patch bulk method handling into the queryset
         from django.db.models.query import QuerySet
 
         base_bulk_create = QuerySet.bulk_create
 
         def bulk_create(queryset, objects, **kwargs):
+            if skip_signal(kwargs):
+                return base_bulk_create(queryset, objects, **kwargs)
             # get model label from queryset
             model = apps.get_model(queryset.model._meta.label)
 
             signals.pre_bulk_create.send(sender=model, objects=objects, **kwargs)
             created_objects = base_bulk_create(queryset, objects, **kwargs)
             signals.post_bulk_create.send(sender=model, objects=objects, **kwargs)
 
             return created_objects
 
         QuerySet.bulk_create = bulk_create
 
         base_bulk_update = QuerySet.bulk_update
 
         def bulk_update(queryset, objects, fields, **kwargs):
+            # add a queryset hint so update signals won't be
+            # triggerd for bulk_update
             queryset._hints["is_bulk_update"] = True
+
+            # check if the signals should be skipped
+            if skip_signal(kwargs):
+                return base_bulk_update(queryset, objects, fields, **kwargs)
+
             model = apps.get_model(queryset.model._meta.label)
 
             signals.pre_bulk_update.send(
                 sender=model, objects=objects, fields=fields, **kwargs
             )
             return_value = base_bulk_update(queryset, objects, fields, **kwargs)
             signals.post_bulk_update.send(
@@ -42,14 +57,18 @@
             return return_value
 
         QuerySet.bulk_update = bulk_update
 
         base_update = QuerySet.update
 
         def update(queryset, **kwargs):
+            # check if the signals should be skipped
+            if skip_signal(kwargs):
+                return base_update(queryset, **kwargs)
+
             model = apps.get_model(queryset.model._meta.label)
 
             # if this update is part of a bulk_update action skip this part
             if queryset._hints.get("is_bulk_update", False):
                 return base_update(queryset, **kwargs)
 
             signals.pre_query_update.send(
```

### Comparing `django-bulk-signals-0.3.0/bulk_signals/tests/migrations/0001_initial.py` & `django-bulk-signals-0.4.0/bulk_signals/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-bulk-signals-0.3.0/bulk_signals/tests/models.py` & `django-bulk-signals-0.4.0/bulk_signals/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-bulk-signals-0.3.0/bulk_signals/tests/tests.py` & `django-bulk-signals-0.4.0/bulk_signals/tests/tests.py`

 * *Files identical despite different names*

### Comparing `django-bulk-signals-0.3.0/django_bulk_signals.egg-info/PKG-INFO` & `django-bulk-signals-0.4.0/django_bulk_signals.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bulk-signals
-Version: 0.3.0
+Version: 0.4.0
 Summary: A product aggregation function to a postgres database and makes it available with django
 Home-page: https://github.com/awmath/django-bulk-signals
 Download-URL: https://github.com/awmath/django-bulk-signals
 Author: Axel Wegener
 Author-email: pypi@sparse-space.de
 License: MIT
 Keywords: django
@@ -48,15 +48,18 @@
 ```
 Import signals and connect.The signals are connected the same way as in Django itself.
 To see them in action use the following snippet:
 ```
 from django.dispatch import receiver
 from bulk_signals import signals
 
-@receiver(signals.post_bulk_update, signals.post_bulk_update, signals.post_query_update)
+@receiver(signals.pre_bulk_update, signals.post_bulk_update, signals.post_query_update)
 def debug(*args, **kwargs):
     print(args)
     print(kwargs)
 ```
 
+You can skip the signals on a single execution by using the `skip_signal=True` keyword argument.
+Which keyword should be used for skipping is configurable via the `BULK_SIGNALS_SKIP_KEY="skip_signal"` configuration in the django settings.
+
 # TODO
 -  test against different database backends
```

### Comparing `django-bulk-signals-0.3.0/setup.cfg` & `django-bulk-signals-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-bulk-signals-0.3.0/setup.py` & `django-bulk-signals-0.4.0/setup.py`

 * *Files identical despite different names*


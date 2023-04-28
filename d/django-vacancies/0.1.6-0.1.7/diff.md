# Comparing `tmp/django-vacancies-0.1.6.tar.gz` & `tmp/django-vacancies-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-vacancies-0.1.6.tar", last modified: Wed Nov 27 03:47:49 2019, max compression
+gzip compressed data, was "django-vacancies-0.1.7.tar", last modified: Fri Apr 28 21:54:41 2023, max compression
```

## Comparing `django-vacancies-0.1.6.tar` & `django-vacancies-0.1.7.tar`

### file list

```diff
@@ -1,47 +1,43 @@
-drwxr-xr-x   0 contmp     (501) staff       (20)        0 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/
--rw-r--r--   0 contmp     (501) staff       (20)     1527 2019-11-26 22:05:40.000000 django-vacancies-0.1.6/LICENSE
--rw-r--r--   0 contmp     (501) staff       (20)      174 2019-11-26 22:59:19.000000 django-vacancies-0.1.6/MANIFEST.in
--rw-r--r--   0 contmp     (501) staff       (20)     4847 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/PKG-INFO
--rw-r--r--   0 contmp     (501) staff       (20)     2885 2019-11-27 03:37:24.000000 django-vacancies-0.1.6/README.md
-drwxr-xr-x   0 contmp     (501) staff       (20)        0 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/django_vacancies.egg-info/
--rw-r--r--   0 contmp     (501) staff       (20)     4847 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/django_vacancies.egg-info/PKG-INFO
--rw-r--r--   0 contmp     (501) staff       (20)      916 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/django_vacancies.egg-info/SOURCES.txt
--rw-r--r--   0 contmp     (501) staff       (20)        1 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/django_vacancies.egg-info/dependency_links.txt
--rw-r--r--   0 contmp     (501) staff       (20)       10 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/django_vacancies.egg-info/top_level.txt
-drwxr-xr-x   0 contmp     (501) staff       (20)        0 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/docs/
--rw-r--r--   0 contmp     (501) staff       (20)        0 2019-11-26 22:10:31.000000 django-vacancies-0.1.6/docs/.gitkeep
--rw-r--r--   0 contmp     (501) staff       (20)      884 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/setup.cfg
--rw-r--r--   0 contmp     (501) staff       (20)      261 2019-11-27 03:17:41.000000 django-vacancies-0.1.6/setup.py
-drwxr-xr-x   0 contmp     (501) staff       (20)        0 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/vacancies/
--rw-r--r--   0 contmp     (501) staff       (20)        0 2019-07-06 01:07:52.000000 django-vacancies-0.1.6/vacancies/__init__.py
--rw-r--r--   0 contmp     (501) staff       (20)     4496 2019-11-27 02:23:26.000000 django-vacancies-0.1.6/vacancies/admin.py
--rw-r--r--   0 contmp     (501) staff       (20)      214 2019-11-26 23:49:05.000000 django-vacancies-0.1.6/vacancies/apps.py
-drwxr-xr-x   0 contmp     (501) staff       (20)        0 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/vacancies/locale/
-drwxr-xr-x   0 contmp     (501) staff       (20)        0 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/vacancies/locale/de/
-drwxr-xr-x   0 contmp     (501) staff       (20)        0 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/vacancies/locale/de/LC_MESSAGES/
--rw-r--r--   0 contmp     (501) staff       (20)     4629 2019-11-27 02:55:54.000000 django-vacancies-0.1.6/vacancies/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 contmp     (501) staff       (20)     4592 2019-11-27 02:55:54.000000 django-vacancies-0.1.6/vacancies/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 contmp     (501) staff       (20)        0 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/vacancies/migrations/
--rw-r--r--   0 contmp     (501) staff       (20)     7847 2019-11-27 02:53:19.000000 django-vacancies-0.1.6/vacancies/migrations/0001_initial.py
--rw-r--r--   0 contmp     (501) staff       (20)        0 2019-07-06 01:07:52.000000 django-vacancies-0.1.6/vacancies/migrations/__init__.py
-drwxr-xr-x   0 contmp     (501) staff       (20)        0 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/vacancies/models/
--rw-r--r--   0 contmp     (501) staff       (20)      150 2019-11-27 01:23:40.000000 django-vacancies-0.1.6/vacancies/models/__init__.py
--rw-r--r--   0 contmp     (501) staff       (20)     1794 2019-11-27 01:40:54.000000 django-vacancies-0.1.6/vacancies/models/contact_person.py
--rw-r--r--   0 contmp     (501) staff       (20)      849 2019-11-27 01:36:27.000000 django-vacancies-0.1.6/vacancies/models/location.py
--rw-r--r--   0 contmp     (501) staff       (20)     5761 2019-11-27 03:46:43.000000 django-vacancies-0.1.6/vacancies/models/vacancy.py
-drwxr-xr-x   0 contmp     (501) staff       (20)        0 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/vacancies/static/
--rw-r--r--   0 contmp     (501) staff       (20)     6148 2019-11-27 00:03:58.000000 django-vacancies-0.1.6/vacancies/static/.DS_Store
-drwxr-xr-x   0 contmp     (501) staff       (20)        0 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/vacancies/static/vacancies/
--rw-r--r--   0 contmp     (501) staff       (20)     6148 2019-11-27 00:04:03.000000 django-vacancies-0.1.6/vacancies/static/vacancies/.DS_Store
-drwxr-xr-x   0 contmp     (501) staff       (20)        0 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/vacancies/static/vacancies/css/
--rw-r--r--   0 contmp     (501) staff       (20)      391 2019-11-27 01:00:28.000000 django-vacancies-0.1.6/vacancies/static/vacancies/css/admin.css
--rw-r--r--   0 contmp     (501) staff       (20)      782 2019-11-27 00:50:07.000000 django-vacancies-0.1.6/vacancies/storage.py
-drwxr-xr-x   0 contmp     (501) staff       (20)        0 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/vacancies/templates/
--rw-r--r--   0 contmp     (501) staff       (20)     6148 2019-11-27 01:57:23.000000 django-vacancies-0.1.6/vacancies/templates/.DS_Store
-drwxr-xr-x   0 contmp     (501) staff       (20)        0 2019-11-27 03:47:49.000000 django-vacancies-0.1.6/vacancies/templates/vacancies/
--rw-r--r--   0 contmp     (501) staff       (20)       26 2019-11-27 01:56:15.000000 django-vacancies-0.1.6/vacancies/templates/vacancies/vacancies_base.html
--rw-r--r--   0 contmp     (501) staff       (20)      223 2019-11-27 02:34:18.000000 django-vacancies-0.1.6/vacancies/templates/vacancies/vacancy_detail.html
--rw-r--r--   0 contmp     (501) staff       (20)      564 2019-11-27 03:38:37.000000 django-vacancies-0.1.6/vacancies/templates/vacancies/vacancy_list.html
--rw-r--r--   0 contmp     (501) staff       (20)      269 2019-11-27 03:46:31.000000 django-vacancies-0.1.6/vacancies/urls.py
--rw-r--r--   0 contmp     (501) staff       (20)      362 2019-11-27 02:38:31.000000 django-vacancies-0.1.6/vacancies/utils.py
--rw-r--r--   0 contmp     (501) staff       (20)      374 2019-11-27 02:32:58.000000 django-vacancies-0.1.6/vacancies/views.py
+drwxr-xr-x   0 contmp     (501) staff       (20)        0 2023-04-28 21:54:41.021076 django-vacancies-0.1.7/
+-rw-r--r--   0 contmp     (501) staff       (20)     1527 2020-08-24 21:38:01.000000 django-vacancies-0.1.7/LICENSE
+-rw-r--r--   0 contmp     (501) staff       (20)      174 2020-08-24 21:38:01.000000 django-vacancies-0.1.7/MANIFEST.in
+-rw-r--r--   0 contmp     (501) staff       (20)     3865 2023-04-28 21:54:41.021170 django-vacancies-0.1.7/PKG-INFO
+-rw-r--r--   0 contmp     (501) staff       (20)     2904 2023-04-28 21:54:24.000000 django-vacancies-0.1.7/README.md
+drwxr-xr-x   0 contmp     (501) staff       (20)        0 2023-04-28 21:54:41.016051 django-vacancies-0.1.7/django_vacancies.egg-info/
+-rw-r--r--   0 contmp     (501) staff       (20)     3865 2023-04-28 21:54:41.000000 django-vacancies-0.1.7/django_vacancies.egg-info/PKG-INFO
+-rw-r--r--   0 contmp     (501) staff       (20)      780 2023-04-28 21:54:41.000000 django-vacancies-0.1.7/django_vacancies.egg-info/SOURCES.txt
+-rw-r--r--   0 contmp     (501) staff       (20)        1 2023-04-28 21:54:41.000000 django-vacancies-0.1.7/django_vacancies.egg-info/dependency_links.txt
+-rw-r--r--   0 contmp     (501) staff       (20)       10 2023-04-28 21:54:41.000000 django-vacancies-0.1.7/django_vacancies.egg-info/top_level.txt
+drwxr-xr-x   0 contmp     (501) staff       (20)        0 2023-04-28 21:54:41.016252 django-vacancies-0.1.7/docs/
+-rw-r--r--   0 contmp     (501) staff       (20)        0 2020-08-24 21:38:01.000000 django-vacancies-0.1.7/docs/.gitkeep
+-rw-r--r--   0 contmp     (501) staff       (20)      884 2023-04-28 21:54:41.021777 django-vacancies-0.1.7/setup.cfg
+-rw-r--r--   0 contmp     (501) staff       (20)      261 2020-08-24 21:38:01.000000 django-vacancies-0.1.7/setup.py
+drwxr-xr-x   0 contmp     (501) staff       (20)        0 2023-04-28 21:54:41.018309 django-vacancies-0.1.7/vacancies/
+-rw-r--r--   0 contmp     (501) staff       (20)        0 2020-08-24 21:38:01.000000 django-vacancies-0.1.7/vacancies/__init__.py
+-rw-r--r--   0 contmp     (501) staff       (20)     4470 2023-04-28 21:52:16.000000 django-vacancies-0.1.7/vacancies/admin.py
+-rw-r--r--   0 contmp     (501) staff       (20)      189 2023-04-28 21:52:12.000000 django-vacancies-0.1.7/vacancies/apps.py
+drwxr-xr-x   0 contmp     (501) staff       (20)        0 2023-04-28 21:54:41.013389 django-vacancies-0.1.7/vacancies/locale/
+drwxr-xr-x   0 contmp     (501) staff       (20)        0 2023-04-28 21:54:41.013457 django-vacancies-0.1.7/vacancies/locale/de/
+drwxr-xr-x   0 contmp     (501) staff       (20)        0 2023-04-28 21:54:41.018663 django-vacancies-0.1.7/vacancies/locale/de/LC_MESSAGES/
+-rw-r--r--   0 contmp     (501) staff       (20)     4592 2020-08-24 21:38:01.000000 django-vacancies-0.1.7/vacancies/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 contmp     (501) staff       (20)        0 2023-04-28 21:54:41.019145 django-vacancies-0.1.7/vacancies/migrations/
+-rw-r--r--   0 contmp     (501) staff       (20)     7847 2020-08-24 21:38:01.000000 django-vacancies-0.1.7/vacancies/migrations/0001_initial.py
+-rw-r--r--   0 contmp     (501) staff       (20)        0 2020-08-24 21:38:01.000000 django-vacancies-0.1.7/vacancies/migrations/__init__.py
+drwxr-xr-x   0 contmp     (501) staff       (20)        0 2023-04-28 21:54:41.020000 django-vacancies-0.1.7/vacancies/models/
+-rw-r--r--   0 contmp     (501) staff       (20)      126 2023-04-28 21:52:27.000000 django-vacancies-0.1.7/vacancies/models/__init__.py
+-rw-r--r--   0 contmp     (501) staff       (20)     1768 2023-04-28 21:52:06.000000 django-vacancies-0.1.7/vacancies/models/contact_person.py
+-rw-r--r--   0 contmp     (501) staff       (20)      824 2023-04-28 21:52:01.000000 django-vacancies-0.1.7/vacancies/models/location.py
+-rw-r--r--   0 contmp     (501) staff       (20)     5735 2023-04-28 21:51:46.000000 django-vacancies-0.1.7/vacancies/models/vacancy.py
+drwxr-xr-x   0 contmp     (501) staff       (20)        0 2023-04-28 21:54:41.013846 django-vacancies-0.1.7/vacancies/static/
+drwxr-xr-x   0 contmp     (501) staff       (20)        0 2023-04-28 21:54:41.013911 django-vacancies-0.1.7/vacancies/static/vacancies/
+drwxr-xr-x   0 contmp     (501) staff       (20)        0 2023-04-28 21:54:41.020288 django-vacancies-0.1.7/vacancies/static/vacancies/css/
+-rw-r--r--   0 contmp     (501) staff       (20)      391 2020-08-24 21:38:01.000000 django-vacancies-0.1.7/vacancies/static/vacancies/css/admin.css
+-rw-r--r--   0 contmp     (501) staff       (20)      759 2023-04-28 21:52:33.000000 django-vacancies-0.1.7/vacancies/storage.py
+drwxr-xr-x   0 contmp     (501) staff       (20)        0 2023-04-28 21:54:41.014093 django-vacancies-0.1.7/vacancies/templates/
+drwxr-xr-x   0 contmp     (501) staff       (20)        0 2023-04-28 21:54:41.020888 django-vacancies-0.1.7/vacancies/templates/vacancies/
+-rw-r--r--   0 contmp     (501) staff       (20)       26 2020-08-24 21:38:01.000000 django-vacancies-0.1.7/vacancies/templates/vacancies/vacancies_base.html
+-rw-r--r--   0 contmp     (501) staff       (20)      223 2020-08-24 21:38:01.000000 django-vacancies-0.1.7/vacancies/templates/vacancies/vacancy_detail.html
+-rw-r--r--   0 contmp     (501) staff       (20)      564 2020-08-24 21:38:01.000000 django-vacancies-0.1.7/vacancies/templates/vacancies/vacancy_list.html
+-rw-r--r--   0 contmp     (501) staff       (20)      244 2023-04-28 21:52:31.000000 django-vacancies-0.1.7/vacancies/urls.py
+-rw-r--r--   0 contmp     (501) staff       (20)      338 2023-04-28 21:52:30.000000 django-vacancies-0.1.7/vacancies/utils.py
+-rw-r--r--   0 contmp     (501) staff       (20)      350 2023-04-28 21:52:28.000000 django-vacancies-0.1.7/vacancies/views.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-vacancies-0.1.6/LICENSE` & `django-vacancies-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-vacancies-0.1.6/README.md` & `django-vacancies-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 # Use Po-Edit or other editor to edit locales
 ```
 
 ### Package and Install Development Version
 
 ```sh
 # Inside cloned repository folder:
+# Adjust setup.cfg
 python setup.py sdist
 
 # Inside Dev Project Apps Dir:
 ln -s  ../../django-vacancies/vacancies
 
 # Or:
 pip install --user django-vacancies/dist/django-vacancies-0.1.tar.gz
```

### Comparing `django-vacancies-0.1.6/setup.cfg` & `django-vacancies-0.1.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-vacancies
-version = 0.1.6
+version = 0.1.7
 description = A Django app to publish Web-based vacancies.
 long_description = file: README.rst
 url = https://github.com/contmp/django-vacancies
 author = Bastian Probian
 author_email = contmp@me.com
 license = BSD-3-Clause
 classifiers =
```

### Comparing `django-vacancies-0.1.6/vacancies/admin.py` & `django-vacancies-0.1.7/vacancies/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-# -*- coding: utf-8 -*-
 from django.contrib import admin
 from django.utils.safestring import mark_safe
-from django.utils.translation import ugettext_lazy as _
-
+from django.utils.translation import gettext_lazy as _
 from vacancies.models import ContactPerson, Location, Vacancy
 
 
 @admin.register(Vacancy)
 class VacancyAdmin(admin.ModelAdmin):
 
     save_as = True
```

### Comparing `django-vacancies-0.1.6/vacancies/locale/de/LC_MESSAGES/django.po` & `django-vacancies-0.1.7/vacancies/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-vacancies-0.1.6/vacancies/migrations/0001_initial.py` & `django-vacancies-0.1.7/vacancies/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-vacancies-0.1.6/vacancies/models/contact_person.py` & `django-vacancies-0.1.7/vacancies/models/contact_person.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# -*- coding: utf-8 -*-
 from django.db import models
-from django.utils.translation import ugettext_lazy as _
-
+from django.utils.translation import gettext_lazy as _
 from vacancies.storage import contact_person_image
 
 
 class ContactPerson(models.Model):
 
     SALUTATION_MRS = 1
     SALUTATION_MR = 2
```

### Comparing `django-vacancies-0.1.6/vacancies/models/location.py` & `django-vacancies-0.1.7/vacancies/models/location.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 from django.db import models
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
 class Location(models.Model):
 
     label = models.CharField(max_length=255, blank=True, verbose_name=_('Label'))
     city = models.CharField(max_length=100, verbose_name=_('City'))
     country = models.CharField(max_length=100, blank=True, verbose_name=_('Country'))
```

### Comparing `django-vacancies-0.1.6/vacancies/models/vacancy.py` & `django-vacancies-0.1.7/vacancies/models/vacancy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# -*- coding: utf-8 -*-
 from django.core.validators import FileExtensionValidator
 from django.db import models
 from django.urls import reverse
-from django.utils.translation import ugettext_lazy as _
-
-from vacancies.storage import vacancy_pdf, vacancy_image
+from django.utils.translation import gettext_lazy as _
+from vacancies.storage import vacancy_image, vacancy_pdf
 from vacancies.utils import generate_unique_slug
 
 
 class Vacancy(models.Model):
 
     MANAGEMENT_RESPONSIBILITY_NONE = 1
     MANAGEMENT_RESPONSIBILITY_ALL = 2
```

### Comparing `django-vacancies-0.1.6/vacancies/storage.py` & `django-vacancies-0.1.7/vacancies/storage.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# -*- coding: utf-8 -*-
-import os
 import hashlib
+import os
+
 from django.utils.text import slugify
 
 
 def contact_person_image(instance, filename):
     _, ext = os.path.splitext(filename)
     uu = hashlib.md5(instance.image.read()).hexdigest()
     return '/'.join(['vacancies', 'contact_persons', uu[:2], uu[2:4], uu, slugify(instance.full_name) + ext.lower()])
```

### Comparing `django-vacancies-0.1.6/vacancies/templates/vacancies/vacancy_list.html` & `django-vacancies-0.1.7/vacancies/templates/vacancies/vacancy_list.html`

 * *Files identical despite different names*


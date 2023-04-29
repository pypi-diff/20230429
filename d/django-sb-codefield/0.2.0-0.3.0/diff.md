# Comparing `tmp/django_sb_codefield-0.2.0.tar.gz` & `tmp/django_sb_codefield-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_sb_codefield-0.2.0.tar", max compression
+gzip compressed data, was "django_sb_codefield-0.3.0.tar", max compression
```

## Comparing `django_sb_codefield-0.2.0.tar` & `django_sb_codefield-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      473 2023-04-29 10:13:48.473281 django_sb_codefield-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-04-29 07:54:22.661525 django_sb_codefield-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1650 2023-04-29 10:13:14.169168 django_sb_codefield-0.2.0/README.md
--rw-r--r--   0        0        0     1961 2023-04-29 10:13:48.469280 django_sb_codefield-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      208 2023-04-29 07:54:22.665525 django_sb_codefield-0.2.0/src/django_sb_codefield/__init__.py
--rw-r--r--   0        0        0      433 2023-04-29 07:54:22.665525 django_sb_codefield-0.2.0/src/django_sb_codefield/admin.py
--rw-r--r--   0        0        0      168 2023-04-29 07:54:22.665525 django_sb_codefield-0.2.0/src/django_sb_codefield/apps.py
--rw-r--r--   0        0        0     1368 2023-04-29 07:54:22.665525 django_sb_codefield-0.2.0/src/django_sb_codefield/fields.py
--rw-r--r--   0        0        0        0 2023-04-29 07:54:22.665525 django_sb_codefield-0.2.0/src/django_sb_codefield/models.py
--rw-r--r--   0        0        0      291 2023-04-29 07:54:22.665525 django_sb_codefield-0.2.0/src/django_sb_codefield/static/django_sb_codefield/css/codefield_django_admin.css
--rw-r--r--   0        0        0        0 2023-04-29 07:54:22.665525 django_sb_codefield-0.2.0/src/django_sb_codefield/tests.py
--rw-r--r--   0        0        0       20 2023-04-29 10:13:48.477280 django_sb_codefield-0.2.0/src/django_sb_codefield/version.py
--rw-r--r--   0        0        0        0 2023-04-29 07:54:22.665525 django_sb_codefield-0.2.0/src/django_sb_codefield/views.py
--rw-r--r--   0        0        0     3226 1970-01-01 00:00:00.000000 django_sb_codefield-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      559 2023-04-29 10:28:03.964476 django_sb_codefield-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-04-29 07:54:22.661525 django_sb_codefield-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1650 2023-04-29 10:24:51.943718 django_sb_codefield-0.3.0/README.md
+-rw-r--r--   0        0        0     2016 2023-04-29 10:28:03.960476 django_sb_codefield-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      208 2023-04-29 07:54:22.665525 django_sb_codefield-0.3.0/src/django_sb_codefield/__init__.py
+-rw-r--r--   0        0        0      433 2023-04-29 07:54:22.665525 django_sb_codefield-0.3.0/src/django_sb_codefield/admin.py
+-rw-r--r--   0        0        0      168 2023-04-29 07:54:22.665525 django_sb_codefield-0.3.0/src/django_sb_codefield/apps.py
+-rw-r--r--   0        0        0     1368 2023-04-29 07:54:22.665525 django_sb_codefield-0.3.0/src/django_sb_codefield/fields.py
+-rw-r--r--   0        0        0        0 2023-04-29 07:54:22.665525 django_sb_codefield-0.3.0/src/django_sb_codefield/models.py
+-rw-r--r--   0        0        0      291 2023-04-29 07:54:22.665525 django_sb_codefield-0.3.0/src/django_sb_codefield/static/django_sb_codefield/css/codefield_django_admin.css
+-rw-r--r--   0        0        0        0 2023-04-29 07:54:22.665525 django_sb_codefield-0.3.0/src/django_sb_codefield/tests.py
+-rw-r--r--   0        0        0       20 2023-04-29 10:28:03.968476 django_sb_codefield-0.3.0/src/django_sb_codefield/version.py
+-rw-r--r--   0        0        0        0 2023-04-29 07:54:22.665525 django_sb_codefield-0.3.0/src/django_sb_codefield/views.py
+-rw-r--r--   0        0        0     3281 1970-01-01 00:00:00.000000 django_sb_codefield-0.3.0/PKG-INFO
```

### Comparing `django_sb_codefield-0.2.0/LICENSE.txt` & `django_sb_codefield-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_sb_codefield-0.2.0/README.md` & `django_sb_codefield-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django_sb_codefield-0.2.0/pyproject.toml` & `django_sb_codefield-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-sb-codefield"
-version = "0.2.0"
+version = "0.3.0"
 description = "Use codemirror2 widget directly in Django models, forms and admin."
 authors = [
   "SoftButterfly Development Team <dev@softbutterfly.io>",
   "zodiacfireworks <martin.vuelta@gmail.com>"
 ]
 license = "MIT License"
 readme = "README.md"
@@ -29,16 +29,16 @@
 ]
 include = [
   "LICENSE.txt",
   "CHANGELOG.md",
 ]
 
 [tool.poetry.urls]
-"Download" = "https://github.com/softbutterfly/django-sb-codefield/archive/v0.2.0.tar.gz"
-"Bug Tracker" = "https://github.com/softbutterfly/django-sb-codefield/issues"
+"Download" = "https://gitlab.com/softbutterfly/open-source/django-sb-codefield/-/archive/v0.3.0/django-sb-codefield-v0.3.0.tar.gz"
+"Bug Tracker" = "https://gitlab.com/softbutterfly/open-source/django-sb-codefield/-/issues"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 Django = "<5.0.0"
 django-codemirror2 = "<1.0.0"
```

### Comparing `django_sb_codefield-0.2.0/src/django_sb_codefield/fields.py` & `django_sb_codefield-0.3.0/src/django_sb_codefield/fields.py`

 * *Files identical despite different names*

### Comparing `django_sb_codefield-0.2.0/PKG-INFO` & `django_sb_codefield-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sb-codefield
-Version: 0.2.0
+Version: 0.3.0
 Summary: Use codemirror2 widget directly in Django models, forms and admin.
 Home-page: https://gitlab.com/softbutterfly/open-source/django-sb-codefield
 License: MIT
 Keywords: Softbutterfly,Django,Migrations
 Author: SoftButterfly Development Team
 Author-email: dev@softbutterfly.io
 Requires-Python: >=3.8.1,<4.0.0
@@ -20,17 +20,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Django (<5.0.0)
 Requires-Dist: django-codemirror2 (<1.0.0)
-Project-URL: Bug Tracker, https://github.com/softbutterfly/django-sb-codefield/issues
+Project-URL: Bug Tracker, https://gitlab.com/softbutterfly/open-source/django-sb-codefield/-/issues
 Project-URL: Documentation, https://gitlab.com/softbutterfly/open-source/django-sb-codefield/-/wikis
-Project-URL: Download, https://github.com/softbutterfly/django-sb-codefield/archive/v0.2.0.tar.gz
+Project-URL: Download, https://gitlab.com/softbutterfly/open-source/django-sb-codefield/-/archive/v0.3.0/django-sb-codefield-v0.3.0.tar.gz
 Project-URL: Repository, https://gitlab.com/softbutterfly/open-source/django-sb-codefield
 Description-Content-Type: text/markdown
 
 ![Community-Project](https://gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/softbutterfly-open-source--banner--community-project.png)
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/django-sb-codefield)
 ![PyPI - Package version](https://img.shields.io/pypi/v/django-sb-codefield)
```


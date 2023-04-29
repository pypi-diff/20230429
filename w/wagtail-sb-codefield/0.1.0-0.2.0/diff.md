# Comparing `tmp/wagtail_sb_codefield-0.1.0.tar.gz` & `tmp/wagtail_sb_codefield-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_sb_codefield-0.1.0.tar", max compression
+gzip compressed data, was "wagtail_sb_codefield-0.2.0.tar", max compression
```

## Comparing `wagtail_sb_codefield-0.1.0.tar` & `wagtail_sb_codefield-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      111 2023-04-29 09:59:18.721762 wagtail_sb_codefield-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-04-29 09:12:41.546419 wagtail_sb_codefield-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1797 2023-04-29 09:47:48.483148 wagtail_sb_codefield-0.1.0/README.md
--rw-r--r--   0        0        0     1963 2023-04-29 09:59:18.717761 wagtail_sb_codefield-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      210 2023-04-29 09:19:46.460483 wagtail_sb_codefield-0.1.0/src/wagtail_sb_codefield/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 09:20:00.996552 wagtail_sb_codefield-0.1.0/src/wagtail_sb_codefield/admin.py
--rw-r--r--   0        0        0      170 2023-04-29 09:16:21.703499 wagtail_sb_codefield-0.1.0/src/wagtail_sb_codefield/apps.py
--rw-r--r--   0        0        0      567 2023-04-29 09:52:32.684169 wagtail_sb_codefield-0.1.0/src/wagtail_sb_codefield/fields.py
--rw-r--r--   0        0        0        0 2023-04-29 09:16:21.223497 wagtail_sb_codefield-0.1.0/src/wagtail_sb_codefield/migrations/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 09:20:05.336573 wagtail_sb_codefield-0.1.0/src/wagtail_sb_codefield/models.py
--rw-r--r--   0        0        0      271 2023-04-29 09:30:01.355376 wagtail_sb_codefield-0.1.0/src/wagtail_sb_codefield/static/wagtail_sb_codefield/css/codefield_wagtail_admin.css
--rw-r--r--   0        0        0     1114 2023-04-29 09:25:32.806120 wagtail_sb_codefield-0.1.0/src/wagtail_sb_codefield/templates/wagtail_sb_codefield/wagtail_tabbed_interface_script.html
--rw-r--r--   0        0        0        0 2023-04-29 09:20:08.296587 wagtail_sb_codefield-0.1.0/src/wagtail_sb_codefield/tests.py
--rw-r--r--   0        0        0       20 2023-04-29 09:59:18.725762 wagtail_sb_codefield-0.1.0/src/wagtail_sb_codefield/version.py
--rw-r--r--   0        0        0        0 2023-04-29 09:20:11.572603 wagtail_sb_codefield-0.1.0/src/wagtail_sb_codefield/views.py
--rw-r--r--   0        0        0      331 2023-04-29 09:30:55.599629 wagtail_sb_codefield-0.1.0/src/wagtail_sb_codefield/wagtail_hooks.py
--rw-r--r--   0        0        0     3364 1970-01-01 00:00:00.000000 wagtail_sb_codefield-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      232 2023-04-29 10:31:54.817403 wagtail_sb_codefield-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-04-29 10:00:37.442081 wagtail_sb_codefield-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1797 2023-04-29 10:18:24.674246 wagtail_sb_codefield-0.2.0/README.md
+-rw-r--r--   0        0        0     1990 2023-04-29 10:31:54.813403 wagtail_sb_codefield-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      210 2023-04-29 10:00:37.450081 wagtail_sb_codefield-0.2.0/src/wagtail_sb_codefield/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 10:00:37.450081 wagtail_sb_codefield-0.2.0/src/wagtail_sb_codefield/admin.py
+-rw-r--r--   0        0        0      170 2023-04-29 10:00:37.450081 wagtail_sb_codefield-0.2.0/src/wagtail_sb_codefield/apps.py
+-rw-r--r--   0        0        0      567 2023-04-29 10:00:37.450081 wagtail_sb_codefield-0.2.0/src/wagtail_sb_codefield/fields.py
+-rw-r--r--   0        0        0        0 2023-04-29 10:00:37.450081 wagtail_sb_codefield-0.2.0/src/wagtail_sb_codefield/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 10:00:37.450081 wagtail_sb_codefield-0.2.0/src/wagtail_sb_codefield/models.py
+-rw-r--r--   0        0        0      271 2023-04-29 10:00:37.450081 wagtail_sb_codefield-0.2.0/src/wagtail_sb_codefield/static/wagtail_sb_codefield/css/codefield_wagtail_admin.css
+-rw-r--r--   0        0        0     1114 2023-04-29 10:00:37.450081 wagtail_sb_codefield-0.2.0/src/wagtail_sb_codefield/templates/wagtail_sb_codefield/wagtail_tabbed_interface_script.html
+-rw-r--r--   0        0        0        0 2023-04-29 10:00:37.450081 wagtail_sb_codefield-0.2.0/src/wagtail_sb_codefield/tests.py
+-rw-r--r--   0        0        0       20 2023-04-29 10:31:54.821403 wagtail_sb_codefield-0.2.0/src/wagtail_sb_codefield/version.py
+-rw-r--r--   0        0        0        0 2023-04-29 10:00:37.450081 wagtail_sb_codefield-0.2.0/src/wagtail_sb_codefield/views.py
+-rw-r--r--   0        0        0      331 2023-04-29 10:00:37.450081 wagtail_sb_codefield-0.2.0/src/wagtail_sb_codefield/wagtail_hooks.py
+-rw-r--r--   0        0        0     3399 1970-01-01 00:00:00.000000 wagtail_sb_codefield-0.2.0/PKG-INFO
```

### Comparing `wagtail_sb_codefield-0.1.0/LICENSE.txt` & `wagtail_sb_codefield-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail_sb_codefield-0.1.0/README.md` & `wagtail_sb_codefield-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/wagtail-sb-codefield)
 ![PyPI - Package version](https://img.shields.io/pypi/v/wagtail-sb-codefield)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/wagtail-sb-codefield)
 ![PyPI - MIT License](https://img.shields.io/pypi/l/wagtail-sb-codefield)
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/2f6661a360234960b1800c0bdac37d3c)](https://app.codacy.com/gl/softbutterfly/wagtail-sb-codefield/dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 
-# Wagtail Codefield
+# Wagtail CodeField
 
 Use CodeField from [`django-sb-codefield`](https://gitlab.com/softbutterfly/open-source/django-sb-codefield) in Wagtail Admin
 
 ## Requirements
 
 - Python 3.8.1 or higher but lower than 4.0.0
 - Django lower than 4.0.0
```

### Comparing `wagtail_sb_codefield-0.1.0/pyproject.toml` & `wagtail_sb_codefield-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "wagtail-sb-codefield"
-version = "0.1.0"
-description = "FontAwesome for Wagtail Admin."
+version = "0.2.0"
+description = "Use CodeField from `django-sb-codefield` in Wagtail Admin"
 authors = [
   "SoftButterfly Development Team <dev@softbutterfly.io>",
   "zodiacfireworks <martin.vuelta@gmail.com>"
 ]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-codefield"
@@ -28,21 +28,21 @@
 ]
 include = [
   "LICENSE.txt",
   "CHANGELOG.md",
 ]
 
 [tool.poetry.urls]
-"Download" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-codefield/-/archive/v0.1.0/wagtail-sb-codefield-v0.1.0.tar.gz"
+"Download" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-codefield/-/archive/v0.2.0/wagtail-sb-codefield-v0.2.0.tar.gz"
 "Bug Tracker" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-codefield/-/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 django = "< 5.0"
-django_sb_codefield = "<1.0.0"
+django-sb-codefield = "^0.1.0"
 wagtail = "< 5.0"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.1"
 bandit = "^1.7.4"
 black = "^23.1.0"
 coverage = "^7.1.0"
```

### Comparing `wagtail_sb_codefield-0.1.0/src/wagtail_sb_codefield/fields.py` & `wagtail_sb_codefield-0.2.0/src/wagtail_sb_codefield/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_codefield-0.1.0/src/wagtail_sb_codefield/templates/wagtail_sb_codefield/wagtail_tabbed_interface_script.html` & `wagtail_sb_codefield-0.2.0/src/wagtail_sb_codefield/templates/wagtail_sb_codefield/wagtail_tabbed_interface_script.html`

 * *Files identical despite different names*

### Comparing `wagtail_sb_codefield-0.1.0/PKG-INFO` & `wagtail_sb_codefield-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: wagtail-sb-codefield
-Version: 0.1.0
-Summary: FontAwesome for Wagtail Admin.
+Version: 0.2.0
+Summary: Use CodeField from `django-sb-codefield` in Wagtail Admin
 Home-page: https://gitlab.com/softbutterfly/open-source/wagtail-sb-codefield
 License: MIT
 Keywords: Softbutterfly,Django,Migrations
 Author: SoftButterfly Development Team
 Author-email: dev@softbutterfly.io
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
@@ -18,32 +18,32 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: django (<5.0)
-Requires-Dist: django_sb_codefield (<1.0.0)
+Requires-Dist: django-sb-codefield (>=0.1.0,<0.2.0)
 Requires-Dist: wagtail (<5.0)
 Project-URL: Bug Tracker, https://gitlab.com/softbutterfly/open-source/wagtail-sb-codefield/-/issues
 Project-URL: Documentation, https://gitlab.com/softbutterfly/open-source/wagtail-sb-codefield/-/wikis
-Project-URL: Download, https://gitlab.com/softbutterfly/open-source/wagtail-sb-codefield/-/archive/v0.1.0/wagtail-sb-codefield-v0.1.0.tar.gz
+Project-URL: Download, https://gitlab.com/softbutterfly/open-source/wagtail-sb-codefield/-/archive/v0.2.0/wagtail-sb-codefield-v0.2.0.tar.gz
 Project-URL: Repository, https://gitlab.com/softbutterfly/open-source/wagtail-sb-codefield
 Description-Content-Type: text/markdown
 
 ![Community-Project](https://gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/softbutterfly-open-source--banner--community-project.png)
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/wagtail-sb-codefield)
 ![PyPI - Package version](https://img.shields.io/pypi/v/wagtail-sb-codefield)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/wagtail-sb-codefield)
 ![PyPI - MIT License](https://img.shields.io/pypi/l/wagtail-sb-codefield)
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/2f6661a360234960b1800c0bdac37d3c)](https://app.codacy.com/gl/softbutterfly/wagtail-sb-codefield/dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 
-# Wagtail Codefield
+# Wagtail CodeField
 
 Use CodeField from [`django-sb-codefield`](https://gitlab.com/softbutterfly/open-source/django-sb-codefield) in Wagtail Admin
 
 ## Requirements
 
 - Python 3.8.1 or higher but lower than 4.0.0
 - Django lower than 4.0.0
```


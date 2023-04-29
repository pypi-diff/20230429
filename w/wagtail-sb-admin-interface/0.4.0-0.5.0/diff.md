# Comparing `tmp/wagtail_sb_admin_interface-0.4.0.tar.gz` & `tmp/wagtail_sb_admin_interface-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_sb_admin_interface-0.4.0.tar", max compression
+gzip compressed data, was "wagtail_sb_admin_interface-0.5.0.tar", max compression
```

## Comparing `wagtail_sb_admin_interface-0.4.0.tar` & `wagtail_sb_admin_interface-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      562 2023-04-15 07:12:58.612149 wagtail_sb_admin_interface-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-02-22 19:43:45.772297 wagtail_sb_admin_interface-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     1915 2023-04-15 07:11:11.123751 wagtail_sb_admin_interface-0.4.0/README.md
--rw-r--r--   0        0        0     2056 2023-04-15 07:12:58.612149 wagtail_sb_admin_interface-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      216 2023-02-22 22:54:53.731936 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/__init__.py
--rw-r--r--   0        0        0     4840 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/admin.py
--rw-r--r--   0        0        0      716 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/apps.py
--rw-r--r--   0        0        0      533 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/cache.py
--rw-r--r--   0        0        0      336 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/compat.py
--rw-r--r--   0        0        0     6472 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0001_initial.py
--rw-r--r--   0        0        0     3602 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0002_remove_theme_color_input_focus_and_more.py
--rw-r--r--   0        0        0      389 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0003_remove_theme_sidebar_logo_background_color.py
--rw-r--r--   0        0        0     2040 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0004_alter_theme_color_critical_alter_theme_color_info_and_more.py
--rw-r--r--   0        0        0      484 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0005_rename_sidebar_logo_mobile_theme_sidebar_logo_collapsed.py
--rw-r--r--   0        0        0      606 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0006_theme_sidebar_logo_background_color.py
--rw-r--r--   0        0        0        0 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/__init__.py
--rw-r--r--   0        0        0     8365 2023-02-23 01:02:30.680771 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/models.py
--rw-r--r--   0        0        0     1192 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/settings.py
--rw-r--r--   0        0        0     2798 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/templates/wagtailadmin/base.html
--rw-r--r--   0        0        0        0 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/templatetags/__init__.py
--rw-r--r--   0        0        0     2783 2023-02-22 22:55:26.220082 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/templatetags/wagtail_sb_admin_interface_tags.py
--rw-r--r--   0        0        0        0 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/tests.py
--rw-r--r--   0        0        0       20 2023-04-15 07:12:58.616149 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/version.py
--rw-r--r--   0        0        0        0 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/views.py
--rw-r--r--   0        0        0      817 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/wagtail_hooks.py
--rw-r--r--   0        0        0     3582 1970-01-01 00:00:00.000000 wagtail_sb_admin_interface-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      635 2023-04-29 16:26:38.725693 wagtail_sb_admin_interface-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-02-22 19:43:45.772297 wagtail_sb_admin_interface-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1915 2023-04-15 07:13:49.292338 wagtail_sb_admin_interface-0.5.0/README.md
+-rw-r--r--   0        0        0     2073 2023-04-29 16:26:38.721693 wagtail_sb_admin_interface-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      216 2023-02-22 22:54:53.731936 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/__init__.py
+-rw-r--r--   0        0        0     4840 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/admin.py
+-rw-r--r--   0        0        0      716 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/apps.py
+-rw-r--r--   0        0        0      533 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/cache.py
+-rw-r--r--   0        0        0      336 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/compat.py
+-rw-r--r--   0        0        0     6472 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/migrations/0001_initial.py
+-rw-r--r--   0        0        0     3602 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/migrations/0002_remove_theme_color_input_focus_and_more.py
+-rw-r--r--   0        0        0      389 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/migrations/0003_remove_theme_sidebar_logo_background_color.py
+-rw-r--r--   0        0        0     2040 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/migrations/0004_alter_theme_color_critical_alter_theme_color_info_and_more.py
+-rw-r--r--   0        0        0      484 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/migrations/0005_rename_sidebar_logo_mobile_theme_sidebar_logo_collapsed.py
+-rw-r--r--   0        0        0      606 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/migrations/0006_theme_sidebar_logo_background_color.py
+-rw-r--r--   0        0        0        0 2023-02-22 19:34:33.937823 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/migrations/__init__.py
+-rw-r--r--   0        0        0     8365 2023-02-23 01:02:30.680771 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/models.py
+-rw-r--r--   0        0        0     1192 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/settings.py
+-rw-r--r--   0        0        0     2798 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/templates/wagtailadmin/base.html
+-rw-r--r--   0        0        0        0 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/templatetags/__init__.py
+-rw-r--r--   0        0        0     2783 2023-02-22 22:55:26.220082 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/templatetags/wagtail_sb_admin_interface_tags.py
+-rw-r--r--   0        0        0        0 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/tests.py
+-rw-r--r--   0        0        0       20 2023-04-29 16:26:38.725693 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/version.py
+-rw-r--r--   0        0        0        0 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/views.py
+-rw-r--r--   0        0        0      817 2023-02-22 19:34:33.945823 wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/wagtail_hooks.py
+-rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 wagtail_sb_admin_interface-0.5.0/PKG-INFO
```

### Comparing `wagtail_sb_admin_interface-0.4.0/CHANGELOG.md` & `wagtail_sb_admin_interface-0.5.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 ## [Unreleased]
 
+## [0.5.0] - 2023-04-29
+
+* Update package description in pyproject.toml
+
 ## [0.4.0] - 2023-04-15
 
 * Remove codecov from development requirements
 * Add wagtail_sb_fontawesome to requirements
 * Update repository references to gitlab
 
 ## [0.3.0] - 2023-02-22
```

### Comparing `wagtail_sb_admin_interface-0.4.0/LICENSE.txt` & `wagtail_sb_admin_interface-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.4.0/README.md` & `wagtail_sb_admin_interface-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.4.0/pyproject.toml` & `wagtail_sb_admin_interface-0.5.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "wagtail-sb-admin-interface"
-version = "0.4.0"
-description = "Social Networks settings for wagtail sites."
+version = "0.5.0"
+description = "Customize the Wagtail admin interface from the admin itself."
 authors = [
   "SoftButterfly Development Team <dev@softbutterfly.io>",
   "zodiacfireworks <martin.vuelta@gmail.com>"
 ]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface"
@@ -28,15 +28,15 @@
 ]
 include = [
   "LICENSE.txt",
   "CHANGELOG.md",
 ]
 
 [tool.poetry.urls]
-"Download" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/archive/v0.4.0/wagtail-sb-admin-interface-v0.4.0.tar.gz"
+"Download" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/archive/v0.5.0/wagtail-sb-admin-interface-v0.5.0.tar.gz"
 "Bug Tracker" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 django = "< 5.0"
 django-colorfield = "<1.0.0"
 wagtail = "< 5.0"
```

### Comparing `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/admin.py` & `wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/admin.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/apps.py` & `wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/apps.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/cache.py` & `wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/cache.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0001_initial.py` & `wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0002_remove_theme_color_input_focus_and_more.py` & `wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/migrations/0002_remove_theme_color_input_focus_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0004_alter_theme_color_critical_alter_theme_color_info_and_more.py` & `wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/migrations/0004_alter_theme_color_critical_alter_theme_color_info_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/migrations/0006_theme_sidebar_logo_background_color.py` & `wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/migrations/0006_theme_sidebar_logo_background_color.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/models.py` & `wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/settings.py` & `wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/templates/wagtailadmin/base.html` & `wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/templates/wagtailadmin/base.html`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/templatetags/wagtail_sb_admin_interface_tags.py` & `wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/templatetags/wagtail_sb_admin_interface_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.4.0/src/wagtail_sb_admin_interface/wagtail_hooks.py` & `wagtail_sb_admin_interface-0.5.0/src/wagtail_sb_admin_interface/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_admin_interface-0.4.0/PKG-INFO` & `wagtail_sb_admin_interface-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: wagtail-sb-admin-interface
-Version: 0.4.0
-Summary: Social Networks settings for wagtail sites.
+Version: 0.5.0
+Summary: Customize the Wagtail admin interface from the admin itself.
 Home-page: https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface
 License: MIT
 Keywords: Softbutterfly,Django,Migrations
 Author: SoftButterfly Development Team
 Author-email: dev@softbutterfly.io
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
@@ -23,15 +23,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: django (<5.0)
 Requires-Dist: django-colorfield (<1.0.0)
 Requires-Dist: wagtail (<5.0)
 Requires-Dist: wagtail-sb-fontawesome (<1.0.0)
 Project-URL: Bug Tracker, https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/issues
 Project-URL: Documentation, https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/wikis
-Project-URL: Download, https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/archive/v0.4.0/wagtail-sb-admin-interface-v0.4.0.tar.gz
+Project-URL: Download, https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface/-/archive/v0.5.0/wagtail-sb-admin-interface-v0.5.0.tar.gz
 Project-URL: Repository, https://gitlab.com/softbutterfly/open-source/wagtail-sb-admin-interface
 Description-Content-Type: text/markdown
 
 ![Community-Project](https://gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/softbutterfly-open-source--banner--community-project.png)
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/wagtail-sb-admin-interface)
 ![PyPI - Package version](https://img.shields.io/pypi/v/wagtail-sb-admin-interface)
```


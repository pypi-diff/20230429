# Comparing `tmp/wagtail_sb_socialnetworks-0.5.0.tar.gz` & `tmp/wagtail_sb_socialnetworks-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_sb_socialnetworks-0.5.0.tar", max compression
+gzip compressed data, was "wagtail_sb_socialnetworks-0.6.0.tar", max compression
```

## Comparing `wagtail_sb_socialnetworks-0.5.0.tar` & `wagtail_sb_socialnetworks-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      743 2023-04-15 13:44:49.126311 wagtail_sb_socialnetworks-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2022-12-12 01:51:13.643284 wagtail_sb_socialnetworks-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     1661 2023-04-15 13:42:21.077778 wagtail_sb_socialnetworks-0.5.0/README.md
--rw-r--r--   0        0        0     1996 2023-04-15 13:44:49.126311 wagtail_sb_socialnetworks-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       88 2022-12-12 01:52:00.487482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/__init__.py
--rw-r--r--   0        0        0        0 2022-12-12 01:52:00.487482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/admin.py
--rw-r--r--   0        0        0      180 2022-12-12 01:52:00.487482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/apps.py
--rw-r--r--   0        0        0     1204 2022-12-12 01:52:00.491482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4536 2022-12-12 01:52:00.491482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/migrations/0001_initial.py
--rw-r--r--   0        0        0      684 2022-12-12 01:52:00.491482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/migrations/0002_alter_socialnetwork_icon.py
--rw-r--r--   0        0        0      574 2022-12-12 01:52:00.491482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/migrations/0003_rename_sitesettings_sitesocialnetworkprofile_site_settings_and_more.py
--rw-r--r--   0        0        0        0 2022-12-12 01:52:00.491482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/migrations/__init__.py
--rw-r--r--   0        0        0     3736 2022-12-12 01:52:00.487482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/models.py
--rw-r--r--   0        0        0        0 2022-12-12 01:52:00.487482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/tests.py
--rw-r--r--   0        0        0       20 2023-04-15 13:44:49.130311 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/version.py
--rw-r--r--   0        0        0        0 2022-12-12 01:52:00.487482 wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/views.py
--rw-r--r--   0        0        0     3232 1970-01-01 00:00:00.000000 wagtail_sb_socialnetworks-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      817 2023-04-29 21:57:06.429894 wagtail_sb_socialnetworks-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2022-12-12 01:51:13.643284 wagtail_sb_socialnetworks-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     1661 2023-04-15 13:45:43.322506 wagtail_sb_socialnetworks-0.6.0/README.md
+-rw-r--r--   0        0        0     1996 2023-04-29 21:57:06.421894 wagtail_sb_socialnetworks-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       88 2023-04-17 03:43:34.281612 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 03:43:34.281612 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/admin.py
+-rw-r--r--   0        0        0      180 2023-04-17 03:43:34.273612 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/apps.py
+-rw-r--r--   0        0        0     1069 2023-04-29 21:48:38.016239 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/compat.py
+-rw-r--r--   0        0        0     1204 2022-12-12 01:52:00.491482 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4536 2023-04-17 03:43:34.289612 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/migrations/0001_initial.py
+-rw-r--r--   0        0        0      684 2023-04-17 03:43:34.289612 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/migrations/0002_alter_socialnetwork_icon.py
+-rw-r--r--   0        0        0      574 2023-04-17 03:43:34.281612 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/migrations/0003_rename_sitesettings_sitesocialnetworkprofile_site_settings_and_more.py
+-rw-r--r--   0        0        0        0 2023-04-17 03:43:34.293612 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/migrations/__init__.py
+-rw-r--r--   0        0        0     3177 2023-04-29 21:55:17.869551 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/models.py
+-rw-r--r--   0        0        0        0 2023-04-17 03:43:34.265612 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/tests.py
+-rw-r--r--   0        0        0       20 2023-04-29 21:57:06.433894 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/version.py
+-rw-r--r--   0        0        0        0 2023-04-17 03:43:34.281612 wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/views.py
+-rw-r--r--   0        0        0     3232 1970-01-01 00:00:00.000000 wagtail_sb_socialnetworks-0.6.0/PKG-INFO
```

### Comparing `wagtail_sb_socialnetworks-0.5.0/LICENSE.txt` & `wagtail_sb_socialnetworks-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail_sb_socialnetworks-0.5.0/README.md` & `wagtail_sb_socialnetworks-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_sb_socialnetworks-0.5.0/pyproject.toml` & `wagtail_sb_socialnetworks-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wagtail-sb-socialnetworks"
-version = "0.5.0"
+version = "0.6.0"
 description = "Social Networks settings for wagtail sites."
 authors = [
   "SoftButterfly Development Team <dev@softbutterfly.io>",
   "zodiacfireworks <martin.vuelta@gmail.com>"
 ]
 license = "MIT License"
 readme = "README.md"
@@ -28,15 +28,15 @@
 ]
 include = [
   "LICENSE.txt",
   "CHANGELOG.md",
 ]
 
 [tool.poetry.urls]
-"Download" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/archive/v0.5.0/wagtail-sb-socialnetworks-v0.5.0.tar.gz"
+"Download" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/archive/v0.6.0/wagtail-sb-socialnetworks-v0.6.0.tar.gz"
 "Bug Tracker" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/issues"
 
 
 [tool.poetry.dependencies]
 python = ">= 3.8.1, < 4.0.0"
 Django = "< 5.0"
 wagtail = "< 5.0"
```

### Comparing `wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/locale/es/LC_MESSAGES/django.po` & `wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/migrations/0001_initial.py` & `wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/migrations/0002_alter_socialnetwork_icon.py` & `wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/migrations/0002_alter_socialnetwork_icon.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/migrations/0003_rename_sitesettings_sitesocialnetworkprofile_site_settings_and_more.py` & `wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/migrations/0003_rename_sitesettings_sitesocialnetworkprofile_site_settings_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_socialnetworks-0.5.0/src/wagtail_sb_socialnetworks/models.py` & `wagtail_sb_socialnetworks-0.6.0/src/wagtail_sb_socialnetworks/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,25 @@
 from django.db import models
 from django.utils.text import slugify
 from django.utils.translation import gettext_lazy as _
 from modelcluster.fields import ParentalKey
 from modelcluster.models import ClusterableModel
 from wagtail.contrib.settings.models import register_setting
-from wagtail.core.models import Orderable
 from wagtail.images import get_image_model_string
 from wagtail.snippets.models import register_snippet
 
-try:
-    from wagtail.contrib.settings.models import BaseSiteSetting
-
-    class BaseSetting(BaseSiteSetting):
-        class Meta:
-            abstract = True
-
-except ImportError:
-    from wagtail.contrib.settings.models import BaseSetting  # type: ignore
-
-try:
-    from wagtail.admin.panels import FieldPanel, InlinePanel, MultiFieldPanel
-
-    ImageChooserPanel = FieldPanel
-    SnippetChooserPanel = FieldPanel
-
-except ImportError:
-    from wagtail.admin.edit_handlers import FieldPanel, InlinePanel, MultiFieldPanel
-    from wagtail.images.edit_handlers import ImageChooserPanel  # type: ignore
-    from wagtail.snippets.edit_handlers import SnippetChooserPanel  # type: ignore
+from .compat import (
+    BaseSetting,
+    FieldPanel,
+    ImageChooserPanel,
+    InlinePanel,
+    MultiFieldPanel,
+    Orderable,
+    SnippetChooserPanel,
+)
 
 IMAGE_MODEL = get_image_model_string()
 
 
 @register_snippet
 class SocialNetwork(models.Model):
     name = models.CharField(
@@ -59,15 +47,15 @@
 
     class Meta:
         app_label = "wagtail_sb_socialnetworks"
         verbose_name = _("Social network")
         verbose_name_plural = _("Social networks")
 
     def __str__(self):
-        return self.name
+        return str(self.name)
 
     @property
     def slug(self):
         return slugify(self.name)
 
 
 @register_snippet
```

### Comparing `wagtail_sb_socialnetworks-0.5.0/PKG-INFO` & `wagtail_sb_socialnetworks-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-sb-socialnetworks
-Version: 0.5.0
+Version: 0.6.0
 Summary: Social Networks settings for wagtail sites.
 Home-page: https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks
 License: MIT
 Keywords: Softbutterfly,Django,Migrations
 Author: SoftButterfly Development Team
 Author-email: dev@softbutterfly.io
 Requires-Python: >=3.8.1,<4.0.0
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Django (<5.0)
 Requires-Dist: wagtail (<5.0)
 Project-URL: Bug Tracker, https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/issues
 Project-URL: Documentation, https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/wikis
-Project-URL: Download, https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/archive/v0.5.0/wagtail-sb-socialnetworks-v0.5.0.tar.gz
+Project-URL: Download, https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks/-/archive/v0.6.0/wagtail-sb-socialnetworks-v0.6.0.tar.gz
 Project-URL: Repository, https://gitlab.com/softbutterfly/open-source/wagtail-sb-socialnetworks
 Description-Content-Type: text/markdown
 
 ![Community-Project](https://gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/softbutterfly-open-source--banner--community-project.png)
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/wagtail-sb-socialnetworks)
 ![PyPI - Package version](https://img.shields.io/pypi/v/wagtail-sb-socialnetworks)
```


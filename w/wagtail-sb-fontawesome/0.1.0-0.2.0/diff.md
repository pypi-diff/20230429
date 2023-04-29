# Comparing `tmp/wagtail_sb_fontawesome-0.1.0.tar.gz` & `tmp/wagtail_sb_fontawesome-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_sb_fontawesome-0.1.0.tar", max compression
+gzip compressed data, was "wagtail_sb_fontawesome-0.2.0.tar", max compression
```

## Comparing `wagtail_sb_fontawesome-0.1.0.tar` & `wagtail_sb_fontawesome-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      103 2023-04-15 06:37:18.284131 wagtail_sb_fontawesome-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-04-15 06:37:06.856086 wagtail_sb_fontawesome-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1887 2023-04-15 06:37:06.856086 wagtail_sb_fontawesome-0.1.0/README.md
--rw-r--r--   0        0        0     1948 2023-04-15 06:37:18.284131 wagtail_sb_fontawesome-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      214 2023-04-15 06:37:06.864086 wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 06:37:06.864086 wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/admin.py
--rw-r--r--   0        0        0      273 2023-04-15 06:37:06.864086 wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/apps.py
--rw-r--r--   0        0        0      698 2023-04-15 06:37:06.864086 wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-04-15 06:37:06.864086 wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/models.py
--rw-r--r--   0        0        0    43964 2023-04-15 06:37:06.864086 wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/static/fontawsome/css/font-awesome.css
--rw-r--r--   0        0        0    34832 2023-04-15 06:37:06.864086 wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/static/fontawsome/css/font-awesome.min.css
--rw-r--r--   0        0        0   134808 2023-04-15 06:37:06.864086 wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/FontAwesome.otf
--rw-r--r--   0        0        0   165742 2023-04-15 06:37:06.868086 wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.eot
--rw-r--r--   0        0        0   443670 2023-04-15 06:37:06.872086 wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2023-04-15 06:37:06.872086 wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2023-04-15 06:37:06.876086 wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2023-04-15 06:37:06.876086 wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.woff2
--rw-r--r--   0        0        0        0 2023-04-15 06:37:06.876086 wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/tests.py
--rw-r--r--   0        0        0       20 2023-04-15 06:37:18.284131 wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/version.py
--rw-r--r--   0        0        0        0 2023-04-15 06:37:06.876086 wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/views.py
--rw-r--r--   0        0        0      317 2023-04-15 06:37:06.876086 wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/wagtail_hooks.py
--rw-r--r--   0        0        0     3424 1970-01-01 00:00:00.000000 wagtail_sb_fontawesome-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      171 2023-04-29 17:14:39.599980 wagtail_sb_fontawesome-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-04-15 06:37:06.856086 wagtail_sb_fontawesome-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1590 2023-04-15 07:11:09.667745 wagtail_sb_fontawesome-0.2.0/README.md
+-rw-r--r--   0        0        0     1948 2023-04-29 17:14:39.599980 wagtail_sb_fontawesome-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      214 2023-04-15 06:37:06.864086 wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 06:37:06.864086 wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/admin.py
+-rw-r--r--   0        0        0      273 2023-04-15 06:37:06.864086 wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/apps.py
+-rw-r--r--   0        0        0      119 2023-04-29 17:09:18.994436 wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/compat.py
+-rw-r--r--   0        0        0      698 2023-04-15 06:37:06.864086 wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-04-15 06:37:06.864086 wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/models.py
+-rw-r--r--   0        0        0    43964 2023-04-15 06:37:06.864086 wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/static/fontawsome/css/font-awesome.css
+-rw-r--r--   0        0        0    34832 2023-04-15 06:37:06.864086 wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/static/fontawsome/css/font-awesome.min.css
+-rw-r--r--   0        0        0   134808 2023-04-15 06:37:06.864086 wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/FontAwesome.otf
+-rw-r--r--   0        0        0   165742 2023-04-15 06:37:06.868086 wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   443670 2023-04-15 06:37:06.872086 wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2023-04-15 06:37:06.872086 wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2023-04-15 06:37:06.876086 wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2023-04-15 06:37:06.876086 wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0        0 2023-04-15 06:37:06.876086 wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/tests.py
+-rw-r--r--   0        0        0       20 2023-04-29 17:14:39.603980 wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/version.py
+-rw-r--r--   0        0        0        0 2023-04-15 06:37:06.876086 wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/views.py
+-rw-r--r--   0        0        0      313 2023-04-29 16:59:35.043586 wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/wagtail_hooks.py
+-rw-r--r--   0        0        0     3127 1970-01-01 00:00:00.000000 wagtail_sb_fontawesome-0.2.0/PKG-INFO
```

### Comparing `wagtail_sb_fontawesome-0.1.0/LICENSE.txt` & `wagtail_sb_fontawesome-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail_sb_fontawesome-0.1.0/README.md` & `wagtail_sb_fontawesome-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/wagtail-sb-fontawesome)
 ![PyPI - Package version](https://img.shields.io/pypi/v/wagtail-sb-fontawesome)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/wagtail-sb-fontawesome)
 ![PyPI - MIT License](https://img.shields.io/pypi/l/wagtail-sb-fontawesome)
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/2f6661a360234960b1800c0bdac37d3c)](https://app.codacy.com/gl/softbutterfly/wagtail-sb-fontawesome/dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
-[![Codacy Badge Coverage](https://app.codacy.com/project/badge/Coverage/2f6661a360234960b1800c0bdac37d3c)](https://www.codacy.com/gh/softbutterfly/wagtail-sb-fontawesome/dashboard?utm_source=github.com&utm_medium=referral&utm_content=softbutterfly/wagtail-sb-fontawesome&utm_campaign=Badge_Coverage)
 
 # Wagtail FontAwesome
 
 Use FontAwesome icons in Wagtail admin.
 
 ## Requirements
 
@@ -33,21 +32,21 @@
   # ...
   "wagtail_sb_fontawesome",
 ]
 ```
 
 ## Docs
 
-- [Ejemplos](https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/wiki)
-- [Wiki](https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/wiki)
+- [Ejemplos](https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/-/wikis)
+- [Wiki](https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/-/wikis)
 
 ## Changelog
 
 All changes to versions of this library are listed in the [change history](CHANGELOG.md).
 
 ## Development
 
 Check out our [contribution guide](CONTRIBUTING.md).
 
 ## Contributors
 
-See the list of contributors [here](https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/graphs/contributors).
+See the list of contributors [here](https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/-/graphs/develop).
```

### Comparing `wagtail_sb_fontawesome-0.1.0/pyproject.toml` & `wagtail_sb_fontawesome-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wagtail-sb-fontawesome"
-version = "0.1.0"
+version = "0.2.0"
 description = "FontAwesome for Wagtail Admin."
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
-"Download" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/-/archive/v0.1.0/wagtail-sb-fontawesome-v0.1.0.tar.gz"
+"Download" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/-/archive/v0.2.0/wagtail-sb-fontawesome-v0.2.0.tar.gz"
 "Bug Tracker" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/-/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 django = "< 5.0"
 wagtail = "< 5.0"
```

### Comparing `wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/locale/es/LC_MESSAGES/django.po` & `wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/static/fontawsome/css/font-awesome.css` & `wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/static/fontawsome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/static/fontawsome/css/font-awesome.min.css` & `wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/static/fontawsome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/FontAwesome.otf` & `wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.eot` & `wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.svg` & `wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.ttf` & `wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.woff` & `wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `wagtail_sb_fontawesome-0.1.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.woff2` & `wagtail_sb_fontawesome-0.2.0/src/wagtail_sb_fontawesome/static/fontawsome/fonts/fontawesome/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `wagtail_sb_fontawesome-0.1.0/PKG-INFO` & `wagtail_sb_fontawesome-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-sb-fontawesome
-Version: 0.1.0
+Version: 0.2.0
 Summary: FontAwesome for Wagtail Admin.
 Home-page: https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome
 License: MIT
 Keywords: Softbutterfly,Django,Migrations
 Author: SoftButterfly Development Team
 Author-email: dev@softbutterfly.io
 Requires-Python: >=3.8.1,<4.0.0
@@ -21,27 +21,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: django (<5.0)
 Requires-Dist: wagtail (<5.0)
 Project-URL: Bug Tracker, https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/-/issues
 Project-URL: Documentation, https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/-/wikis
-Project-URL: Download, https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/-/archive/v0.1.0/wagtail-sb-fontawesome-v0.1.0.tar.gz
+Project-URL: Download, https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/-/archive/v0.2.0/wagtail-sb-fontawesome-v0.2.0.tar.gz
 Project-URL: Repository, https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome
 Description-Content-Type: text/markdown
 
 ![Community-Project](https://gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/softbutterfly-open-source--banner--community-project.png)
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/wagtail-sb-fontawesome)
 ![PyPI - Package version](https://img.shields.io/pypi/v/wagtail-sb-fontawesome)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/wagtail-sb-fontawesome)
 ![PyPI - MIT License](https://img.shields.io/pypi/l/wagtail-sb-fontawesome)
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/2f6661a360234960b1800c0bdac37d3c)](https://app.codacy.com/gl/softbutterfly/wagtail-sb-fontawesome/dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
-[![Codacy Badge Coverage](https://app.codacy.com/project/badge/Coverage/2f6661a360234960b1800c0bdac37d3c)](https://www.codacy.com/gh/softbutterfly/wagtail-sb-fontawesome/dashboard?utm_source=github.com&utm_medium=referral&utm_content=softbutterfly/wagtail-sb-fontawesome&utm_campaign=Badge_Coverage)
 
 # Wagtail FontAwesome
 
 Use FontAwesome icons in Wagtail admin.
 
 ## Requirements
 
@@ -64,22 +63,22 @@
   # ...
   "wagtail_sb_fontawesome",
 ]
 ```
 
 ## Docs
 
-- [Ejemplos](https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/wiki)
-- [Wiki](https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/wiki)
+- [Ejemplos](https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/-/wikis)
+- [Wiki](https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/-/wikis)
 
 ## Changelog
 
 All changes to versions of this library are listed in the [change history](CHANGELOG.md).
 
 ## Development
 
 Check out our [contribution guide](CONTRIBUTING.md).
 
 ## Contributors
 
-See the list of contributors [here](https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/graphs/contributors).
+See the list of contributors [here](https://gitlab.com/softbutterfly/open-source/wagtail-sb-fontawesome/-/graphs/develop).
```


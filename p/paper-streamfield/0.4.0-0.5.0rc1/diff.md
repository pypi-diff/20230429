# Comparing `tmp/paper-streamfield-0.4.0.tar.gz` & `tmp/paper-streamfield-0.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-streamfield-0.4.0.tar", last modified: Sun Apr 16 17:54:41 2023, max compression
+gzip compressed data, was "paper-streamfield-0.5.0rc1.tar", last modified: Sat Apr 29 15:18:51 2023, max compression
```

## Comparing `paper-streamfield-0.4.0.tar` & `paper-streamfield-0.5.0rc1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.487895 paper-streamfield-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-16 17:54:41.487895 paper-streamfield-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.479895 paper-streamfield-0.4.0/paper_streamfield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-16 17:54:41.000000 paper-streamfield-0.4.0/paper_streamfield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-16 17:54:41.000000 paper-streamfield-0.4.0/paper_streamfield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:54:41.000000 paper-streamfield-0.4.0/paper_streamfield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:54:41.000000 paper-streamfield-0.4.0/paper_streamfield.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-16 17:54:41.000000 paper-streamfield-0.4.0/paper_streamfield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-16 17:54:41.000000 paper-streamfield-0.4.0/paper_streamfield.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-16 17:54:41.487895 paper-streamfield-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.483895 paper-streamfield-0.4.0/streamfield/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.483895 paper-streamfield-0.4.0/streamfield/admin/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/admin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/admin/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.483895 paper-streamfield-0.4.0/streamfield/field/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/field/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/field/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/field/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.479895 paper-streamfield-0.4.0/streamfield/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.479895 paper-streamfield-0.4.0/streamfield/static/streamfield/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.483895 paper-streamfield-0.4.0/streamfield/static/streamfield/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.483895 paper-streamfield-0.4.0/streamfield/static/streamfield/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-16 17:54:40.000000 paper-streamfield-0.4.0/streamfield/static/streamfield/dist/assets/sortable.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-16 17:54:40.000000 paper-streamfield-0.4.0/streamfield/static/streamfield/dist/assets/spinner.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-16 17:54:40.000000 paper-streamfield-0.4.0/streamfield/static/streamfield/dist/widget.css
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-04-16 17:54:40.000000 paper-streamfield-0.4.0/streamfield/static/streamfield/dist/widget.js
--rw-r--r--   0 runner    (1001) docker     (123)    26424 2023-04-16 17:54:40.000000 paper-streamfield-0.4.0/streamfield/static/streamfield/dist/widget.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.479895 paper-streamfield-0.4.0/streamfield/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.483895 paper-streamfield-0.4.0/streamfield/templates/streamfield/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.487895 paper-streamfield-0.4.0/streamfield/templates/streamfield/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/templates/streamfield/admin/block.html
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/templates/streamfield/admin/invalid_block.html
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/templates/streamfield/admin/popup_response.html
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/templates/streamfield/admin/toolbar.html
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/templates/streamfield/widget.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.487895 paper-streamfield-0.4.0/streamfield/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/templatetags/streamfield.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:18:51.297693 paper-streamfield-0.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-04-29 15:18:51.297693 paper-streamfield-0.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:18:51.285693 paper-streamfield-0.5.0rc1/paper_streamfield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-04-29 15:18:51.000000 paper-streamfield-0.5.0rc1/paper_streamfield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-29 15:18:51.000000 paper-streamfield-0.5.0rc1/paper_streamfield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:18:51.000000 paper-streamfield-0.5.0rc1/paper_streamfield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:18:51.000000 paper-streamfield-0.5.0rc1/paper_streamfield.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-29 15:18:51.000000 paper-streamfield-0.5.0rc1/paper_streamfield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-29 15:18:51.000000 paper-streamfield-0.5.0rc1/paper_streamfield.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-29 15:18:51.297693 paper-streamfield-0.5.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:18:51.289693 paper-streamfield-0.5.0rc1/streamfield/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:18:51.289693 paper-streamfield-0.5.0rc1/streamfield/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/admin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/admin/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:18:51.293693 paper-streamfield-0.5.0rc1/streamfield/field/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/field/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/field/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/field/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/renderers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:18:51.281693 paper-streamfield-0.5.0rc1/streamfield/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:18:51.281693 paper-streamfield-0.5.0rc1/streamfield/static/streamfield/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:18:51.293693 paper-streamfield-0.5.0rc1/streamfield/static/streamfield/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:18:51.293693 paper-streamfield-0.5.0rc1/streamfield/static/streamfield/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-29 15:18:50.000000 paper-streamfield-0.5.0rc1/streamfield/static/streamfield/dist/assets/sortable.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-29 15:18:50.000000 paper-streamfield-0.5.0rc1/streamfield/static/streamfield/dist/assets/spinner.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-29 15:18:50.000000 paper-streamfield-0.5.0rc1/streamfield/static/streamfield/dist/widget.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-04-29 15:18:50.000000 paper-streamfield-0.5.0rc1/streamfield/static/streamfield/dist/widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)    26585 2023-04-29 15:18:50.000000 paper-streamfield-0.5.0rc1/streamfield/static/streamfield/dist/widget.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:18:51.281693 paper-streamfield-0.5.0rc1/streamfield/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:18:51.293693 paper-streamfield-0.5.0rc1/streamfield/templates/streamfield/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:18:51.293693 paper-streamfield-0.5.0rc1/streamfield/templates/streamfield/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/templates/streamfield/admin/block.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/templates/streamfield/admin/buttons.html
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/templates/streamfield/admin/invalid_block.html
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/templates/streamfield/admin/popup_response.html
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/templates/streamfield/widget.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:18:51.293693 paper-streamfield-0.5.0rc1/streamfield/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/templatetags/streamfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-29 15:18:16.000000 paper-streamfield-0.5.0rc1/streamfield/utils.py
```

### Comparing `paper-streamfield-0.4.0/CHANGELOG.md` & `paper-streamfield-0.5.0rc1/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Change Log
 
+## [0.5.0](https://github.com/dldevinc/paper-streamfield/tree/v0.5.0) - 2023-04-29
+
+### ⚠ BREAKING CHANGES
+
+-   Added `StreamBlockMeta` class to provide metadata about a stream block.
+-   The `admin_block_template` property of the block model has been removed and replaced with 
+    `stream_block_template` property of the corresponding `StreamBlockModelAdminMixin`.
+-   The `renderer` module was renamed to `renderers`.
+
 ## [0.4.0](https://github.com/dldevinc/paper-streamfield/tree/v0.4.0) - 2023-04-16
 
 ### ⚠ BREAKING CHANGES
 
 -   Minimum required `paper-admin` version is now `6.0.0`.
 
 ## [0.3.0](https://github.com/dldevinc/paper-streamfield/tree/v0.3.0) - 2022-11-30
```

### Comparing `paper-streamfield-0.4.0/CONTRIBUTING.md` & `paper-streamfield-0.5.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.4.0/LICENSE` & `paper-streamfield-0.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.4.0/PKG-INFO` & `paper-streamfield-0.5.0rc1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: paper-streamfield
-Version: 0.4.0
-Summary: Implementation of the Wagtail's StreamField block picker for paper-admin.
-Home-page: https://github.com/dldevinc/paper-streamfield
-Author: Mihail Mishakin
-Author-email: x896321475@gmail.com
-Maintainer: Mihail Mishakin
-Maintainer-email: x896321475@gmail.com
-License: BSD license
-Platform: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
-Classifier: Framework :: Django :: 4.2
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # paper-streamfield
 
 Implementation of the Wagtail's StreamField block picker for paper-admin.
 
 [![PyPI](https://img.shields.io/pypi/v/paper-streamfield.svg)](https://pypi.org/project/paper-streamfield/)
 [![Build Status](https://github.com/dldevinc/paper-streamfield/actions/workflows/tests.yml/badge.svg)](https://github.com/dldevinc/paper-streamfield)
 [![Software license](https://img.shields.io/pypi/l/paper-streamfield.svg)](https://pypi.org/project/paper-streamfield/)
@@ -70,173 +38,244 @@
 )
 ```
 
 ## How to use
 
 1. Create some models that you want to use as blocks:
 
-```python
-# blocks/models.py
-
-from django.core.validators import MaxValueValidator, MinValueValidator
-from django.db import models
-from django.utils.text import Truncator
-from django.utils.translation import gettext_lazy as _
+   ```python
+   # blocks/models.py
+   
+   from django.core.validators import MaxValueValidator, MinValueValidator
+   from django.db import models
+   from django.utils.text import Truncator
+   
+   
+   class HeadingBlock(models.Model):
+       title = models.TextField()
+       rank = models.PositiveSmallIntegerField(
+           default=1,
+           validators=[
+               MinValueValidator(1),
+               MaxValueValidator(6)
+           ]
+       )
+   
+       class Meta:
+           verbose_name = "Heading"
+   
+       def __str__(self):
+           return Truncator(self.title).chars(128)
+   
+   
+   class TextBlock(models.Model):
+       text = models.TextField()
+   
+       class Meta:
+           verbose_name = "Text"
+   
+       def __str__(self):
+           return Truncator(self.text).chars(128)
+   ```
+
+2. Register your models using `StreamBlockModelAdmin` class.
+
+   ```python
+   # blocks/admin.py
+   
+   from django.contrib import admin
+   from streamfield.admin import StreamBlockModelAdmin
+   from .models import HeadingBlock, TextBlock
+   
+   
+   @admin.register(HeadingBlock)
+   class HeadingBlockAdmin(StreamBlockModelAdmin):
+       list_display = ["__str__", "rank"]
+   
+   
+   @admin.register(TextBlock)
+   class TextBlockAdmin(StreamBlockModelAdmin):
+       pass
+   ```
 
+3. Create templates for each block model, named as lowercase
+   model name or _snake_cased_ model name.
 
-class HeaderBlock(models.Model):
-    text = models.TextField(
-        _("text")
-    )
-    rank = models.PositiveSmallIntegerField(
-        _("rank"),
-        default=1,
-        validators=[
-            MinValueValidator(1),
-            MaxValueValidator(6)
-        ]
-    )
+   ```html
+   <!-- blocks/templates/blocks/headingblock.html -->
+   <!-- or -->
+   <!-- blocks/templates/blocks/heading_block.html -->
+   <h{{ block.rank }}>{{ block.text }}</h{{ block.rank }}>
+   ```
+   
+   ```html
+   <!-- blocks/templates/blocks/textblock.html -->
+   <!-- or -->
+   <!-- blocks/templates/blocks/text_block.html -->
+   <div>{{ block.text|linebreaks }}</div>
+   ```
 
-    class Meta:
-        verbose_name = "Header"
+4. Add `StreamField` to your model:
 
-    def __str__(self):
-        return Truncator(self.text).chars(64)
+   ```python
+   # app/models.py
+   
+   from django.db import models
+   from django.utils.translation import gettext_lazy as _
+   from streamfield.field.models import StreamField
+   
+   
+   class Page(models.Model):
+       stream = StreamField(
+          _("stream"), 
+          models=[
+              "blocks.HeaderBlock",
+              "blocks.TextBlock",
+          ]
+       )
+   
+       class Meta:
+           verbose_name = "Page"
+   ```
+   
+   Result:
+   ![](https://user-images.githubusercontent.com/6928240/190413272-14b95712-de0f-4a9b-a815-40e3fb0a2d85.png)
+   
+   Now you can create some blocks:
+   ![](https://user-images.githubusercontent.com/6928240/190414025-dfe364a9-524e-4529-835d-a3e507d1ee19.png)
+
+5. Use `render_stream` template tag to render the stream field.
+
+   ```html
+   <!-- app/templates/index.html -->
+   {% load streamfield %}
+   
+   {% render_stream page.stream %}
+   ```
+   
+   Result:
+   ![](https://user-images.githubusercontent.com/6928240/190416377-e2ba504f-8aa0-44ed-b59d-0cf1ccea695e.png)
 
+## Special cases
 
-class TextBlock(models.Model):
-    text = models.TextField(
-        _("text")
-    )
+### Use custom template name or template engine
 
-    class Meta:
-        verbose_name = "Text"
+If you need to use custom template name or template engine, you can
+specify 
 
-    def __str__(self):
-        return Truncator(self.text).chars(64)
-```
-
-2. Register this models using `StreamBlockModelAdmin` class.
+You can specify a template name or engine to render a specific block 
+with `StreamBlockMeta` class in your block model:
 
 ```python
-# blocks/admin.py
-
-from django.contrib import admin
-
-from streamfield.admin import StreamBlockModelAdmin
-
-from .models import HeaderBlock, TextBlock
-
+class HeadingBlock(models.Model):
+    # ...
 
-@admin.register(HeaderBlock)
-class HeaderBlockAdmin(StreamBlockModelAdmin):
-    list_display = ["__str__", "rank"]
-
-
-@admin.register(TextBlock)
-class TextBlockAdmin(StreamBlockModelAdmin):
-    pass
+    class StreamBlockMeta:
+        engine = "jinja2"
+        template = "blocks/heading.html"
 ```
 
-3. Create templates for each block model, named as lowercase
-   model name or _snake_cased_ model name.
+### Add extra context
 
-```html
-<!-- blocks/templates/blocks/headerblock.html -->
-<!-- or -->
-<!-- blocks/templates/blocks/header_block.html -->
-<h{{ block.rank }}>{{ block.text }}</h{{ block.rank }}>
-```
+You can add extra context to the template by passing
+additional keyword arguments to `render_stream` template tag:
 
 ```html
 <!-- blocks/templates/blocks/textblock.html -->
-<!-- or -->
-<!-- blocks/templates/blocks/text_block.html -->
-<div>{{ block.text|linebreaks }}</div>
+<div class="{{ classes }}">{{ block.text|linebreaks }}</div>
 ```
 
-You can also use the `block_template` option to specify the template to use:
+```html
+<!-- app/templates/index.html -->
+{% load streamfield %}
 
-```python
-class HeaderBlock(models.Model):
-    block_template = "blocks/header.html"
-    ...
+{% render_stream page.stream classes="text text--small" %}
 ```
 
-4. Add `StreamField` to your model:
-
-```python
-# app/models.py
-
-from django.db import models
-from django.utils.translation import gettext_lazy as _
-
-from streamfield.field.models import StreamField
+### Access parent context from within a block
 
+In some cases you need to access the parent context from the block
+template.
 
-class Page(models.Model):
-    stream = StreamField(_("stream"), models=[
-        "blocks.HeaderBlock",
-        "blocks.TextBlock",
-    ])
+You can access the parent context from the block template by using
+`parent_context` variable:
 
-    class Meta:
-        verbose_name = "Page"
+```html
+<!-- blocks/templates/blocks/textblock.html -->
+<div class="{{ parent_context.classes }}">{{ block.text|linebreaks }}</div>
 ```
 
-Result:
-![](https://user-images.githubusercontent.com/6928240/190413272-14b95712-de0f-4a9b-a815-40e3fb0a2d85.png)
-
-Now you can create some blocks:
-![](https://user-images.githubusercontent.com/6928240/190414025-dfe364a9-524e-4529-835d-a3e507d1ee19.png)
-
-5. Use `render_stream` templatetag to render the stream field.
-
 ```html
 <!-- app/templates/index.html -->
-{% load streamfield %} {% render_stream page.stream %}
-```
+{% load streamfield %}
 
-Result:
-![](https://user-images.githubusercontent.com/6928240/190416377-e2ba504f-8aa0-44ed-b59d-0cf1ccea695e.png)
-
-## Special cases
+<!-- Add classes to the page context -->
+{% with classes="text text--small" %}
+  {% render_stream page.stream %}
+{% endwith %}
+```
 
-### Use another template engine
+### Customize block in admin interface
 
-You can specify a template engine to render a specific block with
-`block_template_engine` option:
+You can customize how a block is rendered in the admin interface
+by specifying `stream_block_template` field in the `StreamBlockModelAdmin`
+class:
 
 ```python
-class HeaderBlock(models.Model):
-    block_template = "blocks/header.html"
-    block_template_engine = "jinja2"
-    ...
-```
-
-### Add extra context to blocks
+from django.contrib import admin
+from streamfield.admin import StreamBlockModelAdmin
+from .models import ImageBlock
 
-You can add additional variables by passing keyword arguments to the `render_stream` templatetag:
 
-```html
-<!-- app/templates/index.html -->
-{% load streamfield %} {% render_stream page.stream css_class="red" %}
+@admin.register(ImageBlock)
+class ImageBlockAdmin(StreamBlockModelAdmin):
+    stream_block_template = "blocks/admin/image.html"
+    list_display = ["__str__", "title", "alt"]
 ```
 
 ```html
-<!-- text_block.html -->
-<div class="{{ css_class }}">{{ block.text|linebreaks }}</div>
+<!-- blocks/admin/image.html -->
+{% extends "streamfield/admin/block.html" %}
+
+{% block content %}
+   <div class="d-flex">
+      <div class="flex-grow-0 mr-2">
+         <img class="preview"
+              src="{{ instance.image }}"
+              width="48"
+              height="36"
+              title="{{ instance.title }}"
+              alt="{{ instance.alt }}"
+              style="object-fit: cover">
+      </div>
+   
+      {{ block.super }}
+   </div>
+{% endblock content %}
 ```
 
-### Access parent context from within a block
+### Caching the rendered HTML of a block
 
-The parent context can be accessed via a `parent_context` variable:
+You can cache the rendered HTML of a block by using `CacheRenderer`
+class:
 
-```html
-<!-- app/templates/index.html -->
-{% load streamfield %} {% with css_class="blue" %} {% render_stream page.stream %} {% endwith %}
-```
+```python
+class HeadingBlock(models.Model):
+    # ...
 
-```html
-<!-- text_block.html -->
-<div class="{{ parent_context.css_class }}">{{ block.text|linebreaks }}</div>
+    class StreamBlockMeta:
+        renderer = "streamfield.renderers.CacheRenderer"
+        cache_ttl = 3600
 ```
+
+> Note that the specified block will **not** be invalidated 
+> when something changes in it.
+
+## Settings
+
+`PAPER_STREAMFIELD_DEFAULT_RENDERER`<br>
+Default renderer for `render_stream` template tag.<br>
+Default: `"streamfield.renderers.DefaultRenderer"`
+
+`PAPER_STREAMFIELD_DEFAULT_TEMPLATE_ENGINE`<br>
+Default template engine for `render_stream` template tag.<br>
+Default: `None`
```

### Comparing `paper-streamfield-0.4.0/package.json` & `paper-streamfield-0.5.0rc1/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9883040935672516%*

 * *Differences: {"'devDependencies'": "{'@babel/core': '^7.21.5', '@babel/preset-env': '^7.21.5', 'postcss': "*

 * *                      "'^8.4.23', 'postcss-loader': '^7.3.0', 'postcss-preset-env': '^8.3.2', "*

 * *                      "'sass': '^1.62.1', 'webpack': '^5.81.0', 'webpack-cli': '^5.0.2'}"}*

```diff
@@ -1,29 +1,29 @@
 {
     "author": "Mihail Mishakin",
     "description": "Implementation of the Wagtail's StreamField block picker for paper-admin.",
     "devDependencies": {
-        "@babel/core": "^7.21.4",
+        "@babel/core": "^7.21.5",
         "@babel/plugin-syntax-dynamic-import": "^7.8.3",
-        "@babel/preset-env": "^7.21.4",
+        "@babel/preset-env": "^7.21.5",
         "babel-loader": "^9.1.2",
         "babel-plugin-transform-imports": "^2.0.0",
         "css-minimizer-webpack-plugin": "^5.0.0",
         "fast-css-loader": "^1.0.2",
         "fibers": "^5.0.3",
         "mini-css-extract-plugin": "^2.7.5",
-        "postcss": "^8.4.22",
-        "postcss-loader": "^7.2.4",
-        "postcss-preset-env": "^8.3.1",
-        "sass": "^1.62.0",
+        "postcss": "^8.4.23",
+        "postcss-loader": "^7.3.0",
+        "postcss-preset-env": "^8.3.2",
+        "sass": "^1.62.1",
         "sass-loader": "^13.2.2",
         "terser-webpack-plugin": "^5.3.7",
         "uuid": "^9.0.0",
-        "webpack": "^5.79.0",
-        "webpack-cli": "^5.0.1",
+        "webpack": "^5.81.0",
+        "webpack-cli": "^5.0.2",
         "webpack-merge": "^5.8.0"
     },
     "license": "BSD license",
     "main": "streamfield/static/streamfield/index.js",
     "name": "paper-streamfield",
     "scripts": {
         "build": "webpack --mode production",
```

### Comparing `paper-streamfield-0.4.0/paper_streamfield.egg-info/PKG-INFO` & `paper-streamfield-0.5.0rc1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-streamfield
-Version: 0.4.0
+Version: 0.5.0rc1
 Summary: Implementation of the Wagtail's StreamField block picker for paper-admin.
 Home-page: https://github.com/dldevinc/paper-streamfield
 Author: Mihail Mishakin
 Author-email: x896321475@gmail.com
 Maintainer: Mihail Mishakin
 Maintainer-email: x896321475@gmail.com
 License: BSD license
@@ -70,173 +70,244 @@
 )
 ```
 
 ## How to use
 
 1. Create some models that you want to use as blocks:
 
-```python
-# blocks/models.py
-
-from django.core.validators import MaxValueValidator, MinValueValidator
-from django.db import models
-from django.utils.text import Truncator
-from django.utils.translation import gettext_lazy as _
+   ```python
+   # blocks/models.py
+   
+   from django.core.validators import MaxValueValidator, MinValueValidator
+   from django.db import models
+   from django.utils.text import Truncator
+   
+   
+   class HeadingBlock(models.Model):
+       title = models.TextField()
+       rank = models.PositiveSmallIntegerField(
+           default=1,
+           validators=[
+               MinValueValidator(1),
+               MaxValueValidator(6)
+           ]
+       )
+   
+       class Meta:
+           verbose_name = "Heading"
+   
+       def __str__(self):
+           return Truncator(self.title).chars(128)
+   
+   
+   class TextBlock(models.Model):
+       text = models.TextField()
+   
+       class Meta:
+           verbose_name = "Text"
+   
+       def __str__(self):
+           return Truncator(self.text).chars(128)
+   ```
+
+2. Register your models using `StreamBlockModelAdmin` class.
+
+   ```python
+   # blocks/admin.py
+   
+   from django.contrib import admin
+   from streamfield.admin import StreamBlockModelAdmin
+   from .models import HeadingBlock, TextBlock
+   
+   
+   @admin.register(HeadingBlock)
+   class HeadingBlockAdmin(StreamBlockModelAdmin):
+       list_display = ["__str__", "rank"]
+   
+   
+   @admin.register(TextBlock)
+   class TextBlockAdmin(StreamBlockModelAdmin):
+       pass
+   ```
 
+3. Create templates for each block model, named as lowercase
+   model name or _snake_cased_ model name.
 
-class HeaderBlock(models.Model):
-    text = models.TextField(
-        _("text")
-    )
-    rank = models.PositiveSmallIntegerField(
-        _("rank"),
-        default=1,
-        validators=[
-            MinValueValidator(1),
-            MaxValueValidator(6)
-        ]
-    )
-
-    class Meta:
-        verbose_name = "Header"
+   ```html
+   <!-- blocks/templates/blocks/headingblock.html -->
+   <!-- or -->
+   <!-- blocks/templates/blocks/heading_block.html -->
+   <h{{ block.rank }}>{{ block.text }}</h{{ block.rank }}>
+   ```
+   
+   ```html
+   <!-- blocks/templates/blocks/textblock.html -->
+   <!-- or -->
+   <!-- blocks/templates/blocks/text_block.html -->
+   <div>{{ block.text|linebreaks }}</div>
+   ```
 
-    def __str__(self):
-        return Truncator(self.text).chars(64)
+4. Add `StreamField` to your model:
 
+   ```python
+   # app/models.py
+   
+   from django.db import models
+   from django.utils.translation import gettext_lazy as _
+   from streamfield.field.models import StreamField
+   
+   
+   class Page(models.Model):
+       stream = StreamField(
+          _("stream"), 
+          models=[
+              "blocks.HeaderBlock",
+              "blocks.TextBlock",
+          ]
+       )
+   
+       class Meta:
+           verbose_name = "Page"
+   ```
+   
+   Result:
+   ![](https://user-images.githubusercontent.com/6928240/190413272-14b95712-de0f-4a9b-a815-40e3fb0a2d85.png)
+   
+   Now you can create some blocks:
+   ![](https://user-images.githubusercontent.com/6928240/190414025-dfe364a9-524e-4529-835d-a3e507d1ee19.png)
+
+5. Use `render_stream` template tag to render the stream field.
+
+   ```html
+   <!-- app/templates/index.html -->
+   {% load streamfield %}
+   
+   {% render_stream page.stream %}
+   ```
+   
+   Result:
+   ![](https://user-images.githubusercontent.com/6928240/190416377-e2ba504f-8aa0-44ed-b59d-0cf1ccea695e.png)
 
-class TextBlock(models.Model):
-    text = models.TextField(
-        _("text")
-    )
+## Special cases
 
-    class Meta:
-        verbose_name = "Text"
+### Use custom template name or template engine
 
-    def __str__(self):
-        return Truncator(self.text).chars(64)
-```
+If you need to use custom template name or template engine, you can
+specify 
 
-2. Register this models using `StreamBlockModelAdmin` class.
+You can specify a template name or engine to render a specific block 
+with `StreamBlockMeta` class in your block model:
 
 ```python
-# blocks/admin.py
-
-from django.contrib import admin
-
-from streamfield.admin import StreamBlockModelAdmin
-
-from .models import HeaderBlock, TextBlock
-
-
-@admin.register(HeaderBlock)
-class HeaderBlockAdmin(StreamBlockModelAdmin):
-    list_display = ["__str__", "rank"]
+class HeadingBlock(models.Model):
+    # ...
 
-
-@admin.register(TextBlock)
-class TextBlockAdmin(StreamBlockModelAdmin):
-    pass
+    class StreamBlockMeta:
+        engine = "jinja2"
+        template = "blocks/heading.html"
 ```
 
-3. Create templates for each block model, named as lowercase
-   model name or _snake_cased_ model name.
+### Add extra context
 
-```html
-<!-- blocks/templates/blocks/headerblock.html -->
-<!-- or -->
-<!-- blocks/templates/blocks/header_block.html -->
-<h{{ block.rank }}>{{ block.text }}</h{{ block.rank }}>
-```
+You can add extra context to the template by passing
+additional keyword arguments to `render_stream` template tag:
 
 ```html
 <!-- blocks/templates/blocks/textblock.html -->
-<!-- or -->
-<!-- blocks/templates/blocks/text_block.html -->
-<div>{{ block.text|linebreaks }}</div>
+<div class="{{ classes }}">{{ block.text|linebreaks }}</div>
 ```
 
-You can also use the `block_template` option to specify the template to use:
+```html
+<!-- app/templates/index.html -->
+{% load streamfield %}
 
-```python
-class HeaderBlock(models.Model):
-    block_template = "blocks/header.html"
-    ...
+{% render_stream page.stream classes="text text--small" %}
 ```
 
-4. Add `StreamField` to your model:
-
-```python
-# app/models.py
-
-from django.db import models
-from django.utils.translation import gettext_lazy as _
-
-from streamfield.field.models import StreamField
+### Access parent context from within a block
 
+In some cases you need to access the parent context from the block
+template.
 
-class Page(models.Model):
-    stream = StreamField(_("stream"), models=[
-        "blocks.HeaderBlock",
-        "blocks.TextBlock",
-    ])
+You can access the parent context from the block template by using
+`parent_context` variable:
 
-    class Meta:
-        verbose_name = "Page"
+```html
+<!-- blocks/templates/blocks/textblock.html -->
+<div class="{{ parent_context.classes }}">{{ block.text|linebreaks }}</div>
 ```
 
-Result:
-![](https://user-images.githubusercontent.com/6928240/190413272-14b95712-de0f-4a9b-a815-40e3fb0a2d85.png)
-
-Now you can create some blocks:
-![](https://user-images.githubusercontent.com/6928240/190414025-dfe364a9-524e-4529-835d-a3e507d1ee19.png)
-
-5. Use `render_stream` templatetag to render the stream field.
-
 ```html
 <!-- app/templates/index.html -->
-{% load streamfield %} {% render_stream page.stream %}
-```
+{% load streamfield %}
 
-Result:
-![](https://user-images.githubusercontent.com/6928240/190416377-e2ba504f-8aa0-44ed-b59d-0cf1ccea695e.png)
-
-## Special cases
+<!-- Add classes to the page context -->
+{% with classes="text text--small" %}
+  {% render_stream page.stream %}
+{% endwith %}
+```
 
-### Use another template engine
+### Customize block in admin interface
 
-You can specify a template engine to render a specific block with
-`block_template_engine` option:
+You can customize how a block is rendered in the admin interface
+by specifying `stream_block_template` field in the `StreamBlockModelAdmin`
+class:
 
 ```python
-class HeaderBlock(models.Model):
-    block_template = "blocks/header.html"
-    block_template_engine = "jinja2"
-    ...
-```
-
-### Add extra context to blocks
+from django.contrib import admin
+from streamfield.admin import StreamBlockModelAdmin
+from .models import ImageBlock
 
-You can add additional variables by passing keyword arguments to the `render_stream` templatetag:
 
-```html
-<!-- app/templates/index.html -->
-{% load streamfield %} {% render_stream page.stream css_class="red" %}
+@admin.register(ImageBlock)
+class ImageBlockAdmin(StreamBlockModelAdmin):
+    stream_block_template = "blocks/admin/image.html"
+    list_display = ["__str__", "title", "alt"]
 ```
 
 ```html
-<!-- text_block.html -->
-<div class="{{ css_class }}">{{ block.text|linebreaks }}</div>
+<!-- blocks/admin/image.html -->
+{% extends "streamfield/admin/block.html" %}
+
+{% block content %}
+   <div class="d-flex">
+      <div class="flex-grow-0 mr-2">
+         <img class="preview"
+              src="{{ instance.image }}"
+              width="48"
+              height="36"
+              title="{{ instance.title }}"
+              alt="{{ instance.alt }}"
+              style="object-fit: cover">
+      </div>
+   
+      {{ block.super }}
+   </div>
+{% endblock content %}
 ```
 
-### Access parent context from within a block
+### Caching the rendered HTML of a block
 
-The parent context can be accessed via a `parent_context` variable:
+You can cache the rendered HTML of a block by using `CacheRenderer`
+class:
 
-```html
-<!-- app/templates/index.html -->
-{% load streamfield %} {% with css_class="blue" %} {% render_stream page.stream %} {% endwith %}
-```
+```python
+class HeadingBlock(models.Model):
+    # ...
 
-```html
-<!-- text_block.html -->
-<div class="{{ parent_context.css_class }}">{{ block.text|linebreaks }}</div>
+    class StreamBlockMeta:
+        renderer = "streamfield.renderers.CacheRenderer"
+        cache_ttl = 3600
 ```
+
+> Note that the specified block will **not** be invalidated 
+> when something changes in it.
+
+## Settings
+
+`PAPER_STREAMFIELD_DEFAULT_RENDERER`<br>
+Default renderer for `render_stream` template tag.<br>
+Default: `"streamfield.renderers.DefaultRenderer"`
+
+`PAPER_STREAMFIELD_DEFAULT_TEMPLATE_ENGINE`<br>
+Default template engine for `render_stream` template tag.<br>
+Default: `None`
```

### Comparing `paper-streamfield-0.4.0/paper_streamfield.egg-info/SOURCES.txt` & `paper-streamfield-0.5.0rc1/paper_streamfield.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 streamfield/__init__.py
 streamfield/apps.py
 streamfield/blocks.py
 streamfield/conf.py
 streamfield/exceptions.py
 streamfield/helpers.py
 streamfield/logging.py
-streamfield/renderer.py
+streamfield/options.py
+streamfield/renderers.py
 streamfield/typing.py
 streamfield/urls.py
 streamfield/utils.py
 streamfield/admin/__init__.py
 streamfield/admin/base.py
 streamfield/admin/views.py
 streamfield/field/__init__.py
@@ -33,12 +34,12 @@
 streamfield/static/streamfield/dist/widget.css
 streamfield/static/streamfield/dist/widget.js
 streamfield/static/streamfield/dist/widget.js.map
 streamfield/static/streamfield/dist/assets/sortable.svg
 streamfield/static/streamfield/dist/assets/spinner.svg
 streamfield/templates/streamfield/widget.html
 streamfield/templates/streamfield/admin/block.html
+streamfield/templates/streamfield/admin/buttons.html
 streamfield/templates/streamfield/admin/invalid_block.html
 streamfield/templates/streamfield/admin/popup_response.html
-streamfield/templates/streamfield/admin/toolbar.html
 streamfield/templatetags/__init__.py
 streamfield/templatetags/streamfield.py
```

### Comparing `paper-streamfield-0.4.0/setup.cfg` & `paper-streamfield-0.5.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.4.0/streamfield/blocks.py` & `paper-streamfield-0.5.0rc1/streamfield/blocks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Dict
 from uuid import uuid4
 
 from django.apps import apps
 from django.core.handlers.wsgi import WSGIRequest
-from django.utils.module_loading import import_string
 
-from . import conf
-from .typing import BlockInstance, BlockModel
+from .options import get_block_opts
+from .typing import BlockInstance
 
 
 def to_dict(instance: BlockInstance) -> Dict[str, str]:
     """
     Сериализация блока для JSON.
 
     Для облегчения управления блоками на фронтенде
@@ -44,26 +43,17 @@
 
 
 def from_dict(value: Dict[str, str]) -> BlockInstance:
     """
     Возвращает экземпляр блока из словаря,
     созданного с помощью функции `to_dict()`.
     """
-    model = apps.get_model(value["model"])  # type: BlockModel
+    model = apps.get_model(value["model"])
     return model._base_manager.get(pk=value["pk"])
 
 
-def render(block: BlockInstance, extra_context: Dict = None, request: WSGIRequest = None) -> str:
+def render(block: BlockInstance, context: Dict = None, request: WSGIRequest = None) -> str:
     """
     Отрисовка экземпляра блока.
     """
-    renderer = getattr(block, "block_renderer", conf.DEFAULT_RENDERER)
-    if isinstance(renderer, str):
-        renderer_name = renderer
-        renderer = import_string(renderer_name)
-        if not callable(renderer):
-            raise ImportError("%s object is not callable" % renderer_name)
-
-    if isinstance(renderer, type):
-        renderer = renderer()
-
-    return renderer(block, extra_context, request=request)
+    opts = get_block_opts(block)
+    return opts.renderer(block, request=request, **(context or {}))
```

### Comparing `paper-streamfield-0.4.0/streamfield/field/forms.py` & `paper-streamfield-0.5.0rc1/streamfield/field/forms.py`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.4.0/streamfield/field/models.py` & `paper-streamfield-0.5.0rc1/streamfield/field/models.py`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.4.0/streamfield/helpers.py` & `paper-streamfield-0.5.0rc1/streamfield/helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from django.core.exceptions import MultipleObjectsReturned, ObjectDoesNotExist
 from django.core.handlers.wsgi import WSGIRequest
 
 from . import blocks, exceptions
 from .logging import logger
 
 
-def render_stream(stream: Union[str, List], extra_context: Dict = None, request: WSGIRequest = None) -> str:
+def render_stream(stream: Union[str, List], context: Dict = None, request: WSGIRequest = None) -> str:
     """
     Отрисовка всех блоков из JSON-массива.
     """
     if isinstance(stream, str):
         stream = json.loads(stream)
 
     if not isinstance(stream, list):
@@ -28,13 +28,13 @@
         except (LookupError, ObjectDoesNotExist, MultipleObjectsReturned):
             logger.warning("Invalid block: %r", record)
             continue
         else:
             output.append(
                 blocks.render(
                     block,
-                    extra_context=extra_context,
-                    request=request
+                    context or {},
+                    request=request,
                 )
             )
 
     return "\n".join(output)
```

### Comparing `paper-streamfield-0.4.0/streamfield/static/streamfield/dist/assets/sortable.svg` & `paper-streamfield-0.5.0rc1/streamfield/static/streamfield/dist/assets/sortable.svg`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.4.0/streamfield/static/streamfield/dist/assets/spinner.svg` & `paper-streamfield-0.5.0rc1/streamfield/static/streamfield/dist/assets/spinner.svg`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.4.0/streamfield/static/streamfield/dist/widget.js` & `paper-streamfield-0.5.0rc1/streamfield/static/streamfield/dist/widget.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,275 +1,278 @@
 ! function() {
     "use strict";
-    var e = /^(?:[0-9a-f]{8}-[0-9a-f]{4}-[1-5][0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}|00000000-0000-0000-0000-000000000000)$/i;
-    var t = function(t) {
-        return "string" == typeof t && e.test(t)
+    var t = /^(?:[0-9a-f]{8}-[0-9a-f]{4}-[1-5][0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}|00000000-0000-0000-0000-000000000000)$/i;
+    var e = function(e) {
+        return "string" == typeof e && t.test(e)
     };
     var o = {
         randomUUID: "undefined" != typeof crypto && crypto.randomUUID && crypto.randomUUID.bind(crypto)
     };
     let s;
     const r = new Uint8Array(16);
 
     function n() {
         if (!s && (s = "undefined" != typeof crypto && crypto.getRandomValues && crypto.getRandomValues.bind(crypto), !s)) throw new Error("crypto.getRandomValues() not supported. See https://github.com/uuidjs/uuid#getrandomvalues-not-supported");
         return s(r)
     }
-    const a = [];
-    for (let e = 0; e < 256; ++e) a.push((e + 256).toString(16).slice(1));
+    const i = [];
+    for (let t = 0; t < 256; ++t) i.push((t + 256).toString(16).slice(1));
 
-    function i(e, t = 0) {
-        return (a[e[t + 0]] + a[e[t + 1]] + a[e[t + 2]] + a[e[t + 3]] + "-" + a[e[t + 4]] + a[e[t + 5]] + "-" + a[e[t + 6]] + a[e[t + 7]] + "-" + a[e[t + 8]] + a[e[t + 9]] + "-" + a[e[t + 10]] + a[e[t + 11]] + a[e[t + 12]] + a[e[t + 13]] + a[e[t + 14]] + a[e[t + 15]]).toLowerCase()
+    function l(t, e = 0) {
+        return (i[t[e + 0]] + i[t[e + 1]] + i[t[e + 2]] + i[t[e + 3]] + "-" + i[t[e + 4]] + i[t[e + 5]] + "-" + i[t[e + 6]] + i[t[e + 7]] + "-" + i[t[e + 8]] + i[t[e + 9]] + "-" + i[t[e + 10]] + i[t[e + 11]] + i[t[e + 12]] + i[t[e + 13]] + i[t[e + 14]] + i[t[e + 15]]).toLowerCase()
     }
-    var l = function(e, t, s) {
-        if (o.randomUUID && !t && !e) return o.randomUUID();
-        const r = (e = e || {}).random || (e.rng || n)();
-        if (r[6] = 15 & r[6] | 64, r[8] = 63 & r[8] | 128, t) {
+    var a = function(t, e, s) {
+        if (o.randomUUID && !e && !t) return o.randomUUID();
+        const r = (t = t || {}).random || (t.rng || n)();
+        if (r[6] = 15 & r[6] | 64, r[8] = 63 & r[8] | 128, e) {
             s = s || 0;
-            for (let e = 0; e < 16; ++e) t[s + e] = r[e];
-            return t
+            for (let t = 0; t < 16; ++t) e[s + t] = r[t];
+            return e
         }
-        return i(r)
+        return l(r)
     };
     const d = window.paperAdmin.popupUtils,
         c = window.paperAdmin.modals;
     class u {
-        constructor(e) {
-            this.field = e, this.control = this.field.querySelector(`.${this.CSS.control}`), this.blocks = this.field.querySelector(`.${this.CSS.blocks}`), this.toolbar = this.field.querySelector(`.${this.CSS.toolbar}`), this._sortable = this._initSortable(), this._addListeners(), this._updateBlockMap(), this.wrapPreloader(Promise.all([this.update(), this.updateToolbar()]))
+        constructor(t) {
+            this.field = t, this.control = this.field.querySelector(`.${this.CSS.control}`), this.blocks = this.field.querySelector(`.${this.CSS.blocks}`), this.buttons = this.field.querySelector(`.${this.CSS.buttons}`), this._sortable = this._initSortable(), this._addListeners(), this._updateBlockMap(), this.wrapPreloader(Promise.all([this.updateBlocks(), this.updateButtons()]))
         }
         get STATUS() {
             return this.constructor.STATUS
         }
         get CSS() {
             return this.constructor.CSS
         }
         get value() {
-            let e;
+            let t;
             try {
-                e = JSON.parse(this.control.value)
+                t = JSON.parse(this.control.value)
             } catch {
-                e = []
+                t = []
             }
-            return e
+            return t
         }
-        set value(e) {
-            "string" != typeof e && (e = JSON.stringify(e)), this.control.value = e
+        set value(t) {
+            "string" != typeof t && (t = JSON.stringify(t)), this.control.value = t
         }
         get status() {
-            return Object.values(this.STATUS).find((e => this.field.classList.contains(`${this.CSS.field}--${e}`)))
+            return Object.values(this.STATUS).find((t => this.field.classList.contains(`${this.CSS.field}--${t}`)))
         }
-        set status(e) {
-            Object.values(this.STATUS).forEach((t => {
-                this.field.classList.toggle(`${this.CSS.field}--${t}`, e === t)
+        set status(t) {
+            Object.values(this.STATUS).forEach((e => {
+                this.field.classList.toggle(`${this.CSS.field}--${e}`, t === e)
             }))
         }
         get allowedModels() {
             return JSON.parse(this.control.dataset.allowedModels)
         }
         getBlocks() {
             return Array.from(this.blocks.querySelectorAll(`.${this.CSS.block}`))
         }
-        getBlockByUUID(e) {
-            return this._blockMap[e]
+        getBlockByUUID(t) {
+            return this._blockMap[t]
         }
         destroy() {
             this._sortable && this._sortable.destroy()
         }
         _updateBlockMap() {
-            let e = !1;
+            let t = !1;
             const o = {},
                 s = this.value.map((s => {
                     let r = s.uuid;
-                    return "string" == typeof r && t(r) ? o[r] = s : (e = !0, r = l(), o[r] = {
+                    return "string" == typeof r && e(r) ? o[r] = s : (t = !0, r = a(), o[r] = {
                         uuid: r
                     })
                 }));
             this._blockMap = o, s && (this.value = s)
         }
         _initSortable() {
             return Sortable.create(this.blocks, {
                 animation: 0,
                 draggable: `.${this.CSS.block}`,
-                filter: (e, t) => this.status === this.STATUS.LOADING || (!t || void 0),
+                filter: (t, e) => this.status === this.STATUS.LOADING || (!e || void 0),
                 handle: `.${this.CSS.sortableHandler}`,
                 ghostClass: "sortable-ghost",
                 onEnd: () => {
                     this.save()
                 }
             })
         }
         _addListeners() {
-            this.field.addEventListener("click", (e => {
-                const t = e.target.closest(`.${this.CSS.deleteBlockButton}`);
-                t && (e.preventDefault(), t.disabled = !0, c.createModal({
+            this.field.addEventListener("click", (t => {
+                const e = t.target.closest(`.${this.CSS.deleteBlockButton}`);
+                e && (t.preventDefault(), e.disabled = !0, c.createModal({
                     modalClass: "paper-modal--warning fade",
                     title: gettext("Confirm deletion"),
                     body: gettext("Are you sure you want to <b>DELETE</b> selected block from this field?"),
                     buttons: [{
                         label: gettext("Cancel"),
                         buttonClass: "btn-light",
-                        onClick: (e, t) => {
-                            t.destroy()
+                        onClick: (t, e) => {
+                            e.destroy()
                         }
                     }, {
                         autofocus: !0,
                         label: gettext("Delete"),
                         buttonClass: "btn-danger",
-                        onClick: (e, o) => {
+                        onClick: (t, o) => {
                             o.destroy();
-                            t.closest(`.${this.CSS.block}`).remove(), this.save(), this.wrapPreloader(this.update())
+                            e.closest(`.${this.CSS.block}`).remove(), this.save(), this.wrapPreloader(this.updateBlocks())
                         }
                     }],
                     onInit: function() {
                         this.show()
                     },
                     onDestroy: function() {
-                        t.disabled = !1
+                        e.disabled = !1
                     }
                 }));
-                const o = e.target.closest(`.${this.CSS.changeBlockButton}`);
+                const o = t.target.closest(`.${this.CSS.changeBlockButton}`);
                 if (o) {
-                    e.preventDefault();
-                    const t = $.Event("django:show-related", {
+                    t.preventDefault();
+                    const e = $.Event("django:show-related", {
                         href: o.href
                     });
-                    $(o).trigger(t), t.isDefaultPrevented() || h(o)
+                    $(o).trigger(e), e.isDefaultPrevented() || h(o)
                 }
-                const s = e.target.closest(`.${this.CSS.dropdownItemButton}`);
+                const s = t.target.closest(`.${this.CSS.dropdownItemButton}`);
                 if (s) {
-                    e.preventDefault();
-                    const t = $.Event("django:show-related", {
+                    t.preventDefault();
+                    const e = $.Event("django:show-related", {
                         href: s.href
                     });
-                    $(s).trigger(t), t.isDefaultPrevented() || h(s)
+                    $(s).trigger(e), e.isDefaultPrevented() || h(s)
                 }
             }))
         }
-        _appendBlock(e) {
-            const o = e.uuid;
-            if (!t(o)) throw new Error("Invalid UUID");
+        _appendBlock(t) {
+            const o = t.uuid;
+            if (!e(o)) throw new Error("Invalid UUID");
             const s = this.value;
-            s.push(e), this.value = s, this._blockMap[o] = e
+            s.push(t), this.value = s, this._blockMap[o] = t
         }
         save() {
-            this.value = this.getBlocks().map((e => {
-                const t = e.dataset.uuid;
-                return this.getBlockByUUID(t)
+            this.value = this.getBlocks().map((t => {
+                const e = t.dataset.uuid;
+                return this.getBlockByUUID(e)
             }))
         }
-        update() {
-            return this.renderStream(this.value)
-        }
-        wrapPreloader(e) {
-            return this.status = this.STATUS.LOADING, e.finally((() => {
+        wrapPreloader(t) {
+            return this.status = this.STATUS.LOADING, t.finally((() => {
                 this.status = this.STATUS.READY
             }))
         }
-        renderStream(e) {
-            const t = this.field.dataset.renderStreamUrl;
-            return fetch(t, {
+        updateBlocks() {
+            return this.renderStream({
+                allowedModels: this.allowedModels,
+                value: this.value
+            })
+        }
+        renderStream(t) {
+            const e = this.field.dataset.renderStreamUrl;
+            return fetch(e, {
                 method: "POST",
                 mode: "same-origin",
                 cache: "no-store",
                 headers: {
                     "Content-Type": "application/json;charset=utf-8"
                 },
-                body: JSON.stringify(e)
-            }).then((e => {
-                if (!e.ok) throw `${e.status} ${e.statusText}`;
-                return e.json()
-            })).then((e => {
-                this.blocks.innerHTML = e.blocks
-            })).catch((e => {
-                e instanceof Error && console.error(e), c.showErrors(e)
+                body: JSON.stringify(t)
+            }).then((t => {
+                if (!t.ok) throw `${t.status} ${t.statusText}`;
+                return t.json()
+            })).then((t => {
+                this.blocks.innerHTML = t.blocks
+            })).catch((t => {
+                t instanceof Error && console.error(t), c.showErrors(t)
             }))
         }
-        renderToolbar(e) {
-            const t = this.field.dataset.renderToolbarUrl;
-            return fetch(t, {
+        updateButtons() {
+            return this.renderButtons({
+                field_id: this.control.id,
+                allowedModels: this.allowedModels
+            })
+        }
+        renderButtons(t) {
+            const e = this.field.dataset.renderButtonsUrl;
+            return fetch(e, {
                 method: "POST",
                 mode: "same-origin",
                 cache: "no-store",
                 headers: {
                     "Content-Type": "application/json;charset=utf-8"
                 },
-                body: JSON.stringify(e)
-            }).then((e => {
-                if (!e.ok) throw `${e.status} ${e.statusText}`;
-                return e.json()
-            })).then((e => {
-                this.toolbar.innerHTML = e.toolbar
+                body: JSON.stringify(t)
+            }).then((t => {
+                if (!t.ok) throw `${t.status} ${t.statusText}`;
+                return t.json()
+            })).then((t => {
+                this.buttons.innerHTML = t.buttons
             }))
         }
-        updateToolbar() {
-            return this.renderToolbar({
-                field_id: this.control.id,
-                models: this.allowedModels
-            })
-        }
     }
 
-    function h(e) {
-        return d.showAdminPopup(e, /^(change|add|lookup)_/, !0)
+    function h(t) {
+        return d.showAdminPopup(t, /^(change|add|lookup)_/, !0)
     }
     var p;
     u.STATUS = {
         LOADING: "loading",
         READY: "ready"
     }, u.CSS = {
         field: "stream-field",
         control: "stream-field__control",
         blocks: "stream-field__blocks",
         block: "stream-field__block",
-        toolbar: "stream-field__toolbar",
+        buttons: "stream-field__buttons",
         sortableHandler: "stream-field__sortable-handler",
         changeBlockButton: "stream-field__change-btn",
         deleteBlockButton: "stream-field__delete-btn",
         dropdownItemButton: "stream-field__dropdown-item"
     }, XClass.register("paper-streamfield", {
-        init: function(e) {
-            e._streamField = new u(e, this)
+        init: function(t) {
+            t._streamField = new u(t, this)
         },
-        destroy: function(e) {
-            e._streamField && (e._streamField.destroy(), delete e._streamField)
+        destroy: function(t) {
+            t._streamField && (t._streamField.destroy(), delete t._streamField)
         }
-    }), window.dismissAddStreamBlockPopup = function(e, t) {
-        const o = d.removePopupIndex(e.name),
+    }), window.dismissAddStreamBlockPopup = function(t, e) {
+        const o = d.removePopupIndex(t.name),
             s = /^(.+)--(.+)\.(.+)$/.exec(o);
         if (s) {
             const o = document.getElementById(s[1]).closest(".stream-field"),
                 r = o && o._streamField;
             r._appendBlock({
                 model: `${s[2]}.${s[3]}`,
-                pk: t,
-                uuid: l()
-            }), r.wrapPreloader(r.update()), d.removeRelatedWindow(e), e.close()
-        }
-    }, window.dismissChangeStreamBlockPopup = function(e) {
-        const t = "change_" + d.removePopupIndex(e.name),
-            o = document.getElementById(t),
+                pk: e,
+                uuid: a()
+            }), r.wrapPreloader(r.updateBlocks()), d.removeRelatedWindow(t), t.close()
+        }
+    }, window.dismissChangeStreamBlockPopup = function(t) {
+        const e = "change_" + d.removePopupIndex(t.name),
+            o = document.getElementById(e),
             s = o && o.closest(".paper-widget"),
             r = s && s.firstElementChild;
-        (r && r._streamField).update(), d.removeRelatedWindow(e), e.close()
-    }, window.dismissDeleteStreamBlockPopup = function(e, t) {
-        const o = d.removePopupIndex(e.name),
+        (r && r._streamField).updateBlocks(), d.removeRelatedWindow(t), t.close()
+    }, window.dismissDeleteStreamBlockPopup = function(t, e) {
+        const o = d.removePopupIndex(t.name),
             s = /^(.+)--(.+)\.(.+)$/.exec(o);
         if (s) {
-            const t = document.getElementById(s[1]).closest(".stream-field"),
-                o = t && t._streamField;
-            o.wrapPreloader(o.update()), d.removeRelatedWindow(e), e.close()
+            const e = document.getElementById(s[1]).closest(".stream-field"),
+                o = e && e._streamField;
+            o.wrapPreloader(o.updateBlocks()), d.removeRelatedWindow(t), t.close()
         }
-    }, window.dismissRelatedLookupPopup = (p = window.dismissRelatedLookupPopup, (e, t) => {
-        const o = d.removePopupIndex(e.name),
+    }, window.dismissRelatedLookupPopup = (p = window.dismissRelatedLookupPopup, (t, e) => {
+        const o = d.removePopupIndex(t.name),
             s = /^(.+)--(.+)\.(.+)$/.exec(o);
         if (s) {
             const o = document.getElementById(s[1]).closest(".stream-field"),
                 r = o && o._streamField;
             r._appendBlock({
                 model: `${s[2]}.${s[3]}`,
-                pk: t,
-                uuid: l()
-            }), r.wrapPreloader(r.update()), d.removeRelatedWindow(e), e.close()
-        } else p(e, t)
+                pk: e,
+                uuid: a()
+            }), r.wrapPreloader(r.updateBlocks()), d.removeRelatedWindow(t), t.close()
+        } else p(t, e)
     })
 }();
 //# sourceMappingURL=widget.js.map
```

### Comparing `paper-streamfield-0.4.0/streamfield/static/streamfield/dist/widget.js.map` & `paper-streamfield-0.5.0rc1/streamfield/static/streamfield/dist/widget.js.map`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9052795031055901%*

 * *Differences: {"'mappings'": "'yBAAA,4HCMA,MAJA,SAAkBA,GAChB,MAAuB,iBAATA,GAAqB,OAAWA,EAChD,ECHA,OACEC,WAFmC,oBAAXC,QAA0BA,OAAOD,YAAcC,OAAOD,WAAWE,KAAKD,SCGhG,IAAIE,EACJ,MAAMC,EAAQ,IAAIC,WAAW,IACd,SAASC,IAEtB,IAAKH,IAEHA,EAAoC,oBAAXF,QAA0BA,OAAOE,iBAAmBF,OAAOE,gBAAgBD,KAAKD,SAEpGE,GACH,MAAM,IAAII,MAAM,4GAIpB,OAAOJ,EAAgBC,EACzB,CCXA,MAAMI,EAAY,GAElB,IAAK,IAAIC,EAAI,EAAGA,EAAI,MAAOA,EACzBD,EAAUE,MAAMD,EAAI,KAAOE,SAAS,IAAIC,MAAM,IAGzC,SAASC,EAAgBC,EAAKC,EAAS,GAG5C,OAAQP,EAAUM,EAAIC,EAAS,IAAMP,EAAUM,EAAIC,EAAS,IAAMP,EAAUM,EA […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "widget.js",
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "uuid",
         "randomUUID",
         "crypto",
         "bind",
         "getRandomValues",
         "rnds8",
@@ -33,24 +33,24 @@
         "element",
         "this",
         "field",
         "control",
         "querySelector",
         "CSS",
         "blocks",
-        "toolbar",
+        "buttons",
         "_sortable",
         "_initSortable",
         "_addListeners",
         "_updateBlockMap",
         "wrapPreloader",
         "Promise",
         "all",
-        "update",
-        "updateToolbar",
+        "updateBlocks",
+        "updateButtons",
         "STATUS",
         "value",
         "data",
         "JSON",
         "parse",
         "stringify",
         "status",
@@ -98,15 +98,14 @@
         "preventDefault",
         "disabled",
         "createModal",
         "modalClass",
         "title",
         "gettext",
         "body",
-        "buttons",
         "label",
         "buttonClass",
         "onClick",
         "popup",
         "autofocus",
         "remove",
         "onInit",
@@ -121,18 +120,18 @@
         "trigger",
         "isDefaultPrevented",
         "showStreamBlockPopup",
         "dropdownItem",
         "dropdownItemButton",
         "_appendBlock",
         "newValue",
-        "renderStream",
         "promise",
         "finally",
         "READY",
+        "renderStream",
         "renderUrl",
         "renderStreamUrl",
         "fetch",
         "method",
         "mode",
         "cache",
         "headers",
@@ -143,19 +142,18 @@
         "json",
         "innerHTML",
         "catch",
         "reason",
         "console",
         "error",
         "showErrors",
-        "renderToolbar",
-        "renderToolbarUrl",
+        "renderButtons",
         "field_id",
         "id",
-        "models",
+        "renderButtonsUrl",
         "triggeringLink",
         "showAdminPopup",
         "originalFunc",
         "XClass",
         "register",
         "init",
         "_streamField",
@@ -194,11 +192,11 @@
     "sourcesContent": [
         "export default /^(?:[0-9a-f]{8}-[0-9a-f]{4}-[1-5][0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}|00000000-0000-0000-0000-000000000000)$/i;",
         "import REGEX from './regex.js';\n\nfunction validate(uuid) {\n  return typeof uuid === 'string' && REGEX.test(uuid);\n}\n\nexport default validate;",
         "const randomUUID = typeof crypto !== 'undefined' && crypto.randomUUID && crypto.randomUUID.bind(crypto);\nexport default {\n  randomUUID\n};",
         "// Unique ID creation requires a high quality random # generator. In the browser we therefore\n// require the crypto API and do not support built-in fallback to lower quality random number\n// generators (like Math.random()).\nlet getRandomValues;\nconst rnds8 = new Uint8Array(16);\nexport default function rng() {\n  // lazy load so that environments that need to polyfill have a chance to do so\n  if (!getRandomValues) {\n    // getRandomValues needs to be invoked in a context where \"this\" is a Crypto implementation.\n    getRandomValues = typeof crypto !== 'undefined' && crypto.getRandomValues && crypto.getRandomValues.bind(crypto);\n\n    if (!getRandomValues) {\n      throw new Error('crypto.getRandomValues() not supported. See https://github.com/uuidjs/uuid#getrandomvalues-not-supported');\n    }\n  }\n\n  return getRandomValues(rnds8);\n}",
         "import validate from './validate.js';\n/**\n * Convert array of 16 byte values to UUID string format of the form:\n * XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX\n */\n\nconst byteToHex = [];\n\nfor (let i = 0; i < 256; ++i) {\n  byteToHex.push((i + 0x100).toString(16).slice(1));\n}\n\nexport function unsafeStringify(arr, offset = 0) {\n  // Note: Be careful editing this code!  It's been tuned for performance\n  // and works in ways you may not expect. See https://github.com/uuidjs/uuid/pull/434\n  return (byteToHex[arr[offset + 0]] + byteToHex[arr[offset + 1]] + byteToHex[arr[offset + 2]] + byteToHex[arr[offset + 3]] + '-' + byteToHex[arr[offset + 4]] + byteToHex[arr[offset + 5]] + '-' + byteToHex[arr[offset + 6]] + byteToHex[arr[offset + 7]] + '-' + byteToHex[arr[offset + 8]] + byteToHex[arr[offset + 9]] + '-' + byteToHex[arr[offset + 10]] + byteToHex[arr[offset + 11]] + byteToHex[arr[offset + 12]] + byteToHex[arr[offset + 13]] + byteToHex[arr[offset + 14]] + byteToHex[arr[offset + 15]]).toLowerCase();\n}\n\nfunction stringify(arr, offset = 0) {\n  const uuid = unsafeStringify(arr, offset); // Consistency check for valid UUID.  If this throws, it's likely due to one\n  // of the following:\n  // - One or more input array values don't map to a hex octet (leading to\n  // \"undefined\" in the uuid)\n  // - Invalid input values for the RFC `version` or `variant` fields\n\n  if (!validate(uuid)) {\n    throw TypeError('Stringified UUID is invalid');\n  }\n\n  return uuid;\n}\n\nexport default stringify;",
         "import native from './native.js';\nimport rng from './rng.js';\nimport { unsafeStringify } from './stringify.js';\n\nfunction v4(options, buf, offset) {\n  if (native.randomUUID && !buf && !options) {\n    return native.randomUUID();\n  }\n\n  options = options || {};\n  const rnds = options.random || (options.rng || rng)(); // Per 4.4, set bits for version and `clock_seq_hi_and_reserved`\n\n  rnds[6] = rnds[6] & 0x0f | 0x40;\n  rnds[8] = rnds[8] & 0x3f | 0x80; // Copy bytes to buffer, if provided\n\n  if (buf) {\n    offset = offset || 0;\n\n    for (let i = 0; i < 16; ++i) {\n      buf[offset + i] = rnds[i];\n    }\n\n    return buf;\n  }\n\n  return unsafeStringify(rnds);\n}\n\nexport default v4;",
-        "/* global gettext */\n/* global Sortable */\n/* global XClass */\nimport { v4 as uuid4, validate as uuid_validate } from \"uuid\";\n\nimport \"./widget.scss\";\n\nconst popupUtils = window.paperAdmin.popupUtils;\nconst modals = window.paperAdmin.modals;\n\nclass StreamField {\n    static STATUS = {\n        LOADING: \"loading\",\n        READY: \"ready\"\n    };\n\n    static CSS = {\n        field: \"stream-field\",\n        control: \"stream-field__control\",\n        blocks: \"stream-field__blocks\",\n        block: \"stream-field__block\",\n        toolbar: \"stream-field__toolbar\",\n        sortableHandler: \"stream-field__sortable-handler\",\n        changeBlockButton: \"stream-field__change-btn\",\n        deleteBlockButton: \"stream-field__delete-btn\",\n        dropdownItemButton: \"stream-field__dropdown-item\" // create or lookup block\n    };\n\n    constructor(element) {\n        this.field = element;\n        this.control = this.field.querySelector(`.${this.CSS.control}`);\n        this.blocks = this.field.querySelector(`.${this.CSS.blocks}`);\n        this.toolbar = this.field.querySelector(`.${this.CSS.toolbar}`);\n\n        this._sortable = this._initSortable();\n        this._addListeners();\n        this._updateBlockMap();\n\n        this.wrapPreloader(Promise.all([this.update(), this.updateToolbar()]));\n    }\n\n    get STATUS() {\n        return this.constructor.STATUS;\n    }\n\n    get CSS() {\n        return this.constructor.CSS;\n    }\n\n    /**\n     * @returns {Array}\n     */\n    get value() {\n        let data;\n        try {\n            data = JSON.parse(this.control.value);\n        } catch {\n            data = [];\n        }\n        return data;\n    }\n\n    /**\n     * @param {string|Array} data\n     */\n    set value(data) {\n        if (typeof data !== \"string\") {\n            data = JSON.stringify(data);\n        }\n        this.control.value = data;\n    }\n\n    /**\n     * @returns {string}\n     */\n    get status() {\n        return Object.values(this.STATUS).find(value => {\n            return this.field.classList.contains(`${this.CSS.field}--${value}`);\n        });\n    }\n\n    /**\n     * @param {string} status\n     */\n    set status(status) {\n        Object.values(this.STATUS).forEach(value => {\n            this.field.classList.toggle(`${this.CSS.field}--${value}`, status === value);\n        });\n    }\n\n    /**\n     * @returns {String[]}\n     */\n    get allowedModels() {\n        return JSON.parse(this.control.dataset.allowedModels);\n    }\n\n    /**\n     * @returns {HTMLElement[]}\n     */\n    getBlocks() {\n        return Array.from(this.blocks.querySelectorAll(`.${this.CSS.block}`));\n    }\n\n    /**\n     * @param {string} uuid\n     * @returns {Object}\n     */\n    getBlockByUUID(uuid) {\n        return this._blockMap[uuid];\n    }\n\n    destroy() {\n        if (this._sortable) {\n            this._sortable.destroy();\n        }\n\n        // TODO: remove event listeners\n    }\n\n    /**\n     * \u0421\u043e\u0437\u0434\u0430\u0451\u0442 \u043e\u0431\u044a\u0435\u043a\u0442 \u0434\u043b\u044f \u0431\u044b\u0441\u0442\u0440\u043e\u0433\u043e \u043f\u043e\u0438\u0441\u043a\u0430 \u0431\u043b\u043e\u043a\u043e\u0432 \u043f\u043e UUID.\n     *\n     * @returns {Object}\n     */\n    _updateBlockMap() {\n        let hasBadBlocks = false;\n        const result = {};\n\n        const processedValue = this.value.map(record => {\n            let uuid = record[\"uuid\"];\n            if (typeof uuid === \"string\" && uuid_validate(uuid)) {\n                return (result[uuid] = record);\n            } else {\n                hasBadBlocks = true;\n                uuid = uuid4();\n                return (result[uuid] = { uuid: uuid });\n            }\n        });\n\n        this._blockMap = result;\n        if (processedValue) {\n            this.value = processedValue;\n        }\n    }\n\n    /**\n     * @returns {*}\n     * @private\n     */\n    _initSortable() {\n        return Sortable.create(this.blocks, {\n            animation: 0,\n            draggable: `.${this.CSS.block}`,\n            filter: (event, target) => {\n                if (this.status === this.STATUS.LOADING) {\n                    return true;\n                }\n\n                if (!target) {\n                    return true;\n                }\n            },\n            handle: `.${this.CSS.sortableHandler}`,\n            ghostClass: \"sortable-ghost\",\n            onEnd: () => {\n                this.save();\n            }\n        });\n    }\n\n    _addListeners() {\n        this.field.addEventListener(\"click\", event => {\n            const deleteButton = event.target.closest(`.${this.CSS.deleteBlockButton}`);\n            if (deleteButton) {\n                event.preventDefault();\n                deleteButton.disabled = true;\n\n                modals.createModal({\n                    modalClass: \"paper-modal--warning fade\",\n                    title: gettext(\"Confirm deletion\"),\n                    body: gettext(\"Are you sure you want to <b>DELETE</b> selected block from this field?\"),\n                    buttons: [\n                        {\n                            label: gettext(\"Cancel\"),\n                            buttonClass: \"btn-light\",\n                            onClick: (event, popup) => {\n                                popup.destroy();\n                            }\n                        },\n                        {\n                            autofocus: true,\n                            label: gettext(\"Delete\"),\n                            buttonClass: \"btn-danger\",\n                            onClick: (event, popup) => {\n                                popup.destroy();\n\n                                const block = deleteButton.closest(`.${this.CSS.block}`);\n                                block.remove();\n\n                                this.save();\n                                this.wrapPreloader(this.update());\n                            }\n                        }\n                    ],\n                    onInit: function () {\n                        this.show();\n                    },\n                    onDestroy: function () {\n                        deleteButton.disabled = false;\n                    }\n                });\n            }\n\n            const changeButton = event.target.closest(`.${this.CSS.changeBlockButton}`);\n            if (changeButton) {\n                event.preventDefault();\n                const jQueryEvent = $.Event(\"django:show-related\", { href: changeButton.href });\n                $(changeButton).trigger(jQueryEvent);\n                if (!jQueryEvent.isDefaultPrevented()) {\n                    showStreamBlockPopup(changeButton);\n                }\n            }\n\n            const dropdownItem = event.target.closest(`.${this.CSS.dropdownItemButton}`);\n            if (dropdownItem) {\n                event.preventDefault();\n                const jQueryEvent = $.Event(\"django:show-related\", { href: dropdownItem.href });\n                $(dropdownItem).trigger(jQueryEvent);\n                if (!jQueryEvent.isDefaultPrevented()) {\n                    showStreamBlockPopup(dropdownItem);\n                }\n            }\n        });\n    }\n\n    /**\n     * @param {Object} block\n     * @private\n     */\n    _appendBlock(block) {\n        const uuid = block.uuid;\n        if (!uuid_validate(uuid)) {\n            throw new Error(\"Invalid UUID\");\n        }\n\n        const newValue = this.value;\n        newValue.push(block);\n        this.value = newValue;\n\n        this._blockMap[uuid] = block;\n    }\n\n    save() {\n        this.value = this.getBlocks().map(block => {\n            const uuid = block.dataset.uuid;\n            return this.getBlockByUUID(uuid);\n        });\n    }\n\n    update() {\n        return this.renderStream(this.value);\n    }\n\n    /**\n     * @param {Promise} promise\n     * @returns {Promise}\n     */\n    wrapPreloader(promise) {\n        this.status = this.STATUS.LOADING;\n        return promise.finally(() => {\n            this.status = this.STATUS.READY;\n        });\n    }\n\n    renderStream(data) {\n        const renderUrl = this.field.dataset.renderStreamUrl;\n        return fetch(renderUrl, {\n            method: \"POST\",\n            mode: \"same-origin\",\n            cache: \"no-store\",\n            headers: {\n                \"Content-Type\": \"application/json;charset=utf-8\"\n            },\n            body: JSON.stringify(data)\n        })\n            .then(response => {\n                if (!response.ok) {\n                    throw `${response.status} ${response.statusText}`;\n                }\n                return response.json();\n            })\n            .then(response => {\n                this.blocks.innerHTML = response.blocks;\n            })\n            .catch(reason => {\n                if (reason instanceof Error) {\n                    // JS-\u043e\u0448\u0438\u0431\u043a\u0438 \u0434\u0443\u0431\u043b\u0438\u0440\u0443\u0435\u043c \u0432 \u043a\u043e\u043d\u0441\u043e\u043b\u044c\n                    console.error(reason);\n                }\n                modals.showErrors(reason);\n            });\n    }\n\n    renderToolbar(data) {\n        const renderUrl = this.field.dataset.renderToolbarUrl;\n        return fetch(renderUrl, {\n            method: \"POST\",\n            mode: \"same-origin\",\n            cache: \"no-store\",\n            headers: {\n                \"Content-Type\": \"application/json;charset=utf-8\"\n            },\n            body: JSON.stringify(data)\n        })\n            .then(response => {\n                if (!response.ok) {\n                    throw `${response.status} ${response.statusText}`;\n                }\n                return response.json();\n            })\n            .then(response => {\n                this.toolbar.innerHTML = response.toolbar;\n            });\n    }\n\n    updateToolbar() {\n        return this.renderToolbar({\n            field_id: this.control.id,\n            models: this.allowedModels\n        });\n    }\n}\n\nXClass.register(\"paper-streamfield\", {\n    init: function (element) {\n        element._streamField = new StreamField(element, this);\n    },\n    destroy: function (element) {\n        if (element._streamField) {\n            element._streamField.destroy();\n            delete element._streamField;\n        }\n    }\n});\n\n/**\n * @param {HTMLElement} triggeringLink\n */\nfunction showStreamBlockPopup(triggeringLink) {\n    return popupUtils.showAdminPopup(triggeringLink, /^(change|add|lookup)_/, true);\n}\n\n/**\n * @param {Window} win\n * @param {String} newId\n */\nfunction dismissAddStreamBlockPopup(win, newId) {\n    const name = popupUtils.removePopupIndex(win.name);\n    const match = /^(.+)--(.+)\\.(.+)$/.exec(name);\n    if (match) {\n        const control = document.getElementById(match[1]);\n        const field = control.closest(\".stream-field\");\n        const streamField = field && field._streamField;\n\n        streamField._appendBlock({\n            model: `${match[2]}.${match[3]}`,\n            pk: newId,\n            uuid: uuid4()\n        });\n\n        streamField.wrapPreloader(streamField.update());\n\n        popupUtils.removeRelatedWindow(win);\n        win.close();\n    }\n}\n\n/**\n * @param {Window} win\n */\nfunction dismissChangeStreamBlockPopup(win) {\n    const name = \"change_\" + popupUtils.removePopupIndex(win.name);\n    const element = document.getElementById(name);\n    const fieldWrapper = element && element.closest(\".paper-widget\");\n    const field = fieldWrapper && fieldWrapper.firstElementChild;\n    const instance = field && field._streamField;\n\n    instance.update();\n\n    popupUtils.removeRelatedWindow(win);\n    win.close();\n}\n\n/**\n * @param {Window} win\n * @param {String} objId\n */\nfunction dismissDeleteStreamBlockPopup(win, objId) {\n    const name = popupUtils.removePopupIndex(win.name);\n    const match = /^(.+)--(.+)\\.(.+)$/.exec(name);\n    if (match) {\n        const control = document.getElementById(match[1]);\n        const field = control.closest(\".stream-field\");\n        const streamField = field && field._streamField;\n\n        streamField.wrapPreloader(streamField.update());\n\n        popupUtils.removeRelatedWindow(win);\n        win.close();\n    }\n}\n\n/**\n * \u041e\u0431\u0451\u0440\u0442\u043a\u0430 \u043d\u0430\u0434 Django-\u043e\u0431\u0440\u0430\u0431\u043e\u0442\u0447\u0438\u043a\u043e\u043c `window.dismissRelatedLookupPopup`.\n * @param {Function} originalFunc\n */\nfunction dismissLookupStreamBlockPopup(originalFunc) {\n    return (win, chosenId) => {\n        const name = popupUtils.removePopupIndex(win.name);\n        const match = /^(.+)--(.+)\\.(.+)$/.exec(name);\n        if (match) {\n            const control = document.getElementById(match[1]);\n            const field = control.closest(\".stream-field\");\n            const streamField = field && field._streamField;\n\n            streamField._appendBlock({\n                model: `${match[2]}.${match[3]}`,\n                pk: chosenId,\n                uuid: uuid4()\n            });\n\n            streamField.wrapPreloader(streamField.update());\n\n            popupUtils.removeRelatedWindow(win);\n            win.close();\n        } else {\n            originalFunc(win, chosenId);\n        }\n    };\n}\n\nwindow.dismissAddStreamBlockPopup = dismissAddStreamBlockPopup;\nwindow.dismissChangeStreamBlockPopup = dismissChangeStreamBlockPopup;\nwindow.dismissDeleteStreamBlockPopup = dismissDeleteStreamBlockPopup;\n\n// Wrap default `dismissRelatedLookupPopup`.\nwindow.dismissRelatedLookupPopup = dismissLookupStreamBlockPopup(window.dismissRelatedLookupPopup);\n"
+        "/* global gettext */\n/* global Sortable */\n/* global XClass */\nimport { v4 as uuid4, validate as uuid_validate } from \"uuid\";\n\nimport \"./widget.scss\";\n\nconst popupUtils = window.paperAdmin.popupUtils;\nconst modals = window.paperAdmin.modals;\n\nclass StreamField {\n    static STATUS = {\n        LOADING: \"loading\",\n        READY: \"ready\"\n    };\n\n    static CSS = {\n        field: \"stream-field\",\n        control: \"stream-field__control\",\n        blocks: \"stream-field__blocks\",\n        block: \"stream-field__block\",\n        buttons: \"stream-field__buttons\",\n        sortableHandler: \"stream-field__sortable-handler\",\n        changeBlockButton: \"stream-field__change-btn\",\n        deleteBlockButton: \"stream-field__delete-btn\",\n        dropdownItemButton: \"stream-field__dropdown-item\" // create or lookup block\n    };\n\n    constructor(element) {\n        this.field = element;\n        this.control = this.field.querySelector(`.${this.CSS.control}`);\n        this.blocks = this.field.querySelector(`.${this.CSS.blocks}`);\n        this.buttons = this.field.querySelector(`.${this.CSS.buttons}`);\n\n        this._sortable = this._initSortable();\n        this._addListeners();\n        this._updateBlockMap();\n\n        this.wrapPreloader(Promise.all([this.updateBlocks(), this.updateButtons()]));\n    }\n\n    get STATUS() {\n        return this.constructor.STATUS;\n    }\n\n    get CSS() {\n        return this.constructor.CSS;\n    }\n\n    /**\n     * @returns {Array}\n     */\n    get value() {\n        let data;\n        try {\n            data = JSON.parse(this.control.value);\n        } catch {\n            data = [];\n        }\n        return data;\n    }\n\n    /**\n     * @param {string|Array} data\n     */\n    set value(data) {\n        if (typeof data !== \"string\") {\n            data = JSON.stringify(data);\n        }\n        this.control.value = data;\n    }\n\n    /**\n     * @returns {string}\n     */\n    get status() {\n        return Object.values(this.STATUS).find(value => {\n            return this.field.classList.contains(`${this.CSS.field}--${value}`);\n        });\n    }\n\n    /**\n     * @param {string} status\n     */\n    set status(status) {\n        Object.values(this.STATUS).forEach(value => {\n            this.field.classList.toggle(`${this.CSS.field}--${value}`, status === value);\n        });\n    }\n\n    /**\n     * @returns {String[]}\n     */\n    get allowedModels() {\n        return JSON.parse(this.control.dataset.allowedModels);\n    }\n\n    /**\n     * @returns {HTMLElement[]}\n     */\n    getBlocks() {\n        return Array.from(this.blocks.querySelectorAll(`.${this.CSS.block}`));\n    }\n\n    /**\n     * @param {string} uuid\n     * @returns {Object}\n     */\n    getBlockByUUID(uuid) {\n        return this._blockMap[uuid];\n    }\n\n    destroy() {\n        if (this._sortable) {\n            this._sortable.destroy();\n        }\n\n        // TODO: remove event listeners\n    }\n\n    /**\n     * \u0421\u043e\u0437\u0434\u0430\u0451\u0442 \u043e\u0431\u044a\u0435\u043a\u0442 \u0434\u043b\u044f \u0431\u044b\u0441\u0442\u0440\u043e\u0433\u043e \u043f\u043e\u0438\u0441\u043a\u0430 \u0431\u043b\u043e\u043a\u043e\u0432 \u043f\u043e UUID.\n     *\n     * @returns {Object}\n     */\n    _updateBlockMap() {\n        let hasBadBlocks = false;\n        const result = {};\n\n        const processedValue = this.value.map(record => {\n            let uuid = record[\"uuid\"];\n            if (typeof uuid === \"string\" && uuid_validate(uuid)) {\n                return (result[uuid] = record);\n            } else {\n                hasBadBlocks = true;\n                uuid = uuid4();\n                return (result[uuid] = { uuid: uuid });\n            }\n        });\n\n        this._blockMap = result;\n        if (processedValue) {\n            this.value = processedValue;\n        }\n    }\n\n    /**\n     * @returns {*}\n     * @private\n     */\n    _initSortable() {\n        return Sortable.create(this.blocks, {\n            animation: 0,\n            draggable: `.${this.CSS.block}`,\n            filter: (event, target) => {\n                if (this.status === this.STATUS.LOADING) {\n                    return true;\n                }\n\n                if (!target) {\n                    return true;\n                }\n            },\n            handle: `.${this.CSS.sortableHandler}`,\n            ghostClass: \"sortable-ghost\",\n            onEnd: () => {\n                this.save();\n            }\n        });\n    }\n\n    _addListeners() {\n        this.field.addEventListener(\"click\", event => {\n            const deleteButton = event.target.closest(`.${this.CSS.deleteBlockButton}`);\n            if (deleteButton) {\n                event.preventDefault();\n                deleteButton.disabled = true;\n\n                modals.createModal({\n                    modalClass: \"paper-modal--warning fade\",\n                    title: gettext(\"Confirm deletion\"),\n                    body: gettext(\"Are you sure you want to <b>DELETE</b> selected block from this field?\"),\n                    buttons: [\n                        {\n                            label: gettext(\"Cancel\"),\n                            buttonClass: \"btn-light\",\n                            onClick: (event, popup) => {\n                                popup.destroy();\n                            }\n                        },\n                        {\n                            autofocus: true,\n                            label: gettext(\"Delete\"),\n                            buttonClass: \"btn-danger\",\n                            onClick: (event, popup) => {\n                                popup.destroy();\n\n                                const block = deleteButton.closest(`.${this.CSS.block}`);\n                                block.remove();\n\n                                this.save();\n                                this.wrapPreloader(this.updateBlocks());\n                            }\n                        }\n                    ],\n                    onInit: function () {\n                        this.show();\n                    },\n                    onDestroy: function () {\n                        deleteButton.disabled = false;\n                    }\n                });\n            }\n\n            const changeButton = event.target.closest(`.${this.CSS.changeBlockButton}`);\n            if (changeButton) {\n                event.preventDefault();\n                const jQueryEvent = $.Event(\"django:show-related\", { href: changeButton.href });\n                $(changeButton).trigger(jQueryEvent);\n                if (!jQueryEvent.isDefaultPrevented()) {\n                    showStreamBlockPopup(changeButton);\n                }\n            }\n\n            const dropdownItem = event.target.closest(`.${this.CSS.dropdownItemButton}`);\n            if (dropdownItem) {\n                event.preventDefault();\n                const jQueryEvent = $.Event(\"django:show-related\", { href: dropdownItem.href });\n                $(dropdownItem).trigger(jQueryEvent);\n                if (!jQueryEvent.isDefaultPrevented()) {\n                    showStreamBlockPopup(dropdownItem);\n                }\n            }\n        });\n    }\n\n    /**\n     * @param {Object} block\n     * @private\n     */\n    _appendBlock(block) {\n        const uuid = block.uuid;\n        if (!uuid_validate(uuid)) {\n            throw new Error(\"Invalid UUID\");\n        }\n\n        const newValue = this.value;\n        newValue.push(block);\n        this.value = newValue;\n\n        this._blockMap[uuid] = block;\n    }\n\n    save() {\n        this.value = this.getBlocks().map(block => {\n            const uuid = block.dataset.uuid;\n            return this.getBlockByUUID(uuid);\n        });\n    }\n\n    /**\n     * @param {Promise} promise\n     * @returns {Promise}\n     */\n    wrapPreloader(promise) {\n        this.status = this.STATUS.LOADING;\n        return promise.finally(() => {\n            this.status = this.STATUS.READY;\n        });\n    }\n\n    updateBlocks() {\n        return this.renderStream({\n            allowedModels: this.allowedModels,\n            value: this.value\n        });\n    }\n\n    renderStream(data) {\n        const renderUrl = this.field.dataset.renderStreamUrl;\n        return fetch(renderUrl, {\n            method: \"POST\",\n            mode: \"same-origin\",\n            cache: \"no-store\",\n            headers: {\n                \"Content-Type\": \"application/json;charset=utf-8\"\n            },\n            body: JSON.stringify(data)\n        })\n            .then(response => {\n                if (!response.ok) {\n                    throw `${response.status} ${response.statusText}`;\n                }\n                return response.json();\n            })\n            .then(response => {\n                this.blocks.innerHTML = response.blocks;\n            })\n            .catch(reason => {\n                if (reason instanceof Error) {\n                    // JS-\u043e\u0448\u0438\u0431\u043a\u0438 \u0434\u0443\u0431\u043b\u0438\u0440\u0443\u0435\u043c \u0432 \u043a\u043e\u043d\u0441\u043e\u043b\u044c\n                    console.error(reason);\n                }\n                modals.showErrors(reason);\n            });\n    }\n\n    updateButtons() {\n        return this.renderButtons({\n            field_id: this.control.id,\n            allowedModels: this.allowedModels\n        });\n    }\n\n    renderButtons(data) {\n        const renderUrl = this.field.dataset.renderButtonsUrl;\n        return fetch(renderUrl, {\n            method: \"POST\",\n            mode: \"same-origin\",\n            cache: \"no-store\",\n            headers: {\n                \"Content-Type\": \"application/json;charset=utf-8\"\n            },\n            body: JSON.stringify(data)\n        })\n            .then(response => {\n                if (!response.ok) {\n                    throw `${response.status} ${response.statusText}`;\n                }\n                return response.json();\n            })\n            .then(response => {\n                this.buttons.innerHTML = response.buttons;\n            });\n    }\n}\n\nXClass.register(\"paper-streamfield\", {\n    init: function (element) {\n        element._streamField = new StreamField(element, this);\n    },\n    destroy: function (element) {\n        if (element._streamField) {\n            element._streamField.destroy();\n            delete element._streamField;\n        }\n    }\n});\n\n/**\n * @param {HTMLElement} triggeringLink\n */\nfunction showStreamBlockPopup(triggeringLink) {\n    return popupUtils.showAdminPopup(triggeringLink, /^(change|add|lookup)_/, true);\n}\n\n/**\n * @param {Window} win\n * @param {String} newId\n */\nfunction dismissAddStreamBlockPopup(win, newId) {\n    const name = popupUtils.removePopupIndex(win.name);\n    const match = /^(.+)--(.+)\\.(.+)$/.exec(name);\n    if (match) {\n        const control = document.getElementById(match[1]);\n        const field = control.closest(\".stream-field\");\n        const streamField = field && field._streamField;\n\n        streamField._appendBlock({\n            model: `${match[2]}.${match[3]}`,\n            pk: newId,\n            uuid: uuid4()\n        });\n\n        streamField.wrapPreloader(streamField.updateBlocks());\n\n        popupUtils.removeRelatedWindow(win);\n        win.close();\n    }\n}\n\n/**\n * @param {Window} win\n */\nfunction dismissChangeStreamBlockPopup(win) {\n    const name = \"change_\" + popupUtils.removePopupIndex(win.name);\n    const element = document.getElementById(name);\n    const fieldWrapper = element && element.closest(\".paper-widget\");\n    const field = fieldWrapper && fieldWrapper.firstElementChild;\n    const instance = field && field._streamField;\n\n    instance.updateBlocks();\n\n    popupUtils.removeRelatedWindow(win);\n    win.close();\n}\n\n/**\n * @param {Window} win\n * @param {String} objId\n */\nfunction dismissDeleteStreamBlockPopup(win, objId) {\n    const name = popupUtils.removePopupIndex(win.name);\n    const match = /^(.+)--(.+)\\.(.+)$/.exec(name);\n    if (match) {\n        const control = document.getElementById(match[1]);\n        const field = control.closest(\".stream-field\");\n        const streamField = field && field._streamField;\n\n        streamField.wrapPreloader(streamField.updateBlocks());\n\n        popupUtils.removeRelatedWindow(win);\n        win.close();\n    }\n}\n\n/**\n * \u041e\u0431\u0451\u0440\u0442\u043a\u0430 \u043d\u0430\u0434 Django-\u043e\u0431\u0440\u0430\u0431\u043e\u0442\u0447\u0438\u043a\u043e\u043c `window.dismissRelatedLookupPopup`.\n * @param {Function} originalFunc\n */\nfunction dismissLookupStreamBlockPopup(originalFunc) {\n    return (win, chosenId) => {\n        const name = popupUtils.removePopupIndex(win.name);\n        const match = /^(.+)--(.+)\\.(.+)$/.exec(name);\n        if (match) {\n            const control = document.getElementById(match[1]);\n            const field = control.closest(\".stream-field\");\n            const streamField = field && field._streamField;\n\n            streamField._appendBlock({\n                model: `${match[2]}.${match[3]}`,\n                pk: chosenId,\n                uuid: uuid4()\n            });\n\n            streamField.wrapPreloader(streamField.updateBlocks());\n\n            popupUtils.removeRelatedWindow(win);\n            win.close();\n        } else {\n            originalFunc(win, chosenId);\n        }\n    };\n}\n\nwindow.dismissAddStreamBlockPopup = dismissAddStreamBlockPopup;\nwindow.dismissChangeStreamBlockPopup = dismissChangeStreamBlockPopup;\nwindow.dismissDeleteStreamBlockPopup = dismissDeleteStreamBlockPopup;\n\n// Wrap default `dismissRelatedLookupPopup`.\nwindow.dismissRelatedLookupPopup = dismissLookupStreamBlockPopup(window.dismissRelatedLookupPopup);\n"
     ],
     "version": 3
 }
```

### Comparing `paper-streamfield-0.4.0/streamfield/templates/streamfield/admin/invalid_block.html` & `paper-streamfield-0.5.0rc1/streamfield/templates/streamfield/admin/invalid_block.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 {% extends "streamfield/admin/block.html" %}
-
 {% load i18n %}
 
 
-{% block classes %}stream-field__block stream-field__block--invalid{% endblock classes %}
+{% block extra_classes %}stream-field__block--invalid{% endblock extra_classes %}
+
 
 {% block content %}
-  {{ title }}
-  <br>
-  <small class="text-muted">{{ model }} ({% trans "Primary key" %}: {{ pk }})</small>
+  <div class="stream-field__content">
+    <p class="stream-field__title">{% blocktrans with reason=reason %}Error: {{ reason }}{% endblocktrans %}</p>
+    <p class="stream-field__type">{{ model }} #{{ pk }}</p>
+  </div>
 {% endblock content %}
 
-{% block tools %}
-  <div class="btn-square-group">
-    <button type="button"
-            class="stream-field__delete-btn btn btn-square btn-sm btn-square--danger"
-            data-toggle="tooltip"
-            data-placement="top"
-            data-trigger="hover"
-            data-html="true"
-            title="{{ delete_button.title }}">
-      <i class="{{ delete_button.icon }}"></i>
-    </button>
-  </div>
-{% endblock %}
+
+{% block tool-items %}
+  <button type="button"
+          class="stream-field__delete-btn btn btn-square btn-sm btn-square--danger bi-trash"
+          data-xclass="bs-tooltip"
+          data-placement="top"
+          data-trigger="hover"
+          data-html="true"
+          title="{{ _("Delete") }}">
+  </button>
+{% endblock tool-items %}
```

### Comparing `paper-streamfield-0.4.0/streamfield/templates/streamfield/admin/popup_response.html` & `paper-streamfield-0.5.0rc1/streamfield/templates/streamfield/admin/popup_response.html`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.4.0/streamfield/templates/streamfield/admin/toolbar.html` & `paper-streamfield-0.5.0rc1/streamfield/templates/streamfield/admin/buttons.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% load i18n %}
 
 <div class="stream-field__dropdown dropdown d-inline-block">
   <button class="btn-success btn dropdown-toggle" type="button" data-toggle="dropdown" aria-expanded="false">
     <i class="bi-plus-lg"></i>
-    {% trans "Create new block" %}
+    <span>{% trans "Create new block" %}</span>
   </button>
   <ul class="stream-field__dropdown-menu dropdown-menu">
     {% for model in creatable_models %}
       <li role="presentation">
         <a class="stream-field__dropdown-item dropdown-item"
            href="{{ model.url }}"
            id="{{ model.id }}"
@@ -18,15 +18,15 @@
     {% endfor %}
   </ul>
 </div>
 
 <div class="stream-field__dropdown dropdown d-inline-block">
   <button class="btn-info btn dropdown-toggle" type="button" data-toggle="dropdown" aria-expanded="false">
     <i class="bi-search"></i>
-    {% trans "Lookup block" %}
+    <span>{% trans "Lookup block" %}</span>
   </button>
   <ul class="stream-field__dropdown-menu dropdown-menu">
     {% for model in searchable_models %}
       <li role="presentation">
         <a class="stream-field__dropdown-item dropdown-item"
            href="{{ model.url }}"
            id="{{ model.id }}"
```

### Comparing `paper-streamfield-0.4.0/streamfield/templatetags/streamfield.py` & `paper-streamfield-0.5.0rc1/streamfield/templatetags/streamfield.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,41 +5,40 @@
 from .. import helpers
 
 try:
     import jinja2
 except ImportError:
     jinja2 = None
 
-
 register = Library()
 
 
 @register.simple_tag(name="render_stream", takes_context=True)
 def do_render_stream(context, stream: str, **kwargs):
     request = context.get("request", None)
-    context = {
+    context = dict(kwargs, **{
         "parent_context": context.flatten(),
-    }
-    context.update(kwargs)
+    })
     output = helpers.render_stream(stream, context, request=request)
     return mark_safe(output)
 
 
 if jinja2 is not None:
     class StreamFieldExtension(StandaloneTag):
+        safe_output = True
         tags = {"render_stream"}
 
         def render(self, stream: str, **kwargs):
             request = self.context.get("request", None)
-            context = {
+            context = dict(kwargs, **{
                 "parent_context": self.context,
-            }
-            context.update(kwargs)
+            })
             return helpers.render_stream(stream, context, request=request)
 
+
     # django-jinja support
     try:
         from django_jinja import library
     except ImportError:
         pass
     else:
         library.extension(StreamFieldExtension)
```


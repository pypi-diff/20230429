# Comparing `tmp/frogmouth-0.2.0.tar.gz` & `tmp/frogmouth-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frogmouth-0.2.0.tar", max compression
+gzip compressed data, was "frogmouth-0.2.1.tar", max compression
```

## Comparing `frogmouth-0.2.0.tar` & `frogmouth-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1072 2023-04-27 14:46:52.801782 frogmouth-0.2.0/LICENSE
--rw-r--r--   0        0        0     2704 2023-04-29 14:55:46.077902 frogmouth-0.2.0/README.md
--rw-r--r--   0        0        0      283 2023-04-27 14:46:52.802054 frogmouth-0.2.0/frogmouth/__init__.py
--rw-r--r--   0        0        0      112 2023-04-27 14:46:52.802125 frogmouth-0.2.0/frogmouth/__main__.py
--rw-r--r--   0        0        0       74 2023-04-27 14:46:52.802222 frogmouth-0.2.0/frogmouth/app/__init__.py
--rw-r--r--   0        0        0     2110 2023-04-27 14:46:52.802301 frogmouth-0.2.0/frogmouth/app/app.py
--rw-r--r--   0        0        0      395 2023-04-27 14:46:52.802403 frogmouth-0.2.0/frogmouth/data/__init__.py
--rw-r--r--   0        0        0     1639 2023-04-27 14:46:52.802497 frogmouth-0.2.0/frogmouth/data/bookmarks.py
--rw-r--r--   0        0        0     2166 2023-04-27 14:46:52.802580 frogmouth-0.2.0/frogmouth/data/config.py
--rw-r--r--   0        0        0      582 2023-04-27 14:46:52.802650 frogmouth-0.2.0/frogmouth/data/data_directory.py
--rw-r--r--   0        0        0     1370 2023-04-27 14:46:52.802714 frogmouth-0.2.0/frogmouth/data/history.py
--rw-r--r--   0        0        0      354 2023-04-27 14:46:52.802828 frogmouth-0.2.0/frogmouth/dialogs/__init__.py
--rw-r--r--   0        0        0      565 2023-04-28 13:52:42.406602 frogmouth-0.2.0/frogmouth/dialogs/error.py
--rw-r--r--   0        0        0     4483 2023-04-29 14:55:46.078480 frogmouth-0.2.0/frogmouth/dialogs/help_dialog.py
--rw-r--r--   0        0        0      269 2023-04-27 14:55:30.387330 frogmouth-0.2.0/frogmouth/dialogs/information.py
--rw-r--r--   0        0        0     4278 2023-04-27 14:46:52.803185 frogmouth-0.2.0/frogmouth/dialogs/input_dialog.py
--rw-r--r--   0        0        0     2168 2023-04-28 17:16:37.419494 frogmouth-0.2.0/frogmouth/dialogs/text_dialog.py
--rw-r--r--   0        0        0     4898 2023-04-27 14:46:52.803359 frogmouth-0.2.0/frogmouth/dialogs/yes_no_dialog.py
--rw-r--r--   0        0        0       83 2023-04-27 14:46:52.803485 frogmouth-0.2.0/frogmouth/screens/__init__.py
--rw-r--r--   0        0        0    19015 2023-04-29 14:55:46.086907 frogmouth-0.2.0/frogmouth/screens/main.py
--rw-r--r--   0        0        0      327 2023-04-27 14:46:52.803762 frogmouth-0.2.0/frogmouth/utility/__init__.py
--rw-r--r--   0        0        0      894 2023-04-28 13:00:47.734733 frogmouth-0.2.0/frogmouth/utility/advertising.py
--rw-r--r--   0        0        0     4237 2023-04-27 14:46:52.803923 frogmouth-0.2.0/frogmouth/utility/forge.py
--rw-r--r--   0        0        0     1205 2023-04-27 14:46:52.804003 frogmouth-0.2.0/frogmouth/utility/type_tests.py
--rw-r--r--   0        0        0      184 2023-04-27 14:46:52.804110 frogmouth-0.2.0/frogmouth/widgets/__init__.py
--rw-r--r--   0        0        0     4398 2023-04-29 14:55:46.079307 frogmouth-0.2.0/frogmouth/widgets/navigation.py
--rw-r--r--   0        0        0      298 2023-04-27 14:46:52.804311 frogmouth-0.2.0/frogmouth/widgets/navigation_panes/__init__.py
--rw-r--r--   0        0        0     5889 2023-04-29 14:55:46.079533 frogmouth-0.2.0/frogmouth/widgets/navigation_panes/bookmarks.py
--rw-r--r--   0        0        0     3235 2023-04-29 14:55:46.079738 frogmouth-0.2.0/frogmouth/widgets/navigation_panes/history.py
--rw-r--r--   0        0        0     3412 2023-04-29 14:55:46.079932 frogmouth-0.2.0/frogmouth/widgets/navigation_panes/local_files.py
--rw-r--r--   0        0        0      667 2023-04-29 14:55:46.080110 frogmouth-0.2.0/frogmouth/widgets/navigation_panes/navigation_pane.py
--rw-r--r--   0        0        0     1704 2023-04-29 14:55:46.080286 frogmouth-0.2.0/frogmouth/widgets/navigation_panes/table_of_contents.py
--rw-r--r--   0        0        0    11675 2023-04-28 17:16:37.437633 frogmouth-0.2.0/frogmouth/widgets/omnibox.py
--rw-r--r--   0        0        0     9806 2023-04-27 15:34:09.464460 frogmouth-0.2.0/frogmouth/widgets/viewer.py
--rw-r--r--   0        0        0     1415 2023-04-28 17:16:37.442604 frogmouth-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4232 1970-01-01 00:00:00.000000 frogmouth-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-27 14:46:52.801782 frogmouth-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2704 2023-04-29 14:55:46.077902 frogmouth-0.2.1/README.md
+-rw-r--r--   0        0        0      283 2023-04-27 14:46:52.802054 frogmouth-0.2.1/frogmouth/__init__.py
+-rw-r--r--   0        0        0      112 2023-04-27 14:46:52.802125 frogmouth-0.2.1/frogmouth/__main__.py
+-rw-r--r--   0        0        0       74 2023-04-27 14:46:52.802222 frogmouth-0.2.1/frogmouth/app/__init__.py
+-rw-r--r--   0        0        0     2110 2023-04-27 14:46:52.802301 frogmouth-0.2.1/frogmouth/app/app.py
+-rw-r--r--   0        0        0      395 2023-04-27 14:46:52.802403 frogmouth-0.2.1/frogmouth/data/__init__.py
+-rw-r--r--   0        0        0     1639 2023-04-27 14:46:52.802497 frogmouth-0.2.1/frogmouth/data/bookmarks.py
+-rw-r--r--   0        0        0     2166 2023-04-27 14:46:52.802580 frogmouth-0.2.1/frogmouth/data/config.py
+-rw-r--r--   0        0        0      582 2023-04-27 14:46:52.802650 frogmouth-0.2.1/frogmouth/data/data_directory.py
+-rw-r--r--   0        0        0     1370 2023-04-27 14:46:52.802714 frogmouth-0.2.1/frogmouth/data/history.py
+-rw-r--r--   0        0        0      354 2023-04-27 14:46:52.802828 frogmouth-0.2.1/frogmouth/dialogs/__init__.py
+-rw-r--r--   0        0        0      565 2023-04-28 13:52:42.406602 frogmouth-0.2.1/frogmouth/dialogs/error.py
+-rw-r--r--   0        0        0     4483 2023-04-29 14:55:46.078480 frogmouth-0.2.1/frogmouth/dialogs/help_dialog.py
+-rw-r--r--   0        0        0      269 2023-04-27 14:55:30.387330 frogmouth-0.2.1/frogmouth/dialogs/information.py
+-rw-r--r--   0        0        0     4278 2023-04-27 14:46:52.803185 frogmouth-0.2.1/frogmouth/dialogs/input_dialog.py
+-rw-r--r--   0        0        0     2168 2023-04-28 17:16:37.419494 frogmouth-0.2.1/frogmouth/dialogs/text_dialog.py
+-rw-r--r--   0        0        0     4898 2023-04-27 14:46:52.803359 frogmouth-0.2.1/frogmouth/dialogs/yes_no_dialog.py
+-rw-r--r--   0        0        0       83 2023-04-27 14:46:52.803485 frogmouth-0.2.1/frogmouth/screens/__init__.py
+-rw-r--r--   0        0        0    19015 2023-04-29 14:55:46.086907 frogmouth-0.2.1/frogmouth/screens/main.py
+-rw-r--r--   0        0        0      327 2023-04-27 14:46:52.803762 frogmouth-0.2.1/frogmouth/utility/__init__.py
+-rw-r--r--   0        0        0      894 2023-04-28 13:00:47.734733 frogmouth-0.2.1/frogmouth/utility/advertising.py
+-rw-r--r--   0        0        0     4237 2023-04-27 14:46:52.803923 frogmouth-0.2.1/frogmouth/utility/forge.py
+-rw-r--r--   0        0        0     1205 2023-04-27 14:46:52.804003 frogmouth-0.2.1/frogmouth/utility/type_tests.py
+-rw-r--r--   0        0        0      184 2023-04-27 14:46:52.804110 frogmouth-0.2.1/frogmouth/widgets/__init__.py
+-rw-r--r--   0        0        0     4398 2023-04-29 14:55:46.079307 frogmouth-0.2.1/frogmouth/widgets/navigation.py
+-rw-r--r--   0        0        0      298 2023-04-27 14:46:52.804311 frogmouth-0.2.1/frogmouth/widgets/navigation_panes/__init__.py
+-rw-r--r--   0        0        0     5889 2023-04-29 14:55:46.079533 frogmouth-0.2.1/frogmouth/widgets/navigation_panes/bookmarks.py
+-rw-r--r--   0        0        0     3235 2023-04-29 14:55:46.079738 frogmouth-0.2.1/frogmouth/widgets/navigation_panes/history.py
+-rw-r--r--   0        0        0     3412 2023-04-29 14:55:46.079932 frogmouth-0.2.1/frogmouth/widgets/navigation_panes/local_files.py
+-rw-r--r--   0        0        0      667 2023-04-29 14:55:46.080110 frogmouth-0.2.1/frogmouth/widgets/navigation_panes/navigation_pane.py
+-rw-r--r--   0        0        0     1704 2023-04-29 14:55:46.080286 frogmouth-0.2.1/frogmouth/widgets/navigation_panes/table_of_contents.py
+-rw-r--r--   0        0        0    11675 2023-04-28 17:16:37.437633 frogmouth-0.2.1/frogmouth/widgets/omnibox.py
+-rw-r--r--   0        0        0     9806 2023-04-27 15:34:09.464460 frogmouth-0.2.1/frogmouth/widgets/viewer.py
+-rw-r--r--   0        0        0     1468 2023-04-29 14:58:49.538003 frogmouth-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4283 1970-01-01 00:00:00.000000 frogmouth-0.2.1/PKG-INFO
```

### Comparing `frogmouth-0.2.0/LICENSE` & `frogmouth-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/README.md` & `frogmouth-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/app/app.py` & `frogmouth-0.2.1/frogmouth/app/app.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/data/bookmarks.py` & `frogmouth-0.2.1/frogmouth/data/bookmarks.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/data/config.py` & `frogmouth-0.2.1/frogmouth/data/config.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/data/data_directory.py` & `frogmouth-0.2.1/frogmouth/data/data_directory.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/data/history.py` & `frogmouth-0.2.1/frogmouth/data/history.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/dialogs/error.py` & `frogmouth-0.2.1/frogmouth/dialogs/error.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/dialogs/help_dialog.py` & `frogmouth-0.2.1/frogmouth/dialogs/help_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/dialogs/input_dialog.py` & `frogmouth-0.2.1/frogmouth/dialogs/input_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/dialogs/text_dialog.py` & `frogmouth-0.2.1/frogmouth/dialogs/text_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/dialogs/yes_no_dialog.py` & `frogmouth-0.2.1/frogmouth/dialogs/yes_no_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/screens/main.py` & `frogmouth-0.2.1/frogmouth/screens/main.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/utility/advertising.py` & `frogmouth-0.2.1/frogmouth/utility/advertising.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/utility/forge.py` & `frogmouth-0.2.1/frogmouth/utility/forge.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/utility/type_tests.py` & `frogmouth-0.2.1/frogmouth/utility/type_tests.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/widgets/navigation.py` & `frogmouth-0.2.1/frogmouth/widgets/navigation.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/widgets/navigation_panes/bookmarks.py` & `frogmouth-0.2.1/frogmouth/widgets/navigation_panes/bookmarks.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/widgets/navigation_panes/history.py` & `frogmouth-0.2.1/frogmouth/widgets/navigation_panes/history.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/widgets/navigation_panes/local_files.py` & `frogmouth-0.2.1/frogmouth/widgets/navigation_panes/local_files.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/widgets/navigation_panes/navigation_pane.py` & `frogmouth-0.2.1/frogmouth/widgets/navigation_panes/navigation_pane.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/widgets/navigation_panes/table_of_contents.py` & `frogmouth-0.2.1/frogmouth/widgets/navigation_panes/table_of_contents.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/widgets/omnibox.py` & `frogmouth-0.2.1/frogmouth/widgets/omnibox.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/frogmouth/widgets/viewer.py` & `frogmouth-0.2.1/frogmouth/widgets/viewer.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.0/pyproject.toml` & `frogmouth-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [tool.poetry]
 name = "frogmouth"
-version = "0.2.0"
+homepage = "https://github.com/Textualize/frogmouth"
+version = "0.2.1"
 description = "A Markdown document viewer for the terminal"
 authors = ["Dave Pearson <dave@textualize.io>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "frogmouth"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `frogmouth-0.2.0/PKG-INFO` & `frogmouth-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: frogmouth
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Markdown document viewer for the terminal
+Home-page: https://github.com/Textualize/frogmouth
 License: MIT
 Author: Dave Pearson
 Author-email: dave@textualize.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: frogmouth Version: 0.2.0 Summary: A Markdown
-document viewer for the terminal License: MIT Author: Dave Pearson Author-
-email: dave@textualize.io Requires-Python: >=3.8,<4.0 Classifier: Development
-Status :: 4 - Beta Classifier: Environment :: Console Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Information Technology Classifier: Intended
-Audience :: Other Audience Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS Classifier: Operating System :: Microsoft
-:: Windows :: Windows 10 Classifier: Operating System :: Microsoft :: Windows
-:: Windows 11 Classifier: Operating System :: POSIX :: Linux Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Topic :: Software Development :: Documentation Classifier: Topic :: Text
-Processing :: Markup :: Markdown Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: textual (>=0.22.2,<0.23.0) Requires-Dist: typing-extensions
-(>=4.5.0,<5.0.0) Requires-Dist: xdg (>=6.0.0,<7.0.0) Description-Content-Type:
-text/markdown
+Metadata-Version: 2.1 Name: frogmouth Version: 0.2.1 Summary: A Markdown
+document viewer for the terminal Home-page: https://github.com/Textualize/
+frogmouth License: MIT Author: Dave Pearson Author-email: dave@textualize.io
+Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
+Audience :: Information Technology Classifier: Intended Audience :: Other
+Audience Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: MacOS Classifier: Operating System :: Microsoft :: Windows
+:: Windows 10 Classifier: Operating System :: Microsoft :: Windows :: Windows
+11 Classifier: Operating System :: POSIX :: Linux Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Software
+Development :: Documentation Classifier: Topic :: Text Processing :: Markup ::
+Markdown Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist: textual
+(>=0.22.2,<0.23.0) Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) Requires-
+Dist: xdg (>=6.0.0,<7.0.0) Description-Content-Type: text/markdown
 [https://user-images.githubusercontent.com/554369/234892488-856f9da7-7b82-4429-
                             ac35-0d0545bf0d24.png]
 [![Discord](https://img.shields.io/discord/1026214085173461072)](https://
 discord.gg/Enf6Z3qhVr) # Frogmouth Frogmouth is a terminal-based Markdown
 viewer / browser, built with [Textual](https://github.com/Textualize/textual).
 Frogmouth can view `*.md` locally or via a URL. There is a familiar browser-
 like navigation stack, history, bookmarks, and table of contents.   ð¬
```


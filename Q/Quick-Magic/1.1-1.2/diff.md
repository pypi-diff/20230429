# Comparing `tmp/quick_magic-1.1.tar.gz` & `tmp/Quick_Magic-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_magic-1.1.tar", last modified: Sat Apr 29 16:02:16 2023, max compression
+gzip compressed data, was "Quick_Magic-1.2.tar", last modified: Sat Apr 29 16:29:25 2023, max compression
```

## Comparing `quick_magic-1.1.tar` & `Quick_Magic-1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:02:16.089177 quick_magic-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-29 16:02:16.089177 quick_magic-1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:02:16.085177 quick_magic-1.1/Quick_Magic/
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-29 16:02:06.000000 quick_magic-1.1/Quick_Magic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 16:02:06.000000 quick_magic-1.1/Quick_Magic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-29 16:02:06.000000 quick_magic-1.1/Quick_Magic/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-29 16:02:06.000000 quick_magic-1.1/Quick_Magic/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-04-29 16:02:06.000000 quick_magic-1.1/Quick_Magic/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-04-29 16:02:06.000000 quick_magic-1.1/Quick_Magic/update_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-29 16:02:06.000000 quick_magic-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:02:16.089177 quick_magic-1.1/quick_magic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-29 16:02:16.000000 quick_magic-1.1/quick_magic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-29 16:02:16.000000 quick_magic-1.1/quick_magic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:02:16.000000 quick_magic-1.1/quick_magic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 16:02:16.000000 quick_magic-1.1/quick_magic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 16:02:16.000000 quick_magic-1.1/quick_magic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 16:02:16.089177 quick_magic-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-29 16:02:06.000000 quick_magic-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:29:25.672764 Quick_Magic-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-29 16:29:25.672764 Quick_Magic-1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:29:25.668764 Quick_Magic-1.2/Quick_Magic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-29 16:29:15.000000 Quick_Magic-1.2/Quick_Magic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 16:29:15.000000 Quick_Magic-1.2/Quick_Magic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-29 16:29:15.000000 Quick_Magic-1.2/Quick_Magic/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-29 16:29:15.000000 Quick_Magic-1.2/Quick_Magic/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-04-29 16:29:15.000000 Quick_Magic-1.2/Quick_Magic/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-04-29 16:29:15.000000 Quick_Magic-1.2/Quick_Magic/update_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:29:25.672764 Quick_Magic-1.2/Quick_Magic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-29 16:29:25.000000 Quick_Magic-1.2/Quick_Magic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-29 16:29:25.000000 Quick_Magic-1.2/Quick_Magic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:29:25.000000 Quick_Magic-1.2/Quick_Magic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 16:29:25.000000 Quick_Magic-1.2/Quick_Magic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 16:29:25.000000 Quick_Magic-1.2/Quick_Magic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-29 16:29:15.000000 Quick_Magic-1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 16:29:25.672764 Quick_Magic-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-29 16:29:15.000000 Quick_Magic-1.2/setup.py
```

### Comparing `quick_magic-1.1/PKG-INFO` & `Quick_Magic-1.2/Quick_Magic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
-Name: quick_magic
-Version: 1.1
+Name: Quick-Magic
+Version: 1.2
 Summary: Open/Close any application by it's name.
 Home-page: https://github.com/athrvvvv/AppOpener/tree/module
 Download-URL: https://pypi.python.org/pypi/AppOpener
 Author: Athrv Chaulkar
 Author-email: athrvchaulkar@gmail.com
 Maintainer: athrvvvv
 Maintainer-email: athrvchaulkar@gmail.com
 License: MIT
 Project-URL: Documentation, https://appopener.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/athrvvvv/AppOpener/tree/module
 Project-URL: Tracker, https://github.com/athrvvvv/AppOpener/issues
-Keywords: test
+Keywords: test,hello
 Platform: Windows 10
 Platform: Windows 8.1
 Platform: Windows 11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `quick_magic-1.1/Quick_Magic/__init__.py` & `Quick_Magic-1.2/Quick_Magic/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_magic-1.1/Quick_Magic/check.py` & `Quick_Magic-1.2/Quick_Magic/check.py`

 * *Files identical despite different names*

### Comparing `quick_magic-1.1/Quick_Magic/commands.py` & `Quick_Magic-1.2/Quick_Magic/commands.py`

 * *Files identical despite different names*

### Comparing `quick_magic-1.1/Quick_Magic/features.py` & `Quick_Magic-1.2/Quick_Magic/features.py`

 * *Files identical despite different names*

### Comparing `quick_magic-1.1/Quick_Magic/update_list.py` & `Quick_Magic-1.2/Quick_Magic/update_list.py`

 * *Files identical despite different names*

### Comparing `quick_magic-1.1/README.md` & `Quick_Magic-1.2/README.md`

 * *Files identical despite different names*

### Comparing `quick_magic-1.1/quick_magic.egg-info/PKG-INFO` & `Quick_Magic-1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
-Name: quick-magic
-Version: 1.1
+Name: Quick_Magic
+Version: 1.2
 Summary: Open/Close any application by it's name.
 Home-page: https://github.com/athrvvvv/AppOpener/tree/module
 Download-URL: https://pypi.python.org/pypi/AppOpener
 Author: Athrv Chaulkar
 Author-email: athrvchaulkar@gmail.com
 Maintainer: athrvvvv
 Maintainer-email: athrvchaulkar@gmail.com
 License: MIT
 Project-URL: Documentation, https://appopener.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/athrvvvv/AppOpener/tree/module
 Project-URL: Tracker, https://github.com/athrvvvv/AppOpener/issues
-Keywords: test
+Keywords: test,hello
 Platform: Windows 10
 Platform: Windows 8.1
 Platform: Windows 11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `quick_magic-1.1/setup.py` & `Quick_Magic-1.2/setup.py`

 * *Files identical despite different names*


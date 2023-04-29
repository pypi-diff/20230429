# Comparing `tmp/textual-astview-0.6.0.tar.gz` & `tmp/textual-astview-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual-astview-0.6.0.tar", last modified: Sat Apr 29 07:26:29 2023, max compression
+gzip compressed data, was "textual-astview-0.6.1.tar", last modified: Sat Apr 29 07:35:35 2023, max compression
```

## Comparing `textual-astview-0.6.0.tar` & `textual-astview-0.6.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:26:29.376639 textual-astview-0.6.0/
--rw-r--r--   0 davep      (501) staff       (20)     1087 2023-04-27 21:09:18.000000 textual-astview-0.6.0/LICENCE
--rw-r--r--   0 davep      (501) staff       (20)     6207 2023-04-29 07:26:29.376694 textual-astview-0.6.0/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)     4828 2023-04-27 21:09:18.000000 textual-astview-0.6.0/README.md
--rw-r--r--   0 davep      (501) staff       (20)      124 2023-04-27 21:09:18.000000 textual-astview-0.6.0/pyproject.toml
--rw-r--r--   0 davep      (501) staff       (20)     1580 2023-04-29 07:26:29.376941 textual-astview-0.6.0/setup.cfg
--rw-r--r--   0 davep      (501) staff       (20)      345 2023-04-27 21:09:18.000000 textual-astview-0.6.0/setup.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:26:29.374525 textual-astview-0.6.0/textual_astview/
--rw-r--r--   0 davep      (501) staff       (20)      934 2023-04-29 07:25:54.000000 textual-astview-0.6.0/textual_astview/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)      352 2023-04-27 21:09:18.000000 textual-astview-0.6.0/textual_astview/__main__.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:26:29.375592 textual-astview-0.6.0/textual_astview/app/
--rw-r--r--   0 davep      (501) staff       (20)       88 2023-04-27 21:09:18.000000 textual-astview-0.6.0/textual_astview/app/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     3676 2023-04-27 21:09:18.000000 textual-astview-0.6.0/textual_astview/app/astare.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:26:29.375815 textual-astview-0.6.0/textual_astview/app/screens/
--rw-r--r--   0 davep      (501) staff       (20)      342 2023-04-27 21:09:18.000000 textual-astview-0.6.0/textual_astview/app/screens/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)    10000 2023-04-29 07:25:54.000000 textual-astview-0.6.0/textual_astview/app/screens/main.py
--rw-r--r--   0 davep      (501) staff       (20)        0 2023-04-27 21:09:18.000000 textual-astview-0.6.0/textual_astview/py.typed
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:26:29.376527 textual-astview-0.6.0/textual_astview/widgets/
--rw-r--r--   0 davep      (501) staff       (20)       72 2023-04-27 21:09:18.000000 textual-astview-0.6.0/textual_astview/widgets/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     7226 2023-04-27 21:09:18.000000 textual-astview-0.6.0/textual_astview/widgets/astview.py
--rw-r--r--   0 davep      (501) staff       (20)     1770 2023-04-27 21:09:18.000000 textual-astview-0.6.0/textual_astview/widgets/node_info.py
--rw-r--r--   0 davep      (501) staff       (20)     7847 2023-04-27 21:09:18.000000 textual-astview-0.6.0/textual_astview/widgets/source.py
--rw-r--r--   0 davep      (501) staff       (20)     3790 2023-04-28 08:00:33.000000 textual-astview-0.6.0/textual_astview/widgets/source_info.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:26:29.375381 textual-astview-0.6.0/textual_astview.egg-info/
--rw-r--r--   0 davep      (501) staff       (20)     6207 2023-04-29 07:26:29.000000 textual-astview-0.6.0/textual_astview.egg-info/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)      687 2023-04-29 07:26:29.000000 textual-astview-0.6.0/textual_astview.egg-info/SOURCES.txt
--rw-r--r--   0 davep      (501) staff       (20)        1 2023-04-29 07:26:29.000000 textual-astview-0.6.0/textual_astview.egg-info/dependency_links.txt
--rw-r--r--   0 davep      (501) staff       (20)       59 2023-04-29 07:26:29.000000 textual-astview-0.6.0/textual_astview.egg-info/entry_points.txt
--rw-r--r--   0 davep      (501) staff       (20)       16 2023-04-29 07:26:29.000000 textual-astview-0.6.0/textual_astview.egg-info/requires.txt
--rw-r--r--   0 davep      (501) staff       (20)       16 2023-04-29 07:26:29.000000 textual-astview-0.6.0/textual_astview.egg-info/top_level.txt
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:35:35.347220 textual-astview-0.6.1/
+-rw-r--r--   0 davep      (501) staff       (20)     1087 2023-04-27 21:09:18.000000 textual-astview-0.6.1/LICENCE
+-rw-r--r--   0 davep      (501) staff       (20)     6207 2023-04-29 07:35:35.347269 textual-astview-0.6.1/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)     4828 2023-04-27 21:09:18.000000 textual-astview-0.6.1/README.md
+-rw-r--r--   0 davep      (501) staff       (20)      124 2023-04-27 21:09:18.000000 textual-astview-0.6.1/pyproject.toml
+-rw-r--r--   0 davep      (501) staff       (20)     1580 2023-04-29 07:35:35.347486 textual-astview-0.6.1/setup.cfg
+-rw-r--r--   0 davep      (501) staff       (20)      345 2023-04-27 21:09:18.000000 textual-astview-0.6.1/setup.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:35:35.345494 textual-astview-0.6.1/textual_astview/
+-rw-r--r--   0 davep      (501) staff       (20)      934 2023-04-29 07:35:10.000000 textual-astview-0.6.1/textual_astview/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)      352 2023-04-27 21:09:18.000000 textual-astview-0.6.1/textual_astview/__main__.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:35:35.346379 textual-astview-0.6.1/textual_astview/app/
+-rw-r--r--   0 davep      (501) staff       (20)       88 2023-04-27 21:09:18.000000 textual-astview-0.6.1/textual_astview/app/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     3676 2023-04-27 21:09:18.000000 textual-astview-0.6.1/textual_astview/app/astare.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:35:35.346607 textual-astview-0.6.1/textual_astview/app/screens/
+-rw-r--r--   0 davep      (501) staff       (20)      342 2023-04-27 21:09:18.000000 textual-astview-0.6.1/textual_astview/app/screens/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)    10012 2023-04-29 07:35:10.000000 textual-astview-0.6.1/textual_astview/app/screens/main.py
+-rw-r--r--   0 davep      (501) staff       (20)        0 2023-04-27 21:09:18.000000 textual-astview-0.6.1/textual_astview/py.typed
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:35:35.347116 textual-astview-0.6.1/textual_astview/widgets/
+-rw-r--r--   0 davep      (501) staff       (20)       72 2023-04-27 21:09:18.000000 textual-astview-0.6.1/textual_astview/widgets/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     7226 2023-04-27 21:09:18.000000 textual-astview-0.6.1/textual_astview/widgets/astview.py
+-rw-r--r--   0 davep      (501) staff       (20)     1770 2023-04-27 21:09:18.000000 textual-astview-0.6.1/textual_astview/widgets/node_info.py
+-rw-r--r--   0 davep      (501) staff       (20)     7847 2023-04-27 21:09:18.000000 textual-astview-0.6.1/textual_astview/widgets/source.py
+-rw-r--r--   0 davep      (501) staff       (20)     3790 2023-04-28 08:00:33.000000 textual-astview-0.6.1/textual_astview/widgets/source_info.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:35:35.346143 textual-astview-0.6.1/textual_astview.egg-info/
+-rw-r--r--   0 davep      (501) staff       (20)     6207 2023-04-29 07:35:35.000000 textual-astview-0.6.1/textual_astview.egg-info/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)      687 2023-04-29 07:35:35.000000 textual-astview-0.6.1/textual_astview.egg-info/SOURCES.txt
+-rw-r--r--   0 davep      (501) staff       (20)        1 2023-04-29 07:35:35.000000 textual-astview-0.6.1/textual_astview.egg-info/dependency_links.txt
+-rw-r--r--   0 davep      (501) staff       (20)       59 2023-04-29 07:35:35.000000 textual-astview-0.6.1/textual_astview.egg-info/entry_points.txt
+-rw-r--r--   0 davep      (501) staff       (20)       16 2023-04-29 07:35:35.000000 textual-astview-0.6.1/textual_astview.egg-info/requires.txt
+-rw-r--r--   0 davep      (501) staff       (20)       16 2023-04-29 07:35:35.000000 textual-astview-0.6.1/textual_astview.egg-info/top_level.txt
```

### Comparing `textual-astview-0.6.0/LICENCE` & `textual-astview-0.6.1/LICENCE`

 * *Files identical despite different names*

### Comparing `textual-astview-0.6.0/PKG-INFO` & `textual-astview-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-astview
-Version: 0.6.0
+Version: 0.6.1
 Summary: An AST viewing widget library plus app, built for and with Textual.
 Home-page: https://github.com/davep/textual-astview
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: MIT License
```

### Comparing `textual-astview-0.6.0/README.md` & `textual-astview-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `textual-astview-0.6.0/setup.cfg` & `textual-astview-0.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `textual-astview-0.6.0/textual_astview/__init__.py` & `textual-astview-0.6.1/textual_astview/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ######################################################################
 # Main app information.
 __author__     = "Dave Pearson"
 __copyright__  = "Copyright 2022-2023, Dave Pearson"
 __credits__    = [ "Dave Pearson" ]
 __maintainer__ = "Dave Pearson"
 __email__      = "davep@davep.org"
-__version__    = "0.6.0"
+__version__    = "0.6.1"
 __licence__    = "MIT"
 
 ##############################################################################
 # Import the widgets to make them easier to get at.
 from .widgets.astview     import ASTView, ASTNode
 from .widgets.node_info   import NodeInfo
 from .widgets.source_info import SourceInfo
```

### Comparing `textual-astview-0.6.0/textual_astview/app/astare.py` & `textual-astview-0.6.1/textual_astview/app/astare.py`

 * *Files identical despite different names*

### Comparing `textual-astview-0.6.0/textual_astview/app/screens/main.py` & `textual-astview-0.6.1/textual_astview/app/screens/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     UPDATE_DELAY: Final = 0.2
     """How long to leave it before updating the highlight in the source."""
 
     rainbow = reactive( False, init=False )
     """Should 'rainbow' highlighting be used for the source?"""
 
-    ast_width: reactive[ int ] = reactive( 10 )
+    ast_width: reactive[ int ] = reactive( 10, init=False )
     """The relative width of the reactive pane."""
 
     def __init__( self, cli_args: Namespace, *args: Any, **kwargs: Any ) -> None:
         """Initialise the main screen.
 
         Args:
             cli_args: The command line arguments.
```

### Comparing `textual-astview-0.6.0/textual_astview/widgets/astview.py` & `textual-astview-0.6.1/textual_astview/widgets/astview.py`

 * *Files identical despite different names*

### Comparing `textual-astview-0.6.0/textual_astview/widgets/node_info.py` & `textual-astview-0.6.1/textual_astview/widgets/node_info.py`

 * *Files identical despite different names*

### Comparing `textual-astview-0.6.0/textual_astview/widgets/source.py` & `textual-astview-0.6.1/textual_astview/widgets/source.py`

 * *Files identical despite different names*

### Comparing `textual-astview-0.6.0/textual_astview/widgets/source_info.py` & `textual-astview-0.6.1/textual_astview/widgets/source_info.py`

 * *Files identical despite different names*

### Comparing `textual-astview-0.6.0/textual_astview.egg-info/PKG-INFO` & `textual-astview-0.6.1/textual_astview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-astview
-Version: 0.6.0
+Version: 0.6.1
 Summary: An AST viewing widget library plus app, built for and with Textual.
 Home-page: https://github.com/davep/textual-astview
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: MIT License
```

### Comparing `textual-astview-0.6.0/textual_astview.egg-info/SOURCES.txt` & `textual-astview-0.6.1/textual_astview.egg-info/SOURCES.txt`

 * *Files identical despite different names*


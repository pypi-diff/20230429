# Comparing `tmp/textual-astview-0.5.0.tar.gz` & `tmp/textual-astview-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual-astview-0.5.0.tar", last modified: Thu Feb 16 20:37:16 2023, max compression
+gzip compressed data, was "textual-astview-0.6.0.tar", last modified: Sat Apr 29 07:26:29 2023, max compression
```

## Comparing `textual-astview-0.5.0.tar` & `textual-astview-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-02-16 20:37:16.183037 textual-astview-0.5.0/
--rw-r--r--   0 davep      (501) staff       (20)     1087 2022-12-19 22:41:07.000000 textual-astview-0.5.0/LICENCE
--rw-r--r--   0 davep      (501) staff       (20)     6207 2023-02-16 20:37:16.183229 textual-astview-0.5.0/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)     4828 2023-02-16 20:36:17.000000 textual-astview-0.5.0/README.md
--rw-r--r--   0 davep      (501) staff       (20)      124 2022-12-25 16:09:27.000000 textual-astview-0.5.0/pyproject.toml
--rw-r--r--   0 davep      (501) staff       (20)     1580 2023-02-16 20:37:16.184312 textual-astview-0.5.0/setup.cfg
--rw-r--r--   0 davep      (501) staff       (20)      345 2022-12-25 16:09:27.000000 textual-astview-0.5.0/setup.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-02-16 20:37:16.145589 textual-astview-0.5.0/textual_astview/
--rw-r--r--   0 davep      (501) staff       (20)      934 2023-02-16 20:36:17.000000 textual-astview-0.5.0/textual_astview/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)      352 2022-12-19 22:02:52.000000 textual-astview-0.5.0/textual_astview/__main__.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-02-16 20:37:16.177903 textual-astview-0.5.0/textual_astview/app/
--rw-r--r--   0 davep      (501) staff       (20)       88 2022-12-19 21:50:19.000000 textual-astview-0.5.0/textual_astview/app/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     3676 2023-02-16 20:36:17.000000 textual-astview-0.5.0/textual_astview/app/astare.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-02-16 20:37:16.179235 textual-astview-0.5.0/textual_astview/app/screens/
--rw-r--r--   0 davep      (501) staff       (20)      342 2022-12-25 16:09:27.000000 textual-astview-0.5.0/textual_astview/app/screens/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     9638 2023-02-16 20:36:17.000000 textual-astview-0.5.0/textual_astview/app/screens/main.py
--rw-r--r--   0 davep      (501) staff       (20)        0 2022-12-20 18:00:37.000000 textual-astview-0.5.0/textual_astview/py.typed
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-02-16 20:37:16.182518 textual-astview-0.5.0/textual_astview/widgets/
--rw-r--r--   0 davep      (501) staff       (20)       72 2022-12-19 21:24:23.000000 textual-astview-0.5.0/textual_astview/widgets/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     7226 2023-02-16 20:36:17.000000 textual-astview-0.5.0/textual_astview/widgets/astview.py
--rw-r--r--   0 davep      (501) staff       (20)     1770 2023-02-16 20:36:17.000000 textual-astview-0.5.0/textual_astview/widgets/node_info.py
--rw-r--r--   0 davep      (501) staff       (20)     7847 2023-02-16 20:36:17.000000 textual-astview-0.5.0/textual_astview/widgets/source.py
--rw-r--r--   0 davep      (501) staff       (20)     3790 2023-02-16 20:36:17.000000 textual-astview-0.5.0/textual_astview/widgets/source_info.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-02-16 20:37:16.176554 textual-astview-0.5.0/textual_astview.egg-info/
--rw-r--r--   0 davep      (501) staff       (20)     6207 2023-02-16 20:37:16.000000 textual-astview-0.5.0/textual_astview.egg-info/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)      687 2023-02-16 20:37:16.000000 textual-astview-0.5.0/textual_astview.egg-info/SOURCES.txt
--rw-r--r--   0 davep      (501) staff       (20)        1 2023-02-16 20:37:16.000000 textual-astview-0.5.0/textual_astview.egg-info/dependency_links.txt
--rw-r--r--   0 davep      (501) staff       (20)       59 2023-02-16 20:37:16.000000 textual-astview-0.5.0/textual_astview.egg-info/entry_points.txt
--rw-r--r--   0 davep      (501) staff       (20)       16 2023-02-16 20:37:16.000000 textual-astview-0.5.0/textual_astview.egg-info/requires.txt
--rw-r--r--   0 davep      (501) staff       (20)       16 2023-02-16 20:37:16.000000 textual-astview-0.5.0/textual_astview.egg-info/top_level.txt
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:26:29.376639 textual-astview-0.6.0/
+-rw-r--r--   0 davep      (501) staff       (20)     1087 2023-04-27 21:09:18.000000 textual-astview-0.6.0/LICENCE
+-rw-r--r--   0 davep      (501) staff       (20)     6207 2023-04-29 07:26:29.376694 textual-astview-0.6.0/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)     4828 2023-04-27 21:09:18.000000 textual-astview-0.6.0/README.md
+-rw-r--r--   0 davep      (501) staff       (20)      124 2023-04-27 21:09:18.000000 textual-astview-0.6.0/pyproject.toml
+-rw-r--r--   0 davep      (501) staff       (20)     1580 2023-04-29 07:26:29.376941 textual-astview-0.6.0/setup.cfg
+-rw-r--r--   0 davep      (501) staff       (20)      345 2023-04-27 21:09:18.000000 textual-astview-0.6.0/setup.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:26:29.374525 textual-astview-0.6.0/textual_astview/
+-rw-r--r--   0 davep      (501) staff       (20)      934 2023-04-29 07:25:54.000000 textual-astview-0.6.0/textual_astview/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)      352 2023-04-27 21:09:18.000000 textual-astview-0.6.0/textual_astview/__main__.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:26:29.375592 textual-astview-0.6.0/textual_astview/app/
+-rw-r--r--   0 davep      (501) staff       (20)       88 2023-04-27 21:09:18.000000 textual-astview-0.6.0/textual_astview/app/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     3676 2023-04-27 21:09:18.000000 textual-astview-0.6.0/textual_astview/app/astare.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:26:29.375815 textual-astview-0.6.0/textual_astview/app/screens/
+-rw-r--r--   0 davep      (501) staff       (20)      342 2023-04-27 21:09:18.000000 textual-astview-0.6.0/textual_astview/app/screens/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)    10000 2023-04-29 07:25:54.000000 textual-astview-0.6.0/textual_astview/app/screens/main.py
+-rw-r--r--   0 davep      (501) staff       (20)        0 2023-04-27 21:09:18.000000 textual-astview-0.6.0/textual_astview/py.typed
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:26:29.376527 textual-astview-0.6.0/textual_astview/widgets/
+-rw-r--r--   0 davep      (501) staff       (20)       72 2023-04-27 21:09:18.000000 textual-astview-0.6.0/textual_astview/widgets/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     7226 2023-04-27 21:09:18.000000 textual-astview-0.6.0/textual_astview/widgets/astview.py
+-rw-r--r--   0 davep      (501) staff       (20)     1770 2023-04-27 21:09:18.000000 textual-astview-0.6.0/textual_astview/widgets/node_info.py
+-rw-r--r--   0 davep      (501) staff       (20)     7847 2023-04-27 21:09:18.000000 textual-astview-0.6.0/textual_astview/widgets/source.py
+-rw-r--r--   0 davep      (501) staff       (20)     3790 2023-04-28 08:00:33.000000 textual-astview-0.6.0/textual_astview/widgets/source_info.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:26:29.375381 textual-astview-0.6.0/textual_astview.egg-info/
+-rw-r--r--   0 davep      (501) staff       (20)     6207 2023-04-29 07:26:29.000000 textual-astview-0.6.0/textual_astview.egg-info/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)      687 2023-04-29 07:26:29.000000 textual-astview-0.6.0/textual_astview.egg-info/SOURCES.txt
+-rw-r--r--   0 davep      (501) staff       (20)        1 2023-04-29 07:26:29.000000 textual-astview-0.6.0/textual_astview.egg-info/dependency_links.txt
+-rw-r--r--   0 davep      (501) staff       (20)       59 2023-04-29 07:26:29.000000 textual-astview-0.6.0/textual_astview.egg-info/entry_points.txt
+-rw-r--r--   0 davep      (501) staff       (20)       16 2023-04-29 07:26:29.000000 textual-astview-0.6.0/textual_astview.egg-info/requires.txt
+-rw-r--r--   0 davep      (501) staff       (20)       16 2023-04-29 07:26:29.000000 textual-astview-0.6.0/textual_astview.egg-info/top_level.txt
```

### Comparing `textual-astview-0.5.0/LICENCE` & `textual-astview-0.6.0/LICENCE`

 * *Files identical despite different names*

### Comparing `textual-astview-0.5.0/PKG-INFO` & `textual-astview-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-astview
-Version: 0.5.0
+Version: 0.6.0
 Summary: An AST viewing widget library plus app, built for and with Textual.
 Home-page: https://github.com/davep/textual-astview
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: MIT License
```

### Comparing `textual-astview-0.5.0/README.md` & `textual-astview-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `textual-astview-0.5.0/setup.cfg` & `textual-astview-0.6.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 	Issues = https://github.com/davep/textual-astview/issues
 	Discussions = https://github.com/davep/textual-astview/discussions
 
 [options]
 packages = find:
 platforms = any
 include_package_data = True
-install_requires = textual==0.11.0
+install_requires = textual==0.22.3
 python_requires = >=3.8
 
 [options.package_data]
 textual_astview = py.typed
 
 [options.entry_points]
 console_scripts =
```

### Comparing `textual-astview-0.5.0/textual_astview/__init__.py` & `textual-astview-0.6.0/textual_astview/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ######################################################################
 # Main app information.
 __author__     = "Dave Pearson"
 __copyright__  = "Copyright 2022-2023, Dave Pearson"
 __credits__    = [ "Dave Pearson" ]
 __maintainer__ = "Dave Pearson"
 __email__      = "davep@davep.org"
-__version__    = "0.5.0"
+__version__    = "0.6.0"
 __licence__    = "MIT"
 
 ##############################################################################
 # Import the widgets to make them easier to get at.
 from .widgets.astview     import ASTView, ASTNode
 from .widgets.node_info   import NodeInfo
 from .widgets.source_info import SourceInfo
```

### Comparing `textual-astview-0.5.0/textual_astview/app/astare.py` & `textual-astview-0.6.0/textual_astview/app/astare.py`

 * *Files identical despite different names*

### Comparing `textual-astview-0.5.0/textual_astview/app/screens/main.py` & `textual-astview-0.6.0/textual_astview/app/screens/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
     def ast_pane( self ) -> ASTView:
         """Make an ASTView pane.
 
         Returns:
             An ASTView pane for viewing the AST.
         """
-        return ASTView( self._args.file )
+        return ASTView( self._args.file, id="ast-view" )
 
     def source_pane( self ) -> Source:
         """Make a Source pane.
 
         Returns:
             A source pane for viewing the code.
         """
@@ -156,46 +156,54 @@
 
         Args:
             node: The node to highlight.
         """
         self.query_one( NodeInfo ).show( node )
         self.query_one( Source ).highlight( node, self.rainbow )
 
-    async def on_tree_node_highlighted( self, event: Tree.NodeHighlighted ) -> None:
+    def on_tree_node_highlighted( self, event: Tree.NodeHighlighted ) -> None:
         """React to a node in the tree being highlighted.
 
         Args:
             event: The event to react to.
         """
-        if isinstance( event.sender, ASTView ):
-            # If there's a refresh pending...
-            if self._refresh is not None:
-                # ...stop it.
-                await self._refresh.stop()
-            # Book in a fresh refresh the full delay on from this event.
-            self._refresh = self.set_timer(
-                self.UPDATE_DELAY, partial( self.highlight_node, event.node )
-            )
+        # Only handle highlight for the AST tree view. Note that for the
+        # moment I have to dive into the private attributes of the node to
+        # figure out which tree is sending the message.
+        if event.node.tree.id != "ast-view":
+            return
+        # If there's a refresh pending...
+        if self._refresh is not None:
+            # ...stop it.
+            self._refresh.stop()
+        # Book in a fresh refresh the full delay on from this event.
+        self._refresh = self.set_timer(
+            self.UPDATE_DELAY, partial( self.highlight_node, event.node )
+        )
 
-    async def on_tree_node_selected( self, event: Tree.NodeSelected ) -> None:
+    def on_tree_node_selected( self, event: Tree.NodeSelected ) -> None:
         """React to a node in the tree being selected.
 
         Args:
             event: The event to react to.
         """
-        if isinstance( event.sender, ASTView ):
-            # If there's a refresh pending...
-            if self._refresh is not None:
-                # ...stop it and nuke all evidence of it.
-                await self._refresh.stop()
-                self._refresh = None
-            # Selected is a mouse click or someone bouncing on the enter key,
-            # there's no point in delaying; so let's make it look a bit more
-            # snappy by updating right away.
-            self.highlight_node( event.node )
+        # Only handle selected for the AST tree view. Note that for the
+        # moment I have to dive into the private attributes of the node to
+        # figure out which tree is sending the message.
+        if event.node.tree.id != "ast-view":
+            return
+        # If there's a refresh pending...
+        if self._refresh is not None:
+            # ...stop it and nuke all evidence of it.
+            self._refresh.stop()
+            self._refresh = None
+        # Selected is a mouse click or someone bouncing on the enter key,
+        # there's no point in delaying; so let's make it look a bit more
+        # snappy by updating right away.
+        self.highlight_node( event.node )
 
     def watch_rainbow( self, new_value: bool ) -> None:
         """React to the rainbow flag being changed.
 
         Args:
             new_value: The new value for the flag.
         """
```

### Comparing `textual-astview-0.5.0/textual_astview/widgets/astview.py` & `textual-astview-0.6.0/textual_astview/widgets/astview.py`

 * *Files identical despite different names*

### Comparing `textual-astview-0.5.0/textual_astview/widgets/node_info.py` & `textual-astview-0.6.0/textual_astview/widgets/node_info.py`

 * *Files identical despite different names*

### Comparing `textual-astview-0.5.0/textual_astview/widgets/source.py` & `textual-astview-0.6.0/textual_astview/widgets/source.py`

 * *Files identical despite different names*

### Comparing `textual-astview-0.5.0/textual_astview/widgets/source_info.py` & `textual-astview-0.6.0/textual_astview/widgets/source_info.py`

 * *Files identical despite different names*

### Comparing `textual-astview-0.5.0/textual_astview.egg-info/PKG-INFO` & `textual-astview-0.6.0/textual_astview.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-astview
-Version: 0.5.0
+Version: 0.6.0
 Summary: An AST viewing widget library plus app, built for and with Textual.
 Home-page: https://github.com/davep/textual-astview
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: MIT License
```

### Comparing `textual-astview-0.5.0/textual_astview.egg-info/SOURCES.txt` & `textual-astview-0.6.0/textual_astview.egg-info/SOURCES.txt`

 * *Files identical despite different names*


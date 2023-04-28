# Comparing `tmp/pyrefact-8.tar.gz` & `tmp/pyrefact-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrefact-8.tar", last modified: Wed Nov  2 19:03:01 2022, max compression
+gzip compressed data, was "pyrefact-9.tar", last modified: Wed Nov  2 20:30:27 2022, max compression
```

## Comparing `pyrefact-8.tar` & `pyrefact-9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 olle       (501) staff       (20)        0 2022-11-02 19:03:01.845573 pyrefact-8/
--rw-r--r--   0 olle       (501) staff       (20)     1069 2022-10-20 08:55:02.000000 pyrefact-8/LICENSE
--rw-r--r--   0 olle       (501) staff       (20)      228 2022-11-02 19:03:01.845421 pyrefact-8/PKG-INFO
--rw-r--r--   0 olle       (501) staff       (20)     1262 2022-11-02 18:36:20.000000 pyrefact-8/README.md
-drwxr-xr-x   0 olle       (501) staff       (20)        0 2022-11-02 19:03:01.844583 pyrefact-8/pyrefact/
--rw-r--r--   0 olle       (501) staff       (20)        0 2022-10-23 21:51:04.000000 pyrefact-8/pyrefact/__init__.py
--rwxr-xr-x   0 olle       (501) staff       (20)      120 2022-10-20 18:11:25.000000 pyrefact-8/pyrefact/__main__.py
--rw-r--r--   0 olle       (501) staff       (20)     2148 2022-11-02 12:50:20.000000 pyrefact-8/pyrefact/completion.py
--rw-r--r--   0 olle       (501) staff       (20)     1065 2022-10-30 20:04:01.000000 pyrefact-8/pyrefact/constants.py
--rw-r--r--   0 olle       (501) staff       (20)    28213 2022-11-02 19:00:06.000000 pyrefact-8/pyrefact/fixes.py
--rwxr-xr-x   0 olle       (501) staff       (20)     3867 2022-11-02 12:50:20.000000 pyrefact-8/pyrefact/main.py
--rw-r--r--   0 olle       (501) staff       (20)    12892 2022-11-02 18:18:48.000000 pyrefact-8/pyrefact/parsing.py
-drwxr-xr-x   0 olle       (501) staff       (20)        0 2022-11-02 19:03:01.845229 pyrefact-8/pyrefact.egg-info/
--rw-r--r--   0 olle       (501) staff       (20)      228 2022-11-02 19:03:01.000000 pyrefact-8/pyrefact.egg-info/PKG-INFO
--rw-r--r--   0 olle       (501) staff       (20)      327 2022-11-02 19:03:01.000000 pyrefact-8/pyrefact.egg-info/SOURCES.txt
--rw-r--r--   0 olle       (501) staff       (20)        1 2022-11-02 19:03:01.000000 pyrefact-8/pyrefact.egg-info/dependency_links.txt
--rw-r--r--   0 olle       (501) staff       (20)       40 2022-11-02 19:03:01.000000 pyrefact-8/pyrefact.egg-info/requires.txt
--rw-r--r--   0 olle       (501) staff       (20)        9 2022-11-02 19:03:01.000000 pyrefact-8/pyrefact.egg-info/top_level.txt
--rw-r--r--   0 olle       (501) staff       (20)       38 2022-11-02 19:03:01.845631 pyrefact-8/setup.cfg
--rw-r--r--   0 olle       (501) staff       (20)      468 2022-11-02 19:02:40.000000 pyrefact-8/setup.py
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2022-11-02 20:30:27.405663 pyrefact-9/
+-rw-r--r--   0 olle       (501) staff       (20)     1069 2022-10-20 08:55:02.000000 pyrefact-9/LICENSE
+-rw-r--r--   0 olle       (501) staff       (20)      228 2022-11-02 20:30:27.405542 pyrefact-9/PKG-INFO
+-rw-r--r--   0 olle       (501) staff       (20)     1262 2022-11-02 18:36:20.000000 pyrefact-9/README.md
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2022-11-02 20:30:27.404795 pyrefact-9/pyrefact/
+-rw-r--r--   0 olle       (501) staff       (20)        0 2022-10-23 21:51:04.000000 pyrefact-9/pyrefact/__init__.py
+-rwxr-xr-x   0 olle       (501) staff       (20)      120 2022-10-20 18:11:25.000000 pyrefact-9/pyrefact/__main__.py
+-rw-r--r--   0 olle       (501) staff       (20)     2148 2022-11-02 19:54:47.000000 pyrefact-9/pyrefact/completion.py
+-rw-r--r--   0 olle       (501) staff       (20)     1065 2022-10-30 20:04:01.000000 pyrefact-9/pyrefact/constants.py
+-rw-r--r--   0 olle       (501) staff       (20)    31081 2022-11-02 20:24:19.000000 pyrefact-9/pyrefact/fixes.py
+-rwxr-xr-x   0 olle       (501) staff       (20)     3867 2022-11-02 12:50:20.000000 pyrefact-9/pyrefact/main.py
+-rw-r--r--   0 olle       (501) staff       (20)    12892 2022-11-02 19:54:47.000000 pyrefact-9/pyrefact/parsing.py
+drwxr-xr-x   0 olle       (501) staff       (20)        0 2022-11-02 20:30:27.405383 pyrefact-9/pyrefact.egg-info/
+-rw-r--r--   0 olle       (501) staff       (20)      228 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/PKG-INFO
+-rw-r--r--   0 olle       (501) staff       (20)      327 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/SOURCES.txt
+-rw-r--r--   0 olle       (501) staff       (20)        1 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/dependency_links.txt
+-rw-r--r--   0 olle       (501) staff       (20)       40 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/requires.txt
+-rw-r--r--   0 olle       (501) staff       (20)        9 2022-11-02 20:30:27.000000 pyrefact-9/pyrefact.egg-info/top_level.txt
+-rw-r--r--   0 olle       (501) staff       (20)       38 2022-11-02 20:30:27.405698 pyrefact-9/setup.cfg
+-rw-r--r--   0 olle       (501) staff       (20)      468 2022-11-02 20:30:04.000000 pyrefact-9/setup.py
```

### Comparing `pyrefact-8/LICENSE` & `pyrefact-9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrefact-8/README.md` & `pyrefact-9/README.md`

 * *Files identical despite different names*

### Comparing `pyrefact-8/pyrefact/completion.py` & `pyrefact-9/pyrefact/completion.py`

 * *Files identical despite different names*

### Comparing `pyrefact-8/pyrefact/constants.py` & `pyrefact-9/pyrefact/constants.py`

 * *Files identical despite different names*

### Comparing `pyrefact-8/pyrefact/fixes.py` & `pyrefact-9/pyrefact/fixes.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,14 +178,16 @@
                 classdefs.append(node)
                 substitute = _rename_class(name, private=_is_private(name))
                 renamings[node].add(substitute)
                 for refnode in _get_uses_of(node, partial_tree, content):
                     renamings[refnode].add(substitute)
             for node in parsing.iter_funcdefs(partial_tree):
                 name = node.name
+                if name.startswith("__") and name.endswith("__"):
+                    continue
                 funcdefs.append(node)
                 substitute = _rename_variable(name, private=_is_private(name), static=False)
                 renamings[node].add(substitute)
                 for refnode in _get_uses_of(node, partial_tree, content):
                     renamings[refnode].add(substitute)
             for node in parsing.iter_assignments(partial_tree):
                 name = node.id
@@ -522,23 +524,30 @@
 
     if renamings:
         content = _fix_variable_names(content, renamings, preserve)
 
     return content
 
 
-def _iter_defs_recursive(
+def _iter_bodies_recursive(
     ast_root: ast.Module,
 ) -> Iterable[Union[ast.FunctionDef, ast.ClassDef, ast.AsyncFunctionDef]]:
     left = list(ast_root.body)
     while left:
         for node in left.copy():
             left.remove(node)
-            if isinstance(node, (ast.FunctionDef, ast.ClassDef, ast.AsyncFunctionDef)):
+            if isinstance(
+                node,
+                (ast.FunctionDef, ast.ClassDef, ast.AsyncFunctionDef, ast.For, ast.While, ast.With),
+            ):
+                left.extend(node.body)
+                yield node
+            if isinstance(node, ast.If):
                 left.extend(node.body)
+                left.extend(node.orelse)
                 yield node
 
 
 def _unique_assignment_targets(
     node: Union[ast.Assign, ast.AnnAssign, ast.AugAssign, ast.For]
 ) -> Collection[ast.Name]:
     targets = set()
@@ -580,40 +589,50 @@
         reference_nodes = {
             node
             for node in ast.walk(def_node)
             if isinstance(node, ast.Name) and isinstance(node.ctx, ast.Load)
         }
         body = queue.PriorityQueue()
         for node in def_node.body:
-            body.put((node.lineno, node))
+            body.put((node.lineno, node, None))
         while not body.empty():
-            _, node = body.get()
-            if isinstance(node, ast.For):
+            _, node, containing_loop_node = body.get()
+            if isinstance(node, (ast.For, ast.While)):
                 for subnode in reversed(node.body):
-                    body.put((subnode.lineno, subnode))
+                    body.put((subnode.lineno, subnode, containing_loop_node or node))
+            elif isinstance(node, ast.If):
+                for subnode in node.body:
+                    body.put((subnode.lineno, subnode, containing_loop_node))
+                for subnode in node.orelse:
+                    body.put((subnode.lineno, subnode, containing_loop_node))
             if isinstance(node, (ast.Assign, ast.AnnAssign, ast.AugAssign, ast.For)):
                 target_nodes = _unique_assignment_targets(node)
                 if not target_nodes:
                     continue
                 target_names = {x.id for x in target_nodes}
                 referenced_names = set()
                 starts = []
                 ends = []
+                if containing_loop_node is not None:
+                    loop_start, loop_end = parsing.get_charnos(containing_loop_node, content)
+                else:
+                    loop_start = loop_end = -1
                 for target_node in target_nodes:
                     s, e = parsing.get_charnos(target_node, content)
                     starts.append(s)
                     ends.append(e)
                 start = min(starts)
                 end = max(ends)
                 for refnode in reference_nodes:
                     n_start, n_end = parsing.get_charnos(refnode, content)
                     if (
                         end < n_start
                         or (isinstance(def_node, (ast.ClassDef, ast.Module)) and n_end < start)
                         or isinstance(def_node, ast.For)
+                        or loop_start <= n_start <= n_end <= loop_end
                     ):
                         referenced_names.add(refnode.id)
                 redundant_targets = target_names - referenced_names - imports
                 if def_node is ast_tree:
                     redundant_targets = redundant_targets - preserve
                 for target_node in target_nodes:
                     if isinstance(target_node, ast.Attribute):
@@ -708,14 +727,15 @@
         if isinstance(node, ast.Name) and isinstance(node.ctx, ast.Store)
     }
     function_defs = {
         node for node in ast.walk(root) if isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef))
     }
     builtin_names = set(dir(builtins))
     safe_callables = builtin_names - {"print", "exit"}
+    safe_callable_nodes = set()
     changes = True
     while changes:
         changes = False
         for node in function_defs:
             if node.name in defined_names:
                 continue
             nonreturn_children = [
@@ -725,17 +745,30 @@
                     child,
                     (ast.Return, ast.Yield, ast.YieldFrom, ast.Continue, ast.Break),
                 )
             ]
             if not any(
                 parsing.has_side_effect(child, safe_callables) for child in nonreturn_children
             ):
+                safe_callable_nodes.add(node)
                 safe_callables.add(node.name)
                 changes = True
         function_defs = {node for node in function_defs if node.name not in safe_callables}
+
+    for node in ast.walk(root):
+        if isinstance(node, ast.ClassDef):
+            constructors = {
+                child
+                for child in node.body
+                if isinstance(child, ast.FunctionDef)
+                and child.name in ("__init__", "__post_init__", "__new__")
+            }
+            if not constructors - safe_callable_nodes:
+                safe_callables.add(node.name)
+
     return safe_callables
 
 
 def delete_pointless_statements(content: str) -> str:
     """Delete pointless statements with no side effects from code
 
     Args:
@@ -743,63 +776,100 @@
 
     Returns:
         str: Modified code
     """
     ast_tree = ast.parse(content)
     delete = []
     safe_callables = _compute_safe_funcdef_calls(ast_tree)
-    for node in itertools.chain([ast_tree], _iter_defs_recursive(ast_tree)):
+    for node in itertools.chain([ast_tree], _iter_bodies_recursive(ast_tree)):
         for i, child in enumerate(node.body):
             if not parsing.has_side_effect(child, safe_callables):
                 if i > 0 or not (
                     isinstance(child, ast.Expr)
                     and isinstance(child.value, ast.Constant)
                     and isinstance(child.value.value, str)
                 ):
                     delete.append(child)
 
     content = remove_nodes(content, delete, ast_tree)
 
     return content
 
 
-def delete_unused_functions_and_classes(
-    content: str, preserve: Collection[str] = frozenset()
-) -> str:
-    """Delete unused functions and classes from code.
-
-    Args:
-        content (str): Python source code
-        preserve (Collection[str], optional): Names to preserve
-
-    Returns:
-        str: Python source code, where unused functions and classes have been deleted.
-    """
-    root = ast.parse(content)
-
-    defs = []
+def _get_unused_functions_classes(root: ast.AST, preserve: Collection[str]) -> Iterable[ast.AST]:
+    funcdefs = []
+    classdefs = []
     names = []
 
     for node in ast.walk(root):
-        if isinstance(node, (ast.FunctionDef, ast.ClassDef, ast.AsyncFunctionDef)):
-            defs.append(node)
-        elif isinstance(node, ast.Name):
+        if isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef)):
+            funcdefs.append(node)
+        elif isinstance(node, ast.ClassDef):
+            classdefs.append(node)
+        elif isinstance(node, ast.Name) and isinstance(node.ctx, ast.Load):
             names.append(node)
 
-    delete = []
-    for def_node in defs:
+    class_magics = collections.defaultdict(set)
+    for node in classdefs:
+        for child in node.body:
+            if (
+                isinstance(child, ast.FunctionDef)
+                and child.name.startswith("__")
+                and child.name.endswith("__")
+            ):
+                class_magics[node].add(child)
+
+    magic_source_classes = {}
+    for classdef, magics in class_magics.items():
+        for magic in magics:
+            magic_source_classes[magic] = classdef
+
+    for def_node in funcdefs:
         if def_node.name in preserve:
             continue
         usages = {node for node in names if node.id == def_node.name}
+        if parent_class := magic_source_classes.get(def_node):
+            usages.update(node for node in names if node.id == parent_class.name)
         recursive_usages = {
             node
             for node in ast.walk(def_node)
             if isinstance(node, ast.Name) and node.id == def_node.name
         }
         if not usages - recursive_usages:
             print(f"{def_node.name} is never used")
-            delete.append(def_node)
+            yield def_node
+
+    for def_node in classdefs:
+        if def_node.name in preserve:
             continue
+        usages = {node for node in names if node.id == def_node.name}
+        internal_usages = {
+            node
+            for node in ast.walk(def_node)
+            if isinstance(node, ast.Name)
+            and isinstance(node.ctx, ast.Load)
+            and node.id in (def_node.name, "self", "cls")
+        }
+        if not usages - internal_usages:
+            print(f"{def_node.name} is never used")
+            yield def_node
+
+
+def delete_unused_functions_and_classes(
+    content: str, preserve: Collection[str] = frozenset()
+) -> str:
+    """Delete unused functions and classes from code.
+
+    Args:
+        content (str): Python source code
+        preserve (Collection[str], optional): Names to preserve
+
+    Returns:
+        str: Python source code, where unused functions and classes have been deleted.
+    """
+    root = ast.parse(content)
+
+    delete = set(_get_unused_functions_classes(root, preserve))
 
     content = remove_nodes(content, delete, root)
 
     return content
```

### Comparing `pyrefact-8/pyrefact/main.py` & `pyrefact-9/pyrefact/main.py`

 * *Files identical despite different names*

### Comparing `pyrefact-8/pyrefact/parsing.py` & `pyrefact-9/pyrefact/parsing.py`

 * *Files identical despite different names*


# Comparing `tmp/jy-0.1.4.tar.gz` & `tmp/jy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jy-0.1.4.tar", last modified: Sat Dec 31 16:46:16 2022, max compression
+gzip compressed data, was "jy-0.1.5.tar", last modified: Sat Apr 29 15:44:22 2023, max compression
```

## Comparing `jy-0.1.4.tar` & `jy-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2022-12-31 16:46:16.532300 jy-0.1.4/
--rw-r--r--   0 thorwhalen   (501) staff       (20)    11357 2022-12-31 13:11:20.000000 jy-0.1.4/LICENSE
--rw-r--r--   0 thorwhalen   (501) staff       (20)     2837 2022-12-31 16:46:16.532740 jy-0.1.4/PKG-INFO
--rw-r--r--   0 thorwhalen   (501) staff       (20)     2554 2022-12-31 15:40:08.000000 jy-0.1.4/README.md
-drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2022-12-31 16:46:16.267006 jy-0.1.4/jy/
--rw-r--r--   0 thorwhalen   (501) staff       (20)       81 2022-12-31 14:20:22.000000 jy-0.1.4/jy/__init__.py
--rw-r--r--   0 thorwhalen   (501) staff       (20)     3201 2022-12-31 16:41:39.000000 jy-0.1.4/jy/bridge.py
--rw-r--r--   0 thorwhalen   (501) staff       (20)     4173 2022-12-31 16:45:33.000000 jy-0.1.4/jy/js_parse.py
-drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2022-12-31 16:46:16.507147 jy-0.1.4/jy/test/
--rw-r--r--   0 thorwhalen   (501) staff       (20)        0 2022-12-31 13:18:12.000000 jy-0.1.4/jy/test/__init__.py
--rw-r--r--   0 thorwhalen   (501) staff       (20)     1788 2022-12-31 15:38:14.000000 jy-0.1.4/jy/test/test_bridge.py
--rw-r--r--   0 thorwhalen   (501) staff       (20)     1028 2022-12-31 15:37:54.000000 jy-0.1.4/jy/test/test_js_parse.py
--rw-r--r--   0 thorwhalen   (501) staff       (20)     1733 2022-12-31 13:30:57.000000 jy-0.1.4/jy/util.py
-drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2022-12-31 16:46:16.434505 jy-0.1.4/jy.egg-info/
--rw-r--r--   0 thorwhalen   (501) staff       (20)     2837 2022-12-31 16:46:15.000000 jy-0.1.4/jy.egg-info/PKG-INFO
--rw-r--r--   0 thorwhalen   (501) staff       (20)      312 2022-12-31 16:46:15.000000 jy-0.1.4/jy.egg-info/SOURCES.txt
--rw-r--r--   0 thorwhalen   (501) staff       (20)        1 2022-12-31 16:46:15.000000 jy-0.1.4/jy.egg-info/dependency_links.txt
--rw-r--r--   0 thorwhalen   (501) staff       (20)        1 2022-12-31 16:46:15.000000 jy-0.1.4/jy.egg-info/not-zip-safe
--rw-r--r--   0 thorwhalen   (501) staff       (20)       15 2022-12-31 16:46:15.000000 jy-0.1.4/jy.egg-info/requires.txt
--rw-r--r--   0 thorwhalen   (501) staff       (20)        3 2022-12-31 16:46:15.000000 jy-0.1.4/jy.egg-info/top_level.txt
--rw-r--r--   0 thorwhalen   (501) staff       (20)      545 2022-12-31 16:46:16.535407 jy-0.1.4/setup.cfg
--rw-r--r--   0 thorwhalen   (501) staff       (20)       91 2022-12-31 13:11:20.000000 jy-0.1.4/setup.py
+drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-04-29 15:44:22.186750 jy-0.1.5/
+-rw-r--r--   0 thorwhalen   (501) staff       (20)    11357 2023-01-17 08:03:54.000000 jy-0.1.5/LICENSE
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     2837 2023-04-29 15:44:22.187144 jy-0.1.5/PKG-INFO
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     2554 2023-01-17 08:03:54.000000 jy-0.1.5/README.md
+drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-04-29 15:44:21.446619 jy-0.1.5/jy/
+-rw-r--r--   0 thorwhalen   (501) staff       (20)       81 2023-01-17 08:03:54.000000 jy-0.1.5/jy/__init__.py
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     3378 2023-04-29 15:37:23.000000 jy-0.1.5/jy/bridge.py
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     4275 2023-04-29 15:42:06.000000 jy-0.1.5/jy/js_parse.py
+drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-04-29 15:44:22.183442 jy-0.1.5/jy/test/
+-rw-r--r--   0 thorwhalen   (501) staff       (20)        0 2023-01-17 08:03:54.000000 jy-0.1.5/jy/test/__init__.py
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     1788 2023-01-17 08:03:54.000000 jy-0.1.5/jy/test/test_bridge.py
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     1028 2023-01-17 08:03:54.000000 jy-0.1.5/jy/test/test_js_parse.py
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     1733 2023-01-17 08:03:54.000000 jy-0.1.5/jy/util.py
+drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-04-29 15:44:22.132220 jy-0.1.5/jy.egg-info/
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     2837 2023-04-29 15:44:19.000000 jy-0.1.5/jy.egg-info/PKG-INFO
+-rw-r--r--   0 thorwhalen   (501) staff       (20)      312 2023-04-29 15:44:20.000000 jy-0.1.5/jy.egg-info/SOURCES.txt
+-rw-r--r--   0 thorwhalen   (501) staff       (20)        1 2023-04-29 15:44:19.000000 jy-0.1.5/jy.egg-info/dependency_links.txt
+-rw-r--r--   0 thorwhalen   (501) staff       (20)        1 2023-04-29 15:44:19.000000 jy-0.1.5/jy.egg-info/not-zip-safe
+-rw-r--r--   0 thorwhalen   (501) staff       (20)       15 2023-04-29 15:44:19.000000 jy-0.1.5/jy.egg-info/requires.txt
+-rw-r--r--   0 thorwhalen   (501) staff       (20)        3 2023-04-29 15:44:19.000000 jy-0.1.5/jy.egg-info/top_level.txt
+-rw-r--r--   0 thorwhalen   (501) staff       (20)      545 2023-04-29 15:44:22.212453 jy-0.1.5/setup.cfg
+-rw-r--r--   0 thorwhalen   (501) staff       (20)       91 2023-01-17 08:03:55.000000 jy-0.1.5/setup.py
```

### Comparing `jy-0.1.4/LICENSE` & `jy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jy-0.1.4/PKG-INFO` & `jy-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tools to control JS from Python (jy for Js pY or Js python proxY)
 Home-page: https://github.com/thorwhalen/jy
 Author: Thor Whalen
 License: apache-2.0
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jy-0.1.4/README.md` & `jy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `jy-0.1.4/jy/bridge.py` & `jy-0.1.5/jy/bridge.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Python portals to JS"""
 
-from typing import Any
+from typing import Any, Optional
 from functools import partial
 
 from dol.signatures import Sig
 
 from jy.js_parse import dflt_py_to_js_value_trans, func_name_and_params_pairs
 
+
 # TODO: Add value transformer (routing). For example, booleans, True->true
 def _js_func_call(
     *args,
     __sig,
     __func_call_template,
     __value_trans=dflt_py_to_js_value_trans,
     __apply_defaults=True,
@@ -20,14 +21,16 @@
         args, kwargs, apply_defaults=__apply_defaults
     )
     inputs = map(__value_trans, _kwargs.values())
     inputs = ', '.join(map(str, inputs))
     return __func_call_template.format(inputs=inputs)
 
 
+# TODO: value_trans only sees value. Might want to transform according to other
+#  contextural information, like the parameter name, or the function name, etc.
 def mk_py_binder_func(
     name,
     params,
     *,
     prefix='',
     suffix='',
     doc='',
@@ -59,16 +62,16 @@
     """
 
 
 def add_js_funcs(
     js_code: str,
     *,
     obj: Any = None,
-    name: str | None = None,
-    encoding: str | None = None,
+    name: Optional[str] = None,
+    encoding: Optional[str] = None,
     forbidden_method_names=(),
     apply_defaults=True
 ):
     '''
     Add js call functions as attributes to an object.
 
     If object is not given, ``add_js_funcs`` will use a new ``JsBridge`` instance.
```

### Comparing `jy-0.1.4/jy/js_parse.py` & `jy-0.1.5/jy/js_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Utils to parse JS"""
 
 import os
 from pathlib import Path
 from functools import wraps
 from itertools import chain
+from typing import Optional
+import json
 
 import esprima
 
 AstScript = esprima.nodes.Script
 AstNode = esprima.nodes.Node
 
 
@@ -36,15 +38,15 @@
                 return output
 
         return _func
 
     return _if_none_output_raise_wrapper
 
 
-def parse_js_code(js_code: str, encoding: str | None = None) -> AstScript:
+def parse_js_code(js_code: str, encoding: Optional[str] = None) -> AstScript:
     if os.path.isfile(js_code):
         js_code = Path(js_code).read_text(encoding=encoding)
     return esprima.parse(js_code)
 
 
 @if_none_output_raise_unknown_type("to extract obj name from")
 def _extract_obj_name(x: AstNode, /):
@@ -127,8 +129,10 @@
 
 
 def dflt_py_to_js_value_trans(x):
     if isinstance(x, bool):
         return str(x).lower()
     elif isinstance(x, str):
         return f'"{x}"'  # surround with quotes
+    elif isinstance(x, dict):
+        return json.dumps(x)
     return x
```

### Comparing `jy-0.1.4/jy/test/test_bridge.py` & `jy-0.1.5/jy/test/test_bridge.py`

 * *Files identical despite different names*

### Comparing `jy-0.1.4/jy/test/test_js_parse.py` & `jy-0.1.5/jy/test/test_js_parse.py`

 * *Files identical despite different names*

### Comparing `jy-0.1.4/jy/util.py` & `jy-0.1.5/jy/util.py`

 * *Files identical despite different names*

### Comparing `jy-0.1.4/jy.egg-info/PKG-INFO` & `jy-0.1.5/jy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tools to control JS from Python (jy for Js pY or Js python proxY)
 Home-page: https://github.com/thorwhalen/jy
 Author: Thor Whalen
 License: apache-2.0
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jy-0.1.4/setup.cfg` & `jy-0.1.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jy
-version = 0.1.4
+version = 0.1.5
 url = https://github.com/thorwhalen/jy
 platforms = any
 description_file = README.md
 root_url = https://github.com/thorwhalen/
 license = apache-2.0
 author = Thor Whalen
 description = Tools to control JS from Python (jy for Js pY or Js python proxY)
```


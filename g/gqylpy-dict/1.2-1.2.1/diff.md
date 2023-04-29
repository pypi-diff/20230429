# Comparing `tmp/gqylpy_dict-1.2.tar.gz` & `tmp/gqylpy_dict-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gqylpy_dict-1.2.tar", last modified: Sat Apr 22 03:59:15 2023, max compression
+gzip compressed data, was "gqylpy_dict-1.2.1.tar", last modified: Sat Apr 29 02:25:21 2023, max compression
```

## Comparing `gqylpy_dict-1.2.tar` & `gqylpy_dict-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:59:15.338949 gqylpy_dict-1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    12343 2023-04-22 03:59:04.000000 gqylpy_dict-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-22 03:59:04.000000 gqylpy_dict-1.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-22 03:59:15.338949 gqylpy_dict-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-22 03:59:04.000000 gqylpy_dict-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:59:15.338949 gqylpy_dict-1.2/gqylpy_dict/
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-22 03:59:04.000000 gqylpy_dict-1.2/gqylpy_dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-04-22 03:59:04.000000 gqylpy_dict-1.2/gqylpy_dict/g dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:59:15.338949 gqylpy_dict-1.2/gqylpy_dict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-22 03:59:15.000000 gqylpy_dict-1.2/gqylpy_dict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-22 03:59:15.000000 gqylpy_dict-1.2/gqylpy_dict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 03:59:15.000000 gqylpy_dict-1.2/gqylpy_dict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-22 03:59:15.000000 gqylpy_dict-1.2/gqylpy_dict.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 03:59:15.338949 gqylpy_dict-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-22 03:59:04.000000 gqylpy_dict-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:25:21.751060 gqylpy_dict-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12343 2023-04-29 02:25:08.000000 gqylpy_dict-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-29 02:25:08.000000 gqylpy_dict-1.2.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-29 02:25:21.747060 gqylpy_dict-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-29 02:25:08.000000 gqylpy_dict-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:25:21.747060 gqylpy_dict-1.2.1/gqylpy_dict/
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-04-29 02:25:08.000000 gqylpy_dict-1.2.1/gqylpy_dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-04-29 02:25:08.000000 gqylpy_dict-1.2.1/gqylpy_dict/g dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:25:21.747060 gqylpy_dict-1.2.1/gqylpy_dict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-29 02:25:21.000000 gqylpy_dict-1.2.1/gqylpy_dict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-29 02:25:21.000000 gqylpy_dict-1.2.1/gqylpy_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 02:25:21.000000 gqylpy_dict-1.2.1/gqylpy_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 02:25:21.000000 gqylpy_dict-1.2.1/gqylpy_dict.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 02:25:21.751060 gqylpy_dict-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-29 02:25:09.000000 gqylpy_dict-1.2.1/setup.py
```

### Comparing `gqylpy_dict-1.2/LICENSE` & `gqylpy_dict-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gqylpy_dict-1.2/NOTICE` & `gqylpy_dict-1.2.1/NOTICE`

 * *Files identical despite different names*

### Comparing `gqylpy_dict-1.2/PKG-INFO` & `gqylpy_dict-1.2.1/gqylpy_dict.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: gqylpy_dict
-Version: 1.2
-Summary: 基于内置 dict，它是对内置 dict 的增强。dict 能做的它能做，dict 不能做的它更能做。
+Name: gqylpy-dict
+Version: 1.2.1
+Summary: 基于内置 dict，它是对内置 dict 的增强。内置 dict 能做的它都能做，内置 dict 不能做的它更能做。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: WTFPL,Apache-2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-dict
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -27,15 +27,15 @@
 [![Release](https://img.shields.io/github/release/gqylpy/gqylpy-dict.svg?style=flat-square")](https://github.com/gqylpy/gqylpy-dict/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/gqylpy_dict)](https://pypi.org/project/gqylpy_dict)
 [![License](https://img.shields.io/pypi/l/gqylpy_dict)](https://github.com/gqylpy/gqylpy-dict/blob/master/LICENSE)
 [![Downloads](https://pepy.tech/badge/gqylpy_dict/month)](https://pepy.tech/project/gqylpy_dict)
 
 # gqylpy-dict
 
-> `gqylpy-dict` 基于内置 `dict`，它是对内置 `dict` 的增强。`dict` 能做的它能做，`dict` 不能做的它更能做。
+> `gqylpy-dict` 基于内置 `dict`，它是对内置 `dict` 的增强。内置 `dict` 能做的它都能做，内置 `dict` 不能做的它更能做。
 
 <kbd>pip3 install gqylpy_dict</kbd>
 
 ```python
 >>> from gqylpy_dict import gdict
 
 >>> gdict == dict
```

### Comparing `gqylpy_dict-1.2/README.md` & `gqylpy_dict-1.2.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![Release](https://img.shields.io/github/release/gqylpy/gqylpy-dict.svg?style=flat-square")](https://github.com/gqylpy/gqylpy-dict/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/gqylpy_dict)](https://pypi.org/project/gqylpy_dict)
 [![License](https://img.shields.io/pypi/l/gqylpy_dict)](https://github.com/gqylpy/gqylpy-dict/blob/master/LICENSE)
 [![Downloads](https://pepy.tech/badge/gqylpy_dict/month)](https://pepy.tech/project/gqylpy_dict)
 
 # gqylpy-dict
 
-> `gqylpy-dict` 基于内置 `dict`，它是对内置 `dict` 的增强。`dict` 能做的它能做，`dict` 不能做的它更能做。
+> `gqylpy-dict` 基于内置 `dict`，它是对内置 `dict` 的增强。内置 `dict` 能做的它都能做，内置 `dict` 不能做的它更能做。
 
 <kbd>pip3 install gqylpy_dict</kbd>
 
 ```python
 >>> from gqylpy_dict import gdict
 
 >>> gdict == dict
```

### Comparing `gqylpy_dict-1.2/gqylpy_dict/__init__.py` & `gqylpy_dict-1.2.1/gqylpy_dict/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     >>> x = gdict(x)
     >>> x.a[0].b
     'B'
 
     >>> x.deepget('a[0].b')
     'B'
 
-    @version: 1.2
+    @version: 1.2.1
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/gqylpy-dict
 
 ────────────────────────────────────────────────────────────────────────────────
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 This file is licensed under the WTFPL:
@@ -45,15 +45,15 @@
 from typing import Optional, Union, Tuple, List, Hashable, Any
 
 
 class gdict(dict):
 
     def __new__(cls, __data__={}, /, **data):
         if isinstance(__data__, dict):
-            return __data__ if __data__.__class__ is cls else dict.__new__(cls)
+            return dict.__new__(cls)
 
         if isinstance(__data__, (list, tuple, set, frozenset)):
             return __data__.__class__(cls(v) for v in __data__)
 
         return __data__
 
     def __init__(self, __data__=None, /, **data):
@@ -89,14 +89,27 @@
         Backstory https://github.com/gqylpy/gqylpy-dict/issues/7
         """
         return -2
 
     def copy(self) -> 'gdict':
         """Get a replica instance."""
 
+    def deepcopy(self) -> 'gdict':
+        """
+        Incomplete deep copy, NOTE not the same as `copy.deepcopy`!
+
+        Copy only the instances of container types (only instances of `dict`,
+        `gdict`, `list`, `tuple`, `set`, and `frozenset`). Just pass `self`
+        directly to `gdict`, you can view the code blocks for `gdict.__new__`
+        and `gdict.__init__`.
+
+        Backstory https://github.com/gqylpy/gqylpy-dict/issues/9
+        """
+        return gdict(self)
+
     def deepget(
             self,
             deepkey: str,
             /,
             default: Optional[Any]                          = None,
             *,
             ignore:  Optional[Union[Tuple[Any], List[Any]]] = None
@@ -208,15 +221,14 @@
         )
         cls.deepset(data, deepkey, value)
 
 
 class _xe6_xad_x8c_xe7_x90_xaa_xe6_x80_xa1_xe7_x8e_xb2_xe8_x90_x8d_xe4_xba_x91:
     import sys
 
-    __import__(f'{__name__}.g {__name__[7:]}')
-    gdict = globals()[f'g {__name__[7:]}'].GqylpyDict
+    gdict = __import__(f'{__name__}.g {__name__[7:]}', fromlist=...).GqylpyDict
 
-    for gname in globals():
+    for gname, gvalue in globals().items():
         if gname[0] == '_' and gname != '__name__':
-            setattr(gdict, gname, globals()[gname])
+            setattr(gdict, gname, gvalue)
 
     sys.modules[__name__] = gdict.gdict = gdict
```

### Comparing `gqylpy_dict-1.2/gqylpy_dict/g dict.py` & `gqylpy_dict-1.2.1/gqylpy_dict/g dict.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             __data__.update(data)
 
         for name, value in __data__.items():
             dict.__setitem__(self, name, GqylpyDict(value))
 
     def __new__(cls, __data__={}, /, **data):
         if isinstance(__data__, dict):
-            return __data__ if __data__.__class__ is cls else dict.__new__(cls)
+            return dict.__new__(cls)
 
         if isinstance(__data__, (list, tuple, set, frozenset)):
             return __data__.__class__(cls(v) for v in __data__)
 
         return __data__
 
     def __getattr__(self, name: str, /) -> Any:
@@ -137,14 +137,17 @@
 
     def copy(self) -> 'GqylpyDict':
         copied = GqylpyDict()
         for name, value in self.items():
             dict.__setitem__(copied, name, value)
         return copied
 
+    def deepcopy(self) -> 'GqylpyDict':
+        return GqylpyDict(self)
+
     def update(self, __data__: Optional[dict] = None, /, **data) -> None:
         try:
             dict.update(self, GqylpyDict(
                 *() if __data__ is None else (__data__,), **data
             ))
         except (TypeError, ValueError):
             x: str = __data__.__class__.__name__
@@ -171,16 +174,22 @@
                     return default
             try:
                 value = value[key]
             except KeyError:
                 try:
                     if key.isdigit() or key[0] == '-' and key[1:].isdigit():
                         value = value[int(key)]
-                    elif key in ('None', 'True', 'False', 'Ellipsis'):
-                        value = value[eval(key)]
+                    elif key == 'None':
+                        value = value[None]
+                    elif key == 'True':
+                        value = value[True]
+                    elif key == 'False':
+                        value = value[False]
+                    elif key == 'Ellipsis':
+                        value = value[...]
                     else:
                         return default
                 except (KeyError, IndexError):
                     return default
             except (IndexError, TypeError):
                 return default
```

### Comparing `gqylpy_dict-1.2/gqylpy_dict.egg-info/PKG-INFO` & `gqylpy_dict-1.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: gqylpy-dict
-Version: 1.2
-Summary: 基于内置 dict，它是对内置 dict 的增强。dict 能做的它能做，dict 不能做的它更能做。
+Name: gqylpy_dict
+Version: 1.2.1
+Summary: 基于内置 dict，它是对内置 dict 的增强。内置 dict 能做的它都能做，内置 dict 不能做的它更能做。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: WTFPL,Apache-2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-dict
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -27,15 +27,15 @@
 [![Release](https://img.shields.io/github/release/gqylpy/gqylpy-dict.svg?style=flat-square")](https://github.com/gqylpy/gqylpy-dict/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/gqylpy_dict)](https://pypi.org/project/gqylpy_dict)
 [![License](https://img.shields.io/pypi/l/gqylpy_dict)](https://github.com/gqylpy/gqylpy-dict/blob/master/LICENSE)
 [![Downloads](https://pepy.tech/badge/gqylpy_dict/month)](https://pepy.tech/project/gqylpy_dict)
 
 # gqylpy-dict
 
-> `gqylpy-dict` 基于内置 `dict`，它是对内置 `dict` 的增强。`dict` 能做的它能做，`dict` 不能做的它更能做。
+> `gqylpy-dict` 基于内置 `dict`，它是对内置 `dict` 的增强。内置 `dict` 能做的它都能做，内置 `dict` 不能做的它更能做。
 
 <kbd>pip3 install gqylpy_dict</kbd>
 
 ```python
 >>> from gqylpy_dict import gdict
 
 >>> gdict == dict
```

### Comparing `gqylpy_dict-1.2/setup.py` & `gqylpy_dict-1.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     name=g.__package__,
     version=version,
     author=author,
     author_email=email,
     license='WTFPL,Apache-2.0',
     url='http://gqylpy.com',
     project_urls={'Source': source},
-    description='基于内置 dict，它是对内置 dict 的增强。dict 能做的它能做，dict 不能做'
-                '的它更能做。',
+    description='基于内置 dict，它是对内置 dict 的增强。内置 dict 能做的它都能做，内置'
+                ' dict 不能做的它更能做。',
     long_description=open('README.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     packages=[g.__package__],
     python_requires='>=3.8, <4',
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
```


# Comparing `tmp/pyarmor.cli.core-2.1.dev9-cp39-none-win_amd64.whl.zip` & `tmp/pyarmor.cli.core-3.2.dev1-cp39-none-win32.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 637892 bytes, number of entries: 7
--rw-r--r--  2.0 unx     3311 b- defN 23-Mar-31 08:45 pyarmor/cli/core/__init__.py
--rwxr-xr-x  2.0 unx   610816 b- defN 23-Apr-08 23:50 pyarmor/cli/core/pyarmor_runtime.pyd
--rwxr-xr-x  2.0 unx   689664 b- defN 23-Apr-08 23:50 pyarmor/cli/core/pytransform3.pyd
--rw-r--r--  2.0 unx     1892 b- defN 23-Apr-08 23:50 pyarmor.cli.core-2.1.dev9.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-08 23:50 pyarmor.cli.core-2.1.dev9.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-08 23:50 pyarmor.cli.core-2.1.dev9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      617 b- defN 23-Apr-08 23:50 pyarmor.cli.core-2.1.dev9.dist-info/RECORD
-7 files, 1306407 bytes uncompressed, 636792 bytes compressed:  51.3%
+Zip file size: 702378 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     3857 b- defN 23-Apr-14 09:43 pyarmor/cli/core/__init__.py
+-rw-r--r--  2.0 unx     2394 b- defN 23-Apr-14 09:46 pyarmor/cli/core/fixup.py
+-rwxr-xr-x  2.0 unx   757774 b- defN 23-Apr-29 01:11 pyarmor/cli/core/pyarmor_runtime.pyd
+-rwxr-xr-x  2.0 unx   849920 b- defN 23-Apr-29 01:11 pyarmor/cli/core/pytransform3.pyd
+-rw-r--r--  2.0 unx     1892 b- defN 23-Apr-29 01:11 pyarmor.cli.core-3.2.dev1.dist-info/METADATA
+-rw-r--r--  2.0 unx       95 b- defN 23-Apr-29 01:11 pyarmor.cli.core-3.2.dev1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-29 01:11 pyarmor.cli.core-3.2.dev1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      699 b- defN 23-Apr-29 01:11 pyarmor.cli.core-3.2.dev1.dist-info/RECORD
+8 files, 1616639 bytes uncompressed, 701152 bytes compressed:  56.6%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: pyarmor/cli/core/__init__.py
 Comment: 
 
+Filename: pyarmor/cli/core/fixup.py
+Comment: 
+
 Filename: pyarmor/cli/core/pyarmor_runtime.pyd
 Comment: 
 
 Filename: pyarmor/cli/core/pytransform3.pyd
 Comment: 
 
-Filename: pyarmor.cli.core-2.1.dev9.dist-info/METADATA
+Filename: pyarmor.cli.core-3.2.dev1.dist-info/METADATA
 Comment: 
 
-Filename: pyarmor.cli.core-2.1.dev9.dist-info/WHEEL
+Filename: pyarmor.cli.core-3.2.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: pyarmor.cli.core-2.1.dev9.dist-info/top_level.txt
+Filename: pyarmor.cli.core-3.2.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli.core-2.1.dev9.dist-info/RECORD
+Filename: pyarmor.cli.core-3.2.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyarmor/cli/core/__init__.py

```diff
@@ -25,23 +25,40 @@
 # Each log
 #    revision, age, (new features), (changed features), (removed features)
 __CHANGE_LOGS__ = (
     (1, 0, (), (), ()),
 )
 
 
+def _import_pytransform3():
+    try:
+        return __import__(
+            'pytransform3', globals=globals(), locals=locals(),
+            fromlist=('__pyarmor__',), level=1
+        )
+    except ImportError as e:
+        # Fix library not load issue
+        from .fixup import _fixup_library_not_load
+        rc = _fixup_library_not_load(getattr(e, 'path', None))
+        if rc == 0:
+            return __import__(
+                'pytransform3', globals=globals(), locals=locals(),
+                fromlist=('__pyarmor__',), level=1
+            )
+        raise
+
+
 class Pytransform3(object):
 
     _pytransform3 = None
 
     @staticmethod
     def init(ctx=None):
         if Pytransform3._pytransform3 is None:
-            from . import pytransform3 as m
-            Pytransform3._pytransform3 = m
+            Pytransform3._pytransform3 = m = _import_pytransform3()
             if ctx:
                 m.init_ctx(ctx)
         return Pytransform3._pytransform3
 
     @staticmethod
     def generate_obfuscated_script(ctx, res):
         m = Pytransform3.init(ctx)
```

## Comparing `pyarmor.cli.core-2.1.dev9.dist-info/METADATA` & `pyarmor.cli.core-3.2.dev1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarmor.cli.core
-Version: 2.1.dev9
+Version: 3.2.dev1
 Summary: Provide extension module pytransform3 for Pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Keywords: protect obfuscate encrypt obfuscation distribute
 Platform: UNKNOWN
```


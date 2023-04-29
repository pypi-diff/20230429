# Comparing `tmp/gqylpy_datastruct-2.2.4-py3-none-any.whl.zip` & `tmp/gqylpy_datastruct-2.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 17200 bytes, number of entries: 7
--rw-r--r--  2.0 unx     7474 b- defN 23-Apr-22 03:40 gqylpy_datastruct/__init__.py
--rw-r--r--  2.0 unx    34341 b- defN 23-Apr-22 03:40 gqylpy_datastruct/g datastruct.py
--rw-r--r--  2.0 unx    11389 b- defN 23-Apr-22 03:41 gqylpy_datastruct-2.2.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     8064 b- defN 23-Apr-22 03:41 gqylpy_datastruct-2.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 03:41 gqylpy_datastruct-2.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Apr-22 03:41 gqylpy_datastruct-2.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      614 b- defN 23-Apr-22 03:41 gqylpy_datastruct-2.2.4.dist-info/RECORD
-7 files, 61992 bytes uncompressed, 16104 bytes compressed:  74.0%
+Zip file size: 16407 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     4265 b- defN 23-Apr-29 01:56 gqylpy_datastruct/__init__.py
+-rw-r--r--  2.0 unx    34341 b- defN 23-Apr-29 01:56 gqylpy_datastruct/g datastruct.py
+-rw-r--r--  2.0 unx    11389 b- defN 23-Apr-29 01:57 gqylpy_datastruct-2.2.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7966 b- defN 23-Apr-29 01:57 gqylpy_datastruct-2.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-29 01:57 gqylpy_datastruct-2.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Apr-29 01:57 gqylpy_datastruct-2.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      614 b- defN 23-Apr-29 01:57 gqylpy_datastruct-2.2.5.dist-info/RECORD
+7 files, 58685 bytes uncompressed, 15311 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: gqylpy_datastruct/__init__.py
 Comment: 
 
 Filename: gqylpy_datastruct/g datastruct.py
 Comment: 
 
-Filename: gqylpy_datastruct-2.2.4.dist-info/LICENSE
+Filename: gqylpy_datastruct-2.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: gqylpy_datastruct-2.2.4.dist-info/METADATA
+Filename: gqylpy_datastruct-2.2.5.dist-info/METADATA
 Comment: 
 
-Filename: gqylpy_datastruct-2.2.4.dist-info/WHEEL
+Filename: gqylpy_datastruct-2.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: gqylpy_datastruct-2.2.4.dist-info/top_level.txt
+Filename: gqylpy_datastruct-2.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: gqylpy_datastruct-2.2.4.dist-info/RECORD
+Filename: gqylpy_datastruct-2.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gqylpy_datastruct/__init__.py

```diff
@@ -2,15 +2,15 @@
 Create a blueprint to draw the data structure of your program, and then use this
 blueprint to verify that the incoming data is correct.
 
     >>> from gqylpy_datastruct import DataStruct
     >>> datastruct = DataStruct({'name': {type: str}})
     >>> err = datastruct.verify({'name': 'Alpha'})
 
-    @version: 2.2.4
+    @version: 2.2.5
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/gqylpy-datastruct
 
 ────────────────────────────────────────────────────────────────────────────────
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
@@ -21,26 +21,27 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
+from typing import Optional, Union
 
 
 class DataStruct:
 
     def __init__(
             self,
             blueprint: dict,
             *,
-            eraise:                bool = None,
-            etitle:                str  = None,
-            ignore_undefined_data: bool = None,
-            allowable_placeholder: list = None
+            eraise:                Optional[bool] = None,
+            etitle:                Optional[str]  = None,
+            ignore_undefined_data: Optional[bool] = None,
+            allowable_placeholder: Optional[list] = None
     ):
         """
         @param blueprint
             Receive a data blueprint.
 
             See the documentation at
                 https://github.com/gqylpy/gqylpy-datastruct
@@ -68,18 +69,18 @@
         """
         self.blueprint = blueprint
 
     def verify(
             self,
             data: dict,
             *,
-            eraise:                bool = None,
-            etitle:                str  = None,
-            ignore_undefined_data: bool = None
-    ) -> 'Union[dict, None]':
+            eraise:                Optional[bool] = None,
+            etitle:                Optional[str]  = None,
+            ignore_undefined_data: Optional[bool] = None
+    ) -> Union[dict, None]:
         """
         @param data
             The data to be verified.
 
         @param eraise
             By default, error information is returned as a return value, but if
             you want to raise an exception based on this error information, can
@@ -94,71 +95,21 @@
             data, can set this parameter to True.
 
         @return: The error information if verification fails.
         """
 
 
 class _xe6_xad_x8c_xe7_x90_xaa_xe6_x80_xa1_xe7_x8e_xb2_xe8_x90_x8d_xe4_xba_x91:
-    """  QYYYQLLYYYYYYYQLYYQYYQQQYQQYQQQQQQQQQQQQQQQQQQQQQQYYYQQQQQQYL
-        YYYYQYLLQYLLYYQYYYYYYYQQYQYQYQQQQQQQQQQQQQQQQQQQQQQQYYYQQQQQQ
-        QYYYYLPQYLPLYYYLLYYYYYYYYQQQYQQQQQQQQQQQQQQQQQQQQQQQYYYYQQQQQP
-        QYYQLPLQYLLYYQPLLLYYYYYYQYYQYQQQQQQQQQQQQQQYQQQQQQQQYYQYQQQQQQP
-       QYYQYLLYYYLLYQYLLYYYYYYYYQYYQYQYYYQQQQQQQQQQYQQQQQQYQQYQYYQQQQQYP
-      LQYQYYYYQYYYYYQYYYYYYYYYYYYYYYQQYYYYYYYYYQQQQYQQQQQQYQQYQYYQQQQQQ P
-      QYQQYYYYQYYYQQQYYYYYYYYQYQYYYYQQYYYQYQYYQQQQYQQQQQQQYQQYQYYQQQQQQ P
-      QYQQYYYYQYYYQQQYYYYYYYYQYQYYYYYQYYYYQYYYQQQQYQQQQQQQYQQYQQYQQQQYYP
-      QYQYYYYYQYYYQQQ PYLLLYP PLYYYYYYQYYYYYYQQQQYYQQQQQQYQQYQQQYQQQQYQ
-      PQQYYYYYQYYQQYQQQQQQQQQQYP        PPLYQYQYQYQLQQQQQYQQYQQQYYQQQYY
-       QQYYYYYQQYQLYQQPQQQQQL QYL           PPYYLYYLQYQQYYQYQQQQYYQPQYL
-       YQYYYYQQQYQ  LYLQQQQQQYQQ           YQQQQQGQQQQQQYQYYQQQQYQPQYQ P
-      L QYYYYQQLYQ   Y YPYQQQQQ           LQQQQQL YQQQQYQQYQYQQYYQQYQP P
-        YYQYYQQ  Q    LQQQQQQY            YQYQQQQQQYYQYLQYQQYQQYYQYQL P
-     Y  LYQLQQPL Y     P  P                QLLQQQQQ Q  PQQQQYQQYYQQL P
-    P   PYQYQQQQPQ                         PQQQQQQY    QQYQYYQQYYQPP
-    L    QQQYQ YYYY              PQ           L  P    LPQYQYYQQLQ P
-    Y   PPQQYYL LYQL                                 PQLQYQQYQYQ  L
-    Y     QQYQPP PYQY        PQ                      Q  QQYQYQYL  L
-    Y     QQYYQ L  QYQP         PLLLLLYL           LQQ LQYYQQQP P L
-     L   PPLQYYQ Y  LQQQ                         LQYQ  QYYYQQ     P
-      L    Q  QYQ  Y  QQPYL                   PQYYYYPPQYYQQQP    L
-       L    L  PQQL   LYQ  PQP             QL PYYYPLQLYQ  QY P   Y
-         P   P    PQQP  QY  QLLQQP   LYYLQ   PQYPQQQP P  QY P   L
-                       PYQYYY           PQ  PQ      L   Q P    L
-              PQYLYYYPQ PLPL             L QY YQYYQYLYQQQ    P
-            PYLLLLLYYYQ P  L    P         PYL  PQYYLLLLLLLQ
-           LYPLLLLLLYYYY   Y  YQY     LLLPPY   LYYYLLLLLLLLY
-           YLLLYLLLLLLYYQ  Q              PQ  YYYLLLLLLLLLLYP
-          YLLLLLLLLLLLLLLYQQ              PYYQYYLLLLLLLLYYYLQ
-          QLLLLLLLLLLLLLLLLLYYQYP        YQYYLLLLLLLLLLLLLLLQ
-          YLLLLLLLLLLLLLLLLLLLYYYLLYYYLLLLLLLLLLLLLLLLLLLLLLYP
-         PLLLLLLLLLLLLLLLLLLLLLLLYLLLLLLLLLLLLLLLLLLLLLLLYLYLL
-         LLLLLLLLLLYYLLLLLLYLLLLLLLLLLLLLLLL GQYLPY LLLYLYLLLY
-         QLLLLYYLYLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLQYYYYLLQ
-         QLLLLLYYQYLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLQLYYLLLQ
-        LYLLYLLLQYYLLLLLLLLLLLLLLLLLLLLLLLLLLLLLYLLLLLQYYYYYLYQ
-        YLLLYYLLYQYLLLLLLLLLLLLLLLLLLLLLLLLLLLLYLLLLLYYYYQLLLLY
-        QLLLYYYYYQLLLLLLLLLLLLLLYLLLLLLLLLLLLLLLLLLLLYYYLQLLPLLQ
-        YLYLLQYYYQLLLLLLLLLLLLLLLLLLLLLLLLLLLLYYLLLLLYYQYYLLLLLQ
-       LYLLLLLYYYQLLYLLLLLLLLLLLLYLYLLYYLLLLYLLLLLLLYYYQQLLLLLLLY
-       YLLLLLLYYYQLLYLLLLLLLYLYLLLLLLLLLLLLLLLLLLLLYYYYQQLYLLLLLQ
-       QLLLYLLLQYQLQLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLYYYQYYLLLLLLLY
-       QLLLLLLLLQQYQLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLQYYQYYLLLLLLLQ
-       QLLLLLLLLLQQYLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLYYYYLLLLLLLLLYL
-       QLLLLYLYYLYQLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLQYYYLLLLLLLLLQ
-       YLLLLLLLYYLQLLLLLLLLLLLLLLLLLLLLLLLLLYLLLLLLLLYQYYLLLLLLLLLQ
-       QLLLLLYLYYYYLLLLLPLLLLLLLYLYLLLLLLLLLLLLLLLLLLLQYYLLLLLLLLYP
-       YYLYYLLYYYQLLLLLLLLYLLLLLLLLLLLLLLLLLLLLLLYLYLLYQYYLLLLLLYL
-        QLLLLLLYQYLLLLLLLLLLLLLLLLLLLLLYYLYLLLLLLLLLLLYQQQQQQQLYL  """
-    import sys
-
-    __import__(f'{__name__}.{__name__[0]} {__name__[7:]}')
-    gpack = sys.modules[__name__]
-    gcode = globals()[f'{__name__[0]} {__name__[7:]}']
-
-    for gname in globals():
-        if gname[0] != '_' and hasattr(gcode, gname):
+    gpack = globals()
+    gpath = f'{__name__}.{__name__[0]} {__name__[7:]}'
+    gcode = __import__(gpath, fromlist=...)
+
+    for gname in gpack:
+        try:
+            assert gname[0] != '_'
             gfunc = getattr(gcode, gname)
-            gfunc.__module__ = __package__
-            setattr(gpack, gname, gfunc)
-
-
-from typing import Union
+            assert gfunc.__module__ == gpath
+        except (AssertionError, AttributeError):
+            continue
+        gfunc.__module__ = __package__
+        gfunc.__doc__ = gpack[gname].__doc__
+        gpack[gname] = gfunc
```

## Comparing `gqylpy_datastruct-2.2.4.dist-info/LICENSE` & `gqylpy_datastruct-2.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gqylpy_datastruct-2.2.4.dist-info/METADATA` & `gqylpy_datastruct-2.2.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: gqylpy-datastruct
-Version: 2.2.4
+Version: 2.2.5
 Summary: 创建一张蓝图来规划好程序需要的数据结构，并在之后使用该蓝图去校验到来的数据是否如期。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-datastruct
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: Topic :: Utilities
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: gqylpy-exception (>=2.0)
+Requires-Dist: gqylpy-exception (>=2.0.1)
 
 [<img alt="LOGO" src="http://www.gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/gqylpy-datastruct.svg?style=flat-square")](https://github.com/gqylpy/gqylpy-datastruct/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/gqylpy_datastruct)](https://pypi.org/project/gqylpy_datastruct)
 [![License](https://img.shields.io/pypi/l/gqylpy_datastruct)](https://github.com/gqylpy/gqylpy-datastruct/blob/master/LICENSE)
 [![Downloads](https://pepy.tech/badge/gqylpy_datastruct/month)](https://pepy.tech/project/gqylpy_datastruct)
```

## Comparing `gqylpy_datastruct-2.2.4.dist-info/RECORD` & `gqylpy_datastruct-2.2.5.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-gqylpy_datastruct/__init__.py,sha256=Ar7SqlYIA5UWyBzqj4ppyEjW2d_rJJb_dcjPi2cc4lU,7474
+gqylpy_datastruct/__init__.py,sha256=H8CqdAuLvLCfNcK1tFK2Pex98rEkvHxI8uxza3lUCHI,4265
 gqylpy_datastruct/g datastruct.py,sha256=ZoA3cIqR4fHHpeoaZrV_if-mok2EhP4A2uxaWGVIIS4,34341
-gqylpy_datastruct-2.2.4.dist-info/LICENSE,sha256=bLEM1yfc38Qf3r9KdVo81p4z2KLd41HT8sSzZ2DZQc4,11389
-gqylpy_datastruct-2.2.4.dist-info/METADATA,sha256=CETb-G-Bd-lx2RXVg1hro35gADfWEgPSGCerjL9MuyE,8064
-gqylpy_datastruct-2.2.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gqylpy_datastruct-2.2.4.dist-info/top_level.txt,sha256=1LhlNO-P1YOVg7hq9YDDm3p_57rXahXQDV0IxJnH_OY,18
-gqylpy_datastruct-2.2.4.dist-info/RECORD,,
+gqylpy_datastruct-2.2.5.dist-info/LICENSE,sha256=bLEM1yfc38Qf3r9KdVo81p4z2KLd41HT8sSzZ2DZQc4,11389
+gqylpy_datastruct-2.2.5.dist-info/METADATA,sha256=zDmgpcdQ-zdPWY7p3wmEP6j0GbKa28er0KD4hx8XUjo,7966
+gqylpy_datastruct-2.2.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gqylpy_datastruct-2.2.5.dist-info/top_level.txt,sha256=1LhlNO-P1YOVg7hq9YDDm3p_57rXahXQDV0IxJnH_OY,18
+gqylpy_datastruct-2.2.5.dist-info/RECORD,,
```


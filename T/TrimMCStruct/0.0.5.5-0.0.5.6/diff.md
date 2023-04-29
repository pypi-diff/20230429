# Comparing `tmp/TrimMCStruct-0.0.5.5.tar.gz` & `tmp/TrimMCStruct-0.0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrimMCStruct-0.0.5.5.tar", last modified: Wed Apr 19 13:43:57 2023, max compression
+gzip compressed data, was "TrimMCStruct-0.0.5.6.tar", last modified: Sat Apr 29 11:28:16 2023, max compression
```

## Comparing `TrimMCStruct-0.0.5.5.tar` & `TrimMCStruct-0.0.5.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 13:43:57.486110 TrimMCStruct-0.0.5.5/
--rw-rw-rw-   0        0        0     1277 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.5/LICENSE(origin).md
--rw-rw-rw-   0        0        0    13331 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.5/LICENSE.md
--rw-rw-rw-   0        0        0     5030 2023-04-19 13:43:57.485110 TrimMCStruct-0.0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     4022 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 13:43:57.474103 TrimMCStruct-0.0.5.5/TrimMCStruct/
--rw-rw-rw-   0        0        0      383 2023-04-19 13:40:40.000000 TrimMCStruct-0.0.5.5/TrimMCStruct/__init__.py
--rw-rw-rw-   0        0        0    21644 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.5/TrimMCStruct/main.py
-drwxrwxrwx   0        0        0        0 2023-04-19 13:43:57.484103 TrimMCStruct-0.0.5.5/TrimMCStruct.egg-info/
--rw-rw-rw-   0        0        0     5030 2023-04-19 13:43:57.000000 TrimMCStruct-0.0.5.5/TrimMCStruct.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-04-19 13:43:57.000000 TrimMCStruct-0.0.5.5/TrimMCStruct.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 13:43:57.000000 TrimMCStruct-0.0.5.5/TrimMCStruct.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-19 13:43:57.000000 TrimMCStruct-0.0.5.5/TrimMCStruct.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-19 13:43:57.000000 TrimMCStruct-0.0.5.5/TrimMCStruct.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 13:43:57.486110 TrimMCStruct-0.0.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1432 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:28:16.277547 TrimMCStruct-0.0.5.6/
+-rw-rw-rw-   0        0        0     1277 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.6/LICENSE(origin).md
+-rw-rw-rw-   0        0        0    13331 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.6/LICENSE.md
+-rw-rw-rw-   0        0        0     5030 2023-04-29 11:28:16.275553 TrimMCStruct-0.0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4022 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 11:28:16.259605 TrimMCStruct-0.0.5.6/TrimMCStruct/
+-rw-rw-rw-   0        0        0      383 2023-04-29 11:25:37.000000 TrimMCStruct-0.0.5.6/TrimMCStruct/__init__.py
+-rw-rw-rw-   0        0        0    21751 2023-04-29 11:25:31.000000 TrimMCStruct-0.0.5.6/TrimMCStruct/main.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:28:16.273560 TrimMCStruct-0.0.5.6/TrimMCStruct.egg-info/
+-rw-rw-rw-   0        0        0     5030 2023-04-29 11:28:15.000000 TrimMCStruct-0.0.5.6/TrimMCStruct.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-04-29 11:28:16.000000 TrimMCStruct-0.0.5.6/TrimMCStruct.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 11:28:15.000000 TrimMCStruct-0.0.5.6/TrimMCStruct.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-29 11:28:15.000000 TrimMCStruct-0.0.5.6/TrimMCStruct.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-29 11:28:15.000000 TrimMCStruct-0.0.5.6/TrimMCStruct.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 11:28:16.277547 TrimMCStruct-0.0.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     1432 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.6/setup.py
```

### Comparing `TrimMCStruct-0.0.5.5/LICENSE(origin).md` & `TrimMCStruct-0.0.5.6/LICENSE(origin).md`

 * *Files identical despite different names*

### Comparing `TrimMCStruct-0.0.5.5/LICENSE.md` & `TrimMCStruct-0.0.5.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TrimMCStruct-0.0.5.5/PKG-INFO` & `TrimMCStruct-0.0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrimMCStruct
-Version: 0.0.5.5
+Version: 0.0.5.6
 Summary: 读写操作《我的世界》.MCSTRUCTURE文件
 Home-page: https://github.com/TriM-Organization/TrimMCStruct
 Author: Eilles Wan, bgArray, phoenixr-codes(original author) 
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `TrimMCStruct-0.0.5.5/README.md` & `TrimMCStruct-0.0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `TrimMCStruct-0.0.5.5/TrimMCStruct/main.py` & `TrimMCStruct-0.0.5.6/TrimMCStruct/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 from functools import partial
 from itertools import repeat
 import json
 from typing import Any, BinaryIO, Optional, Tuple, Union, Dict
 
 import numpy as np
 from numpy.typing import NDArray
-from pynbt import BaseTag, NBTFile, TAG_Compound, TAG_Int, TAG_List, TAG_String, TAG_Byte, TAG_Long, TAG_Short  # type: ignore
+from pynbt import BaseTag, NBTFile, TAG_Compound, TAG_Int, TAG_List, TAG_String, TAG_Byte, TAG_Long, \
+    TAG_Short  # type: ignore
 
 Coordinate = Tuple[int, int, int]
 
 # Compatibility versioning number for blocks in 1.19.
 COMPABILITY_VERSION: int = 17959425
 
 
@@ -126,20 +127,20 @@
 
     namespace: str
     base_name: str
     states: dict[str, Union[int, str, bool]]
     extra_data: dict[str, Union[int, str, bool]]
 
     def __init__(
-        self,
-        namespace: str,
-        base_name: str,
-        states: dict[str, Union[int, str, bool]] = {},
-        extra_data: dict[str, Union[int, str, bool]] = {},
-        compability_version: int = COMPABILITY_VERSION,
+            self,
+            namespace: str,
+            base_name: str,
+            states: dict[str, Union[int, str, bool]] = {},
+            extra_data: dict[str, Union[int, str, bool]] = {},
+            compability_version: int = COMPABILITY_VERSION,
     ):
         """
         Parameters
         ----------
         namespace
             The namespace of the block (e.g. "minecraft").
         base_name
@@ -159,18 +160,18 @@
         self.base_name = base_name
         self.states = states
         self.extra_data = extra_data
         self.compability_version = compability_version
 
     @classmethod
     def from_identifier(
-        cls,
-        identifier: str,
-        compability_version=COMPABILITY_VERSION,
-        **states: Union[int, str, bool],
+            cls,
+            identifier: str,
+            compability_version=COMPABILITY_VERSION,
+            **states: Union[int, str, bool],
     ):
         """
         Parameters
         ----------
         identifier
             The identifier of the block (e.g. "minecraft:wool").
 
@@ -197,50 +198,50 @@
     def __str__(self) -> str:
         return self.stringify()
 
     def __dict__(self) -> dict:
         return self.dictionarify()
 
     def add_states(
-        self,
-        states: dict[str, Union[int, str, bool]],
+            self,
+            states: dict[str, Union[int, str, bool]],
     ) -> None:
         self.states.update(states)
 
     def add_extra_data(
-        self,
-        extra_data: dict[str, Union[int, str, bool]],
+            self,
+            extra_data: dict[str, Union[int, str, bool]],
     ) -> None:
         self.extra_data.update(extra_data)
 
     def dictionarify(self, *, with_states: bool = True) -> Dict[str, Any]:
         result = {
             "name": self.identifier,
             "states": self.states if with_states else {},
             "version": self.compability_version,
         }
 
         return result
 
     def dictionarify_with_block_entity(
-        self, *, with_states: bool = True
+            self, *, with_states: bool = True
     ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         result = {
             "name": self.identifier,
             "states": self.states if with_states else {},
             "version": self.compability_version,
         }
 
         return result, self.extra_data
 
     def stringify(
-        self,
-        *,
-        with_namespace: bool = True,
-        with_states: bool = True,
+            self,
+            *,
+            with_namespace: bool = True,
+            with_states: bool = True,
     ) -> str:
         result = ""
         if with_namespace:
             result += self.namespace + ":"
         result += self.get_name()
         if with_states:
             result += f" [{json.dumps(self.states)[1:-1]}]"
@@ -310,18 +311,18 @@
     _size
         The size of the structure.
     """
 
     structure_indecis: NDArray[np.intc]
 
     def __init__(
-        self,
-        size: tuple[int, int, int],
-        fill: Optional[Block] = None,
-        compability_version: int = COMPABILITY_VERSION,
+            self,
+            size: tuple[int, int, int],
+            fill: Optional[Block] = None,
+            compability_version: int = COMPABILITY_VERSION,
     ):
         """
         Parameters
         ----------
         size
             The size of the structure.
 
@@ -403,15 +404,15 @@
     def __repr__(self) -> str:
         return repr(self._get_str_array())
 
     def __str__(self) -> str:
         return str(self._get_str_array())
 
     def _get_str_array(
-        self, *, with_namespace: bool = False, with_states: bool = False
+            self, *, with_namespace: bool = False, with_states: bool = False
     ) -> NDArray[Any]:
         """
         Returns a numpy array where each entry is a
         readable string of the corresponding block.
 
         Parameters
         ----------
@@ -615,17 +616,17 @@
             ][
                 (index % (self.size[2] * self.size[1]) % self.size[2])
             ].extra_data = exdata
 
         return arr
 
     def set_block(
-        self,
-        coordinate: Coordinate,
-        block: Optional[Block],
+            self,
+            coordinate: Coordinate,
+            block: Optional[Block],
     ) -> Structure:
         """
         Puts a block into the structure.
 
         Parameters
         ----------
         coordinate
@@ -639,22 +640,22 @@
 
         ident = self._add_block_to_palette(block)
 
         self.structure_indecis[x, y, z] = ident
         if block.extra_data:
             self._special_blocks[
                 x * self.size[2] * self.size[1] + y * self.size[2] + z
-            ] = block.extra_data
+                ] = block.extra_data
         return self
 
     def fill_blocks(
-        self,
-        from_coordinate: Coordinate,
-        to_coordinate: Coordinate,
-        block: Block,
+            self,
+            from_coordinate: Coordinate,
+            to_coordinate: Coordinate,
+            block: Block,
     ) -> Structure:
         """
         Puts multiple blocks into the structure.
 
         Notes
         -----
         Both start and end points are filled.
@@ -671,17 +672,17 @@
             The block to place. If this is set to ``None``
             "STructure Void" blocks will be used to fill.
         """
         fx, fy, fz = from_coordinate
         tx, ty, tz = to_coordinate
 
         ident = self._add_block_to_palette(block)
-        
+
         # print([[[ident for k in range(abs(fz-tz)+1) ]for j in range(abs(fy-ty)+1)]for i in range(abs(fx-tx)+1)])
-        self.structure_indecis[fx : tx + 1, fy : ty + 1, fz : tz + 1] = np.array(
+        self.structure_indecis[fx: tx + 1, fy: ty + 1, fz: tz + 1] = np.array(
             [
                 [
                     [ident for k in range(abs(fz - tz) + 1)]
                     for j in range(abs(fy - ty) + 1)
                 ]
                 for i in range(abs(fx - tx) + 1)
             ],
@@ -697,16 +698,16 @@
                             for x in range(fx, tx)
                             for y in range(fy, ty)
                             for z in range(fz, tz)
                         ],
                         [
                             block.extra_data
                             for i in range(
-                                abs((fz - tz) + 1)
-                                * (abs(fy - ty) + 1)
-                                * (abs(fx - tx) + 1)
-                            )
+                            abs((fz - tz) + 1)
+                            * (abs(fy - ty) + 1)
+                            * (abs(fx - tx) + 1)
+                        )
                         ],
                     )
                 )
             )
         return self
```

### Comparing `TrimMCStruct-0.0.5.5/TrimMCStruct.egg-info/PKG-INFO` & `TrimMCStruct-0.0.5.6/TrimMCStruct.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrimMCStruct
-Version: 0.0.5.5
+Version: 0.0.5.6
 Summary: 读写操作《我的世界》.MCSTRUCTURE文件
 Home-page: https://github.com/TriM-Organization/TrimMCStruct
 Author: Eilles Wan, bgArray, phoenixr-codes(original author) 
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `TrimMCStruct-0.0.5.5/setup.py` & `TrimMCStruct-0.0.5.6/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/TrimMCStruct-0.0.5.6.tar.gz` & `tmp/TrimMCStruct-0.0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrimMCStruct-0.0.5.6.tar", last modified: Sat Apr 29 11:28:16 2023, max compression
+gzip compressed data, was "TrimMCStruct-0.0.5.8.tar", last modified: Sat Apr 29 14:12:16 2023, max compression
```

## Comparing `TrimMCStruct-0.0.5.6.tar` & `TrimMCStruct-0.0.5.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 11:28:16.277547 TrimMCStruct-0.0.5.6/
--rw-rw-rw-   0        0        0     1277 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.6/LICENSE(origin).md
--rw-rw-rw-   0        0        0    13331 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.6/LICENSE.md
--rw-rw-rw-   0        0        0     5030 2023-04-29 11:28:16.275553 TrimMCStruct-0.0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     4022 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 11:28:16.259605 TrimMCStruct-0.0.5.6/TrimMCStruct/
--rw-rw-rw-   0        0        0      383 2023-04-29 11:25:37.000000 TrimMCStruct-0.0.5.6/TrimMCStruct/__init__.py
--rw-rw-rw-   0        0        0    21751 2023-04-29 11:25:31.000000 TrimMCStruct-0.0.5.6/TrimMCStruct/main.py
-drwxrwxrwx   0        0        0        0 2023-04-29 11:28:16.273560 TrimMCStruct-0.0.5.6/TrimMCStruct.egg-info/
--rw-rw-rw-   0        0        0     5030 2023-04-29 11:28:15.000000 TrimMCStruct-0.0.5.6/TrimMCStruct.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-04-29 11:28:16.000000 TrimMCStruct-0.0.5.6/TrimMCStruct.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 11:28:15.000000 TrimMCStruct-0.0.5.6/TrimMCStruct.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-29 11:28:15.000000 TrimMCStruct-0.0.5.6/TrimMCStruct.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-29 11:28:15.000000 TrimMCStruct-0.0.5.6/TrimMCStruct.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 11:28:16.277547 TrimMCStruct-0.0.5.6/setup.cfg
--rw-rw-rw-   0        0        0     1432 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 14:12:16.556613 TrimMCStruct-0.0.5.8/
+-rw-rw-rw-   0        0        0     1277 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.8/LICENSE(origin).md
+-rw-rw-rw-   0        0        0    13331 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.8/LICENSE.md
+-rw-rw-rw-   0        0        0     5030 2023-04-29 14:12:16.555616 TrimMCStruct-0.0.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4022 2023-04-19 13:20:57.000000 TrimMCStruct-0.0.5.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 14:12:16.544682 TrimMCStruct-0.0.5.8/TrimMCStruct/
+-rw-rw-rw-   0        0        0      398 2023-04-29 14:06:24.000000 TrimMCStruct-0.0.5.8/TrimMCStruct/__init__.py
+-rw-rw-rw-   0        0        0    21789 2023-04-29 13:57:10.000000 TrimMCStruct-0.0.5.8/TrimMCStruct/main.py
+drwxrwxrwx   0        0        0        0 2023-04-29 14:12:16.554619 TrimMCStruct-0.0.5.8/TrimMCStruct.egg-info/
+-rw-rw-rw-   0        0        0     5030 2023-04-29 14:12:16.000000 TrimMCStruct-0.0.5.8/TrimMCStruct.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-04-29 14:12:16.000000 TrimMCStruct-0.0.5.8/TrimMCStruct.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 14:12:16.000000 TrimMCStruct-0.0.5.8/TrimMCStruct.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-29 14:12:16.000000 TrimMCStruct-0.0.5.8/TrimMCStruct.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-29 14:12:16.000000 TrimMCStruct-0.0.5.8/TrimMCStruct.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 14:12:16.556613 TrimMCStruct-0.0.5.8/setup.cfg
+-rw-rw-rw-   0        0        0     1495 2023-04-29 14:09:51.000000 TrimMCStruct-0.0.5.8/setup.py
```

### Comparing `TrimMCStruct-0.0.5.6/LICENSE(origin).md` & `TrimMCStruct-0.0.5.8/LICENSE(origin).md`

 * *Files identical despite different names*

### Comparing `TrimMCStruct-0.0.5.6/LICENSE.md` & `TrimMCStruct-0.0.5.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TrimMCStruct-0.0.5.6/PKG-INFO` & `TrimMCStruct-0.0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrimMCStruct
-Version: 0.0.5.6
+Version: 0.0.5.8
 Summary: 读写操作《我的世界》.MCSTRUCTURE文件
 Home-page: https://github.com/TriM-Organization/TrimMCStruct
 Author: Eilles Wan, bgArray, phoenixr-codes(original author) 
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `TrimMCStruct-0.0.5.6/README.md` & `TrimMCStruct-0.0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `TrimMCStruct-0.0.5.6/TrimMCStruct/main.py` & `TrimMCStruct-0.0.5.8/TrimMCStruct/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 from functools import partial
 from itertools import repeat
 import json
 from typing import Any, BinaryIO, Optional, Tuple, Union, Dict
 
 import numpy as np
 from numpy.typing import NDArray
-from pynbt import BaseTag, NBTFile, TAG_Compound, TAG_Int, TAG_List, TAG_String, TAG_Byte, TAG_Long, \
-    TAG_Short  # type: ignore
+from pynbt import BaseTag, NBTFile, TAG_Compound, TAG_Int, TAG_List, TAG_String, TAG_Byte, TAG_Long, TAG_Short  # type: ignore
 
 Coordinate = Tuple[int, int, int]
 
 # Compatibility versioning number for blocks in 1.19.
 COMPABILITY_VERSION: int = 17959425
 
 
@@ -73,14 +72,17 @@
             if not isinstance(value, BaseTag):
                 value = _into_tag(value)
             res.append(value)
         return TAG_List(
             tag_type=(type(_into_tag(obj[0])) if obj else TAG_String), value=res
         )
 
+    elif isinstance(obj, bool):
+        return TAG_Byte(obj)
+
     elif isinstance(obj, int):
         return TAG_Int(obj)
 
     elif isinstance(obj, str):
         return TAG_String(obj)
 
     return obj
@@ -127,64 +129,64 @@
 
     namespace: str
     base_name: str
     states: dict[str, Union[int, str, bool]]
     extra_data: dict[str, Union[int, str, bool]]
 
     def __init__(
-            self,
-            namespace: str,
-            base_name: str,
-            states: dict[str, Union[int, str, bool]] = {},
-            extra_data: dict[str, Union[int, str, bool]] = {},
-            compability_version: int = COMPABILITY_VERSION,
+        self,
+        namespace: str,
+        base_name: str,
+        states: dict[str, Union[int, str, bool]] = {},
+        extra_data: dict[str, Union[int, str, bool]] = {},
+        compability_version: int = COMPABILITY_VERSION,
     ):
         """
         Parameters
         ----------
-        namespace
+        namespace: str
             The namespace of the block (e.g. "minecraft").
-        base_name
+        base_name: str
             The name of the block (e.g. "air").
 
         states
             The block states such as {'color': 'white'} or {"stone_type":1}.
             This varies by every block.
 
         extra_data
             [Optional] The additional data of the block.
 
-        compability_version
+        compability_version: int
             [Optional] The compability version of the block, now(1.19) is 17959425
         """
         self.namespace = namespace
         self.base_name = base_name
         self.states = states
         self.extra_data = extra_data
         self.compability_version = compability_version
 
     @classmethod
     def from_identifier(
-            cls,
-            identifier: str,
-            compability_version=COMPABILITY_VERSION,
-            **states: Union[int, str, bool],
+        cls,
+        identifier: str,
+        compability_version: int = COMPABILITY_VERSION,
+        **states: Union[int, str, bool],
     ):
         """
         Parameters
         ----------
-        identifier
+        identifier: str
             The identifier of the block (e.g. "minecraft:wool").
 
-        states
+        compability_version: int
+            [Optional] The compability version of the block, now(1.19) is 17959425
+
+        states:
             The block states such as "color" or "stone_type".
             This varies by every block.
-
-        compability_version
-            It's not written here.
         """
 
         if ":" in identifier:
             namespace, base_name = identifier.split(":", 1)
         else:
             namespace = "minecraft"
             base_name = identifier
@@ -198,50 +200,50 @@
     def __str__(self) -> str:
         return self.stringify()
 
     def __dict__(self) -> dict:
         return self.dictionarify()
 
     def add_states(
-            self,
-            states: dict[str, Union[int, str, bool]],
+        self,
+        states: dict[str, Union[int, str, bool]],
     ) -> None:
         self.states.update(states)
 
     def add_extra_data(
-            self,
-            extra_data: dict[str, Union[int, str, bool]],
+        self,
+        extra_data: dict[str, Union[int, str, bool]],
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
-            self, *, with_states: bool = True
+        self, *, with_states: bool = True
     ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         result = {
             "name": self.identifier,
             "states": self.states if with_states else {},
             "version": self.compability_version,
         }
 
         return result, self.extra_data
 
     def stringify(
-            self,
-            *,
-            with_namespace: bool = True,
-            with_states: bool = True,
+        self,
+        *,
+        with_namespace: bool = True,
+        with_states: bool = True,
     ) -> str:
         result = ""
         if with_namespace:
             result += self.namespace + ":"
         result += self.get_name()
         if with_states:
             result += f" [{json.dumps(self.states)[1:-1]}]"
@@ -275,15 +277,14 @@
     def identifier(self) -> str:
         """
         The identifier of the block.
         """
         return self.get_identifier()
 
     def __eq__(self, obj: Block) -> bool:
-
         if isinstance(obj, Block):
             if self.dictionarify() == obj.dictionarify():
                 return True
 
         return False
 
     def copy(self) -> Block:
@@ -311,33 +312,35 @@
     _size
         The size of the structure.
     """
 
     structure_indecis: NDArray[np.intc]
 
     def __init__(
-            self,
-            size: tuple[int, int, int],
-            fill: Optional[Block] = None,
-            compability_version: int = COMPABILITY_VERSION,
+        self,
+        size: tuple[int, int, int],
+        fill: Optional[Block] = None,
+        compability_version: int = COMPABILITY_VERSION,
     ):
         """
         Parameters
         ----------
         size
             The size of the structure.
 
         fill
             Fill the structure with this block at
             creation of a new structure object.
 
+            However, extra datas of blocks cannot be filled.
+
             If this is set to ``None`` the structure
             is filled with "Structure Void" blocks.
 
-            "minecraft:air" is used as default.
+            "None" is used as default.
         """
 
         self.structure_indecis: NDArray[np.intc]
 
         self._size = size
         self._palette: list[Block] = []
         self._special_blocks: Dict[int, Dict] = {}
@@ -383,36 +386,33 @@
                     **_into_pyobj(block["states"].value),
                     compability_version=_into_pyobj(block["version"]),
                 )
                 for block in nbt["structure"]["palette"]["default"]["block_palette"]
             ]
         )
 
-        for block_index, block_eneity_data in nbt["structure"]["palette"]["default"][
+        for block_index, block_extra_data in nbt["structure"]["palette"]["default"][
             "block_position_data"
         ].items():
-            # struct._palette[int(block_index)].add_extra_data(
-            #     _into_pyobj(block_eneity_data)
-            # )
-            struct._special_blocks[int(block_index)] = _into_pyobj(block_eneity_data)
+            struct._special_blocks[int(block_index)] = _into_pyobj(block_extra_data)
 
         return struct
 
     @property
     def size(self) -> tuple[int, int, int]:
         return self._size
 
     def __repr__(self) -> str:
         return repr(self._get_str_array())
 
     def __str__(self) -> str:
         return str(self._get_str_array())
 
     def _get_str_array(
-            self, *, with_namespace: bool = False, with_states: bool = False
+        self, *, with_namespace: bool = False, with_states: bool = False
     ) -> NDArray[Any]:
         """
         Returns a numpy array where each entry is a
         readable string of the corresponding block.
 
         Parameters
         ----------
@@ -512,23 +512,24 @@
                                                     )
                                                 )
                                                 for block in self._palette
                                             ],
                                         ),
                                         block_position_data=TAG_Compound(
                                             dict(
-                                                [
-                                                    (
-                                                        str(block_index),
-                                                        _into_tag(
-                                                            extra_data
-                                                        ),
-                                                    )
-                                                    for block_index, extra_data in self._special_blocks.items()
-                                                ]
+                                                sorted(
+                                                    [
+                                                        (
+                                                            str(block_index),
+                                                            _into_tag(extra_data),
+                                                        )
+                                                        for block_index, extra_data in self._special_blocks.items()
+                                                    ],
+                                                    key=lambda a: a[0],
+                                                )
                                             )
                                         ),
                                     )
                                 )
                             )
                         ),
                     )
@@ -616,17 +617,17 @@
             ][
                 (index % (self.size[2] * self.size[1]) % self.size[2])
             ].extra_data = exdata
 
         return arr
 
     def set_block(
-            self,
-            coordinate: Coordinate,
-            block: Optional[Block],
+        self,
+        coordinate: Coordinate,
+        block: Optional[Block],
     ) -> Structure:
         """
         Puts a block into the structure.
 
         Parameters
         ----------
         coordinate
@@ -640,22 +641,22 @@
 
         ident = self._add_block_to_palette(block)
 
         self.structure_indecis[x, y, z] = ident
         if block.extra_data:
             self._special_blocks[
                 x * self.size[2] * self.size[1] + y * self.size[2] + z
-                ] = block.extra_data
+            ] = block.extra_data
         return self
 
     def fill_blocks(
-            self,
-            from_coordinate: Coordinate,
-            to_coordinate: Coordinate,
-            block: Block,
+        self,
+        from_coordinate: Coordinate,
+        to_coordinate: Coordinate,
+        block: Block,
     ) -> Structure:
         """
         Puts multiple blocks into the structure.
 
         Notes
         -----
         Both start and end points are filled.
@@ -674,15 +675,15 @@
         """
         fx, fy, fz = from_coordinate
         tx, ty, tz = to_coordinate
 
         ident = self._add_block_to_palette(block)
 
         # print([[[ident for k in range(abs(fz-tz)+1) ]for j in range(abs(fy-ty)+1)]for i in range(abs(fx-tx)+1)])
-        self.structure_indecis[fx: tx + 1, fy: ty + 1, fz: tz + 1] = np.array(
+        self.structure_indecis[fx : tx + 1, fy : ty + 1, fz : tz + 1] = np.array(
             [
                 [
                     [ident for k in range(abs(fz - tz) + 1)]
                     for j in range(abs(fy - ty) + 1)
                 ]
                 for i in range(abs(fx - tx) + 1)
             ],
@@ -698,16 +699,16 @@
                             for x in range(fx, tx)
                             for y in range(fy, ty)
                             for z in range(fz, tz)
                         ],
                         [
                             block.extra_data
                             for i in range(
-                            abs((fz - tz) + 1)
-                            * (abs(fy - ty) + 1)
-                            * (abs(fx - tx) + 1)
-                        )
+                                abs((fz - tz) + 1)
+                                * (abs(fy - ty) + 1)
+                                * (abs(fx - tx) + 1)
+                            )
                         ],
                     )
                 )
             )
         return self
```

### Comparing `TrimMCStruct-0.0.5.6/TrimMCStruct.egg-info/PKG-INFO` & `TrimMCStruct-0.0.5.8/TrimMCStruct.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrimMCStruct
-Version: 0.0.5.6
+Version: 0.0.5.8
 Summary: 读写操作《我的世界》.MCSTRUCTURE文件
 Home-page: https://github.com/TriM-Organization/TrimMCStruct
 Author: Eilles Wan, bgArray, phoenixr-codes(original author) 
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `TrimMCStruct-0.0.5.6/setup.py` & `TrimMCStruct-0.0.5.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 import TrimMCStruct
 
 with open("README.MD", "r", encoding="utf-8") as fh:
     long_description = fh.read().replace(
         "./docs/", "https://github.com/TriM-Organization/TrimMCStruct/blob/master/docs/"
     )
 
+with open("requirements.txt", "r", encoding="utf-8") as fh:
+    dependences = fh.read().strip().split("\n")
+
 setuptools.setup(
     name="TrimMCStruct",
     version=TrimMCStruct.__version__,
     author="Eilles Wan, bgArray, phoenixr-codes(original author) ",
     author_email="TriM-Organization@hotmail.com",
     description="读写操作《我的世界》.MCSTRUCTURE文件\n"
-    "Read and write Minecraft .mcstructure files.",
+                "Read and write Minecraft .mcstructure files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TriM-Organization/TrimMCStruct",
     packages=setuptools.find_packages(),
     classifiers=[
         "Intended Audience :: Developers",
         "Natural Language :: English",
@@ -27,9 +30,9 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     # 需要安装的依赖
-    install_requires=open("requirements.txt",'r',encoding='utf-8').read().strip().split("\n"),
+    install_requires=dependences,
 )
```


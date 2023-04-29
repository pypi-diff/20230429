# Comparing `tmp/jageocoder-2.0.0.tar.gz` & `tmp/jageocoder-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jageocoder-2.0.0.tar", max compression
+gzip compressed data, was "jageocoder-2.0.1.tar", max compression
```

## Comparing `jageocoder-2.0.0.tar` & `jageocoder-2.0.1.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0      113 2023-04-14 08:49:30.870739 jageocoder-2.0.0/LICENSE
--rw-r--r--   0        0        0     8253 2023-04-14 11:42:42.077451 jageocoder-2.0.0/README.md
--rw-r--r--   0        0        0     1405 2023-04-14 11:42:42.077451 jageocoder-2.0.0/jageocoder/__init__.py
--rw-r--r--   0        0        0     4028 2023-04-14 11:42:42.077451 jageocoder-2.0.0/jageocoder/__main__.py
--rw-r--r--   0        0        0     2574 2023-04-14 08:49:30.886739 jageocoder-2.0.0/jageocoder/address.py
--rw-r--r--   0        0        0    12147 2023-04-14 11:42:42.077451 jageocoder-2.0.0/jageocoder/aza_master.py
--rw-r--r--   0        0        0     1171 2023-04-14 11:42:42.077451 jageocoder-2.0.0/jageocoder/dataset.py
--rw-r--r--   0        0        0      691 2023-04-14 08:49:30.886739 jageocoder-2.0.0/jageocoder/exceptions.py
--rw-r--r--   0        0        0    18862 2023-04-14 11:42:42.077451 jageocoder-2.0.0/jageocoder/itaiji.py
--rw-r--r--   0        0        0    14220 2023-04-14 08:49:30.890739 jageocoder-2.0.0/jageocoder/itaiji_dic.json
--rw-r--r--   0        0        0    10983 2023-04-14 11:42:42.077451 jageocoder-2.0.0/jageocoder/module.py
--rw-r--r--   0        0        0    36822 2023-04-14 11:42:42.081451 jageocoder-2.0.0/jageocoder/node.py
--rw-r--r--   0        0        0     2631 2023-04-14 11:42:42.081451 jageocoder-2.0.0/jageocoder/result.py
--rw-r--r--   0        0        0     7854 2023-04-14 08:49:30.890739 jageocoder-2.0.0/jageocoder/strlib.py
--rw-r--r--   0        0        0    48184 2023-04-14 11:42:42.081451 jageocoder-2.0.0/jageocoder/tree.py
--rw-r--r--   0        0        0     4995 2023-04-14 11:42:42.081451 jageocoder-2.0.0/jageocoder/trie.py
--rw-r--r--   0        0        0     1150 2023-04-14 11:42:42.081451 jageocoder-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     9566 1970-01-01 00:00:00.000000 jageocoder-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      113 2023-04-28 00:22:42.161103 jageocoder-2.0.1/LICENSE
+-rw-r--r--   0        0        0     8253 2023-04-28 00:22:42.161103 jageocoder-2.0.1/README.md
+-rw-r--r--   0        0        0     1405 2023-04-29 00:02:26.756784 jageocoder-2.0.1/jageocoder/__init__.py
+-rw-r--r--   0        0        0     4541 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/__main__.py
+-rw-r--r--   0        0        0     2574 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/address.py
+-rw-r--r--   0        0        0     1421 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/aliases.json
+-rw-r--r--   0        0        0    12147 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/aza_master.py
+-rw-r--r--   0        0        0     1171 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/dataset.py
+-rw-r--r--   0        0        0      691 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/exceptions.py
+-rw-r--r--   0        0        0    18862 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/itaiji.py
+-rw-r--r--   0        0        0    14220 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/itaiji_dic.json
+-rw-r--r--   0        0        0    11293 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/module.py
+-rw-r--r--   0        0        0    37186 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/node.py
+-rw-r--r--   0        0        0     2631 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/result.py
+-rw-r--r--   0        0        0    15241 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/rtree.py
+-rw-r--r--   0        0        0     7854 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/strlib.py
+-rw-r--r--   0        0        0    48985 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/tree.py
+-rw-r--r--   0        0        0     4995 2023-04-28 00:22:42.171103 jageocoder-2.0.1/jageocoder/trie.py
+-rw-r--r--   0        0        0     1223 2023-04-29 00:02:40.686784 jageocoder-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     9747 1970-01-01 00:00:00.000000 jageocoder-2.0.1/setup.py
+-rw-r--r--   0        0        0     9684 1970-01-01 00:00:00.000000 jageocoder-2.0.1/PKG-INFO
```

### Comparing `jageocoder-2.0.0/README.md` & `jageocoder-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.0/jageocoder/__init__.py` & `jageocoder-2.0.1/jageocoder/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 running the following steps.
 
     >>> import jageocoder
     >>> jageocoder.init()
     >>> jageocoder.searchNode('<Japanese-address>')
 """
 
-__version__ = '2.0.0'  # The package version
+__version__ = '2.0.1'  # The package version
 __dictionary_version__ = '20230405'  # Compatible dictionary version
 __author__ = 'Takeshi Sagara <sagara@info-proto.com>'
 
 __all__ = [
     'init',
     'free',
     'is_initialized',
```

### Comparing `jageocoder-2.0.0/jageocoder/__main__.py` & `jageocoder-2.0.1/jageocoder/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,26 +9,28 @@
 HELP = """
 'jageocoder' is a Python package of Japanese-address geocoder.
 
 Usage:
   {p} -h
   {p} -v
   {p} search [-d] [--area=<area>] [--db-dir=<dir>] [--force-aza-skip|--disable-aza-skip] <address>
+  {p} reverse [-d] [--level=<level>] [--db-dir=<dir>] <longitude> <latitude>
   {p} get-db-dir [-d]
   {p} download-dictionary [-d] <url>
   {p} install-dictionary [-d] [--db-dir=<dir>] <path>
   {p} uninstall-dictionary [-d] [--db-dir=<dir>]
 
 Options:
   -h --help           Show this help.
   -v --version        Show version number.
   -d --debug          Show debug messages.
   --area=<area>       Specify the target area by jiscode or names.
   --force-aza-skip    Skip aza-names whenever possible.
   --disable-aza-skip  Do not skip aza-names.
+  --level=<level>     Max address level to search.
   --db-dir=<dir>      Specify dictionary directory.
 
 Examples:
 
 - Search address
 
   {p} search 多摩市落合1-15
@@ -107,14 +109,24 @@
                 ensure_ascii=False))
         except RuntimeError as e:
             print(
                 "An error occurred during the search: {}".format(e),
                 file=sys.stderr)
             exit(1)
 
+    elif args['reverse']:
+        from jageocoder.address import AddressLevel
+        jageocoder.init(db_dir=args['--db-dir'], mode='r')
+        print(json.dumps(
+            jageocoder.reverse(
+                x=float(args['<longitude>']),
+                y=float(args['<latitude>']),
+                level=int(args['--level'] or AddressLevel.AZA)),
+            ensure_ascii=False))
+
     elif args['download-dictionary']:
         url = args['<url>']
         try:
             jageocoder.download_dictionary(url=url)
         except JageocoderError:
             logging.warning((
                 'Could not find the dictionary at the URL.'
```

### Comparing `jageocoder-2.0.0/jageocoder/address.py` & `jageocoder-2.0.1/jageocoder/address.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.0/jageocoder/aza_master.py` & `jageocoder-2.0.1/jageocoder/aza_master.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.0/jageocoder/dataset.py` & `jageocoder-2.0.1/jageocoder/dataset.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.0/jageocoder/exceptions.py` & `jageocoder-2.0.1/jageocoder/exceptions.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.0/jageocoder/itaiji.py` & `jageocoder-2.0.1/jageocoder/itaiji.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.0/jageocoder/itaiji_dic.json` & `jageocoder-2.0.1/jageocoder/itaiji_dic.json`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.0/jageocoder/module.py` & `jageocoder-2.0.1/jageocoder/module.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import logging
 import os
 import shutil
 from typing import Optional, Union, List
 import urllib.request
 from urllib.error import URLError
 
@@ -273,19 +274,23 @@
     str
         The version string of the installed dicitionary.
     """
     if db_dir is None:
         db_dir = get_db_dir(mode='a')
 
     metadata_path = os.path.join(db_dir, "metadata.txt")
-    if not os.path.exists(metadata_path):
-        return "(no version information)"
+    if os.path.exists(metadata_path):
+        with open(metadata_path, "r") as f:
+            version = f.readline().rstrip()
 
-    with open(metadata_path, "r") as f:
-        version = f.readline().rstrip()
+    else:
+        readme_path = os.path.join(db_dir, "README.md")
+        stats = os.stat(readme_path)
+        version = datetime.date.fromtimestamp(stats.st_mtime).strftime(
+            '%Y%m%d')
 
     return version
 
 
 def installed_dictionary_readme(db_dir: Optional[os.PathLike] = None) -> str:
     """
     Get the content of README.txt attached to the installed dictionary.
@@ -300,15 +305,15 @@
     -------
     str
         The content of the text.
     """
     if db_dir is None:
         db_dir = get_db_dir(mode='a')
 
-    readme_path = os.path.join(db_dir, "README.txt")
+    readme_path = os.path.join(db_dir, "README.md")
     if not os.path.exists(readme_path):
         return "(no README information)"
 
     with open(readme_path, "r") as f:
         content = f.read()
 
     return content
@@ -383,18 +388,22 @@
     global _tree
     return _tree.searchNode(query)
 
 
 def reverse(x: float, y: float, level: Optional[int] = None) -> dict:
     """
     Reverse geocoding.
-
     """
-    raise JageocoderError(
-        "The 'reverse' method is not yet available in version 2.")
+    if not is_initialized():
+        raise JageocoderError("Not initialized. Call 'init()' first.")
+    from jageocoder.rtree import Index
+
+    global _tree
+    idx = Index(tree=_tree)
+    return idx.nearest(x=x, y=y, level=level)
 
 
 def create_trie_index() -> None:
     """
     Create the TRIE index from the database file.
 
     This function is a shortcut for AddressTree.create_trie_index().
```

### Comparing `jageocoder-2.0.0/jageocoder/node.py` & `jageocoder-2.0.1/jageocoder/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -797,25 +797,37 @@
                 "level": self.level,
                 "priority": self.priority,
                 "note": self.note,
                 "fullname": self.get_fullname(),
             }
         }
 
-    def get_fullname(self):
+    def get_fullname(
+        self,
+        delimiter: Optional[str] = None,
+    ):
         """
         Returns a complete address notation starting with the name of
         the prefecture.
+
+        Parameters
+        ----------
+        delimiter: str, optional
+            Specifies the delimiter character for the address element;
+            If None is specified, returns a list of elements.
         """
         names = []
         cur_node = self
         while cur_node is not None:
             names.insert(0, cur_node.name)
             cur_node = cur_node.get_parent()
 
+        if isinstance(delimiter, str):
+            return delimiter.join(names)
+
         return names
 
     def get_parent_list(self):
         """
         Returns a complete node list starting with the prefecture.
         """
         nodes = []
@@ -865,19 +877,19 @@
 
     def retrieve_upper_node(self, target_levels: List[int]):
         """
         Retrieves the node at the specified level from
         the this node or one of its upper nodes.
         """
         cur_node = self
-        while cur_node.id is not None and \
+        while cur_node is not None and \
                 cur_node.level not in target_levels:
             cur_node = cur_node.get_parent()
 
-        if cur_node.level in target_levels:
+        if cur_node is not None and cur_node.level in target_levels:
             return cur_node
 
         return None
 
     def get_pref_name(self) -> str:
         """
         Returns the name of prefecture that contains this node.
```

### Comparing `jageocoder-2.0.0/jageocoder/result.py` & `jageocoder-2.0.1/jageocoder/result.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.0/jageocoder/strlib.py` & `jageocoder-2.0.1/jageocoder/strlib.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.0/jageocoder/tree.py` & `jageocoder-2.0.1/jageocoder/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import OrderedDict
 import csv
+import json
 from logging import getLogger
 import os
 from pathlib import Path
 import re
 import site
 import sys
 from typing import Any, Union, List, NoReturn, Optional, TextIO
@@ -360,15 +361,15 @@
             - If False, do not skip
             - If True, always skip
 
         - require_coordinates: bool (default = True)
             If set to False, nodes without coordinates are also
             included in the search.
 
-        - target_areas: List[str] (Default = [])
+        - target_area: List[str] (Default = [])
             Specify the areas to be searched.
             The area can be specified by the list of name of the node
             (such as prefecture name or city name), or JIS code.
         """
         for k, v in kwargs.items():
             self._set_config(k, v)
 
@@ -392,15 +393,16 @@
                 return
 
             # Check if the value is a name of node in the database.
             std = self.converter.standardize(value)
             candidates = self.trie.common_prefixes(std)
             if std in candidates:
                 trie_node_id = candidates[std]
-                for node_id in self.trie_nodes.get_record(pos=trie_node_id).nodes:
+                for node_id in self.trie_nodes.get_record(
+                        pos=trie_node_id).nodes:
                     node = self.address_nodes.get_record(pos=node_id)
                     if node.name == value:
                         return
 
             msg = "'{}' is not a valid value for {}.".format(value, key)
             raise RuntimeError(msg)
 
@@ -935,32 +937,49 @@
                 pos = parent.sibling_id
                 continue
 
         logger.debug("  {} records found.".format(
             len(tmp_id_name_table)))
 
         # Extend index_table
+        with open(Path(__file__).parent / "aliases.json") as f:
+            aliases = json.load(f)
+
         for k, v in tmp_id_name_table.items():
             if v.parent_id == AddressNode.ROOT_NODE_ID:
                 continue
 
+            alternatives = []
             parent_node = tmp_id_name_table[v.parent_id]
             if parent_node.level == AddressLevel.PREF:
-                continue
-
-            pref_node = tmp_id_name_table[parent_node.parent_id]
-
-            logger.debug("Extend index by adding '{}/{}'".format(
-                pref_node.name, v.name))
-            label = pref_node.name + v.name
-            label_standardized = self.converter.standardize(label)
-            if label_standardized in self.index_table:
-                self.index_table[label_standardized].append(v.id)
+                parents = [parent_node.name]
             else:
-                self.index_table[label_standardized] = [v.id]
+                pref_node = tmp_id_name_table[parent_node.parent_id]
+                parents = [pref_node.name, parent_node.name]
+
+            if v.name in aliases:
+                for candidate in aliases[v.name]:
+                    for i in range(len(parents) + 1):
+                        alternatives.append(parents[i:] + [candidate])
+
+            if len(parents) > 1:
+                alternatives.append([parents[0], v.name])
+                if v.name in aliases:
+                    for candidate in aliases[v.name]:
+                        alternatives.append([parents[0], candidate])
+
+            for alternative in alternatives:
+                logger.debug("Extend index by adding '{}'".format(
+                    '/'.join(alternative)))
+                label = "".join(alternative)
+                label_standardized = self.converter.standardize(label)
+                if label_standardized in self.index_table:
+                    self.index_table[label_standardized].append(v.id)
+                else:
+                    self.index_table[label_standardized] = [v.id]
 
     def _set_index_table(self) -> list:
         """
         Map all the id of the TRIE index (TRIE id) to the node id.
 
         Collect notations recursively the names of all address elements
         which was registered in the TRIE index, retrieve
```

### Comparing `jageocoder-2.0.0/jageocoder/trie.py` & `jageocoder-2.0.1/jageocoder/trie.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.0/pyproject.toml` & `jageocoder-2.0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jageocoder"
-version = "2.0.0"
+version = "2.0.1"
 description = "A Japanese-address geocoder for Python."
 authors = ["Takeshi Sagara <sagara@info-proto.com>"]
 repository = "https://github.com/t-sagara/jageocoder/"
 license = "The MIT License"
 readme = "README.md"
 documentation = "https://jageocoder.readthedocs.io/"
 packages = [
@@ -13,25 +13,28 @@
 classifiers = [
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows :: Windows 11",
     "Operating System :: POSIX :: Linux",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
-include = ["itaiji_dic.json"]
+include = ["itaiji_dic.json", "islands.json"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 marisa-trie = "^0.7.8"
 jaconv = "^0.3.4"
 docopt = "^0.6.2"
 deprecated = "^1.2.13"
 Werkzeug = ">=2.2.3"
 pycapnp = "^1.3.0"
 portabletab = "0.3.1"
+tqdm = "^4.00.0"
+rtree = "^1.0.0"
+geographiclib = "^2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 flake8 = "^5.0.0"
 twine = "^4.0.2"
 flask = "^2.2.3"
 flask-cors = "^3.0.10"
```

### Comparing `jageocoder-2.0.0/PKG-INFO` & `jageocoder-2.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jageocoder
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Japanese-address geocoder for Python.
 Home-page: https://github.com/t-sagara/jageocoder/
 License: The MIT License
 Author: Takeshi Sagara
 Author-email: sagara@info-proto.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -18,18 +18,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: Werkzeug (>=2.2.3)
 Requires-Dist: deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
+Requires-Dist: geographiclib (>=2.0,<3.0)
 Requires-Dist: jaconv (>=0.3.4,<0.4.0)
 Requires-Dist: marisa-trie (>=0.7.8,<0.8.0)
 Requires-Dist: portabletab (==0.3.1)
 Requires-Dist: pycapnp (>=1.3.0,<2.0.0)
+Requires-Dist: rtree (>=1.0.0,<2.0.0)
+Requires-Dist: tqdm (>=4.00.0,<5.0.0)
 Project-URL: Documentation, https://jageocoder.readthedocs.io/
 Project-URL: Repository, https://github.com/t-sagara/jageocoder/
 Description-Content-Type: text/markdown
 
 # jageocoder - A Python Japanese geocoder
 
 日本語版は README_ja.md をお読みください。
```


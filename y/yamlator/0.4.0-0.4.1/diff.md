# Comparing `tmp/yamlator-0.4.0.tar.gz` & `tmp/yamlator-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamlator-0.4.0.tar", last modified: Thu Mar 30 19:07:57 2023, max compression
+gzip compressed data, was "yamlator-0.4.1.tar", last modified: Sat Apr 29 15:55:42 2023, max compression
```

## Comparing `yamlator-0.4.0.tar` & `yamlator-0.4.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:07:57.874271 yamlator-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-30 19:07:54.000000 yamlator-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-03-30 19:07:57.874271 yamlator-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-03-30 19:07:54.000000 yamlator-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-30 19:07:57.874271 yamlator-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-03-30 19:07:54.000000 yamlator-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:07:57.866271 yamlator-0.4.0/yamlator/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:07:57.866271 yamlator-0.4.0/yamlator/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/cmd/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:07:57.870271 yamlator-0.4.0/yamlator/cmd/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/cmd/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/cmd/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/cmd/outputs/json_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/cmd/outputs/table_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/cmd/outputs/yaml_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:07:57.870271 yamlator-0.4.0/yamlator/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/grammar/grammar.lark
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:07:57.870271 yamlator-0.4.0/yamlator/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14629 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/parser/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/parser/dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/parser/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:07:57.874271 yamlator-0.4.0/yamlator/validators/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/validators/any_type_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/validators/base_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/validators/builtin_type_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/validators/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/validators/entry_point_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/validators/enum_type_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/validators/list_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/validators/map_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/validators/optional_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/validators/required_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/validators/ruleset_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/validators/union_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-03-30 19:07:54.000000 yamlator-0.4.0/yamlator/violations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:07:57.866271 yamlator-0.4.0/yamlator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-03-30 19:07:57.000000 yamlator-0.4.0/yamlator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-03-30 19:07:57.000000 yamlator-0.4.0/yamlator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 19:07:57.000000 yamlator-0.4.0/yamlator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-30 19:07:57.000000 yamlator-0.4.0/yamlator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-30 19:07:57.000000 yamlator-0.4.0/yamlator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-30 19:07:57.000000 yamlator-0.4.0/yamlator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:55:42.510588 yamlator-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-29 15:55:37.000000 yamlator-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-29 15:55:42.510588 yamlator-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-29 15:55:37.000000 yamlator-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-29 15:55:42.510588 yamlator-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-29 15:55:37.000000 yamlator-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:55:42.502587 yamlator-0.4.1/yamlator/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:55:42.502587 yamlator-0.4.1/yamlator/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/cmd/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:55:42.506588 yamlator-0.4.1/yamlator/cmd/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/cmd/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/cmd/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/cmd/outputs/json_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/cmd/outputs/table_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/cmd/outputs/yaml_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:55:42.506588 yamlator-0.4.1/yamlator/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/grammar/grammar.lark
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:55:42.506588 yamlator-0.4.1/yamlator/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14673 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/parser/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/parser/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14704 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/parser/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:55:42.510588 yamlator-0.4.1/yamlator/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/validators/any_type_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/validators/base_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/validators/builtin_type_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/validators/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/validators/entry_point_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/validators/enum_type_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/validators/list_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/validators/map_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/validators/optional_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/validators/required_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/validators/ruleset_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/validators/union_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-04-29 15:55:37.000000 yamlator-0.4.1/yamlator/violations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:55:42.502587 yamlator-0.4.1/yamlator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-29 15:55:42.000000 yamlator-0.4.1/yamlator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-29 15:55:42.000000 yamlator-0.4.1/yamlator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:55:42.000000 yamlator-0.4.1/yamlator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-29 15:55:42.000000 yamlator-0.4.1/yamlator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-29 15:55:42.000000 yamlator-0.4.1/yamlator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-29 15:55:42.000000 yamlator-0.4.1/yamlator.egg-info/top_level.txt
```

### Comparing `yamlator-0.4.0/LICENSE` & `yamlator-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/PKG-INFO` & `yamlator-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlator
-Version: 0.4.0
+Version: 0.4.1
 Summary: Yamlator is a CLI tool that allows a YAML file to be validated using a lightweight schema language
 Home-page: https://github.com/ryan95f/yamlator
 Author: Ryan Flynn
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yamlator-0.4.0/README.md` & `yamlator-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/setup.py` & `yamlator-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 import setuptools
 
-VERSION = '0.4.0'
+VERSION = '0.4.1'
 PACKAGE_NAME = 'yamlator'
 DESCRIPTION = 'Yamlator is a CLI tool that allows a YAML file to be validated using a lightweight schema language'  # nopep8
 
 
 def create_long_description():
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
```

### Comparing `yamlator-0.4.0/yamlator/cmd/core.py` & `yamlator-0.4.1/yamlator/cmd/core.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/cmd/outputs/base.py` & `yamlator-0.4.1/yamlator/cmd/outputs/base.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/cmd/outputs/json_output.py` & `yamlator-0.4.1/yamlator/cmd/outputs/json_output.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/cmd/outputs/table_output.py` & `yamlator-0.4.1/yamlator/cmd/outputs/table_output.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/cmd/outputs/yaml_output.py` & `yamlator-0.4.1/yamlator/cmd/outputs/yaml_output.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/exceptions.py` & `yamlator-0.4.1/yamlator/exceptions.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/grammar/grammar.lark` & `yamlator-0.4.1/yamlator/grammar/grammar.lark`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 
 import_statement: "import" imported_types "from" IMPORT_STATEMENT_PATH ("as" NAMESPACE)?
 imported_types: (CONTAINER_TYPE_NAME ("," CONTAINER_TYPE_NAME)*)
 
 schema_entry: STRICT_KEYWORD? "schema" "{" rule+ "}"
-ruleset: STRICT_KEYWORD? "ruleset" CONTAINER_TYPE_NAME "{" rule+ "}"
+ruleset: STRICT_KEYWORD? "ruleset" CONTAINER_TYPE_NAME (ruleset_parent)? "{" rule+ "}"
 ruleset_parent: "(" container_type ")"
 
 // Enum constructs
 enum: "enum" CONTAINER_TYPE_NAME "{" enum_item+ "}"
 enum_item: ENUM_ITEM_NAME "=" values
 
 // Rule definitions
```

### Comparing `yamlator-0.4.0/yamlator/parser/__init__.py` & `yamlator-0.4.1/yamlator/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/parser/core.py` & `yamlator-0.4.1/yamlator/parser/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,14 +206,16 @@
         Raises:
             yamlator.exceptions.ConstructNotFoundError: Raised if the
                 enum or ruleset cannot be found
         """
         name = tokens[0]
         if len(tokens) > 1:
             name = f'{tokens[0]}.{tokens[1]}'
+        else:
+            name = name.value
 
         schema_type = self.seen_constructs.get(name, SchemaTypes.UNKNOWN)
         rule_type = RuleType(schema_type=schema_type, lookup=name)
         if schema_type == SchemaTypes.UNKNOWN:
             self.unknown_types.append(rule_type)
         return rule_type
```

### Comparing `yamlator-0.4.0/yamlator/parser/dependency.py` & `yamlator-0.4.1/yamlator/parser/dependency.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 """Utilties for managing dependencies in Yamlator"""
 
+import copy
 import hashlib
 from collections import defaultdict
 
 
 class DependencyManager:
     """Tracks and detects dependencies between objects by representing
     data as a Md5 hash. Once a node has been added, a depth first search
     is executed against all nodes to detect a cycle
     """
 
     def __init__(self) -> None:
-        self._graph = defaultdict(list)
+        self._graph = {}
+
+    @property
+    def graph(self) -> dict:
+        return copy.deepcopy(self._graph)
 
     def add(self, node: str) -> str:
         """Add a new node to the graph. The contents of the parameter
         `node` will be hashed with Md5
 
         Args:
             node (str): A string that contains the content or represents
@@ -36,39 +41,43 @@
         Args:
             parent_hash (str): The Md5 hash of the parent node
             child_hash (str): The Md5 hash of the child node
 
         Returns:
             True to indicate that the function completed successfully
         """
+        if not self._graph.get(parent_hash):
+            self._graph[parent_hash] = []
+
         self._graph[parent_hash].append(child_hash)
         return True
 
     def has_cycle(self) -> bool:
         """Detects a cycle against the contents the manager is representing
 
         Returns:
             A boolean to indicate if a cycle is present. True indicates
             a cycle was detected, False indicates no cycle is present
         """
         visited = defaultdict(bool)
         rec_stack = defaultdict(bool)
 
-        for node in self._graph.keys():
+        for node in self._graph:
             if not visited[node]:
                 if self._detect_cycle(node, visited, rec_stack):
                     return True
         return False
 
     def _detect_cycle(self, curr_node: str, visited: dict,
                       rec_stack: dict) -> bool:
         visited[curr_node] = True
         rec_stack[curr_node] = True
 
-        for child_node in self._graph[curr_node]:
+        parent_node = self._graph.get(curr_node, [])
+        for child_node in parent_node:
             if not visited[child_node]:
                 if self._detect_cycle(child_node, visited, rec_stack):
                     return True
             elif rec_stack[child_node]:
                 return True
 
         rec_stack[curr_node] = False
```

### Comparing `yamlator-0.4.0/yamlator/parser/loaders.py` & `yamlator-0.4.1/yamlator/parser/loaders.py`

 * *Files 14% similar despite different names*

```diff
@@ -329,47 +329,84 @@
     Returns:
         A dictionary where all the rulesets parent dependencies have been
         resolved by merging the parent rules in the child rules
 
     Raises:
         ValueError: If the ruleset parameter is `None`
         TypeError: If the ruleset parameter is not a `dict`
-        yamlator.exceptions.ConstructNotFoundError: If the parent of the ruleset
-            cannot be found in the `rulesets` parameter
+        yamlator.exceptions.ConstructNotFoundError: If a parent ruleset
+            that is being inherited cannot be found in the `rulesets` parameter
+        yamlator.exceptions.CycleDependencyError: If there is a cycle in the
+            inheritance chain
     """
     if rulesets is None:
         raise ValueError('Parameter rulesets cannot be None')
 
     if not isinstance(rulesets, dict):
         raise TypeError(
             'Parameter rulesets cannot be None should be a dictionary')
 
     updated_rulesets = {}
 
+    dependencies_mgmr = DependencyManager()
     for key, ruleset in rulesets.items():
-        if ruleset.parent is None:
+        parent = ruleset.parent
+        if not parent:
             updated_rulesets[key] = ruleset
             continue
 
-        parent_name = ruleset.parent.lookup
-        parent = rulesets.get(parent_name)
-        if parent is None:
+        if rulesets.get(parent.lookup) is None:
             raise ConstructNotFoundError(parent)
 
-        base_rules = ruleset.rules.copy()
-        parent_rules = parent.rules.copy()
+        dependencies_mgmr.add_child(key, ruleset.parent.lookup)
+
+    if dependencies_mgmr.has_cycle():
+        msg = 'Detected cycle when resolving inheritance chain'
+        raise CycleDependencyError(msg)
+
+    dependencies = dependencies_mgmr.graph
+    for node in dependencies:
+        if updated_rulesets.get(node) is not None:
+            continue
+
+        stack = [(node, None)]
+        while len(stack) > 0:
+            curr_node, curr_ruleset = stack.pop()
+
+            if curr_ruleset is not None:
+                parent_node, _ = stack.pop()
+                parent_ruleset = rulesets[parent_node]
+                updated_rulesets[parent_node] = _merge_rulesets(parent_ruleset,
+                                                                curr_ruleset)
+                if len(stack) > 1:
+                    stack.append((parent_node, updated_rulesets[parent_node]))
+                continue
+
+            if updated_rulesets.get(curr_node) is not None:
+                stack.append((curr_node, updated_rulesets[curr_node]))
+                continue
+
+            stack.append((curr_node, None))
+            stack.append((dependencies[curr_node][0], None))
 
-        # Index the rules in the base and parent rulesets to make it
-        # easier to merge the different rules together
-        base_rules_index = {rule.name: rule for rule in base_rules}
-        parent_rules_index = {rule.name: rule for rule in parent_rules}
-
-        # Merged the 2 rule lists together. If a rule name is present
-        # in both the base rules will be prioritised since it assumed
-        # it is being overridden
-        merged_rules = list({**parent_rules_index, **base_rules_index}.values())
-        updated_rulesets[key] = YamlatorRuleset(
-            name=ruleset.name,
-            rules=merged_rules,
-            is_strict=ruleset.is_strict
-        )
     return updated_rulesets
+
+
+def _merge_rulesets(ruleset: YamlatorRuleset,
+                    dependent_ruleset: YamlatorRuleset) -> YamlatorRuleset:
+    base_rules = ruleset.rules.copy()
+    dependent_rules = dependent_ruleset.rules.copy()
+
+    # Index the rules in the base and dependent rulesets to make it
+    # easier to merge the different rules together
+    base_rules_index = {rule.name: rule for rule in base_rules}
+    dependent_rules_index = {rule.name: rule for rule in dependent_rules}
+
+    # Merged the 2 rule lists together. If a rule name is present
+    # in both then the base rules will be prioritized since it assumed
+    # it is being overridden
+    merged_rules = list({**dependent_rules_index, **base_rules_index}.values())
+    return YamlatorRuleset(
+        name=ruleset.name,
+        rules=merged_rules,
+        is_strict=ruleset.is_strict
+    )
```

### Comparing `yamlator-0.4.0/yamlator/types.py` & `yamlator-0.4.1/yamlator/types.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/utils.py` & `yamlator-0.4.1/yamlator/utils.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/validators/__init__.py` & `yamlator-0.4.1/yamlator/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/validators/any_type_validator.py` & `yamlator-0.4.1/yamlator/validators/any_type_validator.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/validators/base_validator.py` & `yamlator-0.4.1/yamlator/validators/base_validator.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/validators/builtin_type_validator.py` & `yamlator-0.4.1/yamlator/validators/builtin_type_validator.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/validators/core.py` & `yamlator-0.4.1/yamlator/validators/core.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/validators/entry_point_validator.py` & `yamlator-0.4.1/yamlator/validators/entry_point_validator.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/validators/enum_type_validator.py` & `yamlator-0.4.1/yamlator/validators/enum_type_validator.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/validators/list_validator.py` & `yamlator-0.4.1/yamlator/validators/list_validator.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/validators/map_validator.py` & `yamlator-0.4.1/yamlator/validators/map_validator.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/validators/optional_validator.py` & `yamlator-0.4.1/yamlator/validators/optional_validator.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/validators/regex_validator.py` & `yamlator-0.4.1/yamlator/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/validators/required_validator.py` & `yamlator-0.4.1/yamlator/validators/required_validator.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/validators/ruleset_validator.py` & `yamlator-0.4.1/yamlator/validators/ruleset_validator.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/validators/union_validator.py` & `yamlator-0.4.1/yamlator/validators/union_validator.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator/violations.py` & `yamlator-0.4.1/yamlator/violations.py`

 * *Files identical despite different names*

### Comparing `yamlator-0.4.0/yamlator.egg-info/PKG-INFO` & `yamlator-0.4.1/yamlator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlator
-Version: 0.4.0
+Version: 0.4.1
 Summary: Yamlator is a CLI tool that allows a YAML file to be validated using a lightweight schema language
 Home-page: https://github.com/ryan95f/yamlator
 Author: Ryan Flynn
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yamlator-0.4.0/yamlator.egg-info/SOURCES.txt` & `yamlator-0.4.1/yamlator.egg-info/SOURCES.txt`

 * *Files identical despite different names*


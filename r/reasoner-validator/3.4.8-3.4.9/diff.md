# Comparing `tmp/reasoner_validator-3.4.8.tar.gz` & `tmp/reasoner_validator-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.4.8.tar", max compression
+gzip compressed data, was "reasoner_validator-3.4.9.tar", max compression
```

## Comparing `reasoner_validator-3.4.8.tar` & `reasoner_validator-3.4.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1153 2023-03-15 20:45:25.940245 reasoner_validator-3.4.8/LICENSE
--rw-r--r--   0        0        0    10735 2023-03-15 20:45:25.940245 reasoner_validator-3.4.8/README.md
--rw-r--r--   0        0        0      131 2023-03-15 20:45:25.940245 reasoner_validator-3.4.8/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-03-15 20:45:25.940245 reasoner_validator-3.4.8/docs/Makefile
--rw-r--r--   0        0        0     2288 2023-03-15 20:45:25.940245 reasoner_validator-3.4.8/docs/conf.py
--rw-r--r--   0        0        0    12701 2023-03-15 20:45:25.940245 reasoner_validator-3.4.8/docs/index.rst
--rw-r--r--   0        0        0      795 2023-03-15 20:45:25.940245 reasoner_validator-3.4.8/docs/make.bat
--rw-r--r--   0        0        0      136 2023-03-15 20:45:25.940245 reasoner_validator-3.4.8/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-03-15 20:45:25.940245 reasoner_validator-3.4.8/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-03-15 20:45:25.940245 reasoner_validator-3.4.8/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-03-15 20:45:25.940245 reasoner_validator-3.4.8/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-03-15 20:45:25.940245 reasoner_validator-3.4.8/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-03-15 20:45:25.940245 reasoner_validator-3.4.8/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-03-15 20:45:25.940245 reasoner_validator-3.4.8/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    29934 2023-03-15 20:45:25.940245 reasoner_validator-3.4.8/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     1788 2023-03-15 20:45:25.944245 reasoner_validator-3.4.8/pyproject.toml
--rw-r--r--   0        0        0    18017 2023-03-15 20:45:25.944245 reasoner_validator-3.4.8/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    41321 2023-03-15 20:45:25.944245 reasoner_validator-3.4.8/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    29714 2023-03-15 20:45:25.944245 reasoner_validator-3.4.8/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0    19593 2023-03-15 20:45:25.944245 reasoner_validator-3.4.8/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-03-15 20:45:25.944245 reasoner_validator-3.4.8/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4032 2023-03-15 20:45:25.944245 reasoner_validator-3.4.8/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0     5845 2023-03-15 20:45:25.944245 reasoner_validator-3.4.8/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-03-15 20:45:25.944245 reasoner_validator-3.4.8/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    12518 2023-03-15 20:45:25.944245 reasoner_validator-3.4.8/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0     5115 2023-03-15 20:45:25.944245 reasoner_validator-3.4.8/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      517 2023-03-15 20:45:25.944245 reasoner_validator-3.4.8/tests/README.md
--rw-r--r--   0        0        0        0 2023-03-15 20:45:25.944245 reasoner_validator-3.4.8/tests/__init__.py
--rw-r--r--   0        0        0    86023 2023-03-15 20:45:25.948245 reasoner_validator-3.4.8/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    27505 2023-03-15 20:45:25.948245 reasoner_validator-3.4.8/tests/test_response_validator.py
--rw-r--r--   0        0        0     2722 2023-03-15 20:45:25.948245 reasoner_validator-3.4.8/tests/test_semver.py
--rw-r--r--   0        0        0     8795 2023-03-15 20:45:25.948245 reasoner_validator-3.4.8/tests/test_validate.py
--rw-r--r--   0        0        0    17440 2023-03-15 20:45:25.948245 reasoner_validator-3.4.8/tests/test_validation_report.py
--rw-r--r--   0        0        0    12606 1970-01-01 00:00:00.000000 reasoner_validator-3.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/LICENSE
+-rw-r--r--   0        0        0    10735 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/README.md
+-rw-r--r--   0        0        0      131 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/Makefile
+-rw-r--r--   0        0        0     2288 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/conf.py
+-rw-r--r--   0        0        0    12701 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    30645 2023-03-16 02:12:38.054536 reasoner_validator-3.4.9/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     1788 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/pyproject.toml
+-rw-r--r--   0        0        0    18017 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    41636 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    30438 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0    19593 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4032 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0     5845 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    12518 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0     5115 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      517 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/tests/README.md
+-rw-r--r--   0        0        0        0 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/tests/__init__.py
+-rw-r--r--   0        0        0    86089 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    27505 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/tests/test_response_validator.py
+-rw-r--r--   0        0        0     2722 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/tests/test_semver.py
+-rw-r--r--   0        0        0     8795 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/tests/test_validate.py
+-rw-r--r--   0        0        0    17440 2023-03-16 02:12:38.058536 reasoner_validator-3.4.9/tests/test_validation_report.py
+-rw-r--r--   0        0        0    12606 1970-01-01 00:00:00.000000 reasoner_validator-3.4.9/PKG-INFO
```

### Comparing `reasoner_validator-3.4.8/LICENSE` & `reasoner_validator-3.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.8/README.md` & `reasoner_validator-3.4.9/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.8/docs/Makefile` & `reasoner_validator-3.4.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.8/docs/conf.py` & `reasoner_validator-3.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.8/docs/index.rst` & `reasoner_validator-3.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.8/docs/make.bat` & `reasoner_validator-3.4.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.8/docs/validation_codes_dictionary.md` & `reasoner_validator-3.4.9/docs/validation_codes_dictionary.md`

 * *Files 2% similar despite different names*

```diff
@@ -506,19 +506,25 @@
 
 ### error.query_graph.edge.qualifier_constraints.qualifier_set.empty
 
 **Message:** Edge '{identifier}' qualifier_set property value is empty!
 
 **Description:** Value of a 'qualifier_constraints.qualifier_set' property in a Query Graph must not be non-empty array!
 
-### error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.invalid
+### error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.type_id.unknown
 
-**Message:** Edge '{identifier}' qualifier entry is invalid!
+**Message:** Edge '{identifier}' qualifier type_id '{qualifier_type_id}' is unknown!
 
-**Description:** A 'qualifier' entry must be a valid JSON object with valid 'qualifier_type_id' and corresponding 'qualifier_value'!
+**Description:** A qualifier qualifier_type_id must be defined in the specified version of Biolink!
+
+### error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.value.unresolved
+
+**Message:** Edge '{identifier}' qualifier_value '{qualifier_value}' for '{qualifier_type_id}' cannot be resolved!
+
+**Description:** A 'qualifier_value' for the specified 'qualifier_type_id' of a qualifier likely could not be resolved without knowledge of the edge category!
 
 ### error.knowledge_graph.nodes.empty
 
 **Message:** No nodes found!
 
 **Description:** Knowledge graph in TRAPI messages must have a 'nodes' key and non-empty associated value!
 
@@ -746,13 +752,19 @@
 
 ### error.knowledge_graph.edge.qualifiers.empty
 
 **Message:** Edge '{identifier}' qualifiers property value is empty!
 
 **Description:** Value of a 'qualifiers' property in a Knowledge Graph must not be non-empty array!
 
-### error.knowledge_graph.edge.qualifiers.qualifier.invalid
+### error.knowledge_graph.edge.qualifiers.qualifier.type_id.unknown
+
+**Message:** Edge '{identifier}' qualifier type_id '{qualifier_type_id}' is unknown!
+
+**Description:** A qualifier qualifier_type_id must be defined in the specified version of Biolink!
+
+### error.knowledge_graph.edge.qualifiers.qualifier.value.unresolved
 
-**Message:** Edge '{identifier}' qualifier entry is invalid!
+**Message:** Edge '{identifier}' qualifier_value '{qualifier_value}' for '{qualifier_type_id}' cannot be resolved!
 
-**Description:** A 'qualifier' entry must be a valid JSON object with valid 'qualifier_type_id' and corresponding 'qualifier_value'!
+**Description:** A 'qualifier_value' for the specified 'qualifier_type_id' of a qualifier likely could not be resolved without knowledge of the edge category!
```

### Comparing `reasoner_validator-3.4.8/pyproject.toml` & `reasoner_validator-3.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.4.8"
+version = "3.4.9"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-3.4.8/reasoner_validator/__init__.py` & `reasoner_validator-3.4.9/reasoner_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.8/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.4.9/reasoner_validator/biolink/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -462,21 +462,27 @@
             attribute_constraints: List = edge['attribute_constraints']
 
     def validate_qualifier_entry(self, context: str, edge_id: str, qualifiers: List[Dict[str, str]]):
         for qualifier in qualifiers:
             qualifier_type_id: str = qualifier['qualifier_type_id']
             qualifier_value: str = qualifier['qualifier_value']
             try:
-                if not self.bmt.validate_qualifier(
+                if not self.bmt.is_qualifier(name=qualifier_type_id):
+                    self.report(
+                        code=f"error.{context}.qualifier.type_id.unknown",
+                        identifier=edge_id,
+                        qualifier_type_id=qualifier_type_id
+                    )
+                elif not self.bmt.validate_qualifier(
                         # TODO: temporary workaround, parse 'qualifier_type_id' to core name
                         qualifier_type_id=parse_name(qualifier_type_id),
                         qualifier_value=qualifier_value
                 ):
                     self.report(
-                        code=f"error.{context}.qualifier.invalid",
+                        code=f"error.{context}.qualifier.value.unresolved",
                         identifier=edge_id,
                         qualifier_type_id=qualifier_type_id,
                         qualifier_value=qualifier_value
                     )
 
             except Exception as e:
                 # broad spectrum exception to trap anticipated short term issues with BMT validation
```

### Comparing `reasoner_validator-3.4.8/reasoner_validator/codes.yaml` & `reasoner_validator-3.4.9/reasoner_validator/codes.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -330,17 +330,22 @@
           $description: "Value of 'attribute_constraints' slot value in a Query Graph must be an array data type!"
       qualifier_constraints:
         qualifier_set:
           empty:
               $message: "Edge '{identifier}' qualifier_set property value is empty!"
               $description: "Value of a 'qualifier_constraints.qualifier_set' property in a Query Graph must not be non-empty array!"
           qualifier:
-            invalid:
-              $message: "Edge '{identifier}' qualifier entry is invalid!"
-              $description: "A 'qualifier' entry must be a valid JSON object with valid 'qualifier_type_id' and corresponding 'qualifier_value'!"
+            type_id:
+              unknown:
+                $message: "Edge '{identifier}' qualifier type_id '{qualifier_type_id}' is unknown!"
+                $description: "A qualifier qualifier_type_id must be defined in the specified version of Biolink!"
+            value:
+              unresolved:
+                $message: "Edge '{identifier}' qualifier_value '{qualifier_value}' for '{qualifier_type_id}' cannot be resolved!"
+                $description: "A 'qualifier_value' for the specified 'qualifier_type_id' of a qualifier likely could not be resolved without knowledge of the edge category!"
   knowledge_graph:
     nodes:
       empty:
         $message: "No nodes found!"
         $description: "Knowledge graph in TRAPI messages must have a 'nodes' key and non-empty associated value!"
     edges:
       empty:
@@ -470,10 +475,15 @@
         not_array:
           $message: "Edge '{identifier}' 'qualifiers' are not an array!"
           $description: "Value of the 'qualifiers' slot in Knowledge Graph edge must be an array of attributes!"
         empty:
           $message: "Edge '{identifier}' qualifiers property value is empty!"
           $description: "Value of a 'qualifiers' property in a Knowledge Graph must not be non-empty array!"
         qualifier:
-          invalid:
-            $message: "Edge '{identifier}' qualifier entry is invalid!"
-            $description: "A 'qualifier' entry must be a valid JSON object with valid 'qualifier_type_id' and corresponding 'qualifier_value'!"
+          type_id:
+            unknown:
+              $message: "Edge '{identifier}' qualifier type_id '{qualifier_type_id}' is unknown!"
+              $description: "A qualifier qualifier_type_id must be defined in the specified version of Biolink!"
+          value:
+            unresolved:
+              $message: "Edge '{identifier}' qualifier_value '{qualifier_value}' for '{qualifier_type_id}' cannot be resolved!"
+              $description: "A 'qualifier_value' for the specified 'qualifier_type_id' of a qualifier likely could not be resolved without knowledge of the edge category!"
```

### Comparing `reasoner_validator-3.4.8/reasoner_validator/report.py` & `reasoner_validator-3.4.9/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.8/reasoner_validator/sri/util.py` & `reasoner_validator-3.4.9/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.8/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.4.9/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.8/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.4.9/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.8/reasoner_validator/validation_codes.py` & `reasoner_validator-3.4.9/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.8/reasoner_validator/versioning.py` & `reasoner_validator-3.4.9/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.8/tests/README.md` & `reasoner_validator-3.4.9/tests/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.8/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.4.9/tests/test_biolink_compliance_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1198,30 +1198,30 @@
                                 'qualifier_type_id': "not-a-curie",
                                 'qualifier_value': "fake-qualifier-value"
                             }
                         ]
                     }
                 ]
             },
-            "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.invalid"
+            "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.type_id.unknown"
         ),
         (  # Query 13 - 'qualifier_type_id' property value is unknown
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
                             {
                                 'qualifier_type_id': "biolink:unknown_qualifier",
                                 'qualifier_value': "fake-qualifier-value"
                             }
                         ]
                     }
                 ]
             },
-            "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.invalid"
+            "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.type_id.unknown"
         ),
         (  # Query 14 - 'qualifier_type_id' property value is valid but abstract
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
                             {
@@ -1229,30 +1229,30 @@
                                 'qualifier_value': "stability"
                             }
                         ]
                     }
                 ]
             },
             # "info.query_graph.edge.qualifier.abstract"
-            "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.invalid"
+            "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.value.unresolved"
         ),
         (  # Query 15 - 'qualifier_type_id' property value is not a Biolink qualifier term
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
                             {
                                 'qualifier_type_id': "biolink:related_to",
                                 'qualifier_value': "fake-qualifier-value"
                             }
                         ]
                     }
                 ]
             },
-            "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.invalid"
+            "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.type_id.unknown"
         ),
         (  # Query 16 - 'qualifier' entry is missing its 'qualifier_value' property - invalidated by TRAPI schema
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
                             {
@@ -1376,49 +1376,49 @@
                 'qualifiers': [
                     {
                         'qualifier_type_id': "not-a-curie",
                         'qualifier_value': "fake-qualifier-value"
                     }
                 ]
             },
-            "error.knowledge_graph.edge.qualifiers.qualifier.invalid"
+            "error.knowledge_graph.edge.qualifiers.qualifier.type_id.unknown"
         ),
         (  # Query 8 - 'qualifier_type_id' property value is unknown
             {
                 'qualifiers': [
                     {
                         'qualifier_type_id': "biolink:unknown_qualifier",
                         'qualifier_value': "fake-qualifier-value"
                     }
                 ]
             },
-            "error.knowledge_graph.edge.qualifiers.qualifier.invalid"
+            "error.knowledge_graph.edge.qualifiers.qualifier.type_id.unknown"
         ),
         (  # Query 9 - 'qualifier_type_id' property value is valid but abstract
             {
                 'qualifiers': [
                     {
                         'qualifier_type_id': "biolink:aspect_qualifier",
                         'qualifier_value': "stability"
                     }
                 ]
             },
             # "info.query_graph.edge.qualifier.abstract"
-            "error.knowledge_graph.edge.qualifiers.qualifier.invalid"
+            "error.knowledge_graph.edge.qualifiers.qualifier.value.unresolved"
         ),
         (  # Query 10 - 'qualifier_type_id' property value is not a Biolink qualifier term
             {
                 'qualifiers': [
                     {
                         'qualifier_type_id': "biolink:related_to",
                         'qualifier_value': "fake-qualifier-value"
                     }
                 ]
             },
-            "error.knowledge_graph.edge.qualifiers.qualifier.invalid"
+            "error.knowledge_graph.edge.qualifiers.qualifier.type_id.unknown"
         ),
         (  # Query 11 - 'qualifier' entry is missing its 'qualifier_value' property - invalidated by TRAPI schema
             {
                 'qualifiers': [
                     {
                         'qualifier_type_id': "biolink:object_direction_qualifier"
                     }
```

### Comparing `reasoner_validator-3.4.8/tests/test_response_validator.py` & `reasoner_validator-3.4.9/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.8/tests/test_semver.py` & `reasoner_validator-3.4.9/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.8/tests/test_validate.py` & `reasoner_validator-3.4.9/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.8/tests/test_validation_report.py` & `reasoner_validator-3.4.9/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.4.8/PKG-INFO` & `reasoner_validator-3.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.4.8
+Version: 3.4.9
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```


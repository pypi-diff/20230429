# Comparing `tmp/neoaccess-4.1.0.tar.gz` & `tmp/neoaccess-4.2.0.tar.gz`

## Comparing `neoaccess-4.1.0.tar` & `neoaccess-4.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1092 2020-02-02 00:00:00.000000 neoaccess-4.1.0/LICENSE.txt
--rwxr-xr-x   0        0        0      242 2020-02-02 00:00:00.000000 neoaccess-4.1.0/README.md
--rwxr-xr-x   0        0        0      974 2020-02-02 00:00:00.000000 neoaccess-4.1.0/pyproject.toml
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 neoaccess-4.1.0/src/neoaccess/__init__.py
--rwxr-xr-x   0        0        0    24221 2020-02-02 00:00:00.000000 neoaccess-4.1.0/src/neoaccess/cypher_utils.py
--rwxr-xr-x   0        0        0   157741 2020-02-02 00:00:00.000000 neoaccess-4.1.0/src/neoaccess/neoaccess.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 neoaccess-4.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1092 2020-02-02 00:00:00.000000 neoaccess-4.2.0/LICENSE.txt
+-rwxr-xr-x   0        0        0      242 2020-02-02 00:00:00.000000 neoaccess-4.2.0/README.md
+-rwxr-xr-x   0        0        0      975 2020-02-02 00:00:00.000000 neoaccess-4.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 neoaccess-4.2.0/src/neoaccess/__init__.py
+-rwxr-xr-x   0        0        0    24237 2020-02-02 00:00:00.000000 neoaccess-4.2.0/src/neoaccess/cypher_utils.py
+-rwxr-xr-x   0        0        0   160376 2020-02-02 00:00:00.000000 neoaccess-4.2.0/src/neoaccess/neoaccess.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 neoaccess-4.2.0/PKG-INFO
```

### Comparing `neoaccess-4.1.0/LICENSE.txt` & `neoaccess-4.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neoaccess-4.1.0/pyproject.toml` & `neoaccess-4.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "neoaccess"
-version = "4.1.0"
+version = "4.2.0"
 authors = [
   { name = "Julian West BrainAnnex.org" },
 ]
 maintainers = [
   { email = "julian@brainannex.org" },
 ]
 description = "High-level interface to the Neo4j graph database"
@@ -17,15 +17,15 @@
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "neo4j==4.3.9",
+  "neo4j==4.4.11",
   "numpy~=1.22.4",
   "pandas~=1.4.3",
 ]
 keywords = [
   "graph database",
   "knowledge graph",
   "neo4j",
```

### Comparing `neoaccess-4.1.0/src/neoaccess/cypher_utils.py` & `neoaccess-4.2.0/src/neoaccess/cypher_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         """
         Raise an Exception if the argument is not a valid Neo4j internal database ID
 
         :param internal_id: Alleged Neo4j internal database ID
         :return:            None
         """
         assert type(internal_id) == int, \
-            f"assert_valid_internal_id(): Neo4j internal ID's MUST be integers; the value passed was {type(internal_id)}"
+            f"assert_valid_internal_id(): Neo4j internal ID's MUST be integers; the value passed ({internal_id}) was {type(internal_id)}"
 
         # Note that 0 is a valid Neo4j ID (apparently inconsistently assigned, on occasion, by the database)
         assert internal_id >= 0, \
             f"assert_valid_internal_id(): Neo4j internal ID's cannot be negative; the value passed was {internal_id}"
```

### Comparing `neoaccess-4.1.0/src/neoaccess/neoaccess.py` & `neoaccess-4.2.0/src/neoaccess/neoaccess.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,58 +311,60 @@
             for node in data_as_list:
                 data.append(node[single_column])
 
             return data
 
 
 
-    def query_extended(self, q: str, params = None, flatten = False, fields_to_exclude = None) -> [dict]:
+    def query_extended(self, q: str, data_binding = None, flatten = False, fields_to_exclude = None) -> [dict]:
         """
-        Extended version of query(), meant to extract additional info for queries that return Graph Data Types,
+        Extended version of query(), meant to extract additional info
+        for queries that return Graph Data Types,
         i.e. nodes, relationships or paths,
         such as "MATCH (n) RETURN n", or "MATCH (n1)-[r]->(n2) RETURN r"
 
-        For example, useful in scenarios where nodes were returned, and their Neo4j internal IDs and/or labels are desired
+        For example, useful in scenarios where nodes were returned,
+        and their Neo4j internal IDs and/or labels are desired
         (in addition to all the properties and their values)
 
         Unless the flatten flag is True, individual records are kept as separate lists.
             For example, "MATCH (b:boat), (c:car) RETURN b, c"
             will return a structure such as [ [b1, c1] , [b2, c2] ]  if flatten is False,
             vs.  [b1, c1, b2, c2]  if  flatten is True.  (Note: each b1, c1, etc, is a dictionary.)
 
         TODO:  Scenario to test:
             if b1 == b2, would that still be [b1, c1, b1(b2), c2] or [b1, c1, c2] - i.e. would we remove the duplicates?
             Try running with flatten=True "MATCH (b:boat), (c:car) RETURN b, c" on data like "CREATE (b:boat), (c1:car1), (c2:car2)"
 
         :param q:       A Cypher query
-        :param params:  An optional Cypher dictionary
+        :param data_binding:  An optional Cypher dictionary
                             EXAMPLE, assuming that the cypher string contains the substring "$age":
                                         {'age': 20}
         :param flatten: Flag indicating whether the Graph Data Types need to remain clustered by record,
                         or all placed in a single flattened list
         :param fields_to_exclude:   Optional list of strings with name of fields (in the database or special ones added by this function)
                                     that wishes to drop.  No harm in listing fields that aren't present
 
         :return:        A (possibly empty) list of dictionaries, if flatten is True,
                         or a list of list, if flatten is False.
                         Each item in the lists is a dictionary, with details that will depend on which Graph Data Types
-                                    were returned in the Cypher query.
-                                    EXAMPLE of individual items - for a returned NODE
-                                        {'gender': 'M', 'age': 20, 'internal_id': 123, 'neo4j_labels': ['patient']}
-                                    EXAMPLE of individual items - for a returned RELATIONSHIP
-                                        {'price': 7500, 'internal_id': 2,
-                                         'neo4j_start_node': <Node id=11 labels=frozenset() properties={}>,
-                                         'neo4j_end_node': <Node id=14 labels=frozenset() properties={}>,
-                                         'neo4j_type': 'bought_by'}]
+                                were returned in the Cypher query.
+                                EXAMPLE of *individual items* - for a returned NODE
+                                    {'gender': 'M', 'age': 20, 'internal_id': 123, 'neo4j_labels': ['patient']}
+                                EXAMPLE of *individual items* - for a returned RELATIONSHIP
+                                    {'price': 7500, 'internal_id': 2,
+                                     'neo4j_start_node': <Node id=11 labels=frozenset() properties={}>,
+                                     'neo4j_end_node': <Node id=14 labels=frozenset() properties={}>,
+                                     'neo4j_type': 'bought_by'}]
         """
         # Start a new session, use it, and then immediately close it
         with self.driver.session() as new_session:
-            result = new_session.run(q, params)
+            result = new_session.run(q, data_binding)
             if self.profiling:
-                print("-- query_extended() PROFILING ----------\n", q, "\n", params)
+                print("-- query_extended() PROFILING ----------\n", q, "\n", data_binding)
 
             # Note: A neo4j.Result iterable object (printing it, shows an object of type "neo4j.work.result.Result")
             #       See https://neo4j.com/docs/api/python-driver/current/api.html#neo4j.Result
             if result is None:
                 return []
 
             data_as_list = []
@@ -832,16 +834,14 @@
             print("In get_node_internal_id()")
             print("    match_structure:", match_structure)
 
         # Unpack needed values from the match dictionary
         (node, where, data_binding) = CypherUtils.unpack_match(match_structure, include_dummy=False)
 
         q = f"MATCH {node} {CypherUtils.prepare_where(where)} RETURN id(n) AS INTERNAL_ID"
-        print(q)
-        print(data_binding)
         self.debug_query_print(q, data_binding, "get_node_internal_id")
 
         result = self.query(q, data_binding, single_column="INTERNAL_ID")
 
         assert len(result) != 0, "get_node_internal_id(): node NOT found"
 
         assert len(result) <= 1, f"get_node_internal_id(): node not uniquely identified ({len(result)} matches found)"
@@ -875,19 +875,20 @@
     def ________CREATE_NODES________(DIVIDER):
         pass        # Used to get a better structure view in IDEs
     #####################################################################################################
 
 
     def create_node(self, labels, properties=None) -> int:
         """
-        Create a new node with the given label(s) and with the attributes/values specified in the properties dictionary.
+        Create a new node with the given label(s),
+        and with the attributes/values specified in the properties dictionary.
         Return the Neo4j internal ID of the node just created.
 
         :param labels:      A string, or list/tuple of strings, specifying Neo4j labels (ok to have blank spaces)
-        :param properties:  An optional (possibly empty or None) dictionary of properties to set for the new node.
+        :param properties:  OPTIONAL (possibly empty or None) dictionary of properties to set for the new node.
                                 EXAMPLE: {'age': 22, 'gender': 'F'}
 
         :return:            An integer with the Neo4j internal ID of the node just created
         """
 
         if properties is None:
             properties = {}
@@ -1026,15 +1027,15 @@
         return self.create_node_with_links(labels=labels, properties=properties, links=links, merge=merge)
 
 
 
     def create_node_with_links(self, labels, properties=None, links=None, merge=False) -> int:
         """
         Create a new node, with the given labels and optional properties,
-        and make it a parent of all the EXISTING nodes that are specified
+        and link it up to all the EXISTING nodes that are specified
         in the (possibly empty) list of link nodes, identified by their Neo4j internal ID's.
 
         The list of link nodes also contains the names to give to each link,
         as well as their directions (by default OUTbound from the newly-created node)
         and, optionally, properties on the links.
 
         If any of the requested link nodes isn't found,
@@ -1725,22 +1726,22 @@
 
         return number_relationships_added
 
 
 
     def add_links_fast(self, match_from: int, match_to: int, rel_name:str) -> int:
         """
-        Experimental first method optimized for speed.  Only internal database ID are used
+        Method optimized for speed.  Only internal database ID are used.
 
         Add a links (aka graph edges/relationships), with the specified rel_name,
         originating in the node identified by match_from,
         and terminating in the node identified by match_to
 
-        :param match_from:  An integer with a Neo4j node id
-        :param match_to:    An integer with a Neo4j node id
+        :param match_from:  An integer with an internal Neo4j node id
+        :param match_to:    An integer with an internal Neo4j node id
         :param rel_name:    The name to give to the new relationship between the 2 specified nodes.  Blanks allowed
 
         :return:            The number of links added.  If none got added, or in case of error, an Exception is raised
         """
         # Prepare the query to add the requested links between the given nodes (possibly, sets of nodes)
         q = f'''
             MATCH (from), (to)
@@ -2127,50 +2128,101 @@
 
         self.debug_query_print(q, data_binding, "count_links")
 
         return self.query(q, data_binding, single_cell="link_count")
 
 
 
-    def get_parents_and_children(self, node_id: int) -> ():
+    def get_parents_and_children(self, internal_id: int) -> ():
         """
         Fetch all the nodes connected to the given one by INbound relationships to it (its "parents"),
         as well as by OUTbound relationships to it (its "children")
+        TODO: allow specifying a relationship name to follow
 
-        :param node_id: An integer with a Neo4j internal node ID
-        :return:        A dictionary with 2 keys: 'parent_list' and 'child_list'
-                        The values are lists of dictionaries with 3 keys: "internal_id", "label", "rel"
-                            EXAMPLE of individual items in either parent_list or child_list:
-                            {'internal_id': 163, 'labels': ['Subject'], 'rel': 'HAS_TREATMENT'}
+        :param internal_id: An integer with a Neo4j internal node ID
+        :return:            A dictionary with 2 keys: 'parent_list' and 'child_list'
+                                The values are lists of dictionaries with 3 keys: "internal_id", "label", "rel"
+                                EXAMPLE of individual items in either parent_list or child_list:
+                                {'internal_id': 163, 'labels': ['Subject'], 'rel': 'HAS_TREATMENT'}
         """
 
         # Fetch the parents
-        cypher = f"MATCH (parent)-[inbound]->(n) WHERE id(n) = {node_id} " \
+        cypher = f"MATCH (parent)-[inbound]->(n) WHERE id(n) = {internal_id} " \
                  "RETURN id(parent) AS internal_id, labels(parent) AS labels, type(inbound) AS rel"
 
         parent_list = self.query(cypher)
         # EXAMPLE of parent_list:
         #       [{'internal_id': 163, 'labels': ['Subject'], 'rel': 'HAS_TREATMENT'},
         #        {'internal_id': 150, 'labels': ['Subject'], 'rel': 'HAS_TREATMENT'}]
 
 
         # Fetch the children
-        cypher = f"MATCH (n)-[outbound]->(child) WHERE id(n) = {node_id} " \
+        cypher = f"MATCH (n)-[outbound]->(child) WHERE id(n) = {internal_id} " \
                  "RETURN id(child) AS internal_id, labels(child) AS labels, type(outbound) AS rel"
 
         child_list = self.query(cypher)
         # EXAMPLE of child_list:
         #       [{'internal_id': 107, 'labels': ['Source Data Row'], 'rel': 'FROM_DATA'},
         #        {'internal_id': 103, 'labels': ['Source Data Row'], 'rel': 'FROM_DATA'}]
 
 
         return (parent_list, child_list)
 
 
 
+    def get_siblings(self, internal_id: int, rel_name: str, rel_dir="OUT") -> [int]:
+        """
+        Return the data of all the "sibling" nodes of the given one.
+        "Siblings" is meant as "sharing a link (by default outbound) of the specified name,
+        to a common other node".
+
+        EXAMPLE: 2 nodes, "French" and "German",
+                 each with a outbound link named "subcategory_of" to a third node,
+                 will be considered "siblings" under rel_name="subcategory_of" and rel_dir="OUT
+
+        :param internal_id: Integer with the internal database ID of the node of interest
+        :param rel_name:    The name of the relationship used to establish a "siblings" connection
+        :param rel_dir:     Either "OUT" (default) or "IN".  The link direction expected from the
+                                start node to its "parents" - and then IN REVERSE to the parent's children
+        :return:            A list of dictionaries, with one element for each "sibling";
+                                each element contains the 'internal_id' and 'neo4j_labels' keys,
+                                plus whatever attributes are stored on that node.
+                                EXAMPLE of single element:
+                                {'name': 'French', 'internal_id': 123, 'neo4j_labels': ['Categories']}
+        """
+        CypherUtils.assert_valid_internal_id(internal_id)
+
+        assert type(rel_name) == str, \
+            f"get_siblings(): argument `rel_name` must be a string; " \
+            f"the given value ({rel_name}) is of type {type(rel_name)}"
+
+        # Follow the links with the specified name, in the indicated direction from the given link,
+        # and then in the reverse direction
+        if rel_dir == "OUT":
+            q = f"""
+                MATCH (n) - [:{rel_name}] -> (parent) <- [:{rel_name}] - (sibling)
+                WHERE id(n) = $internal_id
+                RETURN sibling
+                """
+        elif rel_dir == "IN":
+            q = f"""
+                MATCH (n) <- [:{rel_name}] - (parent) - [:{rel_name}] -> (sibling)
+                WHERE id(n) = $internal_id
+                RETURN sibling
+                """
+        else:
+            raise Exception(f"get_siblings(): unknown value for the `rel_dir` argument ({rel_dir}); "
+                            f"allowed values are 'IN' and 'OUT'")
+
+        result = self.query_extended(q, data_binding={"internal_id": internal_id}, flatten=True)
+        return result
+
+
+
+
 
     #####################################################################################################
 
     '''                                      ~   LABELS   ~                                           '''
 
     def ________LABELS________(DIVIDER):
         pass        # Used to get a better structure view in IDEs
@@ -2202,17 +2254,17 @@
         q = """
             CALL db.schema.nodeTypeProperties() 
             YIELD nodeLabels, propertyName
             WHERE $label in nodeLabels and propertyName IS NOT NULL
             RETURN DISTINCT propertyName 
             ORDER BY propertyName
             """
-        params = {'label': label}
+        data_binding = {'label': label}
 
-        return [res['propertyName'] for res in self.query(q, params)]
+        return [res['propertyName'] for res in self.query(q, data_binding)]
 
 
 
 
     #####################################################################################################
 
     '''                                      ~   INDEXES   ~                                          '''
@@ -3040,8 +3092,8 @@
 
     def _debug_local(self) -> str:
         """
         Use to test the switch from a local to remote repository, for debugging
 
         :return:
         """
-        return "remote"
+        return "local"
```

### Comparing `neoaccess-4.1.0/PKG-INFO` & `neoaccess-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: neoaccess
-Version: 4.1.0
+Version: 4.2.0
 Summary: High-level interface to the Neo4j graph database
 Project-URL: Bug Tracker, https://github.com/BrainAnnex/brain-annex/issues
 Project-URL: Documentation, https://brainannex.org/guide.php
 Project-URL: Home-page, https://brainannex.org/guide.php
 Project-URL: Homepage, https://brainannex.org/guide.php
 Project-URL: Source, https://github.com/BrainAnnex/neoaccess
 Author: Julian West BrainAnnex.org
 Maintainer-email: julian@brainannex.org
 Keywords: graph database,knowledge graph,neo4j
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: neo4j==4.3.9
+Requires-Dist: neo4j==4.4.11
 Requires-Dist: numpy~=1.22.4
 Requires-Dist: pandas~=1.4.3
 Description-Content-Type: text/markdown
 
 # High-level interface to the Neo4j graph database    
 
 https://brainannex.org/guide.php
```


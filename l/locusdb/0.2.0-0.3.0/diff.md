# Comparing `tmp/locusdb-0.2.0.tar.gz` & `tmp/locusdb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locusdb-0.2.0.tar", max compression
+gzip compressed data, was "locusdb-0.3.0.tar", max compression
```

## Comparing `locusdb-0.2.0.tar` & `locusdb-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-23 18:03:54.915691 locusdb-0.2.0/LICENSE
--rw-r--r--   0        0        0     1188 2023-04-23 18:03:54.915691 locusdb-0.2.0/README.md
--rw-r--r--   0        0        0      592 2023-04-23 18:04:07.240211 locusdb-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       91 2023-04-23 18:03:54.915691 locusdb-0.2.0/src/locusdb/__init__.py
--rw-r--r--   0        0        0      913 2023-04-23 18:03:54.915691 locusdb-0.2.0/src/locusdb/config.py
--rw-r--r--   0        0        0     3247 2023-04-23 18:03:54.915691 locusdb-0.2.0/src/locusdb/index.py
--rw-r--r--   0        0        0      619 2023-04-23 18:03:54.915691 locusdb-0.2.0/src/locusdb/vector.py
--rw-r--r--   0        0        0     1992 1970-01-01 00:00:00.000000 locusdb-0.2.0/setup.py
--rw-r--r--   0        0        0     1893 1970-01-01 00:00:00.000000 locusdb-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-29 14:38:19.059786 locusdb-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1204 2023-04-29 14:38:19.059786 locusdb-0.3.0/README.md
+-rw-r--r--   0        0        0      592 2023-04-29 14:38:28.695845 locusdb-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-04-29 14:38:19.059786 locusdb-0.3.0/src/locusdb/__init__.py
+-rw-r--r--   0        0        0      913 2023-04-29 14:38:19.059786 locusdb-0.3.0/src/locusdb/config.py
+-rw-r--r--   0        0        0     3352 2023-04-29 14:38:19.059786 locusdb-0.3.0/src/locusdb/index.py
+-rw-r--r--   0        0        0      619 2023-04-29 14:38:19.059786 locusdb-0.3.0/src/locusdb/vector.py
+-rw-r--r--   0        0        0     2004 1970-01-01 00:00:00.000000 locusdb-0.3.0/setup.py
+-rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 locusdb-0.3.0/PKG-INFO
```

### Comparing `locusdb-0.2.0/LICENSE` & `locusdb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `locusdb-0.2.0/README.md` & `locusdb-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,9 @@
 # Locus
-Locus is a local, simple, in-memory vector database.
-
-Why Locus?
-* Easy to use
-* 2 dependencies
-* Store database locally
-
+Locus is a local, simple, append-only, in-memory vector database based on hnswlib.
 
 ## Installation
 ``` bash
 pip install locusdb
 ```
 ## Example Code
 Some example code to illustrate Locus' functionality.
@@ -35,15 +29,17 @@
 # add the vectors to the index
 for vector in vectors:
     index.add_vector(vector)
 
 # retrieve the closest vectors to a query embedding
 query_embedding = np.random.randn(config.dim)
 results = index.retrieve(query_embedding, number_of_results=3)
-print(results)
+
+print(f"Matches: {results}")
+print(f"Items in index: {index.count}")
 
 # store the index on disk
 index._store_on_disk()
 
 # load the index from disk
 new_index = Index.from_file(config.storage_location)
 ```
```

### Comparing `locusdb-0.2.0/pyproject.toml` & `locusdb-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "locusdb"
-version = "v0.2.0"
+version = "v0.3.0"
 license="Apache-2.0"
 description = "Local, in-memory vector database"
 authors = ["Alex <46456279+the-alex-b@users.noreply.github.com>"]
 readme = "README.md"
 repository="https://github.com/the-alex-b/Locus"
 
 [tool.poetry.dependencies]
```

### Comparing `locusdb-0.2.0/src/locusdb/config.py` & `locusdb-0.3.0/src/locusdb/config.py`

 * *Files identical despite different names*

### Comparing `locusdb-0.2.0/src/locusdb/index.py` & `locusdb-0.3.0/src/locusdb/index.py`

 * *Files 14% similar despite different names*

```diff
@@ -62,31 +62,37 @@
         self.structured_memory: dict(Vector) = {}
 
     @classmethod
     def from_file(cls, file="index.db") -> Index:
         with open(file, "rb") as handle:
             return pickle.load(handle)
 
-    def add_vector(self, vector: Vector, persist_on_disk=True) -> None:
+    def add_vector(self, vector: Vector, persist_on_disk=False) -> None:
+        storage_id = len(self.structured_memory)
+
         # add to hnsw index
-        self.hnsw_index.add_items(vector.embedding, len(self.structured_memory))
+        self.hnsw_index.add_items(vector.embedding, storage_id)
 
         # add to stuctured data
-        self.structured_memory[len(self.structured_memory)] = vector.data
+        self.structured_memory[storage_id] = vector.data
 
         if persist_on_disk:
-            self._store_on_disk()
+            self.persist_on_disk()
 
     def retrieve(self, embedding: np.array, number_of_results: int = 3) -> list[dict]:
         labels, distances = self.hnsw_index.knn_query(embedding, k=number_of_results)
 
         return [
             {"element": self.structured_memory[id], "distance": distances[0][i]}
             for i, id in enumerate(labels[0])
         ]
 
-    def _store_on_disk(self) -> None:
+    def persist_on_disk(self) -> None:
         with open(
             self.config.storage_location,
             "wb",
         ) as handle:
             pickle.dump(self, handle, protocol=pickle.HIGHEST_PROTOCOL)
+
+    @property
+    def count(self) -> int:
+        return len(self.structured_memory)
```

### Comparing `locusdb-0.2.0/src/locusdb/vector.py` & `locusdb-0.3.0/src/locusdb/vector.py`

 * *Files identical despite different names*

### Comparing `locusdb-0.2.0/setup.py` & `locusdb-0.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['hnswlib>=0.7.0,<0.8.0', 'numpy>=1.24.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'locusdb',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Local, in-memory vector database',
-    'long_description': '# Locus\nLocus is a local, simple, in-memory vector database.\n\nWhy Locus?\n* Easy to use\n* 2 dependencies\n* Store database locally\n\n\n## Installation\n``` bash\npip install locusdb\n```\n## Example Code\nSome example code to illustrate Locus\' functionality.\n\n``` python\nimport numpy as np\nfrom locusdb import Config, Vector, Index\n\n# create a new configuration\nconfig = Config(max_elements=1000, ef_construction=200, M=16, dim=128, space="cosine", storage_location="index.db")\n\n# create a new index instance\nindex = Index(dimensions=config.dim, config=config)\n\n# create some random vectors\nvectors = []\nfor i in range(10):\n    embedding = np.random.randn(config.dim)\n    data = {"id": i, "message": f"test message {i}"}\n    vector = Vector(embedding=embedding, data=data)\n    vectors.append(vector)\n\n# add the vectors to the index\nfor vector in vectors:\n    index.add_vector(vector)\n\n# retrieve the closest vectors to a query embedding\nquery_embedding = np.random.randn(config.dim)\nresults = index.retrieve(query_embedding, number_of_results=3)\nprint(results)\n\n# store the index on disk\nindex._store_on_disk()\n\n# load the index from disk\nnew_index = Index.from_file(config.storage_location)\n```\n\n',
+    'long_description': '# Locus\nLocus is a local, simple, append-only, in-memory vector database based on hnswlib.\n\n## Installation\n``` bash\npip install locusdb\n```\n## Example Code\nSome example code to illustrate Locus\' functionality.\n\n``` python\nimport numpy as np\nfrom locusdb import Config, Vector, Index\n\n# create a new configuration\nconfig = Config(max_elements=1000, ef_construction=200, M=16, dim=128, space="cosine", storage_location="index.db")\n\n# create a new index instance\nindex = Index(dimensions=config.dim, config=config)\n\n# create some random vectors\nvectors = []\nfor i in range(10):\n    embedding = np.random.randn(config.dim)\n    data = {"id": i, "message": f"test message {i}"}\n    vector = Vector(embedding=embedding, data=data)\n    vectors.append(vector)\n\n# add the vectors to the index\nfor vector in vectors:\n    index.add_vector(vector)\n\n# retrieve the closest vectors to a query embedding\nquery_embedding = np.random.randn(config.dim)\nresults = index.retrieve(query_embedding, number_of_results=3)\n\nprint(f"Matches: {results}")\nprint(f"Items in index: {index.count}")\n\n# store the index on disk\nindex._store_on_disk()\n\n# load the index from disk\nnew_index = Index.from_file(config.storage_location)\n```\n\n',
     'author': 'Alex',
     'author_email': '46456279+the-alex-b@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/the-alex-b/Locus',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `locusdb-0.2.0/PKG-INFO` & `locusdb-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locusdb
-Version: 0.2.0
+Version: 0.3.0
 Summary: Local, in-memory vector database
 Home-page: https://github.com/the-alex-b/Locus
 License: Apache-2.0
 Author: Alex
 Author-email: 46456279+the-alex-b@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,21 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: hnswlib (>=0.7.0,<0.8.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Project-URL: Repository, https://github.com/the-alex-b/Locus
 Description-Content-Type: text/markdown
 
 # Locus
-Locus is a local, simple, in-memory vector database.
-
-Why Locus?
-* Easy to use
-* 2 dependencies
-* Store database locally
-
+Locus is a local, simple, append-only, in-memory vector database based on hnswlib.
 
 ## Installation
 ``` bash
 pip install locusdb
 ```
 ## Example Code
 Some example code to illustrate Locus' functionality.
@@ -54,15 +48,17 @@
 # add the vectors to the index
 for vector in vectors:
     index.add_vector(vector)
 
 # retrieve the closest vectors to a query embedding
 query_embedding = np.random.randn(config.dim)
 results = index.retrieve(query_embedding, number_of_results=3)
-print(results)
+
+print(f"Matches: {results}")
+print(f"Items in index: {index.count}")
 
 # store the index on disk
 index._store_on_disk()
 
 # load the index from disk
 new_index = Index.from_file(config.storage_location)
 ```
```


# Comparing `tmp/spiralflow-0.0.5.tar.gz` & `tmp/spiralflow-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiralflow-0.0.5.tar", last modified: Fri Apr 28 22:12:23 2023, max compression
+gzip compressed data, was "spiralflow-0.0.6.tar", last modified: Sat Apr 29 15:55:38 2023, max compression
```

## Comparing `spiralflow-0.0.5.tar` & `spiralflow-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 22:12:23.834016 spiralflow-0.0.5/
--rw-rw-rw-   0        0        0     1092 2023-04-28 19:29:02.000000 spiralflow-0.0.5/LICENSE
--rw-rw-rw-   0        0        0    13703 2023-04-28 22:12:23.834016 spiralflow-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    13177 2023-04-28 22:11:41.000000 spiralflow-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 22:12:23.834016 spiralflow-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      851 2023-04-28 21:36:21.000000 spiralflow-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 22:12:23.818395 spiralflow-0.0.5/spiralflow/
--rw-rw-rw-   0        0        0       23 2023-04-28 21:36:33.000000 spiralflow-0.0.5/spiralflow/__init__.py
--rw-rw-rw-   0        0        0     5385 2023-04-28 19:29:02.000000 spiralflow-0.0.5/spiralflow/chat_history.py
--rw-rw-rw-   0        0        0     1330 2023-04-28 19:29:02.000000 spiralflow-0.0.5/spiralflow/chat_llm.py
--rw-rw-rw-   0        0        0     7649 2023-04-28 20:16:32.000000 spiralflow-0.0.5/spiralflow/chunking.py
--rw-rw-rw-   0        0        0    53659 2023-04-28 19:29:02.000000 spiralflow-0.0.5/spiralflow/flow.py
--rw-rw-rw-   0        0        0     6096 2023-04-28 19:49:23.000000 spiralflow-0.0.5/spiralflow/loading.py
--rw-rw-rw-   0        0        0     6847 2023-04-28 22:04:46.000000 spiralflow-0.0.5/spiralflow/memory.py
--rw-rw-rw-   0        0        0    16849 2023-04-28 19:29:02.000000 spiralflow-0.0.5/spiralflow/message.py
--rw-rw-rw-   0        0        0     7464 2023-04-28 19:29:02.000000 spiralflow-0.0.5/spiralflow/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-28 22:12:23.818395 spiralflow-0.0.5/spiralflow.egg-info/
--rw-rw-rw-   0        0        0    13703 2023-04-28 22:12:23.000000 spiralflow-0.0.5/spiralflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-04-28 22:12:23.000000 spiralflow-0.0.5/spiralflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 22:12:23.000000 spiralflow-0.0.5/spiralflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-28 22:12:23.000000 spiralflow-0.0.5/spiralflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-28 22:12:23.000000 spiralflow-0.0.5/spiralflow.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 15:55:38.939047 spiralflow-0.0.6/
+-rw-rw-rw-   0        0        0     1092 2023-04-09 17:15:16.000000 spiralflow-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0    13703 2023-04-29 15:55:38.933539 spiralflow-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    13177 2023-04-29 00:59:25.000000 spiralflow-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-29 15:55:38.939047 spiralflow-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      851 2023-04-29 15:53:54.000000 spiralflow-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:55:38.917421 spiralflow-0.0.6/spiralflow/
+-rw-rw-rw-   0        0        0       23 2023-04-29 15:53:47.000000 spiralflow-0.0.6/spiralflow/__init__.py
+-rw-rw-rw-   0        0        0     5385 2023-04-24 19:26:36.000000 spiralflow-0.0.6/spiralflow/chat_history.py
+-rw-rw-rw-   0        0        0     1330 2023-04-24 19:26:36.000000 spiralflow-0.0.6/spiralflow/chat_llm.py
+-rw-rw-rw-   0        0        0     4078 2023-04-29 06:34:36.000000 spiralflow-0.0.6/spiralflow/chunking.py
+-rw-rw-rw-   0        0        0    53255 2023-04-29 01:48:57.000000 spiralflow-0.0.6/spiralflow/flow.py
+-rw-rw-rw-   0        0        0     6096 2023-04-29 00:59:25.000000 spiralflow-0.0.6/spiralflow/loading.py
+-rw-rw-rw-   0        0        0     7102 2023-04-29 03:51:20.000000 spiralflow-0.0.6/spiralflow/memory.py
+-rw-rw-rw-   0        0        0    16849 2023-04-24 19:26:36.000000 spiralflow-0.0.6/spiralflow/message.py
+-rw-rw-rw-   0        0        0     7459 2023-04-29 01:45:44.000000 spiralflow-0.0.6/spiralflow/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:55:38.932540 spiralflow-0.0.6/spiralflow.egg-info/
+-rw-rw-rw-   0        0        0    13703 2023-04-29 15:55:38.000000 spiralflow-0.0.6/spiralflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-04-29 15:55:38.000000 spiralflow-0.0.6/spiralflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 15:55:38.000000 spiralflow-0.0.6/spiralflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-29 15:55:38.000000 spiralflow-0.0.6/spiralflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-29 15:55:38.000000 spiralflow-0.0.6/spiralflow.egg-info/top_level.txt
```

### Comparing `spiralflow-0.0.5/LICENSE` & `spiralflow-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.5/PKG-INFO` & `spiralflow-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiralflow
-Version: 0.0.5
+Version: 0.0.6
 Summary: A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.
 Home-page: https://github.com/Tiger767/Spiralflow
 Author: Travis Hammond
 License: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spiralflow-0.0.5/README.md` & `spiralflow-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.5/setup.py` & `spiralflow-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spiralflow",
-    version="0.0.5",
+    version="0.0.6",
     author="Travis Hammond",
     description="A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tiger767/Spiralflow",
     packages=setuptools.find_packages(),
     install_requires=["regex", "openai", "pandas", "tiktoken", "pymupdf", "bs4"],
```

### Comparing `spiralflow-0.0.5/spiralflow/chat_history.py` & `spiralflow-0.0.6/spiralflow/chat_history.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.5/spiralflow/chat_llm.py` & `spiralflow-0.0.6/spiralflow/chat_llm.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.5/spiralflow/flow.py` & `spiralflow-0.0.6/spiralflow/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,17 +433,14 @@
             )
 
         if len(new_input_chat_histories) > 1:
             raise ValueError(
                 f"FuncChatFlow func must return a empty or single input chat history. Received {len(new_input_chat_histories)}"
             )
 
-        # if len(new_input_chat_histories) != len(internal_histories):
-        #    raise ValueError(f'FuncChatFlow func must return the same number of input and internal chat histories. Received {len(new_input_chat_histories)} and {len(internal_histories)}')
-
         return outputs, (new_input_chat_histories, internal_histories)
 
 
 class ChatFlowWrapper(ChatFlow):
     """
     A ChatFlow wrapper class for others to inherit from.
     """
@@ -1341,17 +1338,14 @@
             input_variables,
             reset_history=reset_history,
             chat_llm=chat_llm,
             input_chat_history=input_chat_history,
             max_iterations=max_iterations,
         )
 
-        # histories = self.compress_histories(histories)
-        # history = ChatHistory(histories[0].messages + histories[1].messages)
-
         if not return_all:
             variables = {
                 k: v for k, v in variables.items() if k in self.output_varnames
             }
         return variables, history
 
     def compress_histories(
```

### Comparing `spiralflow-0.0.5/spiralflow/loading.py` & `spiralflow-0.0.6/spiralflow/loading.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.5/spiralflow/memory.py` & `spiralflow-0.0.6/spiralflow/memory.py`

 * *Files 14% similar despite different names*

```diff
@@ -63,31 +63,33 @@
             self.data = pd.DataFrame(columns=["text", "metadata"])
             self.index = None
         else:
             self.filepath = filepath
             self.load()
 
     def _create_index(self, embeddings: np.ndarray) -> None:
+        embeddings = embeddings.astype(np.float32)
         _, d = embeddings.shape
-        self.index = faiss.IndexFlatL2(d)
-        self.index.add(embeddings.astype(np.float32))
+        self.index = faiss.IndexFlatIP(d)
+        self.index.add(embeddings / np.linalg.norm(embeddings, axis=-1))
 
     def save(self, filepath: Optional[str] = None) -> None:
         """
         Saves the memory to a file.
         :param filepath: Path to the pickle file to save the memory to. If None, the filepath passed in the constructor is used.
         """
         if filepath is None:
             filepath = self.filepath
 
         with open(filepath + ".pkl", "wb") as f:
             pickle.dump(self, f)
 
     def load(self, filepath: Optional[str] = None) -> None:
         """
+        Loads the memory from a pickle file.
         :param filepath: Path to a pickle file to load the memory from. If None, the filepath passed in the constructor is used.
         """
         if filepath is None:
             filepath = self.filepath
 
         with open(filepath, "rb") as f:
             loaded_memory = pickle.load(f)
@@ -105,51 +107,54 @@
         :param filepath: Path to the file (csv or parquet) to save the memory to.
                          If None, the filepath passed in the constructor is used.
         """
 
         if "text" not in data:
             raise ValueError("Data must have a 'text' field.")
 
-        # get embedding of text
         embedding = np.array(
             [get_embedding(data["text"], engine=self.embedding_model)], dtype=np.float32
         )
 
         data = pd.DataFrame(data, index=[0])
         self.data = pd.concat([self.data, data], ignore_index=True)
 
         if self.index is None:
             self._create_index(embedding)
         else:
-            self.index.add(embedding)
+            self.index.add(embedding / np.linalg.norm(embedding, axis=-1))
 
         if save:
             self.save(filepath)
 
     def query(
         self, query: str, k: int = 1, combine_threshold: Optional[float] = None
     ) -> list[Dict[str, str]]:
         """
         Queries the memory with the given query.
         :param query: Query to use to get memory.
         :param k: Max number of results to return.
         :param combine_threshold: Threshold for ratio of overlap to combine results from multiple queries.
                                   If None, no combining is done.
-        :return: Memory obtained from external memories.
+        :return: Memory obtained from external memories with metadata and scores (cosine similarity).
         """
         if self.data.empty:
             raise ValueError(
                 "No memory to query. Add data to memory by calling Memory.add() before querying."
             )
 
         # get embedding of query
-        embeded_query = np.array([get_embedding(query, engine=self.embedding_model)], dtype=np.float32)
+        embeded_query = np.array(
+            [get_embedding(query, engine=self.embedding_model)], dtype=np.float32
+        )
 
         # search for the indexes with similar embeddings
-        scores, similar_indexes = self.index.search(embeded_query, k=k)
+        scores, similar_indexes = self.index.search(
+            embeded_query / np.linalg.norm(embeded_query, axis=-1), k=k
+        )
 
         # get the memory values at the found indexes
         memories = []
 
         for score, i in zip(scores[0], similar_indexes[0]):
             memory = {
                 "text": self.data.iloc[i, 0],
```

### Comparing `spiralflow-0.0.5/spiralflow/message.py` & `spiralflow-0.0.6/spiralflow/message.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.5/spiralflow/tools.py` & `spiralflow-0.0.6/spiralflow/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import Any, Dict, Optional, Union
+from typing import Dict, Optional, Union
 import numpy as np
 
 import os
 
 from googleapiclient.discovery import build
```

### Comparing `spiralflow-0.0.5/spiralflow.egg-info/PKG-INFO` & `spiralflow-0.0.6/spiralflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiralflow
-Version: 0.0.5
+Version: 0.0.6
 Summary: A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.
 Home-page: https://github.com/Tiger767/Spiralflow
 Author: Travis Hammond
 License: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


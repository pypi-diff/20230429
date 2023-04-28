# Comparing `tmp/spiralflow-0.0.4.tar.gz` & `tmp/spiralflow-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiralflow-0.0.4.tar", last modified: Fri Apr 28 17:13:56 2023, max compression
+gzip compressed data, was "spiralflow-0.0.5.tar", last modified: Fri Apr 28 22:12:23 2023, max compression
```

## Comparing `spiralflow-0.0.4.tar` & `spiralflow-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 17:13:56.851030 spiralflow-0.0.4/
--rw-rw-rw-   0        0        0     1092 2023-04-09 17:15:16.000000 spiralflow-0.0.4/LICENSE
--rw-rw-rw-   0        0        0    13703 2023-04-28 17:13:56.846029 spiralflow-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    13177 2023-04-28 16:52:05.000000 spiralflow-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 17:13:56.851030 spiralflow-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      851 2023-04-28 16:34:47.000000 spiralflow-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 17:13:56.831405 spiralflow-0.0.4/spiralflow/
--rw-rw-rw-   0        0        0       23 2023-04-28 15:44:36.000000 spiralflow-0.0.4/spiralflow/__init__.py
--rw-rw-rw-   0        0        0     5385 2023-04-24 19:26:36.000000 spiralflow-0.0.4/spiralflow/chat_history.py
--rw-rw-rw-   0        0        0     1330 2023-04-24 19:26:36.000000 spiralflow-0.0.4/spiralflow/chat_llm.py
--rw-rw-rw-   0        0        0     4257 2023-04-28 17:13:32.000000 spiralflow-0.0.4/spiralflow/chunking.py
--rw-rw-rw-   0        0        0    53659 2023-04-26 01:41:18.000000 spiralflow-0.0.4/spiralflow/flow.py
--rw-rw-rw-   0        0        0     6128 2023-04-28 17:00:18.000000 spiralflow-0.0.4/spiralflow/loading.py
--rw-rw-rw-   0        0        0     6810 2023-04-26 01:46:56.000000 spiralflow-0.0.4/spiralflow/memory.py
--rw-rw-rw-   0        0        0    16849 2023-04-24 19:26:36.000000 spiralflow-0.0.4/spiralflow/message.py
--rw-rw-rw-   0        0        0     7464 2023-04-26 01:41:35.000000 spiralflow-0.0.4/spiralflow/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-28 17:13:56.844029 spiralflow-0.0.4/spiralflow.egg-info/
--rw-rw-rw-   0        0        0    13703 2023-04-28 17:13:56.000000 spiralflow-0.0.4/spiralflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-04-28 17:13:56.000000 spiralflow-0.0.4/spiralflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 17:13:56.000000 spiralflow-0.0.4/spiralflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-28 17:13:56.000000 spiralflow-0.0.4/spiralflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-28 17:13:56.000000 spiralflow-0.0.4/spiralflow.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 22:12:23.834016 spiralflow-0.0.5/
+-rw-rw-rw-   0        0        0     1092 2023-04-28 19:29:02.000000 spiralflow-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0    13703 2023-04-28 22:12:23.834016 spiralflow-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    13177 2023-04-28 22:11:41.000000 spiralflow-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 22:12:23.834016 spiralflow-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      851 2023-04-28 21:36:21.000000 spiralflow-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 22:12:23.818395 spiralflow-0.0.5/spiralflow/
+-rw-rw-rw-   0        0        0       23 2023-04-28 21:36:33.000000 spiralflow-0.0.5/spiralflow/__init__.py
+-rw-rw-rw-   0        0        0     5385 2023-04-28 19:29:02.000000 spiralflow-0.0.5/spiralflow/chat_history.py
+-rw-rw-rw-   0        0        0     1330 2023-04-28 19:29:02.000000 spiralflow-0.0.5/spiralflow/chat_llm.py
+-rw-rw-rw-   0        0        0     7649 2023-04-28 20:16:32.000000 spiralflow-0.0.5/spiralflow/chunking.py
+-rw-rw-rw-   0        0        0    53659 2023-04-28 19:29:02.000000 spiralflow-0.0.5/spiralflow/flow.py
+-rw-rw-rw-   0        0        0     6096 2023-04-28 19:49:23.000000 spiralflow-0.0.5/spiralflow/loading.py
+-rw-rw-rw-   0        0        0     6847 2023-04-28 22:04:46.000000 spiralflow-0.0.5/spiralflow/memory.py
+-rw-rw-rw-   0        0        0    16849 2023-04-28 19:29:02.000000 spiralflow-0.0.5/spiralflow/message.py
+-rw-rw-rw-   0        0        0     7464 2023-04-28 19:29:02.000000 spiralflow-0.0.5/spiralflow/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-28 22:12:23.818395 spiralflow-0.0.5/spiralflow.egg-info/
+-rw-rw-rw-   0        0        0    13703 2023-04-28 22:12:23.000000 spiralflow-0.0.5/spiralflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-04-28 22:12:23.000000 spiralflow-0.0.5/spiralflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 22:12:23.000000 spiralflow-0.0.5/spiralflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-28 22:12:23.000000 spiralflow-0.0.5/spiralflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-28 22:12:23.000000 spiralflow-0.0.5/spiralflow.egg-info/top_level.txt
```

### Comparing `spiralflow-0.0.4/LICENSE` & `spiralflow-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.4/PKG-INFO` & `spiralflow-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiralflow
-Version: 0.0.4
+Version: 0.0.5
 Summary: A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.
 Home-page: https://github.com/Tiger767/Spiralflow
 Author: Travis Hammond
 License: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spiralflow-0.0.4/README.md` & `spiralflow-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.4/setup.py` & `spiralflow-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spiralflow",
-    version="0.0.4",
+    version="0.0.5",
     author="Travis Hammond",
     description="A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tiger767/Spiralflow",
     packages=setuptools.find_packages(),
     install_requires=["regex", "openai", "pandas", "tiktoken", "pymupdf", "bs4"],
```

### Comparing `spiralflow-0.0.4/spiralflow/chat_history.py` & `spiralflow-0.0.5/spiralflow/chat_history.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.4/spiralflow/chat_llm.py` & `spiralflow-0.0.5/spiralflow/chat_llm.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.4/spiralflow/chunking.py` & `spiralflow-0.0.5/spiralflow/chunking.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Tuple, Union
+from typing import List, Tuple, Optional
 
 
 class Chunker:
     def __init__(self, encoder, chunk_size: int, overlap_factor: float) -> None:
         """
         :param encoder: The text encoder object.
         :param chunk_size: The desired chunk size in token units.
@@ -32,28 +32,26 @@
 
 class SmartChunker(Chunker):
     def __init__(
         self,
         encoder,
         chunk_size: int,
         overlap_factor: float,
-        delimiters_tolerances_overlap: Union[
-            None, List[Tuple[str, float, bool]]
-        ] = None,
+        delimiters_tolerances_overlap: Optional[List[Tuple[str, float, bool]]] = None,
     ) -> None:
         """
         :param encoder: The text encoder object.
         :param chunk_size: The desired chunk size in token units.
         :param overlap_factor: The factor to calculate the overlap between chunks.
         :param delimiters_tolerances_overlap: A list of tuples with delimiter,
             tolerance, and overlap values for smart chunking. Defaults to None.
         """
         super().__init__(encoder, chunk_size, overlap_factor)
 
-        self.delimiters_tolerances_overlap = (
+        self._delimiters_tolerances_overlap = (
             [
                 ("\n\n\n", 0.3, False),
                 ("\n\n", 0.15, False),
                 ("\n", 0.05, True),
                 (" ", 0.5, True),
                 ("", 0.01, True),
             ]
@@ -74,15 +72,15 @@
 
         final_chunks = []
 
         start_ndx = 0
         while start_ndx + chunk_size < len(text):
             best_chunk_end_ndx = start_ndx
 
-            for delimiter, tolerance, overlap in self.delimiters_tolerances_overlap:
+            for delimiter, tolerance, overlap in self._delimiters_tolerances_overlap:
                 search_start = start_ndx + int(chunk_size * (1 - tolerance))
                 search_end = start_ndx + chunk_size
                 delimiter_ndx = text[search_start:search_end].rfind(delimiter)
 
                 if delimiter_ndx != -1:
                     best_chunk_end_ndx = delimiter_ndx + search_start
                     break
@@ -107,7 +105,94 @@
                 ndx = text[start_ndx - overlap_offset : start_ndx].find(" ")
                 if ndx != -1:
                     start_ndx += ndx - overlap_offset
         # if start_ndx < len(text):
         final_chunks.append(text[start_ndx:])
 
         return final_chunks
+
+
+class SmartRChunker(SmartChunker):
+    """
+    A chunker similar to SmartChunker, but does the chunking in reverse.
+    This is useful for wanting the splits to begin with the delimiters instead of ending.
+    """
+
+    def __init__(
+        self,
+        encoder,
+        chunk_size: int,
+        overlap_factor: float,
+        delimiters_tolerances_overlap: Optional[List[Tuple[str, float, bool]]
+        ] = None,
+    ) -> None:
+        """
+        :param encoder: The text encoder object.
+        :param chunk_size: The desired chunk size in token units.
+        :param overlap_factor: The factor to calculate the overlap between chunks.
+        :param delimiters_tolerances_overlap: A list of tuples with delimiter,
+            tolerance, and overlap values for smart chunking. Defaults to None.
+        """
+        super().__init__(
+            encoder,
+            chunk_size,
+            overlap_factor,
+            delimiters_tolerances_overlap=delimiters_tolerances_overlap,
+        )
+        self._delimiters_tolerances_overlap = [
+            (delimiter[::-1], tolerance, overlap)
+            for delimiter, tolerance, overlap in self._delimiters_tolerances_overlap
+        ]
+
+    def chunk(self, text: str) -> List[str]:
+        """
+        Chunks text respecting delimiters, tolerances, and overlap into chunk_size
+        (estimated token units) with overlap.
+
+        :param text: The input text to be chunked.
+        :returns: A list of chunked text.
+        """
+        reversed_text = text[::-1]
+
+        token_chunk_size = self.chunk_size
+        chunk_size = self.chunk_size * 4  # estimate token size
+
+        final_chunks = []
+
+        start_ndx = 0
+        while start_ndx + chunk_size < len(text):
+            best_chunk_end_ndx = start_ndx
+
+            for delimiter, tolerance, overlap in self._delimiters_tolerances_overlap:
+                search_start = start_ndx + int(chunk_size * (1 - tolerance))
+                search_end = start_ndx + chunk_size
+                delimiter_ndx = text[search_start:search_end].rfind(delimiter)
+
+                if delimiter_ndx != -1:
+                    best_chunk_end_ndx = delimiter_ndx + search_start
+                    break
+
+            chunk = text[start_ndx:best_chunk_end_ndx]
+
+            # Make sure chunk is actually smaller than chunk_size after the fact
+            # may not lead to best results if truncation is needed
+            encoded_chunk = self.encoder.encode(chunk[::-1])
+            if len(encoded_chunk) > token_chunk_size:
+                print("chunk too large, truncating")
+                encoded_chunk = encoded_chunk[:token_chunk_size]
+                trunc_chunk = self.encoder.decode(encoded_chunk)
+                best_chunk_end_ndx -= len(chunk) - len(trunc_chunk)
+                chunk = trunc_chunk[::-1]
+
+            final_chunks.append(chunk)
+
+            start_ndx = best_chunk_end_ndx
+            if overlap:
+                overlap_offset = int(self.overlap_factor * chunk_size)
+                ndx = text[start_ndx - overlap_offset : start_ndx].find(" ")
+                if ndx != -1:
+                    start_ndx += ndx - overlap_offset
+        # if start_ndx < len(text):
+        final_chunks.append(text[start_ndx:])
+
+        final_chunks = [chunk[::-1] for chunk in final_chunks]
+        return final_chunks
```

### Comparing `spiralflow-0.0.4/spiralflow/flow.py` & `spiralflow-0.0.5/spiralflow/flow.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.4/spiralflow/loading.py` & `spiralflow-0.0.5/spiralflow/loading.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         """
         with open(filepath, "r", encoding=self.encoding) as file:
             content = file.read()
 
         return self.handle_chunking([{"content": content, "path": filepath}])
 
 
-class PDFLoader(TextLoader):
+class PDFLoader(Loader):
     """
     PDFLoader that uses fitz (PyMuPDF) to load PDF files.
     """
 
     def load(self, filepath: str) -> List[Dict[str, Any]]:
         """
         :param filepath: Path to the PDF file to be loaded.
@@ -67,15 +67,15 @@
         """
         doc = fitz.open(filepath)
         pages = []
 
         for page in doc:
             pages.append(
                 {
-                    "content": page.get_text().encode(self.encoding),
+                    "content": page.get_text(),
                     "path": filepath,
                     "page_number": page.number,
                 }
             )
 
         return self.handle_chunking(pages)
 
@@ -86,15 +86,15 @@
     """
 
     def load(self, filepath: str) -> List[Dict[str, Any]]:
         """
         :param filepath: Path to the HTML file to be loaded.
         :return: Dictionary containing the path to the file, its content, and the soup title.
         """
-        with open(filepath, "r", encoding=self.encoding) as file:
+        with open(filepath, "r", encoding="utf-8") as file:
             content = file.read()
 
         soup = BeautifulSoup(content, "html.parser")
 
         return self.handle_chunking(
             [
                 {
```

### Comparing `spiralflow-0.0.4/spiralflow/memory.py` & `spiralflow-0.0.5/spiralflow/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         else:
             self.filepath = filepath
             self.load()
 
     def _create_index(self, embeddings: np.ndarray) -> None:
         _, d = embeddings.shape
         self.index = faiss.IndexFlatL2(d)
-        self.index.add(embeddings)
+        self.index.add(embeddings.astype(np.float32))
 
     def save(self, filepath: Optional[str] = None) -> None:
         """
         Saves the memory to a file.
         :param filepath: Path to the pickle file to save the memory to. If None, the filepath passed in the constructor is used.
         """
         if filepath is None:
@@ -138,15 +138,15 @@
         """
         if self.data.empty:
             raise ValueError(
                 "No memory to query. Add data to memory by calling Memory.add() before querying."
             )
 
         # get embedding of query
-        embeded_query = np.array([get_embedding(query, engine=self.embedding_model)])
+        embeded_query = np.array([get_embedding(query, engine=self.embedding_model)], dtype=np.float32)
 
         # search for the indexes with similar embeddings
         scores, similar_indexes = self.index.search(embeded_query, k=k)
 
         # get the memory values at the found indexes
         memories = []
```

### Comparing `spiralflow-0.0.4/spiralflow/message.py` & `spiralflow-0.0.5/spiralflow/message.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.4/spiralflow/tools.py` & `spiralflow-0.0.5/spiralflow/tools.py`

 * *Files identical despite different names*

### Comparing `spiralflow-0.0.4/spiralflow.egg-info/PKG-INFO` & `spiralflow-0.0.5/spiralflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiralflow
-Version: 0.0.4
+Version: 0.0.5
 Summary: A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.
 Home-page: https://github.com/Tiger767/Spiralflow
 Author: Travis Hammond
 License: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


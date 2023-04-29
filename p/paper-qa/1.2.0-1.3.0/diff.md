# Comparing `tmp/paper-qa-1.2.0.tar.gz` & `tmp/paper-qa-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-1.2.0.tar", last modified: Thu Apr 27 07:47:24 2023, max compression
+gzip compressed data, was "paper-qa-1.3.0.tar", last modified: Sat Apr 29 19:10:37 2023, max compression
```

## Comparing `paper-qa-1.2.0.tar` & `paper-qa-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:47:24.859447 paper-qa-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 07:46:47.000000 paper-qa-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-27 07:47:24.859447 paper-qa-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-04-27 07:46:47.000000 paper-qa-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:47:24.855447 paper-qa-1.2.0/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-27 07:47:24.000000 paper-qa-1.2.0/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-27 07:47:24.000000 paper-qa-1.2.0/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 07:47:24.000000 paper-qa-1.2.0/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-27 07:47:24.000000 paper-qa-1.2.0/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 07:47:24.000000 paper-qa-1.2.0/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:47:24.855447 paper-qa-1.2.0/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:47:24.859447 paper-qa-1.2.0/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    17104 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 07:46:47.000000 paper-qa-1.2.0/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 07:47:24.859447 paper-qa-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-27 07:46:47.000000 paper-qa-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:47:24.859447 paper-qa-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-04-27 07:46:47.000000 paper-qa-1.2.0/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:10:37.070681 paper-qa-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-29 19:09:49.000000 paper-qa-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-29 19:10:37.070681 paper-qa-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-04-29 19:09:49.000000 paper-qa-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:10:37.070681 paper-qa-1.3.0/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-29 19:10:37.000000 paper-qa-1.3.0/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-29 19:10:37.000000 paper-qa-1.3.0/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 19:10:37.000000 paper-qa-1.3.0/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-29 19:10:37.000000 paper-qa-1.3.0/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-29 19:10:37.000000 paper-qa-1.3.0/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:10:37.070681 paper-qa-1.3.0/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:10:37.070681 paper-qa-1.3.0/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17793 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/qaprompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-29 19:09:49.000000 paper-qa-1.3.0/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 19:10:37.070681 paper-qa-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-29 19:09:49.000000 paper-qa-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:10:37.070681 paper-qa-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-29 19:09:49.000000 paper-qa-1.3.0/tests/test_paperqa.py
```

### Comparing `paper-qa-1.2.0/PKG-INFO` & `paper-qa-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.2.0
+Version: 1.3.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -264,7 +264,11 @@
 with open("my_docs.pkl", "wb") as f:
     pickle.dump(docs, f)
 
 # load
 with open("my_docs.pkl", "rb") as f:
     docs = pickle.load(f)
 ```
+
+### Callbacks
+
+TODO
```

### Comparing `paper-qa-1.2.0/README.md` & `paper-qa-1.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -250,7 +250,11 @@
 with open("my_docs.pkl", "wb") as f:
     pickle.dump(docs, f)
 
 # load
 with open("my_docs.pkl", "rb") as f:
     docs = pickle.load(f)
 ```
+
+### Callbacks
+
+TODO
```

### Comparing `paper-qa-1.2.0/paper_qa.egg-info/PKG-INFO` & `paper-qa-1.3.0/paper_qa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.2.0
+Version: 1.3.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -264,7 +264,11 @@
 with open("my_docs.pkl", "wb") as f:
     pickle.dump(docs, f)
 
 # load
 with open("my_docs.pkl", "rb") as f:
     docs = pickle.load(f)
 ```
+
+### Callbacks
+
+TODO
```

### Comparing `paper-qa-1.2.0/paperqa/agent.py` & `paper-qa-1.3.0/paperqa/agent.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.2.0/paperqa/contrib/zotero.py` & `paper-qa-1.3.0/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.2.0/paperqa/docs.py` & `paper-qa-1.3.0/paperqa/docs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Tuple, Union, Callable
 from functools import reduce
 import os
 import sys
 import asyncio
 from pathlib import Path
 import re
 from .paths import CACHE_PATH
@@ -14,19 +14,21 @@
     citation_prompt,
     select_paper_prompt,
     make_chain,
 )
 from .types import Answer, Context
 from .readers import read_doc
 from langchain.vectorstores import FAISS
+from langchain.docstore.document import Document
 from langchain.embeddings.openai import OpenAIEmbeddings
 from langchain.embeddings.base import Embeddings
 from langchain.chat_models import ChatOpenAI
 from langchain.llms.base import LLM
-from langchain.callbacks import get_openai_callback
+from langchain.callbacks import get_openai_callback, OpenAICallbackHandler
+from langchain.callbacks.base import AsyncCallbackHandler, AsyncCallbackManager
 from langchain.cache import SQLiteCache
 import langchain
 from datetime import datetime
 
 os.makedirs(os.path.dirname(CACHE_PATH), exist_ok=True)
 langchain.llm_cache = SQLiteCache(CACHE_PATH)
 
@@ -38,37 +40,41 @@
         self,
         chunk_size_limit: int = 3000,
         llm: Optional[Union[LLM, str]] = None,
         summary_llm: Optional[Union[LLM, str]] = None,
         name: str = "default",
         index_path: Optional[Path] = None,
         embeddings: Optional[Embeddings] = None,
+        get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x : []
     ) -> None:
         """Initialize the collection of documents.
 
         Args:
             chunk_size_limit: The maximum number of characters to use for a single chunk of text.
             llm: The language model to use for answering questions. Default - OpenAI chat-gpt-turbo
             summary_llm: The language model to use for summarizing documents. If None, llm is used.
             name: The name of the collection.
             index_path: The path to the index file IF pickled. If None, defaults to using name in $HOME/.paperqa/name
+            embeddings: The embeddings to use for indexing documents. Default - OpenAI embeddings
+            get_callbacks: A function that allows callbacks to built per stage of the pipeline.
         """
         self.docs = dict()
         self.chunk_size_limit = chunk_size_limit
         self.keys = set()
         self._faiss_index = None
         self._doc_index = None
         self.update_llm(llm, summary_llm)
         if index_path is None:
             index_path = Path.home() / ".paperqa" / name
         self.index_path = index_path
         self.name = name
         if embeddings is None:
             embeddings = OpenAIEmbeddings()
         self.embeddings = embeddings
+        self.get_callbacks = get_callbacks
 
     def update_llm(
         self,
         llm: Optional[Union[LLM, str]] = None,
         summary_llm: Optional[Union[LLM, str]] = None,
     ) -> None:
         """Update the LLM for answering questions."""
@@ -78,18 +84,14 @@
             llm = ChatOpenAI(temperature=0.1, model=llm)
         if type(summary_llm) is str:
             summary_llm = ChatOpenAI(temperature=0.1, model=summary_llm)
         self.llm = llm
         if summary_llm is None:
             summary_llm = llm
         self.summary_llm = summary_llm
-        self.summary_chain = make_chain(prompt=summary_prompt, llm=summary_llm)
-        self.qa_chain = make_chain(prompt=qa_prompt, llm=llm)
-        self.search_chain = make_chain(prompt=search_prompt, llm=summary_llm)
-        self.cite_chain = make_chain(prompt=citation_prompt, llm=summary_llm)
 
     def add(
         self,
         path: str,
         citation: Optional[str] = None,
         key: Optional[str] = None,
         disable_check: bool = False,
@@ -101,18 +103,19 @@
         # first check to see if we already have this document
         # this way we don't make api call to create citation on file we already have
         md5 = md5sum(path)
         if path in self.docs:
             raise ValueError(f"Document {path} already in collection.")
 
         if citation is None:
+            cite_chain = make_chain(prompt=citation_prompt, llm=self.summary_llm)
             # peak first chunk
             texts, _ = read_doc(path, "", "", chunk_chars=chunk_chars)
             with get_openai_callback():
-                citation = self.cite_chain.run(texts[0])
+                citation = cite_chain.run(texts[0])
             if len(citation) < 3 or "Unknown" in citation or "insufficient" in citation:
                 citation = f"Unknown, {os.path.basename(path)}, {datetime.now().year}"
 
         if key is None:
             # get first name and year from citation
             try:
                 author = re.search(r"([A-Z][a-z]+)", citation).group(1)
@@ -200,23 +203,20 @@
         if self._faiss_index is None and len(self.docs) > 0:
             self._build_faiss_index()
         state = self.__dict__.copy()
         if self._faiss_index is not None:
             state["_faiss_index"].save_local(self.index_path)
         del state["_faiss_index"]
         del state["_doc_index"]
-        # remove LLMs (they can have callbacks, which can't be pickled)
-        del state["summary_chain"]
-        del state["qa_chain"]
-        del state["cite_chain"]
-        del state["search_chain"]
+        del state["get_callbacks"]
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
+        self.get_callbacks = lambda x: []
         try:
             self._faiss_index = FAISS.load_local(self.index_path, self.embeddings)
         except:
             # they use some special exception type, but I don't want to import it
             self._faiss_index = None
         if not hasattr(self, "_doc_index"):
             self._doc_index = None
@@ -236,16 +236,16 @@
 
     def get_evidence(
         self,
         answer: Answer,
         k: int = 3,
         max_sources: int = 5,
         marginal_relevance: bool = True,
-        key_filter: Optional[List[str]] = None,
-    ) -> Answer:
+        key_filter: Optional[List[str]] = None    
+        ) -> Answer:
         # special case for jupyter notebooks
         if "get_ipython" in globals() or "google.colab" in sys.modules:
             import nest_asyncio
 
             nest_asyncio.apply()
         try:
             loop = asyncio.get_event_loop()
@@ -254,15 +254,15 @@
             asyncio.set_event_loop(loop)
         return loop.run_until_complete(
             self.aget_evidence(
                 answer,
                 k=k,
                 max_sources=max_sources,
                 marginal_relevance=marginal_relevance,
-                key_filter=key_filter,
+                key_filter=key_filter
             )
         )
 
     async def aget_evidence(
         self,
         answer: Answer,
         k: int = 3,
@@ -285,37 +285,41 @@
         else:
             docs = self._faiss_index.similarity_search(
                 answer.question, k=_k, fetch_k=5 * _k
             )
 
         async def process(doc):
             if key_filter is not None and doc.metadata["dockey"] not in key_filter:
-                return None
+                return None, None
             # check if it is already in answer (possible in agent setting)
             if doc.metadata["key"] in [c.key for c in answer.contexts]:
-                return None
+                return None, None
+            cb = OpenAICallbackHandler()
+            manager = AsyncCallbackManager([cb] + self.get_callbacks('evidence:' + doc.metadata['key']))
+            summary_chain = make_chain(summary_prompt, self.summary_llm, manager)
             c = Context(
                 key=doc.metadata["key"],
                 citation=doc.metadata["citation"],
-                context=await self.summary_chain.arun(
+                context=await summary_chain.arun(
                     question=answer.question,
                     context_str=doc.page_content,
                     citation=doc.metadata["citation"],
                 ),
                 text=doc.page_content,
             )
             if "Not applicable" not in c.context:
-                return c
-            return None
+                return c, cb
+            return None, None
 
-        with get_openai_callback() as cb:
-            contexts = await asyncio.gather(*[process(doc) for doc in docs])
-        answer.tokens += cb.total_tokens
-        answer.cost += cb.total_cost
-        contexts = [c for c in contexts if c is not None]
+        results = await asyncio.gather(*[process(doc) for doc in docs])
+        # filter out failures
+        results = [r for r in results if r[0] is not None]
+        answer.tokens += sum([cb.total_tokens for _, cb in results])
+        answer.cost += sum([cb.total_cost for _, cb in results])
+        contexts = [c for c,_ in results if c is not None]
         if len(contexts) == 0:
             return answer
         contexts = sorted(contexts, key=lambda x: len(x.context), reverse=True)
         contexts = contexts[:max_sources]
         # add to answer (if not already there)
         keys = [c.key for c in answer.contexts]
         for c in contexts:
@@ -341,15 +345,16 @@
         """Generate a list of search strings that can be used to find
         relevant papers.
 
         Args:
             query (str): The query to generate search strings for.
         """
 
-        search_query = self.search_chain.run(question=query)
+        search_chain = make_chain(prompt=search_prompt, llm=self.summary_llm)
+        search_query = search_chain.run(question=query)
         queries = [s for s in search_query.split("\n") if len(s) > 3]
         # remove 2., 3. from queries
         queries = [re.sub(r"^\d+\.\s*", "", q) for q in queries]
         return queries
 
     def query(
         self,
@@ -414,16 +419,18 @@
         bib = dict()
         passages = dict()
         if len(context_str) < 10:
             answer_text = (
                 "I cannot answer this question due to insufficient information."
             )
         else:
-            with get_openai_callback() as cb:
-                answer_text = await self.qa_chain.arun(
+            cb = OpenAICallbackHandler()
+            manager = AsyncCallbackManager([cb] + self.get_callbacks('answer'))
+            qa_chain = make_chain(qa_prompt, self.llm, manager)
+            answer_text = await qa_chain.arun(
                     question=query, context_str=context_str, length=length_prompt
                 )
             answer.tokens += cb.total_tokens
             answer.cost += cb.total_cost
         # it still happens lol
         if "(Foo2012)" in answer_text:
             answer_text = answer_text.replace("(Foo2012)", "")
```

### Comparing `paper-qa-1.2.0/paperqa/qaprompts.py` & `paper-qa-1.3.0/paperqa/qaprompts.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import langchain.prompts as prompts
 from datetime import datetime
 from langchain.chains import LLMChain
 from langchain.chat_models import ChatOpenAI
 from langchain.schema import SystemMessage
 from langchain.prompts.chat import HumanMessagePromptTemplate, ChatPromptTemplate
 
-
 summary_prompt = prompts.PromptTemplate(
     input_variables=["question", "context_str", "citation"],
     template="Summarize and provide direct quotes from the text below to help answer a question. "
     "Do not directly answer the question, instead summarize and "
     "quote to give evidence to help answer the question. "
     "Do not use outside sources. "
     'Reply with "Not applicable" if the text is unrelated to the question. '
@@ -70,16 +69,19 @@
     input_variables=["text"],
     template="Provide a possible citation for the following text in MLA Format. Today's date is {date}\n"
     "{text}\n\n"
     "Citation:",
     partial_variables={"date": _get_datetime},
 )
 
-
-def make_chain(prompt, llm):
+def make_chain(prompt, llm, callback_manager=None):
+    if callback_manager is not None:
+        # need to clone to attach
+        llm = llm.copy()
+        llm.callback_manager = callback_manager
     if type(llm) == ChatOpenAI:
         system_message_prompt = SystemMessage(
             content="You are a scholarly researcher that answers in an unbiased, scholarly tone. "
             "You sometimes refuse to answer if there is insufficient information.",
         )
         human_message_prompt = HumanMessagePromptTemplate(prompt=prompt)
         prompt = ChatPromptTemplate.from_messages(
```

### Comparing `paper-qa-1.2.0/paperqa/readers.py` & `paper-qa-1.3.0/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.2.0/paperqa/types.py` & `paper-qa-1.3.0/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.2.0/paperqa/utils.py` & `paper-qa-1.3.0/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.2.0/setup.py` & `paper-qa-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.2.0/tests/test_paperqa.py` & `paper-qa-1.3.0/tests/test_paperqa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import paperqa
 import requests
 import os
 import pickle
 from paperqa.utils import strings_similarity
 from langchain.llms import OpenAI
+from langchain.llms.fake import FakeListLLM
 from unittest import IsolatedAsyncioTestCase
 
 
 def test_maybe_is_text():
     assert paperqa.maybe_is_text(
         "This is a test. The sample conc. was 1.0 mM (at 245 ^F)"
     )
@@ -248,22 +249,33 @@
         "Information about Fredrick Bates, WikiMedia Foundation, 2023, Accessed now",
     )
     # add with new dockey
     docs.add("example.txt", "WikiMedia Foundation, 2023, Accessed now", key="test")
     answer = docs.query("What country is Bates from?", key_filter=True)
     # the filter shouldn't trigger, so just checking that it doesn't crash
 
+def test_nonopenai_model():
+    responses = ["This is a test", "This is another test"]
+    model = FakeListLLM(responses=responses)
+    doc_path = "example.txt"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get wiki page about politician
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        f.write(r.text)
+    docs = paperqa.Docs(llm=model)
+    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
+    answer = docs.query("What country is Bates from?")
 
-def disabled_test_agent():
+def test_agent():
     docs = paperqa.Docs()
     answer = paperqa.run_agent(docs, "What compounds target AKT1")
     print(answer)
 
 def test_zotera():
     from paperqa.contrib import ZoteroDB
 
     docs = paperqa.Docs()
     try:
         zotero = ZoteroDB(library_type="user")  # "group" if group library
     except ValueError:
         # close enough
-        return
+        return
```


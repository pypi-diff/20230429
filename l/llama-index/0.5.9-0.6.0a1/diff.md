# Comparing `tmp/llama_index-0.5.9.tar.gz` & `tmp/llama_index-0.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index-0.5.9.tar", last modified: Thu Apr  6 17:13:08 2023, max compression
+gzip compressed data, was "llama_index-0.6.0a1.tar", last modified: Fri Apr 28 21:55:20 2023, max compression
```

## Comparing `llama_index-0.5.9.tar` & `llama_index-0.6.0a1.tar`

### file list

```diff
@@ -1,259 +1,299 @@
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.211702 llama_index-0.5.9/
--rw-r--r--   0 suo        (501) staff       (20)     1064 2023-04-06 17:13:07.000000 llama_index-0.5.9/LICENSE
--rw-r--r--   0 suo        (501) staff       (20)       73 2023-04-06 17:13:07.000000 llama_index-0.5.9/MANIFEST.in
--rw-r--r--   0 suo        (501) staff       (20)     4449 2023-04-06 17:13:08.211372 llama_index-0.5.9/PKG-INFO
--rw-r--r--   0 suo        (501) staff       (20)     4221 2023-04-06 17:13:07.000000 llama_index-0.5.9/README.md
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.157193 llama_index-0.5.9/llama_index/
--rw-r--r--   0 suo        (501) staff       (20)        6 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/VERSION
--rw-r--r--   0 suo        (501) staff       (20)     4468 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)      322 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/async_utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.159590 llama_index-0.5.9/llama_index/composability/
--rw-r--r--   0 suo        (501) staff       (20)      220 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/composability/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)      171 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/composability/base.py
--rw-r--r--   0 suo        (501) staff       (20)     2654 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/composability/joint_qa_summary.py
--rw-r--r--   0 suo        (501) staff       (20)      277 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/constants.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.161752 llama_index-0.5.9/llama_index/data_structs/
--rw-r--r--   0 suo        (501) staff       (20)      373 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/data_structs/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)    12377 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/data_structs/data_structs.py
--rw-r--r--   0 suo        (501) staff       (20)    12269 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/data_structs/data_structs_v2.py
--rw-r--r--   0 suo        (501) staff       (20)     4748 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/data_structs/node_v2.py
--rw-r--r--   0 suo        (501) staff       (20)     2669 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/data_structs/struct_type.py
--rw-r--r--   0 suo        (501) staff       (20)      908 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/data_structs/table.py
--rw-r--r--   0 suo        (501) staff       (20)     1032 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/data_structs/table_v2.py
--rw-r--r--   0 suo        (501) staff       (20)     7415 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/docstore.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.163201 llama_index-0.5.9/llama_index/embeddings/
--rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/embeddings/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     7650 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/embeddings/base.py
--rw-r--r--   0 suo        (501) staff       (20)      934 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/embeddings/langchain.py
--rw-r--r--   0 suo        (501) staff       (20)    10103 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/embeddings/openai.py
--rw-r--r--   0 suo        (501) staff       (20)      559 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/embeddings/utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.163751 llama_index-0.5.9/llama_index/evaluation/
--rw-r--r--   0 suo        (501) staff       (20)      118 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/evaluation/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     4409 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/evaluation/base.py
--rw-r--r--   0 suo        (501) staff       (20)      544 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/img_utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.165499 llama_index-0.5.9/llama_index/indices/
--rw-r--r--   0 suo        (501) staff       (20)      542 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)    15287 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/base.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.165775 llama_index-0.5.9/llama_index/indices/common/
--rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/common/__init__.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.166860 llama_index-0.5.9/llama_index/indices/common/struct_store/
--rw-r--r--   0 suo        (501) staff       (20)       19 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/common/struct_store/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     8107 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/common/struct_store/base.py
--rw-r--r--   0 suo        (501) staff       (20)      776 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/common/struct_store/schema.py
--rw-r--r--   0 suo        (501) staff       (20)     2629 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/common/struct_store/sql.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.167399 llama_index-0.5.9/llama_index/indices/common_tree/
--rw-r--r--   0 suo        (501) staff       (20)       19 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/common_tree/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     7146 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/common_tree/base.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.168222 llama_index-0.5.9/llama_index/indices/composability/
--rw-r--r--   0 suo        (501) staff       (20)      180 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/composability/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)    10585 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/composability/graph.py
--rw-r--r--   0 suo        (501) staff       (20)     2382 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/composability/utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.169141 llama_index-0.5.9/llama_index/indices/empty/
--rw-r--r--   0 suo        (501) staff       (20)      202 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/empty/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     2158 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/empty/base.py
--rw-r--r--   0 suo        (501) staff       (20)     2178 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/empty/query.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.170793 llama_index-0.5.9/llama_index/indices/keyword_table/
--rw-r--r--   0 suo        (501) staff       (20)      645 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/keyword_table/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     7054 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/keyword_table/base.py
--rw-r--r--   0 suo        (501) staff       (20)     6271 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/keyword_table/query.py
--rw-r--r--   0 suo        (501) staff       (20)      650 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/keyword_table/rake_base.py
--rw-r--r--   0 suo        (501) staff       (20)      844 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/keyword_table/simple_base.py
--rw-r--r--   0 suo        (501) staff       (20)     2264 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/keyword_table/utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.171611 llama_index-0.5.9/llama_index/indices/knowledge_graph/
--rw-r--r--   0 suo        (501) staff       (20)      279 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     8029 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 suo        (501) staff       (20)     9601 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/knowledge_graph/query.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.172721 llama_index-0.5.9/llama_index/indices/list/
--rw-r--r--   0 suo        (501) staff       (20)      325 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/list/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     3611 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/list/base.py
--rw-r--r--   0 suo        (501) staff       (20)     3089 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/list/embedding_query.py
--rw-r--r--   0 suo        (501) staff       (20)     1539 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/list/query.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.173536 llama_index-0.5.9/llama_index/indices/postprocessor/
--rw-r--r--   0 suo        (501) staff       (20)      457 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/postprocessor/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)       83 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/postprocessor/base.py
--rw-r--r--   0 suo        (501) staff       (20)    11871 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/postprocessor/node.py
--rw-r--r--   0 suo        (501) staff       (20)     8464 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/prompt_helper.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.174860 llama_index-0.5.9/llama_index/indices/query/
--rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/query/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)    14869 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/query/base.py
--rw-r--r--   0 suo        (501) staff       (20)     2581 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/query/embedding_utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.175855 llama_index-0.5.9/llama_index/indices/query/query_combiner/
--rw-r--r--   0 suo        (501) staff       (20)      140 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/query/query_combiner/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     8753 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/query/query_combiner/base.py
--rw-r--r--   0 suo        (501) staff       (20)       30 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/query/query_combiner/prompts.py
--rw-r--r--   0 suo        (501) staff       (20)    13263 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/query/query_runner.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.176660 llama_index-0.5.9/llama_index/indices/query/query_transform/
--rw-r--r--   0 suo        (501) staff       (20)      281 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/query/query_transform/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     9145 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/query/query_transform/base.py
--rw-r--r--   0 suo        (501) staff       (20)     5920 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/query/query_transform/prompts.py
--rw-r--r--   0 suo        (501) staff       (20)     4834 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/query/schema.py
--rw-r--r--   0 suo        (501) staff       (20)     4045 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/registry.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.177175 llama_index-0.5.9/llama_index/indices/response/
--rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/response/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)    15585 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/response/builder.py
--rw-r--r--   0 suo        (501) staff       (20)     3310 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/service_context.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.178881 llama_index-0.5.9/llama_index/indices/struct_store/
--rw-r--r--   0 suo        (501) staff       (20)      616 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/struct_store/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     2115 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/struct_store/base.py
--rw-r--r--   0 suo        (501) staff       (20)     5765 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/struct_store/container_builder.py
--rw-r--r--   0 suo        (501) staff       (20)     2624 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/struct_store/pandas.py
--rw-r--r--   0 suo        (501) staff       (20)     4755 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/struct_store/pandas_query.py
--rw-r--r--   0 suo        (501) staff       (20)     8059 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/struct_store/sql.py
--rw-r--r--   0 suo        (501) staff       (20)     6674 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/struct_store/sql_query.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.180512 llama_index-0.5.9/llama_index/indices/tree/
--rw-r--r--   0 suo        (501) staff       (20)      460 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/tree/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     5179 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/tree/base.py
--rw-r--r--   0 suo        (501) staff       (20)     5493 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/tree/embedding_query.py
--rw-r--r--   0 suo        (501) staff       (20)     7034 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/tree/inserter.py
--rw-r--r--   0 suo        (501) staff       (20)    14258 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/tree/leaf_query.py
--rw-r--r--   0 suo        (501) staff       (20)     1798 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/tree/retrieve_query.py
--rw-r--r--   0 suo        (501) staff       (20)     2229 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/tree/summarize_query.py
--rw-r--r--   0 suo        (501) staff       (20)     2005 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.181398 llama_index-0.5.9/llama_index/indices/vector_store/
--rw-r--r--   0 suo        (501) staff       (20)      720 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/vector_store/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)    10348 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/vector_store/base.py
--rw-r--r--   0 suo        (501) staff       (20)     3782 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/vector_store/base_query.py
--rw-r--r--   0 suo        (501) staff       (20)    17152 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/indices/vector_store/vector_indices.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.182799 llama_index-0.5.9/llama_index/langchain_helpers/
--rw-r--r--   0 suo        (501) staff       (20)       39 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/langchain_helpers/__init__.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.183971 llama_index-0.5.9/llama_index/langchain_helpers/agents/
--rw-r--r--   0 suo        (501) staff       (20)      555 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/langchain_helpers/agents/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     2989 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/langchain_helpers/agents/agents.py
--rw-r--r--   0 suo        (501) staff       (20)     1132 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/langchain_helpers/agents/toolkits.py
--rw-r--r--   0 suo        (501) staff       (20)     3001 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/langchain_helpers/agents/tools.py
--rw-r--r--   0 suo        (501) staff       (20)      252 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/langchain_helpers/chain_wrapper.py
--rw-r--r--   0 suo        (501) staff       (20)     7571 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/langchain_helpers/memory_wrapper.py
--rw-r--r--   0 suo        (501) staff       (20)     3299 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/langchain_helpers/sql_wrapper.py
--rw-r--r--   0 suo        (501) staff       (20)    17458 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/langchain_helpers/text_splitter.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.184997 llama_index-0.5.9/llama_index/llm_predictor/
--rw-r--r--   0 suo        (501) staff       (20)      254 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/llm_predictor/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)    10593 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/llm_predictor/base.py
--rw-r--r--   0 suo        (501) staff       (20)     4275 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/llm_predictor/chatgpt.py
--rw-r--r--   0 suo        (501) staff       (20)     2274 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/llm_predictor/structured.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.185680 llama_index-0.5.9/llama_index/logger/
--rw-r--r--   0 suo        (501) staff       (20)       95 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/logger/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)      995 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/logger/base.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.186773 llama_index-0.5.9/llama_index/node_parser/
--rw-r--r--   0 suo        (501) staff       (20)      184 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/node_parser/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)      530 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/node_parser/interface.py
--rw-r--r--   0 suo        (501) staff       (20)     3606 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/node_parser/node_utils.py
--rw-r--r--   0 suo        (501) staff       (20)     1856 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/node_parser/simple.py
--rw-r--r--   0 suo        (501) staff       (20)     4984 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/old_docstore.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.187243 llama_index-0.5.9/llama_index/optimization/
--rw-r--r--   0 suo        (501) staff       (20)      144 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/optimization/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     4248 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/optimization/optimizer.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.188171 llama_index-0.5.9/llama_index/output_parsers/
--rw-r--r--   0 suo        (501) staff       (20)      230 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/output_parsers/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)      611 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/output_parsers/base.py
--rw-r--r--   0 suo        (501) staff       (20)     2742 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/output_parsers/guardrails.py
--rw-r--r--   0 suo        (501) staff       (20)     1828 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/output_parsers/langchain.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.188630 llama_index-0.5.9/llama_index/playground/
--rw-r--r--   0 suo        (501) staff       (20)      202 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/playground/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     5637 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/playground/base.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.190240 llama_index-0.5.9/llama_index/prompts/
--rw-r--r--   0 suo        (501) staff       (20)       87 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/prompts/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     6626 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/prompts/base.py
--rw-r--r--   0 suo        (501) staff       (20)     1969 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/prompts/chat_prompts.py
--rw-r--r--   0 suo        (501) staff       (20)     1134 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/prompts/default_prompt_selectors.py
--rw-r--r--   0 suo        (501) staff       (20)    10843 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/prompts/default_prompts.py
--rw-r--r--   0 suo        (501) staff       (20)      992 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/prompts/prompt_type.py
--rw-r--r--   0 suo        (501) staff       (20)     7685 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/prompts/prompts.py
--rw-r--r--   0 suo        (501) staff       (20)        0 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/py.typed
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.195649 llama_index-0.5.9/llama_index/readers/
--rw-r--r--   0 suo        (501) staff       (20)     2749 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)      659 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/base.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.196182 llama_index-0.5.9/llama_index/readers/chatgpt_plugin/
--rw-r--r--   0 suo        (501) staff       (20)      145 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/chatgpt_plugin/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     2111 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/chatgpt_plugin/base.py
--rw-r--r--   0 suo        (501) staff       (20)     3895 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/chroma.py
--rw-r--r--   0 suo        (501) staff       (20)     3328 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/database.py
--rw-r--r--   0 suo        (501) staff       (20)     4981 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/discord_reader.py
--rw-r--r--   0 suo        (501) staff       (20)     7413 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/download.py
--rw-r--r--   0 suo        (501) staff       (20)     2392 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/elasticsearch.py
--rw-r--r--   0 suo        (501) staff       (20)     2478 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/faiss.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.199072 llama_index-0.5.9/llama_index/readers/file/
--rw-r--r--   0 suo        (501) staff       (20)       19 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/file/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     8436 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/file/base.py
--rw-r--r--   0 suo        (501) staff       (20)     1342 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/file/base_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     1629 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/file/docs_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     1318 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/file/epub_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     4106 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/file/image_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     3616 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/file/markdown_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     3162 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/file/mbox_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     3945 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/file/slides_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     3357 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/file/tabular_parser.py
--rw-r--r--   0 suo        (501) staff       (20)     1770 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/file/video_audio.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.200089 llama_index-0.5.9/llama_index/readers/github_readers/
--rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/github_readers/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)    11686 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/github_readers/github_api_client.py
--rw-r--r--   0 suo        (501) staff       (20)    15928 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/github_readers/github_repository_reader.py
--rw-r--r--   0 suo        (501) staff       (20)     5473 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/github_readers/utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.200857 llama_index-0.5.9/llama_index/readers/google_readers/
--rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/google_readers/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     5659 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/google_readers/gdocs.py
--rw-r--r--   0 suo        (501) staff       (20)     4989 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/google_readers/gsheets.py
--rw-r--r--   0 suo        (501) staff       (20)     3708 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/json.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.201395 llama_index-0.5.9/llama_index/readers/make_com/
--rw-r--r--   0 suo        (501) staff       (20)       19 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/make_com/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     1696 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/make_com/wrapper.py
--rw-r--r--   0 suo        (501) staff       (20)     1261 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/mbox.py
--rw-r--r--   0 suo        (501) staff       (20)     2260 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/mongo.py
--rw-r--r--   0 suo        (501) staff       (20)     5679 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/notion.py
--rw-r--r--   0 suo        (501) staff       (20)     1601 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/obsidian.py
--rw-r--r--   0 suo        (501) staff       (20)     2766 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/pinecone.py
--rw-r--r--   0 suo        (501) staff       (20)     3279 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/qdrant.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.201931 llama_index-0.5.9/llama_index/readers/schema/
--rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/schema/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     1214 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/schema/base.py
--rw-r--r--   0 suo        (501) staff       (20)     7892 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/slack.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.202453 llama_index-0.5.9/llama_index/readers/steamship/
--rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/steamship/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     3498 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/steamship/file_reader.py
--rw-r--r--   0 suo        (501) staff       (20)      984 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/string_iterable.py
--rw-r--r--   0 suo        (501) staff       (20)     1918 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/twitter.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.203527 llama_index-0.5.9/llama_index/readers/weaviate/
--rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/weaviate/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     9784 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/weaviate/data_structs.py
--rw-r--r--   0 suo        (501) staff       (20)     3986 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/weaviate/reader.py
--rw-r--r--   0 suo        (501) staff       (20)     1867 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/weaviate/utils.py
--rw-r--r--   0 suo        (501) staff       (20)     7987 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/web.py
--rw-r--r--   0 suo        (501) staff       (20)      981 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/wikipedia.py
--rw-r--r--   0 suo        (501) staff       (20)     1255 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/readers/youtube_transcript.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.204720 llama_index-0.5.9/llama_index/response/
--rw-r--r--   0 suo        (501) staff       (20)       19 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/response/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     2039 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/response/notebook_utils.py
--rw-r--r--   0 suo        (501) staff       (20)     3135 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/response/schema.py
--rw-r--r--   0 suo        (501) staff       (20)      262 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/response/utils.py
--rw-r--r--   0 suo        (501) staff       (20)     2768 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/schema.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.206186 llama_index-0.5.9/llama_index/token_counter/
--rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/token_counter/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     4664 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/token_counter/mock_chain_wrapper.py
--rw-r--r--   0 suo        (501) staff       (20)      722 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/token_counter/mock_embed_model.py
--rw-r--r--   0 suo        (501) staff       (20)     2874 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/token_counter/token_counter.py
--rw-r--r--   0 suo        (501) staff       (20)      908 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/token_counter/utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.207038 llama_index-0.5.9/llama_index/tools/
--rw-r--r--   0 suo        (501) staff       (20)       13 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/tools/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)      723 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/tools/file_utils.py
--rw-r--r--   0 suo        (501) staff       (20)    11340 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/tools/migrate_v1_to_v2.py
--rw-r--r--   0 suo        (501) staff       (20)       81 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/types.py
--rw-r--r--   0 suo        (501) staff       (20)     5296 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/utils.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.210989 llama_index-0.5.9/llama_index/vector_stores/
--rw-r--r--   0 suo        (501) staff       (20)      859 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/vector_stores/__init__.py
--rw-r--r--   0 suo        (501) staff       (20)     5682 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/vector_stores/chatgpt_plugin.py
--rw-r--r--   0 suo        (501) staff       (20)     4408 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/vector_stores/chroma.py
--rw-r--r--   0 suo        (501) staff       (20)     4488 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/vector_stores/faiss.py
--rw-r--r--   0 suo        (501) staff       (20)     6886 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/vector_stores/opensearch.py
--rw-r--r--   0 suo        (501) staff       (20)     8805 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/vector_stores/pinecone.py
--rw-r--r--   0 suo        (501) staff       (20)     7164 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/vector_stores/qdrant.py
--rw-r--r--   0 suo        (501) staff       (20)     2568 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/vector_stores/registry.py
--rw-r--r--   0 suo        (501) staff       (20)     3649 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/vector_stores/simple.py
--rw-r--r--   0 suo        (501) staff       (20)     1647 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/vector_stores/types.py
--rw-r--r--   0 suo        (501) staff       (20)     4104 2023-04-06 17:13:07.000000 llama_index-0.5.9/llama_index/vector_stores/weaviate.py
-drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-06 17:13:08.158709 llama_index-0.5.9/llama_index.egg-info/
--rw-r--r--   0 suo        (501) staff       (20)     4449 2023-04-06 17:13:08.000000 llama_index-0.5.9/llama_index.egg-info/PKG-INFO
--rw-r--r--   0 suo        (501) staff       (20)     8021 2023-04-06 17:13:08.000000 llama_index-0.5.9/llama_index.egg-info/SOURCES.txt
--rw-r--r--   0 suo        (501) staff       (20)        1 2023-04-06 17:13:08.000000 llama_index-0.5.9/llama_index.egg-info/dependency_links.txt
--rw-r--r--   0 suo        (501) staff       (20)       87 2023-04-06 17:13:08.000000 llama_index-0.5.9/llama_index.egg-info/requires.txt
--rw-r--r--   0 suo        (501) staff       (20)       12 2023-04-06 17:13:08.000000 llama_index-0.5.9/llama_index.egg-info/top_level.txt
--rw-r--r--   0 suo        (501) staff       (20)       38 2023-04-06 17:13:08.211782 llama_index-0.5.9/setup.cfg
--rw-r--r--   0 suo        (501) staff       (20)     1121 2023-04-06 17:13:07.000000 llama_index-0.5.9/setup.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.258896 llama_index-0.6.0a1/
+-rw-r--r--   0 suo        (501) staff       (20)     1064 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/LICENSE
+-rw-r--r--   0 suo        (501) staff       (20)       73 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/MANIFEST.in
+-rw-r--r--   0 suo        (501) staff       (20)     4270 2023-04-28 21:55:20.258535 llama_index-0.6.0a1/PKG-INFO
+-rw-r--r--   0 suo        (501) staff       (20)     4040 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/README.md
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.160961 llama_index-0.6.0a1/llama_index/
+-rw-r--r--   0 suo        (501) staff       (20)       13 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/VERSION
+-rw-r--r--   0 suo        (501) staff       (20)     4500 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)      322 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/async_utils.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.164407 llama_index-0.6.0a1/llama_index/composability/
+-rw-r--r--   0 suo        (501) staff       (20)      220 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/composability/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)      171 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/composability/base.py
+-rw-r--r--   0 suo        (501) staff       (20)     2739 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/composability/joint_qa_summary.py
+-rw-r--r--   0 suo        (501) staff       (20)      345 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/constants.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.168073 llama_index-0.6.0a1/llama_index/data_structs/
+-rw-r--r--   0 suo        (501) staff       (20)      373 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/data_structs/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)    12377 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/data_structs/data_structs.py
+-rw-r--r--   0 suo        (501) staff       (20)     9476 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/data_structs/data_structs_v2.py
+-rw-r--r--   0 suo        (501) staff       (20)     6221 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/data_structs/node_v2.py
+-rw-r--r--   0 suo        (501) staff       (20)      779 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/data_structs/registry.py
+-rw-r--r--   0 suo        (501) staff       (20)     3256 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/data_structs/struct_type.py
+-rw-r--r--   0 suo        (501) staff       (20)      908 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/data_structs/table.py
+-rw-r--r--   0 suo        (501) staff       (20)     1032 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/data_structs/table_v2.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.170420 llama_index-0.6.0a1/llama_index/embeddings/
+-rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/embeddings/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     7721 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/embeddings/base.py
+-rw-r--r--   0 suo        (501) staff       (20)     1109 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/embeddings/langchain.py
+-rw-r--r--   0 suo        (501) staff       (20)    10103 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/embeddings/openai.py
+-rw-r--r--   0 suo        (501) staff       (20)      559 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/embeddings/utils.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.171742 llama_index-0.6.0a1/llama_index/evaluation/
+-rw-r--r--   0 suo        (501) staff       (20)      259 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/evaluation/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)    11972 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/evaluation/base.py
+-rw-r--r--   0 suo        (501) staff       (20)     5344 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/evaluation/dataset_generation.py
+-rw-r--r--   0 suo        (501) staff       (20)      544 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/img_utils.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.174801 llama_index-0.6.0a1/llama_index/indices/
+-rw-r--r--   0 suo        (501) staff       (20)      542 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     9024 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/base.py
+-rw-r--r--   0 suo        (501) staff       (20)      897 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/base_retriever.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.175185 llama_index-0.6.0a1/llama_index/indices/common/
+-rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/common/__init__.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.176561 llama_index-0.6.0a1/llama_index/indices/common/struct_store/
+-rw-r--r--   0 suo        (501) staff       (20)       19 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/common/struct_store/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     8114 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/common/struct_store/base.py
+-rw-r--r--   0 suo        (501) staff       (20)      776 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/common/struct_store/schema.py
+-rw-r--r--   0 suo        (501) staff       (20)     2629 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/common/struct_store/sql.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.177215 llama_index-0.6.0a1/llama_index/indices/common_tree/
+-rw-r--r--   0 suo        (501) staff       (20)       19 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/common_tree/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     7244 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/common_tree/base.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.177978 llama_index-0.6.0a1/llama_index/indices/composability/
+-rw-r--r--   0 suo        (501) staff       (20)      180 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/composability/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     3962 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/composability/graph.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.179065 llama_index-0.6.0a1/llama_index/indices/empty/
+-rw-r--r--   0 suo        (501) staff       (20)      198 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/empty/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     2151 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/empty/base.py
+-rw-r--r--   0 suo        (501) staff       (20)     1176 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/empty/retrievers.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.180992 llama_index-0.6.0a1/llama_index/indices/keyword_table/
+-rw-r--r--   0 suo        (501) staff       (20)      656 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/keyword_table/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     7652 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/keyword_table/base.py
+-rw-r--r--   0 suo        (501) staff       (20)      650 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/keyword_table/rake_base.py
+-rw-r--r--   0 suo        (501) staff       (20)     5991 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/keyword_table/retrievers.py
+-rw-r--r--   0 suo        (501) staff       (20)      844 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/keyword_table/simple_base.py
+-rw-r--r--   0 suo        (501) staff       (20)     2264 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/keyword_table/utils.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.181949 llama_index-0.6.0a1/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 suo        (501) staff       (20)      254 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     7816 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 suo        (501) staff       (20)     9543 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/knowledge_graph/retrievers.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.183183 llama_index-0.6.0a1/llama_index/indices/list/
+-rw-r--r--   0 suo        (501) staff       (20)      295 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/list/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     3305 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/list/base.py
+-rw-r--r--   0 suo        (501) staff       (20)     3455 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/list/retrievers.py
+-rw-r--r--   0 suo        (501) staff       (20)     3608 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/loading.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.185401 llama_index-0.6.0a1/llama_index/indices/postprocessor/
+-rw-r--r--   0 suo        (501) staff       (20)      888 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/postprocessor/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)       83 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/postprocessor/base.py
+-rw-r--r--   0 suo        (501) staff       (20)    11695 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/postprocessor/node.py
+-rw-r--r--   0 suo        (501) staff       (20)     8778 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/postprocessor/node_recency.py
+-rw-r--r--   0 suo        (501) staff       (20)     4896 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/postprocessor/pii.py
+-rw-r--r--   0 suo        (501) staff       (20)     8492 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/prompt_helper.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.187738 llama_index-0.6.0a1/llama_index/indices/query/
+-rw-r--r--   0 suo        (501) staff       (20)      137 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/query/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     1975 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/query/base.py
+-rw-r--r--   0 suo        (501) staff       (20)     3386 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/query/embedding_utils.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.189097 llama_index-0.6.0a1/llama_index/indices/query/query_transform/
+-rw-r--r--   0 suo        (501) staff       (20)      281 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/query/query_transform/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     8928 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/query/query_transform/base.py
+-rw-r--r--   0 suo        (501) staff       (20)     5920 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/query/query_transform/prompts.py
+-rw-r--r--   0 suo        (501) staff       (20)     8098 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/query/response_synthesis.py
+-rw-r--r--   0 suo        (501) staff       (20)     1203 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/query/schema.py
+-rw-r--r--   0 suo        (501) staff       (20)     1811 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/registry.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.190938 llama_index-0.6.0a1/llama_index/indices/response/
+-rw-r--r--   0 suo        (501) staff       (20)      419 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/response/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)    22075 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/response/response_builder.py
+-rw-r--r--   0 suo        (501) staff       (20)      264 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/response/type.py
+-rw-r--r--   0 suo        (501) staff       (20)     3310 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/service_context.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.195220 llama_index-0.6.0a1/llama_index/indices/struct_store/
+-rw-r--r--   0 suo        (501) staff       (20)      622 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/struct_store/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     2115 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/struct_store/base.py
+-rw-r--r--   0 suo        (501) staff       (20)     5802 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/struct_store/container_builder.py
+-rw-r--r--   0 suo        (501) staff       (20)     2214 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/struct_store/pandas.py
+-rw-r--r--   0 suo        (501) staff       (20)     4688 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/struct_store/pandas_query.py
+-rw-r--r--   0 suo        (501) staff       (20)     5904 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/struct_store/sql.py
+-rw-r--r--   0 suo        (501) staff       (20)     5887 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/struct_store/sql_query.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.197948 llama_index-0.6.0a1/llama_index/indices/tree/
+-rw-r--r--   0 suo        (501) staff       (20)      616 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/tree/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     1612 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0 suo        (501) staff       (20)     5834 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/tree/base.py
+-rw-r--r--   0 suo        (501) staff       (20)     7181 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/tree/inserter.py
+-rw-r--r--   0 suo        (501) staff       (20)     4663 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0 suo        (501) staff       (20)    15299 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0 suo        (501) staff       (20)     1402 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/tree/tree_root_retriever.py
+-rw-r--r--   0 suo        (501) staff       (20)     2005 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/utils.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.198966 llama_index-0.6.0a1/llama_index/indices/vector_store/
+-rw-r--r--   0 suo        (501) staff       (20)      260 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/vector_store/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     8183 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/vector_store/base.py
+-rw-r--r--   0 suo        (501) staff       (20)     3905 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/indices/vector_store/retrievers.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.200969 llama_index-0.6.0a1/llama_index/langchain_helpers/
+-rw-r--r--   0 suo        (501) staff       (20)       39 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/langchain_helpers/__init__.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.202399 llama_index-0.6.0a1/llama_index/langchain_helpers/agents/
+-rw-r--r--   0 suo        (501) staff       (20)      514 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/langchain_helpers/agents/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     2989 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/langchain_helpers/agents/agents.py
+-rw-r--r--   0 suo        (501) staff       (20)      837 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0 suo        (501) staff       (20)     2211 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/langchain_helpers/agents/tools.py
+-rw-r--r--   0 suo        (501) staff       (20)      252 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/langchain_helpers/chain_wrapper.py
+-rw-r--r--   0 suo        (501) staff       (20)     7675 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0 suo        (501) staff       (20)     3299 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/langchain_helpers/sql_wrapper.py
+-rw-r--r--   0 suo        (501) staff       (20)    17463 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/langchain_helpers/text_splitter.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.204454 llama_index-0.6.0a1/llama_index/llm_predictor/
+-rw-r--r--   0 suo        (501) staff       (20)      330 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/llm_predictor/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)    10593 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/llm_predictor/base.py
+-rw-r--r--   0 suo        (501) staff       (20)     4275 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/llm_predictor/chatgpt.py
+-rw-r--r--   0 suo        (501) staff       (20)     4732 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/llm_predictor/stable_lm.py
+-rw-r--r--   0 suo        (501) staff       (20)     2274 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/llm_predictor/structured.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.205141 llama_index-0.6.0a1/llama_index/logger/
+-rw-r--r--   0 suo        (501) staff       (20)       95 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/logger/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)      995 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/logger/base.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.206830 llama_index-0.6.0a1/llama_index/node_parser/
+-rw-r--r--   0 suo        (501) staff       (20)      184 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/node_parser/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)      530 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/node_parser/interface.py
+-rw-r--r--   0 suo        (501) staff       (20)     3585 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/node_parser/node_utils.py
+-rw-r--r--   0 suo        (501) staff       (20)     1821 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/node_parser/simple.py
+-rw-r--r--   0 suo        (501) staff       (20)     4900 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/old_docstore.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.207639 llama_index-0.6.0a1/llama_index/optimization/
+-rw-r--r--   0 suo        (501) staff       (20)      144 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/optimization/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     4301 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/optimization/optimizer.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.209038 llama_index-0.6.0a1/llama_index/output_parsers/
+-rw-r--r--   0 suo        (501) staff       (20)      230 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/output_parsers/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)      611 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/output_parsers/base.py
+-rw-r--r--   0 suo        (501) staff       (20)     2742 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/output_parsers/guardrails.py
+-rw-r--r--   0 suo        (501) staff       (20)     1828 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/output_parsers/langchain.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.209838 llama_index-0.6.0a1/llama_index/playground/
+-rw-r--r--   0 suo        (501) staff       (20)      202 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/playground/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     6471 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/playground/base.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.212629 llama_index-0.6.0a1/llama_index/prompts/
+-rw-r--r--   0 suo        (501) staff       (20)       87 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/prompts/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     6626 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/prompts/base.py
+-rw-r--r--   0 suo        (501) staff       (20)     1969 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/prompts/chat_prompts.py
+-rw-r--r--   0 suo        (501) staff       (20)     1134 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/prompts/default_prompt_selectors.py
+-rw-r--r--   0 suo        (501) staff       (20)    10843 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/prompts/default_prompts.py
+-rw-r--r--   0 suo        (501) staff       (20)      992 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/prompts/prompt_type.py
+-rw-r--r--   0 suo        (501) staff       (20)     7685 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/prompts/prompts.py
+-rw-r--r--   0 suo        (501) staff       (20)        0 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/py.typed
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.214307 llama_index-0.6.0a1/llama_index/query_engine/
+-rw-r--r--   0 suo        (501) staff       (20)      460 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/query_engine/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     3572 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/query_engine/graph_query_engine.py
+-rw-r--r--   0 suo        (501) staff       (20)     5814 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/query_engine/multistep_query_engine.py
+-rw-r--r--   0 suo        (501) staff       (20)     5322 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/query_engine/retriever_query_engine.py
+-rw-r--r--   0 suo        (501) staff       (20)     2967 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/query_engine/transform_query_engine.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.222505 llama_index-0.6.0a1/llama_index/readers/
+-rw-r--r--   0 suo        (501) staff       (20)     2974 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)      659 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/base.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.223301 llama_index-0.6.0a1/llama_index/readers/chatgpt_plugin/
+-rw-r--r--   0 suo        (501) staff       (20)      145 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/chatgpt_plugin/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     2111 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/chatgpt_plugin/base.py
+-rw-r--r--   0 suo        (501) staff       (20)     3755 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/chroma.py
+-rw-r--r--   0 suo        (501) staff       (20)     3328 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/database.py
+-rw-r--r--   0 suo        (501) staff       (20)     3457 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/deeplake.py
+-rw-r--r--   0 suo        (501) staff       (20)     4981 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/discord_reader.py
+-rw-r--r--   0 suo        (501) staff       (20)     7775 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/download.py
+-rw-r--r--   0 suo        (501) staff       (20)     2392 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/elasticsearch.py
+-rw-r--r--   0 suo        (501) staff       (20)     2510 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/faiss.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.228542 llama_index-0.6.0a1/llama_index/readers/file/
+-rw-r--r--   0 suo        (501) staff       (20)       19 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     8527 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/base.py
+-rw-r--r--   0 suo        (501) staff       (20)     1342 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/base_parser.py
+-rw-r--r--   0 suo        (501) staff       (20)     1629 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/docs_parser.py
+-rw-r--r--   0 suo        (501) staff       (20)     1318 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/epub_parser.py
+-rw-r--r--   0 suo        (501) staff       (20)     3180 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/image_caption_parser.py
+-rw-r--r--   0 suo        (501) staff       (20)     4106 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/image_parser.py
+-rw-r--r--   0 suo        (501) staff       (20)     3222 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/image_vision_llm_parser.py
+-rw-r--r--   0 suo        (501) staff       (20)     1027 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/ipynb_parser.py
+-rw-r--r--   0 suo        (501) staff       (20)     3616 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/markdown_parser.py
+-rw-r--r--   0 suo        (501) staff       (20)     3162 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/mbox_parser.py
+-rw-r--r--   0 suo        (501) staff       (20)     3945 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/slides_parser.py
+-rw-r--r--   0 suo        (501) staff       (20)     3357 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/tabular_parser.py
+-rw-r--r--   0 suo        (501) staff       (20)     1770 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/file/video_audio.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.230107 llama_index-0.6.0a1/llama_index/readers/github_readers/
+-rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/github_readers/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)    11730 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/github_readers/github_api_client.py
+-rw-r--r--   0 suo        (501) staff       (20)    15928 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/github_readers/github_repository_reader.py
+-rw-r--r--   0 suo        (501) staff       (20)     5473 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/github_readers/utils.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.231307 llama_index-0.6.0a1/llama_index/readers/google_readers/
+-rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/google_readers/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     5659 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/google_readers/gdocs.py
+-rw-r--r--   0 suo        (501) staff       (20)     4989 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/google_readers/gsheets.py
+-rw-r--r--   0 suo        (501) staff       (20)     3708 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/json.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.231973 llama_index-0.6.0a1/llama_index/readers/make_com/
+-rw-r--r--   0 suo        (501) staff       (20)       19 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/make_com/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     1696 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/make_com/wrapper.py
+-rw-r--r--   0 suo        (501) staff       (20)     1261 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/mbox.py
+-rw-r--r--   0 suo        (501) staff       (20)     4588 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/milvus.py
+-rw-r--r--   0 suo        (501) staff       (20)     2608 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/mongo.py
+-rw-r--r--   0 suo        (501) staff       (20)     5541 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/myscale.py
+-rw-r--r--   0 suo        (501) staff       (20)     5679 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/notion.py
+-rw-r--r--   0 suo        (501) staff       (20)     1601 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/obsidian.py
+-rw-r--r--   0 suo        (501) staff       (20)     2766 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/pinecone.py
+-rw-r--r--   0 suo        (501) staff       (20)     3909 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/qdrant.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.233084 llama_index-0.6.0a1/llama_index/readers/schema/
+-rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/schema/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     1214 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/schema/base.py
+-rw-r--r--   0 suo        (501) staff       (20)     7892 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/slack.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.234210 llama_index-0.6.0a1/llama_index/readers/steamship/
+-rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/steamship/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     3498 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/steamship/file_reader.py
+-rw-r--r--   0 suo        (501) staff       (20)     1042 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/string_iterable.py
+-rw-r--r--   0 suo        (501) staff       (20)     1918 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/twitter.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.236345 llama_index-0.6.0a1/llama_index/readers/weaviate/
+-rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/weaviate/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     7766 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/weaviate/client.py
+-rw-r--r--   0 suo        (501) staff       (20)     3986 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/weaviate/reader.py
+-rw-r--r--   0 suo        (501) staff       (20)     1867 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/weaviate/utils.py
+-rw-r--r--   0 suo        (501) staff       (20)     7987 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/web.py
+-rw-r--r--   0 suo        (501) staff       (20)      981 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/wikipedia.py
+-rw-r--r--   0 suo        (501) staff       (20)     1255 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/readers/youtube_transcript.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.238506 llama_index-0.6.0a1/llama_index/response/
+-rw-r--r--   0 suo        (501) staff       (20)       19 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/response/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     2039 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/response/notebook_utils.py
+-rw-r--r--   0 suo        (501) staff       (20)     3071 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/response/schema.py
+-rw-r--r--   0 suo        (501) staff       (20)      262 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/response/utils.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.239630 llama_index-0.6.0a1/llama_index/retrievers/
+-rw-r--r--   0 suo        (501) staff       (20)     1056 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/retrievers/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     1066 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/retrievers/transform_retriever.py
+-rw-r--r--   0 suo        (501) staff       (20)     2768 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/schema.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.240739 llama_index-0.6.0a1/llama_index/storage/
+-rw-r--r--   0 suo        (501) staff       (20)      124 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/__init__.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.245147 llama_index-0.6.0a1/llama_index/storage/docstore/
+-rw-r--r--   0 suo        (501) staff       (20)      536 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/docstore/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     4825 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/docstore/keyval_docstore.py
+-rw-r--r--   0 suo        (501) staff       (20)     1408 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/docstore/mongo_docstore.py
+-rw-r--r--   0 suo        (501) staff       (20)      762 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/docstore/registry.py
+-rw-r--r--   0 suo        (501) staff       (20)     2294 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/docstore/simple_docstore.py
+-rw-r--r--   0 suo        (501) staff       (20)     2532 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/docstore/types.py
+-rw-r--r--   0 suo        (501) staff       (20)      918 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/docstore/utils.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.248036 llama_index-0.6.0a1/llama_index/storage/index_store/
+-rw-r--r--   0 suo        (501) staff       (20)      301 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/index_store/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     2224 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/index_store/keyval_index_store.py
+-rw-r--r--   0 suo        (501) staff       (20)     1341 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/index_store/mongo_index_store.py
+-rw-r--r--   0 suo        (501) staff       (20)     1508 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/index_store/simple_index_store.py
+-rw-r--r--   0 suo        (501) staff       (20)      884 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/index_store/types.py
+-rw-r--r--   0 suo        (501) staff       (20)      644 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/index_store/utils.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.249673 llama_index-0.6.0a1/llama_index/storage/kvstore/
+-rw-r--r--   0 suo        (501) staff       (20)      187 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/kvstore/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     4061 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/kvstore/mongodb_kvstore.py
+-rw-r--r--   0 suo        (501) staff       (20)     2330 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0 suo        (501) staff       (20)      973 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/kvstore/types.py
+-rw-r--r--   0 suo        (501) staff       (20)     3114 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/storage/storage_context.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.251707 llama_index-0.6.0a1/llama_index/token_counter/
+-rw-r--r--   0 suo        (501) staff       (20)       17 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/token_counter/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     4664 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/token_counter/mock_chain_wrapper.py
+-rw-r--r--   0 suo        (501) staff       (20)      722 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/token_counter/mock_embed_model.py
+-rw-r--r--   0 suo        (501) staff       (20)     2874 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/token_counter/token_counter.py
+-rw-r--r--   0 suo        (501) staff       (20)      908 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/token_counter/utils.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.252495 llama_index-0.6.0a1/llama_index/tools/
+-rw-r--r--   0 suo        (501) staff       (20)       13 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/tools/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)      723 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/tools/file_utils.py
+-rw-r--r--   0 suo        (501) staff       (20)       81 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/types.py
+-rw-r--r--   0 suo        (501) staff       (20)     5847 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/utils.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.258006 llama_index-0.6.0a1/llama_index/vector_stores/
+-rw-r--r--   0 suo        (501) staff       (20)     1132 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/__init__.py
+-rw-r--r--   0 suo        (501) staff       (20)     5240 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/chatgpt_plugin.py
+-rw-r--r--   0 suo        (501) staff       (20)     3947 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/chroma.py
+-rw-r--r--   0 suo        (501) staff       (20)     8631 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/deeplake.py
+-rw-r--r--   0 suo        (501) staff       (20)     4365 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/faiss.py
+-rw-r--r--   0 suo        (501) staff       (20)    15768 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/milvus.py
+-rw-r--r--   0 suo        (501) staff       (20)     8344 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/myscale.py
+-rw-r--r--   0 suo        (501) staff       (20)     7186 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/opensearch.py
+-rw-r--r--   0 suo        (501) staff       (20)    11419 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/pinecone.py
+-rw-r--r--   0 suo        (501) staff       (20)     6505 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/qdrant.py
+-rw-r--r--   0 suo        (501) staff       (20)     1973 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/registry.py
+-rw-r--r--   0 suo        (501) staff       (20)     5084 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/simple.py
+-rw-r--r--   0 suo        (501) staff       (20)     2210 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/types.py
+-rw-r--r--   0 suo        (501) staff       (20)     3385 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/llama_index/vector_stores/weaviate.py
+drwxr-xr-x   0 suo        (501) staff       (20)        0 2023-04-28 21:55:20.163209 llama_index-0.6.0a1/llama_index.egg-info/
+-rw-r--r--   0 suo        (501) staff       (20)     4270 2023-04-28 21:55:20.000000 llama_index-0.6.0a1/llama_index.egg-info/PKG-INFO
+-rw-r--r--   0 suo        (501) staff       (20)     9542 2023-04-28 21:55:20.000000 llama_index-0.6.0a1/llama_index.egg-info/SOURCES.txt
+-rw-r--r--   0 suo        (501) staff       (20)        1 2023-04-28 21:55:20.000000 llama_index-0.6.0a1/llama_index.egg-info/dependency_links.txt
+-rw-r--r--   0 suo        (501) staff       (20)       96 2023-04-28 21:55:20.000000 llama_index-0.6.0a1/llama_index.egg-info/requires.txt
+-rw-r--r--   0 suo        (501) staff       (20)       12 2023-04-28 21:55:20.000000 llama_index-0.6.0a1/llama_index.egg-info/top_level.txt
+-rw-r--r--   0 suo        (501) staff       (20)       38 2023-04-28 21:55:20.258999 llama_index-0.6.0a1/setup.cfg
+-rw-r--r--   0 suo        (501) staff       (20)     1130 2023-04-28 21:55:19.000000 llama_index-0.6.0a1/setup.py
```

### Comparing `llama_index-0.5.9/LICENSE` & `llama_index-0.6.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/PKG-INFO` & `llama_index-0.6.0a1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 Metadata-Version: 2.1
 Name: llama_index
-Version: 0.5.9
+Version: 0.6.0a1
 Summary: Interface between LLMs and your data.
 Home-page: https://github.com/jerryjliu/gpt_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 🗂️ LlamaIndex 🦙 (GPT Index)
-
-> ⚠️ **NOTE**: We are rebranding GPT Index as LlamaIndex! We will carry out this transition gradually.
-
-> **2/25/2023**: By default, our docs/notebooks/instructions now reference "LlamaIndex"
-instead of "GPT Index".
-
-> **2/19/2023**: By default, our docs/notebooks/instructions now use the `llama-index` package. However the `gpt-index` package still exists as a duplicate!
-
-> **2/16/2023**: We have a duplicate `llama-index` pip package. Simply replace all imports of `gpt_index` with `llama_index` if you choose to `pip install llama-index`.
+# 🗂️ LlamaIndex 🦙
 
 LlamaIndex (GPT Index) is a project that provides a central interface to connect your LLM's with external data.
 
 PyPi: 
 - LlamaIndex: https://pypi.org/project/llama-index/.
 - GPT Index (duplicate): https://pypi.org/project/gpt-index/.
 
 Documentation: https://gpt-index.readthedocs.io/en/latest/.
 
 Twitter: https://twitter.com/gpt_index.
 
 Discord: https://discord.gg/dGcwcsnxhU.
 
-LlamaHub (community library of data loaders): https://llamahub.ai
+### Ecosystem
+
+- LlamaHub (community library of data loaders): https://llamahub.ai
+- Llama Lab (cutting-edge AGI projects using LlamaIndex): https://github.com/run-llama/llama-lab
+
 
 ## 🚀 Overview
 
 **NOTE**: This README is not updated as frequently as the documentation. Please check out the documentation above for the latest updates!
 
 ### Context
 - LLMs are a phenomenonal piece of technology for knowledge generation and reasoning. They are pre-trained on large amounts of publicly available data.
@@ -80,32 +75,45 @@
 Examples are in the `examples` folder. Indices are in the `indices` folder (see list of indices below).
 
 To build a simple vector store index:
 ```python
 import os
 os.environ["OPENAI_API_KEY"] = 'YOUR_OPENAI_API_KEY'
 
-from llama_index import GPTSimpleVectorIndex, SimpleDirectoryReader
+from llama_index import GPTVectorStoreIndex, SimpleDirectoryReader
 documents = SimpleDirectoryReader('data').load_data()
-index = GPTSimpleVectorIndex.from_documents(documents)
+index = GPTVectorStoreIndex.from_documents(documents)
+```
+
+
+To query:
+```python
+query_engine = index.as_query_engine()
+query_engine.query("<question_text>?")
 ```
 
-To save to and load from disk:
+
+By default, data is stored in-memory.
+To persist to disk (under `./storage`):
+
 ```python
-# save to disk
-index.save_to_disk('index.json')
-# load from disk
-index = GPTSimpleVectorIndex.load_from_disk('index.json')
+index.storage_context.persist()
 ```
 
-To query:
+To reload from disk:
 ```python
-index.query("<question_text>?")
+from llama_index import StorageContext, load_index_from_storage
+
+# rebuild storage context
+storage_context = StorageContext.from_defaults(persist_dir='./storage')
+# load index
+index = load_index_from_storage(storage_context)
 ```
 
+
 ## 🔧 Dependencies
 
 The main third-party package requirements are `tiktoken`, `openai`, and `langchain`.
 
 All requirements should be contained within the `setup.py` file. To run the package locally without building the wheel, simply run `pip install -r requirements.txt`.
```

### Comparing `llama_index-0.5.9/README.md` & `llama_index-0.6.0a1/llama_index.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-# 🗂️ LlamaIndex 🦙 (GPT Index)
+Metadata-Version: 2.1
+Name: llama-index
+Version: 0.6.0a1
+Summary: Interface between LLMs and your data.
+Home-page: https://github.com/jerryjliu/gpt_index
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-> ⚠️ **NOTE**: We are rebranding GPT Index as LlamaIndex! We will carry out this transition gradually.
-
-> **2/25/2023**: By default, our docs/notebooks/instructions now reference "LlamaIndex"
-instead of "GPT Index".
-
-> **2/19/2023**: By default, our docs/notebooks/instructions now use the `llama-index` package. However the `gpt-index` package still exists as a duplicate!
-
-> **2/16/2023**: We have a duplicate `llama-index` pip package. Simply replace all imports of `gpt_index` with `llama_index` if you choose to `pip install llama-index`.
+# 🗂️ LlamaIndex 🦙
 
 LlamaIndex (GPT Index) is a project that provides a central interface to connect your LLM's with external data.
 
 PyPi: 
 - LlamaIndex: https://pypi.org/project/llama-index/.
 - GPT Index (duplicate): https://pypi.org/project/gpt-index/.
 
 Documentation: https://gpt-index.readthedocs.io/en/latest/.
 
 Twitter: https://twitter.com/gpt_index.
 
 Discord: https://discord.gg/dGcwcsnxhU.
 
-LlamaHub (community library of data loaders): https://llamahub.ai
+### Ecosystem
+
+- LlamaHub (community library of data loaders): https://llamahub.ai
+- Llama Lab (cutting-edge AGI projects using LlamaIndex): https://github.com/run-llama/llama-lab
+
 
 ## 🚀 Overview
 
 **NOTE**: This README is not updated as frequently as the documentation. Please check out the documentation above for the latest updates!
 
 ### Context
 - LLMs are a phenomenonal piece of technology for knowledge generation and reasoning. They are pre-trained on large amounts of publicly available data.
@@ -71,32 +75,45 @@
 Examples are in the `examples` folder. Indices are in the `indices` folder (see list of indices below).
 
 To build a simple vector store index:
 ```python
 import os
 os.environ["OPENAI_API_KEY"] = 'YOUR_OPENAI_API_KEY'
 
-from llama_index import GPTSimpleVectorIndex, SimpleDirectoryReader
+from llama_index import GPTVectorStoreIndex, SimpleDirectoryReader
 documents = SimpleDirectoryReader('data').load_data()
-index = GPTSimpleVectorIndex.from_documents(documents)
+index = GPTVectorStoreIndex.from_documents(documents)
 ```
 
-To save to and load from disk:
+
+To query:
 ```python
-# save to disk
-index.save_to_disk('index.json')
-# load from disk
-index = GPTSimpleVectorIndex.load_from_disk('index.json')
+query_engine = index.as_query_engine()
+query_engine.query("<question_text>?")
 ```
 
-To query:
+
+By default, data is stored in-memory.
+To persist to disk (under `./storage`):
+
 ```python
-index.query("<question_text>?")
+index.storage_context.persist()
 ```
 
+To reload from disk:
+```python
+from llama_index import StorageContext, load_index_from_storage
+
+# rebuild storage context
+storage_context = StorageContext.from_defaults(persist_dir='./storage')
+# load index
+index = load_index_from_storage(storage_context)
+```
+
+
 ## 🔧 Dependencies
 
 The main third-party package requirements are `tiktoken`, `openai`, and `langchain`.
 
 All requirements should be contained within the `setup.py` file. To run the package locally without building the wheel, simply run `pip install -r requirements.txt`.
```

### Comparing `llama_index-0.5.9/llama_index/__init__.py` & `llama_index-0.6.0a1/llama_index/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,27 +27,21 @@
 )
 from llama_index.indices.list import GPTListIndex
 
 # prompt helper
 from llama_index.indices.prompt_helper import PromptHelper
 
 # for composability
-from llama_index.indices.query.schema import QueryConfig, QueryMode
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.struct_store.sql import GPTSQLStructStoreIndex
 from llama_index.indices.tree import GPTTreeIndex
-from llama_index.indices.vector_store import (
-    GPTChromaIndex,
-    GPTFaissIndex,
-    GPTPineconeIndex,
-    GPTQdrantIndex,
-    GPTSimpleVectorIndex,
-    GPTVectorStoreIndex,
-    GPTWeaviateIndex,
-)
+from llama_index.indices.vector_store import GPTVectorStoreIndex
+
+# storage
+from llama_index.storage.storage_context import StorageContext
 
 # langchain helper
 from llama_index.langchain_helpers.chain_wrapper import LLMPredictor
 from llama_index.langchain_helpers.memory_wrapper import GPTIndexMemory
 from llama_index.langchain_helpers.sql_wrapper import SQLDatabase
 
 # prompts
@@ -63,21 +57,23 @@
     TreeSelectPrompt,
 )
 
 # readers
 from llama_index.readers import (
     BeautifulSoupWebReader,
     ChromaReader,
+    DeepLakeReader,
     DiscordReader,
     Document,
     FaissReader,
     GithubRepositoryReader,
     GoogleDocsReader,
     JSONReader,
     MboxReader,
+    MilvusReader,
     NotionPageReader,
     ObsidianReader,
     PineconeReader,
     QdrantReader,
     RssReader,
     SimpleDirectoryReader,
     SimpleMongoReader,
@@ -94,35 +90,37 @@
 # response
 from llama_index.response.schema import Response
 
 # token predictor
 from llama_index.token_counter.mock_chain_wrapper import MockLLMPredictor
 from llama_index.token_counter.mock_embed_model import MockEmbedding
 
+# loading
+from llama_index.indices.loading import (
+    load_graph_from_storage,
+    load_index_from_storage,
+    load_indices_from_storage,
+)
+
 # best practices for library logging:
 # https://docs.python.org/3/howto/logging.html#configuring-logging-for-a-library
 logging.getLogger(__name__).addHandler(NullHandler())
 
 
 __all__ = [
+    "StorageContext",
     "ServiceContext",
     "ComposableGraph",
     "GPTKeywordTableIndex",
     "GPTSimpleKeywordTableIndex",
     "GPTRAKEKeywordTableIndex",
     "GPTListIndex",
     "GPTEmptyIndex",
     "GPTTreeIndex",
-    "GPTFaissIndex",
-    "GPTPineconeIndex",
-    "GPTQdrantIndex",
-    "GPTSimpleVectorIndex",
     "GPTVectorStoreIndex",
-    "GPTWeaviateIndex",
-    "GPTChromaIndex",
     "GPTSQLStructStoreIndex",
     "Prompt",
     "LangchainEmbedding",
     "OpenAIEmbedding",
     "SummaryPrompt",
     "TreeInsertPrompt",
     "TreeSelectPrompt",
@@ -142,32 +140,35 @@
     "GoogleDocsReader",
     "MboxReader",
     "SlackReader",
     "StringIterableReader",
     "WeaviateReader",
     "FaissReader",
     "ChromaReader",
+    "DeepLakeReader",
     "PineconeReader",
     "QdrantReader",
+    "MilvusReader",
     "DiscordReader",
     "SimpleWebPageReader",
     "RssReader",
     "BeautifulSoupWebReader",
     "TrafilaturaWebReader",
     "LLMPredictor",
     "MockLLMPredictor",
     "MockEmbedding",
     "SQLDatabase",
     "GPTIndexMemory",
     "SQLDocumentContextBuilder",
     "SQLContextBuilder",
     "PromptHelper",
-    "QueryConfig",
-    "QueryMode",
     "IndexStructType",
     "TwitterTweetReader",
     "download_loader",
     "GithubRepositoryReader",
+    "load_graph_from_storage",
+    "load_index_from_storage",
+    "load_indices_from_storage",
 ]
 
 # NOTE: keep for backwards compatibility
 SQLContextBuilder = SQLDocumentContextBuilder
```

### Comparing `llama_index-0.5.9/llama_index/composability/joint_qa_summary.py` & `llama_index-0.6.0a1/llama_index/composability/joint_qa_summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Joint QA Summary graph."""
 
 
 from typing import Sequence, Optional
+from llama_index.storage.docstore.registry import get_default_docstore
 
 from llama_index.indices.service_context import ServiceContext
 from llama_index.composability import ComposableGraph
 from llama_index.indices.list.base import GPTListIndex
 from llama_index.indices.tree.base import GPTTreeIndex
-from llama_index.indices.vector_store.vector_indices import GPTSimpleVectorIndex
+from llama_index.indices.vector_store import GPTVectorStoreIndex
 from llama_index.readers.schema.base import Document
-from llama_index.docstore import DocumentStore
+from llama_index.storage.docstore import BaseDocumentStore
 
 DEFAULT_SUMMARY_TEXT = "Use this index for summarization queries"
 DEFAULT_QA_TEXT = (
     "Use this index for queries that require retrieval of specific "
     "context from documents."
 )
 
@@ -23,47 +24,47 @@
 
     Can build a graph that provides a unified query interface
     for both QA and summarization tasks.
 
     NOTE: this is a beta feature. The API may change in the future.
 
     Args:
-        docstore (DocumentStore): A DocumentStore to use for storing nodes.
+        docstore (BaseDocumentStore): A BaseDocumentStore to use for storing nodes.
         service_context (ServiceContext): A ServiceContext to use for
             building indices.
         summary_text (str): Text to use for the summary index.
         qa_text (str): Text to use for the QA index.
         node_parser (NodeParser): A NodeParser to use for parsing.
 
     """
 
     def __init__(
         self,
-        docstore: Optional[DocumentStore] = None,
+        docstore: Optional[BaseDocumentStore] = None,
         service_context: Optional[ServiceContext] = None,
         summary_text: str = DEFAULT_SUMMARY_TEXT,
         qa_text: str = DEFAULT_QA_TEXT,
     ) -> None:
         """Init params."""
-        self._docstore = docstore or DocumentStore()
+        self._docstore = docstore or get_default_docstore()
         self._service_context = service_context or ServiceContext.from_defaults()
         self._summary_text = summary_text
         self._qa_text = qa_text
 
     def build_graph_from_documents(
         self,
         documents: Sequence[Document],
     ) -> "ComposableGraph":
         """Build graph from index."""
 
         nodes = self._service_context.node_parser.get_nodes_from_documents(documents)
         self._docstore.add_documents(nodes, allow_update=True)
 
         # used for QA
-        vector_index = GPTSimpleVectorIndex(
+        vector_index = GPTVectorStoreIndex(
             nodes,
             service_context=self._service_context,
         )
         # used for summarization
         list_index = GPTListIndex(nodes, service_context=self._service_context)
 
         vector_index.index_struct.summary = self._qa_text
```

### Comparing `llama_index-0.5.9/llama_index/data_structs/data_structs.py` & `llama_index-0.6.0a1/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/data_structs/data_structs_v2.py` & `llama_index-0.6.0a1/llama_index/data_structs/data_structs_v2.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 
 import uuid
 from abc import abstractmethod
 from dataclasses import dataclass, field
 from typing import Dict, List, Optional, Sequence, Set, Tuple
 
 from dataclasses_json import DataClassJsonMixin
-from pydantic import Json
 
-from llama_index.constants import DATA_KEY, TYPE_KEY
 from llama_index.data_structs.node_v2 import Node
 from llama_index.data_structs.struct_type import IndexStructType
 
 
 @dataclass
 class V2IndexStruct(DataClassJsonMixin):
     """A base data struct for a LlamaIndex."""
@@ -31,21 +29,14 @@
         return self.summary
 
     @classmethod
     @abstractmethod
     def get_type(cls) -> IndexStructType:
         """Get index struct type."""
 
-    def to_dict(self, encode_json: bool = False) -> Dict[str, Json]:
-        out_dict = {
-            TYPE_KEY: self.get_type(),
-            DATA_KEY: super().to_dict(encode_json),
-        }
-        return out_dict
-
 
 @dataclass
 class IndexGraph(V2IndexStruct):
     """A graph representing the tree-structured index."""
 
     # mapping from index in tree to Node doc id.
     all_nodes: Dict[int, str] = field(default_factory=dict)
@@ -97,14 +88,15 @@
     def insert_under_parent(
         self, node: Node, parent_node: Optional[Node], new_index: Optional[int] = None
     ) -> None:
         """Insert under parent node."""
         new_index = new_index or self.size
         if parent_node is None:
             self.root_nodes[new_index] = node.get_doc_id()
+            self.node_id_to_children_ids[node.get_doc_id()] = []
         else:
             if parent_node.doc_id not in self.node_id_to_children_ids:
                 self.node_id_to_children_ids[parent_node.get_doc_id()] = []
             self.node_id_to_children_ids[parent_node.get_doc_id()].append(
                 node.get_doc_id()
             )
 
@@ -284,123 +276,15 @@
 
     @classmethod
     def get_type(cls) -> IndexStructType:
         """Get type."""
         return IndexStructType.KG
 
 
-# TODO: remove once we centralize UX around vector index
-
-
-@dataclass
-class SimpleIndexDict(IndexDict):
-    """Index dict for simple vector index."""
-
-    @classmethod
-    def get_type(cls) -> IndexStructType:
-        """Get type."""
-        return IndexStructType.SIMPLE_DICT
-
-
-@dataclass
-class FaissIndexDict(IndexDict):
-    """Index dict for Faiss vector index."""
-
-    @classmethod
-    def get_type(cls) -> IndexStructType:
-        """Get type."""
-        return IndexStructType.DICT
-
-
-@dataclass
-class WeaviateIndexDict(IndexDict):
-    """Index dict for Weaviate vector index."""
-
-    @classmethod
-    def get_type(cls) -> IndexStructType:
-        """Get type."""
-        return IndexStructType.WEAVIATE
-
-
-@dataclass
-class PineconeIndexDict(IndexDict):
-    """Index dict for Pinecone vector index."""
-
-    @classmethod
-    def get_type(cls) -> IndexStructType:
-        """Get type."""
-        return IndexStructType.PINECONE
-
-
-@dataclass
-class QdrantIndexDict(IndexDict):
-    """Index dict for Qdrant vector index."""
-
-    @classmethod
-    def get_type(cls) -> IndexStructType:
-        """Get type."""
-        return IndexStructType.QDRANT
-
-
-@dataclass
-class ChromaIndexDict(IndexDict):
-    """Index dict for Chroma vector index."""
-
-    @classmethod
-    def get_type(cls) -> IndexStructType:
-        """Get type."""
-        return IndexStructType.CHROMA
-
-
-@dataclass
-class OpensearchIndexDict(IndexDict):
-    """Index dict for Opensearch vector index."""
-
-    @classmethod
-    def get_type(cls) -> IndexStructType:
-        """Get type."""
-        return IndexStructType.OPENSEARCH
-
-
-class ChatGPTRetrievalPluginIndexDict(IndexDict):
-    """Index dict for ChatGPT Retrieval Plugin."""
-
-    @classmethod
-    def get_type(cls) -> IndexStructType:
-        """Get type."""
-        return IndexStructType.CHATGPT_RETRIEVAL_PLUGIN
-
-
 @dataclass
 class EmptyIndex(IndexDict):
     """Empty index."""
 
     @classmethod
     def get_type(cls) -> IndexStructType:
         """Get type."""
         return IndexStructType.EMPTY
-
-
-@dataclass
-class CompositeIndex(V2IndexStruct):
-    all_index_structs: Dict[str, V2IndexStruct] = field(default_factory=dict)
-    root_id: Optional[str] = None
-
-    @classmethod
-    def get_type(cls) -> IndexStructType:
-        """Get type."""
-        return IndexStructType.COMPOSITE
-
-    def to_dict(self, encode_json: bool = False) -> Dict[str, Json]:
-        data_dict = {
-            "all_index_structs": {
-                id_: struct.to_dict(encode_json=encode_json)
-                for id_, struct in self.all_index_structs.items()
-            },
-            "root_id": self.root_id,
-        }
-
-        out_dict = {
-            TYPE_KEY: self.get_type(),
-            DATA_KEY: data_dict,
-        }
-        return out_dict
```

### Comparing `llama_index-0.5.9/llama_index/data_structs/node_v2.py` & `llama_index-0.6.0a1/llama_index/data_structs/node_v2.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,41 +4,44 @@
 a piece of data (e.g. chunk of text, an image, a table, etc).
 
 In comparison to a raw `Document`, it contains additional metadata
 about its relationship to other `Node` objects (and `Document` objects).
 
 It is often used as an atomic unit of data in various indices.
 """
+import logging
+import warnings
 from dataclasses import dataclass, field
 from enum import Enum, auto
-from typing import Any, Dict, Optional
-import warnings
+from typing import Any, Dict, List, Optional
 
 from dataclasses_json import DataClassJsonMixin
 
 from llama_index.schema import BaseDocument
 
-import logging
-
 _logger = logging.getLogger(__name__)
 
 
 class DocumentRelationship(str, Enum):
     """Document relationships used in `Node` class.
 
     Attributes:
         SOURCE: The node is the source document.
         PREVIOUS: The node is the previous node in the document.
         NEXT: The node is the next node in the document.
+        PARENT: The node is the parent node in the document.
+        CHILD: The node is a child node in the document.
 
     """
 
     SOURCE = auto()
     PREVIOUS = auto()
     NEXT = auto()
+    PARENT = auto()
+    CHILD = auto()
 
 
 class NodeType(str, Enum):
     TEXT = auto()
     IMAGE = auto()
     INDEX = auto()
 
@@ -47,30 +50,36 @@
 class Node(BaseDocument):
     """A generic node of data.
 
     Arguments:
         text (str): The text of the node.
         doc_id (Optional[str]): The document id of the node.
         embeddings (Optional[List[float]]): The embeddings of the node.
-        relationships (Dict[DocumentRelationship, str]): The relationships of the node.
+        relationships (Dict[DocumentRelationship, Any]): The relationships of the node.
 
     """
 
     def __post_init__(self) -> None:
         """Post init."""
         super().__post_init__()
         # NOTE: for Node objects, the text field is required
         if self.text is None:
             raise ValueError("text field not set.")
 
     # extra node info
     node_info: Optional[Dict[str, Any]] = None
 
     # document relationships
-    relationships: Dict[DocumentRelationship, str] = field(default_factory=dict)
+    relationships: Dict[DocumentRelationship, Any] = field(default_factory=dict)
+
+    def get_node_info(self) -> Dict[str, Any]:
+        """Get node info."""
+        if self.node_info is None:
+            raise ValueError("Node info not set.")
+        return self.node_info
 
     @property
     def ref_doc_id(self) -> Optional[str]:
         """Source document id.
 
         Extracted from the relationships field.
 
@@ -78,23 +87,45 @@
         return self.relationships.get(DocumentRelationship.SOURCE, None)
 
     @property
     def prev_node_id(self) -> str:
         """Prev node id."""
         if DocumentRelationship.PREVIOUS not in self.relationships:
             raise ValueError("Node does not have previous node")
+        if not isinstance(self.relationships[DocumentRelationship.PREVIOUS], str):
+            raise ValueError("Previous node must be a string")
         return self.relationships[DocumentRelationship.PREVIOUS]
 
     @property
     def next_node_id(self) -> str:
         """Next node id."""
         if DocumentRelationship.NEXT not in self.relationships:
             raise ValueError("Node does not have next node")
+        if not isinstance(self.relationships[DocumentRelationship.NEXT], str):
+            raise ValueError("Next node must be a string")
         return self.relationships[DocumentRelationship.NEXT]
 
+    @property
+    def parent_node_id(self) -> str:
+        """Parent node id."""
+        if DocumentRelationship.PARENT not in self.relationships:
+            raise ValueError("Node does not have parent node")
+        if not isinstance(self.relationships[DocumentRelationship.PARENT], str):
+            raise ValueError("Parent node must be a string")
+        return self.relationships[DocumentRelationship.PARENT]
+
+    @property
+    def child_node_ids(self) -> List[str]:
+        """Child node ids."""
+        if DocumentRelationship.CHILD not in self.relationships:
+            raise ValueError("Node does not have child nodes")
+        if not isinstance(self.relationships[DocumentRelationship.CHILD], list):
+            raise ValueError("Child nodes must be a list")
+        return self.relationships[DocumentRelationship.CHILD]
+
     def get_text(self) -> str:
         """Get text."""
         text = super().get_text()
         extra_info_exists = self.extra_info is not None and len(self.extra_info) > 0
         result_text = (
             text if not extra_info_exists else f"{self.extra_info_str}\n\n{text}"
         )
```

### Comparing `llama_index-0.5.9/llama_index/data_structs/struct_type.py` & `llama_index-0.6.0a1/llama_index/data_structs/struct_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,23 +20,32 @@
             for more information on the simple vector store index.
         WEAVIATE ("weaviate"): Weaviate Vector Store Index.
             See :ref:`Ref-Indices-VectorStore`
             for more information on the Weaviate vector store index.
         PINECONE ("pinecone"): Pinecone Vector Store Index.
             See :ref:`Ref-Indices-VectorStore`
             for more information on the Pinecone vector store index.
+        DEEPLAKE ("deeplake"): DeepLake Vector Store Index.
+            See :ref:`Ref-Indices-VectorStore`
+            for more information on the Pinecone vector store index.
         QDRANT ("qdrant"): Qdrant Vector Store Index.
             See :ref:`Ref-Indices-VectorStore`
             for more information on the Qdrant vector store index.
+        MILVUS ("milvus"): Milvus Vector Store Index.
+            See :ref:`Ref-Indices-VectorStore`
+            for more information on the Milvus vector store index.
         CHROMA ("chroma"): Chroma Vector Store Index.
             See :ref:`Ref-Indices-VectorStore`
             for more information on the Chroma vector store index.
         OPENSEARCH ("opensearch"): Opensearch Vector Store Index.
             See :ref:`Ref-Indices-VectorStore`
             for more information on the Opensearch vector store index.
+        MYSCALE ("myscale"): MyScale Vector Store Index.
+            See :ref:`Ref-Indices-VectorStore`
+            for more information on the MyScale vector store index.
         CHATGPT_RETRIEVAL_PLUGIN ("chatgpt_retrieval_plugin"): ChatGPT
             retrieval plugin index.
         SQL ("SQL"): SQL Structured Store Index.
             See :ref:`Ref-Indices-StructStore`
             for more information on the SQL vector store index.
         KG ("kg"): Knowledge Graph index.
             See :ref:`Ref-Indices-Knowledge-Graph` for KG indices.
@@ -53,19 +62,21 @@
     # faiss
     DICT = "dict"
     # simple
     SIMPLE_DICT = "simple_dict"
     WEAVIATE = "weaviate"
     PINECONE = "pinecone"
     QDRANT = "qdrant"
+    MILVUS = "milvus"
     CHROMA = "chroma"
+    MYSCALE = "myscale"
     VECTOR_STORE = "vector_store"
     OPENSEARCH = "opensearch"
     CHATGPT_RETRIEVAL_PLUGIN = "chatgpt_retrieval_plugin"
-
+    DEEPLAKE = "deeplake"
     # for SQL index
     SQL = "sql"
     # for KG index
     KG = "kg"
 
     # EMPTY
     EMPTY = "empty"
```

### Comparing `llama_index-0.5.9/llama_index/data_structs/table.py` & `llama_index-0.6.0a1/llama_index/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/data_structs/table_v2.py` & `llama_index-0.6.0a1/llama_index/data_structs/table_v2.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/embeddings/base.py` & `llama_index-0.6.0a1/llama_index/embeddings/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,19 +44,23 @@
         norm = np.linalg.norm(embedding1) * np.linalg.norm(embedding2)
         return product / norm
 
 
 class BaseEmbedding:
     """Base class for embeddings."""
 
-    def __init__(self, embed_batch_size: int = DEFAULT_EMBED_BATCH_SIZE) -> None:
+    def __init__(
+        self,
+        embed_batch_size: int = DEFAULT_EMBED_BATCH_SIZE,
+        tokenizer: Optional[Callable] = None,
+    ) -> None:
         """Init params."""
         self._total_tokens_used = 0
         self._last_token_usage: Optional[int] = None
-        self._tokenizer: Callable = globals_helper.tokenizer
+        self._tokenizer = tokenizer or globals_helper.tokenizer
         # list of tuples of id, text
         self._text_queue: List[Tuple[str, str]] = []
         if embed_batch_size <= 0:
             raise ValueError("embed_batch_size must be > 0")
         self._embed_batch_size = embed_batch_size
 
     @abstractmethod
@@ -118,15 +122,15 @@
     def get_text_embedding(self, text: str) -> List[float]:
         """Get text embedding."""
         text_embedding = self._get_text_embedding(text)
         text_tokens_count = len(self._tokenizer(text))
         self._total_tokens_used += text_tokens_count
         return text_embedding
 
-    def queue_text_for_embeddding(self, text_id: str, text: str) -> None:
+    def queue_text_for_embedding(self, text_id: str, text: str) -> None:
         """Queue text for embedding.
 
         Used for batching texts during embedding calls.
 
         """
         self._text_queue.append((text_id, text))
```

### Comparing `llama_index-0.5.9/llama_index/embeddings/langchain.py` & `llama_index-0.6.0a1/llama_index/embeddings/langchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,7 +24,11 @@
     def _get_query_embedding(self, query: str) -> List[float]:
         """Get query embedding."""
         return self._langchain_embedding.embed_query(query)
 
     def _get_text_embedding(self, text: str) -> List[float]:
         """Get text embedding."""
         return self._langchain_embedding.embed_documents([text])[0]
+
+    def _get_text_embeddings(self, texts: List[str]) -> List[List[float]]:
+        """Get text embeddings."""
+        return self._langchain_embedding.embed_documents(texts)
```

### Comparing `llama_index-0.5.9/llama_index/embeddings/openai.py` & `llama_index-0.6.0a1/llama_index/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/embeddings/utils.py` & `llama_index-0.6.0a1/llama_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/img_utils.py` & `llama_index-0.6.0a1/llama_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/indices/__init__.py` & `llama_index-0.6.0a1/llama_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/indices/common/struct_store/base.py` & `llama_index-0.6.0a1/llama_index/indices/common/struct_store/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 from abc import abstractmethod
 from typing import Any, Callable, Dict, List, Optional, Sequence, cast
 
 from llama_index.data_structs.node_v2 import Node
 from llama_index.data_structs.table import StructDatapoint
-from llama_index.indices.response.builder import ResponseBuilder, TextChunk
+from llama_index.indices.response.response_builder import get_response_builder
 from llama_index.indices.service_context import ServiceContext
 from llama_index.langchain_helpers.chain_wrapper import LLMPredictor
 from llama_index.langchain_helpers.sql_wrapper import SQLDatabase
 from llama_index.langchain_helpers.text_splitter import TextSplitter
 from llama_index.prompts.default_prompt_selectors import (
     DEFAULT_REFINE_TABLE_CONTEXT_PROMPT_SEL,
 )
@@ -100,26 +100,28 @@
         text_splitter = (
             self._text_splitter
             or self._service_context.prompt_helper.get_text_splitter_given_prompt(
                 prompt_with_schema, 1
             )
         )
         # we use the ResponseBuilder to iteratively go through all texts
-        response_builder = ResponseBuilder(
+        response_builder = get_response_builder(
             self._service_context,
             prompt_with_schema,
             refine_prompt_with_schema,
         )
+        text_chunks = []
         for doc in documents:
-            text_chunks = text_splitter.split_text(doc.get_text())
-            for text_chunk in text_chunks:
-                response_builder.add_text_chunks([TextChunk(text_chunk)])
+            chunks = text_splitter.split_text(doc.get_text())
+            text_chunks.extend(chunks)
 
         # feed in the "query_str" or the task
-        table_context = response_builder.get_response(self._table_context_task)
+        table_context = response_builder.get_response(
+            text_chunks=text_chunks, query_str=self._table_context_task
+        )
         return cast(str, table_context)
 
 
 OUTPUT_PARSER_TYPE = Callable[[str], Optional[Dict[str, Any]]]
 
 
 class BaseStructDatapointExtractor:
```

### Comparing `llama_index-0.5.9/llama_index/indices/common/struct_store/schema.py` & `llama_index-0.6.0a1/llama_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/indices/common/struct_store/sql.py` & `llama_index-0.6.0a1/llama_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/indices/common_tree/base.py` & `llama_index-0.6.0a1/llama_index/indices/common_tree/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import asyncio
 import logging
 from typing import Dict, List, Optional, Sequence, Tuple
 
 from llama_index.async_utils import run_async_tasks
 from llama_index.data_structs.data_structs_v2 import IndexGraph
 from llama_index.data_structs.node_v2 import Node
-from llama_index.docstore import DocumentStore
+from llama_index.storage.docstore import BaseDocumentStore
+from llama_index.storage.docstore.registry import get_default_docstore
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.utils import get_sorted_node_list, truncate_text
 from llama_index.prompts.prompts import SummaryPrompt
 
 logger = logging.getLogger(__name__)
 
 
@@ -25,28 +26,28 @@
     """
 
     def __init__(
         self,
         num_children: int,
         summary_prompt: SummaryPrompt,
         service_context: ServiceContext,
-        docstore: Optional[DocumentStore] = None,
+        docstore: Optional[BaseDocumentStore] = None,
         use_async: bool = False,
     ) -> None:
         """Initialize with params."""
         if num_children < 2:
             raise ValueError("Invalid number of children.")
         self.num_children = num_children
         self.summary_prompt = summary_prompt
         self._service_context = service_context
         self._use_async = use_async
-        self._docstore = docstore or DocumentStore()
+        self._docstore = docstore or get_default_docstore()
 
     @property
-    def docstore(self) -> DocumentStore:
+    def docstore(self) -> BaseDocumentStore:
         """Return docstore."""
         return self._docstore
 
     def build_from_nodes(
         self,
         nodes: Sequence[Node],
         build_tree: bool = True,
```

### Comparing `llama_index-0.5.9/llama_index/indices/composability/graph.py` & `llama_index-0.6.0a1/llama_index/indices/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,284 +1,236 @@
-"""Composability graphs."""
+"""Base index classes."""
+import logging
+from abc import ABC, abstractmethod
+from typing import Any, Generic, List, Optional, Sequence, Type, TypeVar
 
-import json
-from typing import Any, Dict, List, Optional, Sequence, Type, Union, cast
-
-from llama_index.constants import (
-    ADDITIONAL_QUERY_CONTEXT_KEY,
-    DOCSTORE_KEY,
-    INDEX_STRUCT_KEY,
-)
-from llama_index.data_structs.data_structs_v2 import CompositeIndex
 from llama_index.data_structs.data_structs_v2 import V2IndexStruct
-from llama_index.data_structs.data_structs_v2 import V2IndexStruct as IndexStruct
-from llama_index.data_structs.node_v2 import IndexNode, DocumentRelationship
-from llama_index.docstore import DocumentStore
-from llama_index.indices.base import BaseGPTIndex
-from llama_index.indices.composability.utils import (
-    load_query_context_from_dict,
-    save_query_context_to_dict,
-)
-from llama_index.indices.query.query_runner import QueryRunner
-from llama_index.indices.query.query_transform.base import BaseQueryTransform
-from llama_index.indices.query.schema import QueryBundle, QueryConfig
+from llama_index.data_structs.node_v2 import Node
+from llama_index.indices.base_retriever import BaseRetriever
+from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.service_context import ServiceContext
-from llama_index.response.schema import RESPONSE_TYPE
+from llama_index.readers.schema.base import Document
+from llama_index.storage.docstore.types import BaseDocumentStore
+from llama_index.storage.storage_context import StorageContext
+from llama_index.token_counter.token_counter import llm_token_counter
+
+IS = TypeVar("IS", bound=V2IndexStruct)
+IndexType = TypeVar("IndexType", bound="BaseGPTIndex")
+
+logger = logging.getLogger(__name__)
+
 
-# TMP: refactor query config type
-QUERY_CONFIG_TYPE = Union[Dict, QueryConfig]
+class BaseGPTIndex(Generic[IS], ABC):
+    """Base LlamaIndex.
 
+    Args:
+        nodes (List[Node]): List of nodes to index
+        service_context (ServiceContext): Service context container (contains
+            components like LLMPredictor, PromptHelper, etc.).
 
-class ComposableGraph:
-    """Composable graph."""
+    """
+
+    index_struct_cls: Type[IS]
 
     def __init__(
         self,
-        index_struct: CompositeIndex,
-        docstore: DocumentStore,
+        nodes: Optional[Sequence[Node]] = None,
+        index_struct: Optional[IS] = None,
+        storage_context: Optional[StorageContext] = None,
         service_context: Optional[ServiceContext] = None,
-        query_context: Optional[Dict[str, Dict[str, Any]]] = None,
         **kwargs: Any,
     ) -> None:
-        """Init params."""
-        self._docstore = docstore
-        self._index_struct = index_struct
-        self._service_context = service_context or ServiceContext.from_defaults()
-        self._query_context = query_context or {}
+        """Initialize with parameters."""
+        if index_struct is None and nodes is None:
+            raise ValueError("One of documents or index_struct must be provided.")
+        if index_struct is not None and nodes is not None:
+            raise ValueError("Only one of documents or index_struct can be provided.")
+        # This is to explicitly make sure that the old UX is not used
+        if nodes is not None and len(nodes) >= 1 and not isinstance(nodes[0], Node):
+            if isinstance(nodes[0], Document):
+                raise ValueError(
+                    "The constructor now takes in a list of Node objects. "
+                    "Since you are passing in a list of Document objects, "
+                    "please use `from_documents` instead."
+                )
+            else:
+                raise ValueError("nodes must be a list of Node objects.")
 
-    @property
-    def index_struct(self) -> CompositeIndex:
-        return self._index_struct
-
-    @property
-    def service_context(self) -> ServiceContext:
-        return self._service_context
+        self._service_context = service_context or ServiceContext.from_defaults()
+        self._storage_context = storage_context or StorageContext.from_defaults()
+        self._docstore = self._storage_context.docstore
+        self._vector_store = self._storage_context.vector_store
+
+        if index_struct is None:
+            assert nodes is not None
+            index_struct = self.build_index_from_nodes(nodes)
+        self._index_struct = index_struct
+        self._storage_context.index_store.add_index_struct(self._index_struct)
 
     @classmethod
-    def from_index_structs_and_docstores(
-        cls,
-        all_index_structs: Dict[str, IndexStruct],
-        root_id: str,
-        docstores: Sequence[DocumentStore],
-        query_context: Optional[Dict[str, Dict[str, Any]]] = None,
+    def from_documents(
+        cls: Type[IndexType],
+        documents: Sequence[Document],
+        storage_context: Optional[StorageContext] = None,
         service_context: Optional[ServiceContext] = None,
-    ) -> "ComposableGraph":
-        composite_index_struct = CompositeIndex(
-            all_index_structs=all_index_structs,
-            root_id=root_id,
-        )
-        merged_docstore = DocumentStore.merge(docstores)
-        return cls(
-            index_struct=composite_index_struct,
-            docstore=merged_docstore,
-            query_context=query_context,
-            service_context=service_context,
-        )
-
-    @classmethod
-    def from_indices(
-        cls,
-        root_index_cls: Type[BaseGPTIndex],
-        children_indices: Sequence[BaseGPTIndex],
-        index_summaries: Optional[Sequence[str]] = None,
         **kwargs: Any,
-    ) -> "ComposableGraph":  # type: ignore
-        """Create composable graph using this index class as the root."""
-        if index_summaries is None:
-            for index in children_indices:
-                if index.index_struct.summary is None:
-                    raise ValueError(
-                        "Summary must be set for children indices. If the index does "
-                        "a summary (through index.index_struct.summary), then it must "
-                        "be specified with then `index_summaries` "
-                        "argument in this function."
-                        "We will support automatically setting the summary in the "
-                        "future."
-                    )
-            index_summaries = [index.index_struct.summary for index in children_indices]
-        else:
-            # set summaries for each index
-            for index, summary in zip(children_indices, index_summaries):
-                index.index_struct.summary = summary
-
-        if len(children_indices) != len(index_summaries):
-            raise ValueError("indices and index_summaries must have same length!")
-
-        # construct index nodes
-        index_nodes = []
-        for index, summary in zip(children_indices, index_summaries):
-            assert isinstance(index.index_struct, V2IndexStruct)
-            index_node = IndexNode(
-                text=summary,
-                index_id=index.index_struct.index_id,
-                relationships={
-                    DocumentRelationship.SOURCE: index.index_struct.index_id
-                },
-            )
-            index_nodes.append(index_node)
-
-        # construct root index
-        root_index = root_index_cls(
-            nodes=index_nodes,
-            **kwargs,
-        )
-        # type: ignore
-        all_indices: List[BaseGPTIndex] = cast(List[BaseGPTIndex], children_indices) + [
-            root_index
-        ]
-
-        # collect query context, e.g. vector stores
-        query_context: Dict[str, Dict[str, Any]] = {}
-        for index in list(children_indices) + [root_index]:
-            assert isinstance(index.index_struct, V2IndexStruct)
-            index_id = index.index_struct.index_id
-            query_context[index_id] = index.query_context
-
-        return cls.from_index_structs_and_docstores(
-            all_index_structs={
-                index.index_struct.index_id: index.index_struct for index in all_indices
-            },
-            root_id=root_index.index_struct.index_id,
-            docstores=[index.docstore for index in all_indices],
-            service_context=root_index.service_context,
-            query_context=query_context,
-        )
+    ) -> IndexType:
+        """Create index from documents.
 
-    def query(
-        self,
-        query_str: Union[str, QueryBundle],
-        query_configs: Optional[List[QUERY_CONFIG_TYPE]] = None,
-        query_transform: Optional[BaseQueryTransform] = None,
-        service_context: Optional[ServiceContext] = None,
-    ) -> RESPONSE_TYPE:
-        """Query the index."""
-        service_context = service_context or self._service_context
-        query_runner = QueryRunner(
-            index_struct=self._index_struct,
-            service_context=service_context,
-            query_context=self._query_context,
-            docstore=self._docstore,
-            query_configs=query_configs,
-            query_transform=query_transform,
-            recursive=True,
-        )
-        return query_runner.query(query_str)
+        Args:
+            documents (Optional[Sequence[BaseDocument]]): List of documents to
+                build the index from.
 
-    async def aquery(
-        self,
-        query_str: Union[str, QueryBundle],
-        query_configs: Optional[List[QUERY_CONFIG_TYPE]] = None,
-        query_transform: Optional[BaseQueryTransform] = None,
-        service_context: Optional[ServiceContext] = None,
-    ) -> RESPONSE_TYPE:
-        """Query the index."""
-        service_context = service_context or self._service_context
-        query_runner = QueryRunner(
-            index_struct=self._index_struct,
-            service_context=service_context,
-            query_context=self._query_context,
-            docstore=self._docstore,
-            query_configs=query_configs,
-            query_transform=query_transform,
-            recursive=True,
-        )
-        return await query_runner.aquery(query_str)
+        """
+        storage_context = storage_context or StorageContext.from_defaults()
+        service_context = service_context or ServiceContext.from_defaults()
+        docstore = storage_context.docstore
 
-    def get_index(
-        self, index_struct_id: str, index_cls: Type[BaseGPTIndex], **kwargs: Any
-    ) -> BaseGPTIndex:
-        """Get index from index struct id."""
-        index_struct = self._index_struct.all_index_structs[index_struct_id]
-        return index_cls(
-            index_struct=index_struct,
-            docstore=self._docstore,
+        for doc in documents:
+            docstore.set_document_hash(doc.get_doc_id(), doc.get_doc_hash())
+
+        nodes = service_context.node_parser.get_nodes_from_documents(documents)
+
+        return cls(
+            nodes=nodes,
+            storage_context=storage_context,
+            service_context=service_context,
             **kwargs,
         )
 
-    @classmethod
-    def load_from_string(cls, index_string: str, **kwargs: Any) -> "ComposableGraph":
-        """Load index from string (in JSON-format).
+    @property
+    def index_struct(self) -> IS:
+        """Get the index struct."""
+        return self._index_struct
 
-        This method loads the index from a JSON string. The index data
-        structure itself is preserved completely. If the index is defined over
-        subindices, those subindices will also be preserved (and subindices of
-        those subindices, etc.).
+    @property
+    def index_id(self) -> str:
+        """Get the index struct."""
+        return self._index_struct.index_id
+
+    def set_index_id(self, index_id: str) -> None:
+        """Set the index id.
+
+        NOTE: if you decide to set the index_id on the index_struct manually,
+        you will need to explicitly call `add_index_struct` on the `index_store`
+        to update the index store.
+
+        .. code-block:: python
+            index.index_struct.index_id = index_id
+            index.storage_context.index_store.add_index_struct(index.index_struct)
 
         Args:
-            save_path (str): The save_path of the file.
-
-        Returns:
-            BaseGPTIndex: The loaded index.
+            index_id (str): Index id to set.
 
         """
-        # lazy load registry
-        from llama_index.indices.registry import load_index_struct_from_dict
+        # delete the old index struct
+        old_id = self._index_struct.index_id
+        self._storage_context.index_store.delete_index_struct(old_id)
+        # add the new index struct
+        self._index_struct.index_id = index_id
+        self._storage_context.index_store.add_index_struct(self._index_struct)
 
-        result_dict: Dict[str, Any] = json.loads(index_string)
-        index_struct = load_index_struct_from_dict(result_dict[INDEX_STRUCT_KEY])
-        docstore = DocumentStore.load_from_dict(result_dict[DOCSTORE_KEY])
-
-        # NOTE: this allows users to pass in kwargs at load time
-        #       e.g. passing in vector store client
-        query_context_kwargs = kwargs.pop("query_context_kwargs", None)
-        query_context = load_query_context_from_dict(
-            result_dict.get(ADDITIONAL_QUERY_CONTEXT_KEY, {}),
-            query_context_kwargs=query_context_kwargs,
-        )
-        assert isinstance(index_struct, CompositeIndex)
-        return cls(
-            index_struct=index_struct,
-            docstore=docstore,
-            query_context=query_context,
-            **kwargs,
-        )
-
-    @classmethod
-    def load_from_disk(cls, save_path: str, **kwargs: Any) -> "ComposableGraph":
-        """Load index from disk.
-
-        This method loads the index from a JSON file stored on disk. The index data
-        structure itself is preserved completely. If the index is defined over
-        subindices, those subindices will also be preserved (and subindices of
-        those subindices, etc.).
+    @property
+    def docstore(self) -> BaseDocumentStore:
+        """Get the docstore corresponding to the index."""
+        return self._docstore
 
-        Args:
-            save_path (str): The save_path of the file.
+    @property
+    def service_context(self) -> ServiceContext:
+        return self._service_context
 
-        Returns:
-            BaseGPTIndex: The loaded index.
+    @property
+    def storage_context(self) -> StorageContext:
+        return self._storage_context
 
-        """
-        with open(save_path, "r") as f:
-            file_contents = f.read()
-            return cls.load_from_string(file_contents, **kwargs)
+    @abstractmethod
+    def _build_index_from_nodes(self, nodes: Sequence[Node]) -> IS:
+        """Build the index from nodes."""
+
+    @llm_token_counter("build_index_from_nodes")
+    def build_index_from_nodes(self, nodes: Sequence[Node]) -> IS:
+        """Build the index from nodes."""
+        self._docstore.add_documents(nodes, allow_update=True)
+        return self._build_index_from_nodes(nodes)
+
+    @abstractmethod
+    def _insert(self, nodes: Sequence[Node], **insert_kwargs: Any) -> None:
+        """Index-specific logic for inserting nodes to the index struct."""
+
+    @llm_token_counter("insert")
+    def insert_nodes(self, nodes: Sequence[Node], **insert_kwargs: Any) -> None:
+        """Insert nodes."""
+        self.docstore.add_documents(nodes, allow_update=True)
+        self._insert(nodes, **insert_kwargs)
+        self._storage_context.index_store.add_index_struct(self._index_struct)
+
+    def insert(self, document: Document, **insert_kwargs: Any) -> None:
+        """Insert a document."""
+        nodes = self.service_context.node_parser.get_nodes_from_documents([document])
+        self.insert_nodes(nodes, **insert_kwargs)
+
+    @abstractmethod
+    def _delete(self, doc_id: str, **delete_kwargs: Any) -> None:
+        """Delete a document."""
 
-    def save_to_string(self, **save_kwargs: Any) -> str:
-        """Save to string.
+    def delete(self, doc_id: str, **delete_kwargs: Any) -> None:
+        """Delete a document from the index.
 
-        This method stores the index into a JSON file stored on disk.
+        All nodes in the index related to the index will be deleted.
 
         Args:
-            save_path (str): The save_path of the file.
+            doc_id (str): document id
 
         """
-        out_dict: Dict[str, Any] = {
-            INDEX_STRUCT_KEY: self._index_struct.to_dict(),
-            DOCSTORE_KEY: self._docstore.serialize_to_dict(),
-            ADDITIONAL_QUERY_CONTEXT_KEY: save_query_context_to_dict(
-                self._query_context
-            ),
-        }
-        return json.dumps(out_dict)
+        logger.debug(f"> Deleting document: {doc_id}")
+        self._delete(doc_id, **delete_kwargs)
+        self._storage_context.index_store.add_index_struct(self._index_struct)
 
-    def save_to_disk(self, save_path: str, **save_kwargs: Any) -> None:
-        """Save to file.
+    def update(self, document: Document, **update_kwargs: Any) -> None:
+        """Update a document.
 
-        This method stores the index into a JSON file stored on disk.
+        This is equivalent to deleting the document and then inserting it again.
 
         Args:
-            save_path (str): The save_path of the file.
+            document (Union[BaseDocument, BaseGPTIndex]): document to update
+            insert_kwargs (Dict): kwargs to pass to insert
+            delete_kwargs (Dict): kwargs to pass to delete
+
+        """
+        self.delete(document.get_doc_id(), **update_kwargs.pop("delete_kwargs", {}))
+        self.insert(document, **update_kwargs.pop("insert_kwargs", {}))
 
+    def refresh(
+        self, documents: Sequence[Document], **update_kwargs: Any
+    ) -> List[bool]:
+        """Refresh an index with documents that have changed.
+
+        This allows users to save LLM and Embedding model calls, while only
+        updating documents that have any changes in text or extra_info. It
+        will also insert any documents that previously were not stored.
         """
-        index_string = self.save_to_string(**save_kwargs)
-        with open(save_path, "w") as f:
-            f.write(index_string)
+        refreshed_documents = [False] * len(documents)
+        for i, document in enumerate(documents):
+            existing_doc_hash = self._docstore.get_document_hash(document.get_doc_id())
+            if existing_doc_hash != document.get_doc_hash():
+                self.update(document, **update_kwargs)
+                refreshed_documents[i] = True
+            elif existing_doc_hash is None:
+                self.insert(document, **update_kwargs.pop("insert_kwargs", {}))
+                refreshed_documents[i] = True
+
+        return refreshed_documents
+
+    @abstractmethod
+    def as_retriever(self, **kwargs: Any) -> BaseRetriever:
+        pass
+
+    def as_query_engine(self, **kwargs: Any) -> BaseQueryEngine:
+        # NOTE: lazy import
+        from llama_index.query_engine.retriever_query_engine import RetrieverQueryEngine
+
+        retriever = self.as_retriever(**kwargs)
+
+        kwargs["retriever"] = retriever
+        if "service_context" not in kwargs:
+            kwargs["service_context"] = self._service_context
+        return RetrieverQueryEngine.from_args(**kwargs)
```

### Comparing `llama_index-0.5.9/llama_index/indices/empty/base.py` & `llama_index-0.6.0a1/llama_index/indices/empty/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 
 """
 
 from typing import Any, Optional, Sequence
 
 from llama_index.data_structs.data_structs_v2 import EmptyIndex
 from llama_index.data_structs.node_v2 import Node
-from llama_index.indices.base import BaseGPTIndex, QueryMap
-from llama_index.indices.empty.query import GPTEmptyIndexQuery
-from llama_index.indices.query.schema import QueryMode
+from llama_index.indices.base import BaseGPTIndex
+from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.service_context import ServiceContext
 
 
 class GPTEmptyIndex(BaseGPTIndex[EmptyIndex]):
     """GPT Empty Index.
 
     An index that doesn't contain any documents. Used for
@@ -32,26 +31,25 @@
         self,
         index_struct: Optional[EmptyIndex] = None,
         service_context: Optional[ServiceContext] = None,
         **kwargs: Any,
     ) -> None:
         """Initialize params."""
         super().__init__(
-            nodes=[],
-            index_struct=index_struct,
+            nodes=None,
+            index_struct=index_struct or EmptyIndex(),
             service_context=service_context,
             **kwargs,
         )
 
-    @classmethod
-    def get_query_map(self) -> QueryMap:
-        """Get query map."""
-        return {
-            QueryMode.DEFAULT: GPTEmptyIndexQuery,
-        }
+    def as_retriever(self, **kwargs: Any) -> BaseRetriever:
+        # NOTE: lazy import
+        from llama_index.indices.empty.retrievers import EmptyIndexRetriever
+
+        return EmptyIndexRetriever(self)
 
     def _build_index_from_nodes(self, nodes: Sequence[Node]) -> EmptyIndex:
         """Build the index from documents.
 
         Args:
             documents (List[BaseDocument]): A list of documents.
```

### Comparing `llama_index-0.5.9/llama_index/indices/keyword_table/base.py` & `llama_index-0.6.0a1/llama_index/indices/keyword_table/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,37 +5,39 @@
 keywords as keys per item. It similarly extracts keywords
 from the query text. Then, it tries to match those keywords to
 existing keywords in the table.
 
 """
 
 from abc import abstractmethod
-from typing import Any, Optional, Sequence, Set
+from enum import Enum
+from typing import Any, Optional, Sequence, Set, Union
 
 from llama_index.async_utils import run_async_tasks
 from llama_index.data_structs.data_structs_v2 import KeywordTable
 from llama_index.data_structs.node_v2 import Node
-from llama_index.indices.base import BaseGPTIndex, QueryMap
+from llama_index.indices.base import BaseGPTIndex
+from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.keyword_table.utils import extract_keywords_given_response
-from llama_index.indices.keyword_table.query import (
-    GPTKeywordTableGPTQuery,
-    GPTKeywordTableRAKEQuery,
-    GPTKeywordTableSimpleQuery,
-)
-from llama_index.indices.query.schema import QueryMode
 from llama_index.indices.service_context import ServiceContext
 from llama_index.prompts.default_prompts import (
     DEFAULT_KEYWORD_EXTRACT_TEMPLATE,
     DEFAULT_QUERY_KEYWORD_EXTRACT_TEMPLATE,
 )
 from llama_index.prompts.prompts import KeywordExtractPrompt
 
 DQKET = DEFAULT_QUERY_KEYWORD_EXTRACT_TEMPLATE
 
 
+class KeywordTableRetrieverMode(str, Enum):
+    DEFAULT = "default"
+    SIMPLE = "simple"
+    RAKE = "rake"
+
+
 class BaseGPTKeywordTableIndex(BaseGPTIndex[KeywordTable]):
     """GPT Keyword Table Index.
 
     This index extracts keywords from the text, and maps each
     keyword to the node(s) that it corresponds to. In this sense it mimicks a
     "hash table". During index construction, the keyword table is constructed
     by extracting keywords from each node and creating an internal mapping.
@@ -78,22 +80,36 @@
         super().__init__(
             nodes=nodes,
             index_struct=index_struct,
             service_context=service_context,
             **kwargs,
         )
 
-    @classmethod
-    def get_query_map(self) -> QueryMap:
-        """Get query map."""
-        return {
-            QueryMode.DEFAULT: GPTKeywordTableGPTQuery,
-            QueryMode.SIMPLE: GPTKeywordTableSimpleQuery,
-            QueryMode.RAKE: GPTKeywordTableRAKEQuery,
-        }
+    def as_retriever(
+        self,
+        retriever_mode: Union[
+            str, KeywordTableRetrieverMode
+        ] = KeywordTableRetrieverMode.DEFAULT,
+        **kwargs: Any,
+    ) -> BaseRetriever:
+        # NOTE: lazy import
+        from llama_index.indices.keyword_table.retrievers import (
+            KeywordTableGPTRetriever,
+            KeywordTableRAKERetriever,
+            KeywordTableSimpleRetriever,
+        )
+
+        if retriever_mode == KeywordTableRetrieverMode.DEFAULT:
+            return KeywordTableGPTRetriever(self, **kwargs)
+        elif retriever_mode == KeywordTableRetrieverMode.SIMPLE:
+            return KeywordTableSimpleRetriever(self, **kwargs)
+        elif retriever_mode == KeywordTableRetrieverMode.RAKE:
+            return KeywordTableRAKERetriever(self, **kwargs)
+        else:
+            raise ValueError(f"Unknown retriever mode: {retriever_mode}")
 
     @abstractmethod
     def _extract_keywords(self, text: str) -> Set[str]:
         """Extract keywords from text."""
 
     async def _async_extract_keywords(self, text: str) -> Set[str]:
         """Extract keywords from text."""
```

### Comparing `llama_index-0.5.9/llama_index/indices/keyword_table/rake_base.py` & `llama_index-0.6.0a1/llama_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/indices/keyword_table/simple_base.py` & `llama_index-0.6.0a1/llama_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/indices/keyword_table/utils.py` & `llama_index-0.6.0a1/llama_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/indices/knowledge_graph/base.py` & `llama_index-0.6.0a1/llama_index/indices/knowledge_graph/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 keywords as keys per item. It similarly extracts keywords
 from the query text. Then, it tries to match those keywords to
 existing keywords in the table.
 
 """
 
 import logging
-from typing import Any, Dict, List, Optional, Sequence, Tuple
+from typing import Any, List, Optional, Sequence, Tuple
 
 from llama_index.data_structs.data_structs_v2 import KG
 from llama_index.data_structs.node_v2 import Node
-from llama_index.indices.base import BaseGPTIndex, QueryMap
-from llama_index.indices.knowledge_graph.query import GPTKGTableQuery, KGQueryMode
-from llama_index.indices.query.schema import QueryMode
+from llama_index.indices.base import BaseGPTIndex
+from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.prompts.default_prompts import (
     DEFAULT_KG_TRIPLET_EXTRACT_PROMPT,
     DEFAULT_QUERY_KEYWORD_EXTRACT_TEMPLATE,
 )
 from llama_index.prompts.prompts import KnowledgeGraphPrompt
 
 DQKET = DEFAULT_QUERY_KEYWORD_EXTRACT_TEMPLATE
@@ -66,20 +65,24 @@
 
         super().__init__(
             nodes=nodes,
             index_struct=index_struct,
             **kwargs,
         )
 
-    @classmethod
-    def get_query_map(self) -> QueryMap:
-        """Get query map."""
-        return {
-            QueryMode.DEFAULT: GPTKGTableQuery,
-        }
+    def as_retriever(self, **kwargs: Any) -> BaseRetriever:
+        from llama_index.indices.knowledge_graph.retrievers import (
+            KGRetrieverMode,
+            KGTableRetriever,
+        )
+
+        if len(self.index_struct.embedding_dict) > 0 and "retriever_mode" not in kwargs:
+            kwargs["retriever_mode"] = KGRetrieverMode.HYBRID
+
+        return KGTableRetriever(self, **kwargs)
 
     def _extract_triplets(self, text: str) -> List[Tuple[str, str, str]]:
         """Extract keywords from text."""
         response, _ = self._service_context.llm_predictor.predict(
             self.kg_triple_extract_template,
             text=text,
         )
@@ -107,15 +110,15 @@
             for triplet in triplets:
                 subj, _, obj = triplet
                 index_struct.upsert_triplet(triplet)
                 index_struct.add_node([subj, obj], n)
 
             if self.include_embeddings:
                 for i, triplet in enumerate(triplets):
-                    self._service_context.embed_model.queue_text_for_embeddding(
+                    self._service_context.embed_model.queue_text_for_embedding(
                         str(triplet), str(triplet)
                     )
 
                 embed_outputs = (
                     self._service_context.embed_model.get_queued_text_embeddings()
                 )
                 for rel_text, rel_embed in zip(*embed_outputs):
@@ -188,22 +191,14 @@
         self._index_struct.upsert_triplet(triplet)
         self._docstore.add_documents([node], allow_update=True)
 
     def _delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         """Delete a document."""
         raise NotImplementedError("Delete is not supported for KG index yet.")
 
-    def _preprocess_query(self, mode: QueryMode, query_kwargs: Dict) -> None:
-        """Set the default embedding mode during query based on current index."""
-        if (
-            len(self.index_struct.embedding_dict) > 0
-            and "embedding_mode" not in query_kwargs
-        ):
-            query_kwargs["embedding_mode"] = KGQueryMode.HYBRID
-
     def get_networkx_graph(self) -> Any:
         """Get networkx representation of the graph structure.
 
         NOTE: This function requires networkx to be installed.
         NOTE: This is a beta feature.
 
         """
```

### Comparing `llama_index-0.5.9/llama_index/indices/knowledge_graph/query.py` & `llama_index-0.6.0a1/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """Query for GPTKGTableIndex."""
 import logging
 from collections import defaultdict
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
-from llama_index.data_structs.data_structs_v2 import KG
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.node_v2 import Node, NodeWithScore
+from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.keyword_table.utils import extract_keywords_given_response
-from llama_index.indices.query.base import BaseGPTIndexQuery
+from llama_index.indices.knowledge_graph.base import GPTKnowledgeGraphIndex
 from llama_index.indices.query.embedding_utils import (
-    SimilarityTracker,
     get_top_k_embeddings,
 )
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.prompts.default_prompts import DEFAULT_QUERY_KEYWORD_EXTRACT_TEMPLATE
 from llama_index.prompts.prompts import QueryKeywordExtractPrompt
 from llama_index.utils import truncate_text
 
+
 DQKET = DEFAULT_QUERY_KEYWORD_EXTRACT_TEMPLATE
+DEFAULT_NODE_SCORE = 1000.0
 
 logger = logging.getLogger(__name__)
 
 
-class KGQueryMode(str, Enum):
+class KGRetrieverMode(str, Enum):
     """Query mode enum for Knowledge Graphs.
 
     Can be passed as the enum struct, or as the underlying string.
 
     Attributes:
         KEYWORD ("keyword"): Default query mode, using keywords to find triplets.
         EMBEDDING ("embedding"): Embedding mode, using embeddings to find
@@ -36,15 +37,15 @@
     """
 
     KEYWORD = "keyword"
     EMBEDDING = "embedding"
     HYBRID = "hybrid"
 
 
-class GPTKGTableQuery(BaseGPTIndexQuery[KG]):
+class KGTableRetriever(BaseRetriever):
     """Base GPT KG Table Index Query.
 
     Arguments are shared among subclasses.
 
     Args:
         query_keyword_extract_template (Optional[QueryKGExtractPrompt]): A Query
             KG Extraction
@@ -53,40 +54,46 @@
             (see :ref:`Prompt-Templates`).
         text_qa_template (Optional[QuestionAnswerPrompt]): A Question Answering Prompt
             (see :ref:`Prompt-Templates`).
         max_keywords_per_query (int): Maximum number of keywords to extract from query.
         num_chunks_per_query (int): Maximum number of text chunks to query.
         include_text (bool): Use the document text source from each relevant triplet
             during queries.
-        embedding_mode (KGQueryMode): Specifies whether to use keyowrds,
+        retriever_mode (KGRetrieverMode): Specifies whether to use keyowrds,
             embeddings, or both to find relevant triplets. Should be one of "keyword",
             "embedding", or "hybrid".
         similarity_top_k (int): The number of top embeddings to use
             (if embeddings are used).
     """
 
     def __init__(
         self,
-        index_struct: KG,
+        index: GPTKnowledgeGraphIndex,
         query_keyword_extract_template: Optional[QueryKeywordExtractPrompt] = None,
         max_keywords_per_query: int = 10,
         num_chunks_per_query: int = 10,
         include_text: bool = True,
-        embedding_mode: Optional[KGQueryMode] = KGQueryMode.KEYWORD,
+        retriever_mode: Optional[KGRetrieverMode] = KGRetrieverMode.KEYWORD,
         similarity_top_k: int = 2,
         **kwargs: Any,
     ) -> None:
         """Initialize params."""
-        super().__init__(index_struct=index_struct, **kwargs)
+
+        assert isinstance(index, GPTKnowledgeGraphIndex)
+        self._index = index
+        self._service_context = self._index.service_context
+        self._index_struct = self._index.index_struct
+        self._docstore = self._index.docstore
+
         self.max_keywords_per_query = max_keywords_per_query
         self.num_chunks_per_query = num_chunks_per_query
         self.query_keyword_extract_template = query_keyword_extract_template or DQKET
         self.similarity_top_k = similarity_top_k
         self._include_text = include_text
-        self._embedding_mode = KGQueryMode(embedding_mode)
+        self._retriever_mode = KGRetrieverMode(retriever_mode)
 
     def _get_keywords(self, query_str: str) -> List[str]:
         """Extract keywords."""
         response, _ = self._service_context.llm_predictor.predict(
             self.query_keyword_extract_template,
             max_keywords=self.max_keywords_per_query,
             question=query_str,
@@ -104,100 +111,93 @@
             if keyword:
                 keywords.append(keyword.strip("(\"'"))
         return keywords
 
     def _retrieve(
         self,
         query_bundle: QueryBundle,
-        similarity_tracker: Optional[SimilarityTracker] = None,
-    ) -> List[Node]:
+    ) -> List[NodeWithScore]:
         """Get nodes for response."""
         logger.info(f"> Starting query: {query_bundle.query_str}")
         keywords = self._get_keywords(query_bundle.query_str)
         logger.info(f"> Query keywords: {keywords}")
         rel_texts = []
         cur_rel_map = {}
         chunk_indices_count: Dict[str, int] = defaultdict(int)
 
-        if self._embedding_mode != KGQueryMode.EMBEDDING:
+        if self._retriever_mode != KGRetrieverMode.EMBEDDING:
             for keyword in keywords:
-                cur_rel_texts = self.index_struct.get_rel_map_texts(keyword)
+                cur_rel_texts = self._index_struct.get_rel_map_texts(keyword)
                 rel_texts.extend(cur_rel_texts)
-                cur_rel_map[keyword] = self.index_struct.get_rel_map_tuples(keyword)
+                cur_rel_map[keyword] = self._index_struct.get_rel_map_tuples(keyword)
                 if self._include_text:
-                    for node_id in self.index_struct.get_node_ids(keyword):
+                    for node_id in self._index_struct.get_node_ids(keyword):
                         chunk_indices_count[node_id] += 1
 
         if (
-            self._embedding_mode != KGQueryMode.KEYWORD
-            and len(self.index_struct.embedding_dict) > 0
+            self._retriever_mode != KGRetrieverMode.KEYWORD
+            and len(self._index_struct.embedding_dict) > 0
         ):
             query_embedding = self._service_context.embed_model.get_text_embedding(
                 query_bundle.query_str
             )
-            all_rel_texts = list(self.index_struct.embedding_dict.keys())
+            all_rel_texts = list(self._index_struct.embedding_dict.keys())
 
             rel_text_embeddings = [
-                self.index_struct.embedding_dict[_id] for _id in all_rel_texts
+                self._index_struct.embedding_dict[_id] for _id in all_rel_texts
             ]
             similarities, top_rel_texts = get_top_k_embeddings(
                 query_embedding,
                 rel_text_embeddings,
                 similarity_top_k=self.similarity_top_k,
                 embedding_ids=all_rel_texts,
-                similarity_cutoff=self.similarity_cutoff,
             )
             logger.debug(
                 f"Found the following rel_texts+query similarites: {str(similarities)}"
             )
             logger.debug(f"Found the following top_k rel_texts: {str(rel_texts)}")
             rel_texts.extend(top_rel_texts)
             if self._include_text:
                 keywords = self._extract_rel_text_keywords(top_rel_texts)
                 nested_node_ids = [
-                    self.index_struct.get_node_ids(keyword) for keyword in keywords
+                    self._index_struct.get_node_ids(keyword) for keyword in keywords
                 ]
                 # flatten list
                 node_ids = [_id for ids in nested_node_ids for _id in ids]
                 for node_id in node_ids:
                     chunk_indices_count[node_id] += 1
-        elif len(self.index_struct.embedding_dict) == 0:
+        elif len(self._index_struct.embedding_dict) == 0:
             logger.error(
                 "Index was not constructed with embeddings, skipping embedding usage..."
             )
 
         # remove any duplicates from keyword + embedding queries
-        if self._embedding_mode == KGQueryMode.HYBRID:
+        if self._retriever_mode == KGRetrieverMode.HYBRID:
             rel_texts = list(set(rel_texts))
 
         sorted_chunk_indices = sorted(
             list(chunk_indices_count.keys()),
             key=lambda x: chunk_indices_count[x],
             reverse=True,
         )
         sorted_chunk_indices = sorted_chunk_indices[: self.num_chunks_per_query]
         sorted_nodes = self._docstore.get_nodes(sorted_chunk_indices)
-        # filter sorted nodes
-        postprocess_info = {"similarity_tracker": similarity_tracker}
-        for node_processor in self.node_preprocessors:
-            sorted_nodes = node_processor.postprocess_nodes(
-                sorted_nodes, postprocess_info
-            )
 
         # TMP/TODO: also filter rel_texts as nodes until we figure out better
         # abstraction
-        rel_text_nodes = [Node(text=rel_text) for rel_text in rel_texts]
-        for node_processor in self.node_preprocessors:
-            rel_text_nodes = node_processor.postprocess_nodes(rel_text_nodes)
-        rel_texts = [node.get_text() for node in rel_text_nodes]
+        # TODO(suo): figure out what this does
+        # rel_text_nodes = [Node(text=rel_text) for rel_text in rel_texts]
+        # for node_processor in self._node_postprocessors:
+        #     rel_text_nodes = node_processor.postprocess_nodes(rel_text_nodes)
+        # rel_texts = [node.get_text() for node in rel_text_nodes]
 
+        sorted_nodes_with_scores = []
         for chunk_idx, node in zip(sorted_chunk_indices, sorted_nodes):
             # nodes are found with keyword mapping, give high conf to avoid cutoff
-            if similarity_tracker is not None:
-                similarity_tracker.add(node, 1000.0)
+            sorted_nodes_with_scores.append(NodeWithScore(node, DEFAULT_NODE_SCORE))
             logger.info(
                 f"> Querying with idx: {chunk_idx}: "
                 f"{truncate_text(node.get_text(), 80)}"
             )
 
         # add relationships as Node
         # TODO: make initial text customizable
@@ -208,21 +208,21 @@
         rel_info = [rel_initial_text] + rel_texts
         rel_node_info = {
             "kg_rel_texts": rel_texts,
             "kg_rel_map": cur_rel_map,
         }
         rel_text_node = Node(text="\n".join(rel_info), node_info=rel_node_info)
         # this node is constructed from rel_texts, give high confidence to avoid cutoff
-        if similarity_tracker is not None:
-            similarity_tracker.add(rel_text_node, 1000.0)
+        sorted_nodes_with_scores.append(
+            NodeWithScore(rel_text_node, DEFAULT_NODE_SCORE)
+        )
         rel_info_text = "\n".join(rel_info)
         logger.info(f"> Extracted relationships: {rel_info_text}")
-        sorted_nodes.append(rel_text_node)
 
-        return sorted_nodes
+        return sorted_nodes_with_scores
 
     def _get_extra_info_for_response(
         self, nodes: List[Node]
     ) -> Optional[Dict[str, Any]]:
         """Get extra info for response."""
         for node in nodes:
             if node.node_info is None or "kg_rel_map" not in node.node_info:
```

### Comparing `llama_index-0.5.9/llama_index/indices/list/base.py` & `llama_index-0.6.0a1/llama_index/indices/list/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """List index.
 
 A simple data structure where LlamaIndex iterates through document chunks
 in sequence in order to answer a given query.
 
 """
 
-from typing import Any, Optional, Sequence
+from enum import Enum
+from typing import Any, Optional, Sequence, Union
 
 from llama_index.data_structs.data_structs_v2 import IndexList
 from llama_index.data_structs.node_v2 import Node
-from llama_index.indices.base import BaseGPTIndex, QueryMap
-from llama_index.indices.list.embedding_query import GPTListIndexEmbeddingQuery
-from llama_index.indices.list.query import GPTListIndexQuery
-from llama_index.indices.query.schema import QueryMode
+from llama_index.indices.base import BaseGPTIndex
+from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.service_context import ServiceContext
-from llama_index.prompts.default_prompts import DEFAULT_TEXT_QA_PROMPT
-from llama_index.prompts.prompts import QuestionAnswerPrompt
 
-# This query is used to summarize the contents of the index.
-GENERATE_TEXT_QUERY = "What is a concise summary of this document?"
+
+class ListRetrieverMode(str, Enum):
+    DEFAULT = "default"
+    EMBEDDING = "embedding"
 
 
 class GPTListIndex(BaseGPTIndex[IndexList]):
     """GPT List Index.
 
     The list index is a simple data structure where nodes are stored in
     a sequence. During index construction, the document texts are
@@ -42,33 +41,40 @@
     index_struct_cls = IndexList
 
     def __init__(
         self,
         nodes: Optional[Sequence[Node]] = None,
         index_struct: Optional[IndexList] = None,
         service_context: Optional[ServiceContext] = None,
-        text_qa_template: Optional[QuestionAnswerPrompt] = None,
         **kwargs: Any,
     ) -> None:
         """Initialize params."""
-        self.text_qa_template = text_qa_template or DEFAULT_TEXT_QA_PROMPT
         super().__init__(
             nodes=nodes,
             index_struct=index_struct,
             service_context=service_context,
             **kwargs,
         )
 
-    @classmethod
-    def get_query_map(self) -> QueryMap:
-        """Get query map."""
-        return {
-            QueryMode.DEFAULT: GPTListIndexQuery,
-            QueryMode.EMBEDDING: GPTListIndexEmbeddingQuery,
-        }
+    def as_retriever(
+        self,
+        retriever_mode: Union[str, ListRetrieverMode] = ListRetrieverMode.DEFAULT,
+        **kwargs: Any,
+    ) -> BaseRetriever:
+        from llama_index.indices.list.retrievers import (
+            ListIndexEmbeddingRetriever,
+            ListIndexRetriever,
+        )
+
+        if retriever_mode == ListRetrieverMode.DEFAULT:
+            return ListIndexRetriever(self, **kwargs)
+        elif retriever_mode == ListRetrieverMode.EMBEDDING:
+            return ListIndexEmbeddingRetriever(self, **kwargs)
+        else:
+            raise ValueError(f"Unknown retriever mode: {retriever_mode}")
 
     def _build_index_from_nodes(self, nodes: Sequence[Node]) -> IndexList:
         """Build the index from documents.
 
         Args:
             documents (List[BaseDocument]): A list of documents.
 
@@ -79,22 +85,16 @@
         for n in nodes:
             index_struct.add_node(n)
         return index_struct
 
     def _insert(self, nodes: Sequence[Node], **insert_kwargs: Any) -> None:
         """Insert a document."""
         for n in nodes:
-            print("inserting node to index struct: ", n.get_doc_id())
+            # print("inserting node to index struct: ", n.get_doc_id())
             self._index_struct.add_node(n)
 
     def _delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         """Delete a document."""
         cur_node_ids = self._index_struct.nodes
         cur_nodes = self._docstore.get_nodes(cur_node_ids)
         nodes_to_keep = [n for n in cur_nodes if n.ref_doc_id != doc_id]
         self._index_struct.nodes = [n.get_doc_id() for n in nodes_to_keep]
-
-    def _preprocess_query(self, mode: QueryMode, query_kwargs: Any) -> None:
-        """Preprocess query."""
-        super()._preprocess_query(mode, query_kwargs)
-        if "text_qa_template" not in query_kwargs:
-            query_kwargs["text_qa_template"] = self.text_qa_template
```

### Comparing `llama_index-0.5.9/llama_index/indices/list/embedding_query.py` & `llama_index-0.6.0a1/llama_index/indices/list/retrievers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,93 +1,108 @@
-"""Embedding query for list index."""
+"""Default query for GPTListIndex."""
 import logging
 from typing import Any, List, Optional, Tuple
 
-from llama_index.data_structs.data_structs_v2 import IndexList
-from llama_index.data_structs.node_v2 import Node
-from llama_index.indices.list.query import BaseGPTListIndexQuery
+from llama_index.data_structs.node_v2 import Node, NodeWithScore
+from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.embedding_utils import (
-    SimilarityTracker,
     get_top_k_embeddings,
 )
 from llama_index.indices.query.schema import QueryBundle
+from llama_index.indices.list.base import GPTListIndex
 
 logger = logging.getLogger(__name__)
 
 
-class GPTListIndexEmbeddingQuery(BaseGPTListIndexQuery):
-    """GPTListIndex query.
+class ListIndexRetriever(BaseRetriever):
+    """Simple retriever for ListIndex that returns all nodes.
 
-    An embedding-based query for GPTListIndex, which traverses
-    each node in sequence and retrieves top-k nodes by
-    embedding similarity to the query.
-    Set when `mode="embedding"` in `query` method of `GPTListIndex`.
+    Args:
+        index (GPTListIndex): The index to retrieve from.
+
+    """
+
+    def __init__(self, index: GPTListIndex, **kwargs: Any) -> None:
+        self._index = index
+
+    def _retrieve(
+        self,
+        query_bundle: QueryBundle,
+    ) -> List[NodeWithScore]:
+        """Retrieve nodes."""
+        del query_bundle
+
+        node_ids = self._index.index_struct.nodes
+        nodes = self._index.docstore.get_nodes(node_ids)
+        return [NodeWithScore(node) for node in nodes]
 
-    .. code-block:: python
 
-        response = index.query("<query_str>", mode="embedding")
+class ListIndexEmbeddingRetriever(BaseRetriever):
+    """Embedding based retriever for ListIndex.
 
-    See BaseGPTListIndexQuery for arguments.
+    Generates embeddings in a lazy fashion for all
+    nodes that are traversed.
+
+    Args:
+        index (GPTListIndex): The index to retrieve from.
+        similarity_top_k (Optional[int]): The number of top nodes to return.
 
     """
 
     def __init__(
         self,
-        index_struct: IndexList,
+        index: GPTListIndex,
         similarity_top_k: Optional[int] = 1,
         **kwargs: Any,
     ) -> None:
-        """Initialize params."""
-        super().__init__(
-            index_struct=index_struct,
-            **kwargs,
-        )
-        self.similarity_top_k = similarity_top_k
+        self._index = index
+        self._similarity_top_k = similarity_top_k
 
     def _retrieve(
         self,
         query_bundle: QueryBundle,
-        similarity_tracker: Optional[SimilarityTracker] = None,
-    ) -> List[Node]:
-        """Get nodes for response."""
-        node_ids = self.index_struct.nodes
+    ) -> List[NodeWithScore]:
+        """Retrieve nodes."""
+        node_ids = self._index.index_struct.nodes
         # top k nodes
-        nodes = self._docstore.get_nodes(node_ids)
+        nodes = self._index.docstore.get_nodes(node_ids)
         query_embedding, node_embeddings = self._get_embeddings(query_bundle, nodes)
 
         top_similarities, top_idxs = get_top_k_embeddings(
             query_embedding,
             node_embeddings,
-            similarity_top_k=self.similarity_top_k,
+            similarity_top_k=self._similarity_top_k,
             embedding_ids=list(range(len(nodes))),
         )
 
         top_k_nodes = [nodes[i] for i in top_idxs]
 
-        if similarity_tracker is not None:
-            for node, similarity in zip(top_k_nodes, top_similarities):
-                similarity_tracker.add(node, similarity)
+        node_with_scores = []
+        for node, similarity in zip(top_k_nodes, top_similarities):
+            node_with_scores.append(NodeWithScore(node, score=similarity))
 
         logger.debug(f"> Top {len(top_idxs)} nodes:\n")
         nl = "\n"
         logger.debug(f"{ nl.join([n.get_text() for n in top_k_nodes]) }")
-        return top_k_nodes
+        return node_with_scores
 
     def _get_embeddings(
         self, query_bundle: QueryBundle, nodes: List[Node]
     ) -> Tuple[List[float], List[List[float]]]:
         """Get top nodes by similarity to the query."""
         if query_bundle.embedding is None:
             query_bundle.embedding = (
-                self._service_context.embed_model.get_agg_embedding_from_queries(
+                self._index._service_context.embed_model.get_agg_embedding_from_queries(
                     query_bundle.embedding_strs
                 )
             )
         node_embeddings: List[List[float]] = []
         for node in nodes:
             if node.embedding is None:
-                node.embedding = self._service_context.embed_model.get_text_embedding(
-                    node.get_text()
+                node.embedding = (
+                    self._index.service_context.embed_model.get_text_embedding(
+                        node.get_text()
+                    )
                 )
 
             node_embeddings.append(node.embedding)
         return query_bundle.embedding, node_embeddings
```

### Comparing `llama_index-0.5.9/llama_index/indices/list/query.py` & `llama_index-0.6.0a1/llama_index/indices/tree/tree_root_retriever.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,40 @@
-"""Default query for GPTListIndex."""
-from typing import List, Optional
+"""Retrieve query."""
+import logging
+from typing import Any, List
 
-from llama_index.data_structs.data_structs_v2 import IndexList
-from llama_index.data_structs.node_v2 import Node
-from llama_index.indices.query.base import BaseGPTIndexQuery
-from llama_index.indices.query.embedding_utils import SimilarityTracker
+from llama_index.data_structs.node_v2 import NodeWithScore
+from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.schema import QueryBundle
+from llama_index.indices.utils import get_sorted_node_list
 
+logger = logging.getLogger(__name__)
 
-class BaseGPTListIndexQuery(BaseGPTIndexQuery[IndexList]):
-    """GPTListIndex query.
 
-    Arguments are shared among subclasses.
+class TreeRootRetriever(BaseRetriever):
+    """GPT Tree Index retrieve query.
 
-    Args:
-        text_qa_template (Optional[QuestionAnswerPrompt]): A Question Answering Prompt
-            (see :ref:`Prompt-Templates`).
-        refine_template (Optional[RefinePrompt]): A Refinement Prompt
-            (see :ref:`Prompt-Templates`).
+    This class directly retrieves the answer from the root nodes.
 
+    Unlike GPTTreeIndexLeafQuery, this class assumes the graph already stores
+    the answer (because it was constructed with a query_str), so it does not
+    attempt to parse information down the graph in order to synthesize an answer.
     """
 
+    def __init__(self, index: Any):
+        from llama_index.indices.tree.base import GPTTreeIndex
 
-class GPTListIndexQuery(BaseGPTListIndexQuery):
-    """GPTListIndex query.
+        assert isinstance(index, GPTTreeIndex)
 
-    The default query mode for GPTListIndex, which traverses
-    each node in sequence and synthesizes a response across all nodes
-    (with an optional keyword filter).
-    Set when `mode="default"` in `query` method of `GPTListIndex`.
-
-    .. code-block:: python
-
-        response = index.query("<query_str>", mode="default")
-
-    See BaseGPTListIndexQuery for arguments.
-
-    """
+        self._index = index
+        self._index_struct = index.index_struct
+        self._docstore = index.docstore
 
     def _retrieve(
         self,
         query_bundle: QueryBundle,
-        similarity_tracker: Optional[SimilarityTracker] = None,
-    ) -> List[Node]:
+    ) -> List[NodeWithScore]:
         """Get nodes for response."""
-        node_ids = self.index_struct.nodes
-        nodes = self._docstore.get_nodes(node_ids)
-        return nodes
+        logger.info(f"> Starting query: {query_bundle.query_str}")
+        root_nodes = self._docstore.get_node_dict(self._index_struct.root_nodes)
+        sorted_nodes = get_sorted_node_list(root_nodes)
+        return [NodeWithScore(node) for node in sorted_nodes]
```

### Comparing `llama_index-0.5.9/llama_index/indices/postprocessor/node.py` & `llama_index-0.6.0a1/llama_index/indices/postprocessor/node.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,204 +4,191 @@
 from abc import abstractmethod
 from typing import Dict, List, Optional, cast
 
 from pydantic import BaseModel, Field, validator
 
 import logging
 from llama_index.indices.query.schema import QueryBundle
+from llama_index.indices.response.type import ResponseMode
 from llama_index.indices.service_context import ServiceContext
 from llama_index.prompts.prompts import QuestionAnswerPrompt, RefinePrompt
-from llama_index.docstore import DocumentStore
-from llama_index.data_structs.node_v2 import Node, DocumentRelationship
+from llama_index.storage.docstore import BaseDocumentStore
+from llama_index.data_structs.node_v2 import DocumentRelationship, NodeWithScore
 from llama_index.indices.postprocessor.base import BasePostprocessor
-from llama_index.indices.query.embedding_utils import SimilarityTracker
-from llama_index.indices.response.builder import ResponseBuilder, TextChunk
+from llama_index.indices.response.response_builder import get_response_builder
 
 logger = logging.getLogger(__name__)
 
 
 class BaseNodePostprocessor(BasePostprocessor, BaseModel):
     """Node postprocessor."""
 
+    class Config:
+        arbitrary_types_allowed = True
+
     @abstractmethod
     def postprocess_nodes(
-        self, nodes: List[Node], extra_info: Optional[Dict] = None
-    ) -> List[Node]:
+        self, nodes: List[NodeWithScore], extra_info: Optional[Dict] = None
+    ) -> List[NodeWithScore]:
         """Postprocess nodes."""
 
 
 class KeywordNodePostprocessor(BaseNodePostprocessor):
     """Keyword-based Node processor."""
 
     required_keywords: List[str] = Field(default_factory=list)
     exclude_keywords: List[str] = Field(default_factory=list)
 
     def postprocess_nodes(
-        self, nodes: List[Node], extra_info: Optional[Dict] = None
-    ) -> List[Node]:
+        self, nodes: List[NodeWithScore], extra_info: Optional[Dict] = None
+    ) -> List[NodeWithScore]:
         """Postprocess nodes."""
         new_nodes = []
-        for node in nodes:
-            words = re.findall(r"\w+", node.get_text())
+        for node_with_score in nodes:
+            node = node_with_score.node
             should_use_node = True
             if self.required_keywords is not None:
-                for w in self.required_keywords:
-                    if w not in words:
+                for keyword in self.required_keywords:
+                    pattern = r"\b" + re.escape(keyword) + r"\b"
+                    keyword_presence = re.search(pattern, node.get_text())
+                    if not keyword_presence:
                         should_use_node = False
 
             if self.exclude_keywords is not None:
-                for w in self.exclude_keywords:
-                    if w in words:
+                for keyword in self.exclude_keywords:
+                    pattern = r"\b" + re.escape(keyword) + r"\b"
+                    keyword_presence = re.search(keyword, node.get_text())
+                    if keyword_presence:
                         should_use_node = False
 
             if should_use_node:
-                new_nodes.append(node)
+                new_nodes.append(node_with_score)
 
         return new_nodes
 
 
 class SimilarityPostprocessor(BaseNodePostprocessor):
     """Similarity-based Node processor."""
 
     similarity_cutoff: float = Field(default=None)
 
     def postprocess_nodes(
-        self, nodes: List[Node], extra_info: Optional[Dict] = None
-    ) -> List[Node]:
+        self, nodes: List[NodeWithScore], extra_info: Optional[Dict] = None
+    ) -> List[NodeWithScore]:
         """Postprocess nodes."""
         extra_info = extra_info or {}
-        similarity_tracker = extra_info.get("similarity_tracker", None)
-        if similarity_tracker is None:
-            return nodes
-        sim_cutoff_exists = (
-            similarity_tracker is not None and self.similarity_cutoff is not None
-        )
+        sim_cutoff_exists = self.similarity_cutoff is not None
 
         new_nodes = []
         for node in nodes:
             should_use_node = True
             if sim_cutoff_exists:
-                similarity = cast(SimilarityTracker, similarity_tracker).find(node)
+                similarity = node.score
                 if similarity is None:
                     should_use_node = False
-                if cast(float, similarity) < cast(float, self.similarity_cutoff):
+                elif cast(float, similarity) < cast(float, self.similarity_cutoff):
                     should_use_node = False
 
             if should_use_node:
                 new_nodes.append(node)
 
         return new_nodes
 
 
 def get_forward_nodes(
-    node: Node, num_nodes: int, docstore: DocumentStore
-) -> Dict[str, Node]:
+    node_with_score: NodeWithScore, num_nodes: int, docstore: BaseDocumentStore
+) -> Dict[str, NodeWithScore]:
     """Get forward nodes."""
-    nodes: Dict[str, Node] = {node.get_doc_id(): node}
+    node = node_with_score.node
+    nodes: Dict[str, NodeWithScore] = {node.get_doc_id(): node_with_score}
     cur_count = 0
     # get forward nodes in an iterative manner
     while cur_count < num_nodes:
         if DocumentRelationship.NEXT not in node.relationships:
             break
         next_node_id = node.relationships[DocumentRelationship.NEXT]
         next_node = docstore.get_node(next_node_id)
         if next_node is None:
             break
-        nodes[next_node.get_doc_id()] = next_node
+        nodes[next_node.get_doc_id()] = NodeWithScore(next_node)
         node = next_node
         cur_count += 1
     return nodes
 
 
 def get_backward_nodes(
-    node: Node, num_nodes: int, docstore: DocumentStore
-) -> Dict[str, Node]:
+    node_with_score: NodeWithScore, num_nodes: int, docstore: BaseDocumentStore
+) -> Dict[str, NodeWithScore]:
     """Get backward nodes."""
+    node = node_with_score.node
     # get backward nodes in an iterative manner
-    nodes: Dict[str, Node] = {node.get_doc_id(): node}
+    nodes: Dict[str, NodeWithScore] = {node.get_doc_id(): node_with_score}
     cur_count = 0
     while cur_count < num_nodes:
         if DocumentRelationship.PREVIOUS not in node.relationships:
             break
         prev_node_id = node.relationships[DocumentRelationship.PREVIOUS]
         prev_node = docstore.get_node(prev_node_id)
         if prev_node is None:
             break
-        nodes[prev_node.get_doc_id()] = prev_node
+        nodes[prev_node.get_doc_id()] = NodeWithScore(prev_node)
         node = prev_node
         cur_count += 1
     return nodes
 
 
 class PrevNextNodePostprocessor(BaseNodePostprocessor):
     """Previous/Next Node post-processor.
 
     Allows users to fetch additional nodes from the document store,
     based on the relationships of the nodes.
 
     NOTE: this is a beta feature.
 
     Args:
-        docstore (DocumentStore): The document store.
+        docstore (BaseDocumentStore): The document store.
         num_nodes (int): The number of nodes to return (default: 1)
         mode (str): The mode of the post-processor.
             Can be "previous", "next", or "both.
 
     """
 
-    docstore: DocumentStore
+    docstore: BaseDocumentStore
     num_nodes: int = Field(default=1)
     mode: str = Field(default="next")
 
-    def _get_backward_nodes(self, node: Node) -> Dict[str, Node]:
-        """Get backward nodes."""
-        # get backward nodes in an iterative manner
-        nodes: Dict[str, Node] = {node.get_doc_id(): node}
-        cur_count = 0
-        while cur_count < self.num_nodes:
-            if DocumentRelationship.PREVIOUS not in node.relationships:
-                break
-            prev_node_id = node.relationships[DocumentRelationship.PREVIOUS]
-            prev_node = self.docstore.get_node(prev_node_id)
-            if prev_node is None:
-                break
-            nodes[prev_node.get_doc_id()] = prev_node
-            node = prev_node
-            cur_count += 1
-        return nodes
-
     @validator("mode")
     def _validate_mode(cls, v: str) -> str:
         """Validate mode."""
         if v not in ["next", "previous", "both"]:
             raise ValueError(f"Invalid mode: {v}")
         return v
 
     def postprocess_nodes(
-        self, nodes: List[Node], extra_info: Optional[Dict] = None
-    ) -> List[Node]:
+        self, nodes: List[NodeWithScore], extra_info: Optional[Dict] = None
+    ) -> List[NodeWithScore]:
         """Postprocess nodes."""
-        all_nodes: Dict[str, Node] = {}
+        all_nodes: Dict[str, NodeWithScore] = {}
         for node in nodes:
-            all_nodes[node.get_doc_id()] = node
+            all_nodes[node.node.get_doc_id()] = node
             if self.mode == "next":
                 all_nodes.update(get_forward_nodes(node, self.num_nodes, self.docstore))
             elif self.mode == "previous":
                 all_nodes.update(
                     get_backward_nodes(node, self.num_nodes, self.docstore)
                 )
             elif self.mode == "both":
                 all_nodes.update(get_forward_nodes(node, self.num_nodes, self.docstore))
                 all_nodes.update(
                     get_backward_nodes(node, self.num_nodes, self.docstore)
                 )
             else:
                 raise ValueError(f"Invalid mode: {self.mode}")
 
-        sorted_nodes = sorted(all_nodes.values(), key=lambda x: x.get_doc_id())
+        sorted_nodes = sorted(all_nodes.values(), key=lambda x: x.node.get_doc_id())
         return list(sorted_nodes)
 
 
 DEFAULT_INFER_PREV_NEXT_TMPL = (
     "The current context information is provided. \n"
     "A question is also provided. \n"
     "You are a retrieval agent deciding whether to search the "
@@ -247,23 +234,23 @@
 
     NOTE: difference with PrevNextPostprocessor is that
     this infers forward/backwards direction.
 
     NOTE: this is a beta feature.
 
     Args:
-        docstore (DocumentStore): The document store.
+        docstore (BaseDocumentStore): The document store.
         llm_predictor (LLMPredictor): The LLM predictor.
         num_nodes (int): The number of nodes to return (default: 1)
         infer_prev_next_tmpl (str): The template to use for inference.
             Required fields are {context_str} and {query_str}.
 
     """
 
-    docstore: DocumentStore
+    docstore: BaseDocumentStore
     service_context: ServiceContext
     num_nodes: int = Field(default=1)
     infer_prev_next_tmpl: str = Field(default=DEFAULT_INFER_PREV_NEXT_TMPL)
     refine_prev_next_tmpl: str = Field(default=DEFAULT_REFINE_INFER_PREV_NEXT_TMPL)
     verbose: bool = Field(default=False)
 
     class Config:
@@ -279,41 +266,41 @@
         elif "next" in pred:
             return "next"
         elif "none" in pred:
             return "none"
         raise ValueError(f"Invalid prediction: {raw_pred}")
 
     def postprocess_nodes(
-        self, nodes: List[Node], extra_info: Optional[Dict] = None
-    ) -> List[Node]:
+        self, nodes: List[NodeWithScore], extra_info: Optional[Dict] = None
+    ) -> List[NodeWithScore]:
         """Postprocess nodes."""
         if extra_info is None or "query_bundle" not in extra_info:
             raise ValueError("Missing query bundle in extra info.")
 
         query_bundle = cast(QueryBundle, extra_info["query_bundle"])
 
         infer_prev_next_prompt = QuestionAnswerPrompt(
             self.infer_prev_next_tmpl,
         )
         refine_infer_prev_next_prompt = RefinePrompt(self.refine_prev_next_tmpl)
 
-        all_nodes: Dict[str, Node] = {}
+        all_nodes: Dict[str, NodeWithScore] = {}
         for node in nodes:
-            all_nodes[node.get_doc_id()] = node
+            all_nodes[node.node.get_doc_id()] = node
             # use response builder instead of llm_predictor directly
             # to be more robust to handling long context
-            response_builder = ResponseBuilder(
-                self.service_context,
-                infer_prev_next_prompt,
-                refine_infer_prev_next_prompt,
+            response_builder = get_response_builder(
+                service_context=self.service_context,
+                text_qa_template=infer_prev_next_prompt,
+                refine_template=refine_infer_prev_next_prompt,
+                mode=ResponseMode.TREE_SUMMARIZE,
             )
-            response_builder.add_text_chunks([TextChunk(node.get_text())])
             raw_pred = response_builder.get_response(
+                text_chunks=[node.node.get_text()],
                 query_str=query_bundle.query_str,
-                response_mode="tree_summarize",
             )
             raw_pred = cast(str, raw_pred)
             mode = self._parse_prediction(raw_pred)
 
             logger.debug(f"> Postprocessor Predicted mode: {mode}")
             if self.verbose:
                 print(f"> Postprocessor Predicted mode: {mode}")
@@ -325,9 +312,9 @@
                     get_backward_nodes(node, self.num_nodes, self.docstore)
                 )
             elif mode == "none":
                 pass
             else:
                 raise ValueError(f"Invalid mode: {mode}")
 
-        sorted_nodes = sorted(all_nodes.values(), key=lambda x: x.get_doc_id())
+        sorted_nodes = sorted(all_nodes.values(), key=lambda x: x.node.get_doc_id())
         return list(sorted_nodes)
```

### Comparing `llama_index-0.5.9/llama_index/indices/prompt_helper.py` & `llama_index-0.6.0a1/llama_index/indices/prompt_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """General prompt helper that can help deal with token limitations.
 
 The helper can split text. It can also concatenate text from Node
 structs but keeping token limitations in mind.
 
 """
 
-from typing import Callable, List, Optional
+from typing import Callable, List, Optional, Sequence
 
 from llama_index.constants import MAX_CHUNK_OVERLAP
 from llama_index.data_structs.node_v2 import Node
 from llama_index.langchain_helpers.chain_wrapper import LLMPredictor
 from llama_index.langchain_helpers.text_splitter import TokenTextSplitter
 from llama_index.prompts.base import Prompt
 from llama_index.utils import globals_helper
@@ -215,15 +215,17 @@
             if text_splitter is not None:
                 node_text = text_splitter.truncate_text(node_text)
             text = f"({number}) {node_text}"
             results.append(text)
             number += 1
         return "\n\n".join(results)
 
-    def compact_text_chunks(self, prompt: Prompt, text_chunks: List[str]) -> List[str]:
+    def compact_text_chunks(
+        self, prompt: Prompt, text_chunks: Sequence[str]
+    ) -> List[str]:
         """Compact text chunks.
 
         This will combine text chunks into consolidated chunks
         that more fully "pack" the prompt template given the max_input_size.
 
         """
         combined_str = "\n\n".join([c.strip() for c in text_chunks if c.strip()])
```

### Comparing `llama_index-0.5.9/llama_index/indices/query/base.py` & `llama_index-0.6.0a1/llama_index/indices/tree/select_leaf_retriever.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,402 +1,417 @@
-"""Base query classes."""
+"""Leaf query mechanism."""
 
 import logging
-from abc import ABC
-from typing import (
-    Any,
-    Dict,
-    Generator,
-    Generic,
-    List,
-    Optional,
-    Sequence,
-    TypeVar,
-)
+from typing import Any, Dict, List, Optional, cast
 
 from langchain.input import print_text
 
-from llama_index.data_structs.data_structs_v2 import V2IndexStruct
 from llama_index.data_structs.node_v2 import Node, NodeWithScore
-from llama_index.docstore import DocumentStore
-from llama_index.indices.postprocessor.node import (
-    BaseNodePostprocessor,
-    KeywordNodePostprocessor,
-    SimilarityPostprocessor,
-)
-from llama_index.indices.query.embedding_utils import SimilarityTracker
+from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.schema import QueryBundle
-from llama_index.indices.response.builder import (
-    ResponseBuilder,
-    ResponseMode,
-    TextChunk,
-)
-from llama_index.indices.service_context import ServiceContext
-from llama_index.optimization.optimizer import BaseTokenUsageOptimizer
+from llama_index.indices.response.response_builder import get_response_builder
+from llama_index.indices.tree.base import GPTTreeIndex
+from llama_index.indices.utils import extract_numbers_given_response, get_sorted_node_list
 from llama_index.prompts.default_prompt_selectors import DEFAULT_REFINE_PROMPT_SEL
-from llama_index.prompts.default_prompts import DEFAULT_TEXT_QA_PROMPT
-from llama_index.prompts.prompts import QuestionAnswerPrompt, RefinePrompt
-from llama_index.response.schema import (
-    RESPONSE_TYPE,
-    Response,
-    StreamingResponse,
+from llama_index.prompts.default_prompts import (
+    DEFAULT_QUERY_PROMPT,
+    DEFAULT_QUERY_PROMPT_MULTIPLE,
+    DEFAULT_TEXT_QA_PROMPT,
 )
+from llama_index.prompts.prompts import (
+    QuestionAnswerPrompt,
+    RefinePrompt,
+    TreeSelectMultiplePrompt,
+    TreeSelectPrompt,
+)
+from llama_index.response.schema import Response
 from llama_index.token_counter.token_counter import llm_token_counter
-from llama_index.types import RESPONSE_TEXT_TYPE
 from llama_index.utils import truncate_text
 
-# to prevent us from having to remove all instances of v2 later
-IndexStruct = V2IndexStruct
-IS = TypeVar("IS", bound=V2IndexStruct)
-
 logger = logging.getLogger(__name__)
 
 
-def _get_initial_node_postprocessors(
-    required_keywords: Optional[List[str]] = None,
-    exclude_keywords: Optional[List[str]] = None,
-    similarity_cutoff: Optional[float] = None,
-) -> List[BaseNodePostprocessor]:
-    """Get initial node postprocessors.
-
-    This function is to help support deprecated keyword arguments.
-
-    """
-    postprocessors: List[BaseNodePostprocessor] = []
-    if required_keywords is not None or exclude_keywords is not None:
-        required_keywords = required_keywords or []
-        exclude_keywords = exclude_keywords or []
-        keyword_postprocessor = KeywordNodePostprocessor(
-            required_keywords=required_keywords, exclude_keywords=exclude_keywords
-        )
-        postprocessors.append(keyword_postprocessor)
-
-    if similarity_cutoff is not None:
-        similarity_postprocessor = SimilarityPostprocessor(
-            similarity_cutoff=similarity_cutoff
-        )
-        postprocessors.append(similarity_postprocessor)
-    return postprocessors
+def get_text_from_node(
+    node: Node,
+    level: Optional[int] = None,
+    verbose: bool = False,
+) -> str:
+    """Get text from node."""
+    level_str = "" if level is None else f"[Level {level}]"
+    fmt_text_chunk = truncate_text(node.get_text(), 50)
+    logger.debug(f">{level_str} Searching in chunk: {fmt_text_chunk}")
+
+    response_txt = node.get_text()
+    fmt_response = truncate_text(response_txt, 200)
+    if verbose:
+        print_text(f">{level_str} Got node text: {fmt_response}\n", color="blue")
+    return response_txt
 
 
-class BaseGPTIndexQuery(Generic[IS], ABC):
-    """Base LlamaIndex Query.
+class TreeSelectLeafRetriever(BaseRetriever):
+    """Tree select leaf retriever.
 
-    Helper class that is used to query an index. Can be called within `query`
-    method of a BaseGPTIndex object, or instantiated independently.
+    This class traverses the index graph and searches for a leaf node that can best
+    answer the query.
 
     Args:
-        service_context (ServiceContext): service context container (contains components
-            like LLMPredictor, PromptHelper).
-        required_keywords (List[str]): Optional list of keywords that must be present
-            in nodes. Can be used to query most indices (tree index is an exception).
-        exclude_keywords (List[str]): Optional list of keywords that must not be
-            present in nodes. Can be used to query most indices (tree index is an
-            exception).
-        response_mode (ResponseMode): Optional ResponseMode. If not provided, will
-            use the default ResponseMode.
-        text_qa_template (QuestionAnswerPrompt): Optional QuestionAnswerPrompt object.
-            If not provided, will use the default QuestionAnswerPrompt.
-        refine_template (RefinePrompt): Optional RefinePrompt object. If not provided,
-            will use the default RefinePrompt.
-        include_summary (bool): Optional bool. If True, will also use the summary
-            text of the index when generating a response (the summary text can be set
-            through `index.set_text("<text>")`).
-        similarity_cutoff (float): Optional float. If set, will filter out nodes with
-            similarity below this cutoff threshold when computing the response
-        streaming (bool): Optional bool. If True, will return a StreamingResponse
-            object. If False, will return a Response object.
+        query_template (Optional[TreeSelectPrompt]): Tree Select Query Prompt
+            (see :ref:`Prompt-Templates`).
+        query_template_multiple (Optional[TreeSelectMultiplePrompt]): Tree Select
+            Query Prompt (Multiple)
+            (see :ref:`Prompt-Templates`).
+        child_branch_factor (int): Number of child nodes to consider at each level.
+            If child_branch_factor is 1, then the query will only choose one child node
+            to traverse for any given parent node.
+            If child_branch_factor is 2, then the query will choose two child nodes.
 
     """
 
     def __init__(
         self,
-        index_struct: IS,
-        service_context: ServiceContext,
-        docstore: Optional[DocumentStore] = None,
-        # TODO: deprecated
-        required_keywords: Optional[List[str]] = None,
-        # TODO: deprecated
-        exclude_keywords: Optional[List[str]] = None,
-        response_mode: ResponseMode = ResponseMode.DEFAULT,
+        index: GPTTreeIndex,
+        query_template: Optional[TreeSelectPrompt] = None,
         text_qa_template: Optional[QuestionAnswerPrompt] = None,
         refine_template: Optional[RefinePrompt] = None,
-        include_summary: bool = False,
-        response_kwargs: Optional[Dict] = None,
-        # TODO: deprecated
-        similarity_cutoff: Optional[float] = None,
-        use_async: bool = False,
-        streaming: bool = False,
-        doc_ids: Optional[List[str]] = None,
-        optimizer: Optional[BaseTokenUsageOptimizer] = None,
-        node_postprocessors: Optional[List[BaseNodePostprocessor]] = None,
+        query_template_multiple: Optional[TreeSelectMultiplePrompt] = None,
+        child_branch_factor: int = 1,
         verbose: bool = False,
-    ) -> None:
-        """Initialize with parameters."""
-        if index_struct is None:
-            raise ValueError("index_struct must be provided.")
-        self._validate_index_struct(index_struct)
-        self._index_struct = index_struct
-        if docstore is None:
-            raise ValueError("docstore must be provided.")
-        self._docstore = docstore
-        self._service_context = service_context
-
-        self._response_mode = ResponseMode(response_mode)
-
-        self.text_qa_template = text_qa_template or DEFAULT_TEXT_QA_PROMPT
-        self.refine_template = refine_template or DEFAULT_REFINE_PROMPT_SEL
-        self._include_summary = include_summary
-
-        self._response_kwargs = response_kwargs or {}
-        self._use_async = use_async
-
-        # initialize logger with metadata
-        if self._service_context.llama_logger is not None:
-            self._service_context.llama_logger.set_metadata(
-                {
-                    "index_type": self._index_struct.get_type(),
-                    "index_id": self._index_struct.index_id,
-                }
-            )
-
-        self.response_builder = ResponseBuilder(
-            self._service_context,
-            self.text_qa_template,
-            self.refine_template,
-            use_async=use_async,
-            streaming=streaming,
-        )
-
-        # TODO: deprecated
-        self.similarity_cutoff = similarity_cutoff
-
-        self._streaming = streaming
-        self._doc_ids = doc_ids
-        self._optimizer = optimizer
-
-        # set default postprocessors
-        init_node_preprocessors = _get_initial_node_postprocessors(
-            required_keywords=required_keywords,
-            exclude_keywords=exclude_keywords,
-            similarity_cutoff=similarity_cutoff,
-        )
-        node_postprocessors = node_postprocessors or []
-        self.node_preprocessors: List[BaseNodePostprocessor] = (
-            init_node_preprocessors + node_postprocessors
+        **kwargs: Any,
+    ):
+        self._index = index
+        self._index_struct = index.index_struct
+        self._docstore = index.docstore
+        self._service_context = index.service_context
+
+        self._text_qa_template = text_qa_template or DEFAULT_TEXT_QA_PROMPT
+        self._refine_template = refine_template or DEFAULT_REFINE_PROMPT_SEL
+        self.query_template = query_template or DEFAULT_QUERY_PROMPT
+        self.query_template_multiple = (
+            query_template_multiple or DEFAULT_QUERY_PROMPT_MULTIPLE
         )
+        self.child_branch_factor = child_branch_factor
         self._verbose = verbose
 
-    def _get_text_from_node(
+    def _query_with_selected_node(
         self,
-        node: Node,
-        level: Optional[int] = None,
-    ) -> TextChunk:
-        """Query a given node.
+        selected_node: Node,
+        query_bundle: QueryBundle,
+        prev_response: Optional[str] = None,
+        level: int = 0,
+    ) -> str:
+        """Get response for selected node.
 
-        If node references a given document, then return the document.
-        If node references a given index, then query the index.
+        If not leaf node, it will recursively call _query on the child nodes.
+        If prev_response is provided, we will update prev_response with the answer.
 
         """
-        level_str = "" if level is None else f"[Level {level}]"
-        fmt_text_chunk = truncate_text(node.get_text(), 50)
-        logger.debug(f">{level_str} Searching in chunk: {fmt_text_chunk}")
+        query_str = query_bundle.query_str
 
-        response_txt = node.get_text()
-        fmt_response = truncate_text(response_txt, 200)
-        if self._verbose:
-            print_text(f">{level_str} Got node text: {fmt_response}\n", color="blue")
-        return TextChunk(response_txt)
+        if len(self._index_struct.get_children(selected_node)) == 0:
+            response_builder = get_response_builder(
+                self._service_context,
+                self._text_qa_template,
+                self._refine_template,
+            )
+            # use response builder to get answer from node
+            node_text = get_text_from_node(selected_node, level=level)
+            cur_response = response_builder.get_response(
+                query_str, [node_text], prev_response=prev_response
+            )
+            cur_response = cast(str, cur_response)
+            logger.debug(f">[Level {level}] Current answer response: {cur_response} ")
+        else:
+            cur_response = self._query_level(
+                self._index_struct.get_children(selected_node),
+                query_bundle,
+                level=level + 1,
+            )
 
-    @property
-    def index_struct(self) -> IS:
-        """Get the index struct."""
-        return self._index_struct
-
-    def _validate_index_struct(self, index_struct: IS) -> None:
-        """Validate the index struct."""
-        pass
-
-    def _give_response_for_nodes(
-        self, response_builder: ResponseBuilder, query_str: str
-    ) -> RESPONSE_TEXT_TYPE:
-        """Give response for nodes."""
-        response = response_builder.get_response(
-            query_str,
-            mode=self._response_mode,
-            **self._response_kwargs,
-        )
-        return response
+        if prev_response is None:
+            return cur_response
+        else:
+            context_msg = selected_node.get_text()
+            (
+                cur_response,
+                formatted_refine_prompt,
+            ) = self._service_context.llm_predictor.predict(
+                self._refine_template,
+                query_str=query_str,
+                existing_answer=prev_response,
+                context_msg=context_msg,
+            )
 
-    async def _agive_response_for_nodes(
-        self, response_builder: ResponseBuilder, query_str: str
-    ) -> RESPONSE_TEXT_TYPE:
-        """Give response for nodes."""
-        response = await response_builder.aget_response(
-            query_str,
-            mode=self._response_mode,
-            **self._response_kwargs,
-        )
-        return response
+            logger.debug(f">[Level {level}] Refine prompt: {formatted_refine_prompt}")
+            logger.debug(f">[Level {level}] Current refined response: {cur_response} ")
+            return cur_response
 
-    def retrieve(self, query_bundle: QueryBundle) -> List[NodeWithScore]:
-        """Get list of tuples of node and similarity for response.
+    def _query_level(
+        self,
+        cur_node_ids: Dict[int, str],
+        query_bundle: QueryBundle,
+        level: int = 0,
+    ) -> str:
+        """Answer a query recursively."""
+        query_str = query_bundle.query_str
+        cur_nodes = {
+            index: self._docstore.get_node(node_id)
+            for index, node_id in cur_node_ids.items()
+        }
+        cur_node_list = get_sorted_node_list(cur_nodes)
 
-        First part of the tuple is the node.
-        Second part of tuple is the distance from query to the node.
-        If not applicable, it's None.
-        """
-        similarity_tracker = SimilarityTracker()
-        nodes = self._retrieve(query_bundle, similarity_tracker=similarity_tracker)
+        if len(cur_node_list) == 1:
+            logger.debug(f">[Level {level}] Only one node left. Querying node.")
+            return self._query_with_selected_node(
+                cur_node_list[0], query_bundle, level=level
+            )
+        elif self.child_branch_factor == 1:
+            query_template = self.query_template.partial_format(
+                num_chunks=len(cur_node_list), query_str=query_str
+            )
+            numbered_node_text = (
+                self._service_context.prompt_helper.get_numbered_text_from_nodes(
+                    cur_node_list, prompt=query_template
+                )
+            )
+            (
+                response,
+                formatted_query_prompt,
+            ) = self._service_context.llm_predictor.predict(
+                query_template,
+                context_list=numbered_node_text,
+            )
+        else:
+            query_template_multiple = self.query_template_multiple.partial_format(
+                num_chunks=len(cur_node_list),
+                query_str=query_str,
+                branching_factor=self.child_branch_factor,
+            )
+            numbered_node_text = (
+                self._service_context.prompt_helper.get_numbered_text_from_nodes(
+                    cur_node_list, prompt=query_template_multiple
+                )
+            )
+            (
+                response,
+                formatted_query_prompt,
+            ) = self._service_context.llm_predictor.predict(
+                query_template_multiple,
+                context_list=numbered_node_text,
+            )
 
-        postprocess_info = {
-            "similarity_tracker": similarity_tracker,
-            "query_bundle": query_bundle,
-        }
-        for node_processor in self.node_preprocessors:
-            nodes = node_processor.postprocess_nodes(nodes, postprocess_info)
+        logger.debug(
+            f">[Level {level}] current prompt template: {formatted_query_prompt}"
+        )
+        self._service_context.llama_logger.add_log(
+            {"formatted_prompt_template": formatted_query_prompt, "level": level}
+        )
+        debug_str = f">[Level {level}] Current response: {response}"
+        logger.debug(debug_str)
+        if self._verbose:
+            print_text(debug_str, end="\n")
 
-        # TODO: create a `display` method to allow subclasses to print the Node
-        return similarity_tracker.get_zipped_nodes(nodes)
+        numbers = extract_numbers_given_response(response, n=self.child_branch_factor)
+        if numbers is None:
+            debug_str = (
+                f">[Level {level}] Could not retrieve response - no numbers present"
+            )
+            logger.debug(debug_str)
+            if self._verbose:
+                print_text(debug_str, end="\n")
+            # just join text from current nodes as response
+            return response
+        result_response = None
+        for number_str in numbers:
+            number = int(number_str)
+            if number > len(cur_node_list):
+                logger.debug(
+                    f">[Level {level}] Invalid response: {response} - "
+                    f"number {number} out of range"
+                )
+                return response
+
+            # number is 1-indexed, so subtract 1
+            selected_node = cur_node_list[number - 1]
+
+            info_str = (
+                f">[Level {level}] Selected node: "
+                f"[{number}]/[{','.join([str(int(n)) for n in numbers])}]"
+            )
+            logger.info(info_str)
+            if self._verbose:
+                print_text(info_str, end="\n")
+            debug_str = " ".join(selected_node.get_text().splitlines())
+            full_debug_str = (
+                f">[Level {level}] Node "
+                f"[{number}] Summary text: "
+                f"{ selected_node.get_text() }"
+            )
+            logger.debug(full_debug_str)
+            if self._verbose:
+                print_text(full_debug_str, end="\n")
+            result_response = self._query_with_selected_node(
+                selected_node,
+                query_bundle,
+                prev_response=result_response,
+                level=level,
+            )
+        # result_response should not be None
+        return cast(str, result_response)
 
-    def _retrieve(
+    def _query(self, query_bundle: QueryBundle) -> Response:
+        """Answer a query."""
+        # NOTE: this overrides the _query method in the base class
+        info_str = f"> Starting query: {query_bundle.query_str}"
+        logger.info(info_str)
+        if self._verbose:
+            print_text(info_str, end="\n")
+        response_str = self._query_level(
+            self._index_struct.root_nodes,
+            query_bundle,
+            level=0,
+        ).strip()
+        # TODO: fix source nodes
+        return Response(response_str, source_nodes=[])
+
+    def _select_nodes(
         self,
+        cur_node_list: List[Node],
         query_bundle: QueryBundle,
-        similarity_tracker: Optional[SimilarityTracker] = None,
+        level: int = 0,
     ) -> List[Node]:
-        """Get nodes for response."""
-        return []
-
-    def _get_extra_info_for_response(
-        self,
-        nodes: List[Node],
-    ) -> Optional[Dict[str, Any]]:
-        """Get extra info for response."""
-        return None
+        query_str = query_bundle.query_str
 
-    def _prepare_response_builder(
-        self,
-        response_builder: ResponseBuilder,
-        query_bundle: QueryBundle,
-        nodes: List[NodeWithScore],
-        additional_source_nodes: Optional[Sequence[NodeWithScore]],
-    ) -> None:
-        """Prepare response builder and return values for query time."""
-        response_builder.reset()
-        for node_with_score in nodes:
-            text = self._get_text_from_node(node_with_score.node)
-            response_builder.add_node_as_source(
-                node_with_score.node, similarity=node_with_score.score
-            )
-            if self._optimizer is not None:
-                text = TextChunk(text=self._optimizer.optimize(query_bundle, text.text))
-            response_builder.add_text_chunks([text])
-
-        # from recursive
-        if additional_source_nodes is not None:
-            for node in additional_source_nodes:
-                response_builder.add_node_with_score(node)
+        if self.child_branch_factor == 1:
+            query_template = self.query_template.partial_format(
+                num_chunks=len(cur_node_list), query_str=query_str
+            )
+            numbered_node_text = (
+                self._service_context.prompt_helper.get_numbered_text_from_nodes(
+                    cur_node_list, prompt=query_template
+                )
+            )
+            (
+                response,
+                formatted_query_prompt,
+            ) = self._service_context.llm_predictor.predict(
+                query_template,
+                context_list=numbered_node_text,
+            )
+        else:
+            query_template_multiple = self.query_template_multiple.partial_format(
+                num_chunks=len(cur_node_list),
+                query_str=query_str,
+                branching_factor=self.child_branch_factor,
+            )
+            numbered_node_text = (
+                self._service_context.prompt_helper.get_numbered_text_from_nodes(
+                    cur_node_list, prompt=query_template_multiple
+                )
+            )
+            (
+                response,
+                formatted_query_prompt,
+            ) = self._service_context.llm_predictor.predict(
+                query_template_multiple,
+                context_list=numbered_node_text,
+            )
 
-    def _prepare_response_output(
-        self,
-        response_builder: ResponseBuilder,
-        response_str: Optional[RESPONSE_TEXT_TYPE],
-        tuples: List[NodeWithScore],
-    ) -> RESPONSE_TYPE:
-        """Prepare response object from response string."""
-        response_extra_info = self._get_extra_info_for_response(
-            [node_with_score.node for node_with_score in tuples]
+        logger.debug(
+            f">[Level {level}] current prompt template: {formatted_query_prompt}"
+        )
+        self._service_context.llama_logger.add_log(
+            {"formatted_prompt_template": formatted_query_prompt, "level": level}
         )
+        debug_str = f">[Level {level}] Current response: {response}"
+        logger.debug(debug_str)
+        if self._verbose:
+            print_text(debug_str, end="\n")
 
-        if response_str is None or isinstance(response_str, str):
-            return Response(
-                response_str,
-                source_nodes=response_builder.get_sources(),
-                extra_info=response_extra_info,
-            )
-        elif response_str is None or isinstance(response_str, Generator):
-            return StreamingResponse(
-                response_str,
-                source_nodes=response_builder.get_sources(),
-                extra_info=response_extra_info,
+        numbers = extract_numbers_given_response(response, n=self.child_branch_factor)
+        if numbers is None:
+            debug_str = (
+                f">[Level {level}] Could not retrieve response - no numbers present"
             )
-        else:
-            raise ValueError("Response must be a string or a generator.")
+            logger.debug(debug_str)
+            if self._verbose:
+                print_text(debug_str, end="\n")
+            # just join text from current nodes as response
+            return []
+
+        selected_nodes = []
+        for number_str in numbers:
+            number = int(number_str)
+            if number > len(cur_node_list):
+                logger.debug(
+                    f">[Level {level}] Invalid response: {response} - "
+                    f"number {number} out of range"
+                )
+                continue
+
+            # number is 1-indexed, so subtract 1
+            selected_node = cur_node_list[number - 1]
+
+            info_str = (
+                f">[Level {level}] Selected node: "
+                f"[{number}]/[{','.join([str(int(n)) for n in numbers])}]"
+            )
+            logger.info(info_str)
+            if self._verbose:
+                print_text(info_str, end="\n")
+            debug_str = " ".join(selected_node.get_text().splitlines())
+            full_debug_str = (
+                f">[Level {level}] Node "
+                f"[{number}] Summary text: "
+                f"{ selected_node.get_text() }"
+            )
+            logger.debug(full_debug_str)
+            if self._verbose:
+                print_text(full_debug_str, end="\n")
+            selected_nodes.append(selected_node)
+
+        return selected_nodes
 
-    def synthesize(
+    def _retrieve_level(
         self,
+        cur_node_ids: Dict[int, str],
         query_bundle: QueryBundle,
-        nodes: List[NodeWithScore],
-        additional_source_nodes: Optional[List[NodeWithScore]] = None,
-    ) -> RESPONSE_TYPE:
-        # prepare response builder
-        self._prepare_response_builder(
-            self.response_builder,
-            query_bundle,
-            nodes,
-            additional_source_nodes=additional_source_nodes,
-        )
+        level: int = 0,
+    ) -> List[Node]:
+        """Answer a query recursively."""
+        cur_nodes = {
+            index: self._docstore.get_node(node_id)
+            for index, node_id in cur_node_ids.items()
+        }
+        cur_node_list = get_sorted_node_list(cur_nodes)
 
-        if self._response_mode != ResponseMode.NO_TEXT:
-            response_str = self._give_response_for_nodes(
-                self.response_builder, query_bundle.query_str
+        if len(cur_node_list) > self.child_branch_factor:
+            selected_nodes = self._select_nodes(
+                cur_node_list,
+                query_bundle,
+                level=level,
             )
         else:
-            response_str = None
+            selected_nodes = cur_node_list
 
-        return self._prepare_response_output(self.response_builder, response_str, nodes)
+        children_nodes = {}
+        for node in selected_nodes:
+            node_dict = self._index_struct.get_children(node)
+            children_nodes.update(node_dict)
+
+        if len(children_nodes) == 0:
+            # NOTE: leaf level
+            return selected_nodes
+        else:
+            return self._retrieve_level(children_nodes, query_bundle, level + 1)
 
-    async def asynthesize(
+    @llm_token_counter("retrieve")
+    def _retrieve(
         self,
         query_bundle: QueryBundle,
-        nodes: List[NodeWithScore],
-        additional_source_nodes: Optional[List[NodeWithScore]] = None,
-    ) -> RESPONSE_TYPE:
-        # define a response builder for async queries
-        response_builder = ResponseBuilder(
-            self._service_context,
-            self.text_qa_template,
-            self.refine_template,
-            use_async=self._use_async,
-            streaming=self._streaming,
-        )
-        # prepare response builder
-        self._prepare_response_builder(
-            response_builder,
+    ) -> List[NodeWithScore]:
+        """Get nodes for response."""
+        nodes = self._retrieve_level(
+            self._index_struct.root_nodes,
             query_bundle,
-            nodes,
-            additional_source_nodes=additional_source_nodes,
+            level=0,
         )
-
-        if self._response_mode != ResponseMode.NO_TEXT:
-            response_str = await self._agive_response_for_nodes(
-                response_builder, query_bundle.query_str
-            )
-        else:
-            response_str = None
-
-        return self._prepare_response_output(response_builder, response_str, nodes)
-
-    def _query(self, query_bundle: QueryBundle) -> RESPONSE_TYPE:
-        """Answer a query."""
-        # TODO: remove _query and just use query
-        nodes = self.retrieve(query_bundle)
-        return self.synthesize(query_bundle, nodes)
-
-    async def _aquery(self, query_bundle: QueryBundle) -> RESPONSE_TYPE:
-        """Answer a query asynchronously."""
-        # TODO: remove _query and just use query
-        nodes = self.retrieve(query_bundle)
-        response = await self.asynthesize(query_bundle, nodes)
-        return response
-
-    @llm_token_counter("query")
-    def query(self, query_bundle: QueryBundle) -> RESPONSE_TYPE:
-        """Answer a query."""
-        # TODO: support include summary
-        return self._query(query_bundle)
-
-    @llm_token_counter("query")
-    async def aquery(self, query_bundle: QueryBundle) -> RESPONSE_TYPE:
-        """Answer a query."""
-        # TODO: support include summary
-        return await self._aquery(query_bundle)
+        return [NodeWithScore(node) for node in nodes]
```

### Comparing `llama_index-0.5.9/llama_index/indices/query/query_transform/base.py` & `llama_index-0.6.0a1/llama_index/indices/query/query_transform/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import dataclasses
 from abc import abstractmethod
 from typing import Dict, Optional, Union, cast
 
 from langchain.input import print_text
 
-from llama_index.data_structs.data_structs_v2 import V2IndexStruct as IndexStruct
 from llama_index.indices.query.query_transform.prompts import (
     DEFAULT_DECOMPOSE_QUERY_TRANSFORM_PROMPT,
     DEFAULT_IMAGE_OUTPUT_PROMPT,
     DEFAULT_STEP_DECOMPOSE_QUERY_TRANSFORM_PROMPT,
     DecomposeQueryTransformPrompt,
     ImageOutputQueryTransformPrompt,
     StepDecomposeQueryTransformPrompt,
@@ -145,27 +144,24 @@
         self._decompose_query_prompt = (
             decompose_query_prompt or DEFAULT_DECOMPOSE_QUERY_TRANSFORM_PROMPT
         )
         self.verbose = verbose
 
     def _run(self, query_bundle: QueryBundle, extra_info: Dict) -> QueryBundle:
         """Run query transform."""
-        index_struct = cast(IndexStruct, extra_info.get("index_struct", None))
         # currently, just get text from the index structure
-        index_text = (
-            index_struct.get_summary() if index_struct.summary is not None else "None"
-        )
+        index_summary = cast(str, extra_info.get("index_summary", "None"))
 
         # given the text from the index, we can use the query bundle to generate
         # a new query bundle
         query_str = query_bundle.query_str
         new_query_str, _ = self._llm_predictor.predict(
             self._decompose_query_prompt,
             query_str=query_str,
-            context_str=index_text,
+            context_str=index_summary,
         )
 
         if self.verbose:
             print_text(f"> Current query: {query_str}\n", color="yellow")
             print_text(f"> New query: {new_query_str}\n", color="pink")
 
         return QueryBundle(
@@ -233,27 +229,29 @@
         self._step_decompose_query_prompt = (
             step_decompose_query_prompt or DEFAULT_STEP_DECOMPOSE_QUERY_TRANSFORM_PROMPT
         )
         self.verbose = verbose
 
     def _run(self, query_bundle: QueryBundle, extra_info: Dict) -> QueryBundle:
         """Run query transform."""
-        index_struct = cast(IndexStruct, extra_info.get("index_struct", None))
-        index_text = index_struct.get_summary()
+        index_summary = cast(
+            str,
+            extra_info.get("index_summary", "None"),
+        )
         prev_reasoning = cast(Response, extra_info.get("prev_reasoning"))
         fmt_prev_reasoning = f"\n{prev_reasoning}" if prev_reasoning else "None"
 
         # given the text from the index, we can use the query bundle to generate
         # a new query bundle
         query_str = query_bundle.query_str
         new_query_str, formatted_prompt = self._llm_predictor.predict(
             self._step_decompose_query_prompt,
             prev_reasoning=fmt_prev_reasoning,
             query_str=query_str,
-            context_str=index_text,
+            context_str=index_summary,
         )
         if self.verbose:
             print_text(f"> Current query: {query_str}\n", color="yellow")
             print_text(f"> Formatted prompt: {formatted_prompt}\n", color="pink")
             print_text(f"> New query: {new_query_str}\n", color="pink")
         return QueryBundle(
             query_str=new_query_str,
```

### Comparing `llama_index-0.5.9/llama_index/indices/query/query_transform/prompts.py` & `llama_index-0.6.0a1/llama_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/indices/response/builder.py` & `llama_index-0.6.0a1/llama_index/indices/response/response_builder.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,75 +3,60 @@
 This class provides general functions for taking in a set of text
 and generating a response.
 
 Will support different modes, from 1) stuffing chunks into prompt,
 2) create and refine separately over each chunk, 3) tree summarization.
 
 """
+from abc import ABC, abstractmethod
 import logging
-from dataclasses import dataclass
-from enum import Enum
-from typing import Any, Dict, Generator, List, Optional, Tuple, cast
+from typing import Any, Dict, Generator, List, Optional, Sequence, Tuple, cast
 
 from llama_index.data_structs.data_structs_v2 import IndexGraph
-from llama_index.data_structs.node_v2 import Node, NodeWithScore
-from llama_index.docstore import DocumentStore
+from llama_index.data_structs.node_v2 import Node
+from llama_index.storage.docstore.registry import get_default_docstore
 from llama_index.indices.common_tree.base import GPTTreeIndexBuilder
+from llama_index.indices.response.type import ResponseMode
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.utils import get_sorted_node_list, truncate_text
-from llama_index.logger.base import LlamaLogger
-from llama_index.prompts.prompts import QuestionAnswerPrompt, RefinePrompt, SummaryPrompt
+from llama_index.prompts.default_prompt_selectors import DEFAULT_REFINE_PROMPT_SEL
+from llama_index.prompts.default_prompts import (
+    DEFAULT_SIMPLE_INPUT_PROMPT,
+    DEFAULT_TEXT_QA_PROMPT,
+)
+from llama_index.prompts.prompts import (
+    QuestionAnswerPrompt,
+    RefinePrompt,
+    SimpleInputPrompt,
+    SummaryPrompt,
+)
 from llama_index.response.utils import get_response_text
+from llama_index.token_counter.token_counter import llm_token_counter
 from llama_index.types import RESPONSE_TEXT_TYPE
 from llama_index.utils import temp_set_attrs
 
 logger = logging.getLogger(__name__)
 
 
-class ResponseMode(str, Enum):
-    """Response modes."""
-
-    DEFAULT = "default"
-    COMPACT = "compact"
-    TREE_SUMMARIZE = "tree_summarize"
-    NO_TEXT = "no_text"
-
-
-@dataclass
-class TextChunk:
-    """Response chunk."""
-
-    text: str
-    # Whether this chunk is already a response
-    is_answer: bool = False
-
-
-class ResponseBuilder:
+class BaseResponseBuilder(ABC):
     """Response builder class."""
 
     def __init__(
         self,
         service_context: ServiceContext,
-        text_qa_template: QuestionAnswerPrompt,
-        refine_template: RefinePrompt,
-        texts: Optional[List[TextChunk]] = None,
-        nodes: Optional[List[Node]] = None,
-        use_async: bool = False,
         streaming: bool = False,
     ) -> None:
         """Init params."""
         self._service_context = service_context
-        self.text_qa_template = text_qa_template
-        self.refine_template = refine_template
-        self._texts = texts or []
-        nodes = nodes or []
-        self.source_nodes: List[NodeWithScore] = [NodeWithScore(node) for node in nodes]
-        self._use_async = use_async
         self._streaming = streaming
 
+    @property
+    def service_context(self) -> ServiceContext:
+        return self._service_context
+
     def _log_prompt_and_response(
         self,
         formatted_prompt: str,
         response: RESPONSE_TEXT_TYPE,
         log_prefix: str = "",
     ) -> None:
         """Log prompt and response from LLM."""
@@ -80,91 +65,96 @@
             {"formatted_prompt_template": formatted_prompt}
         )
         logger.debug(f"> {log_prefix} response: {response}")
         self._service_context.llama_logger.add_log(
             {f"{log_prefix.lower()}_response": response or "Empty Response"}
         )
 
-    def add_text_chunks(self, text_chunks: List[TextChunk]) -> None:
-        """Add text chunk."""
-        self._texts.extend(text_chunks)
-
-    def reset(self) -> None:
-        """Clear text chunks."""
-        self._texts = []
-        self.source_nodes = []
+    @abstractmethod
+    @llm_token_counter("get_response")
+    def get_response(
+        self,
+        query_str: str,
+        text_chunks: Sequence[str],
+        prev_response: Optional[str] = None,
+        **response_kwargs: Any,
+    ) -> RESPONSE_TEXT_TYPE:
+        """Get response."""
+        ...
 
-    def add_node_as_source(
-        self, node: Node, similarity: Optional[float] = None
-    ) -> None:
-        """Add node."""
-        self.add_node_with_score(NodeWithScore(node=node, score=similarity))
+    @abstractmethod
+    @llm_token_counter("aget_response")
+    async def aget_response(
+        self,
+        query_str: str,
+        text_chunks: Sequence[str],
+        prev_response: Optional[str] = None,
+        **response_kwargs: Any,
+    ) -> RESPONSE_TEXT_TYPE:
+        """Get response."""
+        ...
 
-    def add_node_with_score(self, node_with_score: NodeWithScore) -> None:
-        """Add source node directly."""
-        self.source_nodes.append(node_with_score)
-
-    def get_sources(self) -> List[NodeWithScore]:
-        """Get sources."""
-        return self.source_nodes
-
-    def get_logger(self) -> LlamaLogger:
-        """Get logger."""
-        return self._service_context.llama_logger
 
-    def refine_response_single(
+class Refine(BaseResponseBuilder):
+    def __init__(
+        self,
+        service_context: ServiceContext,
+        text_qa_template: QuestionAnswerPrompt,
+        refine_template: RefinePrompt,
+        streaming: bool = False,
+    ) -> None:
+        super().__init__(service_context=service_context, streaming=streaming)
+        self.text_qa_template = text_qa_template
+        self._refine_template = refine_template
+
+    @llm_token_counter("aget_response")
+    async def aget_response(
         self,
-        response: RESPONSE_TEXT_TYPE,
         query_str: str,
-        text_chunk: str,
+        text_chunks: Sequence[str],
+        prev_response: Optional[str] = None,
+        **response_kwargs: Any,
     ) -> RESPONSE_TEXT_TYPE:
-        """Refine response."""
-        # TODO: consolidate with logic in response/schema.py
-        if isinstance(response, Generator):
-            response = get_response_text(response)
+        return self.get_response(query_str, text_chunks, prev_response)
 
-        fmt_text_chunk = truncate_text(text_chunk, 50)
-        logger.debug(f"> Refine context: {fmt_text_chunk}")
-        # NOTE: partial format refine template with query_str and existing_answer here
-        refine_template = self.refine_template.partial_format(
-            query_str=query_str, existing_answer=response
-        )
-        refine_text_splitter = (
-            self._service_context.prompt_helper.get_text_splitter_given_prompt(
-                refine_template, 1
-            )
-        )
-        text_chunks = refine_text_splitter.split_text(text_chunk)
-        for cur_text_chunk in text_chunks:
-            if not self._streaming:
-                (
-                    response,
-                    formatted_prompt,
-                ) = self._service_context.llm_predictor.predict(
-                    refine_template,
-                    context_msg=cur_text_chunk,
+    @llm_token_counter("get_response")
+    def get_response(
+        self,
+        query_str: str,
+        text_chunks: Sequence[str],
+        prev_response: Optional[str] = None,
+        **response_kwargs: Any,
+    ) -> RESPONSE_TEXT_TYPE:
+        """Give response over chunks."""
+        prev_response_obj = cast(Optional[RESPONSE_TEXT_TYPE], prev_response)
+        response: Optional[RESPONSE_TEXT_TYPE] = None
+        for text_chunk in text_chunks:
+            if prev_response_obj is None:
+                # if this is the first chunk, and text chunk already
+                # is an answer, then return it
+                response = self._give_response_single(
+                    query_str,
+                    text_chunk,
                 )
             else:
-                response, formatted_prompt = self._service_context.llm_predictor.stream(
-                    refine_template,
-                    context_msg=cur_text_chunk,
+                response = self._refine_response_single(
+                    prev_response_obj, query_str, text_chunk
                 )
-            refine_template = self.refine_template.partial_format(
-                query_str=query_str, existing_answer=response
-            )
-
-            self._log_prompt_and_response(
-                formatted_prompt, response, log_prefix="Refined"
-            )
+            prev_response_obj = response
+        if isinstance(response, str):
+            response = response or "Empty Response"
+        else:
+            response = cast(Generator, response)
         return response
 
-    def give_response_single(
+    def _give_response_single(
         self,
         query_str: str,
         text_chunk: str,
+        **response_kwargs: Any,
     ) -> RESPONSE_TEXT_TYPE:
         """Give response given a query and a corresponding text chunk."""
         text_qa_template = self.text_qa_template.partial_format(query_str=query_str)
         qa_text_splitter = (
             self._service_context.prompt_helper.get_text_splitter_given_prompt(
                 text_qa_template, 1
             )
@@ -189,227 +179,443 @@
                     text_qa_template,
                     context_str=cur_text_chunk,
                 )
                 self._log_prompt_and_response(
                     formatted_prompt, response, log_prefix="Initial"
                 )
             else:
-                response = self.refine_response_single(
+                response = self._refine_response_single(
                     cast(RESPONSE_TEXT_TYPE, response),
                     query_str,
                     cur_text_chunk,
                 )
         if isinstance(response, str):
             response = response or "Empty Response"
         else:
             response = cast(Generator, response)
         return response
 
-    def get_response_over_chunks(
+    def _refine_response_single(
         self,
+        response: RESPONSE_TEXT_TYPE,
         query_str: str,
-        text_chunks: List[TextChunk],
-        prev_response: Optional[str] = None,
+        text_chunk: str,
+        **response_kwargs: Any,
     ) -> RESPONSE_TEXT_TYPE:
-        """Give response over chunks."""
-        prev_response_obj = cast(Optional[RESPONSE_TEXT_TYPE], prev_response)
-        response: Optional[RESPONSE_TEXT_TYPE] = None
-        for text_chunk in text_chunks:
-            if prev_response_obj is None:
-                # if this is the first chunk, and text chunk already
-                # is an answer, then return it
-                if text_chunk.is_answer:
-                    response = text_chunk.text
-                # otherwise give response
-                else:
-                    response = self.give_response_single(
-                        query_str,
-                        text_chunk.text,
-                    )
+        """Refine response."""
+        # TODO: consolidate with logic in response/schema.py
+        if isinstance(response, Generator):
+            response = get_response_text(response)
+
+        fmt_text_chunk = truncate_text(text_chunk, 50)
+        logger.debug(f"> Refine context: {fmt_text_chunk}")
+        # NOTE: partial format refine template with query_str and existing_answer here
+        refine_template = self._refine_template.partial_format(
+            query_str=query_str, existing_answer=response
+        )
+        refine_text_splitter = (
+            self._service_context.prompt_helper.get_text_splitter_given_prompt(
+                refine_template, 1
+            )
+        )
+        text_chunks = refine_text_splitter.split_text(text_chunk)
+        for cur_text_chunk in text_chunks:
+            if not self._streaming:
+                (
+                    response,
+                    formatted_prompt,
+                ) = self._service_context.llm_predictor.predict(
+                    refine_template,
+                    context_msg=cur_text_chunk,
+                )
             else:
-                response = self.refine_response_single(
-                    prev_response_obj, query_str, text_chunk.text
+                response, formatted_prompt = self._service_context.llm_predictor.stream(
+                    refine_template,
+                    context_msg=cur_text_chunk,
                 )
-            prev_response_obj = response
-        if isinstance(response, str):
-            response = response or "Empty Response"
-        else:
-            response = cast(Generator, response)
+            refine_template = self._refine_template.partial_format(
+                query_str=query_str, existing_answer=response
+            )
+
+            self._log_prompt_and_response(
+                formatted_prompt, response, log_prefix="Refined"
+            )
         return response
 
-    def _get_response_default(
-        self, query_str: str, prev_response: Optional[str]
-    ) -> RESPONSE_TEXT_TYPE:
-        return self.get_response_over_chunks(
-            query_str, self._texts, prev_response=prev_response
+
+class CompactAndRefine(Refine):
+    def __init__(
+        self,
+        service_context: ServiceContext,
+        text_qa_template: QuestionAnswerPrompt,
+        refine_template: RefinePrompt,
+        streaming: bool = False,
+    ) -> None:
+        super().__init__(
+            service_context=service_context,
+            text_qa_template=text_qa_template,
+            refine_template=refine_template,
+            streaming=streaming,
         )
 
-    def _get_response_compact(
-        self, query_str: str, prev_response: Optional[str]
+    @llm_token_counter("aget_response")
+    async def aget_response(
+        self,
+        query_str: str,
+        text_chunks: Sequence[str],
+        prev_response: Optional[str] = None,
+        **response_kwargs: Any,
+    ) -> RESPONSE_TEXT_TYPE:
+        return self.get_response(query_str, text_chunks, prev_response)
+
+    @llm_token_counter("get_response")
+    def get_response(
+        self,
+        query_str: str,
+        text_chunks: Sequence[str],
+        prev_response: Optional[str] = None,
+        **response_kwargs: Any,
     ) -> RESPONSE_TEXT_TYPE:
         """Get compact response."""
         # use prompt helper to fix compact text_chunks under the prompt limitation
         # TODO: This is a temporary fix - reason it's temporary is that
         # the refine template does not account for size of previous answer.
         text_qa_template = self.text_qa_template.partial_format(query_str=query_str)
-        refine_template = self.refine_template.partial_format(query_str=query_str)
+        refine_template = self._refine_template.partial_format(query_str=query_str)
 
         max_prompt = self._service_context.prompt_helper.get_biggest_prompt(
             [text_qa_template, refine_template]
         )
         with temp_set_attrs(
             self._service_context.prompt_helper, use_chunk_size_limit=False
         ):
             new_texts = self._service_context.prompt_helper.compact_text_chunks(
-                max_prompt, [t.text for t in self._texts]
+                max_prompt, text_chunks
             )
-            new_text_chunks = [TextChunk(text=t) for t in new_texts]
-            response = self.get_response_over_chunks(
-                query_str, new_text_chunks, prev_response=prev_response
+            response = super().get_response(
+                query_str=query_str, text_chunks=new_texts, prev_response=prev_response
             )
         return response
 
-    def _get_tree_index_builder_and_nodes(
-        self,
-        summary_template: SummaryPrompt,
-        query_str: str,
-        num_children: int = 10,
-    ) -> Tuple[GPTTreeIndexBuilder, List[Node]]:
-        """Get tree index builder."""
-        # first join all the text chunks into a single text
-        all_text = "\n\n".join([t.text for t in self._texts])
-        # then get text splitter
-        text_splitter = (
-            self._service_context.prompt_helper.get_text_splitter_given_prompt(
-                summary_template, num_children
-            )
-        )
-        text_chunks = text_splitter.split_text(all_text)
-        nodes = [Node(text=t) for t in text_chunks]
 
-        docstore = DocumentStore()
-        docstore.add_documents(nodes, allow_update=False)
-        index_builder = GPTTreeIndexBuilder(
-            num_children,
-            summary_template,
-            service_context=self._service_context,
-            docstore=docstore,
-            use_async=self._use_async,
-        )
-        return index_builder, nodes
-
-    def _get_tree_response_over_root_nodes(
+class TreeSummarize(Refine):
+    def __init__(
         self,
-        query_str: str,
-        prev_response: Optional[str],
-        root_nodes: Dict[int, Node],
+        service_context: ServiceContext,
         text_qa_template: QuestionAnswerPrompt,
-    ) -> RESPONSE_TEXT_TYPE:
-        """Get response from tree builder over root nodes."""
-        node_list = get_sorted_node_list(root_nodes)
-        node_text = self._service_context.prompt_helper.get_text_from_nodes(
-            node_list, prompt=text_qa_template
-        )
-        # NOTE: the final response could be a string or a stream
-        response = self.get_response_over_chunks(
-            query_str,
-            [TextChunk(node_text)],
-            prev_response=prev_response,
+        refine_template: RefinePrompt,
+        streaming: bool = False,
+        use_async: bool = True,
+    ) -> None:
+        super().__init__(
+            service_context=service_context,
+            text_qa_template=text_qa_template,
+            refine_template=refine_template,
+            streaming=streaming,
         )
-        if isinstance(response, str):
-            response = response or "Empty Response"
-        return response
+        self._use_async = use_async
 
-    def _get_response_tree_summarize(
+    @llm_token_counter("aget_response")
+    async def aget_response(
         self,
         query_str: str,
-        prev_response: Optional[str],
+        text_chunks: Sequence[str],
+        prev_response: Optional[str] = None,
         num_children: int = 10,
+        **response_kwargs: Any,
     ) -> RESPONSE_TEXT_TYPE:
         """Get tree summarize response."""
         text_qa_template = self.text_qa_template.partial_format(query_str=query_str)
         summary_template = SummaryPrompt.from_prompt(text_qa_template)
 
         index_builder, nodes = self._get_tree_index_builder_and_nodes(
-            summary_template, query_str, num_children
+            summary_template, query_str, text_chunks, num_children
         )
         index_graph = IndexGraph()
         for node in nodes:
             index_graph.insert(node)
-        index_graph = index_builder.build_index_from_nodes(
+        index_graph = await index_builder.abuild_index_from_nodes(
             index_graph, index_graph.all_nodes, index_graph.all_nodes
         )
         root_node_ids = index_graph.root_nodes
         root_nodes = {
             index: index_builder.docstore.get_node(node_id)
             for index, node_id in root_node_ids.items()
         }
         return self._get_tree_response_over_root_nodes(
             query_str, prev_response, root_nodes, text_qa_template
         )
 
-    async def _aget_response_tree_summarize(
+    @llm_token_counter("get_response")
+    def get_response(
         self,
         query_str: str,
-        prev_response: Optional[str],
+        text_chunks: Sequence[str],
+        prev_response: Optional[str] = None,
         num_children: int = 10,
+        **response_kwargs: Any,
     ) -> RESPONSE_TEXT_TYPE:
         """Get tree summarize response."""
         text_qa_template = self.text_qa_template.partial_format(query_str=query_str)
         summary_template = SummaryPrompt.from_prompt(text_qa_template)
 
         index_builder, nodes = self._get_tree_index_builder_and_nodes(
-            summary_template, query_str, num_children
+            summary_template, query_str, text_chunks, num_children
         )
         index_graph = IndexGraph()
         for node in nodes:
             index_graph.insert(node)
-        index_graph = await index_builder.abuild_index_from_nodes(
+        index_graph = index_builder.build_index_from_nodes(
             index_graph, index_graph.all_nodes, index_graph.all_nodes
         )
         root_node_ids = index_graph.root_nodes
         root_nodes = {
             index: index_builder.docstore.get_node(node_id)
             for index, node_id in root_node_ids.items()
         }
         return self._get_tree_response_over_root_nodes(
             query_str, prev_response, root_nodes, text_qa_template
         )
 
-    def get_response(
+    def _get_tree_index_builder_and_nodes(
         self,
+        summary_template: SummaryPrompt,
         query_str: str,
+        text_chunks: Sequence[str],
+        num_children: int = 10,
+    ) -> Tuple[GPTTreeIndexBuilder, List[Node]]:
+        """Get tree index builder."""
+        # first join all the text chunks into a single text
+        all_text = "\n\n".join(text_chunks)
+
+        # then get text splitter
+        text_splitter = (
+            self._service_context.prompt_helper.get_text_splitter_given_prompt(
+                summary_template, num_children
+            )
+        )
+        text_chunks = text_splitter.split_text(all_text)
+        new_nodes = [Node(text=t) for t in text_chunks]
+
+        docstore = get_default_docstore()
+        docstore.add_documents(new_nodes, allow_update=False)
+        index_builder = GPTTreeIndexBuilder(
+            num_children,
+            summary_template,
+            service_context=self._service_context,
+            docstore=docstore,
+            use_async=self._use_async,
+        )
+        return index_builder, new_nodes
+
+    def _get_tree_response_over_root_nodes(
+        self,
+        query_str: str,
+        prev_response: Optional[str],
+        root_nodes: Dict[int, Node],
+        text_qa_template: QuestionAnswerPrompt,
+    ) -> RESPONSE_TEXT_TYPE:
+        """Get response from tree builder over root text_chunks."""
+        node_list = get_sorted_node_list(root_nodes)
+        node_text = self._service_context.prompt_helper.get_text_from_nodes(
+            node_list, prompt=text_qa_template
+        )
+        # NOTE: the final response could be a string or a stream
+        response = super().get_response(
+            query_str=query_str,
+            text_chunks=[node_text],
+            prev_response=prev_response,
+        )
+        if isinstance(response, str):
+            response = response or "Empty Response"
+        return response
+
+
+class SimpleSummarize(BaseResponseBuilder):
+    def __init__(
+        self,
+        service_context: ServiceContext,
+        text_qa_template: QuestionAnswerPrompt,
+        streaming: bool = False,
+    ) -> None:
+        super().__init__(service_context, streaming)
+        self._text_qa_template = text_qa_template
+
+    @llm_token_counter("aget_response")
+    async def aget_response(
+        self,
+        query_str: str,
+        text_chunks: Sequence[str],
         prev_response: Optional[str] = None,
-        mode: ResponseMode = ResponseMode.DEFAULT,
         **response_kwargs: Any,
     ) -> RESPONSE_TEXT_TYPE:
-        """Get response."""
-        if mode == ResponseMode.DEFAULT:
-            return self._get_response_default(query_str, prev_response)
-        elif mode == ResponseMode.COMPACT:
-            return self._get_response_compact(query_str, prev_response)
-        elif mode == ResponseMode.TREE_SUMMARIZE:
-            return self._get_response_tree_summarize(
-                query_str, prev_response, **response_kwargs
+        text_qa_template = self._text_qa_template.partial_format(query_str=query_str)
+        node_text = self._service_context.prompt_helper.get_text_from_nodes(
+            [Node(text=text) for text in text_chunks], prompt=text_qa_template
+        )
+
+        response: RESPONSE_TEXT_TYPE
+        if not self._streaming:
+            (
+                response,
+                formatted_prompt,
+            ) = await self._service_context.llm_predictor.apredict(
+                text_qa_template,
+                context_str=node_text,
+            )
+            self._log_prompt_and_response(formatted_prompt, response)
+        else:
+            response, formatted_prompt = self._service_context.llm_predictor.stream(
+                text_qa_template,
+                context_str=node_text,
+            )
+            self._log_prompt_and_response(formatted_prompt, response)
+        if isinstance(response, str):
+            response = response or "Empty Response"
+        else:
+            response = cast(Generator, response)
+
+        return response
+
+    @llm_token_counter("get_response")
+    def get_response(
+        self,
+        query_str: str,
+        text_chunks: Sequence[str],
+        prev_response: Optional[str] = None,
+        **kwargs: Any,
+    ) -> RESPONSE_TEXT_TYPE:
+        text_qa_template = self._text_qa_template.partial_format(query_str=query_str)
+        node_text = self._service_context.prompt_helper.get_text_from_nodes(
+            [Node(text=text) for text in text_chunks], prompt=text_qa_template
+        )
+
+        response: RESPONSE_TEXT_TYPE
+        if not self._streaming:
+            (response, formatted_prompt,) = self._service_context.llm_predictor.predict(
+                text_qa_template,
+                context_str=node_text,
+            )
+            self._log_prompt_and_response(formatted_prompt, response)
+        else:
+            response, formatted_prompt = self._service_context.llm_predictor.stream(
+                text_qa_template,
+                context_str=node_text,
             )
+            self._log_prompt_and_response(formatted_prompt, response)
+        if isinstance(response, str):
+            response = response or "Empty Response"
         else:
-            raise ValueError(f"Invalid mode: {mode}")
+            response = cast(Generator, response)
+
+        return response
+
+
+class Generation(BaseResponseBuilder):
+    def __init__(
+        self,
+        service_context: ServiceContext,
+        simple_template: Optional[SimpleInputPrompt] = None,
+        streaming: bool = False,
+    ) -> None:
+        super().__init__(service_context, streaming)
+        self._input_prompt = simple_template or DEFAULT_SIMPLE_INPUT_PROMPT
 
+    @llm_token_counter("aget_response")
     async def aget_response(
         self,
         query_str: str,
+        text_chunks: Sequence[str],
         prev_response: Optional[str] = None,
-        mode: ResponseMode = ResponseMode.DEFAULT,
         **response_kwargs: Any,
     ) -> RESPONSE_TEXT_TYPE:
-        """Get response."""
-        # NOTE: for default and compact response modes, return synchronous version
-        if mode == ResponseMode.DEFAULT:
-            return self._get_response_default(query_str, prev_response)
-        elif mode == ResponseMode.COMPACT:
-            return self._get_response_compact(query_str, prev_response)
-        elif mode == ResponseMode.TREE_SUMMARIZE:
-            return await self._aget_response_tree_summarize(
-                query_str, prev_response, **response_kwargs
+        # NOTE: ignore text chunks and previous response
+        del text_chunks
+        del prev_response
+
+        if not self._streaming:
+            response, _ = await self._service_context.llm_predictor.apredict(
+                self._input_prompt,
+                query_str=query_str,
+            )
+            return response
+        else:
+            stream_response, _ = self._service_context.llm_predictor.stream(
+                self._input_prompt,
+                query_str=query_str,
+            )
+            return stream_response
+
+    @llm_token_counter("get_response")
+    def get_response(
+        self,
+        query_str: str,
+        text_chunks: Sequence[str],
+        prev_response: Optional[str] = None,
+        **response_kwargs: Any,
+    ) -> RESPONSE_TEXT_TYPE:
+        # NOTE: ignore text chunks and previous response
+        del text_chunks
+        del prev_response
+
+        if not self._streaming:
+            response, _ = self._service_context.llm_predictor.predict(
+                self._input_prompt,
+                query_str=query_str,
             )
+            return response
         else:
-            raise ValueError(f"Invalid mode: {mode}")
+            stream_response, _ = self._service_context.llm_predictor.stream(
+                self._input_prompt,
+                query_str=query_str,
+            )
+            return stream_response
+
+
+def get_response_builder(
+    service_context: ServiceContext,
+    text_qa_template: Optional[QuestionAnswerPrompt] = None,
+    refine_template: Optional[RefinePrompt] = None,
+    simple_template: Optional[SimpleInputPrompt] = None,
+    mode: ResponseMode = ResponseMode.DEFAULT,
+    use_async: bool = False,
+    streaming: bool = False,
+) -> BaseResponseBuilder:
+    text_qa_template = text_qa_template or DEFAULT_TEXT_QA_PROMPT
+    refine_template = refine_template or DEFAULT_REFINE_PROMPT_SEL
+    simple_template = simple_template or DEFAULT_SIMPLE_INPUT_PROMPT
+    if mode == ResponseMode.DEFAULT:
+        return Refine(
+            service_context=service_context,
+            text_qa_template=text_qa_template,
+            refine_template=refine_template,
+            streaming=streaming,
+        )
+    elif mode == ResponseMode.COMPACT:
+        return CompactAndRefine(
+            service_context=service_context,
+            text_qa_template=text_qa_template,
+            refine_template=refine_template,
+            streaming=streaming,
+        )
+    elif mode == ResponseMode.TREE_SUMMARIZE:
+        return TreeSummarize(
+            service_context=service_context,
+            text_qa_template=text_qa_template,
+            refine_template=refine_template,
+            streaming=streaming,
+            use_async=use_async,
+        )
+    elif mode == ResponseMode.SIMPLE_SUMMARIZE:
+        return SimpleSummarize(
+            service_context=service_context,
+            text_qa_template=text_qa_template,
+            streaming=streaming,
+        )
+    elif mode == ResponseMode.GENERATION:
+        return Generation(
+            service_context=service_context,
+            simple_template=simple_template,
+            streaming=streaming,
+        )
+    else:
+        raise ValueError(f"Unknown mode: {mode}")
```

### Comparing `llama_index-0.5.9/llama_index/indices/service_context.py` & `llama_index-0.6.0a1/llama_index/indices/service_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/indices/struct_store/__init__.py` & `llama_index-0.6.0a1/llama_index/indices/struct_store/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Structured store indices."""
 
 from llama_index.indices.struct_store.pandas import GPTPandasIndex
-from llama_index.indices.struct_store.pandas_query import GPTNLPandasIndexQuery
+from llama_index.indices.struct_store.pandas_query import GPTNLPandasQueryEngine
 from llama_index.indices.struct_store.sql import (
     GPTSQLStructStoreIndex,
     SQLContextContainerBuilder,
 )
 from llama_index.indices.struct_store.sql_query import (
-    GPTNLStructStoreIndexQuery,
-    GPTSQLStructStoreIndexQuery,
+    GPTNLStructStoreQueryEngine,
+    GPTSQLStructStoreQueryEngine,
 )
 
 __all__ = [
     "GPTSQLStructStoreIndex",
     "SQLContextContainerBuilder",
     "GPTPandasIndex",
-    "GPTNLStructStoreIndexQuery",
-    "GPTSQLStructStoreIndexQuery",
-    "GPTNLPandasIndexQuery",
+    "GPTNLPandasQueryEngine",
+    "GPTNLStructStoreQueryEngine",
+    "GPTSQLStructStoreQueryEngine",
 ]
```

### Comparing `llama_index-0.5.9/llama_index/indices/struct_store/base.py` & `llama_index-0.6.0a1/llama_index/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/indices/struct_store/container_builder.py` & `llama_index-0.6.0a1/llama_index/indices/struct_store/container_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 )
 
 
 class SQLContextContainerBuilder:
     """SQLContextContainerBuilder.
 
     Build a SQLContextContainer that can be passed to the SQL index
-    during index construction or during queryt-time.
+    during index construction or during query-time.
 
     NOTE: if context_str is specified, that will be used as context
     instead of context_dict
 
     Args:
         sql_database (SQLDatabase): SQL database
         context_dict (Optional[Dict[str, str]]): context dict
@@ -134,15 +134,16 @@
             store_context_str (bool): store context_str
 
         """
         if query_tmpl is None:
             context_query_str = query_str
         else:
             context_query_str = query_tmpl.format(orig_query_str=query_str)
-        response = index.query(context_query_str, **index_kwargs)
+        query_engine = index.as_query_engine()
+        response = query_engine.query(context_query_str)
         context_str = str(response)
         if store_context_str:
             self.context_str = context_str
         return context_str
 
     def build_context_container(
         self, ignore_db_schema: bool = False
```

### Comparing `llama_index-0.5.9/llama_index/indices/struct_store/pandas_query.py` & `llama_index-0.6.0a1/llama_index/indices/struct_store/pandas_query.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import logging
 from typing import Any, Callable, Optional
 
 import pandas as pd
 from langchain.input import print_text
 
-from llama_index.data_structs.table_v2 import PandasStructTable
-from llama_index.indices.query.base import BaseGPTIndexQuery
+from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.query.schema import QueryBundle
+from llama_index.indices.struct_store.pandas import GPTPandasIndex
 from llama_index.prompts.default_prompts import DEFAULT_PANDAS_PROMPT
 from llama_index.prompts.prompts import PandasPrompt
 from llama_index.response.schema import Response
 
 logger = logging.getLogger(__name__)
 
 
@@ -60,55 +60,51 @@
             "There was an error running the output as Python code. "
             f"Error message: {e}"
         )
         traceback.print_exc()
         return err_string
 
 
-class GPTNLPandasIndexQuery(BaseGPTIndexQuery[PandasStructTable]):
+class GPTNLPandasQueryEngine(BaseQueryEngine):
     """GPT Pandas query.
 
     Convert natural language to Pandas python code.
 
-    .. code-block:: python
-
-        response = index.query("<query_str>", mode="default")
-
     Args:
         df (pd.DataFrame): Pandas dataframe to use.
         instruction_str (Optional[str]): Instruction string to use.
         output_processor (Optional[Callable[[str], str]]): Output processor.
             A callable that takes in the output string, pandas DataFrame,
             and any output kwargs and returns a string.
         pandas_prompt (Optional[PandasPrompt]): Pandas prompt to use.
         head (int): Number of rows to show in the table context.
 
     """
 
     def __init__(
         self,
-        index_struct: PandasStructTable,
-        df: Optional[pd.DataFrame] = None,
+        index: GPTPandasIndex,
         instruction_str: Optional[str] = None,
         output_processor: Optional[Callable] = None,
         pandas_prompt: Optional[PandasPrompt] = None,
         output_kwargs: Optional[dict] = None,
         head: int = 5,
+        verbose: bool = False,
         **kwargs: Any,
     ) -> None:
         """Initialize params."""
-        super().__init__(index_struct=index_struct, **kwargs)
-        if df is None:
-            raise ValueError("df must be provided.")
-        self.df = df
+        self.df = index.df
+        self._service_context = index.service_context
+
         self._head = head
         self._pandas_prompt = pandas_prompt or DEFAULT_PANDAS_PROMPT
         self._instruction_str = instruction_str or DEFAULT_INSTRUCTION_STR
         self._output_processor = output_processor or default_output_processor
         self._output_kwargs = output_kwargs or {}
+        self._verbose = verbose
 
     def _get_table_context(self) -> str:
         """Get table context."""
         return str(self.df.head(self._head))
 
     def _query(self, query_bundle: QueryBundle) -> Response:
         """Answer a query."""
@@ -131,7 +127,10 @@
             print_text(f"> Pandas Output: {pandas_output}\n")
 
         response_extra_info = {
             "pandas_instruction_str": pandas_response_str,
         }
 
         return Response(response=pandas_output, extra_info=response_extra_info)
+
+    async def _aquery(self, query_bundle: QueryBundle) -> Response:
+        return self._query(query_bundle)
```

### Comparing `llama_index-0.5.9/llama_index/indices/struct_store/sql_query.py` & `llama_index-0.6.0a1/llama_index/indices/struct_store/sql_query.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,102 +1,81 @@
 """Default query for GPTSQLStructStoreIndex."""
 import logging
 from typing import Any, Optional
 
-from llama_index.data_structs.table_v2 import SQLStructTable
-from llama_index.indices.common.struct_store.schema import SQLContextContainer
-from llama_index.indices.query.base import BaseGPTIndexQuery
-from llama_index.indices.query.schema import QueryBundle, QueryMode
-from llama_index.langchain_helpers.sql_wrapper import SQLDatabase
+from llama_index.indices.query.base import BaseQueryEngine
+from llama_index.indices.query.schema import QueryBundle
+from llama_index.indices.struct_store.container_builder import SQLContextContainerBuilder
+from llama_index.indices.struct_store.sql import GPTSQLStructStoreIndex
 from llama_index.prompts.default_prompts import DEFAULT_TEXT_TO_SQL_PROMPT
 from llama_index.prompts.prompts import TextToSQLPrompt
 from llama_index.response.schema import Response
 from llama_index.token_counter.token_counter import llm_token_counter
 
 logger = logging.getLogger(__name__)
 
 
-class GPTSQLStructStoreIndexQuery(BaseGPTIndexQuery[SQLStructTable]):
-    """GPT SQL query over a structured database.
+class GPTSQLStructStoreQueryEngine(BaseQueryEngine):
+    """GPT SQL query engine over a structured database.
 
     Runs raw SQL over a GPTSQLStructStoreIndex. No LLM calls are made here.
     NOTE: this query cannot work with composed indices - if the index
     contains subindices, those subindices will not be queried.
-
-    .. code-block:: python
-
-        response = index.query("<query_str>", mode="sql")
-
     """
 
     def __init__(
         self,
-        index_struct: SQLStructTable,
-        sql_database: Optional[SQLDatabase] = None,
-        sql_context_container: Optional[SQLContextContainer] = None,
+        index: GPTSQLStructStoreIndex,
+        sql_context_container: Optional[SQLContextContainerBuilder] = None,
         **kwargs: Any,
     ) -> None:
         """Initialize params."""
-        super().__init__(index_struct=index_struct, **kwargs)
-        if sql_database is None:
-            raise ValueError("sql_database must be provided.")
-        self._sql_database = sql_database
+        self._sql_database = index.sql_database
+        self._sql_context_container = (
+            sql_context_container or index.sql_context_container
+        )
 
-    @llm_token_counter("query")
-    def query(self, query_bundle: QueryBundle) -> Response:
+    def _query(self, query_bundle: QueryBundle) -> Response:
         """Answer a query."""
         # NOTE: override query method in order to fetch the right results.
         # NOTE: since the query_str is a SQL query, it doesn't make sense
         # to use ResponseBuilder anywhere.
         response_str, extra_info = self._sql_database.run_sql(query_bundle.query_str)
         response = Response(response=response_str, extra_info=extra_info)
         return response
 
-    @llm_token_counter("query")
-    async def aquery(self, query_bundle: QueryBundle) -> Response:
-        return self.query(query_bundle)
+    async def _aquery(self, query_bundle: QueryBundle) -> Response:
+        return self._query(query_bundle)
 
 
-class GPTNLStructStoreIndexQuery(BaseGPTIndexQuery[SQLStructTable]):
-    """GPT natural language query over a structured database.
+class GPTNLStructStoreQueryEngine(BaseQueryEngine):
+    """GPT natural language query engine over a structured database.
 
     Given a natural language query, we will extract the query to SQL.
     Runs raw SQL over a GPTSQLStructStoreIndex. No LLM calls are made during
     the SQL execution.
     NOTE: this query cannot work with composed indices - if the index
     contains subindices, those subindices will not be queried.
-
-    .. code-block:: python
-
-        response = index.query("<query_str>", mode="default")
-
     """
 
     def __init__(
         self,
-        index_struct: SQLStructTable,
-        sql_database: Optional[SQLDatabase] = None,
-        sql_context_container: Optional[SQLContextContainer] = None,
-        ref_doc_id_column: Optional[str] = None,
+        index: GPTSQLStructStoreIndex,
         text_to_sql_prompt: Optional[TextToSQLPrompt] = None,
-        context_query_mode: QueryMode = QueryMode.DEFAULT,
         context_query_kwargs: Optional[dict] = None,
         **kwargs: Any,
     ) -> None:
         """Initialize params."""
-        super().__init__(index_struct=index_struct, **kwargs)
-        if sql_database is None:
-            raise ValueError("sql_database must be provided.")
-        self._sql_database = sql_database
-        if sql_context_container is None:
-            raise ValueError("sql_context_container must be provided.")
-        self._sql_context_container = sql_context_container
-        self._ref_doc_id_column = ref_doc_id_column
+        self._index = index
+        self._sql_database = index.sql_database
+        self._sql_context_container = index.sql_context_container
+        self._service_context = index.service_context
+        self._ref_doc_id_column = index.ref_doc_id_column
+
         self._text_to_sql_prompt = text_to_sql_prompt or DEFAULT_TEXT_TO_SQL_PROMPT
-        self._context_query_mode = context_query_mode
         self._context_query_kwargs = context_query_kwargs or {}
 
     def _parse_response_to_sql(self, response: str) -> str:
         """Parse response to SQL."""
         result_response = response.strip()
         return result_response
 
@@ -119,14 +98,15 @@
                 )
             for table_desc in context_dict.values():
                 table_desc_list.append(table_desc)
             tables_desc_str = "\n\n".join(table_desc_list)
 
         return tables_desc_str
 
+    @llm_token_counter("query")
     def _query(self, query_bundle: QueryBundle) -> Response:
         """Answer a query."""
         table_desc_str = self._get_table_context(query_bundle)
         logger.info(f"> Table desc str: {table_desc_str}")
         response_str, _ = self._service_context.llm_predictor.predict(
             self._text_to_sql_prompt,
             query_str=query_bundle.query_str,
@@ -139,14 +119,15 @@
         logger.debug(f"> Predicted SQL query: {sql_query_str}")
 
         response_str, extra_info = self._sql_database.run_sql(sql_query_str)
         extra_info["sql_query"] = sql_query_str
         response = Response(response=response_str, extra_info=extra_info)
         return response
 
+    @llm_token_counter("aquery")
     async def _aquery(self, query_bundle: QueryBundle) -> Response:
         """Answer a query."""
         table_desc_str = self._get_table_context(query_bundle)
         logger.info(f"> Table desc str: {table_desc_str}")
         response_str, _ = await self._service_context.llm_predictor.apredict(
             self._text_to_sql_prompt,
             query_str=query_bundle.query_str,
```

### Comparing `llama_index-0.5.9/llama_index/indices/tree/embedding_query.py` & `llama_index-0.6.0a1/llama_index/indices/tree/select_leaf_embedding_retriever.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 """Query Tree using embedding similarity between query and node text."""
 
 import logging
-from typing import Any, Dict, List, Optional, Tuple, cast
+from typing import Dict, List, Tuple, cast
+
 
-from llama_index.data_structs.data_structs_v2 import IndexGraph
 from llama_index.data_structs.node_v2 import Node
 from llama_index.indices.query.schema import QueryBundle
-from llama_index.indices.tree.leaf_query import GPTTreeIndexLeafQuery
+from llama_index.indices.tree.select_leaf_retriever import (
+    TreeSelectLeafRetriever,
+)
 from llama_index.indices.utils import get_sorted_node_list
-from llama_index.prompts.prompts import TreeSelectMultiplePrompt, TreeSelectPrompt
 
 logger = logging.getLogger(__name__)
 
 
-class GPTTreeIndexEmbeddingQuery(GPTTreeIndexLeafQuery):
-    """
-    GPT Tree Index embedding query.
+class TreeSelectLeafEmbeddingRetriever(TreeSelectLeafRetriever):
+    """Tree select leaf embedding retriever.
 
     This class traverses the index graph using the embedding similarity between the
     query and the node text.
 
-    .. code-block:: python
-
-        response = index.query("<query_str>", mode="embedding")
-
     Args:
         query_template (Optional[TreeSelectPrompt]): Tree Select Query Prompt
             (see :ref:`Prompt-Templates`).
         query_template_multiple (Optional[TreeSelectMultiplePrompt]): Tree Select
             Query Prompt (Multiple)
             (see :ref:`Prompt-Templates`).
         text_qa_template (Optional[QuestionAnswerPrompt]): Question-Answer Prompt
@@ -39,32 +35,14 @@
             to traverse for any given parent node.
             If child_branch_factor is 2, then the query will choose two child nodes.
         embed_model (Optional[BaseEmbedding]): Embedding model to use for
             embedding similarity.
 
     """
 
-    def __init__(
-        self,
-        index_struct: IndexGraph,
-        query_template: Optional[TreeSelectPrompt] = None,
-        query_template_multiple: Optional[TreeSelectMultiplePrompt] = None,
-        child_branch_factor: int = 1,
-        **kwargs: Any,
-    ) -> None:
-        """Initialize params."""
-        super().__init__(
-            index_struct,
-            query_template=query_template,
-            query_template_multiple=query_template_multiple,
-            child_branch_factor=child_branch_factor,
-            **kwargs,
-        )
-        self.child_branch_factor = child_branch_factor
-
     def _query_level(
         self,
         cur_node_ids: Dict[int, str],
         query_bundle: QueryBundle,
         level: int = 0,
     ) -> str:
         """Answer a query recursively."""
```

### Comparing `llama_index-0.5.9/llama_index/indices/tree/inserter.py` & `llama_index-0.6.0a1/llama_index/indices/tree/inserter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """GPT Tree Index inserter."""
 
 from typing import Optional, Sequence
 
 from llama_index.data_structs.data_structs_v2 import IndexGraph
 from llama_index.data_structs.node_v2 import Node
-from llama_index.docstore import DocumentStore
+from llama_index.storage.docstore import BaseDocumentStore
+from llama_index.storage.docstore.registry import get_default_docstore
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.utils import extract_numbers_given_response, get_sorted_node_list
 from llama_index.prompts.base import Prompt
 from llama_index.prompts.default_prompts import (
     DEFAULT_INSERT_PROMPT,
     DEFAULT_SUMMARY_PROMPT,
 )
@@ -20,25 +21,25 @@
     def __init__(
         self,
         index_graph: IndexGraph,
         service_context: ServiceContext,
         num_children: int = 10,
         insert_prompt: Prompt = DEFAULT_INSERT_PROMPT,
         summary_prompt: Prompt = DEFAULT_SUMMARY_PROMPT,
-        docstore: Optional[DocumentStore] = None,
+        docstore: Optional[BaseDocumentStore] = None,
     ) -> None:
         """Initialize with params."""
         if num_children < 2:
             raise ValueError("Invalid number of children.")
         self.num_children = num_children
         self.summary_prompt = summary_prompt
         self.insert_prompt = insert_prompt
         self.index_graph = index_graph
         self._service_context = service_context
-        self._docstore = docstore or DocumentStore()
+        self._docstore = docstore or get_default_docstore()
 
     def _insert_under_parent_and_consolidate(
         self, text_node: Node, parent_node: Optional[Node]
     ) -> None:
         """Insert node under parent and consolidate.
 
         Consolidation will happen by dividing up child nodes, and creating a new
@@ -151,9 +152,11 @@
                 self.summary_prompt, context_str=text_chunk
             )
 
             parent_node.text = new_summary
 
     def insert(self, nodes: Sequence[Node]) -> None:
         """Insert into index_graph."""
+        print("calling insert")
+        print(nodes)
         for node in nodes:
             self._insert_node(node)
```

### Comparing `llama_index-0.5.9/llama_index/indices/tree/summarize_query.py` & `llama_index-0.6.0a1/llama_index/indices/tree/all_leaf_retriever.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,48 @@
 """Summarize query."""
 
 import logging
-from typing import Any, List, Optional, cast
+from typing import Any, List, cast
+
 
 from llama_index.data_structs.data_structs_v2 import IndexGraph
-from llama_index.data_structs.node_v2 import Node
-from llama_index.indices.query.base import BaseGPTIndexQuery
-from llama_index.indices.query.embedding_utils import SimilarityTracker
+from llama_index.data_structs.node_v2 import NodeWithScore
+from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.schema import QueryBundle
-from llama_index.indices.response.builder import ResponseMode
 from llama_index.indices.utils import get_sorted_node_list
 
 logger = logging.getLogger(__name__)
 
+DEFAULT_NUM_CHILDREN = 10
+
 
-class GPTTreeIndexSummarizeQuery(BaseGPTIndexQuery[IndexGraph]):
-    """GPT Tree Index summarize query.
+class TreeAllLeafRetriever(BaseRetriever):
+    """GPT all leaf retriever.
 
     This class builds a query-specific tree from leaf nodes to return a response.
     Using this query mode means that the tree index doesn't need to be built
     when initialized, since we rebuild the tree for each query.
 
-    .. code-block:: python
-
-        response = index.query("<query_str>", mode="summarize")
-
     Args:
         text_qa_template (Optional[QuestionAnswerPrompt]): Question-Answer Prompt
             (see :ref:`Prompt-Templates`).
 
     """
 
-    def __init__(
-        self,
-        index_struct: IndexGraph,
-        num_children: int = 10,
-        **kwargs: Any,
-    ) -> None:
-        """Initialize params."""
-        if "response_mode" in kwargs:
-            raise ValueError(
-                "response_mode should not be specified for summarize query"
-            )
-        response_kwargs = kwargs.pop("response_kwargs", {})
-        response_kwargs.update(num_children=num_children)
-        super().__init__(
-            index_struct,
-            response_mode=ResponseMode.TREE_SUMMARIZE,
-            response_kwargs=response_kwargs,
-            **kwargs,
-        )
+    def __init__(self, index: Any):
+        from llama_index.indices.tree.base import GPTTreeIndex
+
+        assert isinstance(index, GPTTreeIndex)
+        self._index = index
+        self._index_struct = index.index_struct
+        self._docstore = index.docstore
 
     def _retrieve(
         self,
         query_bundle: QueryBundle,
-        similarity_tracker: Optional[SimilarityTracker] = None,
-    ) -> List[Node]:
+    ) -> List[NodeWithScore]:
         """Get nodes for response."""
         logger.info(f"> Starting query: {query_bundle.query_str}")
         index_struct = cast(IndexGraph, self._index_struct)
         all_nodes = self._docstore.get_node_dict(index_struct.all_nodes)
         sorted_node_list = get_sorted_node_list(all_nodes)
-        return sorted_node_list
+        return [NodeWithScore(node) for node in sorted_node_list]
```

### Comparing `llama_index-0.5.9/llama_index/indices/utils.py` & `llama_index-0.6.0a1/llama_index/indices/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/indices/vector_store/base.py` & `llama_index-0.6.0a1/llama_index/indices/vector_store/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,72 +3,61 @@
 An index that that is built on top of an existing vector store.
 
 """
 
 from typing import Any, Dict, List, Optional, Sequence, Set, Tuple
 
 from llama_index.async_utils import run_async_tasks
-from llama_index.constants import VECTOR_STORE_KEY
 from llama_index.data_structs.data_structs_v2 import IndexDict
 from llama_index.data_structs.node_v2 import ImageNode, IndexNode, Node
-from llama_index.indices.base import BaseGPTIndex, QueryMap
-from llama_index.indices.query.schema import QueryMode
+from llama_index.indices.base import BaseGPTIndex
+from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.service_context import ServiceContext
-from llama_index.indices.vector_store.base_query import GPTVectorStoreIndexQuery
+from llama_index.storage.storage_context import StorageContext
 from llama_index.token_counter.token_counter import llm_token_counter
-from llama_index.vector_stores.registry import (
-    load_vector_store_from_dict,
-    save_vector_store_to_dict,
-)
-from llama_index.vector_stores.simple import SimpleVectorStore
 from llama_index.vector_stores.types import NodeEmbeddingResult, VectorStore
 
 
 class GPTVectorStoreIndex(BaseGPTIndex[IndexDict]):
     """Base GPT Vector Store Index.
 
     Args:
-        embed_model (Optional[BaseEmbedding]): Embedding model to use for
-            embedding similarity.
-        vector_store (Optional[VectorStore]): Vector store to use for
-            embedding similarity. See :ref:`Ref-Indices-VectorStore-Stores`
-            for more details.
         use_async (bool): Whether to use asynchronous calls. Defaults to False.
-
     """
 
     index_struct_cls = IndexDict
 
     def __init__(
         self,
         nodes: Optional[Sequence[Node]] = None,
         index_struct: Optional[IndexDict] = None,
         service_context: Optional[ServiceContext] = None,
-        vector_store: Optional[VectorStore] = None,
+        storage_context: Optional[StorageContext] = None,
         use_async: bool = False,
         **kwargs: Any,
     ) -> None:
         """Initialize params."""
-        self._vector_store = vector_store or SimpleVectorStore()
-
         self._use_async = use_async
         super().__init__(
             nodes=nodes,
             index_struct=index_struct,
             service_context=service_context,
+            storage_context=storage_context,
             **kwargs,
         )
 
-    @classmethod
-    def get_query_map(self) -> QueryMap:
-        """Get query map."""
-        return {
-            QueryMode.DEFAULT: GPTVectorStoreIndexQuery,
-            QueryMode.EMBEDDING: GPTVectorStoreIndexQuery,
-        }
+    @property
+    def vector_store(self) -> VectorStore:
+        return self._vector_store
+
+    def as_retriever(self, **kwargs: Any) -> BaseRetriever:
+        # NOTE: lazy import
+        from llama_index.indices.vector_store.retrievers import VectorIndexRetriever
+
+        return VectorIndexRetriever(self, **kwargs)
 
     def _get_node_embedding_results(
         self, nodes: Sequence[Node], existing_node_ids: Set
     ) -> List[NodeEmbeddingResult]:
         """Get tuples of id, node, and embedding.
 
         Allows us to store these nodes in a vector store.
@@ -77,15 +66,15 @@
         """
         id_to_node_map: Dict[str, Node] = {}
         id_to_embed_map: Dict[str, List[float]] = {}
 
         for n in nodes:
             new_id = n.get_doc_id()
             if n.embedding is None:
-                self._service_context.embed_model.queue_text_for_embeddding(
+                self._service_context.embed_model.queue_text_for_embedding(
                     new_id, n.get_text()
                 )
             else:
                 id_to_embed_map[new_id] = n.embedding
 
             id_to_node_map[new_id] = n
 
@@ -230,55 +219,7 @@
         """
         self._insert(nodes, **insert_kwargs)
 
     def _delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         """Delete a document."""
         self._index_struct.delete(doc_id)
         self._vector_store.delete(doc_id)
-
-    @classmethod
-    def load_from_dict(
-        cls, result_dict: Dict[str, Any], **kwargs: Any
-    ) -> "BaseGPTIndex":
-        """Load index from string (in JSON-format).
-
-        This method loads the index from a JSON string. The index data
-        structure itself is preserved completely. If the index is defined over
-        subindices, those subindices will also be preserved (and subindices of
-        those subindices, etc.).
-
-        NOTE: load_from_string should not be used for indices composed on top
-        of other indices. Please define a `ComposableGraph` and use
-        `save_to_string` and `load_from_string` on that instead.
-
-        Args:
-            index_string (str): The index string (in JSON-format).
-
-        Returns:
-            BaseGPTIndex: The loaded index.
-
-        """
-        vector_store = load_vector_store_from_dict(
-            result_dict[VECTOR_STORE_KEY], **kwargs
-        )
-        return super().load_from_dict(result_dict, vector_store=vector_store, **kwargs)
-
-    def save_to_dict(self, **save_kwargs: Any) -> dict:
-        """Save to string.
-
-        This method stores the index into a JSON string.
-
-        NOTE: save_to_string should not be used for indices composed on top
-        of other indices. Please define a `ComposableGraph` and use
-        `save_to_string` and `load_from_string` on that instead.
-
-        Returns:
-            dict: The JSON dict of the index.
-
-        """
-        out_dict = super().save_to_dict()
-        out_dict[VECTOR_STORE_KEY] = save_vector_store_to_dict(self._vector_store)
-        return out_dict
-
-    @property
-    def query_context(self) -> Dict[str, Any]:
-        return {"vector_store": self._vector_store}
```

### Comparing `llama_index-0.5.9/llama_index/indices/vector_store/base_query.py` & `llama_index-0.6.0a1/llama_index/indices/vector_store/retrievers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,97 +1,104 @@
 """Base vector store index query."""
 
 
 from typing import Any, List, Optional
 
 from llama_index.data_structs.data_structs_v2 import IndexDict
 
-# from llama_index.data_structs.data_structs import IndexDict, Node
-from llama_index.data_structs.node_v2 import Node
-from llama_index.indices.query.base import BaseGPTIndexQuery
-from llama_index.indices.query.embedding_utils import SimilarityTracker
+from llama_index.data_structs.node_v2 import NodeWithScore
+from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.schema import QueryBundle
-from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.utils import log_vector_store_query_result
-from llama_index.vector_stores.types import VectorStore
+from llama_index.indices.vector_store.base import GPTVectorStoreIndex
+from llama_index.token_counter.token_counter import llm_token_counter
+from llama_index.vector_stores.types import (
+    VectorStoreQuery,
+    VectorStoreQueryMode,
+)
 
 
-class GPTVectorStoreIndexQuery(BaseGPTIndexQuery[IndexDict]):
+class VectorIndexRetriever(BaseRetriever):
     """Base vector store query.
 
     Args:
         embed_model (Optional[BaseEmbedding]): embedding model
         similarity_top_k (int): number of top k results to return
         vector_store (Optional[VectorStore]): vector store
 
     """
 
     def __init__(
         self,
-        index_struct: IndexDict,
-        service_context: ServiceContext,
-        vector_store: Optional[VectorStore] = None,
+        index: GPTVectorStoreIndex,
         similarity_top_k: int = 1,
+        vector_store_query_mode: str = VectorStoreQueryMode.DEFAULT,
+        alpha: Optional[float] = None,
+        doc_ids: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> None:
         """Initialize params."""
-        super().__init__(
-            index_struct=index_struct, service_context=service_context, **kwargs
-        )
+        self._index = index
+        self._vector_store = self._index.vector_store
+        self._service_context = self._index.service_context
+        self._docstore = self._index.docstore
+
         self._similarity_top_k = similarity_top_k
-        if vector_store is None:
-            raise ValueError("Vector store is required for vector store query.")
-        self._vector_store = vector_store
+        self._vector_store_query_mode = VectorStoreQueryMode(vector_store_query_mode)
+        self._alpha = alpha
+        self._doc_ids = doc_ids
 
+    @llm_token_counter("retrieve")
     def _retrieve(
         self,
         query_bundle: QueryBundle,
-        similarity_tracker: Optional[SimilarityTracker] = None,
-    ) -> List[Node]:
+    ) -> List[NodeWithScore]:
         if self._vector_store.is_embedding_query:
             if query_bundle.embedding is None:
                 query_bundle.embedding = (
                     self._service_context.embed_model.get_agg_embedding_from_queries(
                         query_bundle.embedding_strs
                     )
                 )
-            query_result = self._vector_store.query(
-                query_bundle.embedding,
-                self._similarity_top_k,
-                self._doc_ids,
-            )
-        else:
-            # TODO: fix function signature of query
-            query_result = self._vector_store.query(
-                [],
-                self._similarity_top_k,
-                self._doc_ids,
-                query_str=query_bundle.query_str,
-            )
+
+        query = VectorStoreQuery(
+            query_embedding=query_bundle.embedding,
+            similarity_top_k=self._similarity_top_k,
+            doc_ids=self._doc_ids,
+            query_str=query_bundle.query_str,
+            mode=self._vector_store_query_mode,
+            alpha=self._alpha,
+        )
+        query_result = self._vector_store.query(query)
 
         if query_result.nodes is None:
             # NOTE: vector store does not keep text and returns node indices.
             # Need to recover all nodes from docstore
             if query_result.ids is None:
                 raise ValueError(
                     "Vector store query result should return at "
                     "least one of nodes or ids."
                 )
-            assert isinstance(self._index_struct, IndexDict)
-            node_ids = [self._index_struct.nodes_dict[idx] for idx in query_result.ids]
+            assert isinstance(self._index.index_struct, IndexDict)
+            node_ids = [
+                self._index.index_struct.nodes_dict[idx] for idx in query_result.ids
+            ]
             nodes = self._docstore.get_nodes(node_ids)
             query_result.nodes = nodes
         else:
             # NOTE: vector store keeps text, returns nodes.
             # Only need to recover image or index nodes from docstore
             for i in range(len(query_result.nodes)):
                 node_id = query_result.nodes[i].get_doc_id()
                 if node_id in self._docstore.docs:
                     query_result.nodes[i] = self._docstore.get_node(node_id)
 
         log_vector_store_query_result(query_result)
 
-        if similarity_tracker is not None and query_result.similarities is not None:
-            for node, similarity in zip(query_result.nodes, query_result.similarities):
-                similarity_tracker.add(node, similarity)
+        node_with_scores: List[NodeWithScore] = []
+        for ind, node in enumerate(query_result.nodes):
+            score: Optional[float] = None
+            if query_result.similarities is not None:
+                score = query_result.similarities[ind]
+            node_with_scores.append(NodeWithScore(node, score=score))
 
-        return query_result.nodes
+        return node_with_scores
```

### Comparing `llama_index-0.5.9/llama_index/langchain_helpers/agents/__init__.py` & `llama_index-0.6.0a1/llama_index/langchain_helpers/agents/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 
 from llama_index.langchain_helpers.agents.agents import (
     create_llama_agent,
     create_llama_chat_agent,
 )
 from llama_index.langchain_helpers.agents.toolkits import LlamaToolkit
 from llama_index.langchain_helpers.agents.tools import (
-    GraphToolConfig,
     IndexToolConfig,
-    LlamaGraphTool,
     LlamaIndexTool,
 )
 
 __all__ = [
     "LlamaIndexTool",
     "LlamaGraphTool",
     "create_llama_agent",
```

### Comparing `llama_index-0.5.9/llama_index/langchain_helpers/agents/agents.py` & `llama_index-0.6.0a1/llama_index/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/langchain_helpers/memory_wrapper.py` & `llama_index-0.6.0a1/llama_index/langchain_helpers/memory_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,16 @@
         """Return key-value pairs given the text input to the chain."""
         prompt_input_key = self._get_prompt_input_key(inputs)
         query_str = inputs[prompt_input_key]
 
         # TODO: wrap in prompt
         # TODO: add option to return the raw text
         # NOTE: currently it's a hack
-        response = self.index.query(query_str, **self.query_kwargs)
+        query_engine = self.index.as_query_engine(**self.query_kwargs)
+        response = query_engine.query(query_str)
         return {self.memory_key: str(response)}
 
     def save_context(self, inputs: Dict[str, Any], outputs: Dict[str, str]) -> None:
         """Save the context of this model run to memory."""
         prompt_input_key = self._get_prompt_input_key(inputs)
         if self.output_key is None:
             if len(outputs) != 1:
@@ -134,15 +135,16 @@
         return prompt_input_key
 
     def load_memory_variables(self, inputs: Dict[str, Any]) -> Dict[str, str]:
         """Return key-value pairs given the text input to the chain."""
         prompt_input_key = self._get_prompt_input_key(inputs)
         query_str = inputs[prompt_input_key]
 
-        response_obj = self.index.query(query_str, **self.query_kwargs)
+        query_engine = self.index.as_query_engine(**self.query_kwargs)
+        response_obj = query_engine.query(query_str)
         if self.return_source:
             source_nodes = response_obj.source_nodes
             if self.return_messages:
                 # get source messages from ids
                 source_ids = [sn.doc_id for sn in source_nodes]
                 source_messages = [
                     m for id, m in self.id_to_message.items() if id in source_ids
```

### Comparing `llama_index-0.5.9/llama_index/langchain_helpers/sql_wrapper.py` & `llama_index-0.6.0a1/llama_index/langchain_helpers/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/langchain_helpers/text_splitter.py` & `llama_index-0.6.0a1/llama_index/langchain_helpers/text_splitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,15 @@
         separator: str = " ",
         chunk_size: int = 4000,
         chunk_overlap: int = 200,
         tokenizer: Optional[Callable] = None,
         backup_separators: Optional[List[str]] = ["\n"],
         paragraph_separator: Optional[str] = "\n\n\n",
         chunking_tokenizer_fn: Optional[Callable[[str], List[str]]] = None,
-        secondary_chunking_regex: Optional[str] = "[^,.;]+[,.;]?",
+        secondary_chunking_regex: Optional[str] = "[^,.;。]+[,.;。]?",
     ):
         """Initialize with parameters."""
         if chunk_overlap > chunk_size:
             raise ValueError(
                 f"Got a larger chunk overlap ({chunk_overlap}) than chunk size "
                 f"({chunk_size}), should be smaller."
             )
@@ -266,15 +266,14 @@
         self._chunk_overlap = chunk_overlap
         self.tokenizer = tokenizer or globals_helper.tokenizer
         self._backup_separators = backup_separators
         if chunking_tokenizer_fn is None:
             import nltk.tokenize.punkt as pkt
 
             class CustomLanguageVars(pkt.PunktLanguageVars):
-
                 _period_context_fmt = r"""
                     %(SentEndChars)s             # a potential sentence ending
                     (\)\"\s)\s*                  # other end chars and
                                                  # any amount of white space
                     (?=(?P<after_tok>
                         %(NonWord)s              # either other punctuation
                         |
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `llama_index-0.5.9/llama_index/llm_predictor/base.py` & `llama_index-0.6.0a1/llama_index/llm_predictor/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/llm_predictor/chatgpt.py` & `llama_index-0.6.0a1/llama_index/llm_predictor/chatgpt.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/llm_predictor/structured.py` & `llama_index-0.6.0a1/llama_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/logger/base.py` & `llama_index-0.6.0a1/llama_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/node_parser/interface.py` & `llama_index-0.6.0a1/llama_index/node_parser/interface.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/node_parser/node_utils.py` & `llama_index-0.6.0a1/llama_index/node_parser/node_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 def get_text_splits_from_document(
     document: BaseDocument,
     text_splitter: TextSplitter,
     include_extra_info: bool = True,
 ) -> List[TextSplit]:
     """Break the document into chunks with additional info."""
     # TODO: clean up since this only exists due to the diff w LangChain's TextSplitter
-    text_splits = []
     if isinstance(text_splitter, TokenTextSplitter):
         # use this to extract extra information about the chunks
         text_splits = text_splitter.split_text_with_overlaps(
             document.get_text(),
             extra_info_str=document.extra_info_str if include_extra_info else None,
         )
     else:
```

### Comparing `llama_index-0.5.9/llama_index/node_parser/simple.py` & `llama_index-0.6.0a1/llama_index/node_parser/simple.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,26 +30,25 @@
         self._text_splitter = text_splitter or TokenTextSplitter()
         self._include_extra_info = include_extra_info
         self._include_prev_next_rel = include_prev_next_rel
 
     def get_nodes_from_documents(
         self,
         documents: Sequence[Document],
-        include_extra_info: bool = True,
     ) -> List[Node]:
         """Parse document into nodes.
 
         Args:
             documents (Sequence[Document]): documents to parse
             include_extra_info (bool): whether to include extra info in nodes
 
         """
         all_nodes: List[Node] = []
         for document in documents:
             nodes = get_nodes_from_document(
                 document,
                 self._text_splitter,
-                include_extra_info,
+                self._include_extra_info,
                 include_prev_next_rel=self._include_prev_next_rel,
             )
             all_nodes.extend(nodes)
         return all_nodes
```

### Comparing `llama_index-0.5.9/llama_index/old_docstore.py` & `llama_index-0.6.0a1/llama_index/old_docstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 """Document store."""
 
 from collections import defaultdict
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional, Type, Union
 
-from dataclasses_json import DataClassJsonMixin
-
 from llama_index.data_structs.data_structs import IndexStruct
 from llama_index.readers.schema.base import Document
 
 DOC_TYPE = Union[IndexStruct, Document]
 
 # type key: used to store type of document
 TYPE_KEY = "__type__"
 
 
 @dataclass
-class V1DocumentStore(DataClassJsonMixin):
+class V1DocumentStore:
     """Document store."""
 
     docs: Dict[str, DOC_TYPE] = field(default_factory=dict)
     ref_doc_info: Dict[str, Dict[str, Any]] = field(
         default_factory=lambda: defaultdict(dict)
     )
 
-    def serialize_to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> Dict[str, Any]:
         """Serialize to dict."""
         docs_dict = {}
         for doc_id, doc in self.docs.items():
             doc_dict = doc.to_dict()
             doc_dict[TYPE_KEY] = doc.get_type()
             docs_dict[doc_id] = doc_dict
         return {"docs": docs_dict, "ref_doc_info": self.ref_doc_info}
@@ -38,15 +36,15 @@
         exclude_ids = exclude_ids or []
         for doc in self.docs.values():
             if isinstance(doc, IndexStruct) and doc.get_doc_id() not in exclude_ids:
                 return True
         return False
 
     @classmethod
-    def load_from_dict(
+    def from_dict(
         cls,
         docs_dict: Dict[str, Any],
         type_to_struct: Optional[Dict[str, Type[IndexStruct]]] = None,
     ) -> "V1DocumentStore":
         """Load from dict."""
         docs_obj_dict = {}
         for doc_id, doc_dict in docs_dict["docs"].items():
```

### Comparing `llama_index-0.5.9/llama_index/optimization/optimizer.py` & `llama_index-0.6.0a1/llama_index/optimization/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,23 +36,24 @@
 
         .. code-block:: python
         from llama_index.optimization.optimizer import Optimizer
         optimizer = SentenceEmbeddingOptimizer(
                         percentile_cutoff=0.5
                         this means that the top 50% of sentences will be used.
                         Alternatively, you can set the cutoff using a threshold
-                        on the similarity score. In this case only setences with a
+                        on the similarity score. In this case only sentences with a
                         similarity score higher than the threshold will be used.
                         threshold_cutoff=0.7
                         these cutoffs can also be used together.
                     )
 
-        response = index.query(
-            "<query_str>", optimizer=optimizer
+        query_engine = index.as_query_engine(
+            optimizer=optimizer
         )
+        response = query_engine.query("<query_str>")
         """
         self.embed_model = embed_model or OpenAIEmbedding()
         self._percentile_cutoff = percentile_cutoff
         self._threshold_cutoff = threshold_cutoff
 
         if tokenizer_fn is None:
             import nltk.data
```

### Comparing `llama_index-0.5.9/llama_index/output_parsers/base.py` & `llama_index-0.6.0a1/llama_index/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/output_parsers/guardrails.py` & `llama_index-0.6.0a1/llama_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/output_parsers/langchain.py` & `llama_index-0.6.0a1/llama_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/playground/base.py` & `llama_index-0.6.0a1/llama_index/playground/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,69 +4,82 @@
 import time
 from typing import Any, Dict, List, Optional, Type, Union
 
 import pandas as pd
 from langchain.input import get_color_mapping, print_text
 
 from llama_index.indices.base import BaseGPTIndex
-from llama_index.indices.list.base import GPTListIndex
-from llama_index.indices.tree.base import GPTTreeIndex
-from llama_index.indices.vector_store import GPTSimpleVectorIndex
+from llama_index.indices.list.base import GPTListIndex, ListRetrieverMode
+from llama_index.indices.tree.base import GPTTreeIndex, TreeRetrieverMode
+from llama_index.indices.vector_store import GPTVectorStoreIndex
 from llama_index.readers.schema.base import Document
 
 DEFAULT_INDEX_CLASSES: List[Type[BaseGPTIndex]] = [
-    GPTSimpleVectorIndex,
+    GPTVectorStoreIndex,
     GPTTreeIndex,
     GPTListIndex,
 ]
-DEFAULT_MODES = ["default", "summarize", "embedding", "retrieve", "recursive"]
+
+INDEX_SPECIFIC_QUERY_MODES_TYPE = Dict[Type[BaseGPTIndex], List[str]]
+
+DEFAULT_MODES: INDEX_SPECIFIC_QUERY_MODES_TYPE = {
+    GPTTreeIndex: [e.value for e in TreeRetrieverMode],
+    GPTListIndex: [e.value for e in ListRetrieverMode],
+    GPTVectorStoreIndex: ["default"],
+}
 
 
 class Playground:
-    """Experiment with indices, models, embeddings, modes, and more."""
+    """Experiment with indices, models, embeddings, retriever_modes, and more."""
 
-    def __init__(self, indices: List[BaseGPTIndex], modes: List[str] = DEFAULT_MODES):
+    def __init__(
+        self,
+        indices: List[BaseGPTIndex],
+        retriever_modes: INDEX_SPECIFIC_QUERY_MODES_TYPE = DEFAULT_MODES,
+    ):
         """Initialize with indices to experiment with.
 
         Args:
             indices: A list of BaseGPTIndex's to experiment with
-            modes: A list of modes that specify which nodes are chosen
-                from the index when a query is made. A full list of modes
-                available to each index can be found here:
+            retriever_modes: A list of retriever_modes that specify which nodes are
+                chosen from the index when a query is made. A full list of
+                retriever_modes available to each index can be found here:
                 https://gpt-index.readthedocs.io/en/latest/reference/query.html
         """
         self._validate_indices(indices)
         self._indices = indices
-        self._validate_modes(modes)
-        self._modes = modes
+        self._validate_modes(retriever_modes)
+        self._retriever_modes = retriever_modes
 
         index_range = [str(i) for i in range(len(indices))]
         self.index_colors = get_color_mapping(index_range)
 
     @classmethod
     def from_docs(
         cls,
         documents: List[Document],
         index_classes: List[Type[BaseGPTIndex]] = DEFAULT_INDEX_CLASSES,
+        retriever_modes: INDEX_SPECIFIC_QUERY_MODES_TYPE = DEFAULT_MODES,
         **kwargs: Any,
     ) -> Playground:
         """Initialize with Documents using the default list of indices.
 
         Args:
             documents: A List of Documents to experiment with.
         """
         if len(documents) == 0:
             raise ValueError(
                 "Playground must be initialized with a nonempty list of Documents."
             )
 
         indices = [
-            index_class.from_documents(documents) for index_class in index_classes
+            index_class.from_documents(documents, **kwargs)
+            for index_class in index_classes
         ]
-        return cls(indices, **kwargs)
+        return cls(indices, retriever_modes)
 
     def _validate_indices(self, indices: List[BaseGPTIndex]) -> None:
         """Validate a list of indices."""
         if len(indices) == 0:
             raise ValueError("Playground must have a non-empty list of indices.")
         for index in indices:
             if not isinstance(index, BaseGPTIndex):
@@ -81,32 +94,33 @@
 
     @indices.setter
     def indices(self, indices: List[BaseGPTIndex]) -> None:
         """Set Playground's indices."""
         self._validate_indices(indices)
         self._indices = indices
 
-    def _validate_modes(self, modes: List[str]) -> None:
-        """Validate a list of modes."""
-        if len(modes) == 0:
+    def _validate_modes(self, retriever_modes: INDEX_SPECIFIC_QUERY_MODES_TYPE) -> None:
+        """Validate a list of retriever_modes."""
+        if len(retriever_modes) == 0:
             raise ValueError(
-                "Playground must have a nonzero number of modes."
-                "Initialize without the `modes` argument to use the default list."
+                "Playground must have a nonzero number of retriever_modes."
+                "Initialize without the `retriever_modes` "
+                "argument to use the default list."
             )
 
     @property
-    def modes(self) -> List[str]:
+    def retriever_modes(self) -> dict:
         """Get Playground's indices."""
-        return self._modes
+        return self._retriever_modes
 
-    @modes.setter
-    def modes(self, modes: List[str]) -> None:
+    @retriever_modes.setter
+    def retriever_modes(self, retriever_modes: INDEX_SPECIFIC_QUERY_MODES_TYPE) -> None:
         """Set Playground's indices."""
-        self._validate_modes(modes)
-        self._modes = modes
+        self._validate_modes(retriever_modes)
+        self._retriever_modes = retriever_modes
 
     def compare(
         self, query_text: str, to_pandas: Optional[bool] = True
     ) -> Union[pd.DataFrame, List[Dict[str, Any]]]:
         """Compare index outputs on an input query.
 
         Args:
@@ -115,36 +129,42 @@
                 True by default.
 
         Returns:
             The output of each index along with other data, such as the time it took to
             compute. Results are stored in a Pandas Dataframe or a list of Dicts.
         """
         print(f"\033[1mQuery:\033[0m\n{query_text}\n")
-        print(f"Trying {len(self._indices) * len(self._modes)} combinations...\n\n")
         result = []
         for i, index in enumerate(self._indices):
-            for mode in self._modes:
-                if mode not in index.get_query_map():
-                    continue
+            for retriever_mode in self._retriever_modes[type(index)]:
                 start_time = time.time()
 
                 index_name = type(index).__name__
-                print_text(f"\033[1m{index_name}\033[0m, mode = {mode}", end="\n")
-                output = index.query(query_text, mode=mode)
+                print_text(
+                    f"\033[1m{index_name}\033[0m, retriever mode = {retriever_mode}",
+                    end="\n",
+                )
+                # TODO: refactor query mode
+                try:
+                    query_engine = index.as_query_engine(retriever_mode=retriever_mode)
+                except ValueError:
+                    continue
+
+                output = query_engine.query(query_text)
                 print_text(str(output), color=self.index_colors[str(i)], end="\n\n")
 
                 duration = time.time() - start_time
 
                 llm_token_usage = index.service_context.llm_predictor.last_token_usage
                 embed_token_usage = index.service_context.embed_model.last_token_usage
 
                 result.append(
                     {
                         "Index": index_name,
-                        "Mode": mode,
+                        "Retriever Mode": retriever_mode,
                         "Output": str(output),
                         "Duration": duration,
                         "LLM Tokens": llm_token_usage,
                         "Embedding Tokens": embed_token_usage,
                     }
                 )
         print(f"\nRan {len(result)} combinations in total.")
```

### Comparing `llama_index-0.5.9/llama_index/prompts/base.py` & `llama_index-0.6.0a1/llama_index/prompts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/prompts/chat_prompts.py` & `llama_index-0.6.0a1/llama_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/prompts/default_prompt_selectors.py` & `llama_index-0.6.0a1/llama_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/prompts/default_prompts.py` & `llama_index-0.6.0a1/llama_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/prompts/prompt_type.py` & `llama_index-0.6.0a1/llama_index/prompts/prompt_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/prompts/prompts.py` & `llama_index-0.6.0a1/llama_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/__init__.py` & `llama_index-0.6.0a1/llama_index/readers/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,28 +8,31 @@
 in our `Insert How-To Guide <../how_to/insert.html>`_. See below for the API
 definition of a Document - the bare minimum is a `text` property.
 
 """
 
 from llama_index.readers.chatgpt_plugin import ChatGPTRetrievalPluginReader
 from llama_index.readers.chroma import ChromaReader
+from llama_index.readers.deeplake import DeepLakeReader
 from llama_index.readers.discord_reader import DiscordReader
 from llama_index.readers.elasticsearch import ElasticsearchReader
 from llama_index.readers.faiss import FaissReader
 
 # readers
 from llama_index.readers.file.base import SimpleDirectoryReader
 from llama_index.readers.github_readers.github_repository_reader import (
     GithubRepositoryReader,
 )
 from llama_index.readers.google_readers.gdocs import GoogleDocsReader
 from llama_index.readers.json import JSONReader
 from llama_index.readers.make_com.wrapper import MakeWrapper
 from llama_index.readers.mbox import MboxReader
+from llama_index.readers.milvus import MilvusReader
 from llama_index.readers.mongo import SimpleMongoReader
+from llama_index.readers.myscale import MyScaleReader
 from llama_index.readers.notion import NotionPageReader
 from llama_index.readers.obsidian import ObsidianReader
 from llama_index.readers.pinecone import PineconeReader
 from llama_index.readers.qdrant import QdrantReader
 from llama_index.readers.schema.base import Document
 from llama_index.readers.slack import SlackReader
 from llama_index.readers.steamship.file_reader import SteamshipFileReader
@@ -54,16 +57,19 @@
     "NotionPageReader",
     "GoogleDocsReader",
     "DiscordReader",
     "SlackReader",
     "WeaviateReader",
     "PineconeReader",
     "QdrantReader",
+    "MilvusReader",
     "ChromaReader",
+    "DeepLakeReader",
     "FaissReader",
+    "MyScaleReader",
     "Document",
     "StringIterableReader",
     "SimpleWebPageReader",
     "BeautifulSoupWebReader",
     "TrafilaturaWebReader",
     "RssReader",
     "MakeWrapper",
```

### Comparing `llama_index-0.5.9/llama_index/readers/base.py` & `llama_index-0.6.0a1/llama_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/chatgpt_plugin/base.py` & `llama_index-0.6.0a1/llama_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/chroma.py` & `llama_index-0.6.0a1/llama_index/readers/chroma.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,28 +33,25 @@
         except ImportError:
             raise ImportError(import_err_msg)
 
         if collection_name is None:
             raise ValueError("Please provide a collection name.")
         from chromadb.config import Settings
 
-        if persist_directory:
-            self._client = chromadb.Client(
-                Settings(
-                    chroma_db_impl="duckdb+parquet", persist_directory=persist_directory
-                )
-            )
-        else:
-            self._client = chromadb.Client(
-                Settings(
-                    chroma_api_impl="rest",
-                    chroma_server_host=host,
-                    chroma_server_http_port=port,
-                )
+        self._client = chromadb.Client(
+            Settings(
+                chroma_api_impl="rest",
+                chroma_server_host=host,
+                chroma_server_http_port=port,
+                persist_directory=persist_directory
+                if persist_directory
+                else "./chroma",
             )
+        )
+
         self._collection = self._client.get_collection(collection_name)
 
     def create_documents(self, results: Any) -> List[Document]:
         """Create documents from the results.
 
         Args:
             results: Results from the query.
```

### Comparing `llama_index-0.5.9/llama_index/readers/database.py` & `llama_index-0.6.0a1/llama_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/discord_reader.py` & `llama_index-0.6.0a1/llama_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/download.py` & `llama_index-0.6.0a1/llama_index/readers/download.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,25 +49,28 @@
         line = line.strip()
         if line.startswith("__all__"):
             exports = line.split("=")[1].strip().strip("[").strip("]").split(",")
             exports = [export.strip().strip("'").strip('"') for export in exports]
     return exports
 
 
-def rewrite_exports(exports: List[str]) -> None:
+def rewrite_exports(exports: List[str], custom_path: Optional[str] = None) -> None:
     """Write the `__all__` variable to the `__init__.py` file in the modules dir.
 
     Removes the line that contains `__all__` and appends a new line with the updated
     `__all__` variable.
 
     Args:
         - exports: A list of exported class names.
 
     """
-    dirpath = Path(__file__).parent / "llamahub_modules"
+    if custom_path is not None:
+        dirpath = Path(custom_path)
+    else:
+        dirpath = Path(__file__).parent / "llamahub_modules"
     init_path = f"{dirpath}/__init__.py"
     with open(init_path, "r") as f:
         lines = f.readlines()
     with open(init_path, "w") as f:
         for line in lines:
             line = line.strip()
             if line.startswith("__all__"):
@@ -77,32 +80,37 @@
 
 
 def download_loader(
     loader_class: str,
     loader_hub_url: str = LOADER_HUB_URL,
     refresh_cache: Optional[bool] = False,
     use_llama_index_import: bool = False,
+    custom_path: Optional[str] = None,
 ) -> Type[BaseReader]:
     """Download a single loader from the Loader Hub.
 
     Args:
         loader_class: The name of the loader class you want to download,
             such as `SimpleWebPageReader`.
         refresh_cache: If true, the local cache will be skipped and the
             loader will be fetched directly from the remote repo.
         use_llama_index_import: If true, the loader files will use
             llama_index as the base dependency. By default (False),
             the loader files use llama_index as the base dependency.
             NOTE: this is a temporary workaround while we fully migrate all usages
             to llama_index.
+        custom_path: Custom dirpath to download loader into.
 
     Returns:
         A Loader.
     """
-    dirpath = Path(__file__).parent / "llamahub_modules"
+    if custom_path is not None:
+        dirpath = Path(custom_path)
+    else:
+        dirpath = Path(__file__).parent / "llamahub_modules"
     if not os.path.exists(dirpath):
         # Create a new directory because it does not exist
         os.makedirs(dirpath)
     if not os.path.exists(f"{dirpath}/__init__.py"):
         # Create an empty __init__.py file if it does not exist yet
         with open(f"{dirpath}/__init__.py", "w") as f:
             pass
@@ -164,15 +172,17 @@
             # add the exports to the __init__.py file in the modules directory
             if extra_file == "__init__.py":
                 loader_exports = get_exports(extra_file_raw_content)
                 existing_exports = []
                 with open(dirpath / "__init__.py", "r+") as f:
                     f.write(f"from .{loader_id} import {', '.join(loader_exports)}")
                     existing_exports = get_exports(f.read())
-                rewrite_exports(existing_exports + loader_exports)
+                rewrite_exports(
+                    existing_exports + loader_exports, custom_path=custom_path
+                )
             with open(f"{loader_path}/{extra_file}", "w") as f:
                 f.write(extra_file_raw_content)
 
     if not os.path.exists(requirements_path):
         # NOTE: need to check the status code
         response_txt, status_code = _get_file_content(
             loader_hub_url, f"/{loader_id}/requirements.txt"
```

### Comparing `llama_index-0.5.9/llama_index/readers/elasticsearch.py` & `llama_index-0.6.0a1/llama_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/faiss.py` & `llama_index-0.6.0a1/llama_index/readers/faiss.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 class FaissReader(BaseReader):
     """Faiss reader.
 
     Retrieves documents through an existing in-memory Faiss index.
     These documents can then be used in a downstream LlamaIndex data structure.
     If you wish use Faiss itself as an index to to organize documents,
-    insert documents, and perform queries on them, please use GPTFaissIndex.
+    insert documents, and perform queries on them, please use GPTVectorStoreIndex
+    with FaissVectorStore.
 
     Args:
         faiss_index (faiss.Index): A Faiss Index object (required)
 
     """
 
     def __init__(self, index: Any):
```

### Comparing `llama_index-0.5.9/llama_index/readers/file/base.py` & `llama_index-0.6.0a1/llama_index/readers/file/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from llama_index.readers.file.epub_parser import EpubParser
 from llama_index.readers.file.image_parser import ImageParser
 from llama_index.readers.file.markdown_parser import MarkdownParser
 from llama_index.readers.file.mbox_parser import MboxParser
 from llama_index.readers.file.slides_parser import PptxParser
 from llama_index.readers.file.tabular_parser import PandasCSVParser
 from llama_index.readers.file.video_audio import VideoAudioParser
+from llama_index.readers.file.ipynb_parser import IPYNBParser
 from llama_index.readers.schema.base import Document, ImageDocument
 
 DEFAULT_FILE_EXTRACTOR: Dict[str, BaseParser] = {
     ".pdf": PDFParser(),
     ".docx": DocxParser(),
     ".pptx": PptxParser(),
     ".jpg": ImageParser(),
@@ -25,14 +26,15 @@
     ".jpeg": ImageParser(),
     ".mp3": VideoAudioParser(),
     ".mp4": VideoAudioParser(),
     ".csv": PandasCSVParser(),
     ".epub": EpubParser(),
     ".md": MarkdownParser(),
     ".mbox": MboxParser(),
+    ".ipynb": IPYNBParser(),
 }
 
 logger = logging.getLogger(__name__)
 
 
 class SimpleDirectoryReader(BaseReader):
     """Simple directory reader.
```

### Comparing `llama_index-0.5.9/llama_index/readers/file/base_parser.py` & `llama_index-0.6.0a1/llama_index/readers/file/base_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/file/docs_parser.py` & `llama_index-0.6.0a1/llama_index/readers/file/docs_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/file/epub_parser.py` & `llama_index-0.6.0a1/llama_index/readers/file/epub_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/file/image_parser.py` & `llama_index-0.6.0a1/llama_index/readers/file/image_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/file/markdown_parser.py` & `llama_index-0.6.0a1/llama_index/readers/file/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/file/mbox_parser.py` & `llama_index-0.6.0a1/llama_index/readers/file/mbox_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/file/slides_parser.py` & `llama_index-0.6.0a1/llama_index/readers/file/slides_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/file/tabular_parser.py` & `llama_index-0.6.0a1/llama_index/readers/file/tabular_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/file/video_audio.py` & `llama_index-0.6.0a1/llama_index/readers/file/video_audio.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/github_readers/github_api_client.py` & `llama_index-0.6.0a1/llama_index/readers/github_readers/github_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,15 @@
         async with httpx.AsyncClient(
             headers=_headers, base_url=self._base_url
         ) as _client:
             try:
                 response = await _client.request(
                     method, url=self._endpoints[endpoint].format(**kwargs)
                 )
+                response.raise_for_status()
             except httpx.HTTPError as excp:
                 print(f"HTTP Exception for {excp.request.url} - {excp}")
                 raise excp
             return response
 
     async def get_branch(
         self, owner: str, repo: str, branch: str
```

### Comparing `llama_index-0.5.9/llama_index/readers/github_readers/github_repository_reader.py` & `llama_index-0.6.0a1/llama_index/readers/github_readers/github_repository_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/github_readers/utils.py` & `llama_index-0.6.0a1/llama_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/google_readers/gdocs.py` & `llama_index-0.6.0a1/llama_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/google_readers/gsheets.py` & `llama_index-0.6.0a1/llama_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/json.py` & `llama_index-0.6.0a1/llama_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/make_com/wrapper.py` & `llama_index-0.6.0a1/llama_index/readers/make_com/wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/mbox.py` & `llama_index-0.6.0a1/llama_index/readers/mbox.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/mongo.py` & `llama_index-0.6.0a1/llama_index/readers/mongo.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,21 +40,27 @@
         else:
             if host is None or port is None:
                 raise ValueError("Either `host` and `port` or `uri` must be provided.")
             self.client = MongoClient(host, port)
         self.max_docs = max_docs
 
     def load_data(
-        self, db_name: str, collection_name: str, query_dict: Optional[Dict] = None
+        self,
+        db_name: str,
+        collection_name: str,
+        field_names: List[str] = ["text"],
+        query_dict: Optional[Dict] = None,
     ) -> List[Document]:
         """Load data from the input directory.
 
         Args:
             db_name (str): name of the database.
             collection_name (str): name of the collection.
+            field_names(List[str]): names of the fields to be concatenated.
+                Defaults to ["text"]
             query_dict (Optional[Dict]): query to filter documents.
                 Defaults to None
 
         Returns:
             List[Document]: A list of documents.
 
         """
@@ -62,11 +68,18 @@
         db = self.client[db_name]
         if query_dict is None:
             cursor = db[collection_name].find()
         else:
             cursor = db[collection_name].find(query_dict)
 
         for item in cursor:
-            if "text" not in item:
-                raise ValueError("`text` field not found in Mongo document.")
-            documents.append(Document(item["text"]))
+            text = ""
+            for field_name in field_names:
+                if field_name not in item:
+                    raise ValueError(
+                        f"`{field_name}` field not found in Mongo document."
+                    )
+                text += item[field_name]
+
+            documents.append(Document(text))
+
         return documents
```

### Comparing `llama_index-0.5.9/llama_index/readers/notion.py` & `llama_index-0.6.0a1/llama_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/obsidian.py` & `llama_index-0.6.0a1/llama_index/readers/obsidian.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/pinecone.py` & `llama_index-0.6.0a1/llama_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/qdrant.py` & `llama_index-0.6.0a1/llama_index/readers/qdrant.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,59 +8,74 @@
 
 class QdrantReader(BaseReader):
     """Qdrant reader.
 
     Retrieve documents from existing Qdrant collections.
 
     Args:
-        host: Host name of Qdrant service.
+        location:
+            If `:memory:` - use in-memory Qdrant instance.
+            If `str` - use it as a `url` parameter.
+            If `None` - use default values for `host` and `port`.
+        url:
+            either host or str of
+            "Optional[scheme], host, Optional[port], Optional[prefix]".
+            Default: `None`
         port: Port of the REST API interface. Default: 6333
         grpc_port: Port of the gRPC interface. Default: 6334
         prefer_grpc: If `true` - use gPRC interface whenever possible in custom methods.
         https: If `true` - use HTTPS(SSL) protocol. Default: `false`
         api_key: API key for authentication in Qdrant Cloud. Default: `None`
         prefix:
             If not `None` - add `prefix` to the REST URL path.
             Example: `service/v1` will result in
             `http://localhost:6333/service/v1/{qdrant-endpoint}` for REST API.
             Default: `None`
         timeout:
             Timeout for REST and gRPC API requests.
             Default: 5.0 seconds for REST and unlimited for gRPC
+        host: Host name of Qdrant service. If url and host are None, set to 'localhost'.
+            Default: `None`
     """
 
     def __init__(
         self,
-        host: str,
-        port: int = 6333,
+        location: Optional[str] = None,
+        url: Optional[str] = None,
+        port: Optional[int] = 6333,
         grpc_port: int = 6334,
         prefer_grpc: bool = False,
         https: Optional[bool] = None,
         api_key: Optional[str] = None,
         prefix: Optional[str] = None,
         timeout: Optional[float] = None,
+        host: Optional[str] = None,
+        path: Optional[str] = None,
     ):
         """Initialize with parameters."""
         import_err_msg = (
             "`qdrant-client` package not found, please run `pip install qdrant-client`"
         )
         try:
             import qdrant_client  # noqa: F401
         except ImportError:
             raise ImportError(import_err_msg)
 
         self._client = qdrant_client.QdrantClient(
-            url=host,
+            location=location,
+            url=url,
             port=port,
             grpc_port=grpc_port,
             prefer_grpc=prefer_grpc,
             https=https,
             api_key=api_key,
             prefix=prefix,
             timeout=timeout,
+            host=host,
+            path=path,
         )
 
     def load_data(
         self,
         collection_name: str,
         query_vector: List[float],
         limit: int = 10,
```

### Comparing `llama_index-0.5.9/llama_index/readers/schema/base.py` & `llama_index-0.6.0a1/llama_index/readers/schema/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/slack.py` & `llama_index-0.6.0a1/llama_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/steamship/file_reader.py` & `llama_index-0.6.0a1/llama_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/string_iterable.py` & `llama_index-0.6.0a1/llama_index/readers/string_iterable.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,16 @@
         .. code-block:: python
 
             from llama_index import StringIterableReader, GPTTreeIndex
 
             documents = StringIterableReader().load_data(
                 texts=["I went to the store", "I bought an apple"])
             index = GPTTreeIndex.from_documents(documents)
-            index.query("what did I buy?")
+            query_engine = index.as_query_engine()
+            query_engine.query("what did I buy?")
 
             # response should be something like "You bought an apple."
     """
 
     def load_data(self, texts: List[str]) -> List[Document]:
         """Load the data."""
         results = []
```

### Comparing `llama_index-0.5.9/llama_index/readers/twitter.py` & `llama_index-0.6.0a1/llama_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/weaviate/data_structs.py` & `llama_index-0.6.0a1/llama_index/readers/weaviate/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,299 +1,266 @@
 """Weaviate-specific serializers for LlamaIndex data structures.
 
 Contain conversion to and from dataclasses that LlamaIndex uses.
 
 """
 
 import json
-from abc import abstractmethod
 from dataclasses import field
-from typing import Any, Dict, Generic, List, Optional, TypeVar, cast
+from typing import Any, Dict, List, Optional, cast
 
 from llama_index.data_structs.data_structs_v2 import Node
-from llama_index.data_structs.data_structs_v2 import V2IndexStruct as IndexStruct
 from llama_index.data_structs.node_v2 import DocumentRelationship
 from llama_index.readers.weaviate.utils import (
     get_by_id,
     parse_get_response,
     validate_client,
 )
 from llama_index.utils import get_new_id
+from llama_index.vector_stores.types import VectorStoreQuery, VectorStoreQueryMode
 
-IS = TypeVar("IS", bound=Node)
+import logging
 
+_logger = logging.getLogger(__name__)
 
-class BaseWeaviateIndexStruct(IndexStruct, Generic[IS]):
-    """Base Weaviate index struct."""
-
-    @classmethod
-    @abstractmethod
-    def _class_name(cls, class_prefix: str) -> str:
-        """Return class name."""
-
-    @classmethod
-    def _get_common_properties(cls) -> List[Dict]:
-        """Get common properties."""
-        return [
-            {
-                "dataType": ["string"],
-                "description": "Text property",
-                "name": "text",
-            },
-            {
-                "dataType": ["string"],
-                "description": "Document id",
-                "name": "doc_id",
-            },
-            {
-                "dataType": ["string"],
-                "description": "extra_info (in JSON)",
-                "name": "extra_info",
-            },
-        ]
-
-    @classmethod
-    @abstractmethod
-    def _get_properties(cls) -> List[Dict]:
-        """Get properties specific to each index struct.
-
-        Used in creating schema.
-
-        """
-
-    @classmethod
-    def _get_by_id(cls, client: Any, object_id: str, class_prefix: str) -> Dict:
-        """Get entry by id."""
-        validate_client(client)
-        class_name = cls._class_name(class_prefix)
-        properties = cls._get_common_properties() + cls._get_properties()
-        prop_names = [p["name"] for p in properties]
-        entry = get_by_id(client, object_id, class_name, prop_names)
-        return entry
-
-    @classmethod
-    def create_schema(cls, client: Any, class_prefix: str) -> None:
-        """Create schema."""
-        validate_client(client)
-        # first check if schema exists
-        schema = client.schema.get()
-        classes = schema["classes"]
-        existing_class_names = {c["class"] for c in classes}
-        # if schema already exists, don't create
-        class_name = cls._class_name(class_prefix)
-        if class_name in existing_class_names:
-            return
-
-        # get common properties
-        properties = cls._get_common_properties()
-        # get specific properties
-        properties.extend(cls._get_properties())
-        class_obj = {
-            "class": cls._class_name(class_prefix),  # <= note the capital "A".
-            "description": f"Class for {class_name}",
-            "properties": properties,
-        }
-        client.schema.create_class(class_obj)
-
-    @classmethod
-    @abstractmethod
-    def _entry_to_llama_index(cls, entry: Dict) -> IS:
-        """Convert to LlamaIndex list."""
-
-    @classmethod
-    def to_llama_index_list(
-        cls,
-        client: Any,
-        class_prefix: str,
-        vector: Optional[List[float]] = None,
-        object_limit: Optional[int] = None,
-    ) -> List[IS]:
-        """Convert to LlamaIndex list."""
-        validate_client(client)
-        class_name = cls._class_name(class_prefix)
-        properties = cls._get_common_properties() + cls._get_properties()
-        prop_names = [p["name"] for p in properties]
-        query = client.query.get(class_name, prop_names).with_additional(
-            ["id", "vector"]
-        )
+NODE_SCHEMA: List[Dict] = [
+    {
+        "dataType": ["string"],
+        "description": "Text property",
+        "name": "text",
+    },
+    {
+        "dataType": ["string"],
+        "description": "Document id",
+        "name": "doc_id",
+    },
+    {
+        "dataType": ["string"],
+        "description": "extra_info (in JSON)",
+        "name": "extra_info",
+    },
+    {
+        "dataType": ["string"],
+        "description": "The ref_doc_id of the Node",
+        "name": "ref_doc_id",
+    },
+    {
+        "dataType": ["string"],
+        "description": "node_info (in JSON)",
+        "name": "node_info",
+    },
+    {
+        "dataType": ["string"],
+        "description": "The hash of the Document",
+        "name": "doc_hash",
+    },
+    {
+        "dataType": ["string"],
+        "description": "The relationships of the node (in JSON)",
+        "name": "relationships",
+    },
+]
+
+
+def _get_by_id(client: Any, object_id: str, class_prefix: str) -> Dict:
+    """Get entry by id."""
+    validate_client(client)
+    class_name = _class_name(class_prefix)
+    properties = NODE_SCHEMA
+    prop_names = [p["name"] for p in properties]
+    entry = get_by_id(client, object_id, class_name, prop_names)
+    return entry
+
+
+def create_schema(client: Any, class_prefix: str) -> None:
+    """Create schema."""
+    validate_client(client)
+    # first check if schema exists
+    schema = client.schema.get()
+    classes = schema["classes"]
+    existing_class_names = {c["class"] for c in classes}
+    # if schema already exists, don't create
+    class_name = _class_name(class_prefix)
+    if class_name in existing_class_names:
+        return
+
+    properties = NODE_SCHEMA
+    class_obj = {
+        "class": _class_name(class_prefix),  # <= note the capital "A".
+        "description": f"Class for {class_name}",
+        "properties": properties,
+    }
+    client.schema.create_class(class_obj)
+
+
+def weaviate_query(
+    client: Any,
+    class_prefix: str,
+    query_spec: VectorStoreQuery,
+) -> List[Node]:
+    """Convert to LlamaIndex list."""
+    validate_client(client)
+
+    class_name = _class_name(class_prefix)
+    prop_names = [p["name"] for p in NODE_SCHEMA]
+    vector = query_spec.query_embedding
+
+    # build query
+    query = client.query.get(class_name, prop_names).with_additional(["id", "vector"])
+    if query_spec.mode == VectorStoreQueryMode.DEFAULT:
+        _logger.debug("Using vector search")
         if vector is not None:
             query = query.with_near_vector(
                 {
                     "vector": vector,
                 }
             )
-        if object_limit is not None:
-            query = query.with_limit(object_limit)
-        query_result = query.do()
-        parsed_result = parse_get_response(query_result)
-        entries = parsed_result[class_name]
-
-        results: List[IS] = []
-        for entry in entries:
-            results.append(cls._entry_to_llama_index(entry))
-
-        return results
-
-    @classmethod
-    @abstractmethod
-    def _from_llama_index(
-        cls, client: Any, index: IS, class_prefix: str, batch: Optional[Any] = None
-    ) -> str:
-        """Convert from LlamaIndex."""
-
-    @classmethod
-    def from_llama_index(cls, client: Any, index: IS, class_prefix: str) -> str:
-        """Convert from LlamaIndex."""
-        validate_client(client)
-        index_id = cls._from_llama_index(client, index, class_prefix)
-        client.batch.flush()
-        return index_id
-
-
-class WeaviateNode(BaseWeaviateIndexStruct[Node]):
-    """Weaviate node."""
-
-    @classmethod
-    def _class_name(cls, class_prefix: str) -> str:
-        """Return class name."""
-        return f"{class_prefix}_Node"
-
-    @classmethod
-    def _get_properties(cls) -> List[Dict]:
-        """Create schema."""
-        return [
-            {
-                "dataType": ["string"],
-                "description": "The ref_doc_id of the Node",
-                "name": "ref_doc_id",
-            },
-            {
-                "dataType": ["string"],
-                "description": "node_info (in JSON)",
-                "name": "node_info",
-            },
-            {
-                "dataType": ["string"],
-                "description": "The hash of the Document",
-                "name": "doc_hash",
-            },
-            {
-                "dataType": ["string"],
-                "description": "The relationships of the node (in JSON)",
-                "name": "relationships",
-            },
-        ]
-
-    @classmethod
-    def _entry_to_llama_index(cls, entry: Dict) -> Node:
-        """Convert to LlamaIndex list."""
-        extra_info_str = entry["extra_info"]
-        if extra_info_str == "":
-            extra_info = None
-        else:
-            extra_info = json.loads(extra_info_str)
-
-        node_info_str = entry["node_info"]
-        if node_info_str == "":
-            node_info = None
-        else:
-            node_info = json.loads(node_info_str)
-
-        relationships_str = entry["relationships"]
-        relationships: Dict[DocumentRelationship, str]
-        if relationships_str == "":
-            relationships = field(default_factory=dict)
-        else:
-            relationships = {
-                DocumentRelationship(k): v
-                for k, v in json.loads(relationships_str).items()
-            }
-
-        return Node(
-            text=entry["text"],
-            doc_id=entry["doc_id"],
-            embedding=entry["_additional"]["vector"],
-            extra_info=extra_info,
-            node_info=node_info,
-            relationships=relationships,
+    elif query_spec.mode == VectorStoreQueryMode.HYBRID:
+        _logger.debug(f"Using hybrid search with alpha {query_spec.alpha}")
+        query = query.with_hybrid(
+            query=query_spec.query_str,
+            alpha=query_spec.alpha,
+            vector=vector,
         )
+    query = query.with_limit(query_spec.similarity_top_k)
+    _logger.debug(f"Using limit of {query_spec.similarity_top_k}")
+
+    # execute query
+    query_result = query.do()
 
-    @classmethod
-    def _from_llama_index(
-        cls, client: Any, node: Node, class_prefix: str, batch: Optional[Any] = None
-    ) -> str:
-        """Convert from LlamaIndex."""
-        node_dict = node.to_dict()
-        vector = node_dict.pop("embedding")
-        # json-serialize the extra_info
-        extra_info = node_dict.pop("extra_info")
-        extra_info_str = ""
-        if extra_info is not None:
-            extra_info_str = json.dumps(extra_info)
-        node_dict["extra_info"] = extra_info_str
-        # json-serialize the node_info
-        node_info = node_dict.pop("node_info")
-        node_info_str = ""
-        if node_info is not None:
-            node_info_str = json.dumps(node_info)
-        node_dict["node_info"] = node_info_str
-        # json-serialize the relationships
-        relationships = node_dict.pop("relationships")
-        relationships_str = ""
-        if relationships is not None:
-            relationships_str = json.dumps(relationships)
-        node_dict["relationships"] = relationships_str
-
-        ref_doc_id = node.ref_doc_id
-        if ref_doc_id is not None:
-            node_dict["ref_doc_id"] = ref_doc_id
-
-        # TODO: account for existing nodes that are stored
-        node_id = get_new_id(set())
-        class_name = cls._class_name(class_prefix)
-
-        # if batch object is provided (via a contexxt manager), use that instead
-        if batch is not None:
-            batch.add_data_object(node_dict, class_name, node_id, vector)
-        else:
-            client.batch.add_data_object(node_dict, class_name, node_id, vector)
-
-        return node_id
-
-    @classmethod
-    def delete_document(cls, client: Any, ref_doc_id: str, class_prefix: str) -> None:
-        """Delete entry."""
-        validate_client(client)
-        # make sure that each entry
-        class_name = cls._class_name(class_prefix)
-        where_filter = {
-            "path": ["ref_doc_id"],
-            "operator": "Equal",
-            "valueString": ref_doc_id,
+    # parse results
+    parsed_result = parse_get_response(query_result)
+    entries = parsed_result[class_name]
+    results = [_to_node(entry) for entry in entries]
+    return results
+
+
+def _class_name(class_prefix: str) -> str:
+    """Return class name."""
+    return f"{class_prefix}_Node"
+
+
+def _to_node(entry: Dict) -> Node:
+    """Convert to Node."""
+    extra_info_str = entry["extra_info"]
+    if extra_info_str == "":
+        extra_info = None
+    else:
+        extra_info = json.loads(extra_info_str)
+
+    node_info_str = entry["node_info"]
+    if node_info_str == "":
+        node_info = None
+    else:
+        node_info = json.loads(node_info_str)
+
+    relationships_str = entry["relationships"]
+    relationships: Dict[DocumentRelationship, str]
+    if relationships_str == "":
+        relationships = field(default_factory=dict)
+    else:
+        relationships = {
+            DocumentRelationship(k): v for k, v in json.loads(relationships_str).items()
         }
-        query = (
-            client.query.get(class_name)
-            .with_additional(["id"])
-            .with_where(where_filter)
-        )
 
-        query_result = query.do()
-        parsed_result = parse_get_response(query_result)
-        entries = parsed_result[class_name]
-        for entry in entries:
-            client.data_object.delete(entry["_additional"]["id"], class_name)
-
-    @classmethod
-    def from_llama_index_batch(
-        cls, client: Any, nodes: List[Node], class_prefix: str
-    ) -> List[str]:
-        """Convert from gpt index."""
-        from weaviate import Client  # noqa: F401
-
-        client = cast(Client, client)
-        validate_client(client)
-        index_ids = []
-        with client.batch as batch:
-            for node in nodes:
-                index_id = cls._from_llama_index(client, node, class_prefix, batch=batch)
-                index_ids.append(index_id)
-        return index_ids
+    return Node(
+        text=entry["text"],
+        doc_id=entry["doc_id"],
+        embedding=entry["_additional"]["vector"],
+        extra_info=extra_info,
+        node_info=node_info,
+        relationships=relationships,
+    )
+
+
+def _node_to_dict(node: Node) -> dict:
+    node_dict = node.to_dict()
+    node_dict.pop("embedding")  # NOTE: stored outside of dict
+
+    # json-serialize the extra_info
+    extra_info = node_dict.pop("extra_info")
+    extra_info_str = ""
+    if extra_info is not None:
+        extra_info_str = json.dumps(extra_info)
+    node_dict["extra_info"] = extra_info_str
+
+    # json-serialize the node_info
+    node_info = node_dict.pop("node_info")
+    node_info_str = ""
+    if node_info is not None:
+        node_info_str = json.dumps(node_info)
+    node_dict["node_info"] = node_info_str
+
+    # json-serialize the relationships
+    relationships = node_dict.pop("relationships")
+    relationships_str = ""
+    if relationships is not None:
+        relationships_str = json.dumps(relationships)
+    node_dict["relationships"] = relationships_str
+
+    ref_doc_id = node.ref_doc_id
+    if ref_doc_id is not None:
+        node_dict["ref_doc_id"] = ref_doc_id
+    return node_dict
+
+
+def _add_node(
+    client: Any, node: Node, class_prefix: str, batch: Optional[Any] = None
+) -> str:
+    """Add node."""
+    node_dict = _node_to_dict(node)
+    vector = node.embedding
+
+    # TODO: account for existing nodes that are stored
+    node_id = get_new_id(set())
+    class_name = _class_name(class_prefix)
+
+    # if batch object is provided (via a context manager), use that instead
+    if batch is not None:
+        batch.add_data_object(node_dict, class_name, node_id, vector)
+    else:
+        client.batch.add_data_object(node_dict, class_name, node_id, vector)
+
+    return node_id
+
+
+def delete_document(client: Any, ref_doc_id: str, class_prefix: str) -> None:
+    """Delete entry."""
+    validate_client(client)
+    # make sure that each entry
+    class_name = _class_name(class_prefix)
+    where_filter = {
+        "path": ["ref_doc_id"],
+        "operator": "Equal",
+        "valueString": ref_doc_id,
+    }
+    query = (
+        client.query.get(class_name).with_additional(["id"]).with_where(where_filter)
+    )
+
+    query_result = query.do()
+    parsed_result = parse_get_response(query_result)
+    entries = parsed_result[class_name]
+    for entry in entries:
+        client.data_object.delete(entry["_additional"]["id"], class_name)
+
+
+def add_node(client: Any, node: Node, class_prefix: str) -> str:
+    """Convert from LlamaIndex."""
+    validate_client(client)
+    index_id = _add_node(client, node, class_prefix)
+    client.batch.flush()
+    return index_id
+
+
+def add_nodes(client: Any, nodes: List[Node], class_prefix: str) -> List[str]:
+    """Add nodes."""
+    from weaviate import Client  # noqa: F401
+
+    client = cast(Client, client)
+    validate_client(client)
+    index_ids = []
+    with client.batch as batch:
+        for node in nodes:
+            index_id = _add_node(client, node, class_prefix, batch=batch)
+            index_ids.append(index_id)
+    return index_ids
```

### Comparing `llama_index-0.5.9/llama_index/readers/weaviate/reader.py` & `llama_index-0.6.0a1/llama_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/weaviate/utils.py` & `llama_index-0.6.0a1/llama_index/readers/weaviate/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/web.py` & `llama_index-0.6.0a1/llama_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/wikipedia.py` & `llama_index-0.6.0a1/llama_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/readers/youtube_transcript.py` & `llama_index-0.6.0a1/llama_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/response/notebook_utils.py` & `llama_index-0.6.0a1/llama_index/response/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/response/schema.py` & `llama_index-0.6.0a1/llama_index/response/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from llama_index.utils import truncate_text
 
 
 @dataclass
 class Response:
     """Response object.
 
-    Returned if streaming=False during the `index.query()` call.
+    Returned if streaming=False.
 
     Attributes:
         response: The response text.
 
     """
 
     response: Optional[str]
@@ -37,15 +37,15 @@
         return "\n\n".join(texts)
 
 
 @dataclass
 class StreamingResponse:
     """StreamingResponse object.
 
-    Returned if streaming=True during the `index.query()` call.
+    Returned if streaming=True.
 
     Attributes:
         response_gen: The response generator.
 
     """
 
     response_gen: Optional[Generator]
```

### Comparing `llama_index-0.5.9/llama_index/schema.py` & `llama_index-0.6.0a1/llama_index/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/token_counter/mock_chain_wrapper.py` & `llama_index-0.6.0a1/llama_index/token_counter/mock_chain_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/token_counter/mock_embed_model.py` & `llama_index-0.6.0a1/llama_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/token_counter/token_counter.py` & `llama_index-0.6.0a1/llama_index/token_counter/token_counter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/token_counter/utils.py` & `llama_index-0.6.0a1/llama_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/tools/file_utils.py` & `llama_index-0.6.0a1/llama_index/tools/file_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.5.9/llama_index/utils.py` & `llama_index-0.6.0a1/llama_index/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,27 @@
 import random
 import sys
 import time
 import traceback
 import uuid
 from contextlib import contextmanager
 from dataclasses import dataclass
-from typing import Any, Callable, Generator, List, Optional, Set, Type, cast
+from itertools import islice
+from typing import (
+    Any,
+    Callable,
+    Generator,
+    List,
+    Optional,
+    Set,
+    Type,
+    cast,
+    Union,
+    Iterable,
+)
 
 
 class GlobalsHelper:
     """Helper to retrieve globals.
 
     Helpful for global caching of certain variables that can be expensive to load.
     (e.g. tokenization)
@@ -61,15 +73,18 @@
             try:
                 import nltk
                 from nltk.corpus import stopwords
             except ImportError:
                 raise ImportError(
                     "`nltk` package not found, please run `pip install nltk`"
                 )
-            nltk.download("stopwords")
+            try:
+                nltk.data.find("corpora/stopwords")
+            except LookupError:
+                nltk.download("stopwords")
             self._stopwords = stopwords.words("english")
         return self._stopwords
 
 
 globals_helper = GlobalsHelper()
 
 
@@ -171,7 +186,21 @@
             time.sleep(backoff_secs)
             backoff_secs = min(backoff_secs * 2, max_backoff_secs)
 
 
 def truncate_text(text: str, max_length: int) -> str:
     """Truncate text to a maximum length."""
     return text[: max_length - 3] + "..."
+
+
+def iter_batch(iterable: Union[Iterable, Generator], size: int) -> Iterable:
+    """Iterate over an iterable in batches.
+
+    >>> list(iter_batch([1,2,3,4,5], 3))
+    [[1, 2, 3], [4, 5]]
+    """
+    source_iter = iter(iterable)
+    while source_iter:
+        b = list(islice(source_iter, size))
+        if len(b) == 0:
+            break
+        yield b
```

### Comparing `llama_index-0.5.9/llama_index/vector_stores/__init__.py` & `llama_index-0.6.0a1/llama_index/vector_stores/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """Vector stores."""
 
 from llama_index.vector_stores.chatgpt_plugin import ChatGPTRetrievalPluginClient
 from llama_index.vector_stores.chroma import ChromaVectorStore
+from llama_index.vector_stores.deeplake import DeepLakeVectorStore
 from llama_index.vector_stores.faiss import FaissVectorStore
+from llama_index.vector_stores.milvus import MilvusVectorStore
+from llama_index.vector_stores.myscale import MyScaleVectorStore
 from llama_index.vector_stores.opensearch import (
     OpensearchVectorClient,
     OpensearchVectorStore,
 )
 from llama_index.vector_stores.pinecone import PineconeVectorStore
 from llama_index.vector_stores.qdrant import QdrantVectorStore
 from llama_index.vector_stores.simple import SimpleVectorStore
@@ -18,8 +21,11 @@
     "PineconeVectorStore",
     "WeaviateVectorStore",
     "QdrantVectorStore",
     "ChromaVectorStore",
     "OpensearchVectorStore",
     "OpensearchVectorClient",
     "ChatGPTRetrievalPluginClient",
+    "MilvusVectorStore",
+    "DeepLakeVectorStore",
+    "MyScaleVectorStore",
 ]
```

### Comparing `llama_index-0.5.9/llama_index/vector_stores/chatgpt_plugin.py` & `llama_index-0.6.0a1/llama_index/vector_stores/chatgpt_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from tqdm.auto import tqdm
 
 from llama_index.data_structs.node_v2 import Node, DocumentRelationship
 from llama_index.vector_stores.types import (
     NodeEmbeddingResult,
     VectorStore,
     VectorStoreQueryResult,
+    VectorStoreQuery,
 )
 
 
 def convert_docs_to_json(embedding_results: List[NodeEmbeddingResult]) -> List[Dict]:
     """Convert docs to JSON."""
     docs = []
     for embedding_result in embedding_results:
@@ -77,32 +78,19 @@
         self._bearer_token = bearer_token or os.getenv("BEARER_TOKEN")
         self._retries = retries
         self._batch_size = batch_size
 
         self._s = requests.Session()
         self._s.mount("http://", HTTPAdapter(max_retries=self._retries))
 
-    @classmethod
-    def from_dict(cls, config_dict: Dict[str, Any]) -> "VectorStore":
-        return cls(**config_dict)
-
     @property
     def client(self) -> None:
         """Get client."""
         return None
 
-    @property
-    def config_dict(self) -> dict:
-        """Get config dict."""
-        return {
-            "endpoint_url": self._endpoint_url,
-            "batch_size": self._batch_size,
-            "retries": self._retries,
-        }
-
     def add(
         self,
         embedding_results: List[NodeEmbeddingResult],
     ) -> List[str]:
         """Add embedding_results to index."""
         headers = {"Authorization": f"Bearer {self._bearer_token}"}
 
@@ -124,25 +112,22 @@
             f"{self._endpoint_url}/delete",
             headers=headers,
             json={"ids": [doc_id]},
         )
 
     def query(
         self,
-        query_embedding: List[float],
-        similarity_top_k: int,
-        doc_ids: Optional[List[str]] = None,
-        query_str: Optional[str] = None,
+        query: VectorStoreQuery,
     ) -> VectorStoreQueryResult:
         """Get nodes for response."""
-        if query_str is None:
+        if query.query_str is None:
             raise ValueError("query_str must be provided")
         headers = {"Authorization": f"Bearer {self._bearer_token}"}
         # TODO: add metadata filter
-        queries = [{"query": query_str, "top_k": similarity_top_k}]
+        queries = [{"query": query.query_str, "top_k": query.similarity_top_k}]
         res = requests.post(
             f"{self._endpoint_url}/query", headers=headers, json={"queries": queries}
         )
 
         nodes = []
         similarities = []
         ids = []
```

### Comparing `llama_index-0.5.9/llama_index/vector_stores/chroma.py` & `llama_index-0.6.0a1/llama_index/vector_stores/chroma.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Chroma vector store."""
 import logging
 import math
-from typing import Any, Dict, List, Optional, cast
+from typing import Any, List, cast
 
 from llama_index.data_structs.node_v2 import DocumentRelationship, Node
 from llama_index.utils import truncate_text
 from llama_index.vector_stores.types import (
     NodeEmbeddingResult,
     VectorStore,
+    VectorStoreQuery,
     VectorStoreQueryResult,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class ChromaVectorStore(VectorStore):
@@ -39,25 +40,14 @@
             import chromadb  # noqa: F401
         except ImportError:
             raise ImportError(import_err_msg)
         from chromadb.api.models.Collection import Collection
 
         self._collection = cast(Collection, chroma_collection)
 
-    @classmethod
-    def from_dict(cls, config_dict: Dict[str, Any]) -> "VectorStore":
-        if "chroma_collection" not in config_dict:
-            raise ValueError("Missing chroma collection!")
-        return cls(**config_dict)
-
-    @property
-    def config_dict(self) -> dict:
-        """Return config dict."""
-        return {}
-
     def add(self, embedding_results: List[NodeEmbeddingResult]) -> List[str]:
         """Add embedding results to index.
 
         Args
             embedding_results: List[NodeEmbeddingResult]: list of embedding results
 
         """
@@ -93,30 +83,24 @@
         self._collection.delete(where={"document_id": doc_id})
 
     @property
     def client(self) -> Any:
         """Return client."""
         return self._collection
 
-    def query(
-        self,
-        query_embedding: List[float],
-        similarity_top_k: int,
-        doc_ids: Optional[List[str]] = None,
-        query_str: Optional[str] = None,
-    ) -> VectorStoreQueryResult:
+    def query(self, query: VectorStoreQuery) -> VectorStoreQueryResult:
         """Query index for top k most similar nodes.
 
         Args:
             query_embedding (List[float]): query embedding
             similarity_top_k (int): top k most similar nodes
 
         """
         results = self._collection.query(
-            query_embeddings=query_embedding, n_results=similarity_top_k
+            query_embeddings=query.query_embedding, n_results=query.similarity_top_k
         )
 
         logger.debug(f"> Top {len(results['documents'])} nodes:")
         nodes = []
         similarities = []
         ids = []
         for result in zip(
```

### Comparing `llama_index-0.5.9/llama_index/vector_stores/opensearch.py` & `llama_index-0.6.0a1/llama_index/vector_stores/opensearch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Elasticsearch/Opensearch vector store."""
 import json
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, cast
 
 from llama_index.data_structs import Node
 from llama_index.vector_stores.types import (
     NodeEmbeddingResult,
     VectorStore,
     VectorStoreQueryResult,
+    VectorStoreQuery,
 )
 
 
 class OpensearchVectorClient:
     """Object encapsulating an Opensearch index that has vector search enabled.
 
     If the index does not yet exist, it is created during init.
@@ -36,14 +37,15 @@
         self,
         endpoint: str,
         index: str,
         dim: int,
         embedding_field: str = "embedding",
         text_field: str = "content",
         method: Optional[dict] = None,
+        auth: Optional[dict] = None,
     ):
         """Init params."""
         if method is None:
             method = {
                 "name": "hnsw",
                 "space_type": "l2",
                 "engine": "nmslib",
@@ -53,15 +55,30 @@
         if embedding_field is None:
             embedding_field = "embedding"
         try:
             import httpx  # noqa: F401
         except ImportError:
             raise ImportError(import_err_msg)
         self._embedding_field = embedding_field
-        self._client = httpx.Client(base_url=endpoint)
+
+        if auth is None:
+            self._client = httpx.Client(base_url=endpoint)
+        else:
+            if "verify" not in auth:
+                # "Open search" docker image for Dev/Test requires SSL verification
+                # when accessing with HTTPS, https://localhost:9200.
+                auth["verify"] = False
+            if "basic_auth" not in auth:
+                # 'admin:admin' is the default username/password for the "Open search"
+                # docker image.
+                auth["basic_auth"] = ("admin", "admin")
+            self._client = httpx.Client(
+                base_url=endpoint, verify=auth["verify"], auth=auth["basic_auth"]
+            )
+
         self._endpoint = endpoint
         self._dim = dim
         self._index = index
         self._text_field = text_field
         # initialize mapping
         idx_conf = {
             "settings": {"index": {"knn": True, "knn.algo_param.ef_search": 100}},
@@ -152,30 +169,19 @@
         import_err_msg = "`httpx` package not found, please run `pip install httpx`"
         try:
             import httpx  # noqa: F401
         except ImportError:
             raise ImportError(import_err_msg)
         self._client = client
 
-    @classmethod
-    def from_dict(cls, config_dict: Dict[str, Any]) -> "VectorStore":
-        if "client" not in config_dict:
-            raise ValueError("Missing Opensearch client!")
-        return cls(**config_dict)
-
     @property
     def client(self) -> Any:
         """Get client."""
         return self._client
 
-    @property
-    def config_dict(self) -> dict:
-        """Get config dict."""
-        return {}
-
     def add(
         self,
         embedding_results: List[NodeEmbeddingResult],
     ) -> List[str]:
         """Add embedding results to index.
 
         Args
@@ -190,22 +196,17 @@
 
         Args:
             doc_id (str): document id
 
         """
         self._client.delete_doc_id(doc_id)
 
-    def query(
-        self,
-        query_embedding: List[float],
-        similarity_top_k: int,
-        doc_ids: Optional[List[str]] = None,
-        query_str: Optional[str] = None,
-    ) -> VectorStoreQueryResult:
+    def query(self, query: VectorStoreQuery) -> VectorStoreQueryResult:
         """Query index for top k most similar nodes.
 
         Args:
             query_embedding (List[float]): query embedding
             similarity_top_k (int): top k most similar nodes
 
         """
-        return self._client.do_approx_knn(query_embedding, similarity_top_k)
+        query_embedding = cast(List[float], query.query_embedding)
+        return self._client.do_approx_knn(query_embedding, query.similarity_top_k)
```

### Comparing `llama_index-0.5.9/llama_index/vector_stores/qdrant.py` & `llama_index-0.6.0a1/llama_index/vector_stores/qdrant.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Qdrant vector store index.
 
 An index that is built on top of an existing Qdrant collection.
 
 """
 import logging
-from typing import Any, Dict, List, Optional, cast
+from typing import Any, List, Optional, cast
 
 from llama_index.data_structs.node_v2 import DocumentRelationship, Node
-from llama_index.utils import get_new_id
+from llama_index.utils import iter_batch
 from llama_index.vector_stores.types import (
     NodeEmbeddingResult,
     VectorStore,
     VectorStoreQueryResult,
+    VectorStoreQuery,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class QdrantVectorStore(VectorStore):
     """Qdrant Vector Store.
@@ -48,78 +49,57 @@
         if client is None:
             raise ValueError("Missing Qdrant client!")
 
         self._client = cast(qdrant_client.QdrantClient, client)
         self._collection_name = collection_name
         self._collection_initialized = self._collection_exists(collection_name)
 
-    @classmethod
-    def from_dict(cls, config_dict: Dict[str, Any]) -> "VectorStore":
-        if "client" not in config_dict:
-            raise ValueError("Missing Qdrant client!")
-        return cls(**config_dict)
-
-    @property
-    def config_dict(self) -> dict:
-        """Return config dict."""
-        return {
-            "collection_name": self._collection_name,
-        }
+        self._batch_size = kwargs.get("batch_size", 100)
 
     def add(self, embedding_results: List[NodeEmbeddingResult]) -> List[str]:
         """Add embedding results to index.
 
         Args
             embedding_results: List[NodeEmbeddingResult]: list of embedding results
 
         """
         from qdrant_client.http import models as rest
-        from qdrant_client.http.exceptions import UnexpectedResponse
+
+        if len(embedding_results) > 0 and not self._collection_initialized:
+            self._create_collection(
+                collection_name=self._collection_name,
+                vector_size=len(embedding_results[0].embedding),
+            )
 
         ids = []
-        for result in embedding_results:
-            new_id = result.id
-            node = result.node
-            text_embedding = result.embedding
-            collection_name = self._collection_name
-            # assign a new_id if current_id conflicts with existing ids
-            while True:
-                try:
-                    self._client.http.points_api.get_point(
-                        collection_name=collection_name, id=new_id
-                    )
-                except UnexpectedResponse:
-                    break
-                new_id = get_new_id(set())
-
-            # Create the Qdrant collection, if it does not exist yet
-            if not self._collection_initialized:
-                self._create_collection(
-                    collection_name=collection_name,
-                    vector_size=len(text_embedding),
+        for result_batch in iter_batch(embedding_results, self._batch_size):
+            new_ids = []
+            vectors = []
+            payloads = []
+            for result in result_batch:
+                new_ids.append(result.id)
+                vectors.append(result.embedding)
+                node = result.node
+                payloads.append(
+                    {
+                        "doc_id": result.doc_id,
+                        "text": node.get_text(),
+                        "extra_info": node.extra_info,
+                    }
                 )
-                self._collection_initialized = True
-
-            payload = {
-                "doc_id": result.doc_id,
-                "text": node.get_text(),
-                "extra_info": node.extra_info,
-            }
 
             self._client.upsert(
-                collection_name=collection_name,
-                points=[
-                    rest.PointStruct(
-                        id=new_id,
-                        vector=text_embedding,
-                        payload=payload,
-                    )
-                ],
+                collection_name=self._collection_name,
+                points=rest.Batch.construct(
+                    ids=new_ids,
+                    vectors=vectors,
+                    payloads=payloads,
+                ),
             )
-            ids.append(new_id)
+            ids.extend(new_ids)
         return ids
 
     def delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         """Delete a document.
 
         Args:
             doc_id: (str): document id
@@ -150,63 +130,45 @@
         self._client.recreate_collection(
             collection_name=collection_name,
             vectors_config=rest.VectorParams(
                 size=vector_size,
                 distance=rest.Distance.COSINE,
             ),
         )
+        self._collection_initialized = True
 
     def _collection_exists(self, collection_name: str) -> bool:
         """Check if a collection exists."""
+        from grpc import RpcError
         from qdrant_client.http.exceptions import UnexpectedResponse
 
         try:
-            response = self._client.http.collections_api.get_collection(collection_name)
-            return response.result is not None
-        except UnexpectedResponse:
+            self._client.get_collection(collection_name)
+        except (RpcError, UnexpectedResponse, ValueError):
             return False
+        return True
 
     def query(
         self,
-        query_embedding: List[float],
-        similarity_top_k: int,
-        doc_ids: Optional[List[str]] = None,
-        query_str: Optional[str] = None,
+        query: VectorStoreQuery,
     ) -> VectorStoreQueryResult:
         """Query index for top k most similar nodes.
 
         Args:
-            query_embedding (List[float]): query embedding
-            similarity_top_k (int): top k most similar nodes
-            doc_ids (Optional[List[str]]): list of doc_ids to filter by
-
+            query (VectorStoreQuery): query
         """
-        from qdrant_client.http.models.models import (
-            FieldCondition,
-            Filter,
-            MatchValue,
-            Payload,
-        )
+        from qdrant_client.http.models import Payload, Filter
+
+        query_embedding = cast(List[float], query.query_embedding)
 
         response = self._client.search(
             collection_name=self._collection_name,
             query_vector=query_embedding,
-            limit=cast(int, similarity_top_k),
-            query_filter=None
-            if not doc_ids
-            else Filter(
-                must=[
-                    Filter(
-                        should=[
-                            FieldCondition(key="doc_id", match=MatchValue(value=doc_id))
-                            for doc_id in doc_ids
-                        ],
-                    )
-                ]
-            ),
+            limit=cast(int, query.similarity_top_k),
+            query_filter=cast(Filter, self._build_query_filter(query)),
         )
 
         logger.debug(f"> Top {len(response)} nodes:")
 
         nodes = []
         similarities = []
         ids = []
@@ -221,7 +183,28 @@
                 },
             )
             nodes.append(node)
             similarities.append(point.score)
             ids.append(str(point.id))
 
         return VectorStoreQueryResult(nodes=nodes, similarities=similarities, ids=ids)
+
+    def _build_query_filter(self, query: VectorStoreQuery) -> Optional[Any]:
+        if not query.doc_ids and not query.query_str:
+            return None
+
+        from qdrant_client.http.models import (
+            FieldCondition,
+            Filter,
+            MatchAny,
+        )
+
+        must_conditions = []
+
+        if query.doc_ids:
+            must_conditions.append(
+                FieldCondition(
+                    key="doc_id",
+                    match=MatchAny(any=[doc_id for doc_id in query.doc_ids]),
+                )
+            )
+        return Filter(must=must_conditions)
```

### Comparing `llama_index-0.5.9/llama_index/vector_stores/registry.py` & `llama_index-0.6.0a1/llama_index/vector_stores/registry.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,48 @@
 from enum import Enum
-from typing import Any, Dict, Optional, Type
-from llama_index.constants import DATA_KEY, TYPE_KEY
+from typing import Dict, Type
+
 from llama_index.vector_stores.chatgpt_plugin import ChatGPTRetrievalPluginClient
 from llama_index.vector_stores.chroma import ChromaVectorStore
+from llama_index.vector_stores.deeplake import DeepLakeVectorStore
 from llama_index.vector_stores.faiss import FaissVectorStore
+from llama_index.vector_stores.milvus import MilvusVectorStore
+from llama_index.vector_stores.myscale import MyScaleVectorStore
 from llama_index.vector_stores.opensearch import OpensearchVectorStore
 from llama_index.vector_stores.pinecone import PineconeVectorStore
 from llama_index.vector_stores.qdrant import QdrantVectorStore
 from llama_index.vector_stores.simple import SimpleVectorStore
-
 from llama_index.vector_stores.types import VectorStore
 from llama_index.vector_stores.weaviate import WeaviateVectorStore
 
 
 class VectorStoreType(str, Enum):
     SIMPLE = "simple"
     WEAVIATE = "weaviate"
     QDRANT = "qdrant"
     PINECONE = "pinecone"
     OPENSEARCH = "opensearch"
     FAISS = "faiss"
     CHROMA = "chroma"
     CHATGPT_PLUGIN = "chatgpt_plugin"
+    MILVUS = "milvus"
+    DEEPLAKE = "deeplake"
+    MYSCALE = "myscale"
 
 
 VECTOR_STORE_TYPE_TO_VECTOR_STORE_CLASS: Dict[VectorStoreType, Type[VectorStore]] = {
     VectorStoreType.SIMPLE: SimpleVectorStore,
     VectorStoreType.WEAVIATE: WeaviateVectorStore,
     VectorStoreType.QDRANT: QdrantVectorStore,
+    VectorStoreType.MILVUS: MilvusVectorStore,
     VectorStoreType.PINECONE: PineconeVectorStore,
     VectorStoreType.OPENSEARCH: OpensearchVectorStore,
     VectorStoreType.FAISS: FaissVectorStore,
     VectorStoreType.CHROMA: ChromaVectorStore,
     VectorStoreType.CHATGPT_PLUGIN: ChatGPTRetrievalPluginClient,
+    VectorStoreType.DEEPLAKE: DeepLakeVectorStore,
+    VectorStoreType.MYSCALE: MyScaleVectorStore,
 }
 
 VECTOR_STORE_CLASS_TO_VECTOR_STORE_TYPE: Dict[Type[VectorStore], VectorStoreType] = {
     cls_: type_ for type_, cls_ in VECTOR_STORE_TYPE_TO_VECTOR_STORE_CLASS.items()
 }
-
-
-def load_vector_store_from_dict(
-    vector_store_dict: Dict[str, Any],
-    type_to_cls: Optional[Dict[VectorStoreType, Type[VectorStore]]] = None,
-    **kwargs: Any,
-) -> VectorStore:
-    type_to_cls = type_to_cls or VECTOR_STORE_TYPE_TO_VECTOR_STORE_CLASS
-    type = vector_store_dict[TYPE_KEY]
-    config_dict: Dict[str, Any] = vector_store_dict[DATA_KEY]
-
-    # Inject kwargs into data dict.
-    # This allows us to explicitly pass in unserializable objects
-    # like the vector store client.
-    config_dict.update(kwargs)
-
-    cls = type_to_cls[type]
-    return cls.from_dict(config_dict)
-
-
-def save_vector_store_to_dict(
-    vector_store: VectorStore,
-    cls_to_type: Optional[Dict[Type[VectorStore], VectorStoreType]] = None,
-) -> Dict[str, Any]:
-    cls_to_type = cls_to_type or VECTOR_STORE_CLASS_TO_VECTOR_STORE_TYPE
-    type_ = cls_to_type[type(vector_store)]
-    return {TYPE_KEY: type_, DATA_KEY: vector_store.config_dict}
```

### Comparing `llama_index-0.5.9/llama_index/vector_stores/types.py` & `llama_index-0.6.0a1/llama_index/vector_stores/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 """Vector store index types."""
 
 
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Protocol, runtime_checkable
+from typing import Any, List, Optional, Protocol, runtime_checkable
 
+from enum import Enum
 from llama_index.data_structs.node_v2 import Node
 
 
+DEFAULT_PERSIST_DIR = "./storage"
+DEFAULT_PERSIST_FNAME = "vector_store.json"
+
+
 @dataclass
 class NodeEmbeddingResult:
     """Node embedding result.
 
     Args:
         id (str): Node id
         node (Node): Node
@@ -30,48 +35,69 @@
     """Vector store query result."""
 
     nodes: Optional[List[Node]] = None
     similarities: Optional[List[float]] = None
     ids: Optional[List[str]] = None
 
 
+class VectorStoreQueryMode(str, Enum):
+    """Vector store query mode."""
+
+    DEFAULT = "default"
+    SPARSE = "sparse"
+    HYBRID = "hybrid"
+
+    # fit learners
+    SVM = "svm"
+    LOGISTIC_REGRESSION = "logistic_regression"
+    LINEAR_REGRESSION = "linear_regression"
+
+
+@dataclass
+class VectorStoreQuery:
+    """Vector store query."""
+
+    # dense embedding
+    query_embedding: Optional[List[float]] = None
+    similarity_top_k: int = 1
+    doc_ids: Optional[List[str]] = None
+    query_str: Optional[str] = None
+
+    # NOTE: current mode
+    mode: VectorStoreQueryMode = VectorStoreQueryMode.DEFAULT
+
+    # NOTE: only for hybrid search (0 for bm25, 1 for vector search)
+    alpha: Optional[float] = None
+
+
 @runtime_checkable
 class VectorStore(Protocol):
     """Abstract vector store protocol."""
 
     stores_text: bool
     is_embedding_query: bool = True
 
-    @classmethod
-    def from_dict(cls, config_dict: Dict[str, Any]) -> "VectorStore":
-        ...
-
     @property
     def client(self) -> Any:
         """Get client."""
         ...
 
-    @property
-    def config_dict(self) -> dict:
-        """Get config dict."""
-        ...
-
     def add(
         self,
         embedding_results: List[NodeEmbeddingResult],
     ) -> List[str]:
         """Add embedding results to vector store."""
         ...
 
     def delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         """Delete doc."""
         ...
 
     def query(
         self,
-        query_embedding: List[float],
-        similarity_top_k: int,
-        doc_ids: Optional[List[str]] = None,
-        query_str: Optional[str] = None,
+        query: VectorStoreQuery,
     ) -> VectorStoreQueryResult:
         """Query vector store."""
         ...
+
+    def persist(self, persist_path: str) -> None:
+        return None
```

### Comparing `llama_index-0.5.9/llama_index/vector_stores/weaviate.py` & `llama_index-0.6.0a1/llama_index/vector_stores/weaviate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 """Weaviate Vector store index.
 
 An index that that is built on top of an existing vector store.
 
 """
 
-from typing import Any, Dict, List, Optional, cast
+from typing import Any, List, Optional, cast
 
-from llama_index.readers.weaviate.data_structs import WeaviateNode
+from llama_index.readers.weaviate.client import (
+    add_nodes,
+    create_schema,
+    delete_document,
+    weaviate_query,
+)
 from llama_index.readers.weaviate.utils import get_default_class_prefix
 from llama_index.vector_stores.types import (
     NodeEmbeddingResult,
     VectorStore,
     VectorStoreQueryResult,
+    VectorStoreQuery,
 )
 
 
 class WeaviateVectorStore(VectorStore):
     """Weaviate vector store.
 
     In this vector store, embeddings and docs are stored within a
@@ -56,32 +62,21 @@
         # validate class prefix starts with a capital letter
         if class_prefix is not None and not class_prefix[0].isupper():
             raise ValueError(
                 "Class prefix must start with a capital letter, e.g. 'Gpt'"
             )
         self._class_prefix = class_prefix or get_default_class_prefix()
         # try to create schema
-        WeaviateNode.create_schema(self._client, self._class_prefix)
-
-    @classmethod
-    def from_dict(cls, config_dict: Dict[str, Any]) -> "VectorStore":
-        if "weaviate_client" not in config_dict:
-            raise ValueError("Missing Weaviate client!")
-        return cls(**config_dict)
+        create_schema(self._client, self._class_prefix)
 
     @property
     def client(self) -> Any:
         """Get client."""
         return self._client
 
-    @property
-    def config_dict(self) -> dict:
-        """Get config dict."""
-        return {"class_prefix": self._class_prefix}
-
     def add(
         self,
         embedding_results: List[NodeEmbeddingResult],
     ) -> List[str]:
         """Add embedding results to index.
 
         Args
@@ -90,45 +85,30 @@
         """
         for result in embedding_results:
             node = result.node
             embedding = result.embedding
             # TODO: always store embedding in node
             node.embedding = embedding
 
-        WeaviateNode.from_llama_index_batch(
-            self._client, [r.node for r in embedding_results], self._class_prefix
-        )
+        add_nodes(self._client, [r.node for r in embedding_results], self._class_prefix)
         return [result.id for result in embedding_results]
 
     def delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         """Delete a document.
 
         Args:
             doc_id (str): document id
 
         """
-        WeaviateNode.delete_document(self._client, doc_id, self._class_prefix)
+        delete_document(self._client, doc_id, self._class_prefix)
 
-    def query(
-        self,
-        query_embedding: List[float],
-        similarity_top_k: int,
-        doc_ids: Optional[List[str]] = None,
-        query_str: Optional[str] = None,
-    ) -> VectorStoreQueryResult:
-        """Query index for top k most similar nodes.
-
-        Args:
-            query_embedding (List[float]): query embedding
-            similarity_top_k (int): top k most similar nodes
-
-        """
-        nodes = WeaviateNode.to_llama_index_list(
-            self.client,
+    def query(self, query: VectorStoreQuery) -> VectorStoreQueryResult:
+        """Query index for top k most similar nodes."""
+        nodes = weaviate_query(
+            self._client,
             self._class_prefix,
-            vector=query_embedding,
-            object_limit=similarity_top_k,
+            query,
         )
-        nodes = nodes[:similarity_top_k]
+        nodes = nodes[: query.similarity_top_k]
         node_idxs = [str(i) for i in range(len(nodes))]
 
         return VectorStoreQueryResult(nodes=nodes, ids=node_idxs)
```

### Comparing `llama_index-0.5.9/llama_index.egg-info/PKG-INFO` & `llama_index-0.6.0a1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,26 @@
-Metadata-Version: 2.1
-Name: llama-index
-Version: 0.5.9
-Summary: Interface between LLMs and your data.
-Home-page: https://github.com/jerryjliu/gpt_index
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# 🗂️ LlamaIndex 🦙 (GPT Index)
-
-> ⚠️ **NOTE**: We are rebranding GPT Index as LlamaIndex! We will carry out this transition gradually.
-
-> **2/25/2023**: By default, our docs/notebooks/instructions now reference "LlamaIndex"
-instead of "GPT Index".
-
-> **2/19/2023**: By default, our docs/notebooks/instructions now use the `llama-index` package. However the `gpt-index` package still exists as a duplicate!
-
-> **2/16/2023**: We have a duplicate `llama-index` pip package. Simply replace all imports of `gpt_index` with `llama_index` if you choose to `pip install llama-index`.
+# 🗂️ LlamaIndex 🦙
 
 LlamaIndex (GPT Index) is a project that provides a central interface to connect your LLM's with external data.
 
 PyPi: 
 - LlamaIndex: https://pypi.org/project/llama-index/.
 - GPT Index (duplicate): https://pypi.org/project/gpt-index/.
 
 Documentation: https://gpt-index.readthedocs.io/en/latest/.
 
 Twitter: https://twitter.com/gpt_index.
 
 Discord: https://discord.gg/dGcwcsnxhU.
 
-LlamaHub (community library of data loaders): https://llamahub.ai
+### Ecosystem
+
+- LlamaHub (community library of data loaders): https://llamahub.ai
+- Llama Lab (cutting-edge AGI projects using LlamaIndex): https://github.com/run-llama/llama-lab
+
 
 ## 🚀 Overview
 
 **NOTE**: This README is not updated as frequently as the documentation. Please check out the documentation above for the latest updates!
 
 ### Context
 - LLMs are a phenomenonal piece of technology for knowledge generation and reasoning. They are pre-trained on large amounts of publicly available data.
@@ -80,32 +66,45 @@
 Examples are in the `examples` folder. Indices are in the `indices` folder (see list of indices below).
 
 To build a simple vector store index:
 ```python
 import os
 os.environ["OPENAI_API_KEY"] = 'YOUR_OPENAI_API_KEY'
 
-from llama_index import GPTSimpleVectorIndex, SimpleDirectoryReader
+from llama_index import GPTVectorStoreIndex, SimpleDirectoryReader
 documents = SimpleDirectoryReader('data').load_data()
-index = GPTSimpleVectorIndex.from_documents(documents)
+index = GPTVectorStoreIndex.from_documents(documents)
 ```
 
-To save to and load from disk:
+
+To query:
 ```python
-# save to disk
-index.save_to_disk('index.json')
-# load from disk
-index = GPTSimpleVectorIndex.load_from_disk('index.json')
+query_engine = index.as_query_engine()
+query_engine.query("<question_text>?")
 ```
 
-To query:
+
+By default, data is stored in-memory.
+To persist to disk (under `./storage`):
+
+```python
+index.storage_context.persist()
+```
+
+To reload from disk:
 ```python
-index.query("<question_text>?")
+from llama_index import StorageContext, load_index_from_storage
+
+# rebuild storage context
+storage_context = StorageContext.from_defaults(persist_dir='./storage')
+# load index
+index = load_index_from_storage(storage_context)
 ```
 
+
 ## 🔧 Dependencies
 
 The main third-party package requirements are `tiktoken`, `openai`, and `langchain`.
 
 All requirements should be contained within the `setup.py` file. To run the package locally without building the wheel, simply run `pip install -r requirements.txt`.
```

### Comparing `llama_index-0.5.9/llama_index.egg-info/SOURCES.txt` & `llama_index-0.6.0a1/llama_index.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 MANIFEST.in
 README.md
 setup.py
 llama_index/VERSION
 llama_index/__init__.py
 llama_index/async_utils.py
 llama_index/constants.py
-llama_index/docstore.py
 llama_index/img_utils.py
 llama_index/old_docstore.py
 llama_index/py.typed
 llama_index/schema.py
 llama_index/types.py
 llama_index/utils.py
 llama_index.egg-info/PKG-INFO
@@ -21,102 +20,104 @@
 llama_index/composability/__init__.py
 llama_index/composability/base.py
 llama_index/composability/joint_qa_summary.py
 llama_index/data_structs/__init__.py
 llama_index/data_structs/data_structs.py
 llama_index/data_structs/data_structs_v2.py
 llama_index/data_structs/node_v2.py
+llama_index/data_structs/registry.py
 llama_index/data_structs/struct_type.py
 llama_index/data_structs/table.py
 llama_index/data_structs/table_v2.py
 llama_index/embeddings/__init__.py
 llama_index/embeddings/base.py
 llama_index/embeddings/langchain.py
 llama_index/embeddings/openai.py
 llama_index/embeddings/utils.py
 llama_index/evaluation/__init__.py
 llama_index/evaluation/base.py
+llama_index/evaluation/dataset_generation.py
 llama_index/indices/__init__.py
 llama_index/indices/base.py
+llama_index/indices/base_retriever.py
+llama_index/indices/loading.py
 llama_index/indices/prompt_helper.py
 llama_index/indices/registry.py
 llama_index/indices/service_context.py
 llama_index/indices/utils.py
 llama_index/indices/common/__init__.py
 llama_index/indices/common/struct_store/__init__.py
 llama_index/indices/common/struct_store/base.py
 llama_index/indices/common/struct_store/schema.py
 llama_index/indices/common/struct_store/sql.py
 llama_index/indices/common_tree/__init__.py
 llama_index/indices/common_tree/base.py
 llama_index/indices/composability/__init__.py
 llama_index/indices/composability/graph.py
-llama_index/indices/composability/utils.py
 llama_index/indices/empty/__init__.py
 llama_index/indices/empty/base.py
-llama_index/indices/empty/query.py
+llama_index/indices/empty/retrievers.py
 llama_index/indices/keyword_table/__init__.py
 llama_index/indices/keyword_table/base.py
-llama_index/indices/keyword_table/query.py
 llama_index/indices/keyword_table/rake_base.py
+llama_index/indices/keyword_table/retrievers.py
 llama_index/indices/keyword_table/simple_base.py
 llama_index/indices/keyword_table/utils.py
 llama_index/indices/knowledge_graph/__init__.py
 llama_index/indices/knowledge_graph/base.py
-llama_index/indices/knowledge_graph/query.py
+llama_index/indices/knowledge_graph/retrievers.py
 llama_index/indices/list/__init__.py
 llama_index/indices/list/base.py
-llama_index/indices/list/embedding_query.py
-llama_index/indices/list/query.py
+llama_index/indices/list/retrievers.py
 llama_index/indices/postprocessor/__init__.py
 llama_index/indices/postprocessor/base.py
 llama_index/indices/postprocessor/node.py
+llama_index/indices/postprocessor/node_recency.py
+llama_index/indices/postprocessor/pii.py
 llama_index/indices/query/__init__.py
 llama_index/indices/query/base.py
 llama_index/indices/query/embedding_utils.py
-llama_index/indices/query/query_runner.py
+llama_index/indices/query/response_synthesis.py
 llama_index/indices/query/schema.py
-llama_index/indices/query/query_combiner/__init__.py
-llama_index/indices/query/query_combiner/base.py
-llama_index/indices/query/query_combiner/prompts.py
 llama_index/indices/query/query_transform/__init__.py
 llama_index/indices/query/query_transform/base.py
 llama_index/indices/query/query_transform/prompts.py
 llama_index/indices/response/__init__.py
-llama_index/indices/response/builder.py
+llama_index/indices/response/response_builder.py
+llama_index/indices/response/type.py
 llama_index/indices/struct_store/__init__.py
 llama_index/indices/struct_store/base.py
 llama_index/indices/struct_store/container_builder.py
 llama_index/indices/struct_store/pandas.py
 llama_index/indices/struct_store/pandas_query.py
 llama_index/indices/struct_store/sql.py
 llama_index/indices/struct_store/sql_query.py
 llama_index/indices/tree/__init__.py
+llama_index/indices/tree/all_leaf_retriever.py
 llama_index/indices/tree/base.py
-llama_index/indices/tree/embedding_query.py
 llama_index/indices/tree/inserter.py
-llama_index/indices/tree/leaf_query.py
-llama_index/indices/tree/retrieve_query.py
-llama_index/indices/tree/summarize_query.py
+llama_index/indices/tree/select_leaf_embedding_retriever.py
+llama_index/indices/tree/select_leaf_retriever.py
+llama_index/indices/tree/tree_root_retriever.py
 llama_index/indices/vector_store/__init__.py
 llama_index/indices/vector_store/base.py
-llama_index/indices/vector_store/base_query.py
-llama_index/indices/vector_store/vector_indices.py
+llama_index/indices/vector_store/retrievers.py
 llama_index/langchain_helpers/__init__.py
 llama_index/langchain_helpers/chain_wrapper.py
 llama_index/langchain_helpers/memory_wrapper.py
 llama_index/langchain_helpers/sql_wrapper.py
 llama_index/langchain_helpers/text_splitter.py
 llama_index/langchain_helpers/agents/__init__.py
 llama_index/langchain_helpers/agents/agents.py
 llama_index/langchain_helpers/agents/toolkits.py
 llama_index/langchain_helpers/agents/tools.py
 llama_index/llm_predictor/__init__.py
 llama_index/llm_predictor/base.py
 llama_index/llm_predictor/chatgpt.py
+llama_index/llm_predictor/stable_lm.py
 llama_index/llm_predictor/structured.py
 llama_index/logger/__init__.py
 llama_index/logger/base.py
 llama_index/node_parser/__init__.py
 llama_index/node_parser/interface.py
 llama_index/node_parser/node_utils.py
 llama_index/node_parser/simple.py
@@ -131,25 +132,33 @@
 llama_index/prompts/__init__.py
 llama_index/prompts/base.py
 llama_index/prompts/chat_prompts.py
 llama_index/prompts/default_prompt_selectors.py
 llama_index/prompts/default_prompts.py
 llama_index/prompts/prompt_type.py
 llama_index/prompts/prompts.py
+llama_index/query_engine/__init__.py
+llama_index/query_engine/graph_query_engine.py
+llama_index/query_engine/multistep_query_engine.py
+llama_index/query_engine/retriever_query_engine.py
+llama_index/query_engine/transform_query_engine.py
 llama_index/readers/__init__.py
 llama_index/readers/base.py
 llama_index/readers/chroma.py
 llama_index/readers/database.py
+llama_index/readers/deeplake.py
 llama_index/readers/discord_reader.py
 llama_index/readers/download.py
 llama_index/readers/elasticsearch.py
 llama_index/readers/faiss.py
 llama_index/readers/json.py
 llama_index/readers/mbox.py
+llama_index/readers/milvus.py
 llama_index/readers/mongo.py
+llama_index/readers/myscale.py
 llama_index/readers/notion.py
 llama_index/readers/obsidian.py
 llama_index/readers/pinecone.py
 llama_index/readers/qdrant.py
 llama_index/readers/slack.py
 llama_index/readers/string_iterable.py
 llama_index/readers/twitter.py
@@ -159,15 +168,18 @@
 llama_index/readers/chatgpt_plugin/__init__.py
 llama_index/readers/chatgpt_plugin/base.py
 llama_index/readers/file/__init__.py
 llama_index/readers/file/base.py
 llama_index/readers/file/base_parser.py
 llama_index/readers/file/docs_parser.py
 llama_index/readers/file/epub_parser.py
+llama_index/readers/file/image_caption_parser.py
 llama_index/readers/file/image_parser.py
+llama_index/readers/file/image_vision_llm_parser.py
+llama_index/readers/file/ipynb_parser.py
 llama_index/readers/file/markdown_parser.py
 llama_index/readers/file/mbox_parser.py
 llama_index/readers/file/slides_parser.py
 llama_index/readers/file/tabular_parser.py
 llama_index/readers/file/video_audio.py
 llama_index/readers/github_readers/__init__.py
 llama_index/readers/github_readers/github_api_client.py
@@ -179,33 +191,56 @@
 llama_index/readers/make_com/__init__.py
 llama_index/readers/make_com/wrapper.py
 llama_index/readers/schema/__init__.py
 llama_index/readers/schema/base.py
 llama_index/readers/steamship/__init__.py
 llama_index/readers/steamship/file_reader.py
 llama_index/readers/weaviate/__init__.py
-llama_index/readers/weaviate/data_structs.py
+llama_index/readers/weaviate/client.py
 llama_index/readers/weaviate/reader.py
 llama_index/readers/weaviate/utils.py
 llama_index/response/__init__.py
 llama_index/response/notebook_utils.py
 llama_index/response/schema.py
 llama_index/response/utils.py
+llama_index/retrievers/__init__.py
+llama_index/retrievers/transform_retriever.py
+llama_index/storage/__init__.py
+llama_index/storage/storage_context.py
+llama_index/storage/docstore/__init__.py
+llama_index/storage/docstore/keyval_docstore.py
+llama_index/storage/docstore/mongo_docstore.py
+llama_index/storage/docstore/registry.py
+llama_index/storage/docstore/simple_docstore.py
+llama_index/storage/docstore/types.py
+llama_index/storage/docstore/utils.py
+llama_index/storage/index_store/__init__.py
+llama_index/storage/index_store/keyval_index_store.py
+llama_index/storage/index_store/mongo_index_store.py
+llama_index/storage/index_store/simple_index_store.py
+llama_index/storage/index_store/types.py
+llama_index/storage/index_store/utils.py
+llama_index/storage/kvstore/__init__.py
+llama_index/storage/kvstore/mongodb_kvstore.py
+llama_index/storage/kvstore/simple_kvstore.py
+llama_index/storage/kvstore/types.py
 llama_index/token_counter/__init__.py
 llama_index/token_counter/mock_chain_wrapper.py
 llama_index/token_counter/mock_embed_model.py
 llama_index/token_counter/token_counter.py
 llama_index/token_counter/utils.py
 llama_index/tools/__init__.py
 llama_index/tools/file_utils.py
-llama_index/tools/migrate_v1_to_v2.py
 llama_index/vector_stores/__init__.py
 llama_index/vector_stores/chatgpt_plugin.py
 llama_index/vector_stores/chroma.py
+llama_index/vector_stores/deeplake.py
 llama_index/vector_stores/faiss.py
+llama_index/vector_stores/milvus.py
+llama_index/vector_stores/myscale.py
 llama_index/vector_stores/opensearch.py
 llama_index/vector_stores/pinecone.py
 llama_index/vector_stores/qdrant.py
 llama_index/vector_stores/registry.py
 llama_index/vector_stores/simple.py
 llama_index/vector_stores/types.py
 llama_index/vector_stores/weaviate.py
```

### Comparing `llama_index-0.5.9/setup.py` & `llama_index-0.6.0a1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     __version__ = _f.read().strip()
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 install_requires = [
     "dataclasses_json",
-    "langchain",
+    "langchain==0.0.142",
     "numpy",
     "tenacity>=8.2.0,<9.0.0",
     "openai>=0.26.4",
     "pandas",
 ]
 
 # NOTE: if python version >= 3.9, install tiktoken
```


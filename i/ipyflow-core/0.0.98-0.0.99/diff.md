# Comparing `tmp/ipyflow-core-0.0.98.tar.gz` & `tmp/ipyflow-core-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyflow-core-0.0.98.tar", last modified: Mon Jun  6 01:56:05 2022, max compression
+gzip compressed data, was "ipyflow-core-0.0.99.tar", last modified: Mon Jun  6 21:50:00 2022, max compression
```

## Comparing `ipyflow-core-0.0.98.tar` & `ipyflow-core-0.0.99.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:05.152081 ipyflow-core-0.0.98/
--rw-r--r--   0 smacke     (501) staff       (20)     1458 2022-03-26 20:08:59.000000 ipyflow-core-0.0.98/LICENSE.txt
--rw-r--r--   0 smacke     (501) staff       (20)       50 2022-03-27 01:32:25.000000 ipyflow-core-0.0.98/MANIFEST.in
--rw-r--r--   0 smacke     (501) staff       (20)      895 2022-06-06 01:56:05.152211 ipyflow-core-0.0.98/PKG-INFO
--rw-r--r--   0 smacke     (501) staff       (20)       29 2022-03-26 20:08:59.000000 ipyflow-core-0.0.98/README.md
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:05.117908 ipyflow-core-0.0.98/ipyflow/
--rw-r--r--   0 smacke     (501) staff       (20)      648 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/__init__.py
--rw-r--r--   0 smacke     (501) staff       (20)    23704 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/_version.py
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:05.121009 ipyflow-core-0.0.98/ipyflow/analysis/
--rw-r--r--   0 smacke     (501) staff       (20)       24 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/analysis/__init__.py
--rw-r--r--   0 smacke     (501) staff       (20)    16198 2022-05-15 17:47:02.000000 ipyflow-core-0.0.98/ipyflow/analysis/live_refs.py
--rw-r--r--   0 smacke     (501) staff       (20)     1245 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/analysis/mixins.py
--rw-r--r--   0 smacke     (501) staff       (20)     4799 2022-04-17 06:28:05.000000 ipyflow-core-0.0.98/ipyflow/analysis/resolved_symbols.py
--rw-r--r--   0 smacke     (501) staff       (20)     9116 2022-05-29 17:08:26.000000 ipyflow-core-0.0.98/ipyflow/analysis/slicing.py
--rw-r--r--   0 smacke     (501) staff       (20)     4062 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/analysis/symbol_edges.py
--rw-r--r--   0 smacke     (501) staff       (20)    13213 2022-04-19 03:49:49.000000 ipyflow-core-0.0.98/ipyflow/analysis/symbol_ref.py
--rw-r--r--   0 smacke     (501) staff       (20)     1220 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/analysis/utils.py
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:05.122102 ipyflow-core-0.0.98/ipyflow/api/
--rw-r--r--   0 smacke     (501) staff       (20)       58 2022-05-29 16:33:19.000000 ipyflow-core-0.0.98/ipyflow/api/__init__.py
--rw-r--r--   0 smacke     (501) staff       (20)      580 2022-06-02 06:08:23.000000 ipyflow-core-0.0.98/ipyflow/api/lift.py
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:05.125516 ipyflow-core-0.0.98/ipyflow/data_model/
--rw-r--r--   0 smacke     (501) staff       (20)       24 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/data_model/__init__.py
--rw-r--r--   0 smacke     (501) staff       (20)     4088 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/data_model/annotation_utils.py
--rw-r--r--   0 smacke     (501) staff       (20)    16815 2022-05-14 20:46:11.000000 ipyflow-core-0.0.98/ipyflow/data_model/code_cell.py
--rw-r--r--   0 smacke     (501) staff       (20)    36058 2022-05-30 16:57:20.000000 ipyflow-core-0.0.98/ipyflow/data_model/data_symbol.py
--rw-r--r--   0 smacke     (501) staff       (20)    12768 2022-05-04 23:30:31.000000 ipyflow-core-0.0.98/ipyflow/data_model/namespace.py
--rw-r--r--   0 smacke     (501) staff       (20)    12844 2022-05-15 17:38:57.000000 ipyflow-core-0.0.98/ipyflow/data_model/scope.py
--rw-r--r--   0 smacke     (501) staff       (20)     1371 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/data_model/sizing.py
--rw-r--r--   0 smacke     (501) staff       (20)     1891 2022-05-16 03:00:35.000000 ipyflow-core-0.0.98/ipyflow/data_model/timestamp.py
--rw-r--r--   0 smacke     (501) staff       (20)     8196 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/data_model/update_protocol.py
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:05.126213 ipyflow-core-0.0.98/ipyflow/experimental/
--rw-r--r--   0 smacke     (501) staff       (20)       24 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/experimental/__init__.py
--rw-r--r--   0 smacke     (501) staff       (20)     3388 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/experimental/dag.py
--rw-r--r--   0 smacke     (501) staff       (20)    16976 2022-06-06 01:31:39.000000 ipyflow-core-0.0.98/ipyflow/flow.py
--rw-r--r--   0 smacke     (501) staff       (20)    16958 2022-05-23 06:09:09.000000 ipyflow-core-0.0.98/ipyflow/frontend.py
--rw-r--r--   0 smacke     (501) staff       (20)      177 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/install.py
--rw-r--r--   0 smacke     (501) staff       (20)     4947 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/ipython_utils.py
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:05.128636 ipyflow-core-0.0.98/ipyflow/kernel/
--rw-r--r--   0 smacke     (501) staff       (20)       59 2022-05-21 18:38:35.000000 ipyflow-core-0.0.98/ipyflow/kernel/__init__.py
--rw-r--r--   0 smacke     (501) staff       (20)      467 2022-05-21 18:39:20.000000 ipyflow-core-0.0.98/ipyflow/kernel/__main__.py
--rw-r--r--   0 smacke     (501) staff       (20)     2536 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/kernel/install.py
--rw-r--r--   0 smacke     (501) staff       (20)    18145 2022-05-21 18:39:00.000000 ipyflow-core-0.0.98/ipyflow/kernel/kernel.py
--rw-r--r--   0 smacke     (501) staff       (20)     1344 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/kernel/patched_nest_asyncio.py
--rw-r--r--   0 smacke     (501) staff       (20)    14963 2022-05-21 18:47:30.000000 ipyflow-core-0.0.98/ipyflow/line_magics.py
--rw-r--r--   0 smacke     (501) staff       (20)      705 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/run_mode.py
--rw-r--r--   0 smacke     (501) staff       (20)     1139 2022-05-21 18:38:05.000000 ipyflow-core-0.0.98/ipyflow/singletons.py
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:05.133159 ipyflow-core-0.0.98/ipyflow/tracing/
--rw-r--r--   0 smacke     (501) staff       (20)       24 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/tracing/__init__.py
--rw-r--r--   0 smacke     (501) staff       (20)      712 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/tracing/flow_ast_rewriter.py
--rw-r--r--   0 smacke     (501) staff       (20)    57696 2022-06-02 06:13:19.000000 ipyflow-core-0.0.98/ipyflow/tracing/ipyflow_tracer.py
--rw-r--r--   0 smacke     (501) staff       (20)     2341 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/tracing/mutation_event.py
--rw-r--r--   0 smacke     (501) staff       (20)     1130 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/tracing/mutation_special_cases.py
--rw-r--r--   0 smacke     (501) staff       (20)    10110 2022-05-21 19:39:36.000000 ipyflow-core-0.0.98/ipyflow/tracing/symbol_resolver.py
--rw-r--r--   0 smacke     (501) staff       (20)    20598 2022-06-02 19:07:30.000000 ipyflow-core-0.0.98/ipyflow/tracing/trace_stmt.py
--rw-r--r--   0 smacke     (501) staff       (20)     1319 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/tracing/utils.py
--rw-r--r--   0 smacke     (501) staff       (20)      251 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/types.py
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:05.135043 ipyflow-core-0.0.98/ipyflow/utils/
--rw-r--r--   0 smacke     (501) staff       (20)       96 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/utils/__init__.py
--rw-r--r--   0 smacke     (501) staff       (20)       84 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/utils/ast_utils.py
--rw-r--r--   0 smacke     (501) staff       (20)      140 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/utils/misc_utils.py
--rw-r--r--   0 smacke     (501) staff       (20)      169 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/utils/mixins.py
--rw-r--r--   0 smacke     (501) staff       (20)      520 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/ipyflow/version.py
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:05.137625 ipyflow-core-0.0.98/ipyflow_core.egg-info/
--rw-r--r--   0 smacke     (501) staff       (20)      895 2022-06-06 01:56:04.000000 ipyflow-core-0.0.98/ipyflow_core.egg-info/PKG-INFO
--rw-r--r--   0 smacke     (501) staff       (20)     2210 2022-06-06 01:56:05.000000 ipyflow-core-0.0.98/ipyflow_core.egg-info/SOURCES.txt
--rw-r--r--   0 smacke     (501) staff       (20)        1 2022-06-06 01:56:04.000000 ipyflow-core-0.0.98/ipyflow_core.egg-info/dependency_links.txt
--rw-r--r--   0 smacke     (501) staff       (20)        1 2022-06-06 01:56:03.000000 ipyflow-core-0.0.98/ipyflow_core.egg-info/not-zip-safe
--rw-r--r--   0 smacke     (501) staff       (20)      362 2022-06-06 01:56:04.000000 ipyflow-core-0.0.98/ipyflow_core.egg-info/requires.txt
--rw-r--r--   0 smacke     (501) staff       (20)        8 2022-06-06 01:56:05.000000 ipyflow-core-0.0.98/ipyflow_core.egg-info/top_level.txt
--rw-r--r--   0 smacke     (501) staff       (20)      866 2022-03-27 01:43:17.000000 ipyflow-core-0.0.98/pyproject.toml
--rw-r--r--   0 smacke     (501) staff       (20)     1661 2022-06-06 01:56:05.152924 ipyflow-core-0.0.98/setup.cfg
--rw-r--r--   0 smacke     (501) staff       (20)      116 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/setup.py
-drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 01:56:05.151623 ipyflow-core-0.0.98/test/
--rw-r--r--   0 smacke     (501) staff       (20)     2634 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/test/test_annotations.py
--rw-r--r--   0 smacke     (501) staff       (20)      775 2022-05-30 16:58:35.000000 ipyflow-core-0.0.98/test/test_api.py
--rw-r--r--   0 smacke     (501) staff       (20)      810 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/test/test_ast_rewriting.py
--rw-r--r--   0 smacke     (501) staff       (20)     1409 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/test/test_attribute_symbols.py
--rw-r--r--   0 smacke     (501) staff       (20)     1252 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/test/test_cell_dag.py
--rw-r--r--   0 smacke     (501) staff       (20)    15505 2022-04-26 05:34:13.000000 ipyflow-core-0.0.98/test/test_dynamic_slicing.py
--rw-r--r--   0 smacke     (501) staff       (20)    16119 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/test/test_frontend_checker.py
--rw-r--r--   0 smacke     (501) staff       (20)     6828 2022-05-21 18:47:30.000000 ipyflow-core-0.0.98/test/test_line_magics.py
--rw-r--r--   0 smacke     (501) staff       (20)     1996 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/test/test_lineno_stmt_map.py
--rw-r--r--   0 smacke     (501) staff       (20)     2470 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/test/test_liveness_analysis.py
--rw-r--r--   0 smacke     (501) staff       (20)     7739 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/test/test_nested_symbols.py
--rw-r--r--   0 smacke     (501) staff       (20)     1342 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/test/test_no_prints.py
--rw-r--r--   0 smacke     (501) staff       (20)     3281 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/test/test_reactive_atom_detection.py
--rw-r--r--   0 smacke     (501) staff       (20)    13575 2022-05-14 20:45:38.000000 ipyflow-core-0.0.98/test/test_reactivity.py
--rw-r--r--   0 smacke     (501) staff       (20)     1060 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/test/test_refcount.py
--rw-r--r--   0 smacke     (501) staff       (20)     4481 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/test/test_stability.py
--rw-r--r--   0 smacke     (501) staff       (20)    65188 2022-05-04 23:31:47.000000 ipyflow-core-0.0.98/test/test_staleness_propagation.py
--rw-r--r--   0 smacke     (501) staff       (20)    24411 2022-05-30 18:12:09.000000 ipyflow-core-0.0.98/test/test_trace_events.py
--rw-r--r--   0 smacke     (501) staff       (20)     1454 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/test/test_typechecking.py
--rw-r--r--   0 smacke     (501) staff       (20)     1408 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/test/test_updated_symbols.py
--rw-r--r--   0 smacke     (501) staff       (20)    81180 2022-04-17 02:14:02.000000 ipyflow-core-0.0.98/versioneer.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:50:00.177916 ipyflow-core-0.0.99/
+-rw-r--r--   0 smacke     (501) staff       (20)     1458 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/LICENSE.txt
+-rw-r--r--   0 smacke     (501) staff       (20)       50 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/MANIFEST.in
+-rw-r--r--   0 smacke     (501) staff       (20)      895 2022-06-06 21:50:00.178137 ipyflow-core-0.0.99/PKG-INFO
+-rw-r--r--   0 smacke     (501) staff       (20)       29 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/README.md
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:50:00.153138 ipyflow-core-0.0.99/ipyflow/
+-rw-r--r--   0 smacke     (501) staff       (20)      648 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/__init__.py
+-rw-r--r--   0 smacke     (501) staff       (20)    23704 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/_version.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:50:00.156114 ipyflow-core-0.0.99/ipyflow/analysis/
+-rw-r--r--   0 smacke     (501) staff       (20)       24 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/analysis/__init__.py
+-rw-r--r--   0 smacke     (501) staff       (20)    16198 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/analysis/live_refs.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1245 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/analysis/mixins.py
+-rw-r--r--   0 smacke     (501) staff       (20)     4799 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/analysis/resolved_symbols.py
+-rw-r--r--   0 smacke     (501) staff       (20)     9116 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/analysis/slicing.py
+-rw-r--r--   0 smacke     (501) staff       (20)     4062 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/analysis/symbol_edges.py
+-rw-r--r--   0 smacke     (501) staff       (20)    13213 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/analysis/symbol_ref.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1220 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/analysis/utils.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:50:00.156761 ipyflow-core-0.0.99/ipyflow/api/
+-rw-r--r--   0 smacke     (501) staff       (20)       58 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/api/__init__.py
+-rw-r--r--   0 smacke     (501) staff       (20)      580 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/api/lift.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:50:00.160602 ipyflow-core-0.0.99/ipyflow/data_model/
+-rw-r--r--   0 smacke     (501) staff       (20)       24 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/data_model/__init__.py
+-rw-r--r--   0 smacke     (501) staff       (20)     4088 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/data_model/annotation_utils.py
+-rw-r--r--   0 smacke     (501) staff       (20)    16815 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/data_model/code_cell.py
+-rw-r--r--   0 smacke     (501) staff       (20)    36058 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/data_model/data_symbol.py
+-rw-r--r--   0 smacke     (501) staff       (20)    12768 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/data_model/namespace.py
+-rw-r--r--   0 smacke     (501) staff       (20)    12844 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/data_model/scope.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1371 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/data_model/sizing.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1891 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/data_model/timestamp.py
+-rw-r--r--   0 smacke     (501) staff       (20)     8196 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/data_model/update_protocol.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:50:00.161458 ipyflow-core-0.0.99/ipyflow/experimental/
+-rw-r--r--   0 smacke     (501) staff       (20)       24 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/experimental/__init__.py
+-rw-r--r--   0 smacke     (501) staff       (20)     3388 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/experimental/dag.py
+-rw-r--r--   0 smacke     (501) staff       (20)    17202 2022-06-06 21:20:47.000000 ipyflow-core-0.0.99/ipyflow/flow.py
+-rw-r--r--   0 smacke     (501) staff       (20)    16983 2022-06-06 21:18:10.000000 ipyflow-core-0.0.99/ipyflow/frontend.py
+-rw-r--r--   0 smacke     (501) staff       (20)      177 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/install.py
+-rw-r--r--   0 smacke     (501) staff       (20)     4947 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/ipython_utils.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:50:00.163357 ipyflow-core-0.0.99/ipyflow/kernel/
+-rw-r--r--   0 smacke     (501) staff       (20)       59 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/kernel/__init__.py
+-rw-r--r--   0 smacke     (501) staff       (20)      467 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/kernel/__main__.py
+-rw-r--r--   0 smacke     (501) staff       (20)     2536 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/kernel/install.py
+-rw-r--r--   0 smacke     (501) staff       (20)    18145 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/kernel/kernel.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1344 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/kernel/patched_nest_asyncio.py
+-rw-r--r--   0 smacke     (501) staff       (20)    14963 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/line_magics.py
+-rw-r--r--   0 smacke     (501) staff       (20)      705 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/run_mode.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1139 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/singletons.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:50:00.166617 ipyflow-core-0.0.99/ipyflow/tracing/
+-rw-r--r--   0 smacke     (501) staff       (20)       24 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/tracing/__init__.py
+-rw-r--r--   0 smacke     (501) staff       (20)      712 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/tracing/flow_ast_rewriter.py
+-rw-r--r--   0 smacke     (501) staff       (20)    57696 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/tracing/ipyflow_tracer.py
+-rw-r--r--   0 smacke     (501) staff       (20)     2341 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/tracing/mutation_event.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1130 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/tracing/mutation_special_cases.py
+-rw-r--r--   0 smacke     (501) staff       (20)    10110 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/tracing/symbol_resolver.py
+-rw-r--r--   0 smacke     (501) staff       (20)    20598 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/tracing/trace_stmt.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1319 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/tracing/utils.py
+-rw-r--r--   0 smacke     (501) staff       (20)      251 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/types.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:50:00.168054 ipyflow-core-0.0.99/ipyflow/utils/
+-rw-r--r--   0 smacke     (501) staff       (20)       96 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/utils/__init__.py
+-rw-r--r--   0 smacke     (501) staff       (20)       84 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/utils/ast_utils.py
+-rw-r--r--   0 smacke     (501) staff       (20)      140 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/utils/misc_utils.py
+-rw-r--r--   0 smacke     (501) staff       (20)      169 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/utils/mixins.py
+-rw-r--r--   0 smacke     (501) staff       (20)      520 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/ipyflow/version.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:50:00.170159 ipyflow-core-0.0.99/ipyflow_core.egg-info/
+-rw-r--r--   0 smacke     (501) staff       (20)      895 2022-06-06 21:49:59.000000 ipyflow-core-0.0.99/ipyflow_core.egg-info/PKG-INFO
+-rw-r--r--   0 smacke     (501) staff       (20)     2210 2022-06-06 21:50:00.000000 ipyflow-core-0.0.99/ipyflow_core.egg-info/SOURCES.txt
+-rw-r--r--   0 smacke     (501) staff       (20)        1 2022-06-06 21:49:59.000000 ipyflow-core-0.0.99/ipyflow_core.egg-info/dependency_links.txt
+-rw-r--r--   0 smacke     (501) staff       (20)        1 2022-06-06 21:49:58.000000 ipyflow-core-0.0.99/ipyflow_core.egg-info/not-zip-safe
+-rw-r--r--   0 smacke     (501) staff       (20)      362 2022-06-06 21:50:00.000000 ipyflow-core-0.0.99/ipyflow_core.egg-info/requires.txt
+-rw-r--r--   0 smacke     (501) staff       (20)        8 2022-06-06 21:50:00.000000 ipyflow-core-0.0.99/ipyflow_core.egg-info/top_level.txt
+-rw-r--r--   0 smacke     (501) staff       (20)      866 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/pyproject.toml
+-rw-r--r--   0 smacke     (501) staff       (20)     1661 2022-06-06 21:50:00.178942 ipyflow-core-0.0.99/setup.cfg
+-rw-r--r--   0 smacke     (501) staff       (20)      116 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/setup.py
+drwxr-xr-x   0 smacke     (501) staff       (20)        0 2022-06-06 21:50:00.177593 ipyflow-core-0.0.99/test/
+-rw-r--r--   0 smacke     (501) staff       (20)     2634 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_annotations.py
+-rw-r--r--   0 smacke     (501) staff       (20)      775 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_api.py
+-rw-r--r--   0 smacke     (501) staff       (20)      810 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_ast_rewriting.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1409 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_attribute_symbols.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1252 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_cell_dag.py
+-rw-r--r--   0 smacke     (501) staff       (20)    15505 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_dynamic_slicing.py
+-rw-r--r--   0 smacke     (501) staff       (20)    16119 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_frontend_checker.py
+-rw-r--r--   0 smacke     (501) staff       (20)     6828 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_line_magics.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1996 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_lineno_stmt_map.py
+-rw-r--r--   0 smacke     (501) staff       (20)     2470 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_liveness_analysis.py
+-rw-r--r--   0 smacke     (501) staff       (20)     7739 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_nested_symbols.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1342 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_no_prints.py
+-rw-r--r--   0 smacke     (501) staff       (20)     3281 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_reactive_atom_detection.py
+-rw-r--r--   0 smacke     (501) staff       (20)    13575 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_reactivity.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1060 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_refcount.py
+-rw-r--r--   0 smacke     (501) staff       (20)     4481 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_stability.py
+-rw-r--r--   0 smacke     (501) staff       (20)    65188 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_staleness_propagation.py
+-rw-r--r--   0 smacke     (501) staff       (20)    24411 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_trace_events.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1454 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_typechecking.py
+-rw-r--r--   0 smacke     (501) staff       (20)     1408 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/test/test_updated_symbols.py
+-rw-r--r--   0 smacke     (501) staff       (20)    81180 2022-06-06 21:07:30.000000 ipyflow-core-0.0.99/versioneer.py
```

### Comparing `ipyflow-core-0.0.98/LICENSE.txt` & `ipyflow-core-0.0.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/PKG-INFO` & `ipyflow-core-0.0.99/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyflow-core
-Version: 0.0.98
+Version: 0.0.99
 Summary: Backend package for ipyflow's dataflow functionality
 Home-page: https://github.com/smacke/nbsafety-project/nbsafety
 Author: Stephen Macke
 Author-email: stephen.macke@gmail.com
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ipyflow-core-0.0.98/ipyflow/__init__.py` & `ipyflow-core-0.0.99/ipyflow/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/_version.py` & `ipyflow-core-0.0.99/ipyflow/_version.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/analysis/live_refs.py` & `ipyflow-core-0.0.99/ipyflow/analysis/live_refs.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/analysis/mixins.py` & `ipyflow-core-0.0.99/ipyflow/analysis/mixins.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/analysis/resolved_symbols.py` & `ipyflow-core-0.0.99/ipyflow/analysis/resolved_symbols.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/analysis/slicing.py` & `ipyflow-core-0.0.99/ipyflow/analysis/slicing.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/analysis/symbol_edges.py` & `ipyflow-core-0.0.99/ipyflow/analysis/symbol_edges.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/analysis/symbol_ref.py` & `ipyflow-core-0.0.99/ipyflow/analysis/symbol_ref.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/analysis/utils.py` & `ipyflow-core-0.0.99/ipyflow/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/api/lift.py` & `ipyflow-core-0.0.99/ipyflow/api/lift.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/data_model/annotation_utils.py` & `ipyflow-core-0.0.99/ipyflow/data_model/annotation_utils.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/data_model/code_cell.py` & `ipyflow-core-0.0.99/ipyflow/data_model/code_cell.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/data_model/data_symbol.py` & `ipyflow-core-0.0.99/ipyflow/data_model/data_symbol.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/data_model/namespace.py` & `ipyflow-core-0.0.99/ipyflow/data_model/namespace.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/data_model/scope.py` & `ipyflow-core-0.0.99/ipyflow/data_model/scope.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/data_model/sizing.py` & `ipyflow-core-0.0.99/ipyflow/data_model/sizing.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/data_model/timestamp.py` & `ipyflow-core-0.0.99/ipyflow/data_model/timestamp.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/data_model/update_protocol.py` & `ipyflow-core-0.0.99/ipyflow/data_model/update_protocol.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/experimental/dag.py` & `ipyflow-core-0.0.99/ipyflow/experimental/dag.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/flow.py` & `ipyflow-core-0.0.99/ipyflow/flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,21 @@
         if handler is None:
             dbg_msg = "Unsupported request type for request %s" % request
             logger.error(dbg_msg)
             self._saved_debug_message = dbg_msg
             return
         response = handler(request)
         if response is not None and comm is not None:
-            comm.send(response)
+            try:
+                comm.send(response)
+            except TypeError as e:
+                raise Exception(
+                    "unable to serialize response for request of type %s"
+                    % request["type"]
+                ) from e
 
     def handle_change_active_cell(self, request) -> Optional[Dict[str, Any]]:
         self.set_active_cell(request["active_cell_id"])
         return None
 
     def handle_compute_exec_schedule(self, request) -> Optional[Dict[str, Any]]:
         if self._active_cell_id is None:
```

### Comparing `ipyflow-core-0.0.98/ipyflow/frontend.py` & `ipyflow-core-0.0.99/ipyflow/frontend.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             # TODO: we should probably have separate fields for waiting vs non-typechecking cells,
             #  or at least change the name to a more general "unsafe_cells" or equivalent
             "waiting_cells": list(self.waiting_cells | self.typecheck_error_cells),
             "ready_cells": list(self.ready_cells),
             "new_ready_cells": list(self.new_ready_cells),
             "forced_reactive_cells": list(self.forced_reactive_cells),
             "unsafe_order_cells": {
-                cell_id: list(unsafe_order_cells)
+                cell_id: [unsafe.cell_id for unsafe in unsafe_order_cells]
                 for cell_id, unsafe_order_cells in self.unsafe_order_cells.items()
             },
             "unsafe_order_symbol_usage": self.unsafe_order_symbol_usage,
             "waiter_links": {
                 cell_id: list(linked_cell_ids)
                 for cell_id, linked_cell_ids in self.waiter_links.items()
             },
```

### Comparing `ipyflow-core-0.0.98/ipyflow/ipython_utils.py` & `ipyflow-core-0.0.99/ipyflow/ipython_utils.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/kernel/install.py` & `ipyflow-core-0.0.99/ipyflow/kernel/install.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/kernel/kernel.py` & `ipyflow-core-0.0.99/ipyflow/kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/kernel/patched_nest_asyncio.py` & `ipyflow-core-0.0.99/ipyflow/kernel/patched_nest_asyncio.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/line_magics.py` & `ipyflow-core-0.0.99/ipyflow/line_magics.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/run_mode.py` & `ipyflow-core-0.0.99/ipyflow/run_mode.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/singletons.py` & `ipyflow-core-0.0.99/ipyflow/singletons.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/tracing/flow_ast_rewriter.py` & `ipyflow-core-0.0.99/ipyflow/tracing/flow_ast_rewriter.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/tracing/ipyflow_tracer.py` & `ipyflow-core-0.0.99/ipyflow/tracing/ipyflow_tracer.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/tracing/mutation_event.py` & `ipyflow-core-0.0.99/ipyflow/tracing/mutation_event.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/tracing/mutation_special_cases.py` & `ipyflow-core-0.0.99/ipyflow/tracing/mutation_special_cases.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/tracing/symbol_resolver.py` & `ipyflow-core-0.0.99/ipyflow/tracing/symbol_resolver.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/tracing/trace_stmt.py` & `ipyflow-core-0.0.99/ipyflow/tracing/trace_stmt.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/tracing/utils.py` & `ipyflow-core-0.0.99/ipyflow/tracing/utils.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow/version.py` & `ipyflow-core-0.0.99/ipyflow/version.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/ipyflow_core.egg-info/PKG-INFO` & `ipyflow-core-0.0.99/ipyflow_core.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyflow-core
-Version: 0.0.98
+Version: 0.0.99
 Summary: Backend package for ipyflow's dataflow functionality
 Home-page: https://github.com/smacke/nbsafety-project/nbsafety
 Author: Stephen Macke
 Author-email: stephen.macke@gmail.com
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ipyflow-core-0.0.98/ipyflow_core.egg-info/SOURCES.txt` & `ipyflow-core-0.0.99/ipyflow_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/pyproject.toml` & `ipyflow-core-0.0.99/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/setup.cfg` & `ipyflow-core-0.0.99/setup.cfg`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_annotations.py` & `ipyflow-core-0.0.99/test/test_annotations.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_api.py` & `ipyflow-core-0.0.99/test/test_api.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_ast_rewriting.py` & `ipyflow-core-0.0.99/test/test_ast_rewriting.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_attribute_symbols.py` & `ipyflow-core-0.0.99/test/test_attribute_symbols.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_cell_dag.py` & `ipyflow-core-0.0.99/test/test_cell_dag.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_dynamic_slicing.py` & `ipyflow-core-0.0.99/test/test_dynamic_slicing.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_frontend_checker.py` & `ipyflow-core-0.0.99/test/test_frontend_checker.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_line_magics.py` & `ipyflow-core-0.0.99/test/test_line_magics.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_lineno_stmt_map.py` & `ipyflow-core-0.0.99/test/test_lineno_stmt_map.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_liveness_analysis.py` & `ipyflow-core-0.0.99/test/test_liveness_analysis.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_nested_symbols.py` & `ipyflow-core-0.0.99/test/test_nested_symbols.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_no_prints.py` & `ipyflow-core-0.0.99/test/test_no_prints.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_reactive_atom_detection.py` & `ipyflow-core-0.0.99/test/test_reactive_atom_detection.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_reactivity.py` & `ipyflow-core-0.0.99/test/test_reactivity.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_refcount.py` & `ipyflow-core-0.0.99/test/test_refcount.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_stability.py` & `ipyflow-core-0.0.99/test/test_stability.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_staleness_propagation.py` & `ipyflow-core-0.0.99/test/test_staleness_propagation.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_trace_events.py` & `ipyflow-core-0.0.99/test/test_trace_events.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_typechecking.py` & `ipyflow-core-0.0.99/test/test_typechecking.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/test/test_updated_symbols.py` & `ipyflow-core-0.0.99/test/test_updated_symbols.py`

 * *Files identical despite different names*

### Comparing `ipyflow-core-0.0.98/versioneer.py` & `ipyflow-core-0.0.99/versioneer.py`

 * *Files identical despite different names*


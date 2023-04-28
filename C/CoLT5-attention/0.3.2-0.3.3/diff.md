# Comparing `tmp/CoLT5-attention-0.3.2.tar.gz` & `tmp/CoLT5-attention-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.3.2.tar", last modified: Fri Apr 28 23:24:04 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.3.3.tar", last modified: Fri Apr 28 23:30:18 2023, max compression
```

## Comparing `CoLT5-attention-0.3.2.tar` & `CoLT5-attention-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:24:04.324190 CoLT5-attention-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:24:04.320190 CoLT5-attention-0.3.2/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 23:24:04.000000 CoLT5-attention-0.3.2/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-28 23:24:04.000000 CoLT5-attention-0.3.2/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:24:04.000000 CoLT5-attention-0.3.2/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 23:24:04.000000 CoLT5-attention-0.3.2/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 23:24:04.000000 CoLT5-attention-0.3.2/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-28 23:23:48.000000 CoLT5-attention-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 23:24:04.324190 CoLT5-attention-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-04-28 23:23:48.000000 CoLT5-attention-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:24:04.324190 CoLT5-attention-0.3.2/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 23:23:48.000000 CoLT5-attention-0.3.2/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-28 23:23:48.000000 CoLT5-attention-0.3.2/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-28 23:23:48.000000 CoLT5-attention-0.3.2/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31723 2023-04-28 23:23:48.000000 CoLT5-attention-0.3.2/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:24:04.324190 CoLT5-attention-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-28 23:23:48.000000 CoLT5-attention-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:30:18.936483 CoLT5-attention-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:30:18.936483 CoLT5-attention-0.3.3/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 23:30:18.000000 CoLT5-attention-0.3.3/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-28 23:30:18.000000 CoLT5-attention-0.3.3/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:30:18.000000 CoLT5-attention-0.3.3/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 23:30:18.000000 CoLT5-attention-0.3.3/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 23:30:18.000000 CoLT5-attention-0.3.3/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-28 23:30:05.000000 CoLT5-attention-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 23:30:18.936483 CoLT5-attention-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-04-28 23:30:05.000000 CoLT5-attention-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:30:18.936483 CoLT5-attention-0.3.3/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 23:30:05.000000 CoLT5-attention-0.3.3/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-28 23:30:05.000000 CoLT5-attention-0.3.3/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-28 23:30:05.000000 CoLT5-attention-0.3.3/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31818 2023-04-28 23:30:05.000000 CoLT5-attention-0.3.3/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:30:18.936483 CoLT5-attention-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-28 23:30:05.000000 CoLT5-attention-0.3.3/setup.py
```

### Comparing `CoLT5-attention-0.3.2/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.3.3/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.3.2
+Version: 0.3.3
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.3.2/LICENSE` & `CoLT5-attention-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.2/PKG-INFO` & `CoLT5-attention-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.3.2
+Version: 0.3.3
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.3.2/README.md` & `CoLT5-attention-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.2/colt5_attention/coor_descent.py` & `CoLT5-attention-0.3.3/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.2/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.3.3/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.2/colt5_attention/transformer_block.py` & `CoLT5-attention-0.3.3/colt5_attention/transformer_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -894,19 +894,20 @@
         normalized_scores_kv = None
 
         should_route_kv = key_value_length > num_tokens_kv
 
         if should_route_kv:
             normalized_scores_kv, indices_kv = self.kv_router(context, num_tokens = num_tokens_kv, mask = context_mask)
 
-            routed_tokens_kv = x[batch_range, indices_kv]
+            kv_batch_range = create_batch_range(x, right_pad_dims = indices_kv.ndim - 1)
+            routed_tokens_kv = x[kv_batch_range, indices_kv]
 
             routed_tokens_kv_mask = None
             if exists(context_mask):
-                routed_tokens_kv_mask = context_mask[batch_range, indices_kv]
+                routed_tokens_kv_mask = context_mask[kv_batch_range, indices_kv]
 
         # do the heavier branch with only routed tokens
 
         routed_tokens_out = self.heavy_attn(
             routed_tokens_q,
             mask = routed_tokens_kv_mask,
             context = routed_tokens_kv,
```

### Comparing `CoLT5-attention-0.3.2/setup.py` & `CoLT5-attention-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.3.2',
+  version = '0.3.3',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```


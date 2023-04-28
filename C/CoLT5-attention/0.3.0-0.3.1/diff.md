# Comparing `tmp/CoLT5-attention-0.3.0.tar.gz` & `tmp/CoLT5-attention-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.3.0.tar", last modified: Fri Apr 28 22:48:00 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.3.1.tar", last modified: Fri Apr 28 22:50:20 2023, max compression
```

## Comparing `CoLT5-attention-0.3.0.tar` & `CoLT5-attention-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:48:00.439718 CoLT5-attention-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:48:00.435718 CoLT5-attention-0.3.0/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 22:48:00.000000 CoLT5-attention-0.3.0/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-28 22:48:00.000000 CoLT5-attention-0.3.0/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:48:00.000000 CoLT5-attention-0.3.0/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 22:48:00.000000 CoLT5-attention-0.3.0/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 22:48:00.000000 CoLT5-attention-0.3.0/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-28 22:47:47.000000 CoLT5-attention-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 22:48:00.439718 CoLT5-attention-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-28 22:47:47.000000 CoLT5-attention-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:48:00.439718 CoLT5-attention-0.3.0/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 22:47:47.000000 CoLT5-attention-0.3.0/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-28 22:47:47.000000 CoLT5-attention-0.3.0/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-28 22:47:47.000000 CoLT5-attention-0.3.0/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31431 2023-04-28 22:47:47.000000 CoLT5-attention-0.3.0/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:48:00.439718 CoLT5-attention-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-28 22:47:47.000000 CoLT5-attention-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:20.752855 CoLT5-attention-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:20.752855 CoLT5-attention-0.3.1/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 22:50:20.000000 CoLT5-attention-0.3.1/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-28 22:50:20.000000 CoLT5-attention-0.3.1/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:50:20.000000 CoLT5-attention-0.3.1/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 22:50:20.000000 CoLT5-attention-0.3.1/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 22:50:20.000000 CoLT5-attention-0.3.1/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-28 22:50:07.000000 CoLT5-attention-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 22:50:20.752855 CoLT5-attention-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-28 22:50:07.000000 CoLT5-attention-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:20.752855 CoLT5-attention-0.3.1/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 22:50:07.000000 CoLT5-attention-0.3.1/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-28 22:50:07.000000 CoLT5-attention-0.3.1/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-28 22:50:07.000000 CoLT5-attention-0.3.1/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31530 2023-04-28 22:50:07.000000 CoLT5-attention-0.3.1/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:50:20.752855 CoLT5-attention-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-28 22:50:07.000000 CoLT5-attention-0.3.1/setup.py
```

### Comparing `CoLT5-attention-0.3.0/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.3.1/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.3.0
+Version: 0.3.1
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.3.0/LICENSE` & `CoLT5-attention-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.0/PKG-INFO` & `CoLT5-attention-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.3.0
+Version: 0.3.1
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.3.0/README.md` & `CoLT5-attention-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.0/colt5_attention/coor_descent.py` & `CoLT5-attention-0.3.1/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.0/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.3.1/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.0/colt5_attention/transformer_block.py` & `CoLT5-attention-0.3.1/colt5_attention/transformer_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -783,20 +783,23 @@
             routed_tokens_q,
             mask = routed_tokens_kv_mask,
             context = routed_tokens_kv,
             normalized_scores_kv = normalized_scores_kv,
             normalized_scores_q = normalized_scores_q if self.multiply_queries_by_score else None
         )
 
-        routed_tokens_out = routed_tokens_out * rearrange(normalized_scores_q, '... -> ... 1')
+        if should_route_q:
+            routed_tokens_out = routed_tokens_out * rearrange(normalized_scores_q, '... -> ... 1')
 
-        # scatter back the output of the heavy branch
+            # scatter back the output of the heavy branch
 
-        heavy_out = torch.zeros_like(q)
-        heavy_out = self.q_router.route_back(heavy_out, routed_tokens_out, indices_q)
+            heavy_out = torch.zeros_like(q)
+            heavy_out = self.q_router.route_back(heavy_out, routed_tokens_out, indices_q)
+        else:
+            heavy_out = routed_tokens_out
 
         # un-window and slice out original sequence
 
         heavy_out = rearrange(heavy_out, '(b n) w d -> b (n w) d', b = batch)
         heavy_out = heavy_out[:, :seq_len]
 
         # sum light and heavy branches
```

### Comparing `CoLT5-attention-0.3.0/setup.py` & `CoLT5-attention-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.3.0',
+  version = '0.3.1',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```


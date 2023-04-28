# Comparing `tmp/CoLT5-attention-0.3.1.tar.gz` & `tmp/CoLT5-attention-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.3.1.tar", last modified: Fri Apr 28 22:50:20 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.3.2.tar", last modified: Fri Apr 28 23:24:04 2023, max compression
```

## Comparing `CoLT5-attention-0.3.1.tar` & `CoLT5-attention-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:20.752855 CoLT5-attention-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:20.752855 CoLT5-attention-0.3.1/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 22:50:20.000000 CoLT5-attention-0.3.1/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-28 22:50:20.000000 CoLT5-attention-0.3.1/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:50:20.000000 CoLT5-attention-0.3.1/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 22:50:20.000000 CoLT5-attention-0.3.1/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 22:50:20.000000 CoLT5-attention-0.3.1/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-28 22:50:07.000000 CoLT5-attention-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 22:50:20.752855 CoLT5-attention-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-28 22:50:07.000000 CoLT5-attention-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:20.752855 CoLT5-attention-0.3.1/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 22:50:07.000000 CoLT5-attention-0.3.1/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-28 22:50:07.000000 CoLT5-attention-0.3.1/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-28 22:50:07.000000 CoLT5-attention-0.3.1/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31530 2023-04-28 22:50:07.000000 CoLT5-attention-0.3.1/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:50:20.752855 CoLT5-attention-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-28 22:50:07.000000 CoLT5-attention-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:24:04.324190 CoLT5-attention-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:24:04.320190 CoLT5-attention-0.3.2/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 23:24:04.000000 CoLT5-attention-0.3.2/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-28 23:24:04.000000 CoLT5-attention-0.3.2/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:24:04.000000 CoLT5-attention-0.3.2/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 23:24:04.000000 CoLT5-attention-0.3.2/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 23:24:04.000000 CoLT5-attention-0.3.2/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-28 23:23:48.000000 CoLT5-attention-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 23:24:04.324190 CoLT5-attention-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-04-28 23:23:48.000000 CoLT5-attention-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:24:04.324190 CoLT5-attention-0.3.2/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 23:23:48.000000 CoLT5-attention-0.3.2/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-28 23:23:48.000000 CoLT5-attention-0.3.2/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-28 23:23:48.000000 CoLT5-attention-0.3.2/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31723 2023-04-28 23:23:48.000000 CoLT5-attention-0.3.2/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:24:04.324190 CoLT5-attention-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-28 23:23:48.000000 CoLT5-attention-0.3.2/setup.py
```

### Comparing `CoLT5-attention-0.3.1/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.3.2/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.3.1
+Version: 0.3.2
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.3.1/LICENSE` & `CoLT5-attention-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.1/PKG-INFO` & `CoLT5-attention-0.3.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.3.1
+Version: 0.3.2
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.3.1/README.md` & `CoLT5-attention-0.3.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -118,17 +118,18 @@
 
 cross_attn_out.shape # (2, 1024, 512) - same as tokens
 ```
 
 ## Todo
 
 - [x] add the coordinate descent method as another router
-- [x] figure out if it can be done autoregressively and try it out - moving to <a href="https://github.com/lucidrains/coordinate-descent-attention">this repo</a>
 - [x] allow for multi-headed routing (multiple routing tokens), only for key-values
+- [x] add an autoregressive version of the conditionally routed attention
 
+- [ ] test out the autoregressive version and verify that more routed key / value tokens lead to better results
 - [ ] for variable sequence lengths, allow for setting k as a function of sequence lengths per sample in batch
 - [ ] create a variant of CoLT5 for high resolution feature maps (image attention) - then try out for diffusion
 - [ ] in the cross attention scenario, support for routing token that first queries the source tokens, before retrieving from memories
 - [ ] make flash attention compatible
 - [ ] work out a triton forward / backward version of coordinate descent (coor_descent), as it seems torch compile does not work well enough for coor_descent function just yet
 
 ## Citations
```

#### html2text {}

```diff
@@ -45,22 +45,23 @@
 num_tokens_q = 512, # only 512 routed from 1024 num_tokens_kv = 1024, # only
 1024 routed from 1 million kv_routing_tokens = 2, # say you want 2 routing
 tokens to route different sets of key / values to the queries. 4 attention
 heads will be allocated to each routed set in this example (8 / 2) ).cuda()
 cross_attn_out = cross_attn( tokens, context = memories, mask = tokens_mask,
 context_mask = memories_mask ) cross_attn_out.shape # (2, 1024, 512) - same as
 tokens ``` ## Todo - [x] add the coordinate descent method as another router -
-[x] figure out if it can be done autoregressively and try it out - moving to
-this_repo - [x] allow for multi-headed routing (multiple routing tokens), only
-for key-values - [ ] for variable sequence lengths, allow for setting k as a
-function of sequence lengths per sample in batch - [ ] create a variant of
-CoLT5 for high resolution feature maps (image attention) - then try out for
-diffusion - [ ] in the cross attention scenario, support for routing token that
-first queries the source tokens, before retrieving from memories - [ ] make
-flash attention compatible - [ ] work out a triton forward / backward version
-of coordinate descent (coor_descent), as it seems torch compile does not work
-well enough for coor_descent function just yet ## Citations ```bibtex
-@inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range
-Transformers with Conditional Computation}, author = {Joshua Ainslie and Tao
-Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury
-Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and
-Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ```
+[x] allow for multi-headed routing (multiple routing tokens), only for key-
+values - [x] add an autoregressive version of the conditionally routed
+attention - [ ] test out the autoregressive version and verify that more routed
+key / value tokens lead to better results - [ ] for variable sequence lengths,
+allow for setting k as a function of sequence lengths per sample in batch - [ ]
+create a variant of CoLT5 for high resolution feature maps (image attention) -
+then try out for diffusion - [ ] in the cross attention scenario, support for
+routing token that first queries the source tokens, before retrieving from
+memories - [ ] make flash attention compatible - [ ] work out a triton forward
+/ backward version of coordinate descent (coor_descent), as it seems torch
+compile does not work well enough for coor_descent function just yet ##
+Citations ```bibtex @inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster
+Long-Range Transformers with Conditional Computation}, author = {Joshua Ainslie
+and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and
+Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay
+and Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ```
```

### Comparing `CoLT5-attention-0.3.1/colt5_attention/coor_descent.py` & `CoLT5-attention-0.3.2/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.1/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.3.2/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.1/colt5_attention/transformer_block.py` & `CoLT5-attention-0.3.2/colt5_attention/transformer_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,18 +34,19 @@
     remainder = math.ceil(m) * multiple - seq_len
     pad_offset = (0,) * (-1 - dim) * 2
     padded_tensor = F.pad(tensor, (*pad_offset, 0, remainder), value = value)
     return padded_tensor, seq_len
 
 # tensor helpers
 
-def create_batch_range(t):
+def create_batch_range(t, right_pad_dims = 1):
     b, device = t.shape[0], t.device
     batch_range = torch.arange(b, device = device)
-    return rearrange(batch_range, 'b -> b 1')
+    pad_dims = ((1,) * right_pad_dims)
+    return batch_range.reshape(-1, *pad_dims)
 
 # normalization
 
 class RMSNorm(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.scale = dim ** 0.5
@@ -594,35 +595,37 @@
         mask = None
     ):
         batch, device = x.shape[0], x.device
 
         num_heavy_tokens_q = default(num_heavy_tokens_q, self.num_heavy_tokens_q)
         num_heavy_tokens_kv = default(num_heavy_tokens_kv, self.num_heavy_tokens_kv)
 
-        batch_range = create_batch_range(x)
 
         # light local attention sees all tokens in a limited context
 
         light_out = self.light_attn(x, mask = mask)
 
         # route tokens appropriately for heavy branch
 
         normalized_scores_q, indices_q = self.q_router(x, num_tokens = num_heavy_tokens_q, mask = mask)
         normalized_scores_kv, indices_kv = self.kv_router(x, num_tokens = num_heavy_tokens_kv, mask = mask)
 
         # select the tokens to be routed to full attention
 
-        routed_tokens_q = x[batch_range, indices_q]
-        routed_tokens_kv = x[batch_range, indices_kv]
+        q_batch_range = create_batch_range(x)
+        routed_tokens_q = x[q_batch_range, indices_q]
+
+        kv_batch_range = create_batch_range(x, right_pad_dims = indices_kv.ndim - 1)
+        routed_tokens_kv = x[kv_batch_range, indices_kv]
 
         # calculate key padding mask
 
         routed_tokens_kv_mask = None
         if exists(mask):
-            routed_tokens_kv_mask = mask[batch_range, indices_kv]
+            routed_tokens_kv_mask = mask[kv_batch_range, indices_kv]
 
         # do the heavier branch with only routed tokens
 
         routed_tokens_out = self.heavy_attn(
             routed_tokens_q,
             mask = routed_tokens_kv_mask,
             context = routed_tokens_kv,
@@ -764,15 +767,15 @@
         else:
             normalized_scores_q = 1.
             routed_tokens_q = q
 
         if should_route_kv:
             normalized_scores_kv, indices_kv = self.kv_router(kv, num_tokens = num_heavy_tokens_kv, mask = kv_mask)
 
-            kv_batch_range = create_batch_range(kv)
+            kv_batch_range = create_batch_range(kv, right_pad_dims = indices_kv.ndim - 1)
 
             routed_tokens_kv = kv[kv_batch_range, indices_kv]
             routed_tokens_kv_mask = kv_mask[kv_batch_range, indices_kv]
         else:
             normalized_scores_kv = 1.
             routed_tokens_kv = kv
             routed_tokens_kv_mask = kv_mask
```

### Comparing `CoLT5-attention-0.3.1/setup.py` & `CoLT5-attention-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.3.1',
+  version = '0.3.2',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```


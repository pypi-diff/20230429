# Comparing `tmp/gptq_triton-0.0.3.tar.gz` & `tmp/gptq_triton-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptq_triton-0.0.3.tar", last modified: Thu Apr 20 03:24:13 2023, max compression
+gzip compressed data, was "gptq_triton-0.0.4.tar", last modified: Sat Apr 29 16:08:06 2023, max compression
```

## Comparing `gptq_triton-0.0.3.tar` & `gptq_triton-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 night     (1000) night     (1000)        0 2023-04-20 03:24:13.591881 gptq_triton-0.0.3/
--rw-rw-r--   0 night     (1000) night     (1000)    11357 2023-03-27 23:24:52.000000 gptq_triton-0.0.3/LICENSE
--rw-rw-r--   0 night     (1000) night     (1000)     8518 2023-04-20 03:24:13.591881 gptq_triton-0.0.3/PKG-INFO
--rw-rw-r--   0 night     (1000) night     (1000)     7471 2023-04-18 23:16:22.000000 gptq_triton-0.0.3/README.md
--rw-rw-r--   0 night     (1000) night     (1000)      100 2023-04-14 00:43:30.000000 gptq_triton-0.0.3/pyproject.toml
--rw-rw-r--   0 night     (1000) night     (1000)     1226 2023-04-20 03:24:13.591881 gptq_triton-0.0.3/setup.cfg
--rw-rw-r--   0 night     (1000) night     (1000)       87 2023-04-14 00:46:34.000000 gptq_triton-0.0.3/setup.py
-drwxrwxr-x   0 night     (1000) night     (1000)        0 2023-04-20 03:24:13.587881 gptq_triton-0.0.3/src/
-drwxrwxr-x   0 night     (1000) night     (1000)        0 2023-04-20 03:24:13.587881 gptq_triton-0.0.3/src/gptq_triton/
--rw-rw-r--   0 night     (1000) night     (1000)     4086 2023-04-19 07:53:33.000000 gptq_triton-0.0.3/src/gptq_triton/__init__.py
--rw-rw-r--   0 night     (1000) night     (1000)     7046 2023-04-17 19:30:37.000000 gptq_triton-0.0.3/src/gptq_triton/custom_autotune.py
--rw-rw-r--   0 night     (1000) night     (1000)     5134 2023-04-19 00:26:19.000000 gptq_triton-0.0.3/src/gptq_triton/fused_attention.py
--rw-rw-r--   0 night     (1000) night     (1000)    12834 2023-04-18 23:21:21.000000 gptq_triton-0.0.3/src/gptq_triton/fused_mlp.py
--rw-rw-r--   0 night     (1000) night     (1000)    12617 2023-04-19 18:15:29.000000 gptq_triton-0.0.3/src/gptq_triton/quant_linear.py
--rw-rw-r--   0 night     (1000) night     (1000)     1046 2023-04-10 02:28:16.000000 gptq_triton-0.0.3/src/gptq_triton/utils.py
-drwxrwxr-x   0 night     (1000) night     (1000)        0 2023-04-20 03:24:13.591881 gptq_triton-0.0.3/src/gptq_triton.egg-info/
--rw-rw-r--   0 night     (1000) night     (1000)     8518 2023-04-20 03:24:13.000000 gptq_triton-0.0.3/src/gptq_triton.egg-info/PKG-INFO
--rw-rw-r--   0 night     (1000) night     (1000)      467 2023-04-20 03:24:13.000000 gptq_triton-0.0.3/src/gptq_triton.egg-info/SOURCES.txt
--rw-rw-r--   0 night     (1000) night     (1000)        1 2023-04-20 03:24:13.000000 gptq_triton-0.0.3/src/gptq_triton.egg-info/dependency_links.txt
--rw-rw-r--   0 night     (1000) night     (1000)        1 2023-04-14 00:46:41.000000 gptq_triton-0.0.3/src/gptq_triton.egg-info/not-zip-safe
--rw-rw-r--   0 night     (1000) night     (1000)       40 2023-04-20 03:24:13.000000 gptq_triton-0.0.3/src/gptq_triton.egg-info/requires.txt
--rw-rw-r--   0 night     (1000) night     (1000)       12 2023-04-20 03:24:13.000000 gptq_triton-0.0.3/src/gptq_triton.egg-info/top_level.txt
+drwxrwxr-x   0 night     (1000) night     (1000)        0 2023-04-29 16:08:06.066935 gptq_triton-0.0.4/
+-rw-rw-r--   0 night     (1000) night     (1000)    11357 2023-03-27 23:24:52.000000 gptq_triton-0.0.4/LICENSE
+-rw-rw-r--   0 night     (1000) night     (1000)     9010 2023-04-29 16:08:06.066935 gptq_triton-0.0.4/PKG-INFO
+-rw-rw-r--   0 night     (1000) night     (1000)     7963 2023-04-28 20:29:53.000000 gptq_triton-0.0.4/README.md
+-rw-rw-r--   0 night     (1000) night     (1000)      100 2023-04-14 00:43:30.000000 gptq_triton-0.0.4/pyproject.toml
+-rw-rw-r--   0 night     (1000) night     (1000)     1226 2023-04-29 16:08:06.066935 gptq_triton-0.0.4/setup.cfg
+-rw-rw-r--   0 night     (1000) night     (1000)       87 2023-04-14 00:46:34.000000 gptq_triton-0.0.4/setup.py
+drwxrwxr-x   0 night     (1000) night     (1000)        0 2023-04-29 16:08:06.062935 gptq_triton-0.0.4/src/
+drwxrwxr-x   0 night     (1000) night     (1000)        0 2023-04-29 16:08:06.062935 gptq_triton-0.0.4/src/gptq_triton/
+-rw-rw-r--   0 night     (1000) night     (1000)     4086 2023-04-19 07:53:33.000000 gptq_triton-0.0.4/src/gptq_triton/__init__.py
+-rw-rw-r--   0 night     (1000) night     (1000)     7046 2023-04-17 19:30:37.000000 gptq_triton-0.0.4/src/gptq_triton/custom_autotune.py
+-rw-rw-r--   0 night     (1000) night     (1000)     5495 2023-04-29 16:00:14.000000 gptq_triton-0.0.4/src/gptq_triton/fused_attention.py
+-rw-rw-r--   0 night     (1000) night     (1000)    12834 2023-04-18 23:21:21.000000 gptq_triton-0.0.4/src/gptq_triton/fused_mlp.py
+-rw-rw-r--   0 night     (1000) night     (1000)    12617 2023-04-19 18:15:29.000000 gptq_triton-0.0.4/src/gptq_triton/quant_linear.py
+-rw-rw-r--   0 night     (1000) night     (1000)     1046 2023-04-10 02:28:16.000000 gptq_triton-0.0.4/src/gptq_triton/utils.py
+drwxrwxr-x   0 night     (1000) night     (1000)        0 2023-04-29 16:08:06.066935 gptq_triton-0.0.4/src/gptq_triton.egg-info/
+-rw-rw-r--   0 night     (1000) night     (1000)     9010 2023-04-29 16:08:06.000000 gptq_triton-0.0.4/src/gptq_triton.egg-info/PKG-INFO
+-rw-rw-r--   0 night     (1000) night     (1000)      467 2023-04-29 16:08:06.000000 gptq_triton-0.0.4/src/gptq_triton.egg-info/SOURCES.txt
+-rw-rw-r--   0 night     (1000) night     (1000)        1 2023-04-29 16:08:06.000000 gptq_triton-0.0.4/src/gptq_triton.egg-info/dependency_links.txt
+-rw-rw-r--   0 night     (1000) night     (1000)        1 2023-04-14 00:46:41.000000 gptq_triton-0.0.4/src/gptq_triton.egg-info/not-zip-safe
+-rw-rw-r--   0 night     (1000) night     (1000)       40 2023-04-29 16:08:06.000000 gptq_triton-0.0.4/src/gptq_triton.egg-info/requires.txt
+-rw-rw-r--   0 night     (1000) night     (1000)       12 2023-04-29 16:08:06.000000 gptq_triton-0.0.4/src/gptq_triton.egg-info/top_level.txt
```

### Comparing `gptq_triton-0.0.3/LICENSE` & `gptq_triton-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gptq_triton-0.0.3/PKG-INFO` & `gptq_triton-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptq_triton
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fast GPTQ kernels written in Triton
 Home-page: https://github.com/fpgaminer/GPTQ-triton
 Author: fpgaminer
 Author-email: fpgaminer@bitcoin-mining.com
 License: Apache License 2.0
 Keywords: gptq,triton,torch,cuda,gpu,quantization,quantize,quantized,inference,deep learning,machine learning
 Classifier: Development Status :: 3 - Alpha
@@ -63,26 +63,30 @@
 it/s numbers are from a 3090.
 
 
 | [LLaMA-7B](https://arxiv.org/abs/2302.13971)       | Bits | group-size | memory(MiB) | it/s | Wikitext2 |  PTB  |  C4  | 
 | -------------------------------------------------- | ---- | ---------- | ----------- | ---- | --------- | ----- | ---- |
 | FP16                                               |  16  |      -     |    17373    | 1.64 |    5.04   |  7.85 | 6.99 |
 | GPTQ CUDA                                          |   4  |     -1     |     8805    | 0.11 |    5.44   |  8.24 |   -  |
-| GPTQ Triton                                        |   4  |     -1     |     8099    | 1.63 |    5.44   |  8.24 | 7.48 |
+| GPTQ Triton                                        |   4  |     -1     |     6323    | 1.70 |    5.44   |  8.24 | 7.48 |
 
 
 | [LLaMA-13B](https://arxiv.org/abs/2302.13971)      | Bits | group-size | memory(MiB) | it/s | Wikitext2 |  PTB  |  C4  |
 | -------------------------------------------------- | ---- | ---------- | ----------- | ---- | --------- | ----- | ---- |
 | FP16                                               |  16  |      -     |    31633    |   -  |    4.52   |  7.19 | 6.66 |
-| GPTQ Triton                                        |   4  |     -1     |    13241    | 0.89 |    4.74   |  7.49 | 7.00 |
+| GPTQ Triton                                        |   4  |     -1     |    10325    | 0.95 |    4.74   |  7.49 | 7.00 |
+| GPTQ Triton                                        |   4  |    128     |     9547    | 0.92 |    4.67   |  7.38 | 6.99 |
 
 
 | [LLaMA-30B](https://arxiv.org/abs/2302.13971)      | Bits | group-size | memory(MiB) | it/s | Wikitext2 |  PTB  |  C4  |
 | -------------------------------------------------- | ---- | ---------- | ----------- | ---- | --------- | ----- | ---- |
 | FP16                                               |  16  |      -     |    72491    |   -  |    3.61   |  6.50 | 6.07 |
+| GPTQ Triton                                        |   4  |     -1     |    19989    | 0.40 |    3.89   |  6.71 | 6.44 |
+| GPTQ Triton                                        |   4  |    128     |    20055    | 0.39 |    3.79   |  6.70 | 6.34 |
+| GPTQ Triton                                        |   4  |    512     |    19547    | 0.39 |    3.78   |  6.62 | 6.30 |
 
 
 ## Requirements
 
 See `setup.cfg`, but note that a nightly `transformers` is preferred right now. v4.28.1 might work.  Known working `transformers` commit is `28f26c107b4a1c5c7e32ed4d9575622da0627a40`.
```

### Comparing `gptq_triton-0.0.3/README.md` & `gptq_triton-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -39,26 +39,30 @@
 it/s numbers are from a 3090.
 
 
 | [LLaMA-7B](https://arxiv.org/abs/2302.13971)       | Bits | group-size | memory(MiB) | it/s | Wikitext2 |  PTB  |  C4  | 
 | -------------------------------------------------- | ---- | ---------- | ----------- | ---- | --------- | ----- | ---- |
 | FP16                                               |  16  |      -     |    17373    | 1.64 |    5.04   |  7.85 | 6.99 |
 | GPTQ CUDA                                          |   4  |     -1     |     8805    | 0.11 |    5.44   |  8.24 |   -  |
-| GPTQ Triton                                        |   4  |     -1     |     8099    | 1.63 |    5.44   |  8.24 | 7.48 |
+| GPTQ Triton                                        |   4  |     -1     |     6323    | 1.70 |    5.44   |  8.24 | 7.48 |
 
 
 | [LLaMA-13B](https://arxiv.org/abs/2302.13971)      | Bits | group-size | memory(MiB) | it/s | Wikitext2 |  PTB  |  C4  |
 | -------------------------------------------------- | ---- | ---------- | ----------- | ---- | --------- | ----- | ---- |
 | FP16                                               |  16  |      -     |    31633    |   -  |    4.52   |  7.19 | 6.66 |
-| GPTQ Triton                                        |   4  |     -1     |    13241    | 0.89 |    4.74   |  7.49 | 7.00 |
+| GPTQ Triton                                        |   4  |     -1     |    10325    | 0.95 |    4.74   |  7.49 | 7.00 |
+| GPTQ Triton                                        |   4  |    128     |     9547    | 0.92 |    4.67   |  7.38 | 6.99 |
 
 
 | [LLaMA-30B](https://arxiv.org/abs/2302.13971)      | Bits | group-size | memory(MiB) | it/s | Wikitext2 |  PTB  |  C4  |
 | -------------------------------------------------- | ---- | ---------- | ----------- | ---- | --------- | ----- | ---- |
 | FP16                                               |  16  |      -     |    72491    |   -  |    3.61   |  6.50 | 6.07 |
+| GPTQ Triton                                        |   4  |     -1     |    19989    | 0.40 |    3.89   |  6.71 | 6.44 |
+| GPTQ Triton                                        |   4  |    128     |    20055    | 0.39 |    3.79   |  6.70 | 6.34 |
+| GPTQ Triton                                        |   4  |    512     |    19547    | 0.39 |    3.78   |  6.62 | 6.30 |
 
 
 ## Requirements
 
 See `setup.cfg`, but note that a nightly `transformers` is preferred right now. v4.28.1 might work.  Known working `transformers` commit is `28f26c107b4a1c5c7e32ed4d9575622da0627a40`.
```

### Comparing `gptq_triton-0.0.3/setup.cfg` & `gptq_triton-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gptq_triton
-version = 0.0.3
+version = 0.0.4
 author = fpgaminer
 author_email = fpgaminer@bitcoin-mining.com
 description = Fast GPTQ kernels written in Triton
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://github.com/fpgaminer/GPTQ-triton
 keywords = gptq, triton, torch, cuda, gpu, quantization, quantize, quantized, inference, deep learning, machine learning
```

### Comparing `gptq_triton-0.0.3/src/gptq_triton/__init__.py` & `gptq_triton-0.0.4/src/gptq_triton/__init__.py`

 * *Files identical despite different names*

### Comparing `gptq_triton-0.0.3/src/gptq_triton/custom_autotune.py` & `gptq_triton-0.0.4/src/gptq_triton/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `gptq_triton-0.0.3/src/gptq_triton/fused_attention.py` & `gptq_triton-0.0.4/src/gptq_triton/fused_attention.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,14 +102,21 @@
 		query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin, position_ids)
 		# [bsz, nh, t, hd]
 
 		if past_key_value is not None:
 			# reuse k, v, self_attention
 			key_states = torch.cat([past_key_value[0], key_states], dim=2)
 			value_states = torch.cat([past_key_value[1], value_states], dim=2)
+		
+		if use_cache:
+			# Since qkv_proj is fused, query_states etc will hold a reference to the original qkv_states tensor
+			# which can cause excessive memory usage by the cache. `contiguous` is a convenient way to workaround this.
+			query_states = query_states.contiguous()
+			key_states = key_states.contiguous()
+			value_states = value_states.contiguous()
 
 		past_key_value = (key_states, value_states) if use_cache else None
 
 		attn_weights = torch.matmul(query_states, key_states.transpose(2, 3)) / math.sqrt(self.head_dim)
 
 		if attn_weights.size() != (bsz, self.num_heads, q_len, kv_seq_len):
 			raise ValueError(
```

### Comparing `gptq_triton-0.0.3/src/gptq_triton/fused_mlp.py` & `gptq_triton-0.0.4/src/gptq_triton/fused_mlp.py`

 * *Files identical despite different names*

### Comparing `gptq_triton-0.0.3/src/gptq_triton/quant_linear.py` & `gptq_triton-0.0.4/src/gptq_triton/quant_linear.py`

 * *Files identical despite different names*

### Comparing `gptq_triton-0.0.3/src/gptq_triton/utils.py` & `gptq_triton-0.0.4/src/gptq_triton/utils.py`

 * *Files identical despite different names*

### Comparing `gptq_triton-0.0.3/src/gptq_triton.egg-info/PKG-INFO` & `gptq_triton-0.0.4/src/gptq_triton.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptq-triton
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fast GPTQ kernels written in Triton
 Home-page: https://github.com/fpgaminer/GPTQ-triton
 Author: fpgaminer
 Author-email: fpgaminer@bitcoin-mining.com
 License: Apache License 2.0
 Keywords: gptq,triton,torch,cuda,gpu,quantization,quantize,quantized,inference,deep learning,machine learning
 Classifier: Development Status :: 3 - Alpha
@@ -63,26 +63,30 @@
 it/s numbers are from a 3090.
 
 
 | [LLaMA-7B](https://arxiv.org/abs/2302.13971)       | Bits | group-size | memory(MiB) | it/s | Wikitext2 |  PTB  |  C4  | 
 | -------------------------------------------------- | ---- | ---------- | ----------- | ---- | --------- | ----- | ---- |
 | FP16                                               |  16  |      -     |    17373    | 1.64 |    5.04   |  7.85 | 6.99 |
 | GPTQ CUDA                                          |   4  |     -1     |     8805    | 0.11 |    5.44   |  8.24 |   -  |
-| GPTQ Triton                                        |   4  |     -1     |     8099    | 1.63 |    5.44   |  8.24 | 7.48 |
+| GPTQ Triton                                        |   4  |     -1     |     6323    | 1.70 |    5.44   |  8.24 | 7.48 |
 
 
 | [LLaMA-13B](https://arxiv.org/abs/2302.13971)      | Bits | group-size | memory(MiB) | it/s | Wikitext2 |  PTB  |  C4  |
 | -------------------------------------------------- | ---- | ---------- | ----------- | ---- | --------- | ----- | ---- |
 | FP16                                               |  16  |      -     |    31633    |   -  |    4.52   |  7.19 | 6.66 |
-| GPTQ Triton                                        |   4  |     -1     |    13241    | 0.89 |    4.74   |  7.49 | 7.00 |
+| GPTQ Triton                                        |   4  |     -1     |    10325    | 0.95 |    4.74   |  7.49 | 7.00 |
+| GPTQ Triton                                        |   4  |    128     |     9547    | 0.92 |    4.67   |  7.38 | 6.99 |
 
 
 | [LLaMA-30B](https://arxiv.org/abs/2302.13971)      | Bits | group-size | memory(MiB) | it/s | Wikitext2 |  PTB  |  C4  |
 | -------------------------------------------------- | ---- | ---------- | ----------- | ---- | --------- | ----- | ---- |
 | FP16                                               |  16  |      -     |    72491    |   -  |    3.61   |  6.50 | 6.07 |
+| GPTQ Triton                                        |   4  |     -1     |    19989    | 0.40 |    3.89   |  6.71 | 6.44 |
+| GPTQ Triton                                        |   4  |    128     |    20055    | 0.39 |    3.79   |  6.70 | 6.34 |
+| GPTQ Triton                                        |   4  |    512     |    19547    | 0.39 |    3.78   |  6.62 | 6.30 |
 
 
 ## Requirements
 
 See `setup.cfg`, but note that a nightly `transformers` is preferred right now. v4.28.1 might work.  Known working `transformers` commit is `28f26c107b4a1c5c7e32ed4d9575622da0627a40`.
```


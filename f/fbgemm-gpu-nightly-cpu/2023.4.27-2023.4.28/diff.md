# Comparing `tmp/fbgemm_gpu_nightly_cpu-2023.4.27-cp39-cp39-manylinux1_x86_64.whl.zip` & `tmp/fbgemm_gpu_nightly_cpu-2023.4.28-cp39-cp39-manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,39 +1,39 @@
-Zip file size: 3845303 bytes, number of entries: 37
--rw-r--r--  2.0 unx      566 b- defN 23-Apr-27 12:59 fbgemm_gpu/__init__.py
--rw-r--r--  2.0 unx    14798 b- defN 23-Apr-27 12:59 fbgemm_gpu/_fbgemm_gpu_docs.py
--rw-r--r--  2.0 unx     2746 b- defN 23-Apr-27 12:59 fbgemm_gpu/batched_unary_embeddings_ops.py
--rw-r--r--  2.0 unx      817 b- defN 23-Apr-27 12:59 fbgemm_gpu/enums.py
--rwxr-xr-x  2.0 unx 13805488 b- defN 23-Apr-27 12:59 fbgemm_gpu/fbgemm_gpu_py.so
--rw-r--r--  2.0 unx     5646 b- defN 23-Apr-27 12:59 fbgemm_gpu/metrics.py
--rw-r--r--  2.0 unx     2338 b- defN 23-Apr-27 12:59 fbgemm_gpu/permute_pooled_embedding_modules.py
--rw-r--r--  2.0 unx     2476 b- defN 23-Apr-27 12:59 fbgemm_gpu/permute_pooled_embedding_modules_split.py
--rw-r--r--  2.0 unx     7682 b- defN 23-Apr-27 12:59 fbgemm_gpu/quantize_comm.py
--rw-r--r--  2.0 unx     4004 b- defN 23-Apr-27 12:59 fbgemm_gpu/quantize_utils.py
--rw-r--r--  2.0 unx     5726 b- defN 23-Apr-27 12:59 fbgemm_gpu/split_embedding_configs.py
--rw-r--r--  2.0 unx     8737 b- defN 23-Apr-27 12:59 fbgemm_gpu/split_embedding_inference_converter.py
--rw-r--r--  2.0 unx    20501 b- defN 23-Apr-27 12:59 fbgemm_gpu/split_embedding_utils.py
--rw-r--r--  2.0 unx   133511 b- defN 23-Apr-27 12:59 fbgemm_gpu/split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx    39017 b- defN 23-Apr-27 12:59 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx      909 b- defN 23-Apr-27 12:59 fbgemm_gpu/uvm.py
--rw-r--r--  2.0 unx     1912 b- defN 23-Apr-27 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
--rw-r--r--  2.0 unx     4399 b- defN 23-Apr-27 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
--rw-r--r--  2.0 unx     5220 b- defN 23-Apr-27 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
--rw-r--r--  2.0 unx     4717 b- defN 23-Apr-27 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad.py
--rw-r--r--  2.0 unx     6838 b- defN 23-Apr-27 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     4753 b- defN 23-Apr-27 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     3918 b- defN 23-Apr-27 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_sgd.py
--rw-r--r--  2.0 unx     1532 b- defN 23-Apr-27 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
--rw-r--r--  2.0 unx     5220 b- defN 23-Apr-27 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
--rw-r--r--  2.0 unx     4653 b- defN 23-Apr-27 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
--rw-r--r--  2.0 unx     5252 b- defN 23-Apr-27 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
--rw-r--r--  2.0 unx     5252 b- defN 23-Apr-27 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
--rw-r--r--  2.0 unx     4703 b- defN 23-Apr-27 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
--rw-r--r--  2.0 unx     6824 b- defN 23-Apr-27 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     4739 b- defN 23-Apr-27 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     4659 b- defN 23-Apr-27 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
--rw-r--r--  2.0 unx     3904 b- defN 23-Apr-27 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
--rw-r--r--  2.0 unx     4508 b- defN 23-Apr-27 12:59 fbgemm_gpu_nightly_cpu-2023.4.27.dist-info/METADATA
--rw-r--r--  2.0 unx      102 b- defN 23-Apr-27 12:59 fbgemm_gpu_nightly_cpu-2023.4.27.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-27 12:59 fbgemm_gpu_nightly_cpu-2023.4.27.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4129 b- defN 23-Apr-27 12:59 fbgemm_gpu_nightly_cpu-2023.4.27.dist-info/RECORD
-37 files, 14142207 bytes uncompressed, 3838327 bytes compressed:  72.9%
+Zip file size: 3845360 bytes, number of entries: 37
+-rw-r--r--  2.0 unx      566 b- defN 23-Apr-28 12:58 fbgemm_gpu/__init__.py
+-rw-r--r--  2.0 unx    14798 b- defN 23-Apr-28 12:58 fbgemm_gpu/_fbgemm_gpu_docs.py
+-rw-r--r--  2.0 unx     2746 b- defN 23-Apr-28 12:58 fbgemm_gpu/batched_unary_embeddings_ops.py
+-rw-r--r--  2.0 unx      817 b- defN 23-Apr-28 12:58 fbgemm_gpu/enums.py
+-rwxr-xr-x  2.0 unx 13805488 b- defN 23-Apr-28 12:58 fbgemm_gpu/fbgemm_gpu_py.so
+-rw-r--r--  2.0 unx     5646 b- defN 23-Apr-28 12:58 fbgemm_gpu/metrics.py
+-rw-r--r--  2.0 unx     2338 b- defN 23-Apr-28 12:58 fbgemm_gpu/permute_pooled_embedding_modules.py
+-rw-r--r--  2.0 unx     2476 b- defN 23-Apr-28 12:58 fbgemm_gpu/permute_pooled_embedding_modules_split.py
+-rw-r--r--  2.0 unx     7682 b- defN 23-Apr-28 12:58 fbgemm_gpu/quantize_comm.py
+-rw-r--r--  2.0 unx     4004 b- defN 23-Apr-28 12:58 fbgemm_gpu/quantize_utils.py
+-rw-r--r--  2.0 unx     5726 b- defN 23-Apr-28 12:58 fbgemm_gpu/split_embedding_configs.py
+-rw-r--r--  2.0 unx     8737 b- defN 23-Apr-28 12:58 fbgemm_gpu/split_embedding_inference_converter.py
+-rw-r--r--  2.0 unx    20501 b- defN 23-Apr-28 12:58 fbgemm_gpu/split_embedding_utils.py
+-rw-r--r--  2.0 unx   133909 b- defN 23-Apr-28 12:58 fbgemm_gpu/split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx    39017 b- defN 23-Apr-28 12:58 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx      909 b- defN 23-Apr-28 12:58 fbgemm_gpu/uvm.py
+-rw-r--r--  2.0 unx     1912 b- defN 23-Apr-28 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
+-rw-r--r--  2.0 unx     4399 b- defN 23-Apr-28 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
+-rw-r--r--  2.0 unx     5220 b- defN 23-Apr-28 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
+-rw-r--r--  2.0 unx     4717 b- defN 23-Apr-28 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     6838 b- defN 23-Apr-28 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     4753 b- defN 23-Apr-28 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     3918 b- defN 23-Apr-28 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_sgd.py
+-rw-r--r--  2.0 unx     1532 b- defN 23-Apr-28 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
+-rw-r--r--  2.0 unx     5220 b- defN 23-Apr-28 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
+-rw-r--r--  2.0 unx     4653 b- defN 23-Apr-28 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
+-rw-r--r--  2.0 unx     5252 b- defN 23-Apr-28 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
+-rw-r--r--  2.0 unx     5252 b- defN 23-Apr-28 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
+-rw-r--r--  2.0 unx     4703 b- defN 23-Apr-28 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     6824 b- defN 23-Apr-28 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     4739 b- defN 23-Apr-28 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     4659 b- defN 23-Apr-28 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
+-rw-r--r--  2.0 unx     3904 b- defN 23-Apr-28 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
+-rw-r--r--  2.0 unx     4508 b- defN 23-Apr-28 12:58 fbgemm_gpu_nightly_cpu-2023.4.28.dist-info/METADATA
+-rw-r--r--  2.0 unx      102 b- defN 23-Apr-28 12:58 fbgemm_gpu_nightly_cpu-2023.4.28.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-28 12:58 fbgemm_gpu_nightly_cpu-2023.4.28.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4129 b- defN 23-Apr-28 12:58 fbgemm_gpu_nightly_cpu-2023.4.28.dist-info/RECORD
+37 files, 14142605 bytes uncompressed, 3838384 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -93,20 +93,20 @@
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.4.27.dist-info/METADATA
+Filename: fbgemm_gpu_nightly_cpu-2023.4.28.dist-info/METADATA
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.4.27.dist-info/WHEEL
+Filename: fbgemm_gpu_nightly_cpu-2023.4.28.dist-info/WHEEL
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.4.27.dist-info/top_level.txt
+Filename: fbgemm_gpu_nightly_cpu-2023.4.28.dist-info/top_level.txt
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.4.27.dist-info/RECORD
+Filename: fbgemm_gpu_nightly_cpu-2023.4.28.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbgemm_gpu/split_table_batched_embeddings_ops.py

```diff
@@ -454,14 +454,21 @@
         if (
             weight_decay_mode == WeightDecayMode.COUNTER
             and counter_based_regularization is None
         ):
             raise AssertionError(
                 "weight_decay_mode is set to WeightDecayMode.COUNTER but counter_based_regularization is None"
             )
+        if (
+            weight_decay_mode != WeightDecayMode.COUNTER
+            and counter_based_regularization is not None
+        ):
+            raise AssertionError(
+                "Need to set weight_decay_mode to WeightDecayMode.COUNTER together with counter_based_regularization"
+            )
 
         self._used_rowwise_adagrad_with_counter: bool = (
             optimizer in (OptimType.EXACT_ROWWISE_ADAGRAD, OptimType.ROWWISE_ADAGRAD)
             and weight_decay_mode == WeightDecayMode.COUNTER
             and counter_based_regularization is not None
         )
 
@@ -636,15 +643,16 @@
             cache_load_factor,
             cache_sets,
             cache_reserved_memory,
             dtype=cache_embedding_dtype,
         )
 
         logging.info(
-            f"Using fused {optimizer} with optimizer_args={self.optimizer_args}"
+            f"Using fused {optimizer} with optimizer_args={self.optimizer_args}\n"
+            f"Using rowwise_adagrad_with_counter={self._used_rowwise_adagrad_with_counter}"
         )
 
         self.step = 0
 
     def _register_nonpersistent_buffers(self, prefix: str) -> None:
         # NOTE: make TorchScript work!
         self.register_buffer(
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.4.27.dist-info/METADATA` & `fbgemm_gpu_nightly_cpu-2023.4.28.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbgemm-gpu-nightly-cpu
-Version: 2023.4.27
+Version: 2023.4.28
 Home-page: https://github.com/pytorch/fbgemm
 Author: FBGEMM Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: PyTorch,Recommendation Models,High Performance Computing,GPU,CUDA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.4.27.dist-info/RECORD` & `fbgemm_gpu_nightly_cpu-2023.4.28.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 fbgemm_gpu/permute_pooled_embedding_modules.py,sha256=sYThngxF_hVIfDArggWW0fKW2m99mT255ytCteqWwfY,2338
 fbgemm_gpu/permute_pooled_embedding_modules_split.py,sha256=fNyzhUOV6yaRZLnpLYtQsg83WUY8YXiTCFrrvmSJ4r8,2476
 fbgemm_gpu/quantize_comm.py,sha256=qONCevOTVA89K7vFJe-Bcc903lHsKDg6s661pTHCF2k,7682
 fbgemm_gpu/quantize_utils.py,sha256=_EvEb4NbNsKd0wFJN4hl0vzlOm4twkkh24zb5l4hg8Y,4004
 fbgemm_gpu/split_embedding_configs.py,sha256=cOJy6WDwH03uXjAHO-KcpndFYydaw5qg2wQLUGf9xLg,5726
 fbgemm_gpu/split_embedding_inference_converter.py,sha256=RR_tp_Ds3ijF5-nW0iJyWPGImH91t6kNfMi9KOcVXOc,8737
 fbgemm_gpu/split_embedding_utils.py,sha256=Ql3Y6qMekT2NEaOmRcgYropWaks1bV9h61cMHgra56c,20501
-fbgemm_gpu/split_table_batched_embeddings_ops.py,sha256=Tg5mn2JHGC_rRJCZmsC_3XhK34tK5O1ewEOFvJcPd5o,133511
+fbgemm_gpu/split_table_batched_embeddings_ops.py,sha256=lce5D26m2dfPUZohT-usG49HTnvXAZr0gdl_SebcmYU,133909
 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py,sha256=ny6r_ZS1TnkO5pHD_B8couJI6HlQGrxQdqRRRJjFLbk,39017
 fbgemm_gpu/uvm.py,sha256=bIjcw3-T5JS9l6QRd-4vobiuXiuik_UGGHIrx20GFbk,909
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py,sha256=urwpbmpUGaoOY-5IgiFvDj53cu3jvJ1_f4r7jru-yhI,1912
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py,sha256=RCY4NBdVW_4ODUxphZZOugGdhHuFQXy3M5bSNnK8quA,4399
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py,sha256=wKRLpkhIba2EoBnx1Sczh-5ytepdQ4FeIKnAyGl1Vqc,5220
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad.py,sha256=RKw2ta5LK23Hn6y-VKDkTIiUXEx61OQFyp3iR-g03W8,4717
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_counter.py,sha256=5fVXsvr8wXxu_5TEaNb-nxMkk7CLp7hDhZF_GNk3EZ8,6838
@@ -27,11 +27,11 @@
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py,sha256=dzvN4ncV0v_CbbNsH1GvSlD4e8NPAXBTsm3jJcjIZXk,5252
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py,sha256=8DhgL58GU-fRk_F0naL641aES3lRWw5wllP2Zfe2wBo,5252
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py,sha256=hN1jKQl_3iWFF96XBx30skWBucd7EnVXzmWND8fKip8,4703
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py,sha256=wCSrH66-R4cMXNoJ9mnbXuEpZiSRYDe_3rJqaSCJya4,6824
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py,sha256=QdQtmO6YCVQSbt7hnrTKuxoIy23ZOkGDmGgG7RMuGMo,4739
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py,sha256=OcL6PJf1eccTqsMphXbcD4bTjOSnWG2QZHnIslFtuR8,4659
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=8h7h5UGzaTX4Hs5zwpsmhbUP1DX2pQytYmLe1-yyFyY,3904
-fbgemm_gpu_nightly_cpu-2023.4.27.dist-info/METADATA,sha256=gRrfdecr10SrzG2PVPO7bZa7qBQBgM-HehIDJSdOzg8,4508
-fbgemm_gpu_nightly_cpu-2023.4.27.dist-info/WHEEL,sha256=7fnRuWrgVZ-We1c67_7QZCYn_AQfJ-Z7mCmVro0eJMM,102
-fbgemm_gpu_nightly_cpu-2023.4.27.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
-fbgemm_gpu_nightly_cpu-2023.4.27.dist-info/RECORD,,
+fbgemm_gpu_nightly_cpu-2023.4.28.dist-info/METADATA,sha256=6n1OJakeRXiAia26CYJy9oxucJIUM9osLS310skhygs,4508
+fbgemm_gpu_nightly_cpu-2023.4.28.dist-info/WHEEL,sha256=7fnRuWrgVZ-We1c67_7QZCYn_AQfJ-Z7mCmVro0eJMM,102
+fbgemm_gpu_nightly_cpu-2023.4.28.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
+fbgemm_gpu_nightly_cpu-2023.4.28.dist-info/RECORD,,
```


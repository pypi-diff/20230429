# Comparing `tmp/colossalai-nightly-2023.4.29.tar.gz` & `tmp/colossalai-nightly-2023.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colossalai-nightly-2023.4.29.tar", last modified: Sat Apr 29 00:14:12 2023, max compression
+gzip compressed data, was "colossalai-nightly-2023.4.8.tar", last modified: Sat Apr  8 00:13:40 2023, max compression
```

## Comparing `colossalai-nightly-2023.4.29.tar` & `colossalai-nightly-2023.4.8.tar`

### file list

```diff
@@ -1,872 +1,871 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.662504 colossalai-nightly-2023.4.29/
--rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-04-29 00:14:12.662504 colossalai-nightly-2023.4.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19962 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.562502 colossalai-nightly-2023.4.29/colossalai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.562502 colossalai-nightly-2023.4.29/colossalai/_C/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/_C/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.562502 colossalai-nightly-2023.4.29/colossalai/amp/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/amp/amp_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.562502 colossalai-nightly-2023.4.29/colossalai/amp/apex_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/amp/apex_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/amp/apex_amp/apex_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.562502 colossalai-nightly-2023.4.29/colossalai/amp/naive_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/amp/naive_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/amp/naive_amp/_fp16_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/amp/naive_amp/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.562502 colossalai-nightly-2023.4.29/colossalai/amp/naive_amp/grad_scaler/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/amp/naive_amp/grad_scaler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/amp/naive_amp/naive_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.562502 colossalai-nightly-2023.4.29/colossalai/amp/torch_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/amp/torch_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/amp/torch_amp/_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/amp/torch_amp/torch_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.562502 colossalai-nightly-2023.4.29/colossalai/auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.562502 colossalai-nightly-2023.4.29/colossalai/auto_parallel/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/checkpoint/build_c_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
--rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/checkpoint/operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.566503 colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.566503 colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.566503 colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/amp_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/base_offload_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/mem_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/region.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/region_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/training_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.566503 colossalai-nightly-2023.4.29/colossalai/auto_parallel/passes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/passes/comm_metainfo_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/passes/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/passes/runtime_apply_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    22689 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/passes/runtime_preparation_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.566503 colossalai-nightly-2023.4.29/colossalai/auto_parallel/pipeline_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/pipeline_shard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.566503 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.570503 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14745 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20533 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.574503 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43503 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.574503 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9987 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/solver/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.574503 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/utils/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/utils/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/utils/sharding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.574503 colossalai-nightly-2023.4.29/colossalai/booster/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/booster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/booster/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/booster/booster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.574503 colossalai-nightly-2023.4.29/colossalai/booster/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/booster/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/booster/mixed_precision/bf16.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/booster/mixed_precision/fp16_apex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/booster/mixed_precision/fp16_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/booster/mixed_precision/fp8.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/booster/mixed_precision/mixed_precision_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.574503 colossalai-nightly-2023.4.29/colossalai/booster/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/booster/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/booster/plugin/gemini_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/booster/plugin/low_level_zero_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/booster/plugin/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/booster/plugin/torch_ddp_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.574503 colossalai-nightly-2023.4.29/colossalai/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/builder/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.574503 colossalai-nightly-2023.4.29/colossalai/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/checkpoint_io/checkpoint_io_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/checkpoint_io/general_checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/checkpoint_io/index_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/checkpoint_io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.578503 colossalai-nightly-2023.4.29/colossalai/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.578503 colossalai-nightly-2023.4.29/colossalai/cli/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/cli/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/cli/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/cli/benchmark/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/cli/benchmark/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.578503 colossalai-nightly-2023.4.29/colossalai/cli/check/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/cli/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/cli/check/check_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.578503 colossalai-nightly-2023.4.29/colossalai/cli/launcher/
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/cli/launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/cli/launcher/hostinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/cli/launcher/multinode_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/cli/launcher/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.578503 colossalai-nightly-2023.4.29/colossalai/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/cluster/device_mesh_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/cluster/dist_coordinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/cluster/process_group_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.578503 colossalai-nightly-2023.4.29/colossalai/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/communication/collective.py
--rw-r--r--   0 runner    (1001) docker     (123)    19463 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/communication/p2p.py
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/communication/p2p_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/communication/ring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/communication/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.578503 colossalai-nightly-2023.4.29/colossalai/context/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/moe_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/parallel_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/parallel_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.582503 colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/initializer_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/initializer_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/initializer_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/initializer_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/initializer_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/initializer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/initializer_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/initializer_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/initializer_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/process_group_initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.582503 colossalai-nightly-2023.4.29/colossalai/context/random/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/random/_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/random/seed_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/context/singleton_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.582503 colossalai-nightly-2023.4.29/colossalai/device/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/device/alpha_beta_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/device/calc_pipeline_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/device/device_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.582503 colossalai-nightly-2023.4.29/colossalai/engine/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/engine/_base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.582503 colossalai-nightly-2023.4.29/colossalai/engine/gradient_accumulation/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/engine/gradient_accumulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/engine/gradient_accumulation/_gradient_accumulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.582503 colossalai-nightly-2023.4.29/colossalai/engine/gradient_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/engine/gradient_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/engine/gradient_handler/_base_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/engine/gradient_handler/_moe_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/engine/gradient_handler/_zero_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/engine/gradient_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.582503 colossalai-nightly-2023.4.29/colossalai/engine/schedule/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/engine/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/engine/schedule/_base_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/engine/schedule/_non_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/engine/schedule/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/engine/schedule/_pipeline_schedule_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.582503 colossalai-nightly-2023.4.29/colossalai/fx/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/_meta_regist_12.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/_meta_regist_13.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.582503 colossalai-nightly-2023.4.29/colossalai/fx/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44751 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/codegen/activation_checkpoint_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/graph_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.586503 colossalai-nightly-2023.4.29/colossalai/fx/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/passes/adding_split_node_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/passes/concrete_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/passes/passes_for_gpt2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/passes/shard_1d_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/passes/split_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/passes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.586503 colossalai-nightly-2023.4.29/colossalai/fx/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.586503 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.586503 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_function/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_function/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_function/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.590503 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_module/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_module/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_module/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/memory_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/opcount.py
--rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/profiler/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.590503 colossalai-nightly-2023.4.29/colossalai/fx/tracer/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/_meta_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/_symbolic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/_tracer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.590503 colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.590503 colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.590503 colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.590503 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.590503 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_function/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.594503 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_module/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    24623 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/fx/tracer/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/global_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.594503 colossalai-nightly-2023.4.29/colossalai/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/interface/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/interface/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.594503 colossalai-nightly-2023.4.29/colossalai/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.594503 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.594503 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/compat.h
--rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/cpu_adam.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.598503 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu
--rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.602503 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/context.h
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
--rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/type_shim.h
--rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/scaled_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.602503 colossalai-nightly-2023.4.29/colossalai/kernel/jit/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/jit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/jit/bias_dropout_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/jit/bias_gelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/jit/option.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.610503 colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/fused_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/moe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/multi_head_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/scaled_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.610503 colossalai-nightly-2023.4.29/colossalai/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.610503 colossalai-nightly-2023.4.29/colossalai/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.614503 colossalai-nightly-2023.4.29/colossalai/nn/_ops/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/_ops/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/_ops/addmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/_ops/batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/_ops/element_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/_ops/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/_ops/embedding_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/_ops/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/_ops/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/_ops/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/_ops/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.614503 colossalai-nightly-2023.4.29/colossalai/nn/layer/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/base_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.614503 colossalai-nightly-2023.4.29/colossalai/nn/layer/colossalai_layer/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/colossalai_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/colossalai_layer/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/colossalai_layer/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/colossalai_layer/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/colossalai_layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/colossalai_layer/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.618503 colossalai-nightly-2023.4.29/colossalai/nn/layer/moe/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/moe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/moe/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/moe/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/moe/experts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/moe/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/moe/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/moe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.618503 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_1d/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_1d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_1d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49753 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_1d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.618503 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_2d/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_2d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_2d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50524 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_2d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.618503 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_2p5d/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_2p5d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37643 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_2p5d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_2p5d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_2p5d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.618503 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_3d/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_3d/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22769 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_3d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_3d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_3d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.618503 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_sequence/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_sequence/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_sequence/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.618503 colossalai-nightly-2023.4.29/colossalai/nn/layer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.618503 colossalai-nightly-2023.4.29/colossalai/nn/layer/vanilla/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/vanilla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/vanilla/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.622503 colossalai-nightly-2023.4.29/colossalai/nn/layer/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/layer/wrapper/pipeline_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.622503 colossalai-nightly-2023.4.29/colossalai/nn/loss/
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/loss/loss_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/loss/loss_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/loss/loss_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/loss/loss_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/loss/loss_moe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.622503 colossalai-nightly-2023.4.29/colossalai/nn/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/lr_scheduler/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/lr_scheduler/delayed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/lr_scheduler/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/lr_scheduler/multistep.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/lr_scheduler/onecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/lr_scheduler/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/lr_scheduler/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.622503 colossalai-nightly-2023.4.29/colossalai/nn/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/metric/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/metric/accuracy_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/metric/accuracy_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/metric/accuracy_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.622503 colossalai-nightly-2023.4.29/colossalai/nn/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/optimizer/colossalai_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/optimizer/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/optimizer/fused_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/optimizer/fused_lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/optimizer/fused_sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/optimizer/hybrid_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/optimizer/lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/optimizer/lars.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/optimizer/nvme_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.622503 colossalai-nightly-2023.4.29/colossalai/nn/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/parallel/data_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.622503 colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.626504 colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/copyer.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/colo_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/nn/parallel/reducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.626504 colossalai-nightly-2023.4.29/colossalai/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/pipeline/layer_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.626504 colossalai-nightly-2023.4.29/colossalai/pipeline/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/pipeline/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.626504 colossalai-nightly-2023.4.29/colossalai/pipeline/middleware/adaptor/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/pipeline/middleware/adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/pipeline/middleware/adaptor/fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/pipeline/middleware/topo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/pipeline/pipelinable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/pipeline/pipeline_process_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.626504 colossalai-nightly-2023.4.29/colossalai/pipeline/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/pipeline/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59163 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/pipeline/rpc/_pipeline_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/pipeline/rpc/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/pipeline/rpc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.626504 colossalai-nightly-2023.4.29/colossalai/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/registry/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.630504 colossalai-nightly-2023.4.29/colossalai/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/colo_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/colo_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22269 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/compute_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.630504 colossalai-nightly-2023.4.29/colossalai/tensor/d_tensor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/d_tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/d_tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/d_tensor/d_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/d_tensor/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    25229 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/d_tensor/layout_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/d_tensor/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/d_tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/d_tensor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/dist_spec_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/distspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/op_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/param_op_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/process_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    36495 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/shape_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/tensor_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.630504 colossalai-nightly-2023.4.29/colossalai/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/testing/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/testing/pytest_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/testing/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.630504 colossalai-nightly-2023.4.29/colossalai/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/trainer/_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.630504 colossalai-nightly-2023.4.29/colossalai/trainer/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/trainer/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/trainer/hooks/_base_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/trainer/hooks/_checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/trainer/hooks/_commons_.py
--rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/trainer/hooks/_log_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/trainer/hooks/_lr_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/trainer/hooks/_metric_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.630504 colossalai-nightly-2023.4.29/colossalai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/activation_checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.630504 colossalai-nightly-2023.4.29/colossalai/utils/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/checkpoint/module_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/checkpoint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.634504 colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/convertor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17451 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.634504 colossalai-nightly-2023.4.29/colossalai/utils/data_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/data_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/data_sampler/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/data_sampler/data_parallel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.634504 colossalai-nightly-2023.4.29/colossalai/utils/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/model/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/model/lazy_init_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/moe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.634504 colossalai-nightly-2023.4.29/colossalai/utils/multi_tensor_apply/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/multi_tensor_apply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.634504 colossalai-nightly-2023.4.29/colossalai/utils/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/profiler/extention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.634504 colossalai-nightly-2023.4.29/colossalai/utils/profiler/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/profiler/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/profiler/legacy/comm_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/profiler/legacy/pcie_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/profiler/legacy/prof_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/profiler/stateful_tensor_mem_extention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.634504 colossalai-nightly-2023.4.29/colossalai/utils/rank_recorder/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/rank_recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/rank_recorder/rank_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.634504 colossalai-nightly-2023.4.29/colossalai/utils/tensor_detector/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/tensor_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/tensor_detector/tensor_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.634504 colossalai-nightly-2023.4.29/colossalai/zero/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.634504 colossalai-nightly-2023.4.29/colossalai/zero/gemini/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.638504 colossalai-nightly-2023.4.29/colossalai/zero/gemini/chunk/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/chunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/chunk/chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/chunk/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/chunk/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/chunk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/colo_init_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    35211 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/gemini_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/gemini_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/gemini_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/gemini_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.638504 colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/memory_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/gemini/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.638504 colossalai-nightly-2023.4.29/colossalai/zero/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.638504 colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/gemini_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.642504 colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/ophooks/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/ophooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/ophooks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.642504 colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/paramhooks/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/paramhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/stateful_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/tensor_placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/tensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.642504 colossalai-nightly-2023.4.29/colossalai/zero/legacy/init_ctx/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/init_ctx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/init_ctx/init_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.642504 colossalai-nightly-2023.4.29/colossalai/zero/legacy/shard_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/shard_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/shard_utils/base_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/shard_utils/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.646504 colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_model/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_model/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_model/reduce_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29015 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_model/sharded_model_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_model/zero_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.646504 colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_optim/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.646504 colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_param/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_param/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_param/sharded_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_param/sharded_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.646504 colossalai-nightly-2023.4.29/colossalai/zero/low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/low_level/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.646504 colossalai-nightly-2023.4.29/colossalai/zero/low_level/bookkeeping/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/low_level/bookkeeping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/low_level/bookkeeping/base_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/low_level/bookkeeping/bucket_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/low_level/bookkeeping/gradient_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/low_level/bookkeeping/parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    25694 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/low_level/low_level_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/colossalai/zero/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.650504 colossalai-nightly-2023.4.29/colossalai_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-04-29 00:14:12.000000 colossalai-nightly-2023.4.29/colossalai_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36337 2023-04-29 00:14:12.000000 colossalai-nightly-2023.4.29/colossalai_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:14:12.000000 colossalai-nightly-2023.4.29/colossalai_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-29 00:14:12.000000 colossalai-nightly-2023.4.29/colossalai_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-29 00:14:12.000000 colossalai-nightly-2023.4.29/colossalai_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-29 00:14:12.000000 colossalai-nightly-2023.4.29/colossalai_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.650504 colossalai-nightly-2023.4.29/op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/op_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/op_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/op_builder/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/op_builder/fused_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/op_builder/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/op_builder/moe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/op_builder/multi_head_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/op_builder/scaled_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/op_builder/scaled_upper_triangle_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/op_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.650504 colossalai-nightly-2023.4.29/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 00:14:12.662504 colossalai-nightly-2023.4.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.562502 colossalai-nightly-2023.4.29/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.650504 colossalai-nightly-2023.4.29/tests/components_to_test/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/components_to_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/components_to_test/albert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/components_to_test/beit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/components_to_test/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/components_to_test/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/components_to_test/hanging_param_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/components_to_test/inline_op_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/components_to_test/nested_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/components_to_test/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/components_to_test/repeated_computed_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/components_to_test/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/components_to_test/simple_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.654504 colossalai-nightly-2023.4.29/tests/components_to_test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/components_to_test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/components_to_test/utils/dummy_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/components_to_test/utils/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.654504 colossalai-nightly-2023.4.29/tests/kit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.654504 colossalai-nightly-2023.4.29/tests/kit/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/model_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.654504 colossalai-nightly-2023.4.29/tests/kit/model_zoo/diffusers/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/model_zoo/diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/model_zoo/diffusers/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/model_zoo/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.654504 colossalai-nightly-2023.4.29/tests/kit/model_zoo/timm/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/model_zoo/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/model_zoo/timm/timm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.654504 colossalai-nightly-2023.4.29/tests/kit/model_zoo/torchaudio/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/model_zoo/torchaudio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/model_zoo/torchaudio/torchaudio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.654504 colossalai-nightly-2023.4.29/tests/kit/model_zoo/torchrec/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/model_zoo/torchrec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/model_zoo/torchrec/torchrec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.654504 colossalai-nightly-2023.4.29/tests/kit/model_zoo/torchvision/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/model_zoo/torchvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/model_zoo/torchvision/torchvision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.654504 colossalai-nightly-2023.4.29/tests/kit/model_zoo/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/model_zoo/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/model_zoo/transformers/albert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/model_zoo/transformers/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/model_zoo/transformers/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/model_zoo/transformers/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/kit/model_zoo/transformers/t5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.654504 colossalai-nightly-2023.4.29/tests/test_analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.658504 colossalai-nightly-2023.4.29/tests/test_analyzer/test_fx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_analyzer/test_fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_analyzer/test_fx/test_bias_addition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_analyzer/test_fx/test_mod_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_analyzer/test_fx/test_nested_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_analyzer/test_fx/test_shape_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_analyzer/test_fx/test_symbolic_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_analyzer/test_fx/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.658504 colossalai-nightly-2023.4.29/tests/test_analyzer/test_subclasses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_analyzer/test_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_analyzer/test_subclasses/test_aten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_analyzer/test_subclasses/test_flop_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_analyzer/test_subclasses/test_meta_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.658504 colossalai-nightly-2023.4.29/tests/test_auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.658504 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_pass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_pass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.658504 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.658504 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:12.662504 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 00:14:03.000000 colossalai-nightly-2023.4.29/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.453257 colossalai-nightly-2023.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    24234 2023-04-08 00:13:40.453257 colossalai-nightly-2023.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19848 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/_C/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/_C/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/amp_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/amp/apex_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/apex_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/apex_amp/apex_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/_fp16_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/grad_scaler/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/grad_scaler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/naive_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/amp/torch_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/torch_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/torch_amp/_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/torch_amp/torch_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/build_c_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.381252 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.381252 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/amp_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/base_offload_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/mem_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/region_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18548 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/training_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.381252 colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/comm_metainfo_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/runtime_apply_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22687 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/runtime_preparation_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.381252 colossalai-nightly-2023.4.8/colossalai/auto_parallel/pipeline_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/pipeline_shard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.381252 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.385252 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14745 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20533 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43503 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9987 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/sharding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/booster/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/booster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/bf16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/fp16_apex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/fp16_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/fp8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/mixed_precision_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/booster/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/plugin/gemini_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/plugin/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/plugin/torch_ddp_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/builder/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/checkpoint_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/checkpoint_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/checkpoint_io/checkpoint_io_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/checkpoint_io/general_checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/checkpoint_io/index_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/checkpoint_io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/cli/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/benchmark/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/benchmark/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.393253 colossalai-nightly-2023.4.8/colossalai/cli/check/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/check/check_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.393253 colossalai-nightly-2023.4.8/colossalai/cli/launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/launcher/hostinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/launcher/multinode_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/launcher/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.393253 colossalai-nightly-2023.4.8/colossalai/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cluster/device_mesh_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cluster/dist_coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cluster/process_group_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.393253 colossalai-nightly-2023.4.8/colossalai/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/communication/collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19463 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/communication/p2p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/communication/p2p_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/communication/ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/communication/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.393253 colossalai-nightly-2023.4.8/colossalai/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/moe_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23922 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/parallel_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/parallel_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.393253 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/process_group_initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.393253 colossalai-nightly-2023.4.8/colossalai/context/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/random/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/random/seed_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/singleton_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.393253 colossalai-nightly-2023.4.8/colossalai/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/device/alpha_beta_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/device/calc_pipeline_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/device/device_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.397253 colossalai-nightly-2023.4.8/colossalai/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/_base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.397253 colossalai-nightly-2023.4.8/colossalai/engine/gradient_accumulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_accumulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_accumulation/_gradient_accumulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.397253 colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_base_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_moe_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_zero_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.397253 colossalai-nightly-2023.4.8/colossalai/engine/schedule/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/schedule/_base_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/schedule/_non_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/schedule/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/schedule/_pipeline_schedule_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.397253 colossalai-nightly-2023.4.8/colossalai/fx/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/_meta_regist_12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/_meta_regist_13.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.397253 colossalai-nightly-2023.4.8/colossalai/fx/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/codegen/activation_checkpoint_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/graph_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.397253 colossalai-nightly-2023.4.8/colossalai/fx/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/passes/adding_split_node_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/passes/concrete_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/passes/passes_for_gpt2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/passes/shard_1d_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/passes/split_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/passes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.401254 colossalai-nightly-2023.4.8/colossalai/fx/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.401254 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.401254 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.401254 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/memory_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/opcount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.401254 colossalai-nightly-2023.4.8/colossalai/fx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/_meta_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/_symbolic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/_tracer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.401254 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.405254 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.405254 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.405254 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.405254 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.405254 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24623 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/global_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.405254 colossalai-nightly-2023.4.8/colossalai/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/interface/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/interface/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.405254 colossalai-nightly-2023.4.8/colossalai/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.405254 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.409254 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/cpu_adam.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.409254 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.413254 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/context.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/type_shim.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/scaled_softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.413254 colossalai-nightly-2023.4.8/colossalai/kernel/jit/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/jit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/jit/bias_dropout_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/jit/bias_gelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/jit/option.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.413254 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/fused_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/multi_head_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/scaled_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.413254 colossalai-nightly-2023.4.8/colossalai/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.413254 colossalai-nightly-2023.4.8/colossalai/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.413254 colossalai-nightly-2023.4.8/colossalai/nn/_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/element_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/embedding_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.413254 colossalai-nightly-2023.4.8/colossalai/nn/layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/base_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.413254 colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.417255 colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/experts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.417255 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_1d/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_1d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_1d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_1d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49748 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_1d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.417255 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2d/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50524 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.417255 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2p5d/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2p5d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37643 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2p5d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2p5d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2p5d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.417255 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_3d/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22769 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_3d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_3d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_3d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.417255 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_sequence/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_sequence/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_sequence/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.417255 colossalai-nightly-2023.4.8/colossalai/nn/layer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.417255 colossalai-nightly-2023.4.8/colossalai/nn/layer/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/vanilla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/vanilla/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.417255 colossalai-nightly-2023.4.8/colossalai/nn/layer/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/wrapper/pipeline_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.421255 colossalai-nightly-2023.4.8/colossalai/nn/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_moe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.421255 colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/delayed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/multistep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/onecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.421255 colossalai-nightly-2023.4.8/colossalai/nn/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/metric/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/metric/accuracy_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/metric/accuracy_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/metric/accuracy_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.421255 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/colossalai_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/fused_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/fused_lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/fused_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/hybrid_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/lars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/nvme_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.421255 colossalai-nightly-2023.4.8/colossalai/nn/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/data_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.421255 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.425255 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/copyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/colo_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/reducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.425255 colossalai-nightly-2023.4.8/colossalai/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/layer_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.425255 colossalai-nightly-2023.4.8/colossalai/pipeline/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/middleware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.425255 colossalai-nightly-2023.4.8/colossalai/pipeline/middleware/adaptor/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/middleware/adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/middleware/adaptor/fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/middleware/topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/pipelinable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/pipeline_process_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.425255 colossalai-nightly-2023.4.8/colossalai/pipeline/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59163 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/rpc/_pipeline_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/rpc/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/rpc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.425255 colossalai-nightly-2023.4.8/colossalai/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/registry/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.425255 colossalai-nightly-2023.4.8/colossalai/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/colo_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/colo_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22268 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/compute_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.429255 colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/d_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25229 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/layout_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/dist_spec_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/distspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/op_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/param_op_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/process_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36491 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/shape_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/tensor_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.429255 colossalai-nightly-2023.4.8/colossalai/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/testing/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/testing/pytest_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/testing/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.429255 colossalai-nightly-2023.4.8/colossalai/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/trainer/_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.429255 colossalai-nightly-2023.4.8/colossalai/trainer/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/trainer/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_base_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_commons_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_log_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_lr_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_metric_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.429255 colossalai-nightly-2023.4.8/colossalai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/activation_checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.429255 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint/module_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/convertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17451 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/utils/data_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/data_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/data_sampler/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/data_sampler/data_parallel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/utils/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21939 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/model/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/model/lazy_init_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/moe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/utils/multi_tensor_apply/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/multi_tensor_apply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/utils/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/profiler/extention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/utils/profiler/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/profiler/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/profiler/legacy/comm_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/profiler/legacy/pcie_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/profiler/legacy/prof_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/profiler/stateful_tensor_mem_extention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/utils/rank_recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/rank_recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/rank_recorder/rank_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/utils/tensor_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/tensor_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/tensor_detector/tensor_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/zero/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/zero/gemini/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.437256 colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/colo_init_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28189 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/gemini_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/gemini_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/gemini_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/gemini_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.437256 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/memory_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.437256 colossalai-nightly-2023.4.8/colossalai/zero/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.437256 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/gemini_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.437256 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.437256 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/paramhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/paramhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/stateful_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/tensor_placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/tensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.437256 colossalai-nightly-2023.4.8/colossalai/zero/legacy/init_ctx/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/init_ctx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/init_ctx/init_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.437256 colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/base_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.441256 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/reduce_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29011 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/sharded_model_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/zero_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.441256 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18665 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.441256 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_param/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_param/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_param/sharded_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_param/sharded_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.441256 colossalai-nightly-2023.4.8/colossalai/zero/low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/low_level/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.441256 colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/base_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/bucket_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/gradient_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25467 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/low_level/low_level_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.441256 colossalai-nightly-2023.4.8/colossalai_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24234 2023-04-08 00:13:40.000000 colossalai-nightly-2023.4.8/colossalai_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36286 2023-04-08 00:13:40.000000 colossalai-nightly-2023.4.8/colossalai_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 00:13:40.000000 colossalai-nightly-2023.4.8/colossalai_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-08 00:13:40.000000 colossalai-nightly-2023.4.8/colossalai_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-08 00:13:40.000000 colossalai-nightly-2023.4.8/colossalai_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-08 00:13:40.000000 colossalai-nightly-2023.4.8/colossalai_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.441256 colossalai-nightly-2023.4.8/op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/fused_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/multi_head_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/scaled_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/scaled_upper_triangle_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.441256 colossalai-nightly-2023.4.8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 00:13:40.453257 colossalai-nightly-2023.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.373252 colossalai-nightly-2023.4.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/components_to_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/albert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/beit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/hanging_param_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/inline_op_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/nested_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/repeated_computed_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/simple_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/components_to_test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/utils/dummy_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/utils/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/kit/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/kit/model_zoo/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/diffusers/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/kit/model_zoo/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/timm/timm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchaudio/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchaudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchaudio/torchaudio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchrec/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchrec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchrec/torchrec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchvision/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchvision/torchvision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/albert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/t5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/test_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_bias_addition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_mod_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_nested_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_shape_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_symbolic_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.449257 colossalai-nightly-2023.4.8/tests/test_analyzer/test_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_subclasses/test_aten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_subclasses/test_flop_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_subclasses/test_meta_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.449257 colossalai-nightly-2023.4.8/tests/test_auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.449257 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_pass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.449257 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.449257 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.453257 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/version.txt
```

### Comparing `colossalai-nightly-2023.4.29/LICENSE` & `colossalai-nightly-2023.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/PKG-INFO` & `colossalai-nightly-2023.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai-nightly
-Version: 2023.4.29
+Version: 2023.4.8
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
@@ -46,22 +46,14 @@
         * [2022/09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https://www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-fundraising-led-by-bluerun-ventures-in-the)
         
         ## Table of Contents
         <ul>
          <li><a href="#Why-Colossal-AI">Why Colossal-AI</a> </li>
          <li><a href="#Features">Features</a> </li>
          <li>
-           <a href="#Colossal-AI-in-the-Real-World">Colossal-AI for Real World Applications</a>
-           <ul>
-             <li><a href="#ColossalChat">ColossalChat: An Open-Source Solution for Cloning ChatGPT With a Complete RLHF Pipeline</a></li>
-             <li><a href="#AIGC">AIGC: Acceleration of Stable Diffusion</a></li>
-             <li><a href="#Biomedicine">Biomedicine: Acceleration of AlphaFold Protein Structure</a></li>
-           </ul>
-         </li>
-         <li>
            <a href="#Parallel-Training-Demo">Parallel Training Demo</a>
            <ul>
              <li><a href="#GPT-3">GPT-3</a></li>
              <li><a href="#GPT-2">GPT-2</a></li>
              <li><a href="#BERT">BERT</a></li>
              <li><a href="#PaLM">PaLM</a></li>
              <li><a href="#OPT">OPT</a></li>
@@ -80,14 +72,22 @@
            <a href="#Inference-Energon-AI-Demo">Inference (Energon-AI) Demo</a>
            <ul>
              <li><a href="#GPT-3-Inference">GPT-3</a></li>
              <li><a href="#OPT-Serving">OPT-175B Online Serving for Text Generation</a></li>
              <li><a href="#BLOOM-Inference">176B BLOOM</a></li>
            </ul>
          </li>
+           <li>
+           <a href="#Colossal-AI-in-the-Real-World">Colossal-AI for Real World Applications</a>
+           <ul>
+             <li><a href="#ColossalChat">ColossalChat: An Open-Source Solution for Cloning ChatGPT With a Complete RLHF Pipeline</a></li>
+             <li><a href="#AIGC">AIGC: Acceleration of Stable Diffusion</a></li>
+             <li><a href="#Biomedicine">Biomedicine: Acceleration of AlphaFold Protein Structure</a></li>
+           </ul>
+         </li>
          <li>
            <a href="#Installation">Installation</a>
            <ul>
              <li><a href="#PyPI">PyPI</a></li>
              <li><a href="#Install-From-Source">Install From Source</a></li>
            </ul>
          </li>
@@ -129,96 +129,14 @@
           - Parallelism based on the configuration file
         
         - Inference
           - [Energon-AI](https://github.com/hpcaitech/EnergonAI)
         
         <p align="right">(<a href="#top">back to top</a>)</p>
         
-        ## Colossal-AI in the Real World
-        
-        ### ColossalChat
-        
-        <div align="center">
-           <a href="https://chat.colossalai.org/">
-           <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Chat-demo.png" width="700" />
-           </a>
-        </div>
-        
-        [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://chat.colossalai.org)
-        
-        <p id="ColossalChat_scaling" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT%20scaling.png" width=800/>
-        </p>
-        
-        - Up to 7.73 times faster for single server training and 1.42 times faster for single-GPU inference
-        
-        <p id="ColossalChat-1GPU" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT-1GPU.jpg" width=450/>
-        </p>
-        
-        - Up to 10.3x growth in model capacity on one GPU
-        - A mini demo training process requires only 1.62GB of GPU memory (any consumer-grade GPU)
-        
-        <p id="ColossalChat-LoRA" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/LoRA%20data.jpg" width=600/>
-        </p>
-        
-        - Increase the capacity of the fine-tuning model by up to 3.7 times on a single GPU
-        - Keep at a sufficiently high running speed
-        
-        <p align="right">(<a href="#top">back to top</a>)</p>
-        
-        
-        ### AIGC
-        Acceleration of AIGC (AI-Generated Content) models such as [Stable Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable Diffusion v2](https://github.com/Stability-AI/stablediffusion).
-        <p id="diffusion_train" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20v2.png" width=800/>
-        </p>
-        
-        - [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and hardware cost by up to 46x (from A100 to RTX3060).
-        
-        <p id="diffusion_demo" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/DreamBooth.png" width=800/>
-        </p>
-        
-        - [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/dreambooth): Personalize your model using just 3-5 images of the desired subject.
-        
-        <p id="inference" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20Inference.jpg" width=800/>
-        </p>
-        
-        - [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce inference GPU memory consumption by 2.5x.
-        
-        
-        <p align="right">(<a href="#top">back to top</a>)</p>
-        
-        ### Biomedicine
-        Acceleration of [AlphaFold Protein Structure](https://alphafold.ebi.ac.uk/)
-        
-        <p id="FastFold" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/FastFold.jpg" width=800/>
-        </p>
-        
-        - [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and inference on GPU Clusters, faster data processing, inference sequence containing more than 10000 residues.
-        
-        <p id="FastFold-Intel" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/data%20preprocessing%20with%20Intel.jpg" width=600/>
-        </p>
-        
-        - [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference acceleration and 39% cost reduce.
-        
-        <p id="xTrimoMultimer" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/xTrimoMultimer_Table.jpg" width=800/>
-        </p>
-        
-        - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer): accelerating structure prediction of protein monomers and multimer by 11x.
-        
-        
-        <p align="right">(<a href="#top">back to top</a>)</p>
-        
         ## Parallel Training Demo
         
         ### GPT-3
         <p align="center">
         <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT3-v5.png" width=700/>
         </p>
         
@@ -304,22 +222,102 @@
         <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/BLOOM%20Inference.PNG" width=800/>
         </p>
         
         - [BLOOM](https://github.com/hpcaitech/EnergonAI/tree/main/examples/bloom): Reduce hardware deployment costs of 176-billion-parameter BLOOM by more than 10 times.
         
         <p align="right">(<a href="#top">back to top</a>)</p>
         
+        ## Colossal-AI in the Real World
+        
+        ### ColossalChat
+        
+        <div align="center">
+           <a href="https://chat.colossalai.org/">
+           <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Chat-demo.png" width="700" />
+           </a>
+        </div>
+        
+        [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://chat.colossalai.org)
+        
+        <p id="ColossalChat_scaling" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT%20scaling.png" width=800/>
+        </p>
+        
+        - Up to 7.73 times faster for single server training and 1.42 times faster for single-GPU inference
+        
+        <p id="ColossalChat-1GPU" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT-1GPU.jpg" width=450/>
+        </p>
+        
+        - Up to 10.3x growth in model capacity on one GPU
+        - A mini demo training process requires only 1.62GB of GPU memory (any consumer-grade GPU)
+        
+        <p id="ColossalChat-LoRA" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/LoRA%20data.jpg" width=600/>
+        </p>
+        
+        - Increase the capacity of the fine-tuning model by up to 3.7 times on a single GPU
+        - Keep at a sufficiently high running speed
+        
+        <p align="right">(<a href="#top">back to top</a>)</p>
+        
+        
+        ### AIGC
+        Acceleration of AIGC (AI-Generated Content) models such as [Stable Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable Diffusion v2](https://github.com/Stability-AI/stablediffusion).
+        <p id="diffusion_train" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20v2.png" width=800/>
+        </p>
+        
+        - [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and hardware cost by up to 46x (from A100 to RTX3060).
+        
+        <p id="diffusion_demo" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/DreamBooth.png" width=800/>
+        </p>
+        
+        - [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/dreambooth): Personalize your model using just 3-5 images of the desired subject.
+        
+        <p id="inference" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20Inference.jpg" width=800/>
+        </p>
+        
+        - [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce inference GPU memory consumption by 2.5x.
+        
+        
+        <p align="right">(<a href="#top">back to top</a>)</p>
+        
+        ### Biomedicine
+        Acceleration of [AlphaFold Protein Structure](https://alphafold.ebi.ac.uk/)
+        
+        <p id="FastFold" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/FastFold.jpg" width=800/>
+        </p>
+        
+        - [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and inference on GPU Clusters, faster data processing, inference sequence containing more than 10000 residues.
+        
+        <p id="FastFold-Intel" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/data%20preprocessing%20with%20Intel.jpg" width=600/>
+        </p>
+        
+        - [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference acceleration and 39% cost reduce.
+        
+        <p id="xTrimoMultimer" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/xTrimoMultimer_Table.jpg" width=800/>
+        </p>
+        
+        - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer): accelerating structure prediction of protein monomers and multimer by 11x.
+        
+        
+        <p align="right">(<a href="#top">back to top</a>)</p>
+        
         ## Installation
         
         Requirements:
         - PyTorch >= 1.11 (PyTorch 2.x in progress)
         - Python >= 3.7
         - CUDA >= 11.0
-        - [NVIDIA GPU Compute Capability](https://developer.nvidia.com/cuda-gpus) >= 7.0 (V100/RTX20 and higher)
-        - Linux OS
         
         If you encounter any problem with installation, you may want to raise an [issue](https://github.com/hpcaitech/ColossalAI/issues/new/choose) in this repository.
         
         ### Install from PyPI
         
         You can easily install Colossal-AI with the following command. **By default, we do not build PyTorch extensions during installation.**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.4.29 Summary: An
+Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.4.8 Summary: An
 integrated large-scale model training system with efficient parallelization
 techniques Home-page: https://www.colossalai.org License: Apache Software
 License 2.0 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/
 discussions Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/
 issues Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
@@ -45,19 +45,14 @@
 Sequence Exceeding 10,000](https://www.hpc-ai.tech/blog/use-a-laptop-to-
 analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding) * [2022/
 09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https:/
 /www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-
 fundraising-led-by-bluerun-ventures-in-the) ## Table of Contents
     * Why_Colossal-AI
     * Features
-    * Colossal-AI_for_Real_World_Applications
-          o ColossalChat:_An_Open-Source_Solution_for_Cloning_ChatGPT_With_a
-            Complete_RLHF_Pipeline
-          o AIGC:_Acceleration_of_Stable_Diffusion
-          o Biomedicine:_Acceleration_of_AlphaFold_Protein_Structure
     * Parallel_Training_Demo
           o GPT-3
           o GPT-2
           o BERT
           o PaLM
           o OPT
           o ViT
@@ -65,14 +60,19 @@
     * Single_GPU_Training_Demo
           o GPT-2
           o PaLM
     * Inference_(Energon-AI)_Demo
           o GPT-3
           o OPT-175B_Online_Serving_for_Text_Generation
           o 176B_BLOOM
+    * Colossal-AI_for_Real_World_Applications
+          o ColossalChat:_An_Open-Source_Solution_for_Cloning_ChatGPT_With_a
+            Complete_RLHF_Pipeline
+          o AIGC:_Acceleration_of_Stable_Diffusion
+          o Biomedicine:_Acceleration_of_AlphaFold_Protein_Structure
     * Installation
           o PyPI
           o Install_From_Source
     * Use_Docker
     * Community
     * Contributing
     * Cite_Us
@@ -91,71 +91,14 @@
 (https://arxiv.org/abs/2105.13120) - [Zero Redundancy Optimizer (ZeRO)](https:/
 /arxiv.org/abs/1910.02054) - [Auto-Parallelism](https://arxiv.org/abs/
 2302.02599) - Heterogeneous Memory Management - [PatrickStar](https://
 arxiv.org/abs/2108.05818) - Friendly Usage - Parallelism based on the
 configuration file - Inference - [Energon-AI](https://github.com/hpcaitech/
 EnergonAI)
                                                                   (back_to_top)
-## Colossal-AI in the Real World ### ColossalChat
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                Chat-demo.png]
-[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/
-Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/
-chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/
-ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/
-@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://
-chat.colossalai.org)
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                        chatgpt/ChatGPT%20scaling.png]
-- Up to 7.73 times faster for single server training and 1.42 times faster for
-single-GPU inference
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                           chatgpt/ChatGPT-1GPU.jpg]
-- Up to 10.3x growth in model capacity on one GPU - A mini demo training
-process requires only 1.62GB of GPU memory (any consumer-grade GPU)
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                           chatgpt/LoRA%20data.jpg]
-- Increase the capacity of the fine-tuning model by up to 3.7 times on a single
-GPU - Keep at a sufficiently high running speed
-                                                                  (back_to_top)
-### AIGC Acceleration of AIGC (AI-Generated Content) models such as [Stable
-Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable
-Diffusion v2](https://github.com/Stability-AI/stablediffusion).
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                         Stable%20Diffusion%20v2.png]
-- [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/
-diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and
-hardware cost by up to 46x (from A100 to RTX3060).
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                DreamBooth.png]
-- [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/
-examples/images/dreambooth): Personalize your model using just 3-5 images of
-the desired subject.
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                      Stable%20Diffusion%20Inference.jpg]
-- [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/
-images/diffusion): Reduce inference GPU memory consumption by 2.5x.
-                                                                  (back_to_top)
-### Biomedicine Acceleration of [AlphaFold Protein Structure](https://
-alphafold.ebi.ac.uk/)
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                 FastFold.jpg]
-- [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and
-inference on GPU Clusters, faster data processing, inference sequence
-containing more than 10000 residues.
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                   data%20preprocessing%20with%20Intel.jpg]
-- [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference
-acceleration and 39% cost reduce.
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                           xTrimoMultimer_Table.jpg]
-- [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer):
-accelerating structure prediction of protein monomers and multimer by 11x.
-                                                                  (back_to_top)
 ## Parallel Training Demo ### GPT-3
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                                  GPT3-v5.png]
 - Save 50% GPU resources and 10.7% acceleration ### GPT-2 [https://
 raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT2.png]
 - 11x lower GPU memory consumption, and superlinear scaling efficiency with
 Tensor Parallelism [https://raw.githubusercontent.com/hpcaitech/public_assets/
@@ -205,35 +148,91 @@
 Try 175-billion-parameter OPT online services
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                             BLOOM%20Inference.PNG]
 - [BLOOM](https://github.com/hpcaitech/EnergonAI/tree/main/examples/bloom):
 Reduce hardware deployment costs of 176-billion-parameter BLOOM by more than 10
 times.
                                                                   (back_to_top)
+## Colossal-AI in the Real World ### ColossalChat
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                Chat-demo.png]
+[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/
+Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/
+chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/
+ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/
+@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
+with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://
+chat.colossalai.org)
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                        chatgpt/ChatGPT%20scaling.png]
+- Up to 7.73 times faster for single server training and 1.42 times faster for
+single-GPU inference
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                           chatgpt/ChatGPT-1GPU.jpg]
+- Up to 10.3x growth in model capacity on one GPU - A mini demo training
+process requires only 1.62GB of GPU memory (any consumer-grade GPU)
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                           chatgpt/LoRA%20data.jpg]
+- Increase the capacity of the fine-tuning model by up to 3.7 times on a single
+GPU - Keep at a sufficiently high running speed
+                                                                  (back_to_top)
+### AIGC Acceleration of AIGC (AI-Generated Content) models such as [Stable
+Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable
+Diffusion v2](https://github.com/Stability-AI/stablediffusion).
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                         Stable%20Diffusion%20v2.png]
+- [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/
+diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and
+hardware cost by up to 46x (from A100 to RTX3060).
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                DreamBooth.png]
+- [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/
+examples/images/dreambooth): Personalize your model using just 3-5 images of
+the desired subject.
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                      Stable%20Diffusion%20Inference.jpg]
+- [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/
+images/diffusion): Reduce inference GPU memory consumption by 2.5x.
+                                                                  (back_to_top)
+### Biomedicine Acceleration of [AlphaFold Protein Structure](https://
+alphafold.ebi.ac.uk/)
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                 FastFold.jpg]
+- [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and
+inference on GPU Clusters, faster data processing, inference sequence
+containing more than 10000 residues.
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                   data%20preprocessing%20with%20Intel.jpg]
+- [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference
+acceleration and 39% cost reduce.
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                           xTrimoMultimer_Table.jpg]
+- [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer):
+accelerating structure prediction of protein monomers and multimer by 11x.
+                                                                  (back_to_top)
 ## Installation Requirements: - PyTorch >= 1.11 (PyTorch 2.x in progress) -
-Python >= 3.7 - CUDA >= 11.0 - [NVIDIA GPU Compute Capability](https://
-developer.nvidia.com/cuda-gpus) >= 7.0 (V100/RTX20 and higher) - Linux OS If
-you encounter any problem with installation, you may want to raise an [issue]
-(https://github.com/hpcaitech/ColossalAI/issues/new/choose) in this repository.
-### Install from PyPI You can easily install Colossal-AI with the following
-command. **By default, we do not build PyTorch extensions during
-installation.** ```bash pip install colossalai ``` **Note: only Linux is
-supported for now.** However, if you want to build the PyTorch extensions
-during installation, you can set `CUDA_EXT=1`. ```bash CUDA_EXT=1 pip install
-colossalai ``` **Otherwise, CUDA kernels will be built during runtime when you
-actually need them.** We also keep releasing the nightly version to PyPI every
-week. This allows you to access the unreleased features and bug fixes in the
-main branch. Installation can be made via ```bash pip install colossalai-
-nightly ``` ### Download From Source > The version of Colossal-AI will be in
-line with the main branch of the repository. Feel free to raise an issue if you
-encounter any problems. :) ```shell git clone https://github.com/hpcaitech/
-ColossalAI.git cd ColossalAI # install colossalai pip install . ``` By default,
-we do not compile CUDA/C++ kernels. ColossalAI will build them during runtime.
-If you want to install and enable CUDA kernel fusion (compulsory installation
-when using fused optimizer): ```shell CUDA_EXT=1 pip install . ```
+Python >= 3.7 - CUDA >= 11.0 If you encounter any problem with installation,
+you may want to raise an [issue](https://github.com/hpcaitech/ColossalAI/
+issues/new/choose) in this repository. ### Install from PyPI You can easily
+install Colossal-AI with the following command. **By default, we do not build
+PyTorch extensions during installation.** ```bash pip install colossalai ```
+**Note: only Linux is supported for now.** However, if you want to build the
+PyTorch extensions during installation, you can set `CUDA_EXT=1`. ```bash
+CUDA_EXT=1 pip install colossalai ``` **Otherwise, CUDA kernels will be built
+during runtime when you actually need them.** We also keep releasing the
+nightly version to PyPI every week. This allows you to access the unreleased
+features and bug fixes in the main branch. Installation can be made via ```bash
+pip install colossalai-nightly ``` ### Download From Source > The version of
+Colossal-AI will be in line with the main branch of the repository. Feel free
+to raise an issue if you encounter any problems. :) ```shell git clone https://
+github.com/hpcaitech/ColossalAI.git cd ColossalAI # install colossalai pip
+install . ``` By default, we do not compile CUDA/C++ kernels. ColossalAI will
+build them during runtime. If you want to install and enable CUDA kernel fusion
+(compulsory installation when using fused optimizer): ```shell CUDA_EXT=1 pip
+install . ```
                                                                   (back_to_top)
 ## Use Docker ### Pull from DockerHub You can directly pull the docker image
 from our [DockerHub page](https://hub.docker.com/r/hpcaitech/colossalai). The
 image is automatically uploaded upon release. ### Build On Your Own Run the
 following command to build a docker image from Dockerfile provided. > Building
 Colossal-AI from scratch requires GPU support, you need to use Nvidia Docker
 Runtime as the default when doing `docker build`. More details can be found
```

### Comparing `colossalai-nightly-2023.4.29/README.md` & `colossalai-nightly-2023.4.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,22 +35,14 @@
 * [2022/09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https://www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-fundraising-led-by-bluerun-ventures-in-the)
 
 ## Table of Contents
 <ul>
  <li><a href="#Why-Colossal-AI">Why Colossal-AI</a> </li>
  <li><a href="#Features">Features</a> </li>
  <li>
-   <a href="#Colossal-AI-in-the-Real-World">Colossal-AI for Real World Applications</a>
-   <ul>
-     <li><a href="#ColossalChat">ColossalChat: An Open-Source Solution for Cloning ChatGPT With a Complete RLHF Pipeline</a></li>
-     <li><a href="#AIGC">AIGC: Acceleration of Stable Diffusion</a></li>
-     <li><a href="#Biomedicine">Biomedicine: Acceleration of AlphaFold Protein Structure</a></li>
-   </ul>
- </li>
- <li>
    <a href="#Parallel-Training-Demo">Parallel Training Demo</a>
    <ul>
      <li><a href="#GPT-3">GPT-3</a></li>
      <li><a href="#GPT-2">GPT-2</a></li>
      <li><a href="#BERT">BERT</a></li>
      <li><a href="#PaLM">PaLM</a></li>
      <li><a href="#OPT">OPT</a></li>
@@ -69,14 +61,22 @@
    <a href="#Inference-Energon-AI-Demo">Inference (Energon-AI) Demo</a>
    <ul>
      <li><a href="#GPT-3-Inference">GPT-3</a></li>
      <li><a href="#OPT-Serving">OPT-175B Online Serving for Text Generation</a></li>
      <li><a href="#BLOOM-Inference">176B BLOOM</a></li>
    </ul>
  </li>
+   <li>
+   <a href="#Colossal-AI-in-the-Real-World">Colossal-AI for Real World Applications</a>
+   <ul>
+     <li><a href="#ColossalChat">ColossalChat: An Open-Source Solution for Cloning ChatGPT With a Complete RLHF Pipeline</a></li>
+     <li><a href="#AIGC">AIGC: Acceleration of Stable Diffusion</a></li>
+     <li><a href="#Biomedicine">Biomedicine: Acceleration of AlphaFold Protein Structure</a></li>
+   </ul>
+ </li>
  <li>
    <a href="#Installation">Installation</a>
    <ul>
      <li><a href="#PyPI">PyPI</a></li>
      <li><a href="#Install-From-Source">Install From Source</a></li>
    </ul>
  </li>
@@ -118,96 +118,14 @@
   - Parallelism based on the configuration file
 
 - Inference
   - [Energon-AI](https://github.com/hpcaitech/EnergonAI)
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
-## Colossal-AI in the Real World
-
-### ColossalChat
-
-<div align="center">
-   <a href="https://chat.colossalai.org/">
-   <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Chat-demo.png" width="700" />
-   </a>
-</div>
-
-[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://chat.colossalai.org)
-
-<p id="ColossalChat_scaling" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT%20scaling.png" width=800/>
-</p>
-
-- Up to 7.73 times faster for single server training and 1.42 times faster for single-GPU inference
-
-<p id="ColossalChat-1GPU" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT-1GPU.jpg" width=450/>
-</p>
-
-- Up to 10.3x growth in model capacity on one GPU
-- A mini demo training process requires only 1.62GB of GPU memory (any consumer-grade GPU)
-
-<p id="ColossalChat-LoRA" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/LoRA%20data.jpg" width=600/>
-</p>
-
-- Increase the capacity of the fine-tuning model by up to 3.7 times on a single GPU
-- Keep at a sufficiently high running speed
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-
-### AIGC
-Acceleration of AIGC (AI-Generated Content) models such as [Stable Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable Diffusion v2](https://github.com/Stability-AI/stablediffusion).
-<p id="diffusion_train" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20v2.png" width=800/>
-</p>
-
-- [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and hardware cost by up to 46x (from A100 to RTX3060).
-
-<p id="diffusion_demo" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/DreamBooth.png" width=800/>
-</p>
-
-- [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/dreambooth): Personalize your model using just 3-5 images of the desired subject.
-
-<p id="inference" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20Inference.jpg" width=800/>
-</p>
-
-- [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce inference GPU memory consumption by 2.5x.
-
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-### Biomedicine
-Acceleration of [AlphaFold Protein Structure](https://alphafold.ebi.ac.uk/)
-
-<p id="FastFold" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/FastFold.jpg" width=800/>
-</p>
-
-- [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and inference on GPU Clusters, faster data processing, inference sequence containing more than 10000 residues.
-
-<p id="FastFold-Intel" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/data%20preprocessing%20with%20Intel.jpg" width=600/>
-</p>
-
-- [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference acceleration and 39% cost reduce.
-
-<p id="xTrimoMultimer" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/xTrimoMultimer_Table.jpg" width=800/>
-</p>
-
-- [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer): accelerating structure prediction of protein monomers and multimer by 11x.
-
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
 ## Parallel Training Demo
 
 ### GPT-3
 <p align="center">
 <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT3-v5.png" width=700/>
 </p>
 
@@ -293,22 +211,102 @@
 <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/BLOOM%20Inference.PNG" width=800/>
 </p>
 
 - [BLOOM](https://github.com/hpcaitech/EnergonAI/tree/main/examples/bloom): Reduce hardware deployment costs of 176-billion-parameter BLOOM by more than 10 times.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
+## Colossal-AI in the Real World
+
+### ColossalChat
+
+<div align="center">
+   <a href="https://chat.colossalai.org/">
+   <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Chat-demo.png" width="700" />
+   </a>
+</div>
+
+[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://chat.colossalai.org)
+
+<p id="ColossalChat_scaling" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT%20scaling.png" width=800/>
+</p>
+
+- Up to 7.73 times faster for single server training and 1.42 times faster for single-GPU inference
+
+<p id="ColossalChat-1GPU" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT-1GPU.jpg" width=450/>
+</p>
+
+- Up to 10.3x growth in model capacity on one GPU
+- A mini demo training process requires only 1.62GB of GPU memory (any consumer-grade GPU)
+
+<p id="ColossalChat-LoRA" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/LoRA%20data.jpg" width=600/>
+</p>
+
+- Increase the capacity of the fine-tuning model by up to 3.7 times on a single GPU
+- Keep at a sufficiently high running speed
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+
+### AIGC
+Acceleration of AIGC (AI-Generated Content) models such as [Stable Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable Diffusion v2](https://github.com/Stability-AI/stablediffusion).
+<p id="diffusion_train" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20v2.png" width=800/>
+</p>
+
+- [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and hardware cost by up to 46x (from A100 to RTX3060).
+
+<p id="diffusion_demo" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/DreamBooth.png" width=800/>
+</p>
+
+- [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/dreambooth): Personalize your model using just 3-5 images of the desired subject.
+
+<p id="inference" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20Inference.jpg" width=800/>
+</p>
+
+- [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce inference GPU memory consumption by 2.5x.
+
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+### Biomedicine
+Acceleration of [AlphaFold Protein Structure](https://alphafold.ebi.ac.uk/)
+
+<p id="FastFold" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/FastFold.jpg" width=800/>
+</p>
+
+- [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and inference on GPU Clusters, faster data processing, inference sequence containing more than 10000 residues.
+
+<p id="FastFold-Intel" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/data%20preprocessing%20with%20Intel.jpg" width=600/>
+</p>
+
+- [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference acceleration and 39% cost reduce.
+
+<p id="xTrimoMultimer" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/xTrimoMultimer_Table.jpg" width=800/>
+</p>
+
+- [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer): accelerating structure prediction of protein monomers and multimer by 11x.
+
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
 ## Installation
 
 Requirements:
 - PyTorch >= 1.11 (PyTorch 2.x in progress)
 - Python >= 3.7
 - CUDA >= 11.0
-- [NVIDIA GPU Compute Capability](https://developer.nvidia.com/cuda-gpus) >= 7.0 (V100/RTX20 and higher)
-- Linux OS
 
 If you encounter any problem with installation, you may want to raise an [issue](https://github.com/hpcaitech/ColossalAI/issues/new/choose) in this repository.
 
 ### Install from PyPI
 
 You can easily install Colossal-AI with the following command. **By default, we do not build PyTorch extensions during installation.**
```

#### html2text {}

```diff
@@ -38,19 +38,14 @@
 Sequence Exceeding 10,000](https://www.hpc-ai.tech/blog/use-a-laptop-to-
 analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding) * [2022/
 09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https:/
 /www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-
 fundraising-led-by-bluerun-ventures-in-the) ## Table of Contents
     * Why_Colossal-AI
     * Features
-    * Colossal-AI_for_Real_World_Applications
-          o ColossalChat:_An_Open-Source_Solution_for_Cloning_ChatGPT_With_a
-            Complete_RLHF_Pipeline
-          o AIGC:_Acceleration_of_Stable_Diffusion
-          o Biomedicine:_Acceleration_of_AlphaFold_Protein_Structure
     * Parallel_Training_Demo
           o GPT-3
           o GPT-2
           o BERT
           o PaLM
           o OPT
           o ViT
@@ -58,14 +53,19 @@
     * Single_GPU_Training_Demo
           o GPT-2
           o PaLM
     * Inference_(Energon-AI)_Demo
           o GPT-3
           o OPT-175B_Online_Serving_for_Text_Generation
           o 176B_BLOOM
+    * Colossal-AI_for_Real_World_Applications
+          o ColossalChat:_An_Open-Source_Solution_for_Cloning_ChatGPT_With_a
+            Complete_RLHF_Pipeline
+          o AIGC:_Acceleration_of_Stable_Diffusion
+          o Biomedicine:_Acceleration_of_AlphaFold_Protein_Structure
     * Installation
           o PyPI
           o Install_From_Source
     * Use_Docker
     * Community
     * Contributing
     * Cite_Us
@@ -84,71 +84,14 @@
 (https://arxiv.org/abs/2105.13120) - [Zero Redundancy Optimizer (ZeRO)](https:/
 /arxiv.org/abs/1910.02054) - [Auto-Parallelism](https://arxiv.org/abs/
 2302.02599) - Heterogeneous Memory Management - [PatrickStar](https://
 arxiv.org/abs/2108.05818) - Friendly Usage - Parallelism based on the
 configuration file - Inference - [Energon-AI](https://github.com/hpcaitech/
 EnergonAI)
                                                                   (back_to_top)
-## Colossal-AI in the Real World ### ColossalChat
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                Chat-demo.png]
-[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/
-Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/
-chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/
-ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/
-@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://
-chat.colossalai.org)
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                        chatgpt/ChatGPT%20scaling.png]
-- Up to 7.73 times faster for single server training and 1.42 times faster for
-single-GPU inference
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                           chatgpt/ChatGPT-1GPU.jpg]
-- Up to 10.3x growth in model capacity on one GPU - A mini demo training
-process requires only 1.62GB of GPU memory (any consumer-grade GPU)
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                           chatgpt/LoRA%20data.jpg]
-- Increase the capacity of the fine-tuning model by up to 3.7 times on a single
-GPU - Keep at a sufficiently high running speed
-                                                                  (back_to_top)
-### AIGC Acceleration of AIGC (AI-Generated Content) models such as [Stable
-Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable
-Diffusion v2](https://github.com/Stability-AI/stablediffusion).
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                         Stable%20Diffusion%20v2.png]
-- [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/
-diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and
-hardware cost by up to 46x (from A100 to RTX3060).
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                DreamBooth.png]
-- [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/
-examples/images/dreambooth): Personalize your model using just 3-5 images of
-the desired subject.
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                      Stable%20Diffusion%20Inference.jpg]
-- [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/
-images/diffusion): Reduce inference GPU memory consumption by 2.5x.
-                                                                  (back_to_top)
-### Biomedicine Acceleration of [AlphaFold Protein Structure](https://
-alphafold.ebi.ac.uk/)
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                 FastFold.jpg]
-- [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and
-inference on GPU Clusters, faster data processing, inference sequence
-containing more than 10000 residues.
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                   data%20preprocessing%20with%20Intel.jpg]
-- [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference
-acceleration and 39% cost reduce.
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                           xTrimoMultimer_Table.jpg]
-- [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer):
-accelerating structure prediction of protein monomers and multimer by 11x.
-                                                                  (back_to_top)
 ## Parallel Training Demo ### GPT-3
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                                  GPT3-v5.png]
 - Save 50% GPU resources and 10.7% acceleration ### GPT-2 [https://
 raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT2.png]
 - 11x lower GPU memory consumption, and superlinear scaling efficiency with
 Tensor Parallelism [https://raw.githubusercontent.com/hpcaitech/public_assets/
@@ -198,35 +141,91 @@
 Try 175-billion-parameter OPT online services
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                             BLOOM%20Inference.PNG]
 - [BLOOM](https://github.com/hpcaitech/EnergonAI/tree/main/examples/bloom):
 Reduce hardware deployment costs of 176-billion-parameter BLOOM by more than 10
 times.
                                                                   (back_to_top)
+## Colossal-AI in the Real World ### ColossalChat
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                Chat-demo.png]
+[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/
+Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/
+chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/
+ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/
+@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
+with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://
+chat.colossalai.org)
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                        chatgpt/ChatGPT%20scaling.png]
+- Up to 7.73 times faster for single server training and 1.42 times faster for
+single-GPU inference
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                           chatgpt/ChatGPT-1GPU.jpg]
+- Up to 10.3x growth in model capacity on one GPU - A mini demo training
+process requires only 1.62GB of GPU memory (any consumer-grade GPU)
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                           chatgpt/LoRA%20data.jpg]
+- Increase the capacity of the fine-tuning model by up to 3.7 times on a single
+GPU - Keep at a sufficiently high running speed
+                                                                  (back_to_top)
+### AIGC Acceleration of AIGC (AI-Generated Content) models such as [Stable
+Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable
+Diffusion v2](https://github.com/Stability-AI/stablediffusion).
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                         Stable%20Diffusion%20v2.png]
+- [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/
+diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and
+hardware cost by up to 46x (from A100 to RTX3060).
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                DreamBooth.png]
+- [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/
+examples/images/dreambooth): Personalize your model using just 3-5 images of
+the desired subject.
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                      Stable%20Diffusion%20Inference.jpg]
+- [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/
+images/diffusion): Reduce inference GPU memory consumption by 2.5x.
+                                                                  (back_to_top)
+### Biomedicine Acceleration of [AlphaFold Protein Structure](https://
+alphafold.ebi.ac.uk/)
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                 FastFold.jpg]
+- [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and
+inference on GPU Clusters, faster data processing, inference sequence
+containing more than 10000 residues.
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                   data%20preprocessing%20with%20Intel.jpg]
+- [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference
+acceleration and 39% cost reduce.
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                           xTrimoMultimer_Table.jpg]
+- [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer):
+accelerating structure prediction of protein monomers and multimer by 11x.
+                                                                  (back_to_top)
 ## Installation Requirements: - PyTorch >= 1.11 (PyTorch 2.x in progress) -
-Python >= 3.7 - CUDA >= 11.0 - [NVIDIA GPU Compute Capability](https://
-developer.nvidia.com/cuda-gpus) >= 7.0 (V100/RTX20 and higher) - Linux OS If
-you encounter any problem with installation, you may want to raise an [issue]
-(https://github.com/hpcaitech/ColossalAI/issues/new/choose) in this repository.
-### Install from PyPI You can easily install Colossal-AI with the following
-command. **By default, we do not build PyTorch extensions during
-installation.** ```bash pip install colossalai ``` **Note: only Linux is
-supported for now.** However, if you want to build the PyTorch extensions
-during installation, you can set `CUDA_EXT=1`. ```bash CUDA_EXT=1 pip install
-colossalai ``` **Otherwise, CUDA kernels will be built during runtime when you
-actually need them.** We also keep releasing the nightly version to PyPI every
-week. This allows you to access the unreleased features and bug fixes in the
-main branch. Installation can be made via ```bash pip install colossalai-
-nightly ``` ### Download From Source > The version of Colossal-AI will be in
-line with the main branch of the repository. Feel free to raise an issue if you
-encounter any problems. :) ```shell git clone https://github.com/hpcaitech/
-ColossalAI.git cd ColossalAI # install colossalai pip install . ``` By default,
-we do not compile CUDA/C++ kernels. ColossalAI will build them during runtime.
-If you want to install and enable CUDA kernel fusion (compulsory installation
-when using fused optimizer): ```shell CUDA_EXT=1 pip install . ```
+Python >= 3.7 - CUDA >= 11.0 If you encounter any problem with installation,
+you may want to raise an [issue](https://github.com/hpcaitech/ColossalAI/
+issues/new/choose) in this repository. ### Install from PyPI You can easily
+install Colossal-AI with the following command. **By default, we do not build
+PyTorch extensions during installation.** ```bash pip install colossalai ```
+**Note: only Linux is supported for now.** However, if you want to build the
+PyTorch extensions during installation, you can set `CUDA_EXT=1`. ```bash
+CUDA_EXT=1 pip install colossalai ``` **Otherwise, CUDA kernels will be built
+during runtime when you actually need them.** We also keep releasing the
+nightly version to PyPI every week. This allows you to access the unreleased
+features and bug fixes in the main branch. Installation can be made via ```bash
+pip install colossalai-nightly ``` ### Download From Source > The version of
+Colossal-AI will be in line with the main branch of the repository. Feel free
+to raise an issue if you encounter any problems. :) ```shell git clone https://
+github.com/hpcaitech/ColossalAI.git cd ColossalAI # install colossalai pip
+install . ``` By default, we do not compile CUDA/C++ kernels. ColossalAI will
+build them during runtime. If you want to install and enable CUDA kernel fusion
+(compulsory installation when using fused optimizer): ```shell CUDA_EXT=1 pip
+install . ```
                                                                   (back_to_top)
 ## Use Docker ### Pull from DockerHub You can directly pull the docker image
 from our [DockerHub page](https://hub.docker.com/r/hpcaitech/colossalai). The
 image is automatically uploaded upon release. ### Build On Your Own Run the
 following command to build a docker image from Dockerfile provided. > Building
 Colossal-AI from scratch requires GPU support, you need to use Nvidia Docker
 Runtime as the default when doing `docker build`. More details can be found
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/amp/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/amp/apex_amp/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/amp/apex_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/amp/apex_amp/apex_amp.py` & `colossalai-nightly-2023.4.8/colossalai/amp/apex_amp/apex_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/amp/naive_amp/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/amp/naive_amp/_fp16_optimizer.py` & `colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/_fp16_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/amp/naive_amp/_utils.py` & `colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py` & `colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py` & `colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py` & `colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/amp/naive_amp/naive_amp.py` & `colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/naive_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/amp/torch_amp/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/amp/torch_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/amp/torch_amp/_grad_scaler.py` & `colossalai-nightly-2023.4.8/colossalai/amp/torch_amp/_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/amp/torch_amp/torch_amp.py` & `colossalai-nightly-2023.4.8/colossalai/amp/torch_amp/torch_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/checkpoint/operation.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/meta_registry/where.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/where.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/registry.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/meta_profiler/shard_metainfo.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/shard_metainfo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/amp_optimizer.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/amp_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/base_offload_module.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/base_offload_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/mem_optimize.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/mem_optimize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/region.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/region.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         # torch.cuda.empty_cache()
 
     def copy_grad_to_region_slice(self, param: torch.nn.Parameter, data_slice: torch.Tensor) -> None:
         """
         Copy data slice to the memory space indexed by the input tensor in the region.
 
         Args:
-            param (torch.nn.Parameter): the param used to retrieve meta information
+            param (torch.nn.Parameter): the param used to retrive meta information
             data_slice (torch.Tensor): the tensor to be copied to the region
         """
 
         begin, end = self.param_to_range[param]
         self.fp16_data[begin:end].copy_(data_slice.data.flatten())
         param.data = self.fp16_data[begin:end].view(param.data.shape)
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/region_manager.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/region_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/runtime.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/runtime.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/solver.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/solver.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/training_simulator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/training_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class TrainingSimulator(ABC):
     """
     The Training Simulator is used to simulate the training process.
     It records computation, communication, and runtime memory during forward and backward passes.
 
     Args:
         region_list (List[Region]): represents the linearized DNN computing graph.
-        comp_power (float): the NVIDIA GPU FP16 computing power.
+        comp_power (float): the NVIDIA GPU FP16 compuing power.
         link_to_bw (Dict[str, Dict[float, float]]): communication links and the corresponding bandwidth.
     """
 
     def __init__(self,
                  region_list: List[Region],
                  comp_power: float,
                  link_to_bw: Dict[str, Dict[float, float]]) -> None:
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/offload/util.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/util.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/passes/comm_metainfo_pass.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/comm_metainfo_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/passes/meta_info_prop.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/meta_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/passes/runtime_apply_pass.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/runtime_apply_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/passes/runtime_preparation_pass.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/runtime_preparation_pass.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     # DeviceMesh information instructs the scaling of the size value
     device_mesh_info = {}
     for dim, dim_size in enumerate(device_mesh.mesh_shape):
         device_mesh_info[dim] = dim_size
 
     def _extract_target_dim(node):
         '''
-        A helper function to extract the target dimension from size node.
+        A helper function to etract the target dimension from size node.
         There are two usages of torch.Tensor.size:
         1. tensor.size()
         2. tensor.size(dim)
 
         If a target_dim is assigned, then the output will be in type of int, instead of torch.Size.
         Otherwise, the output will be in type of torch.Size and this function will return None.
         '''
@@ -423,15 +423,15 @@
                 wrapper(param, comm_spec_to_use, reduction_stream, overlap=overlap)
 
     def _shard_param(param, target_sharding_spec):
         # apply the sharding spec of parameters
         if target_sharding_spec.dim_partition_dict != {}:
             origin_sharding_spec = ShardingSpec(device_mesh, param.shape, {})
             setattr(param, 'sharding_spec', origin_sharding_spec)
-            # TODO: build a ColoParameter class to manager the distributed parameters
+            # TODO: build a ColoParamter class to manager the distributed parameters
             # we could use .data here, because all the operations just happen before the real training
             # loop, so we don't need to track these operations in the autograd graph.
             param = torch.nn.Parameter(
                 shape_consistency_manager.apply_for_autoparallel_runtime(param.data, param.sharding_spec,
                                                                          target_sharding_spec).detach().clone())
         return param
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/constants.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/initialize.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/registry.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/options.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/options.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/sharding_strategy.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/sharding_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/solver/solver.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/solver.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/utils/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/utils/broadcast.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/broadcast.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/utils/factory.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/factory.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/utils/misc.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/misc.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/utils/reshape.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/reshape.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/auto_parallel/tensor_shard/utils/sharding.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/sharding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/booster/accelerator.py` & `colossalai-nightly-2023.4.8/colossalai/booster/accelerator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/booster/booster.py` & `colossalai-nightly-2023.4.8/colossalai/booster/booster.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 __all__ = ['Booster']
 
 
 class Booster:
     """
     Booster is a high-level API for training neural networks. It provides a unified interface for
-    training with different precision, accelerator, and plugin.
+    training with different precisio, accelerator, and plugin.
 
     Examples:
         >>> colossalai.launch(...)
         >>> plugin = GeminiPlugin(stage=3, ...)
         >>> booster = Booster(precision='fp16', plugin=plugin)
         >>>
         >>> model = GPT2()
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/booster/mixed_precision/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/booster/mixed_precision/fp16_torch.py` & `colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/fp16_torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/booster/mixed_precision/mixed_precision_base.py` & `colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/mixed_precision_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/booster/plugin/gemini_plugin.py` & `colossalai-nightly-2023.4.8/colossalai/booster/plugin/gemini_plugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,23 +12,69 @@
 from torch.utils.data import DataLoader
 from torch.utils.data.distributed import DistributedSampler
 
 from colossalai.checkpoint_io import CheckpointIO, GeneralCheckpointIO
 from colossalai.checkpoint_io.utils import save_state_dict
 from colossalai.cluster import DistCoordinator
 from colossalai.interface import ModelWrapper, OptimizerWrapper
+from colossalai.tensor.colo_parameter import ColoParameter
 from colossalai.utils import get_current_device
 from colossalai.zero import GeminiDDP, zero_model_wrapper, zero_optim_wrapper
+from colossalai.zero.gemini.colo_init_context import _convert_to_coloparam
 from colossalai.zero.gemini.memory_tracer import MemStats
 
 from .plugin_base import Plugin
 
 __all__ = ['GeminiPlugin']
 
 
+def convert_to_colo_param(module: nn.Module) -> None:
+    """Convert module's paramters to ColoParameter. This is a workaround and will be deprecated when lazy init is compatible with Gemini.
+
+    Args:
+        module (nn.Module): Module to be converted.
+    """
+    converted_modules = set()    # handle shared modules
+    converted_params = dict()    # record mapping between (torch.Tensor, ColoTensor) to distinguish the same reference
+
+    def convert_recursively(m: nn.Module):
+        for child in m.children():
+            if child not in converted_modules:
+                converted_modules.add(child)
+                convert_recursively(child)
+
+        for name, p in m.named_parameters(recurse=False):
+            assert not isinstance(p, ColoParameter)
+            if p in converted_params:
+                target = converted_params[p]
+            else:
+                target = _convert_to_coloparam(p, p.device, p.dtype)
+                converted_params[p] = target
+            setattr(m, name, target)
+            target.shared_param_modules.append(m)
+
+    convert_recursively(module)
+
+    # optimizer should replace params in group as well. This attr should be deleted after replacing to avoid memory leak
+    module._converted_params = converted_params
+
+
+def replace_param_in_group(optimizer: Optimizer, converted_params: dict) -> None:
+    """Replace param in optimizer's group with converted ColoParameter.
+
+    Args:
+        optimizer (Optimizer): Optimizer to be replaced.
+        converted_params (dict): Mapping between (torch.Tensor, ColoTensor).
+    """
+    for group in optimizer.param_groups:
+        for i, p in enumerate(group['params']):
+            if p in converted_params:
+                group['params'][i] = converted_params[p]
+
+
 class GeminiCheckpointIO(GeneralCheckpointIO):
 
     def __init__(self) -> None:
         super().__init__()
         self.coordinator = DistCoordinator()
 
     def load_unsharded_model(self, model: GeminiDDP, checkpoint: str, strict: bool = True):
@@ -61,36 +107,31 @@
         """
         if self.coordinator.is_master():
             super().save_lr_scheduler(lr_scheduler, checkpoint)
 
 
 class GeminiModel(ModelWrapper):
 
-    def __init__(self, module: nn.Module, gemini_config: dict, verbose: bool = False) -> None:
+    def __init__(self, module: nn.Module, gemini_config: dict) -> None:
         super().__init__(module)
-        self.module = zero_model_wrapper(module, zero_stage=3, gemini_config=gemini_config, verbose=verbose)
+        # TODO(ver217): only support Gemini now
+        convert_to_colo_param(module)
+        self.module = zero_model_wrapper(module, zero_stage=3, gemini_config=gemini_config)
 
     def unwrap(self):
         # as save/load state dict is coupled with the GeminiDDP, we only return GeminiDDP model
         return self.module
 
 
 class GeminiOptimizer(OptimizerWrapper):
 
-    def __init__(self,
-                 module: GeminiDDP,
-                 optimizer: Optimizer,
-                 zero_optim_config: dict,
-                 optim_kwargs: dict,
-                 verbose: bool = False) -> None:
-        optimizer = zero_optim_wrapper(module,
-                                       optimizer,
-                                       optim_config=zero_optim_config,
-                                       **optim_kwargs,
-                                       verbose=verbose)
+    def __init__(self, module: GeminiDDP, optimizer: Optimizer, zero_optim_config: dict, optim_kwargs: dict) -> None:
+        replace_param_in_group(optimizer, module.module._converted_params)
+        del module.module._converted_params
+        optimizer = zero_optim_wrapper(module, optimizer, optim_config=zero_optim_config, **optim_kwargs)
         super().__init__(optimizer)
 
     def backward(self, loss: Tensor, *args, **kwargs):
         self.optim.backward(loss)
 
     def clip_grad_by_norm(self,
                           max_norm: Union[float, int],
@@ -143,15 +184,14 @@
         backoff_factor (float, optional): backoff_factor used by DynamicGradScaler. Defaults to 0.5.
         growth_interval (float, optional): growth_interval used by DynamicGradScaler. Defaults to 1000.
         hysteresis (float, optional): hysteresis used by DynamicGradScaler. Defaults to 2.
         max_scale (int, optional): max_scale used by DynamicGradScaler. Defaults to 2**32.
         max_norm (float, optional): max_norm used for `clip_grad_norm`. You should notice that you shall not do
             clip_grad_norm by yourself when using ZeRO DDP. The ZeRO optimizer will take care of clip_grad_norm.
         norm_type (float, optional): norm_type used for `clip_grad_norm`.
-        verbose (bool, optional): verbose mode. Debug info including chunk search result will be printed. Defaults to False.
     """
 
     def __init__(
         self,
         device: Optional[torch.device] = None,
         placement_policy: str = "cpu",
         pin_memory: bool = False,
@@ -167,15 +207,14 @@
         growth_factor: float = 2,
         backoff_factor: float = 0.5,
         growth_interval: int = 1000,
         hysteresis: int = 2,
         max_scale: float = 2**32,
         max_norm: float = 0.0,
         norm_type: float = 2.0,
-        verbose: bool = False,
     ) -> None:
 
         assert dist.is_initialized(
         ), 'torch.distributed is not initialized, please use colossalai.launch to create the distributed environment'
         self.rank = dist.get_rank()
         self.world_size = dist.get_world_size()
         self.gemini_config = dict(
@@ -195,15 +234,14 @@
                                  backoff_factor=backoff_factor,
                                  growth_interval=growth_interval,
                                  hysteresis=hysteresis,
                                  min_scale=min_scale,
                                  max_scale=max_scale,
                                  max_norm=max_norm,
                                  norm_type=norm_type)
-        self.verbose = verbose
 
     def support_no_sync(self) -> bool:
         return False
 
     def control_precision(self) -> bool:
         return True
 
@@ -283,19 +321,18 @@
             # This inconsistency of dtype will cause the error.
             # We have two possible solutions:
             # 1. keep batch norm always in fp32. This is hard for gemini, as it use chunks.
             # 2. patch sync bn or write a new on. This is relatively easy, but we need to test it.
             # model = nn.SyncBatchNorm.convert_sync_batchnorm(model, None)
 
             # wrap the model with Gemini
-            model = GeminiModel(model, self.gemini_config, self.verbose)
+            model = GeminiModel(model, self.gemini_config)
 
         if not isinstance(optimizer, OptimizerWrapper):
-            optimizer = GeminiOptimizer(model.unwrap(), optimizer, self.zero_optim_config, self.optim_kwargs,
-                                        self.verbose)
+            optimizer = GeminiOptimizer(model.unwrap(), optimizer, self.zero_optim_config, self.optim_kwargs)
 
         return model, optimizer, criterion, dataloader, lr_scheduler
 
     def control_checkpoint_io(self) -> bool:
         return True
 
     def get_checkpoint_io(self) -> CheckpointIO:
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/booster/plugin/plugin_base.py` & `colossalai-nightly-2023.4.8/colossalai/booster/plugin/plugin_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/booster/plugin/torch_ddp_plugin.py` & `colossalai-nightly-2023.4.8/colossalai/booster/plugin/torch_ddp_plugin.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/builder/builder.py` & `colossalai-nightly-2023.4.8/colossalai/builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/checkpoint_io/checkpoint_io_base.py` & `colossalai-nightly-2023.4.8/colossalai/checkpoint_io/checkpoint_io_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Union
-from typing import Optional
 
 import torch
 import torch.nn as nn
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 
 from colossalai.interface import ModelWrapper
@@ -67,15 +66,15 @@
                    checkpoint: str,
                    strict: bool = True) -> Union[nn.Module, ModelWrapper]:
         """
         Load model from checkpoint.
 
         Args:
             model (nn.Module): model to be loaded.
-            checkpoint (str): checkpoint path. This value is made compatibility with the model checkpoints in the
+            checkpoint (str): checkpoint path. This value is made compatiblity with the model checkpoints in the
                         mainstream model zoos such as Hugging Face and TIMM. The checkpoint path can be:
                         1. a file path, e.g. 'model.pt'
                         2. a path to a json file which defines the index to the sharded checkpoint
                         3. a path to a folder containing a unique .index.json file for sharded checkpoint
                         Distributed tensors cannot be loaded directly unless gathered offline via our CLI.
             strict (bool): whether to strictly enforce that the param name in
                 the checkpoint match the keys returned by this module's.
@@ -101,15 +100,15 @@
         return origin_model
 
     def save_model(self,
                    model: Union[nn.Module, ModelWrapper],
                    checkpoint: str,
                    shard: bool = False,
                    gather_dtensor: bool = True,
-                   variant: str = None,
+                   prefix: str = None,
                    size_per_shard: int = 1024,
                    use_safetensors: bool = False):
         """
         Save model to checkpoint.
 
         Examples:
             >>> from colossalai.checkpoint_io import GeneralCheckpointIO
@@ -123,37 +122,37 @@
 
         Args:
             model (nn.Module): model to be saved.
             checkpoint (str): checkpoint path. The checkpoint path can be :
                 1. a file path, e.g. 'model.pt'
                 2. a directory path to save the sharded checkpoint, e.g. './checkpoints/' when shard = True.
             shard (bool): whether to shard the checkpoint. Default: False. If set to True, the checkpoint will be sharded into
-                multiple files. The model shards will be specified by a `model.index.json` file. When shard = True, please ensure
+                multiple files. The model shards will be specificed by a `model.index.json` file. When shard = True, please ensure
                 that the checkpoint path is a directory path instead of a file path.
             gather_dtensor (bool): whether to gather the distributed tensor to the first device. Default: True.
-            variant (str): If specified, weights are saved in the format pytorch_model.<variant>.bin. Default: None.
+            prefix (str): prefix for the model checkpoint file name when shard=True. Default: None.
             size_per_shard (int): size per shard in MB. Default: 1024. This value is only used when shard = True.
             use_safetensors (bool): whether to use safe tensors. Default: False. If set to True, the checkpoint will be saved
         """
 
         if isinstance(model, ModelWrapper):
             model = model.unwrap()
 
         if shard:
-            self.save_sharded_model(model, checkpoint, gather_dtensor, variant, size_per_shard, use_safetensors)
+            self.save_sharded_model(model, checkpoint, gather_dtensor, prefix, size_per_shard, use_safetensors)
         else:
             self.save_unsharded_model(model, checkpoint, gather_dtensor, use_safetensors)
 
     def load_optimizer(self, optimizer: Optimizer, checkpoint: str):
         """
         Load optimizer from checkpoint.
 
         Args:
             optimizer (Optimizer): optimizer to be loaded.
-            checkpoint (str): checkpoint path. This value is made compatibility with the model checkpoints in the
+            checkpoint (str): checkpoint path. This value is made compatiblity with the model checkpoints in the
         """
         index_file_exists, index_file_path = has_index_file(checkpoint)
 
         if Path(checkpoint).is_dir() and not index_file_exists:
             # if the checkpoint is a directory and there is no index file, raise error
             raise ValueError(f'Cannot find index file in {checkpoint}')
 
@@ -176,15 +175,15 @@
         Args:
             optimizer (Optimizer): optimizer to be saved.
             checkpoint (str): checkpoint path. The checkpoint path can be :
                 1. a file path, e.g. 'model.pt'
                 2. a path to a json file which defines the index to the sharded checkpoint for the optimizer
                 3. a path to a folder containing a unique .index.json file for sharded checkpoint
             shard (bool): whether to shard the checkpoint. Default: False. If set to True, the checkpoint will be sharded into
-                multiple files. The optimizer shards will be specified by a `optimizer.index.json` file.
+                multiple files. The optimizer shards will be specificed by a `optimizer.index.json` file.
             gather_dtensor (bool): whether to gather the distributed tensor to the first device. Default: True.
             prefix (str): prefix for the optimizer checkpoint when shard = True. Default: None.
             size_per_shard (int): size per shard in MB. Default: 1024. This value is only used when shard is set to True.
         """
         if shard:
             self.save_sharded_optimizer(optimizer, checkpoint, gather_dtensor, prefix, size_per_shard)
         else:
@@ -216,15 +215,15 @@
             checkpoint (str): checkpoint path. It should be a single file path pointing to a model weight binary.
             strict (bool): whether to strictly enforce that the param name in
                 the checkpoint match the keys returned by this module's.
         """
         pass
 
     @abstractmethod
-    def save_sharded_model(self, model: nn.Module, checkpoint: str, gather_dtensor: bool, variant: Optional[str],
+    def save_sharded_model(self, model: nn.Module, checkpoint: str, gather_dtensor: bool, prefix: str,
                            size_per_shard: int, use_safetensors: bool):
         """
         Save model to sharded checkpoint.
 
         Args:
             model (nn.Module): model to be saved.
             checkpoint (str): checkpoint path. It should be a directory path.
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/checkpoint_io/general_checkpoint_io.py` & `colossalai-nightly-2023.4.8/colossalai/checkpoint_io/general_checkpoint_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,31 +2,28 @@
 
 import torch.nn as nn
 from torch.optim import Optimizer
 import logging
 import os
 import json
 import gc
-from typing import Optional
 
 from .checkpoint_io_base import CheckpointIO
 from .index_file import CheckpointIndexFile
 from .utils import (
     has_index_file, 
     load_state_dict, 
     save_state_dict, 
     is_safetensors_available,
     shard_checkpoint,
     load_shard_state_dict,
-    load_state_dict_into_model,
-    add_variant
+    load_state_dict_into_model
     )
 from .utils import SAFE_WEIGHTS_NAME, WEIGHTS_NAME, SAFE_WEIGHTS_INDEX_NAME, WEIGHTS_INDEX_NAME
 
-
 __all__ = ['GeneralCheckpointIO']
 
 
 class GeneralCheckpointIO(CheckpointIO):
     """
     Checkpoint IO
     """
@@ -68,40 +65,38 @@
         gather_dtensor: bool,
     ):
         # TODO(FrankLeeeee): handle distributed tensors
         save_state_dict(optimizer.state_dict(), checkpoint, use_safetensors=False)
 
 
     def save_sharded_model(self, model: nn.Module, checkpoint_path: str, gather_dtensor:bool = False, 
-                           variant: Optional[str] = None, max_shard_size: int = 1024, use_safetensors: bool = False):
+                           prefix: str = "", max_shard_size: int = 1024, use_safetensors: bool = False):
         """ 
         implement this method as it can be supported by Huggingface model,
         save shard model, save model to multiple files
         """
         if os.path.isfile(checkpoint_path):
             logging.error(f"Provided path ({checkpoint_path}) should be a directory, not a file")
             return
         
         Path(checkpoint_path).mkdir(parents=True, exist_ok=True)
         
         # shard checkpoint
         state_dict = model.state_dict()
         weights_name = SAFE_WEIGHTS_NAME if use_safetensors else WEIGHTS_NAME
-        weights_name = add_variant(weights_name, variant)
         shards, index = shard_checkpoint(state_dict, max_shard_size=max_shard_size, weights_name=weights_name)
 
         # Save the model
         for shard_file, shard in shards.items():
             checkpoint_file_path = os.path.join(checkpoint_path, shard_file)
             save_state_dict(shard, checkpoint_file_path, use_safetensors)
 
         # save index file
         save_index_file = SAFE_WEIGHTS_INDEX_NAME if use_safetensors else WEIGHTS_INDEX_NAME
-
-        save_index_file = os.path.join(checkpoint_path, add_variant(save_index_file, variant))
+        save_index_file = os.path.join(checkpoint_path, save_index_file)
         with open(save_index_file, "w", encoding="utf-8") as f:
             content = json.dumps(index, indent=2, sort_keys=True) + "\n"
             f.write(content)
         logging.info(
             f"The model is bigger than the maximum size per checkpoint ({max_shard_size}) and is going to be "
             f"split in {len(shards)} checkpoint shards. You can find where each parameters has been saved in the "
             f"index located at {save_index_file}."
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/checkpoint_io/index_file.py` & `colossalai-nightly-2023.4.8/colossalai/checkpoint_io/index_file.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/checkpoint_io/utils.py` & `colossalai-nightly-2023.4.8/colossalai/checkpoint_io/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # coding=utf-8
 from pathlib import Path
 import torch
 import torch.nn as nn
 from typing import List, Dict, Mapping, OrderedDict, Optional, Tuple
 from colossalai.tensor.d_tensor.d_tensor import DTensor
-import re
 
 SAFE_WEIGHTS_NAME = "model.safetensors"
-WEIGHTS_NAME = "pytorch_model.bin"
+WEIGHTS_NAME = "model.bin"
 SAFE_WEIGHTS_INDEX_NAME = "model.safetensors.index.json"
-WEIGHTS_INDEX_NAME = "pytorch_model.bin.index.json"
+WEIGHTS_INDEX_NAME = "model.bin.index.json"
 
 # ======================================
 # General helper functions
 # ======================================
 
 def calculate_tensor_size(tensor: torch.Tensor) -> float:
     """
@@ -24,14 +23,15 @@
         tenosr (torch.Tensor): the tensor to calculate size for.
 
     Returns:
         float: size of the tensor in MB.
     """
     return tensor.numel() * tensor.element_size() / 1024 / 1024
 
+
 def is_safetensors_available() -> bool:
     """
     Check whether safetensors is available.
 
     Returns:
         bool: whether safetensors is available.
     """
@@ -354,22 +354,21 @@
 
     Returns:
         Tuple[bool, Optional[Path]]: a tuple of (has_index_file, index_file_path)
     """
     checkpoint_path = Path(checkpoint_path)
     if checkpoint_path.is_file():
         # check if it is .index.json
-        reg = re.compile("(.*?).index((\..*)?).json")
-        if reg.fullmatch(checkpoint_path.name) is not None:
+        if checkpoint_path.name.endswith('.index.json'):
             return True, checkpoint_path
         else:
             return False, None
     elif checkpoint_path.is_dir():
         # check if there is only one a file ending with .index.json in this directory
-        index_files = list(checkpoint_path.glob('*.index.*json'))
+        index_files = list(checkpoint_path.glob('*.index.json'))
 
         # if we found a .index.json file, make sure there is only one
         if len(index_files) > 0:
             assert len(
                 index_files
             ) == 1, f'Expected to find one .index.json file in {checkpoint_path}, but found {len(index_files)}'
 
@@ -403,17 +402,7 @@
             for k in f.keys():
                 state_dict[k] = f.get_tensor(k)
         return state_dict
 
     else:
         # load with torch
         return torch.load(checkpoint_file_path)
-    
-
-
-def add_variant(weights_name: str, variant: Optional[str] = None) -> str:
-    if variant is not None and len(variant) > 0:
-        splits = weights_name.split(".")
-        splits = splits[:-1] + [variant] + splits[-1:]
-        weights_name = ".".join(splits)
-
-    return weights_name
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/cli/benchmark/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/cli/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/cli/benchmark/benchmark.py` & `colossalai-nightly-2023.4.8/colossalai/cli/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/cli/benchmark/utils.py` & `colossalai-nightly-2023.4.8/colossalai/cli/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/cli/check/check_installation.py` & `colossalai-nightly-2023.4.8/colossalai/cli/check/check_installation.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,27 +72,27 @@
     click.echo(f'\n------------ CUDA Extensions AOT Compilation ------------')
     click.echo(f"Found AOT CUDA Extension: {to_click_output(found_aot_cuda_ext)}")
     click.echo(f"PyTorch version used for AOT compilation: {to_click_output(prebuilt_torch_version_required)}")
     click.echo(f"CUDA version used for AOT compilation: {to_click_output(prebuilt_cuda_version_required)}")
     click.echo("")
     click.echo(f"Note:")
     click.echo(
-        f"1. AOT (ahead-of-time) compilation of the CUDA kernels occurs during installation when the environment variable CUDA_EXT=1 is set"
+        f"1. AOT (ahead-of-time) compilation of the CUDA kernels occurs during installation when the environment varialbe CUDA_EXT=1 is set"
     )
     click.echo(f"2. If AOT compilation is not enabled, stay calm as the CUDA kernels can still be built during runtime")
 
     click.echo(f"\n------------ Compatibility ------------")
     click.echo(f'PyTorch version match: {to_click_output(torch_compatibility)}')
     click.echo(f"System and PyTorch CUDA version match: {to_click_output(sys_torch_cuda_compatibility)}")
     click.echo(f"System and Colossal-AI CUDA version match: {to_click_output(sys_colossalai_cuda_compatibility)}")
     click.echo(f"")
     click.echo(f"Note:")
     click.echo(f"1. The table above checks the version compatibility of the libraries/tools in the current environment")
     click.echo(
-        f"   - PyTorch version mismatch: whether the PyTorch version in the current environment is compatible with the PyTorch version used for AOT compilation"
+        f"   - PyTorch version mistach: whether the PyTorch version in the current environment is compatible with the PyTorch version used for AOT compilation"
     )
     click.echo(
         f"   - System and PyTorch CUDA version match: whether the CUDA version in the current environment is compatible with the CUDA version required by PyTorch"
     )
     click.echo(
         f"   - System and Colossal-AI CUDA version match: whether the CUDA version in the current environment is compatible with the CUDA version used for AOT compilation"
     )
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/cli/launcher/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/cli/launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/cli/launcher/hostinfo.py` & `colossalai-nightly-2023.4.8/colossalai/cli/launcher/hostinfo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/cli/launcher/multinode_runner.py` & `colossalai-nightly-2023.4.8/colossalai/cli/launcher/multinode_runner.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/cli/launcher/run.py` & `colossalai-nightly-2023.4.8/colossalai/cli/launcher/run.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/cluster/device_mesh_manager.py` & `colossalai-nightly-2023.4.8/colossalai/cluster/device_mesh_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/cluster/dist_coordinator.py` & `colossalai-nightly-2023.4.8/colossalai/cluster/dist_coordinator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/cluster/process_group_manager.py` & `colossalai-nightly-2023.4.8/colossalai/cluster/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/communication/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/communication/collective.py` & `colossalai-nightly-2023.4.8/colossalai/communication/collective.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/communication/p2p.py` & `colossalai-nightly-2023.4.8/colossalai/communication/p2p.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,18 +99,18 @@
                           set to None).
         object_send_prev (Union[:class:`torch.Tensor`, List[:class:`torch.Tensor`]]): tensor to send to prev rank (no tensor sent if
                           set to None).
         recv_prev (bool): boolean for whether tensor should be received from
                    previous rank.
         recv_next (bool): boolean for whether tensor should be received from
                    next rank.
-        recv_prev_shape (Union[:class:`torch.Size`, List[:class:`torch.Size`]]): shape of the tensor to be received from the previous stage, defaults to None.
-        recv_next_shape (Union[:class:`torch.Size`, List[:class:`torch.Size`]]): shape of the tensor to be received from the next stage, defaults to None.
-        prev_rank (int): the rank of the previous pipeline stage, defaults to None,
-        next_rank (int): the rank of the next pipeline stage, defaults to None,
+        recv_prev_shape (Union[:class:`torch.Size`, List[:class:`torch.Size`]]): shape of the tensor to be received from the previous stage, defualts to None.
+        recv_next_shape (Union[:class:`torch.Size`, List[:class:`torch.Size`]]): shape of the tensor to be received from the next stage, defualts to None.
+        prev_rank (int): the rank of the previous pipeline stage, defualts to None,
+        next_rank (int): the rank of the next pipeline stage, defualts to None,
         dtype (torch.dtype): data type of intermediate buffers, defaults to None
         scatter_gather_tensors (bool): whether to scatter and gather tensor between pipeline stages, defaults to False
 
     Returns:
         Tuple[Union[:class:`torch.Tensor`, List[:class:`torch.Tensor`]]]: returns tensor_recv_prev, tensor_recv_next
     """
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/communication/p2p_v2.py` & `colossalai-nightly-2023.4.8/colossalai/communication/p2p_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
     """Copy the gradient tensor from the next stage in pipeline as the input gradient of this stage.
 
     Args:
         output_grad_shape (Union[:class:`torch.Size`, List[:class:`torch.Size`]]): The shape of the tensor to be received.
         next_rank (int, optional): The rank of the source of the tensor.
 
     Returns:
-        Any: The input gradient tensor or gradient tensor list.
+        Any: The input gradient tensor or gradident tensor list.
     """
     if gpc.is_pipeline_last_stage():
         output_tensor_grad = None
     else:
         if next_rank is None:
             next_rank = gpc.get_next_global_rank(ParallelMode.PIPELINE)
         output_tensor_grad = _recv_object(next_rank)
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/communication/ring.py` & `colossalai-nightly-2023.4.8/colossalai/communication/ring.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/communication/utils.py` & `colossalai-nightly-2023.4.8/colossalai/communication/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/constants.py` & `colossalai-nightly-2023.4.8/colossalai/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/context/config.py` & `colossalai-nightly-2023.4.8/colossalai/context/config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/context/moe_context.py` & `colossalai-nightly-2023.4.8/colossalai/context/moe_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         assert torch.cuda.is_available(), "MoE requires to enable CUDA first"
 
         self.world_size = dist.get_world_size()
 
         from colossalai.core import global_context as gpc
         self.max_ep_size = gpc.config.get('max_ep_size', self.world_size)
         assert self.world_size % self.max_ep_size == 0, \
-            "Maximum expert parallel size must be a factor of the number of GPUs"
+            "Maximum epxert parallel size must be a factor of the number of GPUs"
         self.min_dp_size = self.world_size // self.max_ep_size
 
         # Enabling kernel optimization may raise error in some cases
         # Users can close kernel optimization manually
         self.use_kernel_optim = use_kernel_optim
 
         from .random import moe_set_seed
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/context/parallel_context.py` & `colossalai-nightly-2023.4.8/colossalai/context/parallel_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         self._groups = dict()
         self._cpu_groups = dict()
         self._ranks_in_group = dict()
 
         # load config from file
         self._config = None
 
-        # default 3D parallel args, will be overwritten during process group initialization
+        # default 3D parallel args, will be overwritten during process group intialization
         self.world_size = 1
         self.data_parallel_size = 1
         self.pipeline_parallel_size = 1
         self.tensor_parallel_size = 1
         self.num_processes_on_current_node = -1
         self.virtual_pipeline_parallel_size = None
         self.virtual_pipeline_parallel_rank = None
@@ -260,15 +260,15 @@
         self._check_parallel_mode(parallel_mode)
         return self._world_sizes[parallel_mode]
 
     def _add_world_size(self, parallel_mode: ParallelMode, world_size: int):
         """Adds world size for `parallel_mode`.
 
         Args:
-            parallel_mode (:class:`colossalai.context.ParallelMode`): The parallel mode corresponding to the process group
+            parallel_mode (:class:`colossalai.context.ParallelMode`): The parallel mode correponding to the process group
             world_size (int): The world size to be added
 
         Raises:
             AssertionError: Raises an AssertionError if `parallel_mode` is not an instance
                 of :class:`colossalai.context.ParallelMode`.
         """
         self._check_parallel_mode(parallel_mode)
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/context/parallel_mode.py` & `colossalai-nightly-2023.4.8/colossalai/context/parallel_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/initializer_1d.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_1d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/initializer_2d.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/initializer_2p5d.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/initializer_3d.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/initializer_data.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_data.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/initializer_model.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/initializer_pipeline.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_pipeline.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/initializer_sequence.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_sequence.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/initializer_tensor.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/context/process_group_initializer/process_group_initializer.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/process_group_initializer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/context/random/_helper.py` & `colossalai-nightly-2023.4.8/colossalai/context/random/_helper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/context/random/seed_manager.py` & `colossalai-nightly-2023.4.8/colossalai/context/random/seed_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,31 +55,31 @@
             # save the current state for current mode
             self._seed_states[self._current_mode] = torch.cuda.get_rng_state()
 
         # set the new state for new mode
         self._current_mode = parallel_mode
         torch.cuda.set_rng_state(self._seed_states[parallel_mode])
 
-    def add_seed(self, parallel_mode: ParallelMode, seed: int, overwrite: bool = False):
+    def add_seed(self, parallel_mode: ParallelMode, seed: int, overwrtie: bool = False):
         """Adds a seed to the seed manager for `parallel_mode`.
 
         Args:
             parallel_mode (:class:`colossalai.context.ParallelMode`): The chosen parallel mode.
             seed (int): The seed to be added.
-            overwrite (bool, optional): Whether allows to overwrite the seed that has been set already
+            overwrtie (bool, optional): Whether allows to overwrite the seed that has been set already
 
         Raises:
             AssertionError: Raises an AssertionError if `parallel_mode` is not an instance of :class:`colossalai.context.ParallelMode`
                 or the seed for `parallel_mode` has been added.
         """
         assert isinstance(parallel_mode, ParallelMode), 'A valid ParallelMode must be provided'
-        if overwrite is False:
+        if overwrtie is False:
             assert parallel_mode not in self._seed_states, f'The seed for {parallel_mode} has been added'
         elif parallel_mode in self._seed_states:
-            print(f"Warning: {parallel_mode} seed has been overwritten.", flush=True)
+            print(f"Warnning: {parallel_mode} seed has been overwritten.", flush=True)
 
         current_state = torch.cuda.get_rng_state()
         torch.cuda.manual_seed(seed)
         self._seed_states[parallel_mode] = torch.cuda.get_rng_state()
         self._seeds[parallel_mode] = seed
         torch.cuda.set_rng_state(current_state)
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/context/singleton_meta.py` & `colossalai-nightly-2023.4.8/colossalai/context/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/device/alpha_beta_profiler.py` & `colossalai-nightly-2023.4.8/colossalai/device/alpha_beta_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/device/calc_pipeline_strategy.py` & `colossalai-nightly-2023.4.8/colossalai/device/calc_pipeline_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/device/device_mesh.py` & `colossalai-nightly-2023.4.8/colossalai/device/device_mesh.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/engine/_base_engine.py` & `colossalai-nightly-2023.4.8/colossalai/engine/_base_engine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/engine/gradient_accumulation/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_accumulation/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/engine/gradient_accumulation/_gradient_accumulation.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_accumulation/_gradient_accumulation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/engine/gradient_handler/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/engine/gradient_handler/_base_gradient_handler.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_base_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/engine/gradient_handler/_moe_gradient_handler.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_moe_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/engine/gradient_handler/_zero_gradient_handler.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_zero_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/engine/gradient_handler/utils.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/engine/schedule/_base_schedule.py` & `colossalai-nightly-2023.4.8/colossalai/engine/schedule/_base_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/engine/schedule/_non_pipeline_schedule.py` & `colossalai-nightly-2023.4.8/colossalai/engine/schedule/_non_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/engine/schedule/_pipeline_schedule.py` & `colossalai-nightly-2023.4.8/colossalai/engine/schedule/_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/engine/schedule/_pipeline_schedule_v2.py` & `colossalai-nightly-2023.4.8/colossalai/engine/schedule/_pipeline_schedule_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/_compatibility.py` & `colossalai-nightly-2023.4.8/colossalai/fx/_compatibility.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/_meta_regist_12.py` & `colossalai-nightly-2023.4.8/colossalai/fx/_meta_regist_12.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/_meta_regist_13.py` & `colossalai-nightly-2023.4.8/colossalai/fx/_meta_regist_13.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/codegen/activation_checkpoint_codegen.py` & `colossalai-nightly-2023.4.8/colossalai/fx/codegen/activation_checkpoint_codegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,15 @@
 def emit_ckpt_func(body,
                    ckpt_func,
                    node_list: List[Node],
                    emit_node_func,
                    delete_unused_value_func,
                    level=0,
                    in_ckpt=False):
-    """Emit ckpt function in nested way
+    """Emit ckpt fuction in nested way
     Args:
         body: forward code, in recursive calls, this part will be checkpoint
         functions code
         ckpt_func: checkpoint functions code, in recursive calls, this part
         will be a buffer
         node_list (List[Node]): list of torch.fx.Node
         emit_node_func: function to emit a node
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/graph_module.py` & `colossalai-nightly-2023.4.8/colossalai/fx/graph_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/passes/adding_split_node_pass.py` & `colossalai-nightly-2023.4.8/colossalai/fx/passes/adding_split_node_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/passes/concrete_info_prop.py` & `colossalai-nightly-2023.4.8/colossalai/fx/passes/concrete_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/passes/meta_info_prop.py` & `colossalai-nightly-2023.4.8/colossalai/fx/passes/meta_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/passes/passes_for_gpt2_test.py` & `colossalai-nightly-2023.4.8/colossalai/fx/passes/passes_for_gpt2_test.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/passes/shard_1d_pass.py` & `colossalai-nightly-2023.4.8/colossalai/fx/passes/shard_1d_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/passes/split_module.py` & `colossalai-nightly-2023.4.8/colossalai/fx/passes/split_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                     use_partition.partitions_dependent_on.setdefault(def_partition_name)
             use_partition.outputs.setdefault(def_node.name)
         else:
             if use_partition_name is not None:
                 use_partition = partitions[use_partition_name]
                 use_partition.outputs.setdefault(def_node.name)
 
-    # split nodes into partitions
+    # split nodes into parititons
     for node in m.graph.nodes:
         orig_nodes[node.name] = node
 
         if node.op in ["placeholder"]:
             continue
         if node.op == 'output':
             if merge_output:
@@ -194,15 +194,15 @@
         for dependent in partitions[root_partition].partition_dependents:
             partitions[dependent].partitions_dependent_on.pop(root_partition)
             if not partitions[dependent].partitions_dependent_on:
                 root_partitions.append(dependent)
     if len(sorted_partitions) != len(partitions):
         raise RuntimeError("cycle exists between partitions!")
 
-    # add placeholders to partitions
+    # add placeholders to parititons
     for partition_name in sorted_partitions:
         partition = partitions[partition_name]
         for input in partition.inputs:
             placeholder = partition.graph.placeholder(input)
             placeholder.meta = orig_nodes[input].meta.copy()
             partition.environment[orig_nodes[input]] = placeholder
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/passes/utils.py` & `colossalai-nightly-2023.4.8/colossalai/fx/passes/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/constants.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/dataflow.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/dataflow.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/constants.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_function/activation_function.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_function/embedding.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_function/normalization.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_function/pooling.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_module/activation_function.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_module/attention.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_module/convolution.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_module/normalization.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_module/pooling.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/profiler_module/rnn.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/registry.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/experimental/shard_utils.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/memory_utils.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/memory_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/opcount.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/opcount.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/profiler.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/shard_utils.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/profiler/tensor.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/proxy.py` & `colossalai-nightly-2023.4.8/colossalai/fx/proxy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/_meta_trace.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/_meta_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/_symbolic_trace.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/_symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/_tracer_utils.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/_tracer_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/experimental.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/experimental.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_function/convolution.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_function/embedding.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_function/normalization.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_module/convolution.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_module/normalization.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_module/pooling.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/meta_patch/patched_module/rnn.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/registry.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/fx/tracer/tracer.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/global_variables.py` & `colossalai-nightly-2023.4.8/colossalai/global_variables.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/initialize.py` & `colossalai-nightly-2023.4.8/colossalai/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/interface/model.py` & `colossalai-nightly-2023.4.8/colossalai/interface/model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/interface/optimizer.py` & `colossalai-nightly-2023.4.8/colossalai/interface/optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/cpu_adam.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/context.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/context.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/csrc/type_shim.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/type_shim.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/flash_attention.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/flash_attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/layer_norm.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/layer_norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/multihead_attention.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/multihead_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
         layer_id: The layer-index counter starting from 0 and incrementing by 1 every time a layer object is instantiated,
         e.g. if a model has 24 transformer layers, layer_id goes from 0 to 23.
 
     Arguments:
         hidden_size: Total dimension of hidden_size.
         nhead: Number of parallel attention heads.
-        batch_size: Batch Size for one forward
+        batch_size: Batch Size for one foward
         max_seq_len: Max length of input sequence
         dropout: Dropout probability
         norm_first: perform LayerNorms before attention
     """
 
     layer_id = 0
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/cuda_native/scaled_softmax.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/scaled_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/jit/bias_dropout_add.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/jit/bias_dropout_add.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/jit/bias_gelu.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/jit/bias_gelu.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/jit/option.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/jit/option.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/builder.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Licensed under the MIT License.
 import importlib
 import os
 import time
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import List, Optional
+from typing import List
 
 from .utils import check_cuda_availability, check_system_pytorch_cuda_match, print_rank_0
 
 
 class Builder(ABC):
     """
     Builder is the base class to build extensions for PyTorch.
@@ -74,15 +74,15 @@
         This function should return a list of source files for extensions.
         """
         raise NotImplementedError
 
     @abstractmethod
     def include_dirs(self) -> List[str]:
         """
-        This function should return a list of include files for extensions.
+        This function should return a list of inlcude files for extensions.
         """
         pass
 
     @abstractmethod
     def cxx_flags(self) -> List[str]:
         """
         This function should return a list of cxx compilation flags for extensions.
@@ -123,49 +123,47 @@
 
         if not TORCH_AVAILABLE:
             raise ModuleNotFoundError(
                 "PyTorch is not found. You need to install PyTorch first in order to build CUDA extensions")
 
         if CUDA_HOME is None:
             raise RuntimeError(
-                "CUDA_HOME is not found. You need to export CUDA_HOME environment variable or install CUDA Toolkit first in order to build CUDA extensions"
+                "CUDA_HOME is not found. You need to export CUDA_HOME environment vairable or install CUDA Toolkit first in order to build CUDA extensions"
             )
 
         # make sure CUDA is available for compilation during
         cuda_available = check_cuda_availability()
         if not cuda_available:
-            raise RuntimeError("CUDA is not available on your system as torch.cuda.is_available() returns False.")
+            raise RuntimeError("CUDA is not available on your system as torch.cuda.is_avaible() returns False.")
 
         # make sure system CUDA and pytorch CUDA match, an error will raised inside the function if not
         check_system_pytorch_cuda_match(CUDA_HOME)
 
-    def load(self, verbose: Optional[bool] = None):
+    def load(self, verbose=True):
         """
         load the kernel during runtime. If the kernel is not built during pip install, it will build the kernel.
         If the kernel is built during runtime, it will be stored in `~/.cache/colossalai/torch_extensions/`. If the
         kernel is built during pip install, it can be accessed through `colossalai._C`.
 
         Warning: do not load this kernel repeatedly during model execution as it could slow down the training process.
 
         Args:
             verbose (bool, optional): show detailed info. Defaults to True.
         """
-        if verbose is None:
-            verbose = os.environ.get('CAI_KERNEL_VERBOSE', '0') == '1'
         # if the kernel has be compiled and cached, we directly use it
         if self.cached_op_module is not None:
             return self.cached_op_module
 
         try:
             # if the kernel has been pre-built during installation
             # we just directly import it
             op_module = self.import_op()
             if verbose:
                 print_rank_0(
-                    f"[extension] OP {self.prebuilt_import_path} has been compiled ahead of time, skip building.")
+                    f"[extension] OP {self.prebuilt_import_path} has been compileed ahead of time, skip building.")
         except ImportError:
             # check environment
             self.check_runtime_build_environment()
 
             # time the kernel compilation
             start_build = time.time()
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/cpu_adam.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/fused_optim.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/fused_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/layernorm.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/moe.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/multi_head_attn.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/scaled_masked_softmax.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/scaled_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/kernel/op_builder/utils.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     if bare_metal_major != torch_cuda_major:
         raise Exception(
             f'[extension] Failed to build PyTorch extension because the detected CUDA version ({bare_metal_major}.{bare_metal_minor}) '
             f'mismatches the version that was used to compile PyTorch ({torch_cuda_major}.{torch_cuda_minor}).'
             'Please make sure you have set the CUDA_HOME correctly and installed the correct PyTorch in https://pytorch.org/get-started/locally/ .'
         )
 
+    print(bare_metal_minor != torch_cuda_minor)
     if bare_metal_minor != torch_cuda_minor:
         warnings.warn(
             f"[extension] The CUDA version on the system ({bare_metal_major}.{bare_metal_minor}) does not match with the version ({torch_cuda_major}.{torch_cuda_minor}) torch was compiled with. "
             "The mismatch is found in the minor version. As the APIs are compatible, we will allow compilation to proceed. "
             "If you encounter any issue when using the built kernel, please try to build it again with fully matched CUDA versions"
         )
     return True
@@ -151,23 +152,24 @@
     This function sets the PyTorch TORCH_CUDA_ARCH_LIST variable for ahead-of-time extension compilation.
     Ahead-of-time compilation occurs when CUDA_EXT=1 is set when running 'pip install'.
     """
     cuda_available = check_cuda_availability()
 
     # we only need to set this when CUDA is not available for cross-compilation
     if not cuda_available:
-        warnings.warn('\n[extension]  PyTorch did not find available GPUs on this system.\n'
-                      'If your intention is to cross-compile, this is not an error.\n'
-                      'By default, Colossal-AI will cross-compile for \n'
-                      '1. Pascal (compute capabilities 6.0, 6.1, 6.2),\n'
-                      '2. Volta (compute capability 7.0)\n'
-                      '3. Turing (compute capability 7.5),\n'
-                      '4. Ampere (compute capability 8.0, 8.6)if the CUDA version is >= 11.0\n'
-                      '\nIf you wish to cross-compile for a single specific architecture,\n'
-                      'export TORCH_CUDA_ARCH_LIST="compute capability" before running setup.py.\n')
+        warnings.warn(
+            '\n[extension]  PyTorch did not find available GPUs on this system.\n'
+            'If your intention is to cross-compile, this is not an error.\n'
+            'By default, Colossal-AI will cross-compile for \n'
+            '1. Pascal (compute capabilities 6.0, 6.1, 6.2),\n'
+            '2. Volta (compute capability 7.0)\n'
+            '3. Turing (compute capability 7.5),\n'
+            '4. Ampere (compute capability 8.0, 8.6)if the CUDA version is >= 11.0\n'
+            '\nIf you wish to cross-compile for a single specific architecture,\n'
+            'export TORCH_CUDA_ARCH_LIST="compute capability" before running setup.py.\n')
 
         if os.environ.get("TORCH_CUDA_ARCH_LIST", None) is None:
             bare_metal_major, bare_metal_minor = get_cuda_bare_metal_version(cuda_dir)
 
             arch_list = ['6.0', '6.1', '6.2', '7.0', '7.5']
 
             if int(bare_metal_major) == 11:
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/logging/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/logging/logger.py` & `colossalai-nightly-2023.4.8/colossalai/logging/logger.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/_ops/_utils.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/_ops/addmm.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/_ops/batch_norm.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/batch_norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/_ops/element_wise.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/element_wise.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/_ops/embedding.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/_ops/embedding_bag.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/embedding_bag.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                        padding_idx: Optional[int] = None):
     """Handles ``__torch_function__`` dispatch for ``torch.nn.functional.embedding_bag``.
     This method looks up an embedding table.
     """
     assert isinstance(weight, ColoTensor)
     input_tensor = convert_to_colo_tensor(input_tensor, weight.get_process_group())
 
-    # Handle different parallel actions.
+    # Handle differen parallel actions.
 
     if not weight.has_compute_spec():    # No Model Parallel Applied
         assert weight.is_replicate(), 'Invalid weight spec for native embedding op'
         return ColoTensor.from_torch_tensor(tensor=F.embedding_bag(input_tensor,
                                                                    weight,
                                                                    offsets=offsets,
                                                                    max_norm=max_norm,
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/_ops/layernorm.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/_ops/linear.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/_ops/loss.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/loss.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/_ops/view.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/view.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/init.py` & `colossalai-nightly-2023.4.8/colossalai/nn/init.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/base_layer.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/base_layer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/colossalai_layer/_utils.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/colossalai_layer/dropout.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/dropout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/colossalai_layer/embedding.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/colossalai_layer/linear.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/colossalai_layer/normalization.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/moe/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/moe/_operation.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/moe/checkpoint.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/moe/experts.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/experts.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,34 +9,34 @@
 from colossalai.context import ParallelMode, seed
 from colossalai.context.moe_context import MOE_CONTEXT
 from colossalai.utils import get_current_device
 from colossalai.zero.legacy.init_ctx import no_shard_zero_decrator
 
 
 class MoeExperts(nn.Module):
-    """Basic class for experts in MoE. It stores what kind of communication experts use
+    """Basic class for experts in MoE. It stores what kind of communication expersts use
     to exchange tokens, how many experts in a single GPU and parallel information such as
     expert parallel size, data parallel size and their distributed communication groups.
     """
 
     def __init__(self, comm_name: str, num_experts: int):
         super().__init__()
         assert comm_name in {"all_to_all", "all_gather"}, \
             "This kind of communication has not been implemented yet.\n Please use Experts build function."
         self.comm_name = comm_name
         self.num_total_experts = num_experts
-        # Get the configuration of experts' deployment and parallel information from moe context
+        # Get the configuration of experts' deployment and parallel information from moe contex
         self.num_local_experts, self.dist_info = MOE_CONTEXT.get_info(num_experts)
 
 
 @no_shard_zero_decrator(is_replicated=False)
 class Experts(MoeExperts):
     """A wrapper class to create experts. It will create E experts across the
     moe model parallel group, where E is the number of experts. Every expert
-    is a instance of the class, 'expert' in initialization parameters.
+    is a instence of the class, 'expert' in initialization parameters.
 
     Args:
         expert_cls (:class:`torch.nn.Module`): The class of all experts
         num_experts (int): The number of experts
         expert_args: Args used to initialize experts, the args could be found in corresponding expert class
     """
 
@@ -142,23 +142,23 @@
         outputs = outputs.reshape(inshape)
         outputs = outputs.transpose(0, 1).contiguous()
         return outputs
 
 
 class TPExperts(MoeExperts):
     """Use tensor parallelism to split each expert evenly, which can deploy experts in
-    case that the number of experts can't be divide by maximum expert parallel size or
-    maximum expert parallel size can't be divide by the number of experts.
+    case that the number of experts can't be divied by maximum expert parallel size or
+    maximum expert parallel size can't be divied by the number of experts.
     """
 
     def __init__(self, num_experts: int, d_model: int, d_ff: int, activation=None, drop_rate: float = 0):
         super().__init__("all_gather", MOE_CONTEXT.max_ep_size)
 
         assert d_ff % MOE_CONTEXT.max_ep_size == 0, \
-            "d_ff should be divide by maximum expert parallel size"
+            "d_ff should be divied by maximum expert parallel size"
 
         p_ff = d_ff // MOE_CONTEXT.max_ep_size
 
         self.w1 = nn.Parameter(torch.empty(num_experts, d_model, p_ff, device=get_current_device()))
         self.b1 = nn.Parameter(torch.empty(num_experts, 1, p_ff, device=get_current_device()))
 
         self.w2 = nn.Parameter(torch.empty(num_experts, p_ff, d_model, device=get_current_device()))
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/moe/layers.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from colossalai.zero.legacy.init_ctx import no_shard_zero_context, no_shard_zero_decrator
 
 
 @no_shard_zero_decrator(is_replicated=True)
 class MoeLayer(nn.Module):
     """A MoE layer, that puts its input tensor to its gate and uses the output logits
     to router all tokens, is mainly used to exchange all tokens for every expert across
-    the moe tensor group by all to all communication. Then it will get the output of all
+    the moe tensor group by all to all comunication. Then it will get the output of all
     experts and exchange the output. At last returns the output of the moe system.
 
     Args:
         dim_model (int): Dimension of model.
         num_experts (int): The number of experts.
         router (MoeRouter): Instance of router used in routing.
         experts (MoeExperts): Instance of experts generated by Expert.
@@ -118,15 +118,15 @@
         min_capacity (int, optional): The minimum number of the capacity of each expert
         noisy_policy (str, optional): The policy of noisy function. Now we have 'Jitter' and 'Gaussian'.
             'Jitter' can be found in `Switch Transformer paper`_.
             'Gaussian' can be found in `ViT-MoE paper`_.
         drop_tks (bool, optional): Whether drops tokens in evaluation
         use_residual (bool, optional): Makes this MoE layer a Residual MoE.
             More information can be found in `Microsoft paper`_.
-        residual_instance (nn.Module, optional): The instance of residual module in Residual MoE
+        residual_instance (nn.Module, optional): The instance of residual module in Resiual MoE
         expert_instance (MoeExperts, optional): The instance of experts module in MoeLayer
         expert_cls (Type[nn.Module], optional): The class of each expert when no instance is given
         expert_args (optional): The args of expert when no instance is given
 
     .. _Switch Transformer paper:
         https://arxiv.org/abs/2101.03961
     .. _ViT-MoE paper:
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/moe/routers.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/routers.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         reservation = self._routing_loss
         self._routing_loss = None
         return reservation
 
 
 class Top1Router(MoeRouter):
     """Top1 router that returns the dispatch mask [s, e, c] and combine weight [s, e, c]
-    for routing usage. More detailed function can be found in the paper about Switch Transformer
+    for routing usage. More deailted function can be found in the paper about Switch Transformer
     of Google.
     Args:
         capacity_factor_train (float, optional): Capacity factor in routing of training.
         capacity_factor_eval (float, optional): Capacity factor in routing of evaluation.
         min_capacity (int, optional): The minimum number of the capacity of each expert.
         select_policy (str, optional): The policy about tokens selection.
         noisy_func (:class:`typing.Callable`, optional): Noisy function used in logits.
@@ -139,15 +139,15 @@
             combine_weights = weight.unsqueeze(2) * ranks.unsqueeze(1)
             sec_mask = combine_weights.bool()
             return combine_weights, sec_mask
 
 
 class Top2Router(MoeRouter):
     """Top2 router that returns the dispatch mask [s, e, c] and combine weight [s, e, c]
-    for routing usage. More detailed function can be found in the paper about ViT-MoE.
+    for routing usage. More deailted function can be found in the paper about ViT-MoE.
     Args:
         capacity_factor_train (float, optional): Capacity factor in routing of training.
         capacity_factor_eval (float, optional): Capacity factor in routing of evaluation.
         min_capacity (int, optional): The minimum number of the capacity of each expert
         noisy_func (:class:`typing.Callable`, optional): Noisy function used in logits.
         drop_tks (bool, optional): Whether drops tokens in evaluation.
     """
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/moe/utils.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class ForceFP32Parameter(torch.nn.Parameter):
 
     def half(self, memory_format=None):
         return self.data.clone()
 
 
 class NormalNoiseGenerator:
-    """Generates a random noisy mask for logits tensor.
+    """Generates a random noisy mask for logtis tensor.
 
     All noise is generated from a normal distribution :math:`(0, 1 / E^2)`, where
     `E = the number of experts`.
 
     Args:
         num_experts (int): The number of experts.
     """
@@ -28,15 +28,15 @@
 
     def __call__(self, inputs: torch.Tensor):
         noisy = self.normal(inputs.shape)
         return inputs + noisy
 
 
 class UniformNoiseGenerator:
-    """Generates a random noisy mask for logits tensor.
+    """Generates a random noisy mask for logtis tensor.
     copied from mesh tensorflow:
     Multiply values by a random number between :math:`1-epsilon` and :math:`1+epsilon`.
     Makes models more resilient to rounding errors introduced by bfloat16.
     This seems particularly important for logits.
 
     Args:
         eps (float, optional): Epsilon in generator, defaults 1e-2.
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_1d/_operation.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_1d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_1d/_utils.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_1d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_1d/layers.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_1d/layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,15 +435,15 @@
         out_features (int): size of each output sample.
         bias (bool, optional): If set to ``False``, the layer will not learn an additive bias, defaults to ``True``.
         dtype (:class:`torch.dtype`, optional): The dtype of parameters, defaults to None.
         gather_output (bool, optional): If true, call all-gather on output and make Y available
                     to all GPUs, otherwise, every GPU will have its output
                     which is :math:`Y_i = XA_i`, defaults to False
         skip_bias_add (bool, optional): If set to ``True``, it will skip bias add for linear layer,
-            which is preserved for kernel fusion, defaults to False
+            which is preserved for kernel fusion, defaults to Fals
         weight_initializer (:class:`typing.Callable`, optional):
             The initializer of weight, defaults to kaiming uniform initializer.
         bias_initializer (:class:`typing.Callable`, optional):
             The initializer of bias, defaults to xavier uniform initializer.
 
     More details about ``initializer`` please refer to
     `init <https://github.com/hpcaitech/ColossalAI/blob/main/colossalai/nn/init.py>`_.
@@ -574,15 +574,15 @@
     Args:
         in_features (int): size of each input sample.
         out_features (int): size of each output sample.
         bias (bool, optional): If set to ``False``, the layer will not learn an additive bias, defaults to ``True``.
         dtype (:class:`torch.dtype`, optional): The dtype of parameters, defaults to None.
         parallel_input (bool, optional): If set to ``True``, it's assumed that the input is split, defaults to False.
         skip_bias_add (bool, optional): If set to ``True``, it will skip bias add for linear layer,
-            which is preserved for kernel fusion, defaults to False
+            which is preserved for kernel fusion, defaults to Fals
         weight_initializer (:class:`typing.Callable`, optional):
             The initializer of weight, defaults to kaiming uniform initializer.
         bias_initializer (:class:`typing.Callable`, optional):
             The initializer of bias, defaults to xavier uniform initializer.
 
     More details about ``initializer`` please refer to
     `init <https://github.com/hpcaitech/ColossalAI/blob/main/colossalai/nn/init.py>`_.
@@ -990,19 +990,19 @@
     :type in_chans: int
     :param embed_size: size of embedding
     :type embed_size: int
     :param dtype: The dtype of parameters, defaults to None
     :type dtype: torch.dtype, optional
     :param flatten: whether to flatten output tensor, defaults to True
     :type flatten: bool, optional
-    :param weight_initializer: The initializer of weight, defaults to kaiming uniform initializer
+    :param weight_initializer: The intializer of weight, defaults to kaiming uniform initializer
     :type weight_initializer: typing.Callable, optional
-    :param bias_initializer: The initializer of bias, defaults to xavier uniform initializer
+    :param bias_initializer: The intializer of bias, defaults to xavier uniform initializer
     :type bias_initializer: typing.Callable, optional
-    :param position_embed_initializer: The initializer of position embedding, defaults to zero
+    :param position_embed_initializer: The intializer of position embedding, defaults to zero
     :type position_embed_initializer: typing.Callable, optional
     """
 
     def __init__(self,
                  img_size: int,
                  patch_size: int,
                  in_chans: int,
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_2d/_operation.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_2d/_utils.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_2d/layers.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_2p5d/_operation.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2p5d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_2p5d/_utils.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2p5d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_2p5d/layers.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2p5d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_3d/_operation.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_3d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_3d/_utils.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_3d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_3d/layers.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_3d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_sequence/_operation.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_sequence/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/parallel_sequence/layers.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_sequence/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/utils/common.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/vanilla/layers.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/vanilla/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/layer/wrapper/pipeline_wrapper.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/wrapper/pipeline_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/loss/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/nn/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/loss/loss_1d.py` & `colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_1d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/loss/loss_2d.py` & `colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/loss/loss_2p5d.py` & `colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/loss/loss_3d.py` & `colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/loss/loss_moe.py` & `colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/lr_scheduler/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/lr_scheduler/cosine.py` & `colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/cosine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/lr_scheduler/delayed.py` & `colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/delayed.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/lr_scheduler/linear.py` & `colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/lr_scheduler/multistep.py` & `colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/multistep.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/lr_scheduler/onecycle.py` & `colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/onecycle.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/lr_scheduler/poly.py` & `colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/poly.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/lr_scheduler/torch.py` & `colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/metric/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/nn/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/metric/accuracy_2d.py` & `colossalai-nightly-2023.4.8/colossalai/nn/metric/accuracy_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/metric/accuracy_2p5d.py` & `colossalai-nightly-2023.4.8/colossalai/nn/metric/accuracy_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/metric/accuracy_3d.py` & `colossalai-nightly-2023.4.8/colossalai/nn/metric/accuracy_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/optimizer/colossalai_optimizer.py` & `colossalai-nightly-2023.4.8/colossalai/nn/optimizer/colossalai_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/optimizer/cpu_adam.py` & `colossalai-nightly-2023.4.8/colossalai/nn/optimizer/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/optimizer/fused_adam.py` & `colossalai-nightly-2023.4.8/colossalai/nn/optimizer/fused_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/optimizer/fused_lamb.py` & `colossalai-nightly-2023.4.8/colossalai/nn/optimizer/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/optimizer/fused_sgd.py` & `colossalai-nightly-2023.4.8/colossalai/nn/optimizer/fused_sgd.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/optimizer/hybrid_adam.py` & `colossalai-nightly-2023.4.8/colossalai/nn/optimizer/hybrid_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/optimizer/lamb.py` & `colossalai-nightly-2023.4.8/colossalai/nn/optimizer/lamb.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/optimizer/lars.py` & `colossalai-nightly-2023.4.8/colossalai/nn/optimizer/lars.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/optimizer/nvme_optimizer.py` & `colossalai-nightly-2023.4.8/colossalai/nn/optimizer/nvme_optimizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import math
+import torch
 import os
 import tempfile
-from typing import Callable, Dict, List, Optional
-
-import torch
+import math
 from torch.nn.parameter import Parameter
+from typing import Optional, List, Dict, Callable
 
 
 class NVMeOptimizer(torch.optim.Optimizer):
     """A base class for offloading optimizer states.
 
     Args:
         params: parameters
@@ -39,17 +38,16 @@
             backend = 'uring' if 'uring' in get_backends() else 'aio'
             self.offloader = DiskOffloader(self.offload_dir, 8, backend=backend)
         else:
             self.offload_dir = None
             self.offloader = None
         self.is_on_nvme: Dict[Parameter, bool] = {}
         self.offloaded_numel: int = 0
-        # As param may be not materialized here, these attributes are initalized when the first step
-        self.total_numel: Optional[int] = None
-        self.can_offload_numel: Optional[int] = None
+        self.total_numel: int = self._get_numel()
+        self.can_offload_numel = math.floor(self.total_numel * self.nvme_offload_fraction)
 
         self.prefetch_params: List[Parameter] = []
         self.param_to_prefetch_idx: Dict[Parameter, int] = {}
 
     def _get_numel(self) -> int:
         numel = 0
         for group in self.param_groups:
@@ -75,17 +73,14 @@
                     continue
                 if len(self.state[p]) > 0 and self.is_on_nvme[p]:
                     assert p.device.type == 'cpu'
                     self.param_to_prefetch_idx[p] = len(self.prefetch_params)
                     self.prefetch_params.append(p)
 
     def _pre_step(self, *state_keys: str) -> None:
-        if self.total_numel is None:
-            self.total_numel = self._get_numel()
-            self.can_offload_numel = math.floor(self.total_numel * self.nvme_offload_fraction)
         self._setup_prefetch_params()
         if self.offloader is None or len(self.prefetch_params) == 0:
             return
         state = self.state[self.prefetch_params[0]]
         for key in state_keys:
             self.offloader.async_read(state[key])
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/parallel/data_parallel.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/copyer.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/copyer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/colo_module.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/colo_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/embedding.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/linear.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/parallel/layers/module_utils.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/module_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/nn/parallel/reducer.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/reducer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/pipeline/layer_spec.py` & `colossalai-nightly-2023.4.8/colossalai/pipeline/layer_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/pipeline/middleware/adaptor/fx.py` & `colossalai-nightly-2023.4.8/colossalai/pipeline/middleware/adaptor/fx.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/pipeline/middleware/topo.py` & `colossalai-nightly-2023.4.8/colossalai/pipeline/middleware/topo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/pipeline/pipelinable.py` & `colossalai-nightly-2023.4.8/colossalai/pipeline/pipelinable.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/pipeline/pipeline_process_group.py` & `colossalai-nightly-2023.4.8/colossalai/pipeline/pipeline_process_group.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/pipeline/rpc/_pipeline_base.py` & `colossalai-nightly-2023.4.8/colossalai/pipeline/rpc/_pipeline_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/pipeline/rpc/_pipeline_schedule.py` & `colossalai-nightly-2023.4.8/colossalai/pipeline/rpc/_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/pipeline/rpc/utils.py` & `colossalai-nightly-2023.4.8/colossalai/pipeline/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/pipeline/utils.py` & `colossalai-nightly-2023.4.8/colossalai/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/registry/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/registry/registry.py` & `colossalai-nightly-2023.4.8/colossalai/registry/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/colo_parameter.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/colo_parameter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/colo_tensor.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/colo_tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
             func = _COLOSSAL_OPS[func]
 
         if cls.torch_major > 1 or (cls.torch_major == 1 and cls.torch_minor >= 12):
             # in order to trigger pre-op hook in the forward of checkpoint module
             # we have to capture the `backward` function
             # and make sure that it does not in `torch._C.DisableTorchFunction()` context
             if func is torch.Tensor.backward:
-                assert len(args) == 1    # only has 1 parameter
+                assert len(args) == 1    # only has 1 paramter
                 backward_tensor = torch.Tensor(args[0])
                 tensor_kwargs = {k: torch.Tensor(v) if torch.is_tensor(v) else v for k, v in kwargs.items()}
                 return backward_tensor.backward(**tensor_kwargs)
 
         with torch._C.DisableTorchFunction():
             ret = func(*args, **kwargs)
             if func in _get_my_nowrap_functions():
@@ -224,15 +224,15 @@
 
         1. If the pg is None, then redistribute the tensor payload among the TP process group. Keep the
         DP process group not changed.
 
         2. If the pg is not not None and not equal to the current process group.
         First, convert the tensor as replicated among the TP process group.
         Second, reset the process group to the new pg.
-        Third, convert the tensor (new replicated both among the tp process group) to the new dist_spec.
+        Third, conver the tensor (new replicated both among the tp process group) to the new dist_spec.
 
         Args:
             dist_spec (_DistSpec): the new dist spec.
             pg (Optional[ProcessGroup], optional): the new process group . Defaults to None.
 
         Returns:
             ColoTensor: a redistributed colotensor
@@ -293,15 +293,15 @@
     def size_local(self, *args) -> torch.Size:
         with torch._C.DisableTorchFunction():
             return super().size(*args)
 
     def size_global(self, *args) -> torch.Size:
         """size_global
 
-        override the torch building size()
+        override the torch buildin size()
         the shape passed in must be in a replicate placement.
 
         Returns:
             torch.Size: the global tensor shape
         """
         if self.is_replicate():
             return self.size_local(*args)
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/comm_spec.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/comm_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,15 +387,15 @@
     1. Compute the communication cost which will be used in auto parallel solver.
     2. Convert the communication spec to real action which will be used in runtime.
     It contains comm_pattern to determine the
     communication method, sharding_spec to determine the communication size, gather_dim and shard_dim
     to determine the buffer shape, and logical_process_axis
 
     Argument:
-        comm_pattern(CollectiveCommPattern): describe the communication method used in this spec.
+        comm_pattern(CollectiveCommPattern): decribe the communication method used in this spec.
         sharding_spec(ShardingSpec): This is sharding spec of the tensor which will join the communication action.
         gather_dim(int, Optional): The gather_dim of the tensor will be gathered.
         shard_dim(int, Optional): The shard_dim of the tensor will be sharded.
         logical_process_axis(Union(int, List[int]), Optional): The mesh_dim to implement the communication action.
     '''
 
     def __init__(self,
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/compute_spec.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/compute_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     TP2D = 1
     TP2P5D = 2
     TP3D = 3
 
 
 class ComputeSpec(object):
     """ComputeSpec
-    The Specification for computation pattern
+    The Specification for compuattion pattern
 
     Args:
         compute_pattern (ComputePattern): an Enum instance for compute pattern.
     """
 
     def __init__(self, compute_pattern: ComputePattern) -> None:
         assert isinstance(compute_pattern, ComputePattern)
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/d_tensor/comm_spec.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/comm_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/d_tensor/d_tensor.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/d_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/d_tensor/layout.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .sharding_spec import ShardingSpec
 
 
 class Layout:
     """Layout of a tensor.
 
     Attributes:
-        device_mesh: the device mesh to store the tensor distributed.
+        device_mesh: the device mesh to store the tensor distributedly.
         device_type: the type of the device mesh, e.g. 'cpu' or 'cuda'.
         sharding_spec: the sharding specification to describe how the tensor is sharded.
         entire_shape: the entire shape of the global tensor.
     """
 
     def __init__(self, device_mesh: DeviceMesh, device_type: torch.device, sharding_spec: ShardingSpec,
                  entire_shape: torch.Size):
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/d_tensor/layout_converter.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/layout_converter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/d_tensor/sharding_spec.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/sharding_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 SHARD_COST = 5
 STEP_PENALTY = 6
 NAN = 'nan'
 
 
 class DimSpec:
     '''
-    Sharding spec for single dimension of the sharded tensor describe the sharding dimension of
+    Sharding spec for single dimension of the sharded tensor decribe the sharding dimension of
     logical device mesh and give a method to compute the difference between them.
     This class is used internally in ShardingSpec.
 
     Argument:
         shard_list(List[int]): if shard_list is None, the dim spec will be 'R' type.
             Otherwise, the element in shard_list means the data will be sharded in that dimension.
     '''
@@ -139,15 +139,15 @@
 class ShardingSpec:
     '''
     Sharding spec describes how to shard a tensor with dim_size dimensions. The sharding sequence looks like
     [R, R, S0, S1], which means
 
     Argument:
         dim_partition_dict(Dict[int, List[int]], optional): The key is the dimension of tensor to be sharded,
-            and the value of the key describe which logical axis will be sharded in that dimension.
+            and the value of the key decribe which logical axis will be sharded in that dimension.
         sharding_sequence(List[DimSpec], optional): A straight view of ShardingSpec looks like [R, R, S0, S1].
     '''
 
     def __init__(self,
                  dim_size: int,
                  dim_partition_dict: Dict[int, List[int]] = None,
                  sharding_sequence: List[DimSpec] = None):
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/d_tensor/utils.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/dist_spec_mgr.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/dist_spec_mgr.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     def _shard_as(tensor: torch.Tensor, old_dist_spec: _DistSpec, dist_spec: _DistSpec,
                   pg: ProcessGroup) -> torch.Tensor:
         """_shard_as: shard the tensor w.r.t a distributed specification.
         Assuming the tensor passed in is a global (replicated) tensor.
         Args:
             tensor (torch.Tensor): a global (replicated) tensor before shard
             dist_spec (_DistSpec): the distributed spec. to be sharded as.
-            pg (ProcessGroup): the process group of the corresponding colotensor
+            pg (ProcessGrouo): the process group of the corresponding colotensor
         Returns:
             torch.Tensor: a torch tensor after sharded.
         """
         assert old_dist_spec.placement.value == 'r', f"The old_dist_spec of DistSpecManager._shard_as must be REPLICATE!"
         DistSpecManager._sanity_check(old_dist_spec, dist_spec)
 
         chunk = tensor
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/distspec.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/distspec.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class _DistSpec:
     """_DistSpec
 
     A class indicates Distributed Specification.
     The DistSpec is only works for the tensor parallel process groups.
     Because the dist spec of data parallel process group can be automatically deduced.
-    This is an internal data structure.
+    This is an internal data structrue.
     The API for users should be `ShardSpec` and `ReplicaSpec`.
 
     Args:
         dist_placement_pattern (DistPlacementPattern): the pattern describing how tensors are distributed among processes.
                                                 The dist_placement_pattern is picked from a limited set, now including two patterns: replicate and shard.
         process_group (Optional[ProcessGroup], optional): the process group contains processes. Defaults to None.
     """
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/op_wrapper.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/op_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/param_op_hook.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/param_op_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/process_group.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/process_group.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/shape_consistency.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/shape_consistency.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         assert isinstance(value, bool)
         self._forward_only = value
 
     def get_all_all_gather_spec(self, source_spec: ShardingSpec,
                                 orig_cost_dict: Dict[str, float]) -> Dict[ShardingSpec, float]:
         '''
         Get all valid sharding specs from source_spec with single all-gather operation, and
-        accumulate communication cost on origin cost which will finally be used in auto sharding solver.
+        accumulate commucation cost on origin cost which will finally be used in auto sharding solver.
         For the all-gather operation, we just care about the S dimension.
 
         Argument:
             source_spec(ShardingSpec): the ShardingSpec of the source_spec.
             orig_cost(Dict[str, float]): the original communication cost before this operation.
 
         Return:
@@ -141,15 +141,15 @@
                 pass
         return valid_spec_dict
 
     def get_all_all_to_all_spec(self, source_spec: ShardingSpec,
                                 orig_cost_dict: Dict[str, float]) -> Dict[ShardingSpec, float]:
         '''
         Get all valid sharding specs from source_spec with single all-to-all operation, and
-        accumulate communication cost on origin cost which will finally be used in auto sharding solver.
+        accumulate commucation cost on origin cost which will finally be used in auto sharding solver.
         For the all-to-all operation, we just care about the pairs containing S dimension.
 
         Argument:
             source_spec(ShardingSpec): the ShardingSpec of the source_spec.
             orig_cost(Dict[str, float]): the original communication cost before this operation.
 
         Return:
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/sharding_spec.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/sharding_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 SHARD_COST = 5
 STEP_PENALTY = 6
 NAN = 'nan'
 
 
 class _DimSpec:
     '''
-    Sharding spec for single dimension of the sharded tensor describe the sharding dimension of
+    Sharding spec for single dimension of the sharded tensor decribe the sharding dimension of
     logical device mesh and give a method to compute the difference between them.
     This class is used internally in ShardingSpec.
 
     Argument:
         shard_list(List[int]): if shard_list is None, the dim spec will be 'R' type.
             Otherwise, the element in shard_list means the data will be sharded in that dimension.
     '''
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/tensor_spec.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/tensor_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/tensor/utils.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     We don't allow uncontiguous layout, such as all-gather(S012)->S02 is NOT allowed.
     Therefore, all gather operation just remove the last element in shard list,
     e.g.:
         all-gather(S01) -> S0
 
     Argument:
         target_pair(Tuple[int, List[int]]): The first element is the dimension of tensor to be sharded,
-        and the second element describes which logical axis will be sharded in that dimension.
+        and the second element decribes which logical axis will be sharded in that dimension.
     '''
     _, shard_list = target_pair
     new_shard_list = shard_list[:-1]
 
     return new_shard_list
 
 
@@ -32,25 +32,25 @@
     and simulate the influence of the DimSpec.
 
     We BANNED all representations which shard_list in decreasing order,
     such as S10, so all-to-all(S0, S1) -> RS01 is NOT allowed.
     Therefore, if the behind shard_list is not None, we just extend it to the front shard_list.
     Argument:
         target_pair(Tuple[int, List[int]]): The first element is the dimension of tensor to be sharded,
-        and the second element describes which logical axis will be sharded in that dimension.
+        and the second element decribes which logical axis will be sharded in that dimension.
     e.g.:
         all-to-all(S0, S1) -> [S01, R]
         all-to-all(S0, R) -> [R, S0]
     Otherwise, we extend the front shard_list to behind.
     e.g.:
         all-to-all(R, S1) -> [S1, R]
 
     Argument:
         target_pair(Tuple[int, List[int]]): The first element is the dimension of tensor to be sharded,
-        and the second element describes which logical axis will be sharded in that dimension.
+        and the second element decribes which logical axis will be sharded in that dimension.
     '''
     _, f_shard_list = f_target_pair
     _, b_shard_list = b_target_pair
     if not len(b_shard_list):
         b_shard_list.extend(f_shard_list)
         f_shard_list = []
     else:
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/testing/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/testing/comparison.py` & `colossalai-nightly-2023.4.8/colossalai/testing/comparison.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/testing/pytest_wrapper.py` & `colossalai-nightly-2023.4.8/colossalai/testing/pytest_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/testing/random.py` & `colossalai-nightly-2023.4.8/colossalai/testing/random.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/testing/utils.py` & `colossalai-nightly-2023.4.8/colossalai/testing/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 
 def parameterize(argument: str, values: List[Any]) -> Callable:
     """
     This function is to simulate the same behavior as pytest.mark.parameterize. As
     we want to avoid the number of distributed network initialization, we need to have
     this extra decorator on the function launched by torch.multiprocessing.
 
-    If a function is wrapped with this wrapper, non-parametrized arguments must be keyword arguments,
-    positional arguments are not allowed.
+    If a function is wrapped with this wrapper, non-paramterized arguments must be keyword arguments,
+    positioanl arguments are not allowed.
 
-    Usage::
+    Usgae::
 
         # Example 1:
         @parameterize('person', ['xavier', 'davis'])
         def say_something(person, msg):
             print(f'{person}: {msg}')
 
         say_something(msg='hello')
 
         # This will generate output:
         # > xavier: hello
         # > davis: hello
 
-        # Example 2:
+        # Exampel 2:
         @parameterize('person', ['xavier', 'davis'])
         @parameterize('msg', ['hello', 'bye', 'stop'])
         def say_something(person, msg):
             print(f'{person}: {msg}')
 
         say_something()
 
@@ -106,15 +106,15 @@
 
     Args:
         exception_type (Exception, Optional): The type of exception to detect for rerun
         pattern (str, Optional): The pattern to match the exception message.
             If the pattern is not None and matches the exception message,
             the exception will be detected for rerun
         max_try (int, Optional): Maximum reruns for this function. The default value is 5.
-            If max_try is None, it will rerun forever if exception keeps occurring
+            If max_try is None, it will rerun foreven if exception keeps occurings
     """
 
     def _match_lines(lines, pattern):
         for line in lines:
             if re.match(pattern, line):
                 return True
         return False
@@ -140,15 +140,15 @@
                         continue
                     else:
                         print('Maximum number of attempts is reached or pattern is not matched, no more retrying...')
                         raise e
 
         # Override signature
         # otherwise pytest.mark.parameterize will raise the following error:
-        # function does not use argument xxx
+        # function does not use argumetn xxx
         sig = signature(func)
         _run_until_success.__signature__ = sig
 
         return _run_until_success
 
     return _wrapper
 
@@ -227,15 +227,15 @@
 
 
 def spawn(func, nprocs=1, **kwargs):
     """
     This function is used to spawn processes for testing.
 
     Usage:
-        # must contains arguments rank, world_size, port
+        # must contians arguments rank, world_size, port
         def do_something(rank, world_size, port):
             ...
 
         spawn(do_something, nprocs=8)
 
         # can also pass other arguments
         def do_something(rank, world_size, port, arg1, arg2):
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/trainer/_trainer.py` & `colossalai-nightly-2023.4.8/colossalai/trainer/_trainer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/trainer/hooks/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/trainer/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/trainer/hooks/_base_hook.py` & `colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_base_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/trainer/hooks/_checkpoint_hook.py` & `colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_checkpoint_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/trainer/hooks/_log_hook.py` & `colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_log_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/trainer/hooks/_lr_scheduler_hook.py` & `colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_lr_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/trainer/hooks/_metric_hook.py` & `colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_metric_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/activation_checkpoint.py` & `colossalai-nightly-2023.4.8/colossalai/utils/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/checkpoint/module_checkpoint.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint/module_checkpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         epoch (int): the number of epoch
         model (torch.nn.Module): a torch module initialized by ColoInitContext
         optimizer (ColossalaiOptimizer, optional): optimizers. Defaults to None.
         lr_scheduler (torch.optim.lr_scheduler._LRScheduler, optional): lr schedule. Defaults to None.
         torch_load_kwargs: (dict, optional): The kwargs of torch.load inside the function
         load_state_dict_kwargs (dict, optional): The kwargs of load_state_dict inside the function
     """
-    # initialize the default parameters
+    # initialize the default paramters
     if not torch_load_kwargs:
         torch_load_kwargs = dict()
     if not load_state_dict_kwargs:
         load_state_dict_kwargs = dict()
 
     rank = dist.get_rank()
     mapping = dict()
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/checkpoint/utils.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             if dist.get_rank() != 0:
                 colo_tensor.set_dist_spec(old_dist_spec)
 
         # synchronize all processes for unexpected problems
         dist.barrier()
 
     if dist.get_rank() == 0:
-        setattr(colo_tensor, 'save_ready', True)    # set saving signature
+        setattr(colo_tensor, 'save_ready', True)    # set saving signitrue
 
 
 def scatter_tensor(colo_tensor: ColoTensor, dist_spec: _DistSpec) -> None:
     """Reversal operation of `gather_tensor`.
     """
     if dist_spec.placement == DistPlacementPattern.REPLICATE:
         robust_broadcast(colo_tensor.data)
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/backend.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/backend.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/convertor.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/convertor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/distributed.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/distributed.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/io.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/io.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/meta.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/meta.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/reader.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/reader.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/utils.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/checkpoint_io/writer.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/writer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/checkpointing.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpointing.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/common.py` & `colossalai-nightly-2023.4.8/colossalai/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/cuda.py` & `colossalai-nightly-2023.4.8/colossalai/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/data_sampler/data_parallel_sampler.py` & `colossalai-nightly-2023.4.8/colossalai/utils/data_sampler/data_parallel_sampler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/memory.py` & `colossalai-nightly-2023.4.8/colossalai/utils/memory.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/model/experimental.py` & `colossalai-nightly-2023.4.8/colossalai/utils/model/experimental.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 import torch
 import torch.distributed as dist
 import torch.nn as nn
 from torch import Tensor
 from torch.utils._pytree import tree_map
 
-from colossalai._analyzer._subclasses import MetaTensor
+from colossalai.fx.profiler.tensor import MetaTensor
 from colossalai.tensor.d_tensor.d_tensor import DTensor
 from colossalai.tensor.d_tensor.layout import Layout
 
 # reference: https://pytorch.org/cppdocs/notes/tensor_creation.html
 _NORMAL_FACTORY = [
     "arange",
-    "full",
     "empty",
+    "full",
     "linspace",
     "logspace",
     "ones",
     "rand",
     "randn",
     "randint",
     "randperm",
@@ -33,15 +33,15 @@
 ]
 
 _EARLY_MATERIALIZED_OPS = ['__getitem__', 'split']
 
 # If your intent is to change the metadata of a Tensor (such as sizes / strides / storage / storage_offset)
 # without autograd tracking the change, remove the .data / .detach() call and wrap the change in a `with torch.no_grad():` block.
 # These ops cannot be unwrapped using .data
-_CHANGE_META_OPS = ['_cudnn_rnn_flatten_weight', 'requires_grad_', '__get__', '__set__']
+_CHANGE_META_OPS = ['_cudnn_rnn_flatten_weight', 'requires_grad_', '__get__']
 
 _LEGACY_TENSOR_CONSTRUCTOR = {
     'FloatTensor': torch.float,
     'DoubleTensor': torch.double,
     'HalfTensor': torch.half,
     'BFloat16Tensor': torch.bfloat16,
     'ByteTensor': torch.uint8,
@@ -71,20 +71,14 @@
 
     @classmethod
     def __torch_function__(cls, func, types, args=(), kwargs=None):
         cls._pre_op_fn()
         return super().__torch_function__(func, types, args, kwargs)
 
 
-def _data_tolist(tensor: torch.Tensor) -> list:
-    """tolist() method is not allowed for a subclass of tensor. Tensor.data returns a Tensor.
-    """
-    return tensor.data.tolist()
-
-
 def _convert_cls(tensor: 'LazyTensor', target: torch.Tensor) -> torch.Tensor:
     """Convert a lazy tensor's class to target's class, with target's data.
 
     The reason why we change the class of a lazy tensor in-place is that this can easily handle shared modules/parameters, which is common in huggingface models.
     If we create a new tensor and update the module by ``setattr(module, name, param)``, the shared parameters will not be updated. And we have to track all shared parameters and update them manually.
 
     Args:
@@ -96,15 +90,15 @@
     """
     cls_to_become = nn.Parameter if isinstance(tensor, nn.Parameter) else torch.Tensor
     tensor.__class__ = cls_to_become
     tensor.data = target
     tensor.requires_grad = target.requires_grad
     # subclass of torch.Tensor does not have tolist() method
     # overwrite this method after materialization or distribution
-    tensor.tolist = MethodType(_data_tolist, tensor)
+    tensor.tolist = MethodType(torch.Tensor.tolist, target)
     return tensor
 
 
 class LazyTensor(torch.Tensor):
     """A naive implementation of LazyTensor (https://arxiv.org/pdf/2102.13267.pdf).
 
     Usage:
@@ -146,15 +140,15 @@
         if concrete_data is not None:
             # some ops don't support meta backend and should have concrete data
             elem = concrete_data
         else:
             if meta_data is None:
                 device = kwargs.get('device', 'cpu')
                 elem = func(*args, **{**kwargs, 'device': 'meta'})
-                meta_data = MetaTensor(elem, device=device)
+                meta_data = MetaTensor(elem, fake_device=device)
             elem = meta_data._tensor
         # As a meta tensor cannot be modified __class__ to torch.Tensor, we should use an empty real tensor here
         r = torch.Tensor._make_subclass(cls, _EMPTY_DATA, require_grad=elem.requires_grad)
         r._meta_data = meta_data
         return r
 
     def __init__(self, func, *args, meta_data=None, concrete_data=None, **kwargs):
@@ -257,15 +251,15 @@
         if kwargs is None:
             kwargs = {}
         if func.__name__ in _EARLY_MATERIALIZED_OPS:
             # These OPs cannot be lazy and related tensors should be early materialized
             tree_map(cls._replace_with_materialized, args)
             tree_map(cls._replace_with_materialized, kwargs)
         is_inplace: bool = (func.__name__.endswith('_') and not (func.__name__.endswith('__'))
-                            or func.__name__ in ('__setitem__', '__set__'))
+                            or func.__name__ == "__setitem__")
 
         is_change_meta_op: bool = func.__name__ in _CHANGE_META_OPS
 
         if isinstance(func, torch._C.ScriptMethod):
             # FIXME(ver217): torch script functions are not verified
 
             target = None
@@ -320,45 +314,23 @@
     @classmethod
     def __torch_dispatch__(cls, func, types, args=(), kwargs=None):
         pass    # skip
 
     def clone(self) -> "LazyTensor":
 
         def factory_fn():
-            # if self is materialized, return self
-            new_tensor = self.materialize() if type(self) is LazyTensor else self
-            return new_tensor.clone()
+            return self.materialize().clone()
 
         target = LazyTensor(factory_fn, meta_data=self._meta_data)
 
         return target
 
     def detach(self) -> Tensor:
         return self
 
-    def __deepcopy__(self, memo):
-        if not self.is_leaf:
-            raise RuntimeError("Only Tensors created explicitly by the user "
-                               "(graph leaves) support the deepcopy protocol at the moment")
-        if id(self) in memo:
-            return memo[id(self)]
-
-        def factory_fn():
-            # if self is materialized, return self
-            new_tensor = self.materialize() if type(self) is LazyTensor else self
-            copied = new_tensor.detach().clone()
-            if new_tensor.requires_grad:
-                copied.requires_grad_()
-            return copied
-
-        target = LazyTensor(factory_fn, meta_data=self._meta_data)
-
-        memo[id(self)] = target
-        return target
-
     @property
     def data(self):
         return self
 
     @data.setter
     def data(self, other: 'LazyTensor'):
         """This is sightly different from oringinal `data` setter.
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/model/lazy_init_context.py` & `colossalai-nightly-2023.4.8/colossalai/utils/model/lazy_init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/model/utils.py` & `colossalai-nightly-2023.4.8/colossalai/utils/model/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/moe.py` & `colossalai-nightly-2023.4.8/colossalai/utils/moe.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     Args:
         model (:class:`torch.nn.Module`): A pyTorch model on whose parameters you check the consistency.
     """
     if is_using_ddp():
 
         param_dict = get_moe_epsize_param_dict(model)
 
-        # synchronize the parameters whose dp_group is the whole world
+        # synchrosize the parameters whose dp_group is the whole world
         if 1 in param_dict:
             src_rank = gpc.get_ranks_in_group(ParallelMode.DATA)[0]
             for param in param_dict[1]:
                 dist.broadcast(param, src=src_rank, group=gpc.get_group(ParallelMode.DATA))
 
         for ep_size in param_dict:
             # When ep_size = world_size, communication is not needed
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py` & `colossalai-nightly-2023.4.8/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/profiler/legacy/comm_profiler.py` & `colossalai-nightly-2023.4.8/colossalai/utils/profiler/legacy/comm_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/profiler/legacy/pcie_profiler.py` & `colossalai-nightly-2023.4.8/colossalai/utils/profiler/legacy/pcie_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/profiler/legacy/prof_utils.py` & `colossalai-nightly-2023.4.8/colossalai/utils/profiler/legacy/prof_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/profiler/profiler.py` & `colossalai-nightly-2023.4.8/colossalai/utils/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/profiler/stateful_tensor_mem_extention.py` & `colossalai-nightly-2023.4.8/colossalai/utils/profiler/stateful_tensor_mem_extention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/rank_recorder/rank_recorder.py` & `colossalai-nightly-2023.4.8/colossalai/utils/rank_recorder/rank_recorder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/tensor_detector/tensor_detector.py` & `colossalai-nightly-2023.4.8/colossalai/utils/tensor_detector/tensor_detector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/utils/timer.py` & `colossalai-nightly-2023.4.8/colossalai/utils/timer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/zero/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/chunk/chunk.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/chunk.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/chunk/manager.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/chunk/search_utils.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/search_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,16 @@
 
 from colossalai.tensor import ColoParameter
 from colossalai.utils import is_ddp_ignored
 from colossalai.zero.gemini.memory_tracer import MemStats, OrderedParamGenerator
 
 
 def _filter_exlarge_params(model: nn.Module, size_dict: Dict[int, List[int]]) -> None:
-    """_filter_exlarge_params
-
+    """
     Filter those parameters whose size is too large (more than 3x standard deviations) from others.
-
-    Args:
-        model (nn.Module): the model.
-        size_dict (Dict[int, List[int]]): the size dict of parameters.
     """
     agg_size_list = []
     for key in size_dict:
         agg_size_list.extend(size_dict[key])
 
     if len(agg_size_list) == 0:
         return
@@ -34,77 +29,53 @@
 
     for key in size_dict:
         org_list = size_dict[key]
         size_dict[key] = list(filter(lambda x: x <= upper_limit, org_list))
 
 
 def _get_unused_byte(size_list: List[int], chunk_size: int) -> int:
-    """_get_unused_byte
-
-    Get unused byte for a certain chunk size.
-
-    Args:
-        size_list (List[int]): the size list of parameters.
-        chunk_size (int): the chunk size.
-
-    Returns:
-        int: the unused byte.
+    """Get unused byte for a certain chunk size.
     """
     acc = 0
     left = 0
     for s in size_list:
         if s > left:
             acc += left
             left = chunk_size
         left -= s
     return left + acc
 
 
-def _tensor_numel(local_param: ColoParameter, strict_ddp_flag: bool) -> int:
-    """_tensor_numel
-
-    Get the number of elements of a tensor.
-
-    Args:
-        local_param (ColoParameter): The local parameter.
-        strict_ddp_flag (bool): whether to enable the strict ddp mode.
-
-    Returns:
-        int: the number of elements.
-    """
-    if strict_ddp_flag and type(local_param) is ColoParameter:
+def _tensor_numel(local_param: ColoParameter, strict_ddp_flag: bool):
+    if strict_ddp_flag:
         return local_param.numel_global()
     else:
-        # if local_param is not ColoParameter, we assume it's replicated
         return local_param.numel()
 
 
 def classify_params_by_dp_degree(param_order: OrderedParamGenerator,
                                  strict_ddp_flag: bool = False) -> Dict[int, List[ColoParameter]]:
     """classify_params_by_dp_degree
 
     Classify the parameters by their dp degree
 
     Args:
         param_order (OrderedParamGenerator): the order of param be visied
-        strict_ddp_flag (bool, optional): whether to enable the strict ddp mode. Defaults to False.
 
     Returns:
         Dict[int, List[ColoParameter]]: a dict contains the classification results.
         The keys are dp_degrees and the values are parameters.
     """
     params_dict: Dict[int, List[ColoParameter]] = dict()
     for param in param_order.generate():
-        # assert isinstance(param, ColoParameter), "please init model in the ColoInitContext"
+        assert isinstance(param, ColoParameter), "please init model in the ColoInitContext"
         if is_ddp_ignored(param):
             continue
 
-        if strict_ddp_flag or type(param) is not ColoParameter:
-            # if model is not initialized with ColoInitContext, we assume it's replicated
-            # TODO(ver217): integrate DTensor
+        if strict_ddp_flag:
             param_key = dist.get_world_size()
         else:
             param_key = param.process_group.dp_world_size()
 
         if param_key not in params_dict:
             params_dict[param_key] = []
         params_dict[param_key].append(param)
@@ -118,16 +89,14 @@
         search_interval_byte: int,    # hidden size is the best value for the interval
         min_chunk_size_mb: float = 32,
         filter_exlarge_params: bool = True,
         strict_ddp_flag: bool = False,
         memstas: Optional[MemStats] = None) -> Tuple[Dict, int, int]:
     """search_chunk_configuration
 
-    Search the chunk configuration for a model.
-
     Args:
         model (nn.Module): torch module
         search_range_mb (float): searching range in mega byte.
         search_interval_byte (int): searching interval in byte.
         min_chunk_size_mb (float, optional): the minimum size of a distributed chunk.
         filter_exlarge_params (bool, optional): filter extreme large parameters. Defaults to True.
         strict_ddp_flag (bool, optional): whether to enable the strict ddp mode.
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/chunk/utils.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,14 @@
         return 0
     return a / b
 
 
 def init_chunk_manager(model: nn.Module,
                        init_device: Optional[torch.device] = None,
                        hidden_dim: Optional[int] = None,
-                       verbose: bool = False,
                        **kwargs) -> ChunkManager:
     if hidden_dim:
         search_interval_byte = hidden_dim
     else:
         search_interval_byte = 1024    # defaults to 1kb
     kwargs["search_interval_byte"] = search_interval_byte
 
@@ -36,15 +35,15 @@
     dist.barrier()
     end = time()
     span_s = end - begin
     mb_size = 1024**2
     total_size /= mb_size
     wasted_size /= mb_size
 
-    if verbose and dist.get_rank() == 0:
+    if dist.get_rank() == 0:
         print("searching chunk configuration is completed in {:.2f} s.\n".format(span_s),
               "used number: {:.2f} MB, wasted number: {:.2f} MB\n".format(total_size, wasted_size),
               "total wasted percentage is {:.2f}%".format(100 * safe_div(wasted_size, total_size + wasted_size)),
               sep='',
               flush=True)
     dist.barrier()
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/colo_init_context.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/colo_init_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                  device: torch.device = torch.device('cpu'),
                  dtype: torch.dtype = torch.float,
                  default_pg: Optional[ProcessGroup] = None,
                  default_dist_spec=None):
         """
         Args:
             device (torch.device): the device where parameters initialized are resident. Defaults to torch.device('cpu').
-            dtype (torch.dtype): the dtype of parameters initialized. Defaults to torch.float.
+            dtype (torch.dtype): the dtype of parameters initialized. Defults to torch.float.
             default_pg (ProcessGroup): the default process group for all initialized parameters.
             default_dist_spec: the default distributed specifications.
         """
         super().__init__()
         self._device = device
         self._dtype = dtype
 
@@ -160,15 +160,15 @@
 
     This function is called after `ColoInitContext`.
 
     Args:
         model (torch.nn.module): the model
         device (torch.device, optional): device type of the model params. Defaults to torch.device('cpu').
         dtype (torch.dtype, optional): dtype of the model params. Defaults to torch.float.
-        default_pg (Optional[ProcessGroup], optional): default process group. Defaults to None. Indicates a DP-only process group.
+        default_pg (Optional[ProcessGroup], optional): default process group. Defaults to None. Inidicates a DP-only process group.
         default_dist_spec (Any, optional): default dist spec of params. Defaults to None.
 
     Raises:
         RuntimeError: raise error if
     """
 
     torch_params = []
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/gemini_ddp.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/sharded_model_v2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,409 +1,473 @@
+# this code is inspired by the DeepSpeed library and implemented with our own design from scratch
+import functools
 import itertools
 from collections import OrderedDict
-from contextlib import nullcontext
-from functools import partial
-from typing import Dict, Iterator, List, Optional, Union
+from copy import deepcopy
+from typing import Any, Iterator, Optional, Tuple
 
 import torch
 import torch.distributed as dist
 import torch.nn as nn
+from torch.distributed import ProcessGroup
+from torch.nn.parameter import Parameter
 
-from colossalai.checkpoint_io.utils import calculate_tensor_size
+from colossalai.context.parallel_mode import ParallelMode
+from colossalai.core import global_context as gpc
 from colossalai.logging import get_dist_logger
-from colossalai.nn.parallel.data_parallel import ColoDDP, _cast_float, free_storage
-from colossalai.tensor import ProcessGroup as ColoProcessGroup
-from colossalai.tensor import ReplicaSpec
-from colossalai.tensor.colo_parameter import ColoParameter, ColoTensor, ColoTensorSpec
-from colossalai.tensor.param_op_hook import ColoParamOpHookManager
-from colossalai.utils import get_current_device, is_ddp_ignored
-from colossalai.utils.model.experimental import LazyTensor
-
-from .chunk import Chunk, ChunkManager, TensorState, init_chunk_manager
-from .gemini_hook import GeminiZeROHook
-from .gemini_mgr import GeminiManager
-from .memory_tracer import MemStats, OrderedParamGenerator
-from .utils import get_temp_total_chunk_on_cuda
+from colossalai.utils import disposable, get_current_device
+from colossalai.utils.memory import colo_device_memory_capacity
+from colossalai.zero.gemini.memory_tracer import MemStatsCollector, StaticMemStatsCollector
+from colossalai.zero.legacy.gemini.ophooks import register_ophooks_recursively
+from colossalai.zero.legacy.gemini.paramhooks import BaseParamHookMgr
+from colossalai.zero.legacy.gemini.stateful_tensor import TensorState
+from colossalai.zero.legacy.gemini.stateful_tensor_mgr import StatefulTensorMgr
+from colossalai.zero.legacy.gemini.tensor_placement_policy import TensorPlacementPolicy, TensorPlacementPolicyFactory
+from colossalai.zero.legacy.gemini.tensor_utils import colo_model_data_move_to_cpu
+from colossalai.zero.legacy.shard_utils import BaseShardStrategy
+from colossalai.zero.legacy.sharded_model.reduce_scatter import ReduceScatterBucketer
+
+from ._utils import (
+    cast_float_arguments,
+    cast_tensor_to_fp16,
+    cast_tensor_to_fp32,
+    chunk_and_pad,
+    free_storage,
+    get_gradient_predivide_factor,
+)
+from .zero_hook import ZeroHook
 
 try:
-    from torch.nn.modules.module import _EXTRA_STATE_KEY_SUFFIX, _IncompatibleKeys
+    from torch.nn.modules.module import _EXTRA_STATE_KEY_SUFFIX
 except ImportError:
     _EXTRA_STATE_KEY_SUFFIX = '_extra_state'
 
-__all__ = [
-    'ZeroDDP',
-    'GeminiDDP',
-]
 
-
-class ZeroDDP(ColoDDP):
-    """ZeRO DDP for ColoTensor.
-    Warning: Nested ZeroDDP is not supported now.
-    It is designed to be used with ChunkManager and GeminiManager.
-    For more details, see the API reference of ``ChunkManager`` and ``GeminiManager``.
+class ShardedModelV2(nn.Module):
+    """
+    A wrapper for the PyTorch module shards the model parameters among multiple GPU memory.
+    Only `1/#nproc` of parameters, gradients are stored in local CUDA memory, so forward and backward
+    passes can be executed with limited CUDA memory budget.
+
+    Note:
+        You must use ``ShardedModelV2`` with ``ShardedOptimizerV2``.
+    Note:
+        Make sure you don't use gradient accumulation and your optimizer can work with fp16 gradient and fp32 parameter,
+        if you enable ``reuse_fp16_shard``.
 
     Args:
-        module (torch.nn.Module): Module to apply ZeRO-DP.
-        gemini_manager (GeminiManager): Manages the chunk manager and heterogeneous memory space.
-            For more details, see the API reference of ``GeminiManager``.
-        pin_memory (bool): Chunks on CPU Memory use pin-memory.
-        force_outputs_fp32 (bool): If set to True, outputs will be fp32. Otherwise, outputs will be fp16.
-            Defaults to False.
-        strict_ddp_mode (bool): If set to True, there is no tensor sharding, each tensor is replicated.
-            Defaults to False. Users can set it to True, when they clearly know that they only need DDP.
-        scatter_after_inference (bool): If set to True, the model will be scattered after inference. This will save memory but slow down the consecutive inference.
+        module (nn.Module): A sharded module, which must be initialized by `ZeroInitContext`.
+        shard_strategy (BaseShardStrategy): A shard strategy to manage shard behavior.
+        process_group (Optional[ProcessGroup], optional): Data parallel process group. Defaults to None.
+        reduce_scatter_process_group (Optional[ProcessGroup], optional): Reduce-scatter process group.
+            Generally, it should be `None`, and it's the same as `process_group`. Defaults to None.
+        reduce_scatter_bucket_size_mb (int, optional): Reduce-scatter bucket size in *MB*. Defaults to 25.
+        fp32_reduce_scatter (bool, optional): If set to `True`, gradients are forced to FP32 before reduce-scatter. Defaults to False.
+        tensor_placement_policy (str): Which device to place *held* tensors. It can be 'cpu', 'cuda' and 'auto'.
+            If it's 'cpu', parameters, gradients and optimizer states will be offloaded to CPU, which means min CUDA memory will be used.
+            If it's 'cuda', they won't be offloaded, which means max CUDA memory will be used.
+            If it's 'auto', they are moving dynamically based on CPU and CUDA memory usage. It will utilize heterogeneous memory space evenly and well.
+            Note that 'auto' policy can only work well when no other processes use CUDA during your training.
+            Defaults to 'cuda'.
+        gradient_predivide_factor (Optional[float], optional): Gradient is divived by this value before reduce-scatter. Defaults to 1.0.
+        reuse_fp16_shard (bool, optional): Whether to reuse fp16 shard for param and grad.
+            Enabling this can reduce GPU memory usage, but you have to make sure you disable it when using gradient accumulation.
+            In this mode, grad will be fp16. Make sure your optimizer supports mixed precision (fp32 param and fp16 grad).
+            We find that PyTorch's optimizers don't support mixed precision,
+            so we recommend you enable this only when using our CPUAdam with CPU offload. Defaults to False.
     """
 
     def __init__(self,
-                 module: torch.nn.Module,
-                 gemini_manager: GeminiManager,
-                 pin_memory: bool = False,
-                 force_outputs_fp32: bool = False,
-                 strict_ddp_mode: bool = False,
-                 scatter_after_inference: bool = True) -> None:
-        self.gemini_manager = gemini_manager
-        self.chunk_manager: ChunkManager = gemini_manager.chunk_manager
-        self.force_outputs_fp32 = force_outputs_fp32
-        self.param_op_hook = GeminiZeROHook(gemini_manager)
-        self.fp32_params: List[ColoTensor] = list()
-        self.fp16_params: List[ColoParameter] = list()
-        self.overflow_counter = 0
-        self.grads_device: Dict[torch.Tensor, torch.device] = dict()
-        self.param2name: Dict[nn.Parameter, str] = dict()
-        self.name2param: Dict[str, nn.Parameter] = dict()
-        self.scatter_after_inference = scatter_after_inference
-
-        self._logger = get_dist_logger()
-
-        if self.gemini_manager._premade_memstats_:
-            # build chunk in param runtime visited order.
-            param_order = self.gemini_manager.memstats()._param_runtime_order
-        else:
-            # build chunk in param initialized order.
-            # Note: in this way, it can not get filter unused params during runtime.
-            param_order = OrderedParamGenerator()
-            for p in module.parameters():
-                param_order.append(p)
-
-        self._init_chunks(param_order=param_order,
-                          strict_ddp_mode=strict_ddp_mode,
-                          cpu_offload=self.gemini_manager.policy_name != 'cuda',
-                          pin_memory=pin_memory)
-
-        for name, param in module.named_parameters():
-            self.param2name[param] = name
-        for m_name, m_var in module.named_modules():
-            for p_name, p_var in m_var.named_parameters(recurse=False):
-                param_name = m_name + '.' + p_name if m_name else p_name
-                self.name2param[param_name] = p_var
-        super().__init__(module, process_group=ColoProcessGroup())
-        self._cast_buffers()
-
-    def _post_forward(self):
-        """This function is only triggered for inference.
-        """
-        access_list = list(self.chunk_manager.accessed_chunks)
-        # we need to scatter all accessed chunks and move them to their original places
-        for chunk in access_list:
-            if chunk.keep_gathered:
-                self.chunk_manager.fake_release_chunk(chunk)
+                 module: nn.Module,
+                 shard_strategy: BaseShardStrategy,
+                 process_group: Optional[ProcessGroup] = None,
+                 reduce_scatter_process_group: Optional[ProcessGroup] = None,
+                 reduce_scatter_bucket_size_mb: int = 25,
+                 fp32_reduce_scatter: bool = False,
+                 tensor_placement_policy: str = 'cuda',
+                 gradient_predivide_factor: Optional[float] = 1.0,
+                 reuse_fp16_shard: bool = False,
+                 *args,
+                 **kwargs):
+        assert not isinstance(module, ShardedModelV2), 'Nested ShardedModelV2 is not supported.'
+        super().__init__()
+        self.logger = get_dist_logger()
+
+        # We force users to use ZeroInitContext
+        for submodule in module.modules():
+            sharded_cnt = 0
+            unshard_cnt = 0
+            for param in submodule.parameters(recurse=False):
+                assert hasattr(param, 'colo_attr'), 'You must use ZeroInitContext to init your module first.'
+                if param.colo_attr.param_is_sharded:
+                    sharded_cnt += 1
+                else:
+                    unshard_cnt += 1
+            assert (not sharded_cnt) or (not unshard_cnt), 'nn.Module can not both have shard param and unshard param'
+            submodule.param_is_sharded = (sharded_cnt > 0)
+
+        self.sharded_params = []
+        self.unshard_params = []
+        for param in module.parameters():
+            if param.colo_attr.param_is_sharded:
+                self.sharded_params.append(param)
             else:
-                assert chunk.can_release
-                self.chunk_manager.release_chunk(chunk)
-            first_param = next(iter(chunk.tensors_info))
-            self.chunk_manager.move_chunk(chunk, self.grads_device[first_param])
-        assert self.chunk_manager.accessed_mem == 0
-
-    def forward(self, *args, **kwargs):
-        # check whether we are in a inference mode
-        grad_flag = torch.is_grad_enabled()
-        if not grad_flag:
-            assert not self.gemini_manager.need_warmup or not self.gemini_manager.is_warmup(
-            ), "You should run a completed iteration as your warmup iter"
-
-        args, kwargs = _cast_float(args, torch.half), _cast_float(kwargs, torch.half)
-        self.module.zero_grad(set_to_none=True)
-        if not grad_flag:
-            outputs = self._inference_forward(*args, **kwargs)
+                self.unshard_params.append(param)
+
+        self.module = module
+        self.process_group = process_group or gpc.get_group(ParallelMode.DATA)
+        self.reduce_scatter_process_group = reduce_scatter_process_group or self.process_group
+        self.world_size = dist.get_world_size(self.process_group)
+        self.rank = dist.get_rank(self.process_group)
+        self.shard_strategy = shard_strategy
+
+        self._use_memory_tracer = tensor_placement_policy == 'auto'
+        if self._use_memory_tracer:
+            self._memstats_collector = MemStatsCollector()
+            self._start_collect_memstats = disposable(self._memstats_collector.start_collection)
+            self._finish_collect_memstats = disposable(self._memstats_collector.finish_collection)
         else:
-            self.gemini_manager.pre_iter(*args)
-            with ColoParamOpHookManager.use_hooks(self.param_op_hook):
-                outputs = self.module(*args, **kwargs)
+            self._memstats_collector = None
+        self._tensor_placement_policy: TensorPlacementPolicy = TensorPlacementPolicyFactory.create(
+            tensor_placement_policy)(mem_stats_collector=self._memstats_collector)
+
+        if 'warmup_non_model_data_ratio' in kwargs:
+            if tensor_placement_policy != 'auto':
+                self.logger.warning('setting warmup_non_model_data_ratio is useless if not use auto placement')
+            else:
+                ratio = kwargs['warmup_non_model_data_ratio']
+                self._tensor_placement_policy._warmup_non_model_data_ratio = ratio
+                self.logger.info(f'setting warmup_non_model_data_ratio as {ratio} for auto placement')
+
+        self._stateful_tensor_mgr = StatefulTensorMgr(self._tensor_placement_policy)
+        param_tensor_list = [p.colo_attr.sharded_data_tensor for p in module.parameters() if hasattr(p, 'colo_attr')]
+        self._stateful_tensor_mgr.register_stateful_tensor_list(param_tensor_list)
+
+        # Register hooks
+        self._ophook_list = [
+            ZeroHook(self.shard_strategy, self._memstats_collector, self._stateful_tensor_mgr, self.process_group)
+        ]
+        register_ophooks_recursively(self.module, self._ophook_list)
+        self.param_hook_mgr = BaseParamHookMgr(list(self.module.parameters()))
+        self.param_hook_mgr.register_backward_hooks(self._grad_post_backward_hook)
+
+        self.fp32_reduce_scatter = fp32_reduce_scatter
+        self._cpu_offload: bool = tensor_placement_policy != 'cuda'
+        for param in module.parameters():
+            # Init `offload_grad`
+            param.colo_attr.offload_grad = self._cpu_offload
+
+        # We find if gradient_predivide_factor != 1.0, there may be wrong precision problem
+        # So we use 1.0 as the default gradient_predivide_factor
+        # However, if you set gradient_predivide_factor to None, we will set
+        # gradient_predivide_factor to a value >= 1.0 automatically
+        self.gradient_predivide_factor: float = gradient_predivide_factor if \
+            gradient_predivide_factor is not None else \
+            get_gradient_predivide_factor(self.world_size)
+        self.gradient_postdivide_factor: float = self.world_size / self.gradient_predivide_factor
+
+        self.comm_stream: torch.cuda.Stream = torch.cuda.Stream()
+        self.reducer = ReduceScatterBucketer(reduce_scatter_bucket_size_mb)
+        self._require_backward_grad_sync: bool = True
 
-        if self.force_outputs_fp32:
-            return _cast_float(outputs, torch.float)
-        return outputs
+        self._cuda_margin_space = 0
+        self.reuse_fp16_shard = reuse_fp16_shard
 
-    def _inference_forward(self, *args, **kwargs):
-        """This function is only triggered for inference.
-        """
-        fwd_ctx = ColoParamOpHookManager.use_hooks(self.param_op_hook)
-        if not self.scatter_after_inference:
-            # gather all chunks
-            for chunk in self.chunk_manager.get_chunks(self.fp16_params):
-                self.chunk_manager.access_chunk(chunk)
-            fwd_ctx = nullcontext()
-        with fwd_ctx:
-            outputs = self.module(*args, **kwargs)
-        if self.scatter_after_inference:
-            # scatter chunks
-            self._post_forward()
-        # reset all recorded attributes
-        self.gemini_manager.reset_attributes()
-        return outputs
-
-    def _setup_grads_ptr(self):
-        for p in self.module.parameters():
-            if is_ddp_ignored(p):
-                continue
-            p.grad = None
+        # record whether gradients have inf or nan
+        self.overflow_counter = 0
 
-    def _pre_backward(self):
-        # set a visit label for all parameters
-        # the label is used to check whether the parameter is correctly reduced
-        for param in self.param2name:
-            if not is_ddp_ignored(param):
-                setattr(param, "_gemini_reduced", False)
-
-    def _post_backward(self):
-        if self.chunk_manager.accessed_mem != 0:
-            error_params = ["Reduction failed at followed parameters:"]
-            for param in self.param2name:
-                if not is_ddp_ignored(param) and not getattr(param, "_gemini_reduced"):
-                    error_params.append(self.param2name[param])
-            error_str = "\n\t".join(error_params)
-            raise RuntimeError("ZERO DDP error: the synchronization of gradients doesn't exit properly.",
-                               "The most possible reason is that the model is not compatible with ZeroDDP.\n",
-                               f"{error_str}")
-        self._setup_grads_ptr()
-        self._logger.debug(
-            f'comp cuda demand time: {self.gemini_manager._comp_cuda_demand_time}, layout time: {self.gemini_manager._layout_time}, evict time: {self.gemini_manager._evict_time}, CPU->CUDA vol: {self.gemini_manager._h2d_volume}B, CUDA->CPU vol: {self.gemini_manager._d2h_volume}'
-        )
-        self.gemini_manager.post_iter()
-
-    def backward(self, loss: torch.Tensor):
-        self._pre_backward()
-        with self.param_op_hook.switch_to_backward(), ColoParamOpHookManager.use_hooks(self.param_op_hook):
-            loss.backward()
-        self._post_backward()
+    def adjust_stateful_tensor_layout(self) -> None:
+        self._stateful_tensor_mgr.adjust_layout()
 
-    def backward_by_grad(self, tensor, grad):
-        with self.param_op_hook.switch_to_backward(), ColoParamOpHookManager.use_hooks(self.param_op_hook):
-            torch.autograd.backward(tensor, grad)
-        self._post_backward()
+    @property
+    def use_memory_tracer(self):
+        return self._use_memory_tracer
+
+    @property
+    def cuda_margin_space(self):
+        return self._cuda_margin_space
+
+    @property
+    def cpu_offload(self):
+        return self._cpu_offload
+
+    def dump_memory_stats(self, filename: Optional[str] = 'dump_mem_stats.log') -> None:
+        """
+        dummy memory tracer collected infomation to a file.
+        try:
+            # forward: model(inputs)
+            # backward: optimizer.backward()
+        except Exception as e:
+            model.dump_memory_stats()
+            exit(0)
+        """
+        if self._use_memory_tracer:
+            self.logger.error(f'dump memort tracer collected infomation to a {filename}', ranks=[0])
+            if gpc.get_global_rank() == 0:
+                with open(filename, 'w+') as f:
+                    f.write(f'cuda reserved {torch.cuda.memory_reserved(get_current_device()) / 1e9} GB\n')
+                    f.write(f'cuda max allocated {torch.cuda.max_memory_allocated(get_current_device()) / 1e9} GB\n')
+                    f.write('CUDA model data (GB)\n')
+                    f.write('\n')
+                    f.write('CUDA non model data (GB)\n')
+                    f.write(str(self._memstats_collector._memstats.non_model_data_list('cuda')))
+                    f.write('CPU non model data (GB)\n')
+                    f.write(str(self._memstats_collector._memstats.non_model_data_list('cpu')))
+                    f.write('\n')
+
+    def _pre_forward_operations(self, *args):
+        # the operation will affect the memory tracer behavior in ZeroHook
+        if self._memstats_collector:
+            self._start_collect_memstats()
 
-    def grad_handle(self, p, grad):
-        empty_grad = torch.empty_like(grad)
-        free_storage(empty_grad)
-        with torch._C.DisableTorchFunction():
-            chunk = self.chunk_manager.get_chunk(p)
-            if chunk.tensors_info[p].state != TensorState.HOLD_AFTER_BWD:
-                raise RuntimeError(f"Parameter `{self.param2name[p]}` failed at the gradient reduction. "
-                                   "Some unsupported torch function is operated upon this parameter.")
-            self.chunk_manager.trans_tensor_state(p, TensorState.READY_FOR_REDUCE)
-            chunk.copy_tensor_to_chunk_slice(p, grad)
-            reduced = self.chunk_manager.reduce_chunk(chunk)
-            if reduced:
-                if chunk.is_gathered:
-                    chunk.cuda_global_chunk.div_(chunk.pg_size)
-                else:
-                    chunk.cuda_shard.div_(chunk.pg_size)
-                # check overflow elements
-                self.overflow_counter += chunk.has_inf_or_nan
-                # record l2 norm for gradient clipping
-                if chunk.l2_norm_flag:
-                    chunk.set_l2_norm()
-                self.chunk_manager.move_chunk(chunk, self.grads_device[p], force_copy=True)
-        return empty_grad
+        for p in self.module.parameters():
+            if hasattr(p, 'colo_attr'):
+                p.colo_attr.sharded_data_tensor.trans_state(TensorState.HOLD)
 
-    def zero_grad(self, set_to_none: bool = False) -> None:
-        self.module.zero_grad(set_to_none=True)
+        self._stateful_tensor_mgr.start_iter()
 
-    def set_chunk_grad_device(self, chunk: Chunk, device: torch.device) -> None:
-        for tensor in chunk.get_tensors():
-            self.grads_device[tensor] = device
-
-    def state_dict(self,
-                   destination=None,
-                   prefix='',
-                   keep_vars=False,
-                   only_rank_0: bool = True,
-                   dtype: torch.dtype = torch.float16):
-        """Returns a dictionary containing a whole state of the module.
-
-        Both parameters and persistent buffers (e.g. running averages) are included.
-        Keys are corresponding parameter and buffer names.
-        Parameters and buffers set to ``None`` are not included.
-
-        Warning: The non strict state dict would ignore the parameters if the tensors of the parameters
-            are shared with other parameters which have been included in the dictionary.
-            When you need to load the state dict, you should set the argument `strict` to False.
-
-        Returns:
-            dict:
-                a dictionary containing a whole state of the module
-        """
-        if destination is None:
-            destination = OrderedDict()
-            destination._metadata = OrderedDict()
-        destination._metadata[prefix[:-1]] = local_metadata = dict(version=self._version)
-        self._save_to_state_dict(destination, prefix, keep_vars, only_rank_0, dtype)
-
-        for hook in self._state_dict_hooks.values():
-            hook_result = hook(self, destination, prefix, local_metadata)
-            if hook_result is not None:
-                destination = hook_result
-        return destination
+    def _post_forward_operations(self):
+        for p in self.module.parameters():
+            if hasattr(p, 'colo_attr'):
+                p.colo_attr.sharded_data_tensor.trans_state(TensorState.HOLD)
 
-    def _get_chunk_to_save_data(self, chunk: Chunk, only_rank_0: bool, dtype: torch.dtype = torch.float16) -> Dict:
-        """
-        get gathered chunk content.
+    def forward(self, *args: Any, **kwargs: Any) -> torch.Tensor:
+        self._pre_forward_operations(*args)
+        args, kwargs = cast_float_arguments(cast_tensor_to_fp16, *args, **kwargs)
+        outputs = self.module(*args, **kwargs)
+        self._post_forward_operations()
+        return outputs
 
-        Args:
-            chunk (Chunk): a chunk
-            only_rank_0 (bool): whether to only save data on rank 0
+    def backward(self, loss):
+        loss.backward()
+        self._post_backward_operations()
+        for ophook in self._ophook_list:
+            ophook.post_iter()
 
-        Returns:
-            Dict: a dict whose key is param name and value is param with correct payload
-        """
-        # save parameters
-        chunk_to_save_data = dict()
-        temp_chunk = get_temp_total_chunk_on_cuda(chunk)
-        if torch.is_floating_point(temp_chunk):
-            temp_chunk = temp_chunk.to(dtype)
-        for tensor, tensor_info in chunk.tensors_info.items():
-            record_tensor = torch.empty([0])
-            record_flag = (not only_rank_0) | (dist.get_rank(chunk.torch_pg) == 0)
-            if record_flag:
-                record_tensor = temp_chunk[tensor_info.offset:tensor_info.end].view(tensor.shape).cpu()
+    def backward_by_grad(self, tensor, grad):
+        torch.autograd.backward(tensors=tensor, grad_tensors=grad)
+        self._post_backward_operations()
+        for ophook in self._ophook_list:
+            ophook.post_iter()
+
+    def _update_memstats(self):
+        if self._memstats_collector:
+            self._finish_collect_memstats()
+            # cuda margin space = cuda mem capacity - max fwd/bwd cuda mem used.
+            # the way to calculate margin space is based on the assumption that
+            # model data is fixed in cuda during training.
+            # cuda margin space can be used to store OS.
+            self._cuda_margin_space = colo_device_memory_capacity(
+                get_current_device()) - self._memstats_collector._memstats.max_overall_cuda
+
+    @torch.no_grad()
+    def _post_backward_operations(self) -> None:
+        """
+        The method includes operations required to be processed after backward
+        1. update memory tracer.
+        2. flush the gradient in buckets. Reducing partial gradients in each process.
+        3. shard tensors not dealed in the zero hook
+        4. move sharded param grad payload to param.grad
+        """
+        # 1. update memory tracer.
+        self._update_memstats()
+
+        # 2. flush the gradient in buckets. Reducing partial gradients in each process.
+        if self._require_backward_grad_sync:
+            # Flush any unreduced buckets in the post_backward stream.
+            with torch.cuda.stream(self.comm_stream):
+                self.reducer.flush()
+            torch.cuda.current_stream().wait_stream(self.comm_stream)
+        self.reducer.free()
+
+        # 3. shard tensors not dealed in the zero hook
+        tensor_list = []
+        for p in self.sharded_params:
+            if not p.colo_attr.param_is_sharded:
+                tensor_list.append(p.colo_attr.sharded_data_tensor)
+                p.colo_attr.sharded_data_tensor.trans_state(TensorState.HOLD_AFTER_BWD)
+                p.colo_attr.set_data_none()
+        self.shard_strategy.shard(tensor_list, self.process_group)
 
-            assert tensor not in chunk_to_save_data
-            chunk_to_save_data[tensor] = record_tensor
+        # 4. set all parameters' grad to None
+        for p in self.module.parameters():
+            if not p.requires_grad:
+                continue
+            # Leave the gradient accumulation state (_require_backward_grad_sync) as-is if not synchronizing this pass.
+            # NOTE() (no-sync)/sync pass: (not conduct)/conduct gradient allreducing between process group.
+            # If _require_backward_grad_sync is True,
+            # p.grad remains the accumulated unsharded gradient from prior no-sync passes.
+            # We also allows to interleave no-sync pass with sync passes, if desired.
+            if not self._require_backward_grad_sync:
+                continue
 
-        del temp_chunk
-        return chunk_to_save_data
+            p.grad = None
 
-    def _get_param_to_save_data(self, param_list: List[torch.nn.Parameter], only_rank_0: bool,
-                                dtype: torch.dtype) -> Dict:
+    @torch.no_grad()
+    def _grad_post_backward_hook(self, param: Parameter, grad: torch.Tensor) -> Optional[torch.Tensor]:
         """
-        get param content from chunks.
+        At the start of :func:`_grad_post_backward_hook`, ``param.grad`` contains the
+        full gradient for the local batch. The reduce-scatter op will save
+        a single shard of the summed gradient across all
+        GPUs to param.colo_attr.grad. This shard will align with the current GPU rank. For example::
+
+            before reduce_scatter:
+                param.grad (GPU #0): [1, 2, 3, 4]
+                param.grad (GPU #1): [5, 6, 7, 8]
+
+            after reduce_scatter:
+                param.grad (GPU #0): [6, 8]    # 1+5, 2+6
+                param.grad (GPU #1): [10, 12]  # 3+7, 4+8
+
+        The local GPU's ``optim.step`` is responsible for updating a single
+        shard of params, also corresponding to the current GPU's rank. This
+        alignment is created by `param.colo_attr.grad`, which ensures that
+        the local optimizer only sees the relevant parameter shard.
+        """
+        if grad is None:
+            return
+        assert not grad.requires_grad, 'ShardedModel only works with gradients that don\'t require gradients'
+        if not self._require_backward_grad_sync:
+            return
+        # used to cheat Pytorch, since we can't return None
+        empty_grad = torch.empty_like(grad)
+        free_storage(empty_grad)
+        # As torch didn't allow modifying grad in hook, we make a copy
+        grad = grad.clone()
+        if param.colo_attr.is_replicated:
+            self._reduce_scatter_handler(param, grad)
+        else:
+            self._save_grad(param, grad)
+        return empty_grad
 
-        Args:
-            param_list (_type_): a list of torch.nn.Parameters
-            only_rank_0 (_type_): _description_
+    def _reduce_scatter_handler(self, param: Parameter, grad: torch.Tensor) -> None:
+        self.comm_stream.wait_stream(torch.cuda.current_stream())
+        with torch.cuda.stream(self.comm_stream):
+            if self.fp32_reduce_scatter:
+                grad.data = grad.data.to(param.dtype)
+            if self.gradient_predivide_factor > 1.0:
+                # Average grad by world_size for consistency with PyTorch DDP.
+                grad.data.div_(self.gradient_predivide_factor)
+            if self.world_size > 1:
+                grad_chunks = chunk_and_pad(grad, self.reduce_scatter_process_group.size())
+                self.reducer.reduce_scatter_async(grad_chunks,
+                                                  group=self.reduce_scatter_process_group,
+                                                  callback_fn=functools.partial(self._reduce_scatter_callback, param))
+            else:
+                self._reduce_scatter_callback(param, grad)
+        torch.cuda.current_stream().wait_stream(self.comm_stream)
 
-        Returns:
-            Dict: a dict whose key is param name and value is param with correct payload
-        """
-        # save parameters
-        param_to_save_data = dict()
-        chunk_list = self.chunk_manager.get_chunks(param_list)
-        for chunk in chunk_list:
-            param_to_save_data.update(self._get_chunk_to_save_data(chunk, only_rank_0, dtype))
-        return param_to_save_data
-
-    def _save_to_state_dict(self, destination, prefix, keep_vars, only_rank_0=True, dtype=torch.float16):
-        r"""Saves module state to `destination` dictionary, containing a state
-        of the module, but not its descendants. This is called on every
-        submodule in :meth:`~torch.nn.Module.state_dict`.
+    def _reduce_scatter_callback(self, param: Parameter, reduced_grad: torch.Tensor) -> None:
+        assert isinstance(reduced_grad,
+                          torch.Tensor), f"_reduce_scatter_callback accept reduced_grad as {type(reduced_grad)}"
+        reduced_grad.data = reduced_grad.data.contiguous().view(-1)
+        if self.gradient_postdivide_factor > 1:
+            # Average grad by world_size for consistency with PyTorch DDP.
+            reduced_grad.data.div_(self.gradient_postdivide_factor)
+        self._save_grad(param, reduced_grad)
+
+    # FIXME(ver217): refactor the below line when impl eviction policy
+    def _save_grad(self, param: Parameter, grad: torch.Tensor):
+
+        # record whether we have overflow
+        self.overflow_counter += torch.isinf(grad).any().item()
+        self.overflow_counter += torch.isnan(grad).any().item()
+
+        # move gradient to cpu
+        if param.colo_attr.offload_grad:
+            colo_model_data_move_to_cpu(grad)
+
+        if self.reuse_fp16_shard:
+            # make parameters point to gradient
+
+            assert param.colo_attr.saved_grad.is_null(
+            ), 'Gradien accumulation is not supported when reuse_fp16_shard=True'
+
+            param.colo_attr.grad_payload_reset(grad.data)
+            # release the memory of param
+            # we set a false None for parameter's payload
+            # so we can get paramter's device and dtype later in optimizer
+            param.colo_attr.data_payload_reset(torch.empty(0, device=grad.device, dtype=grad.dtype))
 
-        In rare cases, subclasses can achieve class-specific behavior by
-        overriding this method with custom logic.
+            if param.colo_attr.is_replicated:
+                param.colo_attr.sharded_data_tensor.is_sharded = True
+        else:
 
-        Args:
-            destination (dict): a dict where state will be stored
-            prefix (str): the prefix for parameters and buffers used in this
-                module
-        """
-        assert keep_vars is False, "`state_dict` with parameter, `keep_vars=True`, is not supported now."
+            fp32_grad = cast_tensor_to_fp32(grad)
 
-        # get copies of fp32 parameters in CPU
-        # as memory of fp16_params may be reused by grad, it's not reliable, we should use fp32_params and convert to fp16
-        param_to_save_data = self._get_param_to_save_data(self.fp32_params, only_rank_0, dtype)
-        # get the mapping between copies and fp16 parameters
-        p_mapping = dict()
-        for p, fp32_p in zip(self.fp16_params, self.fp32_params):
-            name = self.param2name[p]
-            assert fp32_p in param_to_save_data, "Parameter '{}' is neglected in the chunk list".format(name)
-            record_parameter = param_to_save_data[fp32_p]
-            p_mapping[p] = record_parameter
-        for name, param in self.name2param.items():
-            if param is not None:
-                if is_ddp_ignored(param):
-                    # deal with ddp ignored parameters
-                    destination[prefix + name] = param if keep_vars else param.detach()
-                else:
-                    destination[prefix + name] = p_mapping[param]
-        del p_mapping
-        del param_to_save_data
-
-        # save all buffers
-        for name, buf in self.named_buffers():
-            if buf is not None and name not in self._non_persistent_buffers_set:
-                destination[prefix + name] = buf if keep_vars else buf.detach()
-        # save extra states
-        extra_state_key = prefix + _EXTRA_STATE_KEY_SUFFIX
-        if getattr(self.__class__, "get_extra_state",
-                   torch.nn.Module.get_extra_state) is not torch.nn.Module.get_extra_state:
-            destination[extra_state_key] = self.get_extra_state()
-
-    def load_state_dict(self, state_dict: 'OrderedDict[str, torch.Tensor]', strict: bool = True):
-        r"""Copies parameters and buffers from :attr:`state_dict` into
-        this module and its descendants. If :attr:`strict` is ``True``, then
-        the keys of :attr:`state_dict` must exactly match the keys returned
-        by this module's :meth:`~torch.nn.Module.state_dict` function.
+            if param.colo_attr.saved_grad.is_null():
+                param.colo_attr.grad_payload_reset(fp32_grad)
+            else:
+                param.colo_attr.grad_payload.add_(fp32_grad.view_as(param.colo_attr.grad_payload))
 
-        Args:
-            state_dict (dict): a dict containing parameters and
-                persistent buffers.
-            strict (bool, optional): whether to strictly enforce that the keys
-                in :attr:`state_dict` match the keys returned by this module's
-                :meth:`~torch.nn.Module.state_dict` function. Default: ``True``
-
-        Returns:
-            ``NamedTuple`` with ``missing_keys`` and ``unexpected_keys`` fields:
-                * **missing_keys** is a list of str containing the missing keys
-                * **unexpected_keys** is a list of str containing the unexpected keys
-
-        Note:
-            If a parameter or buffer is registered as ``None`` and its corresponding key
-            exists in :attr:`state_dict`, :meth:`load_state_dict` will raise a
-            ``RuntimeError``.
-        """
-        missing_keys: List[str] = []
-        unexpected_keys: List[str] = []
-        error_msgs: List[str] = []
-
-        # copy state_dict so _load_from_state_dict can modify it
-        metadata = getattr(state_dict, '_metadata', None)
-        state_dict = state_dict.copy()
-        if metadata is not None:
-            # mypy isn't aware that "_metadata" exists in state_dict
-            state_dict._metadata = metadata    # type: ignore[attr-defined]
-
-        prefix = ''
-        local_metadata = {} if metadata is None else metadata.get(prefix[:-1], {})
-        self._load_from_state_dict(state_dict, prefix, local_metadata, True, missing_keys, unexpected_keys, error_msgs)
+        # keep saved_grad in HOLD state
+        param.colo_attr.saved_grad.trans_state(TensorState.HOLD)
 
-        if strict:
-            if len(unexpected_keys) > 0:
-                error_msgs.insert(
-                    0, 'Unexpected key(s) in state_dict: {}. '.format(', '.join(
-                        '"{}"'.format(k) for k in unexpected_keys)))
-            if len(missing_keys) > 0:
-                error_msgs.insert(
-                    0, 'Missing key(s) in state_dict: {}. '.format(', '.join('"{}"'.format(k) for k in missing_keys)))
-
-        if len(error_msgs) > 0:
-            raise RuntimeError('Error(s) in loading state_dict for {}:\n\t{}'.format(
-                self.__class__.__name__, "\n\t".join(error_msgs)))
-        return _IncompatibleKeys(missing_keys, unexpected_keys)
+    def parameters(self, recurse: bool = True) -> Iterator[Parameter]:
+        return self.module.parameters(recurse=recurse)
 
-    def _load_from_state_dict(self, state_dict, prefix, local_metadata, strict, missing_keys, unexpected_keys,
-                              error_msgs):
+    def named_parameters(self, prefix: str = '', recurse: bool = True) -> Iterator[Tuple[str, Parameter]]:
+        return self.module.named_parameters(prefix, recurse)
+
+    def state_dict(self, destination=None, prefix='', keep_vars=False) -> 'OrderedDict[str, torch.Tensor]':
+        return self._colo_state_dict(destination,
+                                     prefix,
+                                     keep_vars,
+                                     shard_strategy=self.shard_strategy,
+                                     state_dict_func=nn.Module.state_dict,
+                                     module_to_load=self.module,
+                                     sharded_params=self.sharded_params,
+                                     process_group=self.process_group)
+
+    def load_state_dict(self, state_dict: 'OrderedDict[str, torch.Tensor]', strict: bool = True) -> None:
+        for name, p in self.named_parameters():
+            if name in state_dict:
+                p.colo_attr.data_payload_reset(state_dict[name].to(dtype=p.colo_attr.data_payload.dtype,
+                                                                   device=p.colo_attr.data_payload.device))
+                # Force re-shard
+                p.colo_attr.sharded_data_tensor.is_sharded = False
+                self.shard_strategy.shard([p.colo_attr.sharded_data_tensor])
+            elif strict:
+                raise RuntimeError(f'Missing key in state_dict: {name}')
+
+    def _colo_state_dict(self,
+                         destination=None,
+                         prefix='',
+                         keep_vars=False,
+                         shard_strategy: Optional[BaseShardStrategy] = None,
+                         state_dict_func=None,
+                         module_to_load=None,
+                         sharded_params=[],
+                         process_group=None) -> 'OrderedDict[str, torch.Tensor]':
+        if len(sharded_params) == 0:
+            for param in self.parameters():
+                if param.colo_attr.param_is_sharded:
+                    sharded_params.append(param)
+        if shard_strategy is not None:
+            shard_strategy.gather([p.colo_attr.sharded_data_tensor for p in sharded_params], process_group)
+        for p in sharded_params:
+            p.data = p.colo_attr.data_payload
+        module_to_load = module_to_load or self
+        gathered_state_dict = state_dict_func(module_to_load, destination, prefix, keep_vars)
+        gathered_state_dict = {k: v.cpu() if isinstance(v, torch.Tensor) else v for k, v in gathered_state_dict.items()}
+        if shard_strategy is not None:
+            shard_strategy.shard([p.colo_attr.sharded_data_tensor for p in sharded_params], process_group)
+        for p in sharded_params:
+            p.colo_attr.set_data_none()
+        return gathered_state_dict
+
+    def _colo_load_from_state_dict(self,
+                                   state_dict,
+                                   prefix,
+                                   local_metadata,
+                                   strict,
+                                   missing_keys,
+                                   unexpected_keys,
+                                   error_msgs,
+                                   shard_strategy=None):
         r"""Copies parameters and buffers from :attr:`state_dict` into only
         this module, but not its descendants. This is called on every submodule
         in :meth:`~torch.nn.Module.load_state_dict`. Metadata saved for this
         module in input :attr:`state_dict` is provided as :attr:`local_metadata`.
         For state dicts without metadata, :attr:`local_metadata` is empty.
         Subclasses can achieve class-specific backward compatible loading using
         the version number at `local_metadata.get("version", None)`.
@@ -426,322 +490,83 @@
             missing_keys (list of str): if ``strict=True``, add missing keys to
                 this list
             unexpected_keys (list of str): if ``strict=True``, add unexpected
                 keys to this list
             error_msgs (list of str): error messages should be added to this
                 list, and will be reported together in
                 :meth:`~torch.nn.Module.load_state_dict`
+            shard_strategy (Optional[BaseShardStrategy], optional): A shard strategy to manage shard behavior. Defaults to None.
         """
         for hook in self._load_state_dict_pre_hooks.values():
             hook(state_dict, prefix, local_metadata, strict, missing_keys, unexpected_keys, error_msgs)
 
-        persistent_buffers = {k: v for k, v in self.named_buffers() if k not in self._non_persistent_buffers_set}
-        local_name_params = itertools.chain(self.named_parameters(), persistent_buffers.items())
+        persistent_buffers = {k: v for k, v in self._buffers.items() if k not in self._non_persistent_buffers_set}
+        local_name_params = itertools.chain(self._parameters.items(), persistent_buffers.items())
         local_state = {k: v for k, v in local_name_params if v is not None}
 
-        def load(param_name, dest_tensor, copy_func):
-            state_key = prefix + param_name
-            if state_key in state_dict:
-                input_param = state_dict[state_key]
-                # Backward compatibility: loading 1-dim tensor from 0.3.* to version 0.4+
-                if len(dest_tensor.shape) == 0 and len(input_param.shape) == 1:
-                    input_param = input_param[0]
-                if input_param.shape != dest_tensor.shape:
-                    # local shape should match the one in checkpoint
-                    error_msgs.append('size mismatch for {}: copying a param with shape {} from checkpoint, '
-                                      'the shape in current model is {}.'.format(state_key, input_param.shape,
-                                                                                 dest_tensor.shape))
-                    return
-                try:
-                    with torch.no_grad():
-                        copy_func(input_param)
-                except Exception as ex:
-                    error_msgs.append('While copying the parameter named "{}", '
-                                      'whose dimensions in the model are {} and '
-                                      'whose dimensions in the checkpoint are {}, '
-                                      'an exception occurred : {}.'.format(state_key, dest_tensor.size(),
-                                                                           input_param.size(), ex.args))
+        for name, param in local_state.items():
+            key = prefix + name
+            if key in state_dict:
+                input_param = state_dict[key]
+                if hasattr(param, 'colo_attr'):
+                    param.colo_attr.data_payload_reset(
+                        input_param.to(dtype=param.colo_attr.data_payload.dtype,
+                                       device=param.colo_attr.data_payload.device))
+                    if shard_strategy is not None:
+                        # Force re-shard
+                        param.colo_attr.sharded_data_tensor.is_sharded = False
+                        shard_strategy.shard([param.colo_attr.sharded_data_tensor])
+                else:
+                    # This is used to avoid copying uninitialized parameters into
+                    # non-lazy modules, since they dont have the hook to do the checks
+                    # in such case, it will error when accessing the .shape attribute.
+                    is_param_lazy = torch.nn.parameter.is_lazy(param)
+                    # Backward compatibility: loading 1-dim tensor from 0.3.* to version 0.4+
+                    if not is_param_lazy and len(param.shape) == 0 and len(input_param.shape) == 1:
+                        input_param = input_param[0]
+
+                    if not is_param_lazy and input_param.shape != param.shape:
+                        # local shape should match the one in checkpoint
+                        error_msgs.append('size mismatch for {}: copying a param with shape {} from checkpoint, '
+                                          'the shape in current model is {}.'.format(
+                                              key, input_param.shape, param.shape))
+                        continue
+                    try:
+                        with torch.no_grad():
+                            param.copy_(input_param)
+                    except Exception as ex:
+                        error_msgs.append('While copying the parameter named "{}", '
+                                          'whose dimensions in the model are {} and '
+                                          'whose dimensions in the checkpoint are {}, '
+                                          'an exception occurred : {}.'.format(key, param.size(), input_param.size(),
+                                                                               ex.args))
             elif strict:
-                missing_keys.append(state_key)
-
-        def load_fp32_parameter(chunk_slice, data):
-            chunk_slice.copy_(data.flatten())
-
-        for name, param in self.named_parameters():
-            if is_ddp_ignored(param):
-                # deal with ddp ignored parameters
-                load(name, param, param.copy_)
-
-        fp32_to_name = dict()
-        for p, fp32_p in zip(self.fp16_params, self.fp32_params):
-            if p is not None:
-                name = self.param2name[p]
-                fp32_to_name[fp32_p] = name
-
-        chunk_list = self.chunk_manager.get_chunks(self.fp32_params)
-        for chunk in chunk_list:
-            temp_chunk = get_temp_total_chunk_on_cuda(chunk)
-
-            for tensor, tensor_info in chunk.tensors_info.items():
-                parameter_name = fp32_to_name[tensor]
-                parameter_slice = temp_chunk[tensor_info.offset:tensor_info.end]
-                load(parameter_name, tensor, partial(load_fp32_parameter, parameter_slice))
-
-            if chunk.is_gathered:
-                chunk.cuda_global_chunk.copy_(temp_chunk)
-            elif chunk.cuda_shard is not None:
-                chunk.cuda_shard.copy_(temp_chunk[chunk.shard_begin:chunk.shard_end])
-            else:
-                chunk.cpu_shard.copy_(temp_chunk[chunk.shard_begin:chunk.shard_end])
-
-            del temp_chunk
-
-        for chunk_32 in chunk_list:
-            chunk_16 = chunk_32.paired_chunk
-            assert chunk_16 is not None
-            chunk_16.optim_update()
-
-        for name, buf in persistent_buffers.items():
-            if buf is not None:
-                load(name, buf, buf.copy_)
+                missing_keys.append(key)
 
         extra_state_key = prefix + _EXTRA_STATE_KEY_SUFFIX
-        if getattr(self.__class__, "set_extra_state",
-                   torch.nn.Module.set_extra_state) is not torch.nn.Module.set_extra_state:
+        if getattr(self.__class__, "set_extra_state", nn.Module.set_extra_state) is not nn.Module.set_extra_state:
             if extra_state_key in state_dict:
                 self.set_extra_state(state_dict[extra_state_key])
             elif strict:
                 missing_keys.append(extra_state_key)
         elif strict and (extra_state_key in state_dict):
             unexpected_keys.append(extra_state_key)
 
         if strict:
             for key in state_dict.keys():
                 if key.startswith(prefix) and key != extra_state_key:
                     input_name = key[len(prefix):]
-                    if input_name not in local_state:
+                    input_name = input_name.split('.', 1)[0]    # get the name of param/buffer/child
+                    if input_name not in self._modules and input_name not in local_state:
                         unexpected_keys.append(key)
 
-    def _init_chunks(self, param_order, strict_ddp_mode: bool, cpu_offload: bool, pin_memory: bool):
-        ddp_pg = ColoProcessGroup()
-        for p in param_order.generate():
-            self._preprocess_param(p)
-            assert type(p) is ColoParameter
-
-            # gather sharded parameters in the strict ddp mode
-            if strict_ddp_mode:
-                if not p.is_replicate():
-                    p.set_dist_spec(ReplicaSpec())
-                p.set_process_group(pg=ddp_pg)
-
-            # ignore the parameters with no gradient
-            if not p.requires_grad:
-                self.set_params_to_ignore([p])
-
-            # move ignored parameters to CUDA
-            if is_ddp_ignored(p):
-                p.data = p.data.to(device=get_current_device(), dtype=torch.float16)
-                continue
-
-            # create a fp32 parameter
-            fp32_data = p.data.float()
-            fp32_p = ColoTensor(fp32_data, spec=ColoTensorSpec(p.process_group))
-            # create a fp16 parameter
-            p.data = p.data.half()
-
-            # register the fp16 parameter and fp32 parameter in the chunk manager
-            dp_world_size = p.process_group.dp_world_size()
-            self.chunk_manager.register_tensor(tensor=p,
-                                               group_type='fp16_param',
-                                               config_key=dp_world_size,
-                                               cpu_offload=cpu_offload,
-                                               pin_memory=pin_memory)
-            self.chunk_manager.register_tensor(tensor=fp32_p,
-                                               group_type='fp32_param',
-                                               config_key=dp_world_size,
-                                               cpu_offload=cpu_offload,
-                                               pin_memory=pin_memory)
-
-            self.fp16_params.append(p)
-            self.fp32_params.append(fp32_p)
-            self.grads_device[p] = self.gemini_manager.default_device
-
-        self.chunk_manager.close_all_groups()
-
-        for p, fp32_p in zip(self.fp16_params, self.fp32_params):
-            chunk_16 = self.chunk_manager.get_chunk(p)
-            chunk_32 = self.chunk_manager.get_chunk(fp32_p)
-            chunk_32.init_pair(chunk_16)
-
-            # keep gathered chunks are in CUDA
-            if chunk_16.keep_gathered:
-                self.grads_device[p] = get_current_device()
-
-    def _cast_buffers(self):
-        for buffer in self.module.buffers():
-            if isinstance(buffer, LazyTensor):
-                buffer.materialize()
-            buffer.data = buffer.cuda()
-            if torch.is_floating_point(buffer):
-                buffer.data = buffer.half()
-
-    def _preprocess_param(self, p: Union[nn.Parameter, ColoParameter, 'LazyTensor']) -> None:
-        """Convert parameter to ColoParameter in-place.
-        Args:
-            p (Union[nn.Parameter, ColoParameter, LazyTensor]): parameter to be converted
-        """
-        if type(p) is ColoParameter:
-            # model is initialized with ColoInitContext
-            return
-        requires_grad = p.requires_grad
-        if isinstance(p, LazyTensor):
-            # model is initialized with LazyInitContext
-            p.materialize()
-        p.__class__ = ColoParameter
-        p.__init__(p, requires_grad=requires_grad)
-
-    def state_dict_shard(self,
-                         prefix: str = '',
-                         keep_vars: bool = False,
-                         max_shard_size: int = 1024,
-                         only_rank_0: bool = True,
-                         dtype: torch.dtype = torch.float16) -> Iterator[OrderedDict]:
-        """Returns dictionaries containing a whole state of the module one by one. The max size of dictionary shard is specified by ``max_shard_size``.
-
-        Both parameters and persistent buffers (e.g. running averages) are included.
-        Keys are corresponding parameter and buffer names.
-        Parameters and buffers set to ``None`` are not included.
-
-        Args:
-            prefix (str, optional): the prefix for parameters and buffers used in this
-                module. Defaults to ''.
-            keep_vars (bool, optional): whether to keep variables. Defaults to False.
-            max_shard_size (int, optional): max size of state dict shard (in MB). Defaults to 1024.
-            only_rank_0 (bool, optional): only get data on rank0. Defaults to True.
-
-
-        Yields:
-            Iterator[OrderedDict]: A generator of state dict shard
-        """
-        sharder = _StateDictSharder(max_shard_size)
-
-        # get the mapping between copies and fp16 parameters
-        fp16_to_fp32 = dict()
-        for p, fp32_p in zip(self.fp16_params, self.fp32_params):
-            fp16_to_fp32[p] = fp32_p
-
-        # key is fp32 param, and value is gathered param on CPU
-        gathered_param_buffer = dict()
-        for name, param in self.name2param.items():
-            if param is not None:
-                if is_ddp_ignored(param):
-                    # deal with ddp ignored parameters
-                    gathered_param = param if keep_vars else param.detach()
-                else:
-                    # as memory of fp16 param may be reused, we should use fp32 param and then convert to fp16
-                    fp32_param = fp16_to_fp32[param]
-                    if fp32_param not in gathered_param_buffer:
-                        chunk = self.chunk_manager.get_chunk(fp32_param)
-                        gathered_param_buffer.update(self._get_chunk_to_save_data(chunk, only_rank_0, dtype))
-                    gathered_param = gathered_param_buffer.pop(fp32_param)
-
-                block = sharder.append(prefix + name, gathered_param)
-                if block is not None:
-                    yield block
-
-        del fp16_to_fp32
-        del gathered_param_buffer
-
-        # save all buffers
-        for name, buf in self.named_buffers():
-            if buf is not None and name not in self._non_persistent_buffers_set:
-                buffer = buf if keep_vars else buf.detach()
-                block = sharder.append(prefix + name, buffer)
-                if block is not None:
-                    yield block
-        # save extra states
-        extra_state_key = prefix + _EXTRA_STATE_KEY_SUFFIX
-        if getattr(self.__class__, "get_extra_state",
-                   torch.nn.Module.get_extra_state) is not torch.nn.Module.get_extra_state:
-            extra_state = self.get_extra_state()
-            block = sharder.append(extra_state_key, extra_state)
-            if block is not None:
-                yield block
-
-        yield sharder.current_block
-
-
-class _StateDictSharder:
-
-    def __init__(self, max_shard_size: int) -> None:
-        self.max_shard_size = max_shard_size
-        self.current_block = OrderedDict()
-        self.current_block_size = 0
-
-    def append(self, name: str, tensor: torch.Tensor) -> Optional[OrderedDict]:
-        tensor_size = calculate_tensor_size(tensor)
-        ret_block = None
-        if self.current_block_size + tensor_size > self.max_shard_size:
-            ret_block = self.current_block
-            self.current_block = OrderedDict()
-            self.current_block_size = 0
-        self.current_block[name] = tensor
-        self.current_block_size += tensor_size
-        return ret_block
-
-
-class GeminiDDP(ZeroDDP):
-
-    def __init__(self,
-                 module: torch.nn.Module,
-                 device: torch.device,
-                 placement_policy: str = "cpu",
-                 pin_memory: bool = False,
-                 force_outputs_fp32: bool = False,
-                 strict_ddp_mode: bool = False,
-                 scatter_after_inference: bool = True,
-                 search_range_mb: int = 32,
-                 hidden_dim: Optional[int] = None,
-                 min_chunk_size_mb: float = 32,
-                 memstats: Optional[MemStats] = None,
-                 verbose: bool = False) -> None:
-        """
-        A torch.Module wrapper using ZeRO-DP and Gemini.
-        ZeRO is for parallel. Gemini is for memory management.
-        WARNING: The class will modify the module inline!
-
-        Example:
-            model is initialized under the context of ColoInitContext
-            >>> model = GeminiDDP(model, torch.cuda.current_device(), "cuda")
-            >>> logits = model(x)
-            >>> loss = criterion(logits, labels)
-            >>> model.backward(loss)
-
-        Args:
-            module (torch.nn.Module): the model to be wrapped.
-            device (torch.device): device to place the model.
-            placement_policy (str, optional): "cpu", "cuda", "auto". Defaults to "cpu".
-            pin_memory (bool, optional): use pin memory on CPU. Defaults to False.
-            force_outputs_fp32 (bool, optional): force outputs are fp32. Defaults to False.
-            search_range_mb (int, optional): chunk size searching range in MegaByte. Defaults to 32.
-            hidden_dim (int, optional): the hidden dimension of DNN.
-                Users can provide this argument to speed up searching.
-                If users do not know this argument before training, it is ok. We will use a default value 1024.
-            min_chunk_size_mb (float, optional): the minimum chunk size in MegaByte.
-                If the aggregate size of parameters is still smaller than the minimum chunk size,
-                all parameters will be compacted into one small chunk.
-            memstats (MemStats, optional) the memory statistics collector by a runtime memory tracer.
-        """
-        # some ugly hotfix for the compatibility with Lightning
-        if search_range_mb is None:
-            search_range_mb = 32
-
-        chunk_manager = init_chunk_manager(model=module,
-                                           init_device=device,
-                                           hidden_dim=hidden_dim,
-                                           search_range_mb=search_range_mb,
-                                           min_chunk_size_mb=min_chunk_size_mb,
-                                           strict_ddp_flag=strict_ddp_mode,
-                                           verbose=verbose)
-        gemini_manager = GeminiManager(placement_policy, chunk_manager, memstats)
-        super().__init__(module, gemini_manager, pin_memory, force_outputs_fp32, strict_ddp_mode,
-                         scatter_after_inference)
+    def __getitem__(self, idx: int):
+        assert isinstance(self.module, nn.ModuleList)
+        return self.module[idx]
+
+    def __len__(self):
+        assert isinstance(self.module, nn.ModuleList)
+        return len(self.module)
+
+    def __iter__(self):
+        assert isinstance(self.module, nn.ModuleList)
+        return iter(self.module)
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/gemini_hook.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/gemini_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/gemini_mgr.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/gemini_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/gemini_optimizer.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/gemini_optimizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,54 +42,48 @@
         module (ZeroDDP): A ``ZeroDDP`` instance.
         gpu_margin_mem_ratio (float, optional): The ratio of GPU remaining memory (after the first forward-backward)
             which will be used when using hybrid CPU optimizer.
             This argument is meaningless when `placement_policy` of `GeminiManager` is not "auto".
             Defaults to 0.0.
         initial_scale (float, optional): Initial scale used by DynamicGradScaler. Defaults to 2**32.
         min_scale (float, optional): Min scale used by DynamicGradScaler. Defaults to 1.
-        growth_factor (float, optional): Growth_factor used by DynamicGradScaler. Defaults to 2.
-        backoff_factor (float, optional): Backoff_factor used by DynamicGradScaler. Defaults to 0.5.
-        growth_interval (float, optional): Growth_interval used by DynamicGradScaler. Defaults to 1000.
-        hysteresis (float, optional): Hysteresis used by DynamicGradScaler. Defaults to 2.
-        max_scale (int, optional): Max_scale used by DynamicGradScaler. Defaults to 2**32.
-        clipping_norm (float, optional): The norm value used to clip gradient. Defaults to 0.0.
-        norm_type (float, optional): The type of norm used for gradient clipping. Currently, only L2-norm (norm_type=2.0)
-            is supported in ZeroOptimizer. Defaults to 2.0.
-        verbose (bool, optional): Whether to print verbose information, including grad overflow info. Defaults to False.
-    """
+        growth_factor (float, optional): growth_factor used by DynamicGradScaler. Defaults to 2.
+        backoff_factor (float, optional): backoff_factor used by DynamicGradScaler. Defaults to 0.5.
+        growth_interval (float, optional): growth_interval used by DynamicGradScaler. Defaults to 1000.
+        hysteresis (float, optional): hysteresis used by DynamicGradScaler. Defaults to 2.
+        max_scale (int, optional): max_scale used by DynamicGradScaler. Defaults to 2**32.
+        """
 
     def __init__(self,
                  optim: Optimizer,
                  module: ZeroDDP,
                  gpu_margin_mem_ratio: float = 0.0,
                  initial_scale: float = 2**32,
                  min_scale: float = 1,
                  growth_factor: float = 2,
                  backoff_factor: float = 0.5,
                  growth_interval: int = 1000,
                  hysteresis: int = 2,
                  max_scale: float = 2**32,
                  clipping_norm: float = 0.0,
                  norm_type: float = 2.0,
-                 verbose: bool = False,
                  **defaults: Any):
         super().__init__(optim)
         assert isinstance(module, ZeroDDP)
         assert type(optim) in _AVAIL_OPTIM_LIST, "You should use an optimizer in the available list:\n" \
             f"{_AVAIL_OPTIM_LIST}"
         self.module = module
         self.gemini_manager = module.gemini_manager
         self.chunk_manager: ChunkManager = self.gemini_manager.chunk_manager
         self.optim_state = OptimState.UNSCALED
         self.param_to_range: Dict[Parameter, Tuple[int, int]] = dict()
         self.param_to_chunk32: Dict[Parameter, Chunk] = dict()
         self.chunk16_set: Set[Chunk] = set()
         self.clipping_flag = clipping_norm > 0.0
         self.max_norm = clipping_norm
-        self.verbose = verbose
 
         if self.clipping_flag:
             assert norm_type == 2.0, "ZeroOptimizer only supports L2 norm now"
 
         ddp_param_list = []
         for name, param in module.named_parameters():
             if is_ddp_ignored(param):
@@ -220,16 +214,15 @@
         self._maybe_move_fp32_params()
         self._set_grad_ptr()
 
         found_inf = self._check_overflow()
         if found_inf:
             self.optim_state = OptimState.UNSCALED    # no need to unscale grad
             self.grad_scaler.update(found_inf)    # update gradient scaler
-            if self.verbose:
-                self._logger.info(f'Found overflow. Skip step')
+            self._logger.info(f'Found overflow. Skip step')
             self._clear_global_norm()    # clear recorded norm
             self.zero_grad()    # reset all gradients
             self._update_fp16_params()
             return
 
         # get combined scale. combined scale = loss scale * clipping norm
         # so that gradient = gradient / combined scale
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/memory_monitor.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/memory_monitor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/memory_stats.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/memory_stats.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/memstats_collector.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/param_runtime_order.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/param_runtime_order.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/memory_tracer/utils.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/placement_policy.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/gemini/utils.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/gemini_context.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/gemini_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from . import BaseOpHook
 
 
 @OPHOOKS.register_module
 class ShardGradMemTracerHook(BaseOpHook):
     """
-    A hook to process sharded param before and after FWD and BWD operator executing.
+    A hook to process sharded param before and afther FWD and BWD operator executing.
     """
 
     def __init__(self):
         super().__init__()
 
     def pre_fwd_exec(self, module: torch.nn.Module, *args):
         pass
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from . import BaseOpHook
 
 
 @OPHOOKS.register_module
 class ShardParamHook(BaseOpHook):
     """
-    A hook to process sharded param before and after FWD and BWD operator executing.
+    A hook to process sharded param before and afther FWD and BWD operator executing.
     """
 
     def __init__(self):
         super().__init__()
 
     def niter(self):
         return self._niter
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/ophooks/utils.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/stateful_tensor.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/stateful_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         self._warmup = False
         self._compute_idx = -1
         self._cpu_gpu_move_volume = 0
         self._layout_time = 0
         self._evict_time = 0
 
     def adjust_layout(self) -> None:
-        """ Adjust the layout of stateful tensor according to the information provided
+        """ Adjust the layout of statefuil tensor according to the information provided
         by mem_stats_collector, which should belongs to a Sharded Model.
         """
         # find stateful tensor in state COMPUTE
         cuda_demand = StatefulTensor.GST_MGR.state_mem['cpu'][TensorState.COMPUTE]
         start = time()
         move_to_cuda_tensor_list, hold_cuda_tensor_list = self._get_layout_info(self._compute_idx, self._warmup)
         self._layout_time += time() - start
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/tensor_placement_policy.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/tensor_placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/gemini/tensor_utils.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/init_ctx/init_context.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/init_ctx/init_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         return self.config.shard_param
 
     @staticmethod
     def calc_fanin_fanout(tensor: torch.Tensor):
         """We use this function to substitute fan-in and fan-out calculation in torch.nn.init.
         This can help us get correct fan-in and fan-out for sharded tensor.
         """
-        assert isinstance(tensor, nn.Parameter), "Sharded tensor initialization is only allowed for parameters"
+        assert isinstance(tensor, nn.Parameter), "Sharded tensor initilization is only allowed for paramters"
 
         # get correct shape of input tensor
         if not hasattr(tensor, 'colo_attr') or not tensor.colo_attr.param_is_sharded:
             tensor_shape = tensor.shape
         else:
             tensor_shape = tensor.colo_attr.sharded_data_tensor.origin_shape
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/shard_utils/base_shard_strategy.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/base_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .tensor_shard_strategy import TensorShardStrategy
 
 
 class BucketTensorShardStrategy(TensorShardStrategy):
     """Use the same shard scheme as `TensorShardStrategy`'s, but it gathers tensors of a sub-module together,
     which will fully utilize network bandwidth.
     It is especially useful when sub-module contains bias,
-    since we cannot utilize network bandwidth well if we only gather a bias tensor (bias is usually small).
+    since we cannot utilize network bandwidth well if we only gather a bias tensor (bias is usaully small).
     """
 
     def gather(self, tensor_list: List[ShardedTensor], process_group: Optional[dist.ProcessGroup] = None):
 
         tensor_list: List[ShardedTensor] = [t for t in tensor_list if t.is_sharded]
         if len(tensor_list) == 0:
             return
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/shard_utils/commons.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/commons.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_model/_utils.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_model/reduce_scatter.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/reduce_scatter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_model/utils.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_model/zero_hook.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/zero_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,16 @@
         initial_scale (float, optional): Initial scale used by DynamicGradScaler. Defaults to 2**32.
         min_scale (float, optional): Min scale used by DynamicGradScaler. Defaults to 1.
         growth_factor (float, optional): growth_factor used by DynamicGradScaler. Defaults to 2.
         backoff_factor (float, optional): backoff_factor used by DynamicGradScaler. Defaults to 0.5.
         growth_interval (float, optional): growth_interval used by DynamicGradScaler. Defaults to 1000.
         hysteresis (float, optional): hysteresis used by DynamicGradScaler. Defaults to 2.
         max_scale (int, optional): max_scale used by DynamicGradScaler. Defaults to 2**32.
-        dp_process_group (Optional[ProcessGroup], optional): data parallel process group. Defaults to None.
-        mp_process_group (Optional[ProcessGroup], optional): model parallel process group. Defaults to None.
+        dp_process_group (Optional[ProcessGroup], optional): data paralle process group. Defaults to None.
+        mp_process_group (Optional[ProcessGroup], optional): model paralle process group. Defaults to None.
 
     .. _PatrickStar\: Parallel Training of Pre-trained Models via Chunk-based Memory Management:
         https://arxiv.org/abs/2108.05818
     """
 
     def __init__(self,
                  sharded_model: ShardedModelV2,
@@ -270,15 +270,15 @@
     def _register_master_weight(self):
         self.master_params: Dict[Parameter, StatefulTensor] = {}
         for group in self.optim.param_groups:
             for p in group['params']:
                 assert hasattr(p, 'colo_attr'), 'The parameter must be wrapped with ShardedParam'
                 shard_flag = not p.colo_attr.sharded_data_tensor.is_sharded and p.colo_attr.is_replicated
                 if shard_flag:
-                    # we always shard replicated parameters
+                    # we always shard replicated paramters
                     self.shard_strategy.shard([p.colo_attr.sharded_data_tensor], self.dp_process_group)
                 self.master_params[p] = StatefulTensor(cast_tensor_to_fp32(p.colo_attr.data_payload.to(self.device)))
                 if shard_flag:
                     # In this branch, there's no need to shard param
                     # So we gather here
                     self.shard_strategy.gather([p.colo_attr.sharded_data_tensor], self.dp_process_group)
 
@@ -308,15 +308,15 @@
             for p in group['params']:
                 if p.colo_attr.saved_grad.is_null():
                     continue
                 p.colo_attr.saved_grad.trans_state(TensorState.COMPUTE)
                 # If reuse_fp16_shard, grad fp16 which wasn't be offloaded may be evicted to CPU
                 if not p.colo_attr.offload_grad:
                     colo_model_data_tensor_move_inline(p.colo_attr.saved_grad, torch.cuda.current_device())
-                # FIXME(ver217): p.data here is an empty tensor on CUDA and has no useful information
+                # FIXME(ver217): p.data here is an empty tensor on CUDA and has no useful infomation
                 # If we change p.grad directly
                 # it may raise error because of different shape/dtype/device of p.data and p.grad
                 # We just set p.data = p.colo_attr.saved_grad.payload here
                 p.data = p.colo_attr.grad_payload
                 p.grad = p.colo_attr.grad_payload
                 # Set p.data to empty tensor, in case of memory leaking
                 p.colo_attr.set_data_none()
@@ -329,15 +329,15 @@
                 self.master_params[p].trans_state(TensorState.COMPUTE)
                 p.data = self.master_params[p].payload
                 # Now p.data is sharded
                 # So optimizer states are sharded naturally
 
     def _copy_master_model_to_model_fp16(self):
         # Copy master param data (fp32) to payload of colo_attr (fp16)
-        # TODO() improve efficiency by gathering tensors into a chunk and transferring
+        # TODO() improve efficiency by gathering tensors into a chunk and transfering
         # a chunk.
         for group in self.optim.param_groups:
             for p in group['params']:
                 self._copy_master_param_to_param_fp16(p)
 
     def _copy_master_param_to_param_fp16(self, p):
         # flush gradient
@@ -346,15 +346,15 @@
             # in order to use copy below, we should give sharded data tensor a payload
             p.colo_attr.sharded_data_tensor.payload_relay(p.colo_attr.saved_grad)
         else:
             p.colo_attr.saved_grad.set_null()
 
         p.data = self.master_params[p].payload
 
-        # we need to allocate new memory for keep_not_shard parameters
+        # we need to allocate new memory for keep_not_shard paramters
         # in order to use copy, otherwise, the sizes of tensor is not compatible
         if p.colo_attr.data_payload.numel() != p.data.numel():
             p.colo_attr.data_payload_reset(
                 torch.empty(p.data.shape, dtype=p.colo_attr.data_payload.dtype, device=p.colo_attr.data_payload.device))
 
         # TODO() optimize this line CPU (fp32) -> GPU (fp16)
         p.colo_attr.sharded_data_tensor.payload_copy(p.half().detach())
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_param/sharded_param.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_param/sharded_param.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/legacy/sharded_param/sharded_tensor.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_param/sharded_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/low_level/_utils.py` & `colossalai-nightly-2023.4.8/colossalai/zero/low_level/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,26 +87,18 @@
     # where tensor_tmp and tensor indeed point to the same object.
     # You can check this by print(tensor.data_ptr() == tensor_tmp.data_ptr())
     tensor_tmp = tensor.expand_as(tensor)
     grad_acc_obj = tensor_tmp.grad_fn.next_functions[0][0]
     return grad_acc_obj
 
 
-def split_by_dtype(tensor_list):
-    """
-    Splits a list of PyTorch tensors into sublists based on their data type.
-
-    :param tensor_list: A list of PyTorch tensors.
-    :type tensor_list: list[torch.Tensor]
-    :return: A list of sublists, where each sublist contains tensors of a specific data type.
-    :rtype: list[list[torch.Tensor]]
-    """
+def split_half_float_double(tensor_list):
     dtypes = ["torch.cuda.HalfTensor", "torch.cuda.FloatTensor", "torch.cuda.DoubleTensor", "torch.cuda.BFloat16Tensor"]
     buckets = []
-    for _, dtype in enumerate(dtypes):
+    for i, dtype in enumerate(dtypes):
         bucket = [t for t in tensor_list if t.type() == dtype]
         if bucket:
             buckets.append(bucket)
     return buckets
 
 
 def reduce_tensor_dp_group(tensor: torch.Tensor,
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/low_level/bookkeeping/bucket_store.py` & `colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/bucket_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/low_level/bookkeeping/gradient_store.py` & `colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/gradient_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/low_level/bookkeeping/parameter_store.py` & `colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/parameter_store.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 
 class ParameterStore(BaseStore):
 
     def __init__(self, torch_pg: ProcessGroup):
         super().__init__(torch_pg)
         # param partitioning data structures
-        self._param_to_rank = dict()
-        self._rank_group_id_to_param_list = dict()
-        self._rank_group_id_to_flat_param = dict()
+        self._fp16_param_to_rank = dict()
+        self._rank_groupid_to_fp16_param_list = dict()
+        self._rank_group_id_to_flat_fp16_param = dict()
 
         # param reduction data structures
         self._is_param_reduced = dict()
         self._reduced_param = []
 
     def set_param_to_rank(self, tensor: Tensor, rank: int) -> None:
         """
@@ -25,59 +25,59 @@
 
         :param tensor: A :class:`torch.Tensor` object
         :type tensor: torch.Tensor
         :param rank: The rank of which the process is responsible for updating the parameter
         :type rank: int
         """
 
-        self._param_to_rank[tensor] = rank
+        self._fp16_param_to_rank[tensor] = rank
 
     def get_param_rank(self, tensor: Tensor) -> int:
         """
         Gives the rank which the parameter belongs to
 
         :param tensor: A :class:`torch.Tensor` object
         :type tensor: torch.Tensor
         """
-        return self._param_to_rank[tensor]
+        return self._fp16_param_to_rank[tensor]
 
     def belongs_to_current_rank(self, tensor) -> bool:
         """
         Check whether a parameter is supposed to be updated by the process of the current rank
 
         :param tensor: A :class:`torch.Tensor` object
         :type tensor: torch.Tensor
 
         :return: True if the parameter should be updated by the current rank. Otherwise false.
         :rtype: bool
         """
 
-        tensor_rank = self._param_to_rank[tensor]
+        tensor_rank = self._fp16_param_to_rank[tensor]
         return tensor_rank == self._local_rank
 
-    def add_param_list_by_rank_group(self, rank, group_id, tensor_list) -> None:
-        if rank not in self._rank_group_id_to_param_list:
-            self._rank_group_id_to_param_list[rank] = dict()
+    def add_fp16_param_list_by_rank_group(self, rank, group_id, tensor_list) -> None:
+        if rank not in self._rank_groupid_to_fp16_param_list:
+            self._rank_groupid_to_fp16_param_list[rank] = dict()
 
-        if group_id not in self._rank_group_id_to_param_list[rank]:
-            self._rank_group_id_to_param_list[rank][group_id] = []
+        if group_id not in self._rank_groupid_to_fp16_param_list[rank]:
+            self._rank_groupid_to_fp16_param_list[rank][group_id] = []
 
-        self._rank_group_id_to_param_list[rank][group_id].extend(tensor_list)
+        self._rank_groupid_to_fp16_param_list[rank][group_id].extend(tensor_list)
 
-    def get_params_by_rank_group(self, rank, group_id) -> List[Tensor]:
-        return self._rank_group_id_to_param_list[rank][group_id]
+    def get_fp16_params_by_rank_group(self, rank, group_id) -> List[Tensor]:
+        return self._rank_groupid_to_fp16_param_list[rank][group_id]
 
-    def add_flat_param_by_rank_group(self, rank, group_id, tensor) -> None:
-        if rank not in self._rank_group_id_to_flat_param:
-            self._rank_group_id_to_flat_param[rank] = dict()
+    def add_flat_fp16_param_by_rank_group(self, rank, group_id, tensor) -> None:
+        if rank not in self._rank_group_id_to_flat_fp16_param:
+            self._rank_group_id_to_flat_fp16_param[rank] = dict()
 
-        self._rank_group_id_to_flat_param[rank][group_id] = tensor
+        self._rank_group_id_to_flat_fp16_param[rank][group_id] = tensor
 
-    def get_flat_param_by_rank_group(self, rank, group_id) -> Tensor:
-        return self._rank_group_id_to_flat_param[rank][group_id]
+    def get_flat_fp16_param_by_rank_group(self, rank, group_id) -> Tensor:
+        return self._rank_group_id_to_flat_fp16_param[rank][group_id]
 
     def is_param_reduced(self, tensor):
         return self._is_param_reduced[tensor]
 
     def set_param_reduction_state(self, tensor, state):
         self._is_param_reduced[tensor] = state
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/low_level/bookkeeping/tensor_bucket.py` & `colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/tensor_bucket.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/low_level/low_level_optim.py` & `colossalai-nightly-2023.4.8/colossalai/zero/low_level/low_level_optim.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from ._utils import (
     calculate_global_norm_from_list,
     compute_norm,
     flatten,
     has_inf_or_nan,
     reduce_tensor_dp_group,
     release_param_grad,
-    split_by_dtype,
+    split_half_float_double,
     sync_param,
 )
 from .bookkeeping import BucketStore, GradientStore, ParameterStore, TensorBucket
 
 
 class LowLevelZeroOptimizer(ColossalaiOptimizer):
     """Optimizer used for ZeRO-1 and ZeRO-2.
@@ -51,15 +51,14 @@
             forced_dtype: Optional[torch.dtype] = None):
 
         # TODO: add support for
         # 1. fp16 master weights
         # 2. contiguous gradients
         # 3. cpu offload
         # 4. support when some parameters requires_grad = False
-        # 5. support layer drop
         super(LowLevelZeroOptimizer, self).__init__(optim=optimizer)
         self._dtype = self.optim.param_groups[0]['params'][0].dtype
         self._logger = get_dist_logger()
         self._verbose = verbose
 
         # stage 2
         self._partition_grads = partition_grad
@@ -86,18 +85,17 @@
             self._dp_global_ranks = gpc.get_ranks_in_group(dp_parallel_mode)
             self._dp_torch_group = gpc.get_group(dp_parallel_mode)
             self._mp_torch_group = None
             if gpc.is_initialized(mp_parallel_mode) and gpc.get_world_size(mp_parallel_mode) > 1:
                 self._mp_torch_group = gpc.get_group(mp_parallel_mode)
         else:
             raise NotImplementedError
-
-        # working and master params for mixed precision training
-        self._working_param_groups = dict()
-        self._master_flat_param_groups_of_current_rank = dict()
+        # fp16 and fp32 params for mixed precision training
+        self._fp16_param_groups = dict()
+        self._fp32_flat_param_groups_of_current_rank = dict()
 
         # communication params
         self._overlap_communication = overlap_communication
         self._reduce_bucket_size = reduce_bucket_size
         self._communication_dtype = communication_dtype
 
         # gradient scaler
@@ -135,62 +133,62 @@
         # and add buffers to parameter store for future access
         for group_id, param_group in enumerate(self.optim.param_groups):
             group_params = list()
             for param in param_group['params']:
                 if param.requires_grad:
                     group_params.append(param)
 
-            # add the working params to working_param_groups for bookkeeping
-            self._working_param_groups[group_id] = group_params
+            # add the fp16 params to fp16_param_groups for bookkeeping
+            self._fp16_param_groups[group_id] = group_params
 
             # assign parameters to ranks
             # the params in the list are sorted
             params_per_rank = self._partition_param_list(group_params)
 
             # store the mapping between param to rank
             # each param should belong to only one rank
             for rank, params in enumerate(params_per_rank):
-                self._param_store.add_param_list_by_rank_group(rank, group_id, params)
+                self._param_store.add_fp16_param_list_by_rank_group(rank, group_id, params)
                 for param in params:
                     self._param_store.set_param_to_rank(param, rank)
 
             # move to cpu to make room to create the flat tensor
             # move_tensor(params, device='cpu')
             for param in group_params:
                 param.data = param.data.cpu()
 
             # flatten the reordered tensors
             for rank in range(self._world_size):
-                tensor_list = self._param_store.get_params_by_rank_group(rank, group_id)
+                tensor_list = self._param_store.get_fp16_params_by_rank_group(rank, group_id)
                 with torch.no_grad():
                     flat_tensor = flatten(tensor_list)
                 flat_tensor = flat_tensor.data.cuda()
-                self._param_store.add_flat_param_by_rank_group(rank, group_id, flat_tensor)
+                self._param_store.add_flat_fp16_param_by_rank_group(rank, group_id, flat_tensor)
 
             # sync parameters
             for rank in range(self._world_size):
-                flat_tensor = self._param_store.get_flat_param_by_rank_group(rank, group_id)
-                tensor_list = self._param_store.get_params_by_rank_group(rank, group_id)
+                flat_tensor = self._param_store.get_flat_fp16_param_by_rank_group(rank, group_id)
+                tensor_list = self._param_store.get_fp16_params_by_rank_group(rank, group_id)
                 sync_param(flat_tensor=flat_tensor, tensor_list=tensor_list)
 
-            # create a copy of fp32 master weights of the parameters for which this rank is responsible
-            working_flat_current_rank = self._param_store.get_flat_param_by_rank_group(self._local_rank, group_id)
-            master_flat_current_rank = working_flat_current_rank.float()
+            # create a copy of fp32 weights of the parameters for which this rank is responsible
+            fp16_flat_current_rank = self._param_store.get_flat_fp16_param_by_rank_group(self._local_rank, group_id)
+            fp32_flat_current_rank = fp16_flat_current_rank.float()
             device = 'cpu' if self._cpu_offload else get_current_device()
-            master_flat_current_rank = master_flat_current_rank.to(device)
-            master_flat_current_rank.requires_grad = True
-            self._master_flat_param_groups_of_current_rank[group_id] = master_flat_current_rank
+            fp32_flat_current_rank = fp32_flat_current_rank.to(device)
+            fp32_flat_current_rank.requires_grad = True
+            self._fp32_flat_param_groups_of_current_rank[group_id] = fp32_flat_current_rank
 
             # need to replace the params in the `params` field in the optimizer
             # so that when the optimizer calls step(), it only updates the tensors
             # managed by this data parallel rank
-            param_group['params'] = [master_flat_current_rank]
+            param_group['params'] = [fp32_flat_current_rank]
 
             # set reduction state
-            for param in self._working_param_groups[group_id]:
+            for param in self._fp16_param_groups[group_id]:
                 self._param_store.set_param_reduction_state(param, False)
 
         # intialize communication stream for
         # communication-compuation overlapping
         if self._overlap_communication:
             self._comm_stream = torch.cuda.Stream()
 
@@ -206,15 +204,15 @@
 
     @property
     def loss_scale(self):
         return self.grad_scaler.scale
 
     @property
     def num_param_groups(self):
-        return len(self._working_param_groups)
+        return len(self._fp16_param_groups)
 
     def _sanity_checks(self):
         assert torch.cuda.is_available(), 'CUDA is required'
         for param_group in self.optim.param_groups:
             group_params = param_group['params']
             for param in group_params:
                 assert param.dtype == self._dtype, \
@@ -258,18 +256,18 @@
     ###########################
 
     def _grad_handler(self, param, grad, reduce_rank):
         self._add_to_reduction_bucket(param, reduce_rank)
         return grad
 
     def _attach_reduction_hook(self):
-        # we iterate over the working params
+        # we iterate over the fp16 params
         # on each param, we register a hook to its AccumulateGrad object
         for group_id in range(self.num_param_groups):
-            param_group = self._working_param_groups[group_id]
+            param_group = self._fp16_param_groups[group_id]
             for param in param_group:
                 if param.requires_grad:
                     # determines the reduction destionation rank
                     # this is only valid for stage 2
                     # dst_rank = None means using all-reduce
                     # else using reduce
                     if self._partition_grads:
@@ -312,15 +310,15 @@
                 self._reduce_tensor_bucket(bucket=param_bucket, reduce_rank=reduce_rank)
                 param_bucket.empty()
 
         if not param_bucket.is_empty():
             self._reduce_tensor_bucket(bucket=param_bucket, reduce_rank=reduce_rank)
 
     def _reduce_grads(self, reduce_rank, grads, bucket_size):
-        grad_buckets_by_dtype = split_by_dtype(grads)
+        grad_buckets_by_dtype = split_half_float_double(grads)
 
         for tensor_list in grad_buckets_by_dtype:
             self._reduce_tensor_list_with_one_dtype(tensor_list=tensor_list,
                                                     bucket_size=bucket_size,
                                                     reduce_rank=reduce_rank)
 
     #######################
@@ -415,15 +413,15 @@
         """
         Set parameter gradients to zero. If set_to_none = True, gradient
         will be set to None to save memory.
 
         :param set_to_none: Whether set the gradient to None. Default value is True.
         :type set_to_none: bool
         """
-        for _, param_group in self._working_param_groups.items():
+        for _, param_group in self._fp16_param_groups.items():
             for param in param_group:
                 if set_to_none:
                     param.grad = None
                 else:
                     if param.grad is not None:
                         param.grad.detach()
                         param.grad.zero_()
@@ -438,85 +436,83 @@
         # check for overflow
         found_inf = self._check_overflow()
         self.grad_scaler.update(found_inf)
 
         # update loss scale if overflow occurs
         if found_inf:
             self._grad_store.reset_all_average_gradients()
-            if self._verbose:
-                self._logger.info(f'Found overflow. Skip step')
             self.zero_grad()
             return
 
-        # copy the grad of working param to master param
+        # copy the grad of fp16 param to fp32 param
         single_grad_partition_groups = []
         norm_groups = []
 
         for group_id in range(self.num_param_groups):
             # compute norm
             norm_group = compute_norm(gradients=self._grad_store.get_averaged_gradients_by_group(group_id),
-                                      params=self._param_store.get_params_by_rank_group(group_id=group_id,
-                                                                                        rank=self._local_rank),
+                                      params=self._param_store.get_fp16_params_by_rank_group(group_id=group_id,
+                                                                                             rank=self._local_rank),
                                       dp_group=self._dp_torch_group,
                                       mp_group=self._mp_torch_group)
             norm_groups.append(norm_group)
 
-            # create flat gradient for the flat fp32 master params
-            working_avg_grads = self._grad_store.get_averaged_gradients_by_group(group_id)
-            flat_working_avg_grads = flatten(working_avg_grads)
-
-            dtype = self._master_flat_param_groups_of_current_rank[group_id].dtype
-            flat_master_avg_grads = flat_working_avg_grads.to(dtype)
-
-            param_shape = self._master_flat_param_groups_of_current_rank[group_id].shape
-            assert param_shape == flat_master_avg_grads.shape, \
-                f'fp32 param and grad have different shape {param_shape} vs {flat_master_avg_grads.shape}'
-
-            single_grad_partition_groups.append(flat_master_avg_grads)
-            device = self._master_flat_param_groups_of_current_rank[group_id].device
-            self._master_flat_param_groups_of_current_rank[group_id].grad = flat_master_avg_grads.to(device)
+            # create flat gradient for the flat fp32 params
+            fp16_avg_grads = self._grad_store.get_averaged_gradients_by_group(group_id)
+            flat_fp16_avg_grads = flatten(fp16_avg_grads)
+
+            dtype = self._fp32_flat_param_groups_of_current_rank[group_id].dtype
+            flat_fp32_avg_grads = flat_fp16_avg_grads.to(dtype)
+
+            param_shape = self._fp32_flat_param_groups_of_current_rank[group_id].shape
+            assert param_shape == flat_fp32_avg_grads.shape, \
+                f'fp32 param and grad have different shape {param_shape} vs {flat_fp32_avg_grads.shape}'
+
+            single_grad_partition_groups.append(flat_fp32_avg_grads)
+            device = self._fp32_flat_param_groups_of_current_rank[group_id].device
+            self._fp32_flat_param_groups_of_current_rank[group_id].grad = flat_fp32_avg_grads.to(device)
             self._grad_store.reset_average_gradients_by_group(group_id)
 
         # unscale and clip grads
         global_norm = calculate_global_norm_from_list(norm_list=norm_groups)
         self._unscale_and_clip_grads(single_grad_partition_groups, global_norm)
 
         # update the parameters
         self.optim.step()
-        # release the master grad
-        release_param_grad(self._master_flat_param_groups_of_current_rank.values())
+        # release the fp32 grad
+        release_param_grad(self._fp32_flat_param_groups_of_current_rank.values())
 
-        # update working partition updated by the current rank
-        for group_id in range(len(self._working_param_groups)):
-            working_param = self._param_store.get_flat_param_by_rank_group(rank=self._local_rank, group_id=group_id)
-            master_param = self._master_flat_param_groups_of_current_rank[group_id]
-            working_param.data.copy_(master_param)
+        # update fp16 partition updated by the current rank
+        for group_id in range(len(self._fp16_param_groups)):
+            fp16_param = self._param_store.get_flat_fp16_param_by_rank_group(rank=self._local_rank, group_id=group_id)
+            fp32_param = self._fp32_flat_param_groups_of_current_rank[group_id]
+            fp16_param.data.copy_(fp32_param)
 
         # broadcast the updated model weights
         handles = []
         for group_id in range(self.num_param_groups):
             for index in range(self._world_size):
                 rank = self._dp_global_ranks[index]
-                working_param = self._param_store.get_flat_param_by_rank_group(rank=index, group_id=group_id)
-                handle = dist.broadcast(working_param, src=rank, group=self._dp_torch_group, async_op=True)
+                fp16_param = self._param_store.get_flat_fp16_param_by_rank_group(rank=index, group_id=group_id)
+                handle = dist.broadcast(fp16_param, src=rank, group=self._dp_torch_group, async_op=True)
                 handles.append(handle)
 
         for handle in handles:
             handle.wait()
 
-    #############################
-    # Mixed Precision Utilities #
-    #############################
+    ##################
+    # FP16 Utilities #
+    ##################
 
     def _check_overflow(self):
         # clear previous overflow record
         self._found_overflow.fill_(0.0)
 
         # check for overflow
-        for group_id in range(len(self._working_param_groups)):
+        for group_id in range(len(self._fp16_param_groups)):
             for avg_grad in self._grad_store.get_averaged_gradients_by_group(group_id):
                 if avg_grad is not None and has_inf_or_nan(avg_grad):
                     self._found_overflow.fill_(1.0)
                     break
 
         # all-reduce across dp group
         dist.all_reduce(self._found_overflow, op=dist.ReduceOp.MAX, group=self._dp_torch_group)
@@ -551,15 +547,15 @@
         # update param already reduced flag
         reduction_states = self._param_store.get_param_reduction_states()
         for tensor, _ in reduction_states.items():
             reduction_states[tensor] = False
 
         # accumulate gradient
         for group_id in range(self.num_param_groups):
-            param_group = self._param_store.get_params_by_rank_group(self._local_rank, group_id)
+            param_group = self._param_store.get_fp16_params_by_rank_group(self._local_rank, group_id)
 
             avg_gradients_group = self._grad_store.get_averaged_gradients_by_group(group_id)
 
             param_idx = 0
             for param in param_group:
                 if param.grad is not None:
                     if len(avg_gradients_group) == param_idx:
@@ -572,16 +568,16 @@
         # thus, can clear this
         self.zero_grad()
 
     def _reduce_grad_stage1(self):
         # if not overlapping communication (no reduction hook is attached)
         # we need to manually reduce these gradients
         if not self._overlap_communication:
-            for group_id in range(len(self._working_param_groups)):
-                param_group = self._working_param_groups[group_id]
+            for group_id in range(len(self._fp16_param_groups)):
+                param_group = self._fp16_param_groups[group_id]
                 for param in param_group:
                     if param.grad is not None:
                         self._add_to_reduction_bucket(param)
 
         # we need to reduce the gradients
         # left in the communication bucket
         self._run_reduction()
```

### Comparing `colossalai-nightly-2023.4.29/colossalai/zero/wrapper.py` & `colossalai-nightly-2023.4.8/colossalai/zero/wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 
 import torch
 import torch.nn as nn
 
 from .gemini import GeminiDDP
 
 
-def zero_model_wrapper(model: nn.Module,
-                       zero_stage: int = 1,
-                       gemini_config: Optional[Dict] = None,
-                       verbose: bool = False):
+def zero_model_wrapper(model: nn.Module, zero_stage: int = 1, gemini_config: Optional[Dict] = None):
     """This wrapper function is used to wrap your training model for ZeRO DDP.
 
     Example:
 
         >>> with ColoInitContext():
         >>>     my_model = Bert()
         >>> my_optim = SGD(my_model.parameters(), lr = 1e-3)
@@ -22,15 +19,15 @@
         >>> zero_optim = zero_optim_wrapper(zero_model, my_optim)
 
     Args:
         model (nn.Module): The model used in ZeRO DDP.
         zero_stage (int, optional): The stage of ZeRO DDP. You can find more information in ZeRO's paper.
             https://arxiv.org/abs/1910.02054
         gemini_config (dict, optional): The configuration dictionary of `GeminiDDP`. `GeminiDDP` is enabled
-            when the stage is set to 3. You can set the arguments of `GeminiDDP` in the gemini_config.
+            when the stage is set to 3. You can set the arguemnts of `GeminiDDP` in the gemini_config.
             Here is an example where we set the device of the model, the placement policy of Gemini, and the
             size of hidden dimension to help Gemini find out a unified chunk size.
 
             Example:
 
                 >>> config_dict = dict(device=torch.cuda.current_device(), hidden_dim=1024, placement_policy='auto')
                 >>> model = zero_model_wrapper(model, zero_stage=3, gemini_config=config_dict)
@@ -39,15 +36,15 @@
 
     if gemini_config is None:
         gemini_config = dict()
 
     if zero_stage in [1, 2]:
         wrapped_model = model
     else:
-        wrapped_model = GeminiDDP(model, **gemini_config, verbose=verbose)
+        wrapped_model = GeminiDDP(model, **gemini_config)
 
     setattr(wrapped_model, "_colo_zero_stage", zero_stage)
 
     return wrapped_model
 
 
 def zero_optim_wrapper(model: nn.Module,
@@ -57,16 +54,15 @@
                        backoff_factor: float = 0.5,
                        growth_interval: int = 1000,
                        hysteresis: int = 2,
                        min_scale: float = 1,
                        max_scale: float = 2**32,
                        max_norm: float = 0.0,
                        norm_type: float = 2.0,
-                       optim_config: Optional[Dict] = None,
-                       verbose: bool = False):
+                       optim_config: Optional[Dict] = None):
     """This wrapper function is used to wrap your training optimizer for ZeRO DDP.
 
     Args:
         model (nn.Module): Your model wrapped by `zero_model_wrapper`
         optimizer (torch.optim.Optimizer): Your initialized optimizer
         initial_scale (float, optional): initial_scale used by DynamicGradScaler.
         min_scale (float, optional): min_scale used by DynamicGradScaler.
@@ -74,20 +70,19 @@
         backoff_factor (float, optional): backoff_factor used by DynamicGradScaler.
         growth_interval (float, optional): growth_interval used by DynamicGradScaler.
         hysteresis (float, optional): hysteresis used by DynamicGradScaler.
         max_scale (int, optional): max_scale used by DynamicGradScaler.
         max_norm (float, optional): max_norm used for `clip_grad_norm`. You should notice that you shall not do
             clip_grad_norm by yourself when using ZeRO DDP. The ZeRO optimizer will take care of clip_grad_norm.
         norm_type (float, optional): norm_type used for `clip_grad_norm`.
-        optim_config (dict, optional): The configuration used for the ZeRO optimizer.
+        optim_config (dict, optinoal): The configuration used for the ZeRO optimizer.
             Example:
 
                 >>> zero2_config = dict(reduce_bucket_size=12 * 1024 * 1024, overlap_communication=True)
                 >>> optim = zero_optim_wrapper(model, optim, optim_config=zero2_config)
-        verbose (bool, optional): Whether to print the verbose info.
     """
     assert hasattr(model, "_colo_zero_stage"), "You should use `zero_ddp_wrapper` first"
     zero_stage = getattr(model, "_colo_zero_stage")
 
     assert norm_type == 2.0, "Current ZeRO optimizers only support 'norm_type=2'"
 
     if optim_config is None:
@@ -103,12 +98,12 @@
     config_dict['min_scale'] = min_scale
     config_dict['max_scale'] = max_scale
 
     if zero_stage in [1, 2]:
         from colossalai.zero.low_level import LowLevelZeroOptimizer
         config_dict['partition_grad'] = zero_stage == 2
         config_dict['clip_grad_norm'] = max_norm
-        return LowLevelZeroOptimizer(optimizer, **config_dict, verbose=verbose)
+        return LowLevelZeroOptimizer(optimizer, **config_dict)
     else:
         from colossalai.zero.gemini.gemini_optimizer import ZeroOptimizer
         config_dict['clipping_norm'] = max_norm
-        return ZeroOptimizer(optimizer, model, **config_dict, verbose=verbose)
+        return ZeroOptimizer(optimizer, model, **config_dict)
```

### Comparing `colossalai-nightly-2023.4.29/colossalai_nightly.egg-info/PKG-INFO` & `colossalai-nightly-2023.4.8/colossalai_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai-nightly
-Version: 2023.4.29
+Version: 2023.4.8
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
@@ -46,22 +46,14 @@
         * [2022/09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https://www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-fundraising-led-by-bluerun-ventures-in-the)
         
         ## Table of Contents
         <ul>
          <li><a href="#Why-Colossal-AI">Why Colossal-AI</a> </li>
          <li><a href="#Features">Features</a> </li>
          <li>
-           <a href="#Colossal-AI-in-the-Real-World">Colossal-AI for Real World Applications</a>
-           <ul>
-             <li><a href="#ColossalChat">ColossalChat: An Open-Source Solution for Cloning ChatGPT With a Complete RLHF Pipeline</a></li>
-             <li><a href="#AIGC">AIGC: Acceleration of Stable Diffusion</a></li>
-             <li><a href="#Biomedicine">Biomedicine: Acceleration of AlphaFold Protein Structure</a></li>
-           </ul>
-         </li>
-         <li>
            <a href="#Parallel-Training-Demo">Parallel Training Demo</a>
            <ul>
              <li><a href="#GPT-3">GPT-3</a></li>
              <li><a href="#GPT-2">GPT-2</a></li>
              <li><a href="#BERT">BERT</a></li>
              <li><a href="#PaLM">PaLM</a></li>
              <li><a href="#OPT">OPT</a></li>
@@ -80,14 +72,22 @@
            <a href="#Inference-Energon-AI-Demo">Inference (Energon-AI) Demo</a>
            <ul>
              <li><a href="#GPT-3-Inference">GPT-3</a></li>
              <li><a href="#OPT-Serving">OPT-175B Online Serving for Text Generation</a></li>
              <li><a href="#BLOOM-Inference">176B BLOOM</a></li>
            </ul>
          </li>
+           <li>
+           <a href="#Colossal-AI-in-the-Real-World">Colossal-AI for Real World Applications</a>
+           <ul>
+             <li><a href="#ColossalChat">ColossalChat: An Open-Source Solution for Cloning ChatGPT With a Complete RLHF Pipeline</a></li>
+             <li><a href="#AIGC">AIGC: Acceleration of Stable Diffusion</a></li>
+             <li><a href="#Biomedicine">Biomedicine: Acceleration of AlphaFold Protein Structure</a></li>
+           </ul>
+         </li>
          <li>
            <a href="#Installation">Installation</a>
            <ul>
              <li><a href="#PyPI">PyPI</a></li>
              <li><a href="#Install-From-Source">Install From Source</a></li>
            </ul>
          </li>
@@ -129,96 +129,14 @@
           - Parallelism based on the configuration file
         
         - Inference
           - [Energon-AI](https://github.com/hpcaitech/EnergonAI)
         
         <p align="right">(<a href="#top">back to top</a>)</p>
         
-        ## Colossal-AI in the Real World
-        
-        ### ColossalChat
-        
-        <div align="center">
-           <a href="https://chat.colossalai.org/">
-           <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Chat-demo.png" width="700" />
-           </a>
-        </div>
-        
-        [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://chat.colossalai.org)
-        
-        <p id="ColossalChat_scaling" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT%20scaling.png" width=800/>
-        </p>
-        
-        - Up to 7.73 times faster for single server training and 1.42 times faster for single-GPU inference
-        
-        <p id="ColossalChat-1GPU" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT-1GPU.jpg" width=450/>
-        </p>
-        
-        - Up to 10.3x growth in model capacity on one GPU
-        - A mini demo training process requires only 1.62GB of GPU memory (any consumer-grade GPU)
-        
-        <p id="ColossalChat-LoRA" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/LoRA%20data.jpg" width=600/>
-        </p>
-        
-        - Increase the capacity of the fine-tuning model by up to 3.7 times on a single GPU
-        - Keep at a sufficiently high running speed
-        
-        <p align="right">(<a href="#top">back to top</a>)</p>
-        
-        
-        ### AIGC
-        Acceleration of AIGC (AI-Generated Content) models such as [Stable Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable Diffusion v2](https://github.com/Stability-AI/stablediffusion).
-        <p id="diffusion_train" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20v2.png" width=800/>
-        </p>
-        
-        - [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and hardware cost by up to 46x (from A100 to RTX3060).
-        
-        <p id="diffusion_demo" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/DreamBooth.png" width=800/>
-        </p>
-        
-        - [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/dreambooth): Personalize your model using just 3-5 images of the desired subject.
-        
-        <p id="inference" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20Inference.jpg" width=800/>
-        </p>
-        
-        - [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce inference GPU memory consumption by 2.5x.
-        
-        
-        <p align="right">(<a href="#top">back to top</a>)</p>
-        
-        ### Biomedicine
-        Acceleration of [AlphaFold Protein Structure](https://alphafold.ebi.ac.uk/)
-        
-        <p id="FastFold" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/FastFold.jpg" width=800/>
-        </p>
-        
-        - [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and inference on GPU Clusters, faster data processing, inference sequence containing more than 10000 residues.
-        
-        <p id="FastFold-Intel" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/data%20preprocessing%20with%20Intel.jpg" width=600/>
-        </p>
-        
-        - [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference acceleration and 39% cost reduce.
-        
-        <p id="xTrimoMultimer" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/xTrimoMultimer_Table.jpg" width=800/>
-        </p>
-        
-        - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer): accelerating structure prediction of protein monomers and multimer by 11x.
-        
-        
-        <p align="right">(<a href="#top">back to top</a>)</p>
-        
         ## Parallel Training Demo
         
         ### GPT-3
         <p align="center">
         <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT3-v5.png" width=700/>
         </p>
         
@@ -304,22 +222,102 @@
         <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/BLOOM%20Inference.PNG" width=800/>
         </p>
         
         - [BLOOM](https://github.com/hpcaitech/EnergonAI/tree/main/examples/bloom): Reduce hardware deployment costs of 176-billion-parameter BLOOM by more than 10 times.
         
         <p align="right">(<a href="#top">back to top</a>)</p>
         
+        ## Colossal-AI in the Real World
+        
+        ### ColossalChat
+        
+        <div align="center">
+           <a href="https://chat.colossalai.org/">
+           <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Chat-demo.png" width="700" />
+           </a>
+        </div>
+        
+        [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://chat.colossalai.org)
+        
+        <p id="ColossalChat_scaling" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT%20scaling.png" width=800/>
+        </p>
+        
+        - Up to 7.73 times faster for single server training and 1.42 times faster for single-GPU inference
+        
+        <p id="ColossalChat-1GPU" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT-1GPU.jpg" width=450/>
+        </p>
+        
+        - Up to 10.3x growth in model capacity on one GPU
+        - A mini demo training process requires only 1.62GB of GPU memory (any consumer-grade GPU)
+        
+        <p id="ColossalChat-LoRA" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/LoRA%20data.jpg" width=600/>
+        </p>
+        
+        - Increase the capacity of the fine-tuning model by up to 3.7 times on a single GPU
+        - Keep at a sufficiently high running speed
+        
+        <p align="right">(<a href="#top">back to top</a>)</p>
+        
+        
+        ### AIGC
+        Acceleration of AIGC (AI-Generated Content) models such as [Stable Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable Diffusion v2](https://github.com/Stability-AI/stablediffusion).
+        <p id="diffusion_train" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20v2.png" width=800/>
+        </p>
+        
+        - [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and hardware cost by up to 46x (from A100 to RTX3060).
+        
+        <p id="diffusion_demo" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/DreamBooth.png" width=800/>
+        </p>
+        
+        - [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/dreambooth): Personalize your model using just 3-5 images of the desired subject.
+        
+        <p id="inference" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20Inference.jpg" width=800/>
+        </p>
+        
+        - [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce inference GPU memory consumption by 2.5x.
+        
+        
+        <p align="right">(<a href="#top">back to top</a>)</p>
+        
+        ### Biomedicine
+        Acceleration of [AlphaFold Protein Structure](https://alphafold.ebi.ac.uk/)
+        
+        <p id="FastFold" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/FastFold.jpg" width=800/>
+        </p>
+        
+        - [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and inference on GPU Clusters, faster data processing, inference sequence containing more than 10000 residues.
+        
+        <p id="FastFold-Intel" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/data%20preprocessing%20with%20Intel.jpg" width=600/>
+        </p>
+        
+        - [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference acceleration and 39% cost reduce.
+        
+        <p id="xTrimoMultimer" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/xTrimoMultimer_Table.jpg" width=800/>
+        </p>
+        
+        - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer): accelerating structure prediction of protein monomers and multimer by 11x.
+        
+        
+        <p align="right">(<a href="#top">back to top</a>)</p>
+        
         ## Installation
         
         Requirements:
         - PyTorch >= 1.11 (PyTorch 2.x in progress)
         - Python >= 3.7
         - CUDA >= 11.0
-        - [NVIDIA GPU Compute Capability](https://developer.nvidia.com/cuda-gpus) >= 7.0 (V100/RTX20 and higher)
-        - Linux OS
         
         If you encounter any problem with installation, you may want to raise an [issue](https://github.com/hpcaitech/ColossalAI/issues/new/choose) in this repository.
         
         ### Install from PyPI
         
         You can easily install Colossal-AI with the following command. **By default, we do not build PyTorch extensions during installation.**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.4.29 Summary: An
+Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.4.8 Summary: An
 integrated large-scale model training system with efficient parallelization
 techniques Home-page: https://www.colossalai.org License: Apache Software
 License 2.0 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/
 discussions Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/
 issues Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
@@ -45,19 +45,14 @@
 Sequence Exceeding 10,000](https://www.hpc-ai.tech/blog/use-a-laptop-to-
 analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding) * [2022/
 09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https:/
 /www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-
 fundraising-led-by-bluerun-ventures-in-the) ## Table of Contents
     * Why_Colossal-AI
     * Features
-    * Colossal-AI_for_Real_World_Applications
-          o ColossalChat:_An_Open-Source_Solution_for_Cloning_ChatGPT_With_a
-            Complete_RLHF_Pipeline
-          o AIGC:_Acceleration_of_Stable_Diffusion
-          o Biomedicine:_Acceleration_of_AlphaFold_Protein_Structure
     * Parallel_Training_Demo
           o GPT-3
           o GPT-2
           o BERT
           o PaLM
           o OPT
           o ViT
@@ -65,14 +60,19 @@
     * Single_GPU_Training_Demo
           o GPT-2
           o PaLM
     * Inference_(Energon-AI)_Demo
           o GPT-3
           o OPT-175B_Online_Serving_for_Text_Generation
           o 176B_BLOOM
+    * Colossal-AI_for_Real_World_Applications
+          o ColossalChat:_An_Open-Source_Solution_for_Cloning_ChatGPT_With_a
+            Complete_RLHF_Pipeline
+          o AIGC:_Acceleration_of_Stable_Diffusion
+          o Biomedicine:_Acceleration_of_AlphaFold_Protein_Structure
     * Installation
           o PyPI
           o Install_From_Source
     * Use_Docker
     * Community
     * Contributing
     * Cite_Us
@@ -91,71 +91,14 @@
 (https://arxiv.org/abs/2105.13120) - [Zero Redundancy Optimizer (ZeRO)](https:/
 /arxiv.org/abs/1910.02054) - [Auto-Parallelism](https://arxiv.org/abs/
 2302.02599) - Heterogeneous Memory Management - [PatrickStar](https://
 arxiv.org/abs/2108.05818) - Friendly Usage - Parallelism based on the
 configuration file - Inference - [Energon-AI](https://github.com/hpcaitech/
 EnergonAI)
                                                                   (back_to_top)
-## Colossal-AI in the Real World ### ColossalChat
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                Chat-demo.png]
-[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/
-Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/
-chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/
-ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/
-@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://
-chat.colossalai.org)
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                        chatgpt/ChatGPT%20scaling.png]
-- Up to 7.73 times faster for single server training and 1.42 times faster for
-single-GPU inference
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                           chatgpt/ChatGPT-1GPU.jpg]
-- Up to 10.3x growth in model capacity on one GPU - A mini demo training
-process requires only 1.62GB of GPU memory (any consumer-grade GPU)
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                           chatgpt/LoRA%20data.jpg]
-- Increase the capacity of the fine-tuning model by up to 3.7 times on a single
-GPU - Keep at a sufficiently high running speed
-                                                                  (back_to_top)
-### AIGC Acceleration of AIGC (AI-Generated Content) models such as [Stable
-Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable
-Diffusion v2](https://github.com/Stability-AI/stablediffusion).
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                         Stable%20Diffusion%20v2.png]
-- [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/
-diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and
-hardware cost by up to 46x (from A100 to RTX3060).
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                DreamBooth.png]
-- [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/
-examples/images/dreambooth): Personalize your model using just 3-5 images of
-the desired subject.
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                      Stable%20Diffusion%20Inference.jpg]
-- [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/
-images/diffusion): Reduce inference GPU memory consumption by 2.5x.
-                                                                  (back_to_top)
-### Biomedicine Acceleration of [AlphaFold Protein Structure](https://
-alphafold.ebi.ac.uk/)
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                 FastFold.jpg]
-- [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and
-inference on GPU Clusters, faster data processing, inference sequence
-containing more than 10000 residues.
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                   data%20preprocessing%20with%20Intel.jpg]
-- [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference
-acceleration and 39% cost reduce.
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                           xTrimoMultimer_Table.jpg]
-- [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer):
-accelerating structure prediction of protein monomers and multimer by 11x.
-                                                                  (back_to_top)
 ## Parallel Training Demo ### GPT-3
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                                  GPT3-v5.png]
 - Save 50% GPU resources and 10.7% acceleration ### GPT-2 [https://
 raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT2.png]
 - 11x lower GPU memory consumption, and superlinear scaling efficiency with
 Tensor Parallelism [https://raw.githubusercontent.com/hpcaitech/public_assets/
@@ -205,35 +148,91 @@
 Try 175-billion-parameter OPT online services
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                             BLOOM%20Inference.PNG]
 - [BLOOM](https://github.com/hpcaitech/EnergonAI/tree/main/examples/bloom):
 Reduce hardware deployment costs of 176-billion-parameter BLOOM by more than 10
 times.
                                                                   (back_to_top)
+## Colossal-AI in the Real World ### ColossalChat
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                Chat-demo.png]
+[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/
+Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/
+chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/
+ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/
+@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
+with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://
+chat.colossalai.org)
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                        chatgpt/ChatGPT%20scaling.png]
+- Up to 7.73 times faster for single server training and 1.42 times faster for
+single-GPU inference
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                           chatgpt/ChatGPT-1GPU.jpg]
+- Up to 10.3x growth in model capacity on one GPU - A mini demo training
+process requires only 1.62GB of GPU memory (any consumer-grade GPU)
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                           chatgpt/LoRA%20data.jpg]
+- Increase the capacity of the fine-tuning model by up to 3.7 times on a single
+GPU - Keep at a sufficiently high running speed
+                                                                  (back_to_top)
+### AIGC Acceleration of AIGC (AI-Generated Content) models such as [Stable
+Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable
+Diffusion v2](https://github.com/Stability-AI/stablediffusion).
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                         Stable%20Diffusion%20v2.png]
+- [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/
+diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and
+hardware cost by up to 46x (from A100 to RTX3060).
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                DreamBooth.png]
+- [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/
+examples/images/dreambooth): Personalize your model using just 3-5 images of
+the desired subject.
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                      Stable%20Diffusion%20Inference.jpg]
+- [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/
+images/diffusion): Reduce inference GPU memory consumption by 2.5x.
+                                                                  (back_to_top)
+### Biomedicine Acceleration of [AlphaFold Protein Structure](https://
+alphafold.ebi.ac.uk/)
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                 FastFold.jpg]
+- [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and
+inference on GPU Clusters, faster data processing, inference sequence
+containing more than 10000 residues.
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                   data%20preprocessing%20with%20Intel.jpg]
+- [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference
+acceleration and 39% cost reduce.
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                           xTrimoMultimer_Table.jpg]
+- [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer):
+accelerating structure prediction of protein monomers and multimer by 11x.
+                                                                  (back_to_top)
 ## Installation Requirements: - PyTorch >= 1.11 (PyTorch 2.x in progress) -
-Python >= 3.7 - CUDA >= 11.0 - [NVIDIA GPU Compute Capability](https://
-developer.nvidia.com/cuda-gpus) >= 7.0 (V100/RTX20 and higher) - Linux OS If
-you encounter any problem with installation, you may want to raise an [issue]
-(https://github.com/hpcaitech/ColossalAI/issues/new/choose) in this repository.
-### Install from PyPI You can easily install Colossal-AI with the following
-command. **By default, we do not build PyTorch extensions during
-installation.** ```bash pip install colossalai ``` **Note: only Linux is
-supported for now.** However, if you want to build the PyTorch extensions
-during installation, you can set `CUDA_EXT=1`. ```bash CUDA_EXT=1 pip install
-colossalai ``` **Otherwise, CUDA kernels will be built during runtime when you
-actually need them.** We also keep releasing the nightly version to PyPI every
-week. This allows you to access the unreleased features and bug fixes in the
-main branch. Installation can be made via ```bash pip install colossalai-
-nightly ``` ### Download From Source > The version of Colossal-AI will be in
-line with the main branch of the repository. Feel free to raise an issue if you
-encounter any problems. :) ```shell git clone https://github.com/hpcaitech/
-ColossalAI.git cd ColossalAI # install colossalai pip install . ``` By default,
-we do not compile CUDA/C++ kernels. ColossalAI will build them during runtime.
-If you want to install and enable CUDA kernel fusion (compulsory installation
-when using fused optimizer): ```shell CUDA_EXT=1 pip install . ```
+Python >= 3.7 - CUDA >= 11.0 If you encounter any problem with installation,
+you may want to raise an [issue](https://github.com/hpcaitech/ColossalAI/
+issues/new/choose) in this repository. ### Install from PyPI You can easily
+install Colossal-AI with the following command. **By default, we do not build
+PyTorch extensions during installation.** ```bash pip install colossalai ```
+**Note: only Linux is supported for now.** However, if you want to build the
+PyTorch extensions during installation, you can set `CUDA_EXT=1`. ```bash
+CUDA_EXT=1 pip install colossalai ``` **Otherwise, CUDA kernels will be built
+during runtime when you actually need them.** We also keep releasing the
+nightly version to PyPI every week. This allows you to access the unreleased
+features and bug fixes in the main branch. Installation can be made via ```bash
+pip install colossalai-nightly ``` ### Download From Source > The version of
+Colossal-AI will be in line with the main branch of the repository. Feel free
+to raise an issue if you encounter any problems. :) ```shell git clone https://
+github.com/hpcaitech/ColossalAI.git cd ColossalAI # install colossalai pip
+install . ``` By default, we do not compile CUDA/C++ kernels. ColossalAI will
+build them during runtime. If you want to install and enable CUDA kernel fusion
+(compulsory installation when using fused optimizer): ```shell CUDA_EXT=1 pip
+install . ```
                                                                   (back_to_top)
 ## Use Docker ### Pull from DockerHub You can directly pull the docker image
 from our [DockerHub page](https://hub.docker.com/r/hpcaitech/colossalai). The
 image is automatically uploaded upon release. ### Build On Your Own Run the
 following command to build a docker image from Dockerfile provided. > Building
 Colossal-AI from scratch requires GPU support, you need to use Nvidia Docker
 Runtime as the default when doing `docker build`. More details can be found
```

### Comparing `colossalai-nightly-2023.4.29/colossalai_nightly.egg-info/SOURCES.txt` & `colossalai-nightly-2023.4.8/colossalai_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,14 @@
 colossalai/booster/mixed_precision/bf16.py
 colossalai/booster/mixed_precision/fp16_apex.py
 colossalai/booster/mixed_precision/fp16_torch.py
 colossalai/booster/mixed_precision/fp8.py
 colossalai/booster/mixed_precision/mixed_precision_base.py
 colossalai/booster/plugin/__init__.py
 colossalai/booster/plugin/gemini_plugin.py
-colossalai/booster/plugin/low_level_zero_plugin.py
 colossalai/booster/plugin/plugin_base.py
 colossalai/booster/plugin/torch_ddp_plugin.py
 colossalai/builder/__init__.py
 colossalai/builder/builder.py
 colossalai/checkpoint_io/__init__.py
 colossalai/checkpoint_io/checkpoint_io_base.py
 colossalai/checkpoint_io/general_checkpoint_io.py
```

### Comparing `colossalai-nightly-2023.4.29/op_builder/__init__.py` & `colossalai-nightly-2023.4.8/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/op_builder/builder.py` & `colossalai-nightly-2023.4.8/op_builder/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Licensed under the MIT License.
 import importlib
 import os
 import time
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import List, Optional
+from typing import List
 
 from .utils import check_cuda_availability, check_system_pytorch_cuda_match, print_rank_0
 
 
 class Builder(ABC):
     """
     Builder is the base class to build extensions for PyTorch.
@@ -74,15 +74,15 @@
         This function should return a list of source files for extensions.
         """
         raise NotImplementedError
 
     @abstractmethod
     def include_dirs(self) -> List[str]:
         """
-        This function should return a list of include files for extensions.
+        This function should return a list of inlcude files for extensions.
         """
         pass
 
     @abstractmethod
     def cxx_flags(self) -> List[str]:
         """
         This function should return a list of cxx compilation flags for extensions.
@@ -123,49 +123,47 @@
 
         if not TORCH_AVAILABLE:
             raise ModuleNotFoundError(
                 "PyTorch is not found. You need to install PyTorch first in order to build CUDA extensions")
 
         if CUDA_HOME is None:
             raise RuntimeError(
-                "CUDA_HOME is not found. You need to export CUDA_HOME environment variable or install CUDA Toolkit first in order to build CUDA extensions"
+                "CUDA_HOME is not found. You need to export CUDA_HOME environment vairable or install CUDA Toolkit first in order to build CUDA extensions"
             )
 
         # make sure CUDA is available for compilation during
         cuda_available = check_cuda_availability()
         if not cuda_available:
-            raise RuntimeError("CUDA is not available on your system as torch.cuda.is_available() returns False.")
+            raise RuntimeError("CUDA is not available on your system as torch.cuda.is_avaible() returns False.")
 
         # make sure system CUDA and pytorch CUDA match, an error will raised inside the function if not
         check_system_pytorch_cuda_match(CUDA_HOME)
 
-    def load(self, verbose: Optional[bool] = None):
+    def load(self, verbose=True):
         """
         load the kernel during runtime. If the kernel is not built during pip install, it will build the kernel.
         If the kernel is built during runtime, it will be stored in `~/.cache/colossalai/torch_extensions/`. If the
         kernel is built during pip install, it can be accessed through `colossalai._C`.
 
         Warning: do not load this kernel repeatedly during model execution as it could slow down the training process.
 
         Args:
             verbose (bool, optional): show detailed info. Defaults to True.
         """
-        if verbose is None:
-            verbose = os.environ.get('CAI_KERNEL_VERBOSE', '0') == '1'
         # if the kernel has be compiled and cached, we directly use it
         if self.cached_op_module is not None:
             return self.cached_op_module
 
         try:
             # if the kernel has been pre-built during installation
             # we just directly import it
             op_module = self.import_op()
             if verbose:
                 print_rank_0(
-                    f"[extension] OP {self.prebuilt_import_path} has been compiled ahead of time, skip building.")
+                    f"[extension] OP {self.prebuilt_import_path} has been compileed ahead of time, skip building.")
         except ImportError:
             # check environment
             self.check_runtime_build_environment()
 
             # time the kernel compilation
             start_build = time.time()
```

### Comparing `colossalai-nightly-2023.4.29/op_builder/cpu_adam.py` & `colossalai-nightly-2023.4.8/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/op_builder/fused_optim.py` & `colossalai-nightly-2023.4.8/op_builder/fused_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/op_builder/layernorm.py` & `colossalai-nightly-2023.4.8/op_builder/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/op_builder/moe.py` & `colossalai-nightly-2023.4.8/op_builder/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/op_builder/multi_head_attn.py` & `colossalai-nightly-2023.4.8/op_builder/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/op_builder/scaled_masked_softmax.py` & `colossalai-nightly-2023.4.8/op_builder/scaled_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/op_builder/scaled_upper_triangle_masked_softmax.py` & `colossalai-nightly-2023.4.8/op_builder/scaled_upper_triangle_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/op_builder/utils.py` & `colossalai-nightly-2023.4.8/op_builder/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     if bare_metal_major != torch_cuda_major:
         raise Exception(
             f'[extension] Failed to build PyTorch extension because the detected CUDA version ({bare_metal_major}.{bare_metal_minor}) '
             f'mismatches the version that was used to compile PyTorch ({torch_cuda_major}.{torch_cuda_minor}).'
             'Please make sure you have set the CUDA_HOME correctly and installed the correct PyTorch in https://pytorch.org/get-started/locally/ .'
         )
 
+    print(bare_metal_minor != torch_cuda_minor)
     if bare_metal_minor != torch_cuda_minor:
         warnings.warn(
             f"[extension] The CUDA version on the system ({bare_metal_major}.{bare_metal_minor}) does not match with the version ({torch_cuda_major}.{torch_cuda_minor}) torch was compiled with. "
             "The mismatch is found in the minor version. As the APIs are compatible, we will allow compilation to proceed. "
             "If you encounter any issue when using the built kernel, please try to build it again with fully matched CUDA versions"
         )
     return True
@@ -151,23 +152,24 @@
     This function sets the PyTorch TORCH_CUDA_ARCH_LIST variable for ahead-of-time extension compilation.
     Ahead-of-time compilation occurs when CUDA_EXT=1 is set when running 'pip install'.
     """
     cuda_available = check_cuda_availability()
 
     # we only need to set this when CUDA is not available for cross-compilation
     if not cuda_available:
-        warnings.warn('\n[extension]  PyTorch did not find available GPUs on this system.\n'
-                      'If your intention is to cross-compile, this is not an error.\n'
-                      'By default, Colossal-AI will cross-compile for \n'
-                      '1. Pascal (compute capabilities 6.0, 6.1, 6.2),\n'
-                      '2. Volta (compute capability 7.0)\n'
-                      '3. Turing (compute capability 7.5),\n'
-                      '4. Ampere (compute capability 8.0, 8.6)if the CUDA version is >= 11.0\n'
-                      '\nIf you wish to cross-compile for a single specific architecture,\n'
-                      'export TORCH_CUDA_ARCH_LIST="compute capability" before running setup.py.\n')
+        warnings.warn(
+            '\n[extension]  PyTorch did not find available GPUs on this system.\n'
+            'If your intention is to cross-compile, this is not an error.\n'
+            'By default, Colossal-AI will cross-compile for \n'
+            '1. Pascal (compute capabilities 6.0, 6.1, 6.2),\n'
+            '2. Volta (compute capability 7.0)\n'
+            '3. Turing (compute capability 7.5),\n'
+            '4. Ampere (compute capability 8.0, 8.6)if the CUDA version is >= 11.0\n'
+            '\nIf you wish to cross-compile for a single specific architecture,\n'
+            'export TORCH_CUDA_ARCH_LIST="compute capability" before running setup.py.\n')
 
         if os.environ.get("TORCH_CUDA_ARCH_LIST", None) is None:
             bare_metal_major, bare_metal_minor = get_cuda_bare_metal_version(cuda_dir)
 
             arch_list = ['6.0', '6.1', '6.2', '7.0', '7.5']
 
             if int(bare_metal_major) == 11:
```

### Comparing `colossalai-nightly-2023.4.29/setup.py` & `colossalai-nightly-2023.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     if not TORCH_AVAILABLE:
         raise ModuleNotFoundError(
             "[extension] PyTorch is not found while CUDA_EXT=1. You need to install PyTorch first in order to build CUDA extensions"
         )
 
     if not CUDA_HOME:
         raise RuntimeError(
-            "[extension] CUDA_HOME is not found while CUDA_EXT=1. You need to export CUDA_HOME environment variable or install CUDA Toolkit first in order to build CUDA extensions"
+            "[extension] CUDA_HOME is not found while CUDA_EXT=1. You need to export CUDA_HOME environment vairable or install CUDA Toolkit first in order to build CUDA extensions"
         )
 
     check_system_pytorch_cuda_match(CUDA_HOME)
     check_pytorch_version(MIN_PYTORCH_VERSION_MAJOR, MIN_PYTORCH_VERSION_MINOR)
     check_cuda_availability()
```

### Comparing `colossalai-nightly-2023.4.29/tests/components_to_test/albert.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/albert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/components_to_test/beit.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/beit.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/components_to_test/bert.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/components_to_test/gpt2.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/gpt2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/components_to_test/hanging_param_model.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/hanging_param_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/components_to_test/inline_op_model.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/inline_op_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/components_to_test/nested_model.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/nested_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/components_to_test/registry.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/components_to_test/repeated_computed_layers.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/repeated_computed_layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/components_to_test/resnet.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/resnet.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/components_to_test/simple_net.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/simple_net.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/components_to_test/utils/executor.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/utils/executor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 
 
-def run_fwd(model, data, label, criterion) -> torch.Tensor:
-    """run_fwd
-    run fwd for the model
+def run_fwd_bwd(model, data, label, criterion, optimizer=None) -> torch.Tensor:
+    """run_fwd_bwd
+    run fwd and bwd for the model
 
     Args:
         model (torch.nn.Module): a PyTorch model
         data (torch.Tensor): input data
         label (torch.Tensor): label
         criterion (Optional[Callable]): a function of criterion
 
@@ -18,29 +18,12 @@
         y = model(data)
         y = y.float()
         loss = criterion(y, label)
     else:
         loss = model(data, label)
 
     loss = loss.float()
-    return loss
-
-
-def run_fwd_bwd(model, data, label, criterion, optimizer=None) -> torch.Tensor:
-    """run_fwd_bwd
-    run fwd and bwd for the model
-
-    Args:
-        model (torch.nn.Module): a PyTorch model
-        data (torch.Tensor): input data
-        label (torch.Tensor): label
-        criterion (Optional[Callable]): a function of criterion
-
-    Returns:
-        torch.Tensor: loss of fwd
-    """
-    loss = run_fwd(model, data, label, criterion)
     if optimizer:
         optimizer.backward(loss)
     else:
         loss.backward()
     return loss
```

### Comparing `colossalai-nightly-2023.4.29/tests/kit/model_zoo/diffusers/diffusers.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/diffusers/diffusers.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 LATENTS_SHAPE = (BATCH_SIZE, IN_CHANNELS, HEIGHT // 7, WIDTH // 7)
 TIME_STEP = 3
 
 data_vae_fn = lambda: dict(sample=torch.randn(2, 3, 32, 32))
 data_unet_fn = lambda: dict(sample=torch.randn(2, 3, 32, 32), timestep=3)
 
 identity_output = lambda x: x
-clip_vision_model_output = lambda x: dict(pooler_output=x[1])
 
 
 def data_clip_model():
     input_ids = torch.zeros((BATCH_SIZE, SEQ_LENGTH), dtype=torch.int64)
     attention_mask = torch.zeros((BATCH_SIZE, SEQ_LENGTH), dtype=torch.int64)
     position_ids = torch.zeros((BATCH_SIZE, SEQ_LENGTH), dtype=torch.int64)
     pixel_values = torch.zeros((BATCH_SIZE, IN_CHANNELS, HEIGHT, WIDTH), dtype=torch.float32)
@@ -62,13 +61,13 @@
                    model_fn=partial(transformers.CLIPTextModel, config=transformers.CLIPTextConfig()),
                    data_gen_fn=data_clip_text,
                    output_transform_fn=identity_output)
 
 model_zoo.register(name='diffusers_clip_vision_model',
                    model_fn=partial(transformers.CLIPVisionModel, config=transformers.CLIPVisionConfig()),
                    data_gen_fn=data_clip_vision,
-                   output_transform_fn=clip_vision_model_output)
+                   output_transform_fn=identity_output)
 
 model_zoo.register(name='diffusers_unet2d_model',
                    model_fn=diffusers.UNet2DModel,
                    data_gen_fn=data_unet_fn,
                    output_transform_fn=identity_output)
```

### Comparing `colossalai-nightly-2023.4.29/tests/kit/model_zoo/registry.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/kit/model_zoo/timm/timm.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/timm/timm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/kit/model_zoo/torchaudio/torchaudio.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchaudio/torchaudio.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from functools import partial
-
 import torch
 import torchaudio.models as tm
 
 from ..registry import ModelAttribute, model_zoo
 
 INPUT_DIM = 80
 IN_FEATURES = 16
@@ -99,30 +97,32 @@
     mel_specgram_lengths = max_mel_specgram_length * torch.ones((n_batch,))
     return dict(tokens=tokens,
                 token_lengths=token_lengths,
                 mel_specgram=mel_specgram,
                 mel_specgram_lengths=mel_specgram_lengths)
 
 
-model_zoo.register(name='torchaudio_tacotron',
-                   model_fn=lambda: tm.Tacotron2(n_mels=N_MELS),
-                   data_gen_fn=tacotron_data_gen_fn,
-                   output_transform_fn=lambda outputs: dict(summed_output=sum(x.sum() for x in outputs)),
-                   model_attribute=ModelAttribute(has_control_flow=True))
+model_zoo.register(
+    name='torchaudio_tacotron',
+    model_fn=lambda: tm.Tacotron2(n_mels=N_MELS),
+    data_gen_fn=tacotron_data_gen_fn,
+    output_transform_fn=lambda outputs: dict(
+        spectrogram_before=outputs[0], spectrogram_after=outputs[1], stop_tokens=outputs[2], attn_weights=outputs[3]),
+    model_attribute=ModelAttribute(has_control_flow=True))
 
 
 def wav2vec_data_gen_fn():
     batch_size, num_frames = 4, 400
     waveforms = torch.randn(batch_size, num_frames)
     lengths = torch.randint(0, num_frames, (batch_size,))
     return dict(waveforms=waveforms, lengths=lengths)
 
 
 model_zoo.register(name='torchaudio_wav2vec2_base',
-                   model_fn=partial(tm.wav2vec2_base, encoder_layer_drop=0.0),
+                   model_fn=tm.wav2vec2_base,
                    data_gen_fn=wav2vec_data_gen_fn,
                    output_transform_fn=transformer_output_transform_fn,
                    model_attribute=ModelAttribute(has_control_flow=True))
 
 model_zoo.register(name='torchaudio_hubert_base',
                    model_fn=tm.hubert_base,
                    data_gen_fn=wav2vec_data_gen_fn,
```

### Comparing `colossalai-nightly-2023.4.29/tests/kit/model_zoo/torchrec/torchrec.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchrec/torchrec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/kit/model_zoo/torchvision/torchvision.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchvision/torchvision.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,20 @@
         stochastic_depth_prob=0,    # it is originally 0.2, but we set it to 0 to make it deterministic
         weights=weights,
         progress=progress,
     )
 
 
 # special output transform fn
-google_net_output_transform_fn = lambda x: dict(output=sum(x)) if isinstance(x, torchvision.models.GoogLeNetOutputs
-                                                                            ) else dict(output=x)
+google_net_output_transform_fn = lambda x: dict(output=x.logits) if isinstance(x, torchvision.models.GoogLeNetOutputs
+                                                                              ) else dict(output=x)
 swin_s_output_output_transform_fn = lambda x: {f'output{idx}': val
                                                for idx, val in enumerate(x)} if isinstance(x, tuple) else dict(output=x)
-inception_v3_output_transform_fn = lambda x: dict(output=sum(x)) if isinstance(x, torchvision.models.InceptionOutputs
-                                                                              ) else dict(output=x)
+inception_v3_output_transform_fn = lambda x: dict(output=x.logits) if isinstance(x, torchvision.models.InceptionOutputs
+                                                                                ) else dict(output=x)
 
 model_zoo.register(name='torchvision_alexnet',
                    model_fn=tm.alexnet,
                    data_gen_fn=data_gen_fn,
                    output_transform_fn=output_transform_fn)
 model_zoo.register(name='torchvision_densenet121',
                    model_fn=tm.densenet121,
```

### Comparing `colossalai-nightly-2023.4.29/tests/kit/model_zoo/transformers/albert.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/albert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/kit/model_zoo/transformers/bert.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/kit/model_zoo/transformers/gpt.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/gpt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/kit/model_zoo/transformers/opt.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/opt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/kit/model_zoo/transformers/t5.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/t5.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_analyzer/test_fx/test_bias_addition.py` & `colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_bias_addition.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_analyzer/test_fx/test_mod_dir.py` & `colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_mod_dir.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_analyzer/test_fx/test_nested_ckpt.py` & `colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_nested_ckpt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_analyzer/test_fx/test_shape_prop.py` & `colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_shape_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_analyzer/test_fx/test_symbolic_profile.py` & `colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_symbolic_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_analyzer/test_fx/zoo.py` & `colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/zoo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_analyzer/test_subclasses/test_aten.py` & `colossalai-nightly-2023.4.8/tests/test_analyzer/test_subclasses/test_aten.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_analyzer/test_subclasses/test_flop_tensor.py` & `colossalai-nightly-2023.4.8/tests/test_analyzer/test_subclasses/test_flop_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_analyzer/test_subclasses/test_meta_mode.py` & `colossalai-nightly-2023.4.8/tests/test_analyzer/test_subclasses/test_meta_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_pass/test_node_converting_pass.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_pass/test_node_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.29/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py`

 * *Files identical despite different names*


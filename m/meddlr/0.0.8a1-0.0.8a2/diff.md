# Comparing `tmp/meddlr-0.0.8a1.tar.gz` & `tmp/meddlr-0.0.8a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meddlr-0.0.8a1.tar", last modified: Sat Apr 29 19:47:16 2023, max compression
+gzip compressed data, was "meddlr-0.0.8a2.tar", last modified: Sat Apr 29 20:22:37 2023, max compression
```

## Comparing `meddlr-0.0.8a1.tar` & `meddlr-0.0.8a2.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.222715 meddlr-0.0.8a1/
--rw-r--r--   0 arjundd    (501) staff       (20)    11357 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/LICENSE
--rw-r--r--   0 arjundd    (501) staff       (20)     3974 2023-04-29 19:47:16.222805 meddlr-0.0.8a1/PKG-INFO
--rw-r--r--   0 arjundd    (501) staff       (20)     3265 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/README.md
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.202243 meddlr-0.0.8a1/meddlr/
--rw-r--r--   0 arjundd    (501) staff       (20)      299 2023-04-29 19:38:28.000000 meddlr-0.0.8a1/meddlr/__init__.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.203237 meddlr-0.0.8a1/meddlr/checkpoint/
--rw-r--r--   0 arjundd    (501) staff       (20)      165 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/checkpoint/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)     1919 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/checkpoint/checkpoint.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.204089 meddlr-0.0.8a1/meddlr/config/
--rw-r--r--   0 arjundd    (501) staff       (20)       67 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/config/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)     4798 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/config/compat.py
--rw-r--r--   0 arjundd    (501) staff       (20)    14082 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/config/config.py
--rw-r--r--   0 arjundd    (501) staff       (20)    17235 2023-04-29 17:00:34.000000 meddlr-0.0.8a1/meddlr/config/defaults.py
--rw-r--r--   0 arjundd    (501) staff       (20)     4952 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/config/util.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.205035 meddlr-0.0.8a1/meddlr/data/
--rw-r--r--   0 arjundd    (501) staff       (20)      587 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)    13160 2023-04-29 16:30:43.000000 meddlr-0.0.8a1/meddlr/data/build.py
--rw-r--r--   0 arjundd    (501) staff       (20)     8987 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/catalog.py
--rw-r--r--   0 arjundd    (501) staff       (20)     1798 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/collate.py
--rw-r--r--   0 arjundd    (501) staff       (20)    10789 2023-04-29 16:30:52.000000 meddlr-0.0.8a1/meddlr/data/data_utils.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.205499 meddlr-0.0.8a1/meddlr/data/datasets/
--rw-r--r--   0 arjundd    (501) staff       (20)       75 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/datasets/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)     5955 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/datasets/builtin.py
--rw-r--r--   0 arjundd    (501) staff       (20)     4444 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/datasets/register_mrco.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.206433 meddlr-0.0.8a1/meddlr/data/samplers/
--rw-r--r--   0 arjundd    (501) staff       (20)      484 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/samplers/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)     3643 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/samplers/build.py
--rw-r--r--   0 arjundd    (501) staff       (20)    17837 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/samplers/group_sampler.py
--rw-r--r--   0 arjundd    (501) staff       (20)     4895 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/samplers/sampler.py
--rw-r--r--   0 arjundd    (501) staff       (20)     8201 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/slice_dataset.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.207449 meddlr-0.0.8a1/meddlr/data/transforms/
--rw-r--r--   0 arjundd    (501) staff       (20)        0 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/transforms/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)     5329 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/transforms/motion.py
--rw-r--r--   0 arjundd    (501) staff       (20)     6014 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/transforms/noise.py
--rw-r--r--   0 arjundd    (501) staff       (20)     5097 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/transforms/noiseandmotion.py
--rw-r--r--   0 arjundd    (501) staff       (20)    27768 2023-04-29 17:00:34.000000 meddlr-0.0.8a1/meddlr/data/transforms/subsample.py
--rw-r--r--   0 arjundd    (501) staff       (20)    15104 2023-04-29 17:00:34.000000 meddlr-0.0.8a1/meddlr/data/transforms/transform.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.208622 meddlr-0.0.8a1/meddlr/engine/
--rw-r--r--   0 arjundd    (501) staff       (20)      322 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/engine/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)    12982 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/engine/defaults.py
--rw-r--r--   0 arjundd    (501) staff       (20)    13868 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/engine/hooks.py
--rw-r--r--   0 arjundd    (501) staff       (20)     7667 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/engine/model_zoo.py
--rw-r--r--   0 arjundd    (501) staff       (20)     3211 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/engine/sharing.py
--rw-r--r--   0 arjundd    (501) staff       (20)     9387 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/engine/train_loop.py
--rw-r--r--   0 arjundd    (501) staff       (20)    17806 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/engine/trainer.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.209485 meddlr-0.0.8a1/meddlr/evaluation/
--rw-r--r--   0 arjundd    (501) staff       (20)      255 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/evaluation/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)     7703 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/evaluation/evaluator.py
--rw-r--r--   0 arjundd    (501) staff       (20)    18528 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/evaluation/recon_evaluation.py
--rw-r--r--   0 arjundd    (501) staff       (20)     5068 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/evaluation/scan_evaluator.py
--rw-r--r--   0 arjundd    (501) staff       (20)    12615 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/evaluation/seg_evaluation.py
--rw-r--r--   0 arjundd    (501) staff       (20)    16054 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/evaluation/testing.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.209759 meddlr-0.0.8a1/meddlr/forward/
--rw-r--r--   0 arjundd    (501) staff       (20)      129 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/forward/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)     5165 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/forward/mri.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.211874 meddlr-0.0.8a1/meddlr/metrics/
--rw-r--r--   0 arjundd    (501) staff       (20)      477 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/metrics/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)     4417 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/metrics/build.py
--rw-r--r--   0 arjundd    (501) staff       (20)     3042 2023-04-29 16:30:52.000000 meddlr-0.0.8a1/meddlr/metrics/collection.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.212410 meddlr-0.0.8a1/meddlr/metrics/functional/
--rw-r--r--   0 arjundd    (501) staff       (20)      444 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/metrics/functional/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)    15595 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/metrics/functional/image.py
--rw-r--r--   0 arjundd    (501) staff       (20)     5787 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/metrics/functional/sem_seg.py
--rw-r--r--   0 arjundd    (501) staff       (20)     5516 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/metrics/functional/util.py
--rw-r--r--   0 arjundd    (501) staff       (20)    18811 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/metrics/image.py
--rw-r--r--   0 arjundd    (501) staff       (20)     6703 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/metrics/lpip.py
--rw-r--r--   0 arjundd    (501) staff       (20)     8386 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/metrics/metric.py
--rw-r--r--   0 arjundd    (501) staff       (20)     4596 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/metrics/sem_seg.py
--rw-r--r--   0 arjundd    (501) staff       (20)     9571 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/metrics/ssfd.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.212669 meddlr-0.0.8a1/meddlr/modeling/
--rw-r--r--   0 arjundd    (501) staff       (20)      465 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/__init__.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.213118 meddlr-0.0.8a1/meddlr/modeling/blocks/
--rw-r--r--   0 arjundd    (501) staff       (20)      450 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/blocks/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)     6008 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/blocks/conv_blocks.py
--rw-r--r--   0 arjundd    (501) staff       (20)     8180 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/blocks/fuse_blocks.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.213921 meddlr-0.0.8a1/meddlr/modeling/layers/
--rw-r--r--   0 arjundd    (501) staff       (20)      425 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/layers/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)     8557 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/layers/build.py
--rw-r--r--   0 arjundd    (501) staff       (20)     2701 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/layers/conv.py
--rw-r--r--   0 arjundd    (501) staff       (20)     5125 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/layers/gauss.py
--rw-r--r--   0 arjundd    (501) staff       (20)     7428 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/layers/layers2D.py
--rw-r--r--   0 arjundd    (501) staff       (20)     6937 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/layers/layers3D.py
--rw-r--r--   0 arjundd    (501) staff       (20)    13152 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/modeling/loss_computer.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.215720 meddlr-0.0.8a1/meddlr/modeling/meta_arch/
--rw-r--r--   0 arjundd    (501) staff       (20)      565 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)     9129 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/build.py
--rw-r--r--   0 arjundd    (501) staff       (20)     6532 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/cs_model.py
--rw-r--r--   0 arjundd    (501) staff       (20)     7992 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/denoising.py
--rw-r--r--   0 arjundd    (501) staff       (20)     8167 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/generalized_unet.py
--rw-r--r--   0 arjundd    (501) staff       (20)     7288 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/m2r.py
--rw-r--r--   0 arjundd    (501) staff       (20)     9988 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/n2r.py
--rw-r--r--   0 arjundd    (501) staff       (20)     7797 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/nm2r.py
--rw-r--r--   0 arjundd    (501) staff       (20)     9721 2023-04-29 17:00:34.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/ssdu.py
--rw-r--r--   0 arjundd    (501) staff       (20)    14800 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/unet.py
--rw-r--r--   0 arjundd    (501) staff       (20)    17035 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/unrolled.py
--rw-r--r--   0 arjundd    (501) staff       (20)     8649 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/vortex.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.216561 meddlr-0.0.8a1/meddlr/ops/
--rw-r--r--   0 arjundd    (501) staff       (20)      814 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/ops/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)     5436 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/ops/categorical.py
--rw-r--r--   0 arjundd    (501) staff       (20)    12676 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/ops/complex.py
--rw-r--r--   0 arjundd    (501) staff       (20)    11052 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/ops/fft.py
--rw-r--r--   0 arjundd    (501) staff       (20)     1925 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/ops/opt.py
--rw-r--r--   0 arjundd    (501) staff       (20)     5686 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/ops/utils.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.217075 meddlr-0.0.8a1/meddlr/solver/
--rw-r--r--   0 arjundd    (501) staff       (20)      265 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/solver/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)     3526 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/solver/build.py
--rw-r--r--   0 arjundd    (501) staff       (20)     4442 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/solver/lr_scheduler.py
--rw-r--r--   0 arjundd    (501) staff       (20)     2125 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/solver/optimizer.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.217953 meddlr-0.0.8a1/meddlr/transforms/
--rw-r--r--   0 arjundd    (501) staff       (20)      263 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/__init__.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.218815 meddlr-0.0.8a1/meddlr/transforms/base/
--rw-r--r--   0 arjundd    (501) staff       (20)      342 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/base/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)    12049 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/base/mask.py
--rw-r--r--   0 arjundd    (501) staff       (20)     2888 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/transforms/base/motion.py
--rw-r--r--   0 arjundd    (501) staff       (20)     4286 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/base/noise.py
--rw-r--r--   0 arjundd    (501) staff       (20)     8862 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/base/spatial.py
--rw-r--r--   0 arjundd    (501) staff       (20)     4368 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/build.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.219073 meddlr-0.0.8a1/meddlr/transforms/builtin/
--rw-r--r--   0 arjundd    (501) staff       (20)        0 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/builtin/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)    14993 2023-04-29 17:00:34.000000 meddlr-0.0.8a1/meddlr/transforms/builtin/mri.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.219342 meddlr-0.0.8a1/meddlr/transforms/functional/
--rw-r--r--   0 arjundd    (501) staff       (20)       73 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/transforms/functional/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)     1209 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/transforms/functional/mri.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.220166 meddlr-0.0.8a1/meddlr/transforms/gen/
--rw-r--r--   0 arjundd    (501) staff       (20)      388 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/transforms/gen/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)     2959 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/gen/choice.py
--rw-r--r--   0 arjundd    (501) staff       (20)     1864 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/gen/mask.py
--rw-r--r--   0 arjundd    (501) staff       (20)     2318 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/transforms/gen/motion.py
--rw-r--r--   0 arjundd    (501) staff       (20)     1695 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/gen/noise.py
--rw-r--r--   0 arjundd    (501) staff       (20)     6908 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/gen/spatial.py
--rw-r--r--   0 arjundd    (501) staff       (20)      517 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/mixins.py
--rw-r--r--   0 arjundd    (501) staff       (20)       84 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/param_kind.py
--rw-r--r--   0 arjundd    (501) staff       (20)    18373 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/tf_scheduler.py
--rw-r--r--   0 arjundd    (501) staff       (20)     9527 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/transforms/transform.py
--rw-r--r--   0 arjundd    (501) staff       (20)     6841 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/transforms/transform_gen.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.222303 meddlr-0.0.8a1/meddlr/utils/
--rw-r--r--   0 arjundd    (501) staff       (20)       69 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)     1635 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/cfl.py
--rw-r--r--   0 arjundd    (501) staff       (20)     9549 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/cluster.py
--rw-r--r--   0 arjundd    (501) staff       (20)     3896 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/collect_env.py
--rw-r--r--   0 arjundd    (501) staff       (20)     8855 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/comm.py
--rw-r--r--   0 arjundd    (501) staff       (20)     1482 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/deprecated.py
--rw-r--r--   0 arjundd    (501) staff       (20)    12224 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/env.py
--rw-r--r--   0 arjundd    (501) staff       (20)    14904 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/events.py
--rw-r--r--   0 arjundd    (501) staff       (20)     3302 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/general.py
--rw-r--r--   0 arjundd    (501) staff       (20)     7553 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/logger.py
--rw-r--r--   0 arjundd    (501) staff       (20)     2600 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/memory.py
--rw-r--r--   0 arjundd    (501) staff       (20)    19597 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/path.py
--rw-r--r--   0 arjundd    (501) staff       (20)     2806 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/profiler.py
--rw-r--r--   0 arjundd    (501) staff       (20)     2622 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/registry.py
--rw-r--r--   0 arjundd    (501) staff       (20)    10657 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/transforms.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.202968 meddlr-0.0.8a1/meddlr.egg-info/
--rw-r--r--   0 arjundd    (501) staff       (20)     3974 2023-04-29 19:47:16.000000 meddlr-0.0.8a1/meddlr.egg-info/PKG-INFO
--rw-r--r--   0 arjundd    (501) staff       (20)     3949 2023-04-29 19:47:16.000000 meddlr-0.0.8a1/meddlr.egg-info/SOURCES.txt
--rw-r--r--   0 arjundd    (501) staff       (20)        1 2023-04-29 19:47:16.000000 meddlr-0.0.8a1/meddlr.egg-info/dependency_links.txt
--rw-r--r--   0 arjundd    (501) staff       (20)      867 2023-04-29 19:47:16.000000 meddlr-0.0.8a1/meddlr.egg-info/requires.txt
--rw-r--r--   0 arjundd    (501) staff       (20)        7 2023-04-29 19:47:16.000000 meddlr-0.0.8a1/meddlr.egg-info/top_level.txt
--rw-r--r--   0 arjundd    (501) staff       (20)       73 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/pyproject.toml
--rw-r--r--   0 arjundd    (501) staff       (20)      559 2023-04-29 19:47:16.223137 meddlr-0.0.8a1/setup.cfg
--rw-r--r--   0 arjundd    (501) staff       (20)     8059 2023-04-29 19:47:10.000000 meddlr-0.0.8a1/setup.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.222574 meddlr-0.0.8a1/tests/
--rw-r--r--   0 arjundd    (501) staff       (20)     3021 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/tests/test_experiments.py
--rw-r--r--   0 arjundd    (501) staff       (20)     1670 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/tests/test_reproducibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.637338 meddlr-0.0.8a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-29 20:22:37.637338 meddlr-0.0.8a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.585338 meddlr-0.0.8a2/meddlr/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.585338 meddlr-0.0.8a2/meddlr/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/checkpoint/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.589338 meddlr-0.0.8a2/meddlr/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/config/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14082 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17235 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/config/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.593338 meddlr-0.0.8a2/meddlr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13160 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/data_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.593338 meddlr-0.0.8a2/meddlr/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/datasets/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/datasets/register_mrco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.597338 meddlr-0.0.8a2/meddlr/data/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/samplers/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17837 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/samplers/group_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/samplers/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/slice_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.601338 meddlr-0.0.8a2/meddlr/data/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/transforms/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/transforms/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/transforms/noiseandmotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27768 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/transforms/subsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/transforms/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.605338 meddlr-0.0.8a2/meddlr/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/engine/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13868 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/engine/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/engine/model_zoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/engine/sharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/engine/train_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17806 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/engine/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.605338 meddlr-0.0.8a2/meddlr/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/evaluation/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18528 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/evaluation/recon_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/evaluation/scan_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/evaluation/seg_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16054 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/evaluation/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.609338 meddlr-0.0.8a2/meddlr/forward/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/forward/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/forward/mri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.609338 meddlr-0.0.8a2/meddlr/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.613338 meddlr-0.0.8a2/meddlr/metrics/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15595 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/functional/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/functional/sem_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/functional/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/lpip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/sem_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/ssfd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.613338 meddlr-0.0.8a2/meddlr/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.613338 meddlr-0.0.8a2/meddlr/modeling/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/blocks/conv_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/blocks/fuse_blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.617338 meddlr-0.0.8a2/meddlr/modeling/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/layers/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/layers/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/layers/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/layers/layers2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/layers/layers3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/loss_computer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.621338 meddlr-0.0.8a2/meddlr/modeling/meta_arch/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/cs_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/denoising.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/generalized_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/m2r.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/n2r.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/nm2r.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/ssdu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17035 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/unrolled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8649 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/vortex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.625338 meddlr-0.0.8a2/meddlr/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/ops/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/ops/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/ops/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/ops/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/ops/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.625338 meddlr-0.0.8a2/meddlr/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/solver/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/solver/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/solver/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.629338 meddlr-0.0.8a2/meddlr/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.629338 meddlr-0.0.8a2/meddlr/transforms/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/base/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/base/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/base/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/base/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.629338 meddlr-0.0.8a2/meddlr/transforms/builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/builtin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14993 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/builtin/mri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.629338 meddlr-0.0.8a2/meddlr/transforms/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/functional/mri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.633339 meddlr-0.0.8a2/meddlr/transforms/gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/gen/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/gen/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/gen/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/gen/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/gen/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/param_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/tf_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/transform_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.637338 meddlr-0.0.8a2/meddlr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/cfl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/comm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14904 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19597 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.585338 meddlr-0.0.8a2/meddlr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-29 20:22:37.000000 meddlr-0.0.8a2/meddlr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-29 20:22:37.000000 meddlr-0.0.8a2/meddlr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 20:22:37.000000 meddlr-0.0.8a2/meddlr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-29 20:22:37.000000 meddlr-0.0.8a2/meddlr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 20:22:37.000000 meddlr-0.0.8a2/meddlr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-29 20:22:37.637338 meddlr-0.0.8a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.637338 meddlr-0.0.8a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/tests/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/tests/test_reproducibility.py
```

### Comparing `meddlr-0.0.8a1/LICENSE` & `meddlr-0.0.8a2/LICENSE`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/PKG-INFO` & `meddlr-0.0.8a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meddlr
-Version: 0.0.8a1
+Version: 0.0.8a2
 Summary: Meddlr is a config-driven framework built to simplify ML-based medical image reconstruction and analysis.
 Home-page: https://github.com/ad12/meddlr
 Author: The Meddlr Team
 Author-email: arjundd@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `meddlr-0.0.8a1/README.md` & `meddlr-0.0.8a2/README.md`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/checkpoint/checkpoint.py` & `meddlr-0.0.8a2/meddlr/checkpoint/checkpoint.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/config/compat.py` & `meddlr-0.0.8a2/meddlr/config/compat.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/config/config.py` & `meddlr-0.0.8a2/meddlr/config/config.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/config/defaults.py` & `meddlr-0.0.8a2/meddlr/config/defaults.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/config/util.py` & `meddlr-0.0.8a2/meddlr/config/util.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/data/__init__.py` & `meddlr-0.0.8a2/meddlr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/data/build.py` & `meddlr-0.0.8a2/meddlr/data/build.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/data/catalog.py` & `meddlr-0.0.8a2/meddlr/data/catalog.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/data/collate.py` & `meddlr-0.0.8a2/meddlr/data/collate.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/data/data_utils.py` & `meddlr-0.0.8a2/meddlr/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/data/datasets/builtin.py` & `meddlr-0.0.8a2/meddlr/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/data/datasets/register_mrco.py` & `meddlr-0.0.8a2/meddlr/data/datasets/register_mrco.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/data/samplers/build.py` & `meddlr-0.0.8a2/meddlr/data/samplers/build.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/data/samplers/group_sampler.py` & `meddlr-0.0.8a2/meddlr/data/samplers/group_sampler.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/data/samplers/sampler.py` & `meddlr-0.0.8a2/meddlr/data/samplers/sampler.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/data/slice_dataset.py` & `meddlr-0.0.8a2/meddlr/data/slice_dataset.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/data/transforms/motion.py` & `meddlr-0.0.8a2/meddlr/data/transforms/motion.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/data/transforms/noise.py` & `meddlr-0.0.8a2/meddlr/data/transforms/noise.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/data/transforms/noiseandmotion.py` & `meddlr-0.0.8a2/meddlr/data/transforms/noiseandmotion.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/data/transforms/subsample.py` & `meddlr-0.0.8a2/meddlr/data/transforms/subsample.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/data/transforms/transform.py` & `meddlr-0.0.8a2/meddlr/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/engine/defaults.py` & `meddlr-0.0.8a2/meddlr/engine/defaults.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/engine/hooks.py` & `meddlr-0.0.8a2/meddlr/engine/hooks.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/engine/model_zoo.py` & `meddlr-0.0.8a2/meddlr/engine/model_zoo.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/engine/sharing.py` & `meddlr-0.0.8a2/meddlr/engine/sharing.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/engine/train_loop.py` & `meddlr-0.0.8a2/meddlr/engine/train_loop.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/engine/trainer.py` & `meddlr-0.0.8a2/meddlr/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/evaluation/evaluator.py` & `meddlr-0.0.8a2/meddlr/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/evaluation/recon_evaluation.py` & `meddlr-0.0.8a2/meddlr/evaluation/recon_evaluation.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/evaluation/scan_evaluator.py` & `meddlr-0.0.8a2/meddlr/evaluation/scan_evaluator.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/evaluation/seg_evaluation.py` & `meddlr-0.0.8a2/meddlr/evaluation/seg_evaluation.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/evaluation/testing.py` & `meddlr-0.0.8a2/meddlr/evaluation/testing.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/forward/mri.py` & `meddlr-0.0.8a2/meddlr/forward/mri.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/metrics/build.py` & `meddlr-0.0.8a2/meddlr/metrics/build.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/metrics/collection.py` & `meddlr-0.0.8a2/meddlr/metrics/collection.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/metrics/functional/image.py` & `meddlr-0.0.8a2/meddlr/metrics/functional/image.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/metrics/functional/sem_seg.py` & `meddlr-0.0.8a2/meddlr/metrics/functional/sem_seg.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/metrics/functional/util.py` & `meddlr-0.0.8a2/meddlr/metrics/functional/util.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/metrics/image.py` & `meddlr-0.0.8a2/meddlr/metrics/image.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/metrics/lpip.py` & `meddlr-0.0.8a2/meddlr/metrics/lpip.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/metrics/metric.py` & `meddlr-0.0.8a2/meddlr/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/metrics/sem_seg.py` & `meddlr-0.0.8a2/meddlr/metrics/sem_seg.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/metrics/ssfd.py` & `meddlr-0.0.8a2/meddlr/metrics/ssfd.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/blocks/conv_blocks.py` & `meddlr-0.0.8a2/meddlr/modeling/blocks/conv_blocks.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/blocks/fuse_blocks.py` & `meddlr-0.0.8a2/meddlr/modeling/blocks/fuse_blocks.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/layers/build.py` & `meddlr-0.0.8a2/meddlr/modeling/layers/build.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/layers/conv.py` & `meddlr-0.0.8a2/meddlr/modeling/layers/conv.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/layers/gauss.py` & `meddlr-0.0.8a2/meddlr/modeling/layers/gauss.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/layers/layers2D.py` & `meddlr-0.0.8a2/meddlr/modeling/layers/layers2D.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/layers/layers3D.py` & `meddlr-0.0.8a2/meddlr/modeling/layers/layers3D.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/loss_computer.py` & `meddlr-0.0.8a2/meddlr/modeling/loss_computer.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/meta_arch/__init__.py` & `meddlr-0.0.8a2/meddlr/modeling/meta_arch/__init__.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/meta_arch/build.py` & `meddlr-0.0.8a2/meddlr/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/meta_arch/cs_model.py` & `meddlr-0.0.8a2/meddlr/modeling/meta_arch/cs_model.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/meta_arch/denoising.py` & `meddlr-0.0.8a2/meddlr/modeling/meta_arch/denoising.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/meta_arch/generalized_unet.py` & `meddlr-0.0.8a2/meddlr/modeling/meta_arch/generalized_unet.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/meta_arch/m2r.py` & `meddlr-0.0.8a2/meddlr/modeling/meta_arch/m2r.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/meta_arch/n2r.py` & `meddlr-0.0.8a2/meddlr/modeling/meta_arch/n2r.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/meta_arch/nm2r.py` & `meddlr-0.0.8a2/meddlr/modeling/meta_arch/nm2r.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/meta_arch/ssdu.py` & `meddlr-0.0.8a2/meddlr/modeling/meta_arch/ssdu.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/meta_arch/unet.py` & `meddlr-0.0.8a2/meddlr/modeling/meta_arch/unet.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/meta_arch/unrolled.py` & `meddlr-0.0.8a2/meddlr/modeling/meta_arch/unrolled.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/modeling/meta_arch/vortex.py` & `meddlr-0.0.8a2/meddlr/modeling/meta_arch/vortex.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/ops/__init__.py` & `meddlr-0.0.8a2/meddlr/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/ops/categorical.py` & `meddlr-0.0.8a2/meddlr/ops/categorical.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/ops/complex.py` & `meddlr-0.0.8a2/meddlr/ops/complex.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/ops/fft.py` & `meddlr-0.0.8a2/meddlr/ops/fft.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/ops/opt.py` & `meddlr-0.0.8a2/meddlr/ops/opt.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/ops/utils.py` & `meddlr-0.0.8a2/meddlr/ops/utils.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/solver/build.py` & `meddlr-0.0.8a2/meddlr/solver/build.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/solver/lr_scheduler.py` & `meddlr-0.0.8a2/meddlr/solver/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/solver/optimizer.py` & `meddlr-0.0.8a2/meddlr/solver/optimizer.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/transforms/base/mask.py` & `meddlr-0.0.8a2/meddlr/transforms/base/mask.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/transforms/base/motion.py` & `meddlr-0.0.8a2/meddlr/transforms/base/motion.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/transforms/base/noise.py` & `meddlr-0.0.8a2/meddlr/transforms/base/noise.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/transforms/base/spatial.py` & `meddlr-0.0.8a2/meddlr/transforms/base/spatial.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/transforms/build.py` & `meddlr-0.0.8a2/meddlr/transforms/build.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/transforms/builtin/mri.py` & `meddlr-0.0.8a2/meddlr/transforms/builtin/mri.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/transforms/functional/mri.py` & `meddlr-0.0.8a2/meddlr/transforms/functional/mri.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/transforms/gen/choice.py` & `meddlr-0.0.8a2/meddlr/transforms/gen/choice.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/transforms/gen/mask.py` & `meddlr-0.0.8a2/meddlr/transforms/gen/mask.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/transforms/gen/motion.py` & `meddlr-0.0.8a2/meddlr/transforms/gen/motion.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/transforms/gen/noise.py` & `meddlr-0.0.8a2/meddlr/transforms/gen/noise.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/transforms/gen/spatial.py` & `meddlr-0.0.8a2/meddlr/transforms/gen/spatial.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/transforms/mixins.py` & `meddlr-0.0.8a2/meddlr/transforms/mixins.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/transforms/tf_scheduler.py` & `meddlr-0.0.8a2/meddlr/transforms/tf_scheduler.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/transforms/transform.py` & `meddlr-0.0.8a2/meddlr/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/transforms/transform_gen.py` & `meddlr-0.0.8a2/meddlr/transforms/transform_gen.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/utils/cfl.py` & `meddlr-0.0.8a2/meddlr/utils/cfl.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/utils/cluster.py` & `meddlr-0.0.8a2/meddlr/utils/cluster.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/utils/collect_env.py` & `meddlr-0.0.8a2/meddlr/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/utils/comm.py` & `meddlr-0.0.8a2/meddlr/utils/comm.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/utils/deprecated.py` & `meddlr-0.0.8a2/meddlr/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/utils/env.py` & `meddlr-0.0.8a2/meddlr/utils/env.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/utils/events.py` & `meddlr-0.0.8a2/meddlr/utils/events.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/utils/general.py` & `meddlr-0.0.8a2/meddlr/utils/general.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/utils/logger.py` & `meddlr-0.0.8a2/meddlr/utils/logger.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/utils/memory.py` & `meddlr-0.0.8a2/meddlr/utils/memory.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/utils/path.py` & `meddlr-0.0.8a2/meddlr/utils/path.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/utils/profiler.py` & `meddlr-0.0.8a2/meddlr/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/utils/registry.py` & `meddlr-0.0.8a2/meddlr/utils/registry.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr/utils/transforms.py` & `meddlr-0.0.8a2/meddlr/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr.egg-info/PKG-INFO` & `meddlr-0.0.8a2/meddlr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meddlr
-Version: 0.0.8a1
+Version: 0.0.8a2
 Summary: Meddlr is a config-driven framework built to simplify ML-based medical image reconstruction and analysis.
 Home-page: https://github.com/ad12/meddlr
 Author: The Meddlr Team
 Author-email: arjundd@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `meddlr-0.0.8a1/meddlr.egg-info/SOURCES.txt` & `meddlr-0.0.8a2/meddlr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/meddlr.egg-info/requires.txt` & `meddlr-0.0.8a2/meddlr.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -13,45 +13,45 @@
 tqdm
 omegaconf
 torchmetrics>=0.5.1
 iopath
 packaging
 
 [all]
+monai
+lpips
 medpy
-requests
 gdown<4.6.0
-lpips
-monai
 iocursor
+requests
 
 [alldev]
-medpy
-parameterized
-monai
-sphinx-rtd-theme
-m2r2
-black==22.12.0
-pooch
 flake8-bugbear
-pre-commit>=2.9.3
-coverage
-wrapt
+lpips
+sphinx-rtd-theme
 sphinxcontrib-bibtex
-sphinxcontrib.bibtex
+pooch
 flake8
-gdown<4.6.0
 requests
-lpips
 tifffile<=2022.5.4
+coverage
+medpy
+wrapt
 flake8-comprehensions
-sphinx
-iocursor
 pytest
+gdown<4.6.0
+sphinx
+sphinxcontrib.bibtex
 isort
+parameterized
+pre-commit>=2.9.3
+black==22.12.0
+monai
+m2r2
+iocursor
 
 [benchmarking]
 medpy
 
 [deployment]
 gdown<4.6.0
 requests
```

### Comparing `meddlr-0.0.8a1/setup.cfg` & `meddlr-0.0.8a2/setup.cfg`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/setup.py` & `meddlr-0.0.8a2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import subprocess
 import sys
 from os import path
 from shutil import rmtree
 
-from packaging import version
 from setuptools import Command, find_packages, setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 _INIT_FILE = path.join(path.abspath(path.dirname(__file__)), "meddlr", "__init__.py")
 
 
 class UploadCommand(Command):
@@ -67,14 +66,18 @@
         """Prints things in bold."""
         print("\033[1m{0}\033[0m".format(s))
 
     def initialize_options(self):
         self.version = None
 
     def finalize_options(self):
+        # This package cannot be imported at top level because it
+        # is not recognized by Github Actions.
+        from packaging import version
+
         if self.version is None:
             raise ValueError("Please specify a version number.")
 
         current_version = get_version()
         if not version.Version(self.version) > version.Version(current_version):
             raise ValueError(
                 f"New version ({self.version}) must be greater than "
```

### Comparing `meddlr-0.0.8a1/tests/test_experiments.py` & `meddlr-0.0.8a2/tests/test_experiments.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a1/tests/test_reproducibility.py` & `meddlr-0.0.8a2/tests/test_reproducibility.py`

 * *Files identical despite different names*


# Comparing `tmp/meddlr-0.0.7rc1.tar.gz` & `tmp/meddlr-0.0.8a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meddlr-0.0.7rc1.tar", last modified: Wed Dec  7 06:29:10 2022, max compression
+gzip compressed data, was "meddlr-0.0.8a1.tar", last modified: Sat Apr 29 19:47:16 2023, max compression
```

## Comparing `meddlr-0.0.7rc1.tar` & `meddlr-0.0.8a1.tar`

### file list

```diff
@@ -1,160 +1,164 @@
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:10.141643 meddlr-0.0.7rc1/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    11357 2022-08-04 01:44:08.000000 meddlr-0.0.7rc1/LICENSE
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     4012 2022-12-07 06:29:10.142643 meddlr-0.0.7rc1/PKG-INFO
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     3265 2022-08-04 01:44:08.000000 meddlr-0.0.7rc1/README.md
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:09.903643 meddlr-0.0.7rc1/meddlr/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      300 2022-12-07 06:28:17.000000 meddlr-0.0.7rc1/meddlr/__init__.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:09.915643 meddlr-0.0.7rc1/meddlr/checkpoint/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      165 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/checkpoint/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     1919 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/checkpoint/checkpoint.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:09.925643 meddlr-0.0.7rc1/meddlr/config/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)       67 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/config/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     4798 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/config/compat.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    14082 2022-12-05 21:57:19.000000 meddlr-0.0.7rc1/meddlr/config/config.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    17059 2022-12-05 17:30:24.000000 meddlr-0.0.7rc1/meddlr/config/defaults.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     4952 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/config/util.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:09.936643 meddlr-0.0.7rc1/meddlr/data/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      587 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/data/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    12976 2022-11-15 16:24:30.000000 meddlr-0.0.7rc1/meddlr/data/build.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     8987 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/data/catalog.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     1798 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/data/collate.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    10790 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/data/data_utils.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:09.942643 meddlr-0.0.7rc1/meddlr/data/datasets/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)       75 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/data/datasets/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     5955 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/data/datasets/builtin.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     4444 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/data/datasets/register_mrco.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:09.949643 meddlr-0.0.7rc1/meddlr/data/samplers/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      484 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/data/samplers/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     3643 2022-10-21 17:37:55.000000 meddlr-0.0.7rc1/meddlr/data/samplers/build.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    17837 2022-10-21 17:37:55.000000 meddlr-0.0.7rc1/meddlr/data/samplers/group_sampler.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     4895 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/data/samplers/sampler.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     8201 2022-10-30 16:15:02.000000 meddlr-0.0.7rc1/meddlr/data/slice_dataset.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:09.961643 meddlr-0.0.7rc1/meddlr/data/transforms/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)        0 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/data/transforms/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     5329 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/data/transforms/motion.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     6014 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/data/transforms/noise.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     5097 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/data/transforms/noiseandmotion.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    23865 2022-12-07 01:31:05.000000 meddlr-0.0.7rc1/meddlr/data/transforms/subsample.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    15144 2022-11-08 22:25:14.000000 meddlr-0.0.7rc1/meddlr/data/transforms/transform.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:09.973643 meddlr-0.0.7rc1/meddlr/engine/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      322 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/engine/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    12982 2022-10-30 16:37:34.000000 meddlr-0.0.7rc1/meddlr/engine/defaults.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    13868 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/engine/hooks.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     7667 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/engine/model_zoo.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     3211 2022-12-07 01:31:05.000000 meddlr-0.0.7rc1/meddlr/engine/sharing.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     9387 2022-11-08 22:25:14.000000 meddlr-0.0.7rc1/meddlr/engine/train_loop.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    17806 2022-12-07 01:31:05.000000 meddlr-0.0.7rc1/meddlr/engine/trainer.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:09.985643 meddlr-0.0.7rc1/meddlr/evaluation/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      255 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/evaluation/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     7703 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/evaluation/evaluator.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    18528 2022-12-07 01:31:05.000000 meddlr-0.0.7rc1/meddlr/evaluation/recon_evaluation.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     5068 2022-10-21 02:27:52.000000 meddlr-0.0.7rc1/meddlr/evaluation/scan_evaluator.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    12615 2022-10-21 17:37:55.000000 meddlr-0.0.7rc1/meddlr/evaluation/seg_evaluation.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    16054 2022-11-03 07:25:56.000000 meddlr-0.0.7rc1/meddlr/evaluation/testing.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:09.989643 meddlr-0.0.7rc1/meddlr/forward/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      129 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/forward/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     5165 2022-10-21 18:30:15.000000 meddlr-0.0.7rc1/meddlr/forward/mri.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:10.004643 meddlr-0.0.7rc1/meddlr/metrics/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      477 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/metrics/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     4417 2022-10-21 17:37:55.000000 meddlr-0.0.7rc1/meddlr/metrics/build.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     3025 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/metrics/collection.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:10.012643 meddlr-0.0.7rc1/meddlr/metrics/functional/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      444 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/metrics/functional/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    15595 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/metrics/functional/image.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     5787 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/metrics/functional/sem_seg.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     5516 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/metrics/functional/util.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    18811 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/metrics/image.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     6703 2022-12-05 17:30:24.000000 meddlr-0.0.7rc1/meddlr/metrics/lpip.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     8386 2022-10-21 17:37:55.000000 meddlr-0.0.7rc1/meddlr/metrics/metric.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     4596 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/metrics/sem_seg.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     9571 2022-12-05 17:30:24.000000 meddlr-0.0.7rc1/meddlr/metrics/ssfd.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:10.016643 meddlr-0.0.7rc1/meddlr/modeling/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      465 2022-10-31 18:35:33.000000 meddlr-0.0.7rc1/meddlr/modeling/__init__.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:10.022643 meddlr-0.0.7rc1/meddlr/modeling/blocks/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      450 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/modeling/blocks/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     6008 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/modeling/blocks/conv_blocks.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     8180 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/modeling/blocks/fuse_blocks.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:10.035643 meddlr-0.0.7rc1/meddlr/modeling/layers/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      425 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/modeling/layers/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     8557 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/modeling/layers/build.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     2701 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/modeling/layers/conv.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     5125 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/modeling/layers/gauss.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     7428 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/modeling/layers/layers2D.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     6937 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/modeling/layers/layers3D.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    13127 2022-12-07 01:31:05.000000 meddlr-0.0.7rc1/meddlr/modeling/loss_computer.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:10.057643 meddlr-0.0.7rc1/meddlr/modeling/meta_arch/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      550 2022-10-31 18:35:33.000000 meddlr-0.0.7rc1/meddlr/modeling/meta_arch/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     9129 2022-12-07 06:16:39.000000 meddlr-0.0.7rc1/meddlr/modeling/meta_arch/build.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     6532 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/modeling/meta_arch/cs_model.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     7992 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/modeling/meta_arch/denoising.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     8167 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/modeling/meta_arch/generalized_unet.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     7288 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/modeling/meta_arch/m2r.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     9988 2022-11-15 16:25:49.000000 meddlr-0.0.7rc1/meddlr/modeling/meta_arch/n2r.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     7797 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/modeling/meta_arch/nm2r.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     8856 2022-10-31 02:42:47.000000 meddlr-0.0.7rc1/meddlr/modeling/meta_arch/ssdu.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    14800 2022-12-06 03:36:43.000000 meddlr-0.0.7rc1/meddlr/modeling/meta_arch/unet.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    13686 2022-11-21 18:25:37.000000 meddlr-0.0.7rc1/meddlr/modeling/meta_arch/unrolled.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     8649 2022-11-15 16:25:49.000000 meddlr-0.0.7rc1/meddlr/modeling/meta_arch/vortex.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:10.066643 meddlr-0.0.7rc1/meddlr/ops/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      814 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/ops/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     5436 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/ops/categorical.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    12137 2022-11-08 22:25:14.000000 meddlr-0.0.7rc1/meddlr/ops/complex.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    11052 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/ops/fft.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     5686 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/ops/utils.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:10.073643 meddlr-0.0.7rc1/meddlr/solver/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      265 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/solver/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     3526 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/solver/build.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     4442 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/solver/lr_scheduler.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     2125 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/solver/optimizer.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:10.086643 meddlr-0.0.7rc1/meddlr/transforms/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      263 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/transforms/__init__.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:10.095643 meddlr-0.0.7rc1/meddlr/transforms/base/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      342 2022-08-04 01:44:09.000000 meddlr-0.0.7rc1/meddlr/transforms/base/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    12049 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/transforms/base/mask.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     2888 2022-11-08 22:25:14.000000 meddlr-0.0.7rc1/meddlr/transforms/base/motion.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     4286 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/transforms/base/noise.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     8862 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/transforms/base/spatial.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     4368 2022-10-27 18:39:32.000000 meddlr-0.0.7rc1/meddlr/transforms/build.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:10.099643 meddlr-0.0.7rc1/meddlr/transforms/builtin/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)        0 2022-08-04 01:44:10.000000 meddlr-0.0.7rc1/meddlr/transforms/builtin/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    14926 2022-11-08 22:25:14.000000 meddlr-0.0.7rc1/meddlr/transforms/builtin/mri.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:10.102643 meddlr-0.0.7rc1/meddlr/transforms/functional/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)       73 2022-11-08 22:25:14.000000 meddlr-0.0.7rc1/meddlr/transforms/functional/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     1209 2022-11-08 22:25:14.000000 meddlr-0.0.7rc1/meddlr/transforms/functional/mri.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:10.113643 meddlr-0.0.7rc1/meddlr/transforms/gen/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      388 2022-11-08 22:25:14.000000 meddlr-0.0.7rc1/meddlr/transforms/gen/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     2959 2022-08-04 01:44:10.000000 meddlr-0.0.7rc1/meddlr/transforms/gen/choice.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     1864 2022-08-04 01:44:10.000000 meddlr-0.0.7rc1/meddlr/transforms/gen/mask.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     2318 2022-11-08 22:25:14.000000 meddlr-0.0.7rc1/meddlr/transforms/gen/motion.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     1695 2022-11-15 16:25:49.000000 meddlr-0.0.7rc1/meddlr/transforms/gen/noise.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     6908 2022-11-08 22:24:43.000000 meddlr-0.0.7rc1/meddlr/transforms/gen/spatial.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      517 2022-08-04 01:44:10.000000 meddlr-0.0.7rc1/meddlr/transforms/mixins.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)       84 2022-08-04 01:44:10.000000 meddlr-0.0.7rc1/meddlr/transforms/param_kind.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    18373 2022-08-04 01:44:10.000000 meddlr-0.0.7rc1/meddlr/transforms/tf_scheduler.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     9527 2022-11-08 22:25:14.000000 meddlr-0.0.7rc1/meddlr/transforms/transform.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     6841 2022-11-08 22:25:14.000000 meddlr-0.0.7rc1/meddlr/transforms/transform_gen.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:10.140643 meddlr-0.0.7rc1/meddlr/utils/
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)       69 2022-08-04 01:44:10.000000 meddlr-0.0.7rc1/meddlr/utils/__init__.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     1635 2022-08-04 01:44:10.000000 meddlr-0.0.7rc1/meddlr/utils/cfl.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     9549 2022-08-04 01:44:10.000000 meddlr-0.0.7rc1/meddlr/utils/cluster.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     3896 2022-08-04 01:44:10.000000 meddlr-0.0.7rc1/meddlr/utils/collect_env.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     8855 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/utils/comm.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     1482 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/utils/deprecated.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    12224 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/utils/env.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    14904 2022-08-04 01:44:10.000000 meddlr-0.0.7rc1/meddlr/utils/events.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     3302 2022-08-04 01:44:10.000000 meddlr-0.0.7rc1/meddlr/utils/general.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     7553 2022-08-04 01:44:10.000000 meddlr-0.0.7rc1/meddlr/utils/logger.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     2600 2022-08-04 01:44:10.000000 meddlr-0.0.7rc1/meddlr/utils/memory.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    19597 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/utils/path.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     2806 2022-08-04 01:44:10.000000 meddlr-0.0.7rc1/meddlr/utils/profiler.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     2622 2022-08-04 01:44:10.000000 meddlr-0.0.7rc1/meddlr/utils/registry.py
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)    10657 2022-10-21 16:45:16.000000 meddlr-0.0.7rc1/meddlr/utils/transforms.py
-drwxrwxr-x   0 arjundd   (1043) arjundd   (1043)        0 2022-12-07 06:29:09.911643 meddlr-0.0.7rc1/meddlr.egg-info/
--rw-rw-rw-   0 arjundd   (1043) arjundd   (1043)     4012 2022-12-07 06:29:08.000000 meddlr-0.0.7rc1/meddlr.egg-info/PKG-INFO
--rw-rw-rw-   0 arjundd   (1043) arjundd   (1043)     3875 2022-12-07 06:29:09.000000 meddlr-0.0.7rc1/meddlr.egg-info/SOURCES.txt
--rw-rw-rw-   0 arjundd   (1043) arjundd   (1043)        1 2022-12-07 06:29:08.000000 meddlr-0.0.7rc1/meddlr.egg-info/dependency_links.txt
--rw-rw-rw-   0 arjundd   (1043) arjundd   (1043)      853 2022-12-07 06:29:09.000000 meddlr-0.0.7rc1/meddlr.egg-info/requires.txt
--rw-rw-rw-   0 arjundd   (1043) arjundd   (1043)        7 2022-12-07 06:29:09.000000 meddlr-0.0.7rc1/meddlr.egg-info/top_level.txt
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)       73 2022-08-04 01:44:10.000000 meddlr-0.0.7rc1/pyproject.toml
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)      559 2022-12-07 06:29:10.144643 meddlr-0.0.7rc1/setup.cfg
--rw-rw-r--   0 arjundd   (1043) arjundd   (1043)     4159 2022-12-07 01:31:05.000000 meddlr-0.0.7rc1/setup.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.222715 meddlr-0.0.8a1/
+-rw-r--r--   0 arjundd    (501) staff       (20)    11357 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/LICENSE
+-rw-r--r--   0 arjundd    (501) staff       (20)     3974 2023-04-29 19:47:16.222805 meddlr-0.0.8a1/PKG-INFO
+-rw-r--r--   0 arjundd    (501) staff       (20)     3265 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/README.md
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.202243 meddlr-0.0.8a1/meddlr/
+-rw-r--r--   0 arjundd    (501) staff       (20)      299 2023-04-29 19:38:28.000000 meddlr-0.0.8a1/meddlr/__init__.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.203237 meddlr-0.0.8a1/meddlr/checkpoint/
+-rw-r--r--   0 arjundd    (501) staff       (20)      165 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/checkpoint/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     1919 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/checkpoint/checkpoint.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.204089 meddlr-0.0.8a1/meddlr/config/
+-rw-r--r--   0 arjundd    (501) staff       (20)       67 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/config/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     4798 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/config/compat.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    14082 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/config/config.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    17235 2023-04-29 17:00:34.000000 meddlr-0.0.8a1/meddlr/config/defaults.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     4952 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/config/util.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.205035 meddlr-0.0.8a1/meddlr/data/
+-rw-r--r--   0 arjundd    (501) staff       (20)      587 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    13160 2023-04-29 16:30:43.000000 meddlr-0.0.8a1/meddlr/data/build.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     8987 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/catalog.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     1798 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/collate.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    10789 2023-04-29 16:30:52.000000 meddlr-0.0.8a1/meddlr/data/data_utils.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.205499 meddlr-0.0.8a1/meddlr/data/datasets/
+-rw-r--r--   0 arjundd    (501) staff       (20)       75 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/datasets/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     5955 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/datasets/builtin.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     4444 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/datasets/register_mrco.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.206433 meddlr-0.0.8a1/meddlr/data/samplers/
+-rw-r--r--   0 arjundd    (501) staff       (20)      484 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/samplers/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     3643 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/samplers/build.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    17837 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/samplers/group_sampler.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     4895 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/samplers/sampler.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     8201 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/slice_dataset.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.207449 meddlr-0.0.8a1/meddlr/data/transforms/
+-rw-r--r--   0 arjundd    (501) staff       (20)        0 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/transforms/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     5329 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/transforms/motion.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     6014 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/transforms/noise.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     5097 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/data/transforms/noiseandmotion.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    27768 2023-04-29 17:00:34.000000 meddlr-0.0.8a1/meddlr/data/transforms/subsample.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    15104 2023-04-29 17:00:34.000000 meddlr-0.0.8a1/meddlr/data/transforms/transform.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.208622 meddlr-0.0.8a1/meddlr/engine/
+-rw-r--r--   0 arjundd    (501) staff       (20)      322 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/engine/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    12982 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/engine/defaults.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    13868 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/engine/hooks.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     7667 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/engine/model_zoo.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     3211 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/engine/sharing.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     9387 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/engine/train_loop.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    17806 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/engine/trainer.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.209485 meddlr-0.0.8a1/meddlr/evaluation/
+-rw-r--r--   0 arjundd    (501) staff       (20)      255 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/evaluation/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     7703 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/evaluation/evaluator.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    18528 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/evaluation/recon_evaluation.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     5068 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/evaluation/scan_evaluator.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    12615 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/evaluation/seg_evaluation.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    16054 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/evaluation/testing.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.209759 meddlr-0.0.8a1/meddlr/forward/
+-rw-r--r--   0 arjundd    (501) staff       (20)      129 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/forward/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     5165 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/forward/mri.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.211874 meddlr-0.0.8a1/meddlr/metrics/
+-rw-r--r--   0 arjundd    (501) staff       (20)      477 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/metrics/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     4417 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/metrics/build.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     3042 2023-04-29 16:30:52.000000 meddlr-0.0.8a1/meddlr/metrics/collection.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.212410 meddlr-0.0.8a1/meddlr/metrics/functional/
+-rw-r--r--   0 arjundd    (501) staff       (20)      444 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/metrics/functional/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    15595 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/metrics/functional/image.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     5787 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/metrics/functional/sem_seg.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     5516 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/metrics/functional/util.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    18811 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/metrics/image.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     6703 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/metrics/lpip.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     8386 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/metrics/metric.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     4596 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/metrics/sem_seg.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     9571 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/metrics/ssfd.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.212669 meddlr-0.0.8a1/meddlr/modeling/
+-rw-r--r--   0 arjundd    (501) staff       (20)      465 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/__init__.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.213118 meddlr-0.0.8a1/meddlr/modeling/blocks/
+-rw-r--r--   0 arjundd    (501) staff       (20)      450 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/blocks/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     6008 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/blocks/conv_blocks.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     8180 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/blocks/fuse_blocks.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.213921 meddlr-0.0.8a1/meddlr/modeling/layers/
+-rw-r--r--   0 arjundd    (501) staff       (20)      425 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/layers/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     8557 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/layers/build.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     2701 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/layers/conv.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     5125 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/layers/gauss.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     7428 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/layers/layers2D.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     6937 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/layers/layers3D.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    13152 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/modeling/loss_computer.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.215720 meddlr-0.0.8a1/meddlr/modeling/meta_arch/
+-rw-r--r--   0 arjundd    (501) staff       (20)      565 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     9129 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/build.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     6532 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/cs_model.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     7992 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/denoising.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     8167 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/generalized_unet.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     7288 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/m2r.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     9988 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/n2r.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     7797 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/nm2r.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     9721 2023-04-29 17:00:34.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/ssdu.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    14800 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/unet.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    17035 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/unrolled.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     8649 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/modeling/meta_arch/vortex.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.216561 meddlr-0.0.8a1/meddlr/ops/
+-rw-r--r--   0 arjundd    (501) staff       (20)      814 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/ops/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     5436 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/ops/categorical.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    12676 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/ops/complex.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    11052 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/ops/fft.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     1925 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/ops/opt.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     5686 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/ops/utils.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.217075 meddlr-0.0.8a1/meddlr/solver/
+-rw-r--r--   0 arjundd    (501) staff       (20)      265 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/solver/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     3526 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/solver/build.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     4442 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/solver/lr_scheduler.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     2125 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/solver/optimizer.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.217953 meddlr-0.0.8a1/meddlr/transforms/
+-rw-r--r--   0 arjundd    (501) staff       (20)      263 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/__init__.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.218815 meddlr-0.0.8a1/meddlr/transforms/base/
+-rw-r--r--   0 arjundd    (501) staff       (20)      342 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/base/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    12049 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/base/mask.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     2888 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/transforms/base/motion.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     4286 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/base/noise.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     8862 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/base/spatial.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     4368 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/build.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.219073 meddlr-0.0.8a1/meddlr/transforms/builtin/
+-rw-r--r--   0 arjundd    (501) staff       (20)        0 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/builtin/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    14993 2023-04-29 17:00:34.000000 meddlr-0.0.8a1/meddlr/transforms/builtin/mri.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.219342 meddlr-0.0.8a1/meddlr/transforms/functional/
+-rw-r--r--   0 arjundd    (501) staff       (20)       73 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/transforms/functional/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     1209 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/transforms/functional/mri.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.220166 meddlr-0.0.8a1/meddlr/transforms/gen/
+-rw-r--r--   0 arjundd    (501) staff       (20)      388 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/transforms/gen/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     2959 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/gen/choice.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     1864 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/gen/mask.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     2318 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/transforms/gen/motion.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     1695 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/gen/noise.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     6908 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/gen/spatial.py
+-rw-r--r--   0 arjundd    (501) staff       (20)      517 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/mixins.py
+-rw-r--r--   0 arjundd    (501) staff       (20)       84 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/param_kind.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    18373 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/transforms/tf_scheduler.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     9527 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/transforms/transform.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     6841 2023-03-04 21:57:29.000000 meddlr-0.0.8a1/meddlr/transforms/transform_gen.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.222303 meddlr-0.0.8a1/meddlr/utils/
+-rw-r--r--   0 arjundd    (501) staff       (20)       69 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     1635 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/cfl.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     9549 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/cluster.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     3896 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/collect_env.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     8855 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/comm.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     1482 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/deprecated.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    12224 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/env.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    14904 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/events.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     3302 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/general.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     7553 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/logger.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     2600 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/memory.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    19597 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/path.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     2806 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/profiler.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     2622 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/registry.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    10657 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/meddlr/utils/transforms.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.202968 meddlr-0.0.8a1/meddlr.egg-info/
+-rw-r--r--   0 arjundd    (501) staff       (20)     3974 2023-04-29 19:47:16.000000 meddlr-0.0.8a1/meddlr.egg-info/PKG-INFO
+-rw-r--r--   0 arjundd    (501) staff       (20)     3949 2023-04-29 19:47:16.000000 meddlr-0.0.8a1/meddlr.egg-info/SOURCES.txt
+-rw-r--r--   0 arjundd    (501) staff       (20)        1 2023-04-29 19:47:16.000000 meddlr-0.0.8a1/meddlr.egg-info/dependency_links.txt
+-rw-r--r--   0 arjundd    (501) staff       (20)      867 2023-04-29 19:47:16.000000 meddlr-0.0.8a1/meddlr.egg-info/requires.txt
+-rw-r--r--   0 arjundd    (501) staff       (20)        7 2023-04-29 19:47:16.000000 meddlr-0.0.8a1/meddlr.egg-info/top_level.txt
+-rw-r--r--   0 arjundd    (501) staff       (20)       73 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/pyproject.toml
+-rw-r--r--   0 arjundd    (501) staff       (20)      559 2023-04-29 19:47:16.223137 meddlr-0.0.8a1/setup.cfg
+-rw-r--r--   0 arjundd    (501) staff       (20)     8059 2023-04-29 19:47:10.000000 meddlr-0.0.8a1/setup.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-04-29 19:47:16.222574 meddlr-0.0.8a1/tests/
+-rw-r--r--   0 arjundd    (501) staff       (20)     3021 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/tests/test_experiments.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     1670 2022-12-28 01:38:35.000000 meddlr-0.0.8a1/tests/test_reproducibility.py
```

### Comparing `meddlr-0.0.7rc1/LICENSE` & `meddlr-0.0.8a1/LICENSE`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/PKG-INFO` & `meddlr-0.0.8a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: meddlr
-Version: 0.0.7rc1
+Version: 0.0.8a1
 Summary: Meddlr is a config-driven framework built to simplify ML-based medical image reconstruction and analysis.
 Home-page: https://github.com/ad12/meddlr
 Author: The Meddlr Team
 Author-email: arjundd@stanford.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: benchmarking
@@ -93,9 +91,7 @@
 @article{desai2021noise2recon,
   title={Noise2Recon: A Semi-Supervised Framework for Joint MRI Reconstruction and Denoising},
   author={Desai, Arjun D and Ozturkler, Batu M and Sandino, Christopher M and Vasanawala, Shreyas and Hargreaves, Brian A and Re, Christopher M and Pauly, John M and Chaudhari, Akshay S},
   journal={arXiv preprint arXiv:2110.00075},
   year={2021}
 }
 ```
-
-
```

### Comparing `meddlr-0.0.7rc1/README.md` & `meddlr-0.0.8a1/README.md`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/checkpoint/checkpoint.py` & `meddlr-0.0.8a1/meddlr/checkpoint/checkpoint.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/config/compat.py` & `meddlr-0.0.8a1/meddlr/config/compat.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/config/config.py` & `meddlr-0.0.8a1/meddlr/config/config.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/config/defaults.py` & `meddlr-0.0.8a1/meddlr/config/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,19 @@
 _C.MODEL.UNROLLED.CONV_BLOCK.ACTIVATION = "relu"
 # Normalization type. Either "none", "instance", or "batch"
 _C.MODEL.UNROLLED.CONV_BLOCK.NORM = "none"
 # Use affine on normalization block.
 _C.MODEL.UNROLLED.CONV_BLOCK.NORM_AFFINE = False
 _C.MODEL.UNROLLED.CONV_BLOCK.ORDER = ("norm", "act", "drop", "conv")
 
+# Data consistency parameters.
+_C.MODEL.UNROLLED.DC = CN()
+_C.MODEL.UNROLLED.DC.MAX_ITER = 10
+_C.MODEL.UNROLLED.DC.EPS = 1e-4
+
 # Reconstruction loss parameters.
 _C.MODEL.RECON_LOSS = CN()
 # The reconstruction loss type. See :obj:`meddlr.modeling.loss_computer` for options.
 _C.MODEL.RECON_LOSS.NAME = "l1"
 # Whether to renormalize the predicted image before computing the loss.
 _C.MODEL.RECON_LOSS.RENORMALIZE_DATA = True
 # Consistency configuration. Used for Noise2Recon and VORTEX.
@@ -205,14 +210,15 @@
 # -----------------------------------------------------------------------------
 # SSDU model
 # -----------------------------------------------------------------------------
 _C.MODEL.SSDU = CN()
 _C.MODEL.SSDU.META_ARCHITECTURE = "GeneralizedUnrolledCNN"
 _C.MODEL.SSDU.MASKER = CN()
 _C.MODEL.SSDU.MASKER.PARAMS = CN(new_allowed=True)
+_C.MODEL.SSDU.AUGMENTOR = _MRI_RECON_TFM.clone()
 
 # -----------------------------------------------------------------------------
 # MONAI wrapper
 # -----------------------------------------------------------------------------
 _C.MODEL.MONAI = CN(new_allowed=True)
 
 # -----------------------------------------------------------------------------
```

### Comparing `meddlr-0.0.7rc1/meddlr/config/util.py` & `meddlr-0.0.8a1/meddlr/config/util.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/data/__init__.py` & `meddlr-0.0.8a1/meddlr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/data/build.py` & `meddlr-0.0.8a1/meddlr/data/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from meddlr.data.catalog import DatasetCatalog
 from meddlr.data.collate import collate_by_supervision, default_collate
 from meddlr.data.samplers.build import build_train_sampler, build_val_sampler
 from meddlr.data.slice_dataset import SliceData
 from meddlr.data.transforms import transform as T
 from meddlr.data.transforms.subsample import build_mask_func
+from meddlr.utils import env
 
 __all__ = ["build_recon_train_loader", "build_recon_val_loader"]
 
 
 def get_recon_dataset_dicts(
     dataset_names: Sequence[str],
     num_scans_total: Union[int, Tuple] = -1,
@@ -229,20 +230,25 @@
         dl_kwargs = {
             "sampler": sampler,
             "batch_size": cfg.SOLVER.TRAIN_BATCH_SIZE,
             "shuffle": shuffle,
             "drop_last": cfg.DATALOADER.DROP_LAST,
         }
 
+    num_workers = cfg.DATALOADER.NUM_WORKERS
+    prefetch_factor = cfg.DATALOADER.PREFETCH_FACTOR
+    if env.pt_version() >= "2.0" and num_workers == 0:
+        prefetch_factor = None
+
     train_loader = DataLoader(
         dataset=train_data,
-        num_workers=cfg.DATALOADER.NUM_WORKERS,
+        num_workers=num_workers,
         pin_memory=True,
         collate_fn=collate_fn,
-        prefetch_factor=cfg.DATALOADER.PREFETCH_FACTOR,
+        prefetch_factor=prefetch_factor,
         **dl_kwargs,
     )
     return train_loader
 
 
 def build_recon_val_loader(
     cfg,
```

### Comparing `meddlr-0.0.7rc1/meddlr/data/catalog.py` & `meddlr-0.0.8a1/meddlr/data/catalog.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/data/collate.py` & `meddlr-0.0.8a1/meddlr/data/collate.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/data/data_utils.py` & `meddlr-0.0.8a1/meddlr/data/data_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,15 @@
         raise ValueError("All patches must have the same shape")
 
     stack_shape = []
     coords_arr = np.asarray(coords)
     assert coords_arr.ndim == 2
     stack_shape = tuple(np.max(coords_arr[:, c]).item() + 1 for c in range(coords_arr.shape[1]))
 
-    struct = np.empty(stack_shape, dtype=np.object)
+    struct = np.empty(stack_shape, dtype="object")
     for coord, patch in zip(coords, patches):
         struct[coord] = patch
     if any(x is None for x in struct.flatten()):
         raise ValueError("Did not get dense labels.")
     struct = struct.tolist()
 
     out = _recursive_stack(struct)
```

### Comparing `meddlr-0.0.7rc1/meddlr/data/datasets/builtin.py` & `meddlr-0.0.8a1/meddlr/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/data/datasets/register_mrco.py` & `meddlr-0.0.8a1/meddlr/data/datasets/register_mrco.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/data/samplers/build.py` & `meddlr-0.0.8a1/meddlr/data/samplers/build.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/data/samplers/group_sampler.py` & `meddlr-0.0.8a1/meddlr/data/samplers/group_sampler.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/data/samplers/sampler.py` & `meddlr-0.0.8a1/meddlr/data/samplers/sampler.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/data/slice_dataset.py` & `meddlr-0.0.8a1/meddlr/data/slice_dataset.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/data/transforms/motion.py` & `meddlr-0.0.8a1/meddlr/data/transforms/motion.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/data/transforms/noise.py` & `meddlr-0.0.8a1/meddlr/data/transforms/noise.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/data/transforms/noiseandmotion.py` & `meddlr-0.0.8a1/meddlr/data/transforms/noiseandmotion.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/data/transforms/subsample.py` & `meddlr-0.0.8a1/meddlr/data/transforms/subsample.py`

 * *Files 4% similar despite different names*

```diff
@@ -374,14 +374,61 @@
 
         Expected `kspace` shape (batch, ky, kz, ...).
         """
         # TODO: dims should be configured based on the number of dimenions in the input.
         return get_cartesian_edge_mask(kspace, dims=(1, 2), out_shape=out_shape)
 
 
+@MASK_FUNC_REGISTRY.register()
+class EquispacedMaskFunc2D(MaskFunc):
+    """
+
+    Adapted from https://github.com/facebookresearch/fastMRI/blob/master/common/subsample.py
+    """
+
+    def __init__(self, accelerations, calib_size=None, center_fractions=None):
+        if not calib_size and not center_fractions:
+            raise ValueError("Either calib_size or center_fractions must be specified.")
+        if calib_size and center_fractions:
+            raise ValueError("Only one of calib_size or center_fractions can be specified")
+        assert not center_fractions, "Center fractions not supported for equispaced sampling."
+
+        self.center_fractions = center_fractions
+        self.calib_size = calib_size
+        super().__init__(accelerations)
+
+    def choose_acceleration(self) -> int:
+        # Accelerations for equispaced sampling must be an integer.
+        acc = super().choose_acceleration()
+        return int(round(acc))
+
+    def __call__(self, shape, seed: int = None, acceleration: int = None):
+        """
+        Args:
+            shape (iterable[int]): The shape of the mask to be created. The shape should have
+                at least 3 dimensions. Samples are drawn along the second last dimension.
+            seed (int, optional): Seed for the random number generator. Setting the seed
+                ensures the same mask is generated each time for the same shape.
+        Returns:
+            torch.Tensor: A mask of the specified shape.
+        """
+        if len(shape) < 3:
+            raise ValueError("Shape should have 3 or more dimensions")
+
+        calib = self.calib_size
+        if acceleration is None:
+            acceleration = self.choose_acceleration()
+
+        return equispaced_mask(shape, accel=acceleration, calib=calib, dim=2)
+
+    def get_edge_mask(self, kspace: torch.Tensor, out_shape: Sequence[int] = None):
+        # TODO: dims should be configured based on the number of dimenions in the input.
+        return get_cartesian_edge_mask(kspace, dims=(1, 2), out_shape=out_shape)
+
+
 def get_cartesian_edge_mask(
     kspace: torch.Tensor,
     dims: Union[int, Sequence[int]],
     out_shape: Sequence[int] = None,
     dtype=torch.float32,
 ):
     """See :method:`MaskFunc.get_edge_mask`.
@@ -506,14 +553,75 @@
 
 
 def _get_center(size: int) -> float:
     """Get the center of the matrix."""
     return size // 2 if size % 2 == 1 else size // 2 - 0.5
 
 
+def equispaced_mask(
+    shape: Union[int, Tuple[int]],
+    accel: int,
+    offset: Union[int, Tuple[int]] = 0,
+    calib: int = None,
+    device=None,
+    dtype=torch.float32,
+    dim: int = None,
+) -> torch.Tensor:
+    """Generate equispaced mask.
+
+    Args:
+        shape: Shape of the mask to generate.
+        accel: Acceleration factor.
+        offset: Offset of the mask.
+        calib: Size of the calibration region.
+        device: Device to place the mask on.
+        dtype: Data type of the mask.
+        dim: Dimension of undersampling.
+            For example, `dim=1` will generate a 1D undersampling mask.
+            If `None`, `dim` will be set to the length of `shape`.
+
+    Returns:
+        torch.Tensor: The mask.
+    """
+    if isinstance(shape, int):
+        shape = (shape,)
+    if dim is None:
+        dim = len(shape)
+    if isinstance(offset, int):
+        offset = (offset,) * dim
+    if len(offset) != dim:
+        raise ValueError("offset must have the same length as shape")
+    if isinstance(calib, int):
+        calib = (calib,) * dim
+
+    # Perform masking on 1D tensor and reshape.
+    dim_shape = shape[-dim:]
+    offset = _flatten_offset(offset, dim_shape)
+    mask = torch.zeros(np.prod(dim_shape), dtype=dtype, device=device)
+    mask[offset::accel] = 1
+    mask = mask.reshape(dim_shape)
+
+    # TODO: Add calibration region.
+    if calib is not None:
+        pad = ((d - c + 1) // 2 for d, c in zip(dim_shape, calib))
+        calib_sl = tuple(slice(p, p + c) for p, c in zip(pad, calib))
+        mask[(Ellipsis,) + calib_sl] = 1
+
+    return mask.broadcast_to(shape)
+
+
+def _flatten_offset(offset, shape):
+    """Flatten the offset to a single integer."""
+    assert len(offset) == len(shape)
+    offset = np.asarray(offset)
+    multiplier = np.cumprod((1,) + shape[1:][::-1])
+
+    return np.sum(offset[::-1] * multiplier)
+
+
 # ================================================================ #
 # Adapted from sigpy.
 # Duplicated because of https://github.com/mikgroup/sigpy/issues/54
 # TODO: Remove once https://github.com/mikgroup/sigpy/issues/54 is
 # solved and added to release.
 # ================================================================ #
 def poisson(
```

### Comparing `meddlr-0.0.7rc1/meddlr/data/transforms/transform.py` & `meddlr-0.0.8a1/meddlr/data/transforms/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,18 +364,15 @@
         normalized = self._normalizer.normalize(
             **{"masked_kspace": masked_kspace, "image": image, "target": target, "mask": mask}
         )
         masked_kspace = normalized["masked_kspace"]
         target = normalized["target"]
         mean = normalized["mean"]
         std = normalized["std"]
-
-        add_noise = self.add_noise and (
-            self._is_test or (not is_fixed and self.rng.uniform() < self.p_noise)
-        )
+        add_noise = self.add_noise and (self._is_test or (self.rng.uniform() < self.p_noise))
         add_motion = self.add_motion and (
             self._is_test or (not is_fixed and self.rng.uniform() < self.p_motion)
         )
         if add_noise:
             # Seed should be different for each slice of a scan.
             noise_seed = seed + slice_id if seed is not None else None
             masked_kspace = self.noiser(masked_kspace, mask=mask, seed=noise_seed)
```

### Comparing `meddlr-0.0.7rc1/meddlr/engine/defaults.py` & `meddlr-0.0.8a1/meddlr/engine/defaults.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/engine/hooks.py` & `meddlr-0.0.8a1/meddlr/engine/hooks.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/engine/model_zoo.py` & `meddlr-0.0.8a1/meddlr/engine/model_zoo.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/engine/sharing.py` & `meddlr-0.0.8a1/meddlr/engine/sharing.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/engine/train_loop.py` & `meddlr-0.0.8a1/meddlr/engine/train_loop.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/engine/trainer.py` & `meddlr-0.0.8a1/meddlr/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/evaluation/evaluator.py` & `meddlr-0.0.8a1/meddlr/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/evaluation/recon_evaluation.py` & `meddlr-0.0.8a1/meddlr/evaluation/recon_evaluation.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/evaluation/scan_evaluator.py` & `meddlr-0.0.8a1/meddlr/evaluation/scan_evaluator.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/evaluation/seg_evaluation.py` & `meddlr-0.0.8a1/meddlr/evaluation/seg_evaluation.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/evaluation/testing.py` & `meddlr-0.0.8a1/meddlr/evaluation/testing.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/forward/mri.py` & `meddlr-0.0.8a1/meddlr/forward/mri.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/metrics/build.py` & `meddlr-0.0.8a1/meddlr/metrics/build.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/metrics/collection.py` & `meddlr-0.0.8a1/meddlr/metrics/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     def to_dict(self, group_by="Metric", sync_dist: bool = True) -> Dict[str, Any]:
         df = self.to_pandas(sync_dist=sync_dist)
         df = df.melt(id_vars=["Metric", "id"], var_name="category", value_name="value")
         if len(np.unique(df["category"])) > 1:
             df["Metric"] = df["Metric"] + "/" + df["category"]
         df = df.drop(columns="category")
-        values = df.groupby(by=group_by).mean()
+        values = df.groupby(by=group_by).mean(numeric_only=True)
         return values.to_dict()["value"]
 
     def summary(self, sync_dist: bool = True) -> str:
         """Get summary of results overall scans.
         Returns:
             str: Tabulated summary. Rows=metrics. Columns=classes.
         """
```

### Comparing `meddlr-0.0.7rc1/meddlr/metrics/functional/image.py` & `meddlr-0.0.8a1/meddlr/metrics/functional/image.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/metrics/functional/sem_seg.py` & `meddlr-0.0.8a1/meddlr/metrics/functional/sem_seg.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/metrics/functional/util.py` & `meddlr-0.0.8a1/meddlr/metrics/functional/util.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/metrics/image.py` & `meddlr-0.0.8a1/meddlr/metrics/image.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/metrics/lpip.py` & `meddlr-0.0.8a1/meddlr/metrics/lpip.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/metrics/metric.py` & `meddlr-0.0.8a1/meddlr/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/metrics/sem_seg.py` & `meddlr-0.0.8a1/meddlr/metrics/sem_seg.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/metrics/ssfd.py` & `meddlr-0.0.8a1/meddlr/metrics/ssfd.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/blocks/conv_blocks.py` & `meddlr-0.0.8a1/meddlr/modeling/blocks/conv_blocks.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/blocks/fuse_blocks.py` & `meddlr-0.0.8a1/meddlr/modeling/blocks/fuse_blocks.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/layers/build.py` & `meddlr-0.0.8a1/meddlr/modeling/layers/build.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/layers/conv.py` & `meddlr-0.0.8a1/meddlr/modeling/layers/conv.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/layers/gauss.py` & `meddlr-0.0.8a1/meddlr/modeling/layers/gauss.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/layers/layers2D.py` & `meddlr-0.0.8a1/meddlr/modeling/layers/layers2D.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/layers/layers3D.py` & `meddlr-0.0.8a1/meddlr/modeling/layers/layers3D.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/loss_computer.py` & `meddlr-0.0.8a1/meddlr/modeling/loss_computer.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,15 @@
         recon_loss = cfg.MODEL.RECON_LOSS.NAME
         consistency_loss = cfg.MODEL.CONSISTENCY.LOSS_NAME
         latent_loss = cfg.MODEL.CONSISTENCY.LATENT_LOSS_NAME
 
         assert recon_loss in IMAGE_LOSSES or recon_loss in KSPACE_LOSSES
         assert consistency_loss in IMAGE_LOSSES or consistency_loss in KSPACE_LOSSES
 
+        self.loss = None
         self.recon_loss = recon_loss
         self.consistency_loss = consistency_loss
         self.latent_loss = latent_loss
         self.renormalize_data = cfg.MODEL.RECON_LOSS.RENORMALIZE_DATA
         self.consistency_weight = cfg.MODEL.CONSISTENCY.LOSS_WEIGHT
         self.latent_weight = cfg.MODEL.CONSISTENCY.LATENT_LOSS_WEIGHT
         self.use_latent = cfg.MODEL.CONSISTENCY.USE_LATENT
```

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/meta_arch/__init__.py` & `meddlr-0.0.8a1/meddlr/modeling/meta_arch/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,9 +3,9 @@
 from .denoising import DenoisingModel  # noqa: F401
 from .generalized_unet import GeneralizedUNet  # noqa: F401
 from .m2r import M2RModel  # noqa: F401
 from .n2r import N2RModel  # noqa: F401
 from .nm2r import NM2RModel  # noqa: F401
 from .ssdu import SSDUModel  # noqa: F401
 from .unet import UnetModel  # noqa: F401
-from .unrolled import GeneralizedUnrolledCNN  # noqa: F401
+from .unrolled import CGUnrolledCNN, GeneralizedUnrolledCNN  # noqa: F401
 from .vortex import VortexModel  # noqa: F401
```

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/meta_arch/build.py` & `meddlr-0.0.8a1/meddlr/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/meta_arch/cs_model.py` & `meddlr-0.0.8a1/meddlr/modeling/meta_arch/cs_model.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/meta_arch/denoising.py` & `meddlr-0.0.8a1/meddlr/modeling/meta_arch/denoising.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/meta_arch/generalized_unet.py` & `meddlr-0.0.8a1/meddlr/modeling/meta_arch/generalized_unet.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/meta_arch/m2r.py` & `meddlr-0.0.8a1/meddlr/modeling/meta_arch/m2r.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/meta_arch/n2r.py` & `meddlr-0.0.8a1/meddlr/modeling/meta_arch/n2r.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/meta_arch/nm2r.py` & `meddlr-0.0.8a1/meddlr/modeling/meta_arch/nm2r.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/meta_arch/ssdu.py` & `meddlr-0.0.8a1/meddlr/modeling/meta_arch/ssdu.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import meddlr.ops as oF
 from meddlr.config.config import configurable
 from meddlr.forward.mri import SenseModel
 from meddlr.modeling.meta_arch.build import META_ARCH_REGISTRY, build_model
 from meddlr.ops import complex as cplx
 from meddlr.transforms.base.mask import KspaceMaskTransform
+from meddlr.transforms.builtin.mri import MRIReconAugmentor
 from meddlr.transforms.gen.mask import RandomKspaceMask
 from meddlr.utils.events import get_event_storage
 from meddlr.utils.general import move_to_device
 
 
 @META_ARCH_REGISTRY.register()
 class SSDUModel(nn.Module):
@@ -32,23 +33,31 @@
         without fully sampled reference data.
         https://onlinelibrary-wiley-com.stanford.idm.oclc.org/doi/full/10.1002/mrm.28378
     """
 
     _version = 1
 
     @configurable
-    def __init__(self, model: nn.Module, masker: RandomKspaceMask, vis_period: int = None):
+    def __init__(
+        self,
+        model: nn.Module,
+        masker: RandomKspaceMask,
+        augmentor: MRIReconAugmentor = None,
+        vis_period: int = None,
+    ):
         """
         Args:
             model (nn.Module): The base model.
-            masker (NoiseModel): The additive noise module.
+            masker (NoiseModel): The masking model.
+            augmentor: An augmentation model that can be used
         """
         super().__init__()
         self.model = model
         self.masker = masker
+        self.augmentor = augmentor
         # Visualization done by this model
         if hasattr(self.model, "vis_period"):
             if vis_period is not None:
                 self.model.vis_period = vis_period
             else:
                 vis_period = self.model.vis_period
             self.model.vis_period = -1
@@ -84,14 +93,19 @@
 
         # TODO (arjundd): See if we can remove this check for speed reasons.
         assert torch.all(loss_mask >= 0)
 
         inputs = {k: v.clone() for k, v in inputs.items() if k != "kspace"}
         inputs["kspace"] = train_mask * kspace
         inputs["mask"] = train_mask
+
+        if self.augmentor is not None:
+            out, _, _ = self.augmentor(kspace=inputs["kspace"], maps=inputs["maps"])
+            inputs["kspace"] = out["kspace"]
+
         return inputs, mask[..., 0:1], train_mask, loss_mask[..., 0:1]
 
     @torch.no_grad()
     def visualize(self, images_dict):
         for name, images in images_dict.items():
             storage = get_event_storage()
             if isinstance(images, (tuple, list)):
@@ -136,14 +150,17 @@
 
         storage = get_event_storage()
         vis_training = self.training and self.vis_period > 0 and storage.iter % self.vis_period == 0
 
         # Put supervised and unsupervised scans in a single tensor.
         sup = inputs.get("supervised", {})
         unsup = inputs.get("unsupervised", {})
+        # TODO: Make the cat operation recursive.
+        sup = {k: v for k, v in sup.items() if k != "metrics"}
+        unsup = {k: v for k, v in unsup.items() if k != "metrics"}
         if sup or unsup:
             inputs = {
                 k: torch.cat([sup.get(k, torch.tensor([])), unsup.get(k, torch.tensor([]))])
                 for k in sup.keys() | unsup.keys()
             }
         assert all(k in inputs for k in ["kspace"])
 
@@ -201,13 +218,21 @@
     def from_config(cls, cfg):
         model_cfg = cfg.clone()
         model_cfg.defrost()
         model_cfg.MODEL.META_ARCHITECTURE = cfg.MODEL.SSDU.META_ARCHITECTURE
         model_cfg.freeze()
         model = build_model(model_cfg)
 
-        # TODO: Configure this
+        # Train/loss mask splitter.
         params = cfg.MODEL.SSDU.MASKER.PARAMS
         masker = RandomKspaceMask(**params)
         masker.to(cfg.MODEL.DEVICE)
 
-        return {"model": model, "masker": masker}
+        init_kwargs = {"model": model, "masker": masker}
+
+        # Build augmentor.
+        aug_cfg = cfg.MODEL.SSDU.AUGMENTOR
+        if aug_cfg.TRANSFORMS:
+            augmentor = MRIReconAugmentor.from_cfg(aug_cfg, aug_kind=None, seed=cfg.SEED)
+            init_kwargs["augmentor"] = augmentor
+
+        return init_kwargs
```

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/meta_arch/unet.py` & `meddlr-0.0.8a1/meddlr/modeling/meta_arch/unet.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/meta_arch/unrolled.py` & `meddlr-0.0.8a1/meddlr/modeling/meta_arch/unrolled.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from numbers import Number
-from typing import Any, Dict, Sequence, Union
+from typing import Any, Dict, Sequence, Tuple, Union
 
 import torch
 import torchvision.utils as tv_utils
 from torch import nn
 
 import meddlr.ops.complex as cplx
 from meddlr.config import CfgNode
 from meddlr.config.config import configurable
 from meddlr.forward.mri import SenseModel
+from meddlr.ops.opt import conjgrad
 from meddlr.utils.events import get_event_storage
 from meddlr.utils.general import move_to_device
 
 from ..layers.layers2D import ResNet
 from .build import META_ARCH_REGISTRY, build_model
 
 __all__ = ["GeneralizedUnrolledCNN"]
@@ -36,27 +37,31 @@
         self,
         blocks: Union[nn.Module, Sequence[nn.Module]],
         step_sizes: Union[float, Sequence[float]] = -2.0,
         fix_step_size: bool = False,
         num_emaps: int = 1,
         vis_period: int = -1,
         num_grad_steps: int = None,
+        order: Tuple[str] = ("dc", "reg"),
     ):
         """
         Args:
             blocks: A sequence of blocks
             step_sizes: Step size for data consistency prior to each block.
                 If a single float is given, the same step size is used for all blocks.
             fix_step_size: Whether to fix the step size to a given value --
                 i.e. set to ``True`` to make the step size non-trainable.
             num_emaps: Number of sensitivity maps used to estimate the image.
             vis_period: Number of steps between logging visualizations.
             num_grad_steps: Number of unrolled steps in the network.
                 This is deprecated - the number of steps will be determined
                 from the length of ``blocks``.
+            order: The order to apply the data consistency (dc) and model-based
+                regularization (reg) blocks. One of ``('dc', 'reg')`` or
+                ``('reg', 'dc')``.
         """
         super().__init__()
 
         self.resnets = blocks
         if num_grad_steps is None:
             if isinstance(blocks, Sequence) and not isinstance(blocks, nn.ModuleList):
                 blocks = nn.ModuleList(blocks)
@@ -84,14 +89,19 @@
             step_sizes = nn.ParameterList([nn.Parameter(s) for s in step_sizes])
         self.step_sizes: Sequence[Union[torch.Tensor, nn.Parameter]] = step_sizes
 
         self.num_repeat_steps = num_repeat_steps
         self.num_emaps = num_emaps
         self.vis_period = vis_period
 
+        if order not in [("dc", "reg"), ("reg", "dc")]:
+            raise ValueError("`order` must be one of ('dc', 'reg') or ('reg', 'dc')")
+        self.order = order
+        self._dc_first = order[0] == "dc"
+
     def visualize_training(
         self, kspace: torch.Tensor, zfs: torch.Tensor, targets: torch.Tensor, preds: torch.Tensor
     ):
         """Visualize kspace data and reconstructions.
 
         Dimension ``(,2)`` indicates optional dimension for real-valued view of complex tensors.
         For example, a real-valued tensor of shape BxHxWx2 will be interpreted as
@@ -126,14 +136,55 @@
             }
 
             for name, data in imgs_to_write.items():
                 data = data.squeeze(-1).unsqueeze(1)
                 data = tv_utils.make_grid(data, nrow=1, padding=1, normalize=True, scale_each=True)
                 storage.put_image("train/{}".format(name), data.numpy(), data_format="CHW")
 
+    def dc(
+        self,
+        *,
+        image: torch.Tensor,
+        A: SenseModel,
+        zf_image: torch.Tensor,
+        step_size: Union[torch.Tensor, float]
+    ):
+        grad_x = A(A(image), adjoint=True) - zf_image
+        return image + step_size * grad_x
+
+    def reg(self, *, image: torch.Tensor, model: nn.Module, dims: torch.Size):
+        # If the image is a complex tensor, we view it as a real image
+        # where last dimension has 2 channels (real, imaginary).
+        # This may take more time, but is done for backwards compatibility
+        # reasons.
+        # TODO (arjundd): Fix to auto-detect which version of the model is being used.
+        if dims is None:
+            dims = image.size()
+
+        use_cplx = cplx.is_complex(image)
+        if use_cplx:
+            image = torch.view_as_real(image)
+
+        # prox update
+        image = image.reshape(dims[0:3] + (self.num_emaps * 2,)).permute(0, 3, 1, 2)
+        if hasattr(model, "base_forward") and callable(model.base_forward):
+            image = model.base_forward(image)
+        else:
+            image = model(image)
+
+        # This doesn't work when padding is not the same.
+        # i.e. when the output is a different shape than the input.
+        # However, this should not ever happen.
+        image = image.permute(0, 2, 3, 1).reshape(dims[0:3] + (self.num_emaps, 2))
+        if not image.is_contiguous():
+            image = image.contiguous()
+        if use_cplx:
+            image = torch.view_as_complex(image)
+        return image
+
     def forward(self, inputs: Dict[str, Any], return_pp: bool = False, vis_training: bool = False):
         """Reconstructs the image from the kspace.
 
         Dimension ``(,2)`` indicates optional dimension for real-valued view of complex tensors.
         For example, a real-valued tensor of shape BxHxWx2 will be interpreted as
         a complex-valued tensor of shape BxHxW.
 
@@ -201,40 +252,20 @@
 
         # Compute zero-filled image reconstruction
         zf_image = A(kspace, adjoint=True)
 
         # Begin unrolled proximal gradient descent
         image = zf_image
         for resnet, step_size in zip(conv_blocks, step_sizes):
-            # dc update
-            grad_x = A(A(image), adjoint=True) - zf_image
-            image = image + step_size * grad_x
-
-            # If the image is a complex tensor, we view it as a real image
-            # where last dimension has 2 channels (real, imaginary).
-            # This may take more time, but is done for backwards compatibility
-            # reasons.
-            # TODO (arjundd): Fix to auto-detect which version of the model is
-            # being used.
-            use_cplx = cplx.is_complex(image)
-            if use_cplx:
-                image = torch.view_as_real(image)
-
-            # prox update
-            image = image.reshape(dims[0:3] + (self.num_emaps * 2,)).permute(0, 3, 1, 2)
-            if hasattr(resnet, "base_forward") and callable(resnet.base_forward):
-                image = resnet.base_forward(image)
+            if self._dc_first:
+                image = self.dc(image=image, A=A, zf_image=zf_image, step_size=step_size)
+                image = self.reg(image=image, model=resnet, dims=dims)
             else:
-                image = resnet(image)
-
-            image = image.permute(0, 2, 3, 1).reshape(dims[0:3] + (self.num_emaps, 2))
-            if not image.is_contiguous():
-                image = image.contiguous()
-            if use_cplx:
-                image = torch.view_as_complex(image)
+                image = self.reg(image=image, model=resnet, dims=dims)
+                image = self.dc(image=image, A=A, zf_image=zf_image, step_size=step_size)
 
         # pred: shape [batch, height, width, #maps, 2]
         # target: shape [batch, height, width, #maps, 2]
         output_dict = {
             "pred": image,
             "target": target,
             "signal_model": A,
@@ -249,15 +280,15 @@
                 self.visualize_training(kspace, zf_image, target, image)
 
         output_dict["zf_image"] = zf_image
 
         return output_dict
 
     @classmethod
-    def from_config(cls, cfg: CfgNode, **kwargs) -> "GeneralizedUnrolledCNN":
+    def from_config(cls, cfg: CfgNode, **kwargs) -> Dict[str, Any]:
         """Build :cls:`GeneralizedUnrolledCNN` from a config.
 
         Args:
             cfg: The config.
             kwargs: Keyword arguments to override config-specified parameters.
 
         Returns:
@@ -300,14 +331,86 @@
             "vis_period": cfg.VIS_PERIOD,
             "num_grad_steps": num_grad_steps if share_weights else None,
         }
         out.update(kwargs)
         return out
 
 
+@META_ARCH_REGISTRY.register()
+class CGUnrolledCNN(GeneralizedUnrolledCNN):
+    """Unrolled CNN with conjugate gradient descent (CG) data consistency."""
+
+    @configurable
+    def __init__(
+        self,
+        blocks: Union[nn.Module, Sequence[nn.Module]],
+        step_sizes: Union[float, Sequence[float]] = -2,
+        fix_step_size: bool = False,
+        num_emaps: int = 1,
+        vis_period: int = -1,
+        num_grad_steps: int = None,
+        cg_max_iter: int = 10,
+        cg_eps: float = 1e-4,
+    ):
+        super().__init__(
+            blocks=blocks,
+            step_sizes=step_sizes,
+            fix_step_size=fix_step_size,
+            num_emaps=num_emaps,
+            vis_period=vis_period,
+            num_grad_steps=num_grad_steps,
+            order=("reg", "dc"),
+        )
+        self.cg_max_iter = cg_max_iter
+        self.cg_eps = cg_eps
+
+        for step_size in self.step_sizes:
+            if step_size < 0:
+                raise ValueError("Step size must be non-negative.")
+
+    def dc(
+        self,
+        *,
+        image: torch.Tensor,
+        A: SenseModel,
+        zf_image: torch.Tensor,
+        step_size: Union[torch.Tensor, float]
+    ):
+        def A_op(x):
+            return A(A(x), adjoint=True)
+
+        x_opt = conjgrad(
+            x=image,
+            b=zf_image + step_size * image,
+            A_op=A_op,
+            mu=step_size,
+            max_iter=self.cg_max_iter,
+            pbar=False,
+            eps=self.cg_eps,
+        )
+        return x_opt
+
+    @classmethod
+    def from_config(cls, cfg: CfgNode, **kwargs) -> Dict[str, Any]:
+        """Build :cls:`CGUnrolledCNN` from a config.
+
+        Args:
+            cfg: The config.
+            kwargs: Keyword arguments to override config-specified parameters.
+
+        Returns:
+            Dict[str, Any]: The parameters to pass to the constructor.
+        """
+        init_kwargs = super().from_config(cfg=cfg, **kwargs)
+        init_kwargs["cg_max_iter"] = cfg.MODEL.UNROLLED.DC.MAX_ITER
+        init_kwargs["cg_eps"] = cfg.MODEL.UNROLLED.DC.EPS
+        init_kwargs.update(kwargs)
+        return init_kwargs
+
+
 def _build_resblock(cfg: CfgNode) -> ResNet:
     """Build the resblock for unrolled network.
 
     Args:
         cfg (CfgNode): The network configuration.
 
     Note:
```

### Comparing `meddlr-0.0.7rc1/meddlr/modeling/meta_arch/vortex.py` & `meddlr-0.0.8a1/meddlr/modeling/meta_arch/vortex.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/ops/__init__.py` & `meddlr-0.0.8a1/meddlr/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/ops/categorical.py` & `meddlr-0.0.8a1/meddlr/ops/categorical.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/ops/complex.py` & `meddlr-0.0.8a1/meddlr/ops/complex.py`

 * *Files 5% similar despite different names*

```diff
@@ -438,7 +438,24 @@
 
     sl = [slice(None) for _ in range(x.ndim)]
     for d, shp, x_shp in zip(dims, shape, x_shape):
         start = (x_shp - shp) // 2
         end = start + shp
         sl[d] = slice(start, end)
     return x[sl]
+
+
+def bdot(x: torch.Tensor, y: torch.Tensor, keepdim: bool = False) -> torch.Tensor:
+    """Batch dot product (inner product) of two complex-valued tensors.
+
+    Args:
+        x: The first input tensor.
+        y: The second input tensor.
+
+    Returns:
+        torch.Tensor: The batch inner product :math:`<x, y>_i = sum(conj(x_i) * y_i)`.
+
+    Note:
+        To avoid ambiguity, use torch.complex tensors to represent complex values.
+    """
+    dim = tuple(range(1, x.ndim))
+    return torch.sum((x.conj() * y), dim=dim, keepdim=keepdim)
```

### Comparing `meddlr-0.0.7rc1/meddlr/ops/fft.py` & `meddlr-0.0.8a1/meddlr/ops/fft.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/ops/utils.py` & `meddlr-0.0.8a1/meddlr/ops/utils.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/solver/build.py` & `meddlr-0.0.8a1/meddlr/solver/build.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/solver/lr_scheduler.py` & `meddlr-0.0.8a1/meddlr/solver/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/solver/optimizer.py` & `meddlr-0.0.8a1/meddlr/solver/optimizer.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/transforms/base/mask.py` & `meddlr-0.0.8a1/meddlr/transforms/base/mask.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/transforms/base/motion.py` & `meddlr-0.0.8a1/meddlr/transforms/base/motion.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/transforms/base/noise.py` & `meddlr-0.0.8a1/meddlr/transforms/base/noise.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/transforms/base/spatial.py` & `meddlr-0.0.8a1/meddlr/transforms/base/spatial.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/transforms/build.py` & `meddlr-0.0.8a1/meddlr/transforms/build.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/transforms/builtin/mri.py` & `meddlr-0.0.8a1/meddlr/transforms/builtin/mri.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from numbers import Number
-from typing import Callable, Dict, Iterable, List, Sequence, Union
+from typing import Callable, Dict, Iterable, List, Optional, Sequence, Union
 
 import torch
 
 import meddlr.ops.complex as cplx
 from meddlr.config.config import CfgNode
 from meddlr.data.transforms.transform import Normalizer
 from meddlr.evaluation.testing import flatten_results_dict
@@ -315,15 +315,20 @@
         tfms = [tfm for tfm in self.tfms_or_gens if isinstance(tfm, DeviceMixin)]
         for t in tfms:
             t.to(device)
         return self
 
     @classmethod
     def from_cfg(
-        cls, cfg: CfgNode, aug_kind: str, seed: int = None, device: torch.device = None, **kwargs
+        cls,
+        cfg: CfgNode,
+        aug_kind: Optional[str],
+        seed: int = None,
+        device: torch.device = None,
+        **kwargs,
     ):
         """Build :cls:`MRIReconAugmentor` from a config.
 
         TODO (arjundd): Decorate __init__ with @configurable.
 
         Args:
             cfg: A Config node. See ``meddlr/config/defaults.py`` for a complete list of options.
@@ -332,16 +337,17 @@
                 - ``'consistency'``: Data augmentations for consistency training (i.e. VORTEX).
             seed: A random seed to initialize this class.
             device: The device to use for the augmentor.
 
         Returns:
             MRIReconAugmentor: An augmentor.
         """
-        mri_tfm_cfg = None
-        assert aug_kind in ("aug_train", "consistency")
+        assert aug_kind in ("aug_train", "consistency", None)
+
+        mri_tfm_cfg = cfg
         if aug_kind == "aug_train":
             mri_tfm_cfg = cfg.AUG_TRAIN.MRI_RECON
         elif aug_kind == "consistency":
             mri_tfm_cfg = cfg.MODEL.CONSISTENCY.AUG.MRI_RECON
 
         if seed is None and env.is_repro():
             seed = cfg.SEED
```

### Comparing `meddlr-0.0.7rc1/meddlr/transforms/functional/mri.py` & `meddlr-0.0.8a1/meddlr/transforms/functional/mri.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/transforms/gen/choice.py` & `meddlr-0.0.8a1/meddlr/transforms/gen/choice.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/transforms/gen/mask.py` & `meddlr-0.0.8a1/meddlr/transforms/gen/mask.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/transforms/gen/motion.py` & `meddlr-0.0.8a1/meddlr/transforms/gen/motion.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/transforms/gen/noise.py` & `meddlr-0.0.8a1/meddlr/transforms/gen/noise.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/transforms/gen/spatial.py` & `meddlr-0.0.8a1/meddlr/transforms/gen/spatial.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/transforms/mixins.py` & `meddlr-0.0.8a1/meddlr/transforms/mixins.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/transforms/tf_scheduler.py` & `meddlr-0.0.8a1/meddlr/transforms/tf_scheduler.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/transforms/transform.py` & `meddlr-0.0.8a1/meddlr/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/transforms/transform_gen.py` & `meddlr-0.0.8a1/meddlr/transforms/transform_gen.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/utils/cfl.py` & `meddlr-0.0.8a1/meddlr/utils/cfl.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/utils/cluster.py` & `meddlr-0.0.8a1/meddlr/utils/cluster.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/utils/collect_env.py` & `meddlr-0.0.8a1/meddlr/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/utils/comm.py` & `meddlr-0.0.8a1/meddlr/utils/comm.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/utils/deprecated.py` & `meddlr-0.0.8a1/meddlr/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/utils/env.py` & `meddlr-0.0.8a1/meddlr/utils/env.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/utils/events.py` & `meddlr-0.0.8a1/meddlr/utils/events.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/utils/general.py` & `meddlr-0.0.8a1/meddlr/utils/general.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/utils/logger.py` & `meddlr-0.0.8a1/meddlr/utils/logger.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/utils/memory.py` & `meddlr-0.0.8a1/meddlr/utils/memory.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/utils/path.py` & `meddlr-0.0.8a1/meddlr/utils/path.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/utils/profiler.py` & `meddlr-0.0.8a1/meddlr/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/utils/registry.py` & `meddlr-0.0.8a1/meddlr/utils/registry.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr/utils/transforms.py` & `meddlr-0.0.8a1/meddlr/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.7rc1/meddlr.egg-info/PKG-INFO` & `meddlr-0.0.8a1/meddlr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: meddlr
-Version: 0.0.7rc1
+Version: 0.0.8a1
 Summary: Meddlr is a config-driven framework built to simplify ML-based medical image reconstruction and analysis.
 Home-page: https://github.com/ad12/meddlr
 Author: The Meddlr Team
 Author-email: arjundd@stanford.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: benchmarking
@@ -93,9 +91,7 @@
 @article{desai2021noise2recon,
   title={Noise2Recon: A Semi-Supervised Framework for Joint MRI Reconstruction and Denoising},
   author={Desai, Arjun D and Ozturkler, Batu M and Sandino, Christopher M and Vasanawala, Shreyas and Hargreaves, Brian A and Re, Christopher M and Pauly, John M and Chaudhari, Akshay S},
   journal={arXiv preprint arXiv:2110.00075},
   year={2021}
 }
 ```
-
-
```

### Comparing `meddlr-0.0.7rc1/meddlr.egg-info/SOURCES.txt` & `meddlr-0.0.8a1/meddlr.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 meddlr/modeling/meta_arch/unet.py
 meddlr/modeling/meta_arch/unrolled.py
 meddlr/modeling/meta_arch/vortex.py
 meddlr/ops/__init__.py
 meddlr/ops/categorical.py
 meddlr/ops/complex.py
 meddlr/ops/fft.py
+meddlr/ops/opt.py
 meddlr/ops/utils.py
 meddlr/solver/__init__.py
 meddlr/solver/build.py
 meddlr/solver/lr_scheduler.py
 meddlr/solver/optimizer.py
 meddlr/transforms/__init__.py
 meddlr/transforms/build.py
@@ -126,8 +127,10 @@
 meddlr/utils/events.py
 meddlr/utils/general.py
 meddlr/utils/logger.py
 meddlr/utils/memory.py
 meddlr/utils/path.py
 meddlr/utils/profiler.py
 meddlr/utils/registry.py
-meddlr/utils/transforms.py
+meddlr/utils/transforms.py
+tests/test_experiments.py
+tests/test_reproducibility.py
```

### Comparing `meddlr-0.0.7rc1/meddlr.egg-info/requires.txt` & `meddlr-0.0.8a1/meddlr.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -13,63 +13,65 @@
 tqdm
 omegaconf
 torchmetrics>=0.5.1
 iopath
 packaging
 
 [all]
-requests
 medpy
-monai
+requests
+gdown<4.6.0
 lpips
+monai
 iocursor
-gdown<4.6.0
 
 [alldev]
-m2r2
-tifffile<=2022.5.4
-flake8-comprehensions
-monai
-flake8-bugbear
-sphinx-rtd-theme
-coverage
-lpips
-gdown<4.6.0
 medpy
 parameterized
-isort
-iocursor
-black==22.3.0
-requests
-pytest
-sphinx
-flake8
+monai
+sphinx-rtd-theme
+m2r2
+black==22.12.0
 pooch
+flake8-bugbear
 pre-commit>=2.9.3
+coverage
+wrapt
 sphinxcontrib-bibtex
 sphinxcontrib.bibtex
+flake8
+gdown<4.6.0
+requests
+lpips
+tifffile<=2022.5.4
+flake8-comprehensions
+sphinx
+iocursor
+pytest
+isort
 
 [benchmarking]
 medpy
 
 [deployment]
 gdown<4.6.0
 requests
 iocursor
 
 [dev]
 coverage
 flake8
 isort
-black==22.3.0
+black==22.12.0
 flake8-bugbear
 flake8-comprehensions
 pre-commit>=2.9.3
 pytest
 medpy
+wrapt
 pooch
 gdown<4.6.0
 parameterized
 tifffile<=2022.5.4
 sphinx
 sphinxcontrib-bibtex
 sphinx-rtd-theme
```

### Comparing `meddlr-0.0.7rc1/setup.cfg` & `meddlr-0.0.8a1/setup.cfg`

 * *Files identical despite different names*


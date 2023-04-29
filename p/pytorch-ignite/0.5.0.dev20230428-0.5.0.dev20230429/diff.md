# Comparing `tmp/pytorch-ignite-0.5.0.dev20230428.tar.gz` & `tmp/pytorch-ignite-0.5.0.dev20230429.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-ignite-0.5.0.dev20230428.tar", last modified: Fri Apr 28 00:15:39 2023, max compression
+gzip compressed data, was "pytorch-ignite-0.5.0.dev20230429.tar", last modified: Sat Apr 29 00:14:37 2023, max compression
```

## Comparing `pytorch-ignite-0.5.0.dev20230428.tar` & `pytorch-ignite-0.5.0.dev20230429.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.917848 pytorch-ignite-0.5.0.dev20230428/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28334 2023-04-28 00:15:39.917848 pytorch-ignite-0.5.0.dev20230428/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27890 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.901848 pytorch-ignite-0.5.0.dev20230428/ignite/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-28 00:11:11.000000 pytorch-ignite-0.5.0.dev20230428/ignite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.901848 pytorch-ignite-0.5.0.dev20230428/ignite/base/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/base/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.901848 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.901848 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/engines/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28589 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/engines/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/engines/tbptt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.905848 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    37623 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/clearml_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12349 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    27455 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/neptune_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/polyaxon_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/time_profilers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/tqdm_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    21622 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/visdom_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.905848 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/gpu_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/precision_recall_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.909848 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/canberra_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/fractional_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/fractional_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/manhattan_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/maximum_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/mean_absolute_relative_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/mean_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/mean_normalized_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/median_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/median_absolute_percentage_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/median_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/r2_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/wave_hedges_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/roc_auc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.909848 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15409 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.909848 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    26285 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/xla.py
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    22377 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/distributed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.909848 pytorch-ignite-0.5.0.dev20230428/ignite/engine/
--rw-r--r--   0 runner    (1001) docker     (123)    32766 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/engine/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)    54830 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    21213 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/engine/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/engine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.913848 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44800 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/ema_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    21757 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    62888 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20747 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/state_param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/terminate_on_nan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)    30228 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/time_profilers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/handlers/timing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.917848 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/accumulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/classification_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/epoch_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/fbeta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/frequency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.917848 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/gan/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/gan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/gan/fid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/gan/inception_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/gan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/mean_pairwise_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    24270 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/metrics_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/multilabel_confusion_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.917848 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/nlp/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/nlp/rouge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/nlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17066 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/psnr.py
--rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/recall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/root_mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/running_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/ssim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/metrics/top_k_categorical_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/ignite/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:39.917848 pytorch-ignite-0.5.0.dev20230428/pytorch_ignite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28334 2023-04-28 00:15:39.000000 pytorch-ignite-0.5.0.dev20230428/pytorch_ignite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-04-28 00:15:39.000000 pytorch-ignite-0.5.0.dev20230428/pytorch_ignite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:15:39.000000 pytorch-ignite-0.5.0.dev20230428/pytorch_ignite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:15:39.000000 pytorch-ignite-0.5.0.dev20230428/pytorch_ignite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 00:15:39.000000 pytorch-ignite-0.5.0.dev20230428/pytorch_ignite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 00:15:39.000000 pytorch-ignite-0.5.0.dev20230428/pytorch_ignite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-28 00:15:39.921848 pytorch-ignite-0.5.0.dev20230428/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-28 00:10:35.000000 pytorch-ignite-0.5.0.dev20230428/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:37.306777 pytorch-ignite-0.5.0.dev20230429/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28334 2023-04-29 00:14:37.306777 pytorch-ignite-0.5.0.dev20230429/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27890 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:37.286776 pytorch-ignite-0.5.0.dev20230429/ignite/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-29 00:10:09.000000 pytorch-ignite-0.5.0.dev20230429/ignite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:37.286776 pytorch-ignite-0.5.0.dev20230429/ignite/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/base/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:37.286776 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:37.286776 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28587 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/engines/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/engines/tbptt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:37.290776 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37618 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/clearml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27453 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/neptune_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/polyaxon_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/time_profilers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/tqdm_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21620 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/visdom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:37.290776 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/gpu_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/precision_recall_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:37.294776 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/canberra_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/fractional_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/fractional_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/manhattan_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/maximum_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/mean_absolute_relative_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/mean_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/mean_normalized_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/median_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/median_absolute_percentage_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/median_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/r2_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/wave_hedges_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/roc_auc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:37.294776 pytorch-ignite-0.5.0.dev20230429/ignite/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/distributed/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:37.294776 pytorch-ignite-0.5.0.dev20230429/ignite/distributed/comp_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/distributed/comp_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/distributed/comp_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/distributed/comp_models/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26281 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/distributed/comp_models/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/distributed/comp_models/xla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/distributed/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22377 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/distributed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:37.298776 pytorch-ignite-0.5.0.dev20230429/ignite/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)    32766 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/engine/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54830 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21213 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/engine/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/engine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:37.298776 pytorch-ignite-0.5.0.dev20230429/ignite/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44795 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/handlers/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/handlers/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/handlers/ema_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21756 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/handlers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62884 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/handlers/param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/handlers/state_param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/handlers/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/handlers/terminate_on_nan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/handlers/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30228 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/handlers/time_profilers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/handlers/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:37.302776 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/classification_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17638 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/epoch_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/fbeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/frequency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:37.302776 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/gan/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/gan/fid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/gan/inception_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/gan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/mean_pairwise_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24266 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/metrics_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/multilabel_confusion_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:37.302776 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/nlp/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/nlp/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/nlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17059 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/recall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/root_mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/running_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/metrics/top_k_categorical_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/ignite/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:14:37.306777 pytorch-ignite-0.5.0.dev20230429/pytorch_ignite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28334 2023-04-29 00:14:37.000000 pytorch-ignite-0.5.0.dev20230429/pytorch_ignite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-04-29 00:14:37.000000 pytorch-ignite-0.5.0.dev20230429/pytorch_ignite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:14:37.000000 pytorch-ignite-0.5.0.dev20230429/pytorch_ignite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:14:37.000000 pytorch-ignite-0.5.0.dev20230429/pytorch_ignite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-29 00:14:37.000000 pytorch-ignite-0.5.0.dev20230429/pytorch_ignite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 00:14:37.000000 pytorch-ignite-0.5.0.dev20230429/pytorch_ignite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-29 00:14:37.306777 pytorch-ignite-0.5.0.dev20230429/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-29 00:09:37.000000 pytorch-ignite-0.5.0.dev20230429/setup.py
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/LICENSE` & `pytorch-ignite-0.5.0.dev20230429/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/PKG-INFO` & `pytorch-ignite-0.5.0.dev20230429/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-ignite
-Version: 0.5.0.dev20230428
+Version: 0.5.0.dev20230429
 Summary: A lightweight library to help with training neural networks in PyTorch.
 Home-page: https://github.com/pytorch/ignite
 Author: PyTorch Core Team
 Author-email: soumith@pytorch.org
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/README.md` & `pytorch-ignite-0.5.0.dev20230429/README.md`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/base/mixins.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/base/mixins.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from collections import OrderedDict
 from collections.abc import Mapping
 from typing import Tuple
 
 
 class Serializable:
-
     _state_dict_all_req_keys: Tuple = ()
     _state_dict_one_of_opt_keys: Tuple = ()
 
     def state_dict(self) -> OrderedDict:
         raise NotImplementedError
 
     def load_state_dict(self, state_dict: Mapping) -> None:
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/engines/common.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/engines/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,14 @@
         else:
             trainer.add_event_handler(Events.ITERATION_STARTED, lr_scheduler)
 
     if torch.cuda.is_available() and clear_cuda_cache:
         trainer.add_event_handler(Events.EPOCH_COMPLETED, empty_cuda_cache)
 
     if to_save is not None:
-
         if output_path is None and save_handler is None:
             raise ValueError(
                 "If to_save argument is provided then output_path or save_handler arguments should be also defined"
             )
         if output_path is not None:
             save_handler = DiskSaver(dirname=output_path, require_empty=False)
 
@@ -238,15 +237,14 @@
     with_pbar_on_iters: bool = True,
     log_every_iters: int = 100,
     stop_on_nan: bool = True,
     clear_cuda_cache: bool = True,
     save_handler: Optional[Union[Callable, BaseSaveHandler]] = None,
     **kwargs: Any,
 ) -> None:
-
     _setup_common_training_handlers(
         trainer,
         to_save=to_save,
         output_path=output_path,
         save_every_iters=save_every_iters,
         lr_scheduler=lr_scheduler,
         with_gpu_stats=with_gpu_stats,
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/engines/tbptt.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/engines/tbptt.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/__init__.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/base_logger.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/base_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,32 +28,28 @@
 
     def __init__(
         self,
         model: nn.Module,
         tag: Optional[str] = None,
         whitelist: Optional[Union[List[str], Callable[[str, nn.Parameter], bool]]] = None,
     ):
-
         if not isinstance(model, torch.nn.Module):
             raise TypeError(f"Argument model should be of type torch.nn.Module, but given {type(model)}")
 
         self.model = model
         self.tag = tag
 
         weights = {}
         if whitelist is None:
-
             weights = dict(model.named_parameters())
         elif callable(whitelist):
-
             for n, p in model.named_parameters():
                 if whitelist(n, p):
                     weights[n] = p
         else:
-
             for n, p in model.named_parameters():
                 for item in whitelist:
                     if n.startswith(item):
                         weights[n] = p
 
         self.weights = weights.items()
 
@@ -87,15 +83,14 @@
         self,
         tag: str,
         metric_names: Optional[Union[str, List[str]]] = None,
         output_transform: Optional[Callable] = None,
         global_step_transform: Optional[Callable[[Engine, Union[str, Events]], int]] = None,
         state_attributes: Optional[List[str]] = None,
     ):
-
         if metric_names is not None:
             if not (isinstance(metric_names, list) or (isinstance(metric_names, str) and metric_names == "all")):
                 raise TypeError(
                     f"metric_names should be either a list or equal 'all', got {type(metric_names)} instead."
                 )
 
         if output_transform is not None and not callable(output_transform):
@@ -181,15 +176,14 @@
     def __init__(
         self,
         model: nn.Module,
         reduction: Callable[[torch.Tensor], Union[float, torch.Tensor]] = torch.norm,
         tag: Optional[str] = None,
         whitelist: Optional[Union[List[str], Callable[[str, nn.Parameter], bool]]] = None,
     ):
-
         super(BaseWeightsScalarHandler, self).__init__(model, tag=tag, whitelist=whitelist)
 
         if not callable(reduction):
             raise TypeError(f"Argument reduction should be callable, but given {type(reduction)}")
 
         def _is_0D_tensor(t: Any) -> bool:
             return isinstance(t, torch.Tensor) and t.ndimension() == 0
@@ -235,15 +229,14 @@
                 if name not in State.event_to_attr:
                     raise RuntimeError(f"Unknown event name '{name}'")
                 engine.add_event_handler(name, log_handler, self, name)
 
             return RemovableEventHandle(event_name, log_handler, engine)
 
         else:
-
             if event_name not in State.event_to_attr:
                 raise RuntimeError(f"Unknown event name '{event_name}'")
 
             return engine.add_event_handler(event_name, log_handler, self, event_name, *args, **kwargs)
 
     def attach_output_handler(self, engine: Engine, event_name: Any, *args: Any, **kwargs: Any) -> RemovableEventHandle:
         """Shortcut method to attach `OutputHandler` to the logger.
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/clearml_logger.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/clearml_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,14 @@
         state_attributes: Optional[List[str]] = None,
     ):
         super(OutputHandler, self).__init__(
             tag, metric_names, output_transform, global_step_transform, state_attributes
         )
 
     def __call__(self, engine: Engine, logger: ClearMLLogger, event_name: Union[str, Events]) -> None:
-
         if not isinstance(logger, ClearMLLogger):
             raise RuntimeError("Handler OutputHandler works only with ClearMLLogger")
 
         metrics = self._setup_output_metrics_state_attrs(engine)
 
         global_step = self.global_step_transform(engine, event_name)
 
@@ -477,22 +476,20 @@
             )
 
     ..  versionchanged:: 0.4.9
         optional argument `whitelist` added.
     """
 
     def __call__(self, engine: Engine, logger: ClearMLLogger, event_name: Union[str, Events]) -> None:
-
         if not isinstance(logger, ClearMLLogger):
             raise RuntimeError("Handler WeightsScalarHandler works only with ClearMLLogger")
 
         global_step = engine.state.get_event_attrib_value(event_name)
         tag_prefix = f"{self.tag}/" if self.tag else ""
         for name, p in self.weights:
-
             title_name, _, series_name = name.partition(".")
             logger.clearml_logger.report_scalar(
                 title=f"{tag_prefix}weights_{self.reduction.__name__}/{title_name}",
                 series=series_name,
                 value=self.reduction(p.data),
                 iteration=global_step,
             )
@@ -575,15 +572,14 @@
     def __call__(self, engine: Engine, logger: ClearMLLogger, event_name: Union[str, Events]) -> None:
         if not isinstance(logger, ClearMLLogger):
             raise RuntimeError("Handler 'WeightsHistHandler' works only with ClearMLLogger")
 
         global_step = engine.state.get_event_attrib_value(event_name)
         tag_prefix = f"{self.tag}/" if self.tag else ""
         for name, p in self.weights:
-
             title_name, _, series_name = name.partition(".")
 
             logger.grad_helper.add_histogram(
                 title=f"{tag_prefix}weights_{title_name}",
                 series=series_name,
                 step=global_step,
                 hist_data=p.data.cpu().numpy(),
@@ -822,15 +818,14 @@
         self,
         logger: Optional[ClearMLLogger] = None,
         output_uri: Optional[str] = None,
         dirname: Optional[str] = None,
         *args: Any,
         **kwargs: Any,
     ):
-
         self._setup_check_clearml(logger, output_uri)
 
         if not dirname:
             dirname = ""
             if idist.get_rank() == 0:
                 dirname = tempfile.mkdtemp(prefix=f"ignite_checkpoints_{datetime.now().strftime('%Y_%m_%d_%H_%M_%S_')}")
             if idist.get_world_size() > 1:
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/lr_finder.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/mlflow_logger.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/mlflow_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,14 @@
             mlflow.set_tracking_uri(tracking_uri)
 
         self.active_run = mlflow.active_run()
         if self.active_run is None:
             self.active_run = mlflow.start_run()
 
     def __getattr__(self, attr: Any) -> Any:
-
         import mlflow
 
         return getattr(mlflow, attr)
 
     def close(self) -> None:
         import mlflow
 
@@ -226,15 +225,14 @@
         state_attributes: Optional[List[str]] = None,
     ) -> None:
         super(OutputHandler, self).__init__(
             tag, metric_names, output_transform, global_step_transform, state_attributes
         )
 
     def __call__(self, engine: Engine, logger: MLflowLogger, event_name: Union[str, Events]) -> None:
-
         if not isinstance(logger, MLflowLogger):
             raise TypeError("Handler 'OutputHandler' works only with MLflowLogger")
 
         rendered_metrics = self._setup_output_metrics_state_attrs(engine)
 
         global_step = self.global_step_transform(engine, event_name)
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/neptune_logger.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/neptune_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,14 @@
         state_attributes: Optional[List[str]] = None,
     ):
         super(OutputHandler, self).__init__(
             tag, metric_names, output_transform, global_step_transform, state_attributes
         )
 
     def __call__(self, engine: Engine, logger: NeptuneLogger, event_name: Union[str, Events]) -> None:
-
         if not isinstance(logger, NeptuneLogger):
             raise TypeError("Handler OutputHandler works only with NeptuneLogger")
 
         metrics = self._setup_output_metrics_state_attrs(engine, key_tuple=False)
 
         global_step = self.global_step_transform(engine, event_name)
 
@@ -487,15 +486,14 @@
             )
 
     ..  versionchanged:: 0.4.9
         optional argument `whitelist` added.
     """
 
     def __call__(self, engine: Engine, logger: NeptuneLogger, event_name: Union[str, Events]) -> None:
-
         if not isinstance(logger, NeptuneLogger):
             raise TypeError("Handler WeightsScalarHandler works only with NeptuneLogger")
 
         global_step = engine.state.get_event_attrib_value(event_name)
         tag_prefix = f"{self.tag}/" if self.tag else ""
         for name, p in self.weights:
             if p.grad is None:
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/param_scheduler.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/polyaxon_logger.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/polyaxon_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,14 @@
         state_attributes: Optional[List[str]] = None,
     ):
         super(OutputHandler, self).__init__(
             tag, metric_names, output_transform, global_step_transform, state_attributes
         )
 
     def __call__(self, engine: Engine, logger: PolyaxonLogger, event_name: Union[str, Events]) -> None:
-
         if not isinstance(logger, PolyaxonLogger):
             raise RuntimeError("Handler 'OutputHandler' works only with PolyaxonLogger")
 
         metrics = self._setup_output_metrics_state_attrs(engine, key_tuple=False)
 
         global_step = self.global_step_transform(engine, event_name)
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/tensorboard_logger.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/tensorboard_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,14 @@
         state_attributes: Optional[List[str]] = None,
     ):
         super(OutputHandler, self).__init__(
             tag, metric_names, output_transform, global_step_transform, state_attributes
         )
 
     def __call__(self, engine: Engine, logger: TensorboardLogger, event_name: Union[str, Events]) -> None:
-
         if not isinstance(logger, TensorboardLogger):
             raise RuntimeError("Handler 'OutputHandler' works only with TensorboardLogger")
 
         metrics = self._setup_output_metrics_state_attrs(engine, key_tuple=False)
 
         global_step = self.global_step_transform(engine, event_name)
         if not isinstance(global_step, int):
@@ -418,22 +417,20 @@
             )
 
     ..  versionchanged:: 0.4.9
         optional argument `whitelist` added.
     """
 
     def __call__(self, engine: Engine, logger: TensorboardLogger, event_name: Union[str, Events]) -> None:
-
         if not isinstance(logger, TensorboardLogger):
             raise RuntimeError("Handler 'WeightsScalarHandler' works only with TensorboardLogger")
 
         global_step = engine.state.get_event_attrib_value(event_name)
         tag_prefix = f"{self.tag}/" if self.tag else ""
         for name, p in self.weights:
-
             name = name.replace(".", "/")
             logger.writer.add_scalar(
                 f"{tag_prefix}weights_{self.reduction.__name__}/{name}",
                 self.reduction(p.data),
                 global_step,
             )
 
@@ -505,15 +502,14 @@
     def __call__(self, engine: Engine, logger: TensorboardLogger, event_name: Union[str, Events]) -> None:
         if not isinstance(logger, TensorboardLogger):
             raise RuntimeError("Handler 'WeightsHistHandler' works only with TensorboardLogger")
 
         global_step = engine.state.get_event_attrib_value(event_name)
         tag_prefix = f"{self.tag}/" if self.tag else ""
         for name, p in self.weights:
-
             name = name.replace(".", "/")
             logger.writer.add_histogram(
                 tag=f"{tag_prefix}weights/{name}", values=p.data.cpu().numpy(), global_step=global_step
             )
 
 
 class GradsScalarHandler(BaseWeightsScalarHandler):
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/time_profilers.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/time_profilers.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/tqdm_logger.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/tqdm_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,14 @@
         self,
         persist: bool = False,
         bar_format: Union[
             str, None
         ] = "{desc}[{n_fmt}/{total_fmt}] {percentage:3.0f}%|{bar}{postfix} [{elapsed}<{remaining}]",
         **tqdm_kwargs: Any,
     ):
-
         try:
             from tqdm.autonotebook import tqdm
         except ImportError:
             raise ModuleNotFoundError(
                 "This contrib module requires tqdm to be installed. "
                 "Please install it with command: \n pip install tqdm"
             )
@@ -277,15 +276,14 @@
         if event_name in (Events.ITERATION_STARTED, Events.ITERATION_COMPLETED):
             return engine.state.epoch_length
         if event_name in (Events.EPOCH_STARTED, Events.EPOCH_COMPLETED):
             return engine.state.max_epochs
         return 1
 
     def __call__(self, engine: Engine, logger: ProgressBar, event_name: Union[str, Events]) -> None:
-
         pbar_total = self.get_max_number_events(event_name, engine)
         if logger.pbar is None:
             logger._reset(pbar_total=pbar_total)
 
         max_epochs = engine.state.max_epochs
         default_desc = "Iteration" if max_epochs == 1 else "Epoch"
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/visdom_logger.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/visdom_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,15 +360,14 @@
     ):
         super(OutputHandler, self).__init__(
             tag, metric_names, output_transform, global_step_transform, state_attributes
         )
         _BaseVisDrawer.__init__(self, show_legend=show_legend)
 
     def __call__(self, engine: Engine, logger: VisdomLogger, event_name: Union[str, Events]) -> None:
-
         if not isinstance(logger, VisdomLogger):
             raise RuntimeError("Handler 'OutputHandler' works only with VisdomLogger")
 
         metrics = self._setup_output_metrics_state_attrs(engine, key_tuple=False)
 
         global_step = self.global_step_transform(engine, event_name)
 
@@ -469,15 +468,14 @@
     def __init__(
         self, model: nn.Module, reduction: Callable = torch.norm, tag: Optional[str] = None, show_legend: bool = False
     ):
         super(WeightsScalarHandler, self).__init__(model, reduction, tag=tag)
         _BaseVisDrawer.__init__(self, show_legend=show_legend)
 
     def __call__(self, engine: Engine, logger: VisdomLogger, event_name: Union[str, Events]) -> None:
-
         if not isinstance(logger, VisdomLogger):
             raise RuntimeError("Handler 'WeightsScalarHandler' works only with VisdomLogger")
 
         global_step = engine.state.get_event_attrib_value(event_name)
         tag_prefix = f"{self.tag}/" if self.tag else ""
         for name, p in self.model.named_parameters():
             name = name.replace(".", "/")
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/handlers/wandb_logger.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/handlers/wandb_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,14 @@
         sync: Optional[bool] = None,
         state_attributes: Optional[List[str]] = None,
     ):
         super().__init__(tag, metric_names, output_transform, global_step_transform, state_attributes)
         self.sync = sync
 
     def __call__(self, engine: Engine, logger: WandBLogger, event_name: Union[str, Events]) -> None:
-
         if not isinstance(logger, WandBLogger):
             raise RuntimeError(f"Handler '{self.__class__.__name__}' works only with WandBLogger.")
 
         global_step = self.global_step_transform(engine, event_name)
         if not isinstance(global_step, int):
             raise TypeError(
                 f"global_step must be int, got {type(global_step)}."
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/average_precision.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/average_precision.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 
     def __init__(
         self,
         output_transform: Callable = lambda x: x,
         check_compute_fn: bool = False,
         device: Union[str, torch.device] = torch.device("cpu"),
     ):
-
         try:
             from sklearn.metrics import average_precision_score  # noqa: F401
         except ImportError:
             raise ModuleNotFoundError("This contrib module requires scikit-learn to be installed.")
 
         super(AveragePrecision, self).__init__(
             average_precision_compute_fn,
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/cohen_kappa.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/cohen_kappa.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     def __init__(
         self,
         output_transform: Callable = lambda x: x,
         weights: Optional[str] = None,
         check_compute_fn: bool = False,
         device: Union[str, torch.device] = torch.device("cpu"),
     ):
-
         try:
             from sklearn.metrics import cohen_kappa_score  # noqa: F401
         except ImportError:
             raise ModuleNotFoundError("This contrib module requires scikit-learn to be installed.")
         if weights not in (None, "linear", "quadratic"):
             raise ValueError("Kappa Weighting type must be None or linear or quadratic.")
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/gpu_info.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/gpu_info.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/precision_recall_curve.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/__init__.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/_base.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/_base.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/canberra_metric.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/canberra_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/fractional_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/fractional_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/fractional_bias.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/fractional_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/manhattan_distance.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/manhattan_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/maximum_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/maximum_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/mean_absolute_relative_error.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/mean_absolute_relative_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/mean_error.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/mean_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/mean_normalized_bias.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/mean_normalized_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/median_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/median_absolute_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,11 +63,10 @@
 
             0.625
     """
 
     def __init__(
         self, output_transform: Callable = lambda x: x, device: Union[str, torch.device] = torch.device("cpu")
     ):
-
         super(MedianAbsoluteError, self).__init__(
             median_absolute_error_compute_fn, output_transform=output_transform, device=device
         )
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/median_absolute_percentage_error.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/median_absolute_percentage_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/median_relative_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/median_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/r2_score.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/regression/wave_hedges_distance.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/regression/wave_hedges_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/contrib/metrics/roc_auc.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/contrib/metrics/roc_auc.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,14 @@
 
     def __init__(
         self,
         output_transform: Callable = lambda x: x,
         check_compute_fn: bool = False,
         device: Union[str, torch.device] = torch.device("cpu"),
     ):
-
         try:
             from sklearn.metrics import roc_auc_score  # noqa: F401
         except ImportError:
             raise ModuleNotFoundError("This contrib module requires scikit-learn to be installed.")
 
         super(ROC_AUC, self).__init__(
             roc_auc_compute_fn, output_transform=output_transform, check_compute_fn=check_compute_fn, device=device
@@ -148,15 +147,14 @@
 
     def __init__(
         self,
         output_transform: Callable = lambda x: x,
         check_compute_fn: bool = False,
         device: Union[str, torch.device] = torch.device("cpu"),
     ) -> None:
-
         try:
             from sklearn.metrics import roc_curve  # noqa: F401
         except ImportError:
             raise ModuleNotFoundError("This contrib module requires scikit-learn to be installed.")
 
         super(RocCurve, self).__init__(
             roc_auc_curve_compute_fn,  # type: ignore[arg-type]
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/distributed/auto.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/distributed/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,14 @@
     else:
         kwargs["pin_memory"] = kwargs.get("pin_memory", "cuda" in idist.device().type)
 
     logger.info(f"Use data loader kwargs for dataset '{repr(dataset)[:20].strip()}': \n\t{kwargs}")
     dataloader = DataLoader(dataset, **kwargs)
 
     if idist.has_xla_support and idist.backend() == idist_xla.XLA_TPU and world_size > 1:
-
         logger.info("DataLoader is wrapped by `MpDeviceLoader` on XLA")
 
         mp_device_loader_cls = _MpDeviceLoader
         try:
             from torch_xla.distributed.parallel_loader import MpDeviceLoader
 
             mp_device_loader_cls = MpDeviceLoader
@@ -290,15 +289,14 @@
         rank: Rank of the current process within ``num_replicas``.
 
     .. note::
         Input sampler is assumed to have a constant size.
     """
 
     def __init__(self, sampler: Sampler, num_replicas: Optional[int] = None, rank: Optional[int] = None) -> None:
-
         if not isinstance(sampler, Sampler):
             raise TypeError(f"Argument sampler should be instance of torch Sampler, but given: {type(sampler)}")
 
         if isinstance(sampler, DistributedSampler):
             raise TypeError("Argument sampler must not be a distributed sampler already")
 
         if not hasattr(sampler, "__len__"):
@@ -325,15 +323,14 @@
         if len(indices) != self.num_samples:
             raise RuntimeError(f"{len(indices)} vs {self.num_samples}")
 
         return iter(indices)
 
 
 if idist.has_xla_support:
-
     import torch_xla.core.xla_model as xm
     from torch_xla.distributed.parallel_loader import ParallelLoader
 
     class _MpDeviceLoader:
         # https://github.com/pytorch/xla/pull/2117
         # From pytorch/xla if `torch_xla.distributed.parallel_loader.MpDeviceLoader` is not available
         def __init__(self, loader: Any, device: torch.device, **kwargs: Any) -> None:
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/__init__.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/distributed/comp_models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 if TYPE_CHECKING:
     from ignite.distributed.comp_models.horovod import _HorovodDistModel
     from ignite.distributed.comp_models.native import _NativeDistModel
     from ignite.distributed.comp_models.xla import _XlaDistModel
 
 
-def setup_available_computation_models() -> Tuple[
-    Type[Union[_SerialModel, "_NativeDistModel", "_XlaDistModel", "_HorovodDistModel"]], ...
-]:
+def setup_available_computation_models() -> (
+    Tuple[Type[Union[_SerialModel, "_NativeDistModel", "_XlaDistModel", "_HorovodDistModel"]], ...]
+):
     models: List[Type[Union[_SerialModel, "_NativeDistModel", "_XlaDistModel", "_HorovodDistModel"]]] = [
         _SerialModel,
     ]
     if has_native_dist_support:
         from ignite.distributed.comp_models.native import _NativeDistModel
 
         models.append(_NativeDistModel)
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/base.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/distributed/comp_models/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,14 @@
             return ""
         else:
             raise RuntimeError(f"Internal error: unhandled dtype {encoded_msg[0]}, encoded_msg={encoded_msg}")
 
     def _setup_placeholder(
         self, x: Union[torch.Tensor, float, str, None], device: torch.device, is_src: bool
     ) -> Union[torch.Tensor, float, str]:
-
         encoded_msg_per_rank = self._encode_input_data(x, is_src)
         encoded_msg_all_ranks = self._do_all_reduce(torch.tensor(encoded_msg_per_rank, device=device), op="MAX")
 
         if is_src:
             if x is None:
                 raise RuntimeError("Internal error, x is None. Please, file an issue if you encounter this error.")
             return x
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/horovod.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/distributed/comp_models/horovod.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
     has_hvd_support = True
 except ImportError:
     has_hvd_support = False
 
 
 if has_hvd_support:
-
     HOROVOD = "horovod"
 
     class _HorovodDistModel(ComputationModel):
         """Private class for `Horovod <https://horovod.readthedocs.io/en/stable/>`_ distributed computation model."""
 
         name = "horovod-dist"
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/native.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/distributed/comp_models/native.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 from ignite.distributed.comp_models.base import ComputationModel
 
 has_native_dist_support = dist.is_available()
 
 
 if has_native_dist_support:
-
     NCCL = dist.Backend.NCCL
     GLOO = dist.Backend.GLOO
     MPI = dist.Backend.MPI
 
     class _NativeDistModel(ComputationModel):
         """Private class for PyTorch native distributed computation model.
 
@@ -192,15 +191,14 @@
                 raise ValueError(
                     "Failed to correctly estimate local rank. "
                     f"Debugging info: local rank: {local_rank}, node rank: {self._node}, hostnames: {hostnames}"
                 )
             return local_rank
 
         def _identify_local_rank(self) -> None:
-
             if "SLURM_JOB_ID" in os.environ:
                 os.environ["LOCAL_RANK"] = os.environ["SLURM_LOCALID"]
 
             if "LOCAL_RANK" in os.environ:
                 self._local_rank = int(os.environ["LOCAL_RANK"])
             elif self._ext_local_rank is not None:
                 self._local_rank = self._ext_local_rank
@@ -212,15 +210,14 @@
                     "please either set `os.environ['LOCAL_RANK']` "
                     "or use `idist.set_local_rank(local_rank)` with correct local rank index."
                 )
                 # use socket gethostname heuristic to determine number of nodes => local rank
                 self._local_rank = self._compute_local_rank_via_hostname()
 
         def setup_env_vars(self, rank: Optional[int] = None, world_size: Optional[int] = None) -> None:
-
             self._env_backup = os.environ.copy()
 
             if "SLURM_JOB_ID" in os.environ:
                 if rank is not None or world_size is not None:
                     raise ValueError("Arguments rank and world_size should not be specified with SLURM")
                 self._setup_env_in_slurm()
             else:
@@ -471,15 +468,14 @@
         result_hostlist = []
 
         nodelist_match = r"([^,\[\]]+\[[^\[\]]*\][^,\[\]]*|[^,\[\]]*),?"
 
         nodelist = nodelist.replace(" ", "")
 
         for node in re.findall(nodelist_match, nodelist):
-
             node_match = r"(.+)\[((,?[0-9]+-?,?-?){0,})\](.*)?"
 
             match = re.search(node_match, node)
 
             if match is None:
                 if node:
                     result_hostlist.append(node)
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/distributed/comp_models/xla.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/distributed/comp_models/xla.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
     has_xla_support = True
 except ImportError:
     has_xla_support = False
 
 
 if has_xla_support:
-
     XLA_TPU = "xla-tpu"
 
     class _XlaDistModel(ComputationModel):
         """Private class for PyTorch XLA basic distributed computation model.
         It handles single/multi-device computation model.
 
         Supported XLA devices:
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/distributed/launcher.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/distributed/launcher.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/distributed/utils.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/engine/__init__.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/engine/deterministic.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/engine/deterministic.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/engine/engine.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/engine/engine.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/engine/events.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/engine/events.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/engine/utils.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/engine/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/__init__.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/checkpoint.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/handlers/checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,15 +289,14 @@
         n_saved: Union[int, None] = 1,
         global_step_transform: Optional[Callable] = None,
         filename_pattern: Optional[str] = None,
         include_self: bool = False,
         greater_or_equal: bool = False,
         save_on_rank: int = 0,
     ):
-
         if not isinstance(to_save, collections.Mapping):
             raise TypeError(f"Argument `to_save` should be a dictionary, but given {type(to_save)}")
 
         self._check_objects(to_save, "state_dict")
 
         if include_self:
             if not isinstance(to_save, collections.MutableMapping):
@@ -397,30 +396,28 @@
     def _compare_fn(self, new: Union[int, float]) -> bool:
         if self.greater_or_equal:
             return new >= self._saved[0].priority
         else:
             return new > self._saved[0].priority
 
     def __call__(self, engine: Engine) -> None:
-
         global_step = None
         if self.global_step_transform is not None:
             global_step = self.global_step_transform(engine, engine.last_event_name)
 
         if self.score_function is not None:
             priority = self.score_function(engine)
             if not isinstance(priority, numbers.Number):
                 raise ValueError("Output of score_function should be a number")
         else:
             if global_step is None:
                 global_step = engine.state.get_event_attrib_value(Events.ITERATION_COMPLETED)
             priority = global_step
 
         if self._check_lt_n_saved() or self._compare_fn(priority):
-
             priority_str = f"{priority}" if isinstance(priority, numbers.Integral) else f"{priority:.4f}"
 
             checkpoint = self._setup_checkpoint()
 
             name = "checkpoint"
             if len(checkpoint) == 1:
                 for k in checkpoint:
@@ -961,15 +958,14 @@
         global_step_transform: Optional[Callable] = None,
         filename_pattern: Optional[str] = None,
         include_self: bool = False,
         greater_or_equal: bool = False,
         save_on_rank: int = 0,
         **kwargs: Any,
     ):
-
         disk_saver = DiskSaver(
             dirname,
             atomic=atomic,
             create_dir=create_dir,
             require_empty=require_empty,
             save_on_rank=save_on_rank,
             **kwargs,
@@ -996,14 +992,13 @@
 
         if not isinstance(self.save_handler, DiskSaver):
             raise RuntimeError(f"Internal error, save_handler should be DiskSaver, but has {type(self.save_handler)}.")
 
         return self.save_handler.dirname / self._saved[-1].filename
 
     def __call__(self, engine: Engine, to_save: Mapping):  # type: ignore
-
         if len(to_save) == 0:
             raise RuntimeError("No objects to checkpoint found.")
 
         self._check_objects(to_save, "state_dict")
         self.to_save = to_save
         super(ModelCheckpoint, self).__call__(engine)
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/early_stopping.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/handlers/early_stopping.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         self,
         patience: int,
         score_function: Callable,
         trainer: Engine,
         min_delta: float = 0.0,
         cumulative_delta: bool = False,
     ):
-
         if not callable(score_function):
             raise TypeError("Argument score_function should be a function.")
 
         if patience < 1:
             raise ValueError("Argument patience should be positive integer.")
 
         if min_delta < 0.0:
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/ema_handler.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/handlers/ema_handler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/lr_finder.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/handlers/lr_finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,14 @@
         num_iter: int,
         start_lrs: List[float],
         end_lrs: List[float],
         step_mode: str,
         smooth_f: float,
         diverge_th: float,
     ) -> None:
-
         self._history = {"lr": [], "loss": []}
         self._best_loss = None
         self._diverge_flag = False
 
         # attach LRScheduler to trainer.
         if num_iter is None:
             num_iter = trainer.state.epoch_length * trainer.state.max_epochs
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/param_scheduler.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/handlers/param_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,14 @@
             )
 
         self.optimizer = optimizer
         self.param_group_index = param_group_index
         self._state_attrs += ["param_group_index"]
 
     def __call__(self, engine: Optional[Engine], name: Optional[str] = None) -> None:
-
         value = self.get_param()
 
         if isinstance(value, list):
             if len(value) != len(self.optimizer_param_groups):
                 raise ValueError(
                     "size of value is different than optimizer_param_groups "
                     f"{len(value)} != {len(self.optimizer_param_groups)}"
@@ -591,15 +590,14 @@
             0.6000...
             0.3171...
 
     .. versionadded:: 0.4.5
     """
 
     def __init__(self, schedulers: List[ParamScheduler], durations: List[int], save_history: bool = False):
-
         if not isinstance(schedulers, Sequence):
             raise TypeError(f"Argument schedulers should be a sequence, but given {schedulers}")
 
         if len(schedulers) < 2:
             raise ValueError(
                 f"Argument schedulers should be of more than one parameter schedulers, but given {schedulers}"
             )
@@ -844,15 +842,14 @@
 
     def __init__(
         self,
         lr_scheduler: PyTorchLRScheduler,
         save_history: bool = False,
         use_legacy: bool = False,
     ):
-
         if not isinstance(lr_scheduler, PyTorchLRScheduler):
             raise TypeError(
                 "Argument lr_scheduler should be a subclass of "
                 f"torch.optim.lr_scheduler.{PyTorchLRScheduler.__name__}, "
                 f"but given {type(lr_scheduler)}"
             )
 
@@ -1015,15 +1012,14 @@
 
     if not (warmup_duration > 1):
         raise ValueError(f"Argument warmup_duration should be at least 2 events, but given {warmup_duration}")
 
     warmup_schedulers: List[ParamScheduler] = []
 
     for param_group_index, param_group in enumerate(lr_scheduler.optimizer.param_groups):
-
         if warmup_end_value is None:
             param_group_warmup_end_value = param_group["lr"]
         else:
             param_group_warmup_end_value = warmup_end_value
 
         milestones_values = [(0, warmup_start_value), (warmup_duration - 1, param_group_warmup_end_value)]
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/state_param_scheduler.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/handlers/state_param_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,15 +378,15 @@
     ):
         super(ExpStateScheduler, self).__init__(param_name, save_history, create_new)
         self.initial_value = initial_value
         self.gamma = gamma
         self._state_attrs += ["initial_value", "gamma"]
 
     def get_param(self) -> Union[List[float], float]:
-        return self.initial_value * self.gamma ** self.event_index
+        return self.initial_value * self.gamma**self.event_index
 
 
 class StepStateScheduler(StateParamScheduler):
     """Update a parameter during training by using a step function.
     This function decays the parameter value by gamma every step_size.
     Based on StepLR from PyTorch.
     https://pytorch.org/docs/stable/generated/torch.optim.lr_scheduler.StepLR.html
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/stores.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/handlers/stores.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/terminate_on_nan.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/handlers/terminate_on_nan.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         self.logger.addHandler(logging.StreamHandler())
         self._output_transform = output_transform
 
     def __call__(self, engine: Engine) -> None:
         output = self._output_transform(engine.state.output)
 
         def raise_error(x: Union[float, torch.Tensor]) -> None:
-
             if isinstance(x, numbers.Number):
                 x = torch.tensor(x)
 
             if isinstance(x, torch.Tensor) and not bool(torch.isfinite(x).all()):
                 raise RuntimeError("Infinite or NaN tensor found.")
 
         try:
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/time_limit.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/handlers/time_limit.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
             handler = TimeLimit() # 8 hours of training
             trainer.add_event_handler(Events.ITERATION_COMPLETED, handler)
 
     .. versionadded:: 0.4.3
     """
 
     def __init__(self, limit_sec: Optional[int] = 28800):
-
         if not isinstance(limit_sec, int):
             raise TypeError("Argument limit_sec should be an integer.")
         if limit_sec <= 0:
             raise ValueError("Argument limit_sec should be a positive integer.")
 
         self.limit_sec = limit_sec
         self.start_time = time.time()
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/time_profilers.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/handlers/time_profilers.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/handlers/timing.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/handlers/timing.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/__init__.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/accumulation.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/accumulation.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/accuracy.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/accuracy.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,18 +47,18 @@
             raise ValueError(
                 "y and y_pred must have same shape of (batch_size, num_categories, ...) and num_categories > 1."
             )
 
     def _check_binary_multilabel_cases(self, output: Sequence[torch.Tensor]) -> None:
         y_pred, y = output
 
-        if not torch.equal(y, y ** 2):
+        if not torch.equal(y, y**2):
             raise ValueError("For binary cases, y must be comprised of 0's and 1's.")
 
-        if not torch.equal(y_pred, y_pred ** 2):
+        if not torch.equal(y_pred, y_pred**2):
             raise ValueError("For binary cases, y_pred must be comprised of 0's and 1's.")
 
     def _check_type(self, output: Sequence[torch.Tensor]) -> None:
         y_pred, y = output
 
         if y.ndimension() + 1 == y_pred.ndimension():
             num_classes = y_pred.shape[1]
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/classification_report.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/classification_report.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/confusion_matrix.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/confusion_matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         y = y.flatten()
 
         target_mask = (y >= 0) & (y < self.num_classes)
         y = y[target_mask]
         y_pred = y_pred[target_mask]
 
         indices = self.num_classes * y + y_pred
-        m = torch.bincount(indices, minlength=self.num_classes ** 2).reshape(self.num_classes, self.num_classes)
+        m = torch.bincount(indices, minlength=self.num_classes**2).reshape(self.num_classes, self.num_classes)
         self.confusion_matrix += m.to(self.confusion_matrix)
 
     @sync_all_reduce("confusion_matrix", "_num_examples")
     def compute(self) -> torch.Tensor:
         if self._num_examples == 0:
             raise NotComputableError("Confusion matrix must have at least one example before it can be computed.")
         if self.average:
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/epoch_metric.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/epoch_metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,14 @@
     def __init__(
         self,
         compute_fn: Callable[[torch.Tensor, torch.Tensor], float],
         output_transform: Callable = lambda x: x,
         check_compute_fn: bool = True,
         device: Union[str, torch.device] = torch.device("cpu"),
     ) -> None:
-
         if not callable(compute_fn):
             raise TypeError("Argument compute_fn should be callable.")
 
         self.compute_fn = compute_fn
         self._check_compute_fn = check_compute_fn
 
         super(EpochMetric, self).__init__(output_transform=output_transform, device=device)
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/fbeta.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/fbeta.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,13 +163,13 @@
             output_transform=(lambda x: x) if output_transform is None else output_transform,  # type: ignore[arg-type]
             average=False,
             device=device,
         )
     elif recall._average:
         raise ValueError("Input recall metric should have average=False")
 
-    fbeta = (1.0 + beta ** 2) * precision * recall / (beta ** 2 * precision + recall + 1e-15)
+    fbeta = (1.0 + beta**2) * precision * recall / (beta**2 * precision + recall + 1e-15)
 
     if average:
         fbeta = fbeta.mean().item()
 
     return fbeta
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/frequency.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/frequency.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/gan/fid.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/gan/fid.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 else:
     torch_outer = torch.outer
 
 
 def fid_score(
     mu1: torch.Tensor, mu2: torch.Tensor, sigma1: torch.Tensor, sigma2: torch.Tensor, eps: float = 1e-6
 ) -> float:
-
     try:
         import numpy as np
     except ImportError:
         raise ModuleNotFoundError("fid_score requires numpy to be installed.")
 
     try:
         import scipy.linalg
@@ -167,15 +166,14 @@
     def __init__(
         self,
         num_features: Optional[int] = None,
         feature_extractor: Optional[torch.nn.Module] = None,
         output_transform: Callable = lambda x: x,
         device: Union[str, torch.device] = torch.device("cpu"),
     ) -> None:
-
         try:
             import numpy as np  # noqa: F401
         except ImportError:
             raise ModuleNotFoundError("This module requires numpy to be installed.")
 
         try:
             import scipy  # noqa: F401
@@ -193,15 +191,14 @@
             feature_extractor=feature_extractor,
             output_transform=output_transform,
             device=device,
         )
 
     @staticmethod
     def _online_update(features: torch.Tensor, total: torch.Tensor, sigma: torch.Tensor) -> None:
-
         total += features
         sigma += torch_outer(features, features)
 
     def _get_covariance(self, sigma: torch.Tensor, total: torch.Tensor) -> torch.Tensor:
         r"""
         Calculates covariance from mean and sum of products of variables
         """
@@ -209,15 +206,14 @@
         sub_matrix = torch_outer(total, total)
         sub_matrix = sub_matrix / self._num_examples
 
         return (sigma - sub_matrix) / (self._num_examples - 1)
 
     @reinit__is_reduced
     def reset(self) -> None:
-
         self._train_sigma = torch.zeros(
             (self._num_features, self._num_features), dtype=torch.float64, device=self._device
         )
 
         self._train_total = torch.zeros(self._num_features, dtype=torch.float64, device=self._device)
 
         self._test_sigma = torch.zeros(
@@ -227,15 +223,14 @@
         self._test_total = torch.zeros(self._num_features, dtype=torch.float64, device=self._device)
         self._num_examples: int = 0
 
         super(FID, self).reset()
 
     @reinit__is_reduced
     def update(self, output: Sequence[torch.Tensor]) -> None:
-
         train, test = output
         train_features = self._extract_features(train)
         test_features = self._extract_features(test)
 
         if train_features.shape[0] != test_features.shape[0] or train_features.shape[1] != test_features.shape[1]:
             raise ValueError(
                 f"""
@@ -251,15 +246,14 @@
         for features in test_features:
             self._online_update(features, self._test_total, self._test_sigma)
 
         self._num_examples += train_features.shape[0]
 
     @sync_all_reduce("_num_examples", "_train_total", "_test_total", "_train_sigma", "_test_sigma")
     def compute(self) -> float:
-
         fid = fid_score(
             mu1=self._train_total / self._num_examples,
             mu2=self._test_total / self._num_examples,
             sigma1=self._get_covariance(self._train_sigma, self._train_total),
             sigma2=self._get_covariance(self._test_sigma, self._test_total),
             eps=self._eps,
         )
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/gan/inception_score.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/gan/inception_score.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,14 @@
     def __init__(
         self,
         num_features: Optional[int] = None,
         feature_extractor: Optional[torch.nn.Module] = None,
         output_transform: Callable = lambda x: x,
         device: Union[str, torch.device] = torch.device("cpu"),
     ) -> None:
-
         if num_features is None and feature_extractor is None:
             num_features = 1000
             feature_extractor = InceptionModel(return_features=False, device=device)
 
         self._eps = 1e-16
 
         super(InceptionScore, self).__init__(
@@ -96,40 +95,37 @@
             feature_extractor=feature_extractor,
             output_transform=output_transform,
             device=device,
         )
 
     @reinit__is_reduced
     def reset(self) -> None:
-
         self._num_examples = 0
 
         self._prob_total = torch.zeros(self._num_features, dtype=torch.float64, device=self._device)
         self._total_kl_d = torch.zeros(self._num_features, dtype=torch.float64, device=self._device)
 
         super(InceptionScore, self).reset()
 
     @reinit__is_reduced
     def update(self, output: torch.Tensor) -> None:
-
         probabilities = self._extract_features(output)
 
         prob_sum = torch.sum(probabilities, 0, dtype=torch.float64)
         log_prob = torch.log(probabilities + self._eps)
         if log_prob.dtype != probabilities.dtype:
             log_prob = log_prob.to(probabilities)
         kl_sum = torch.sum(probabilities * log_prob, 0, dtype=torch.float64)
 
         self._num_examples += probabilities.shape[0]
         self._prob_total += prob_sum
         self._total_kl_d += kl_sum
 
     @sync_all_reduce("_num_examples", "_prob_total", "_total_kl_d")
     def compute(self) -> float:
-
         if self._num_examples == 0:
             raise NotComputableError("InceptionScore must have at least one example before it can be computed.")
 
         mean_probs = self._prob_total / self._num_examples
         log_mean_probs = torch.log(mean_probs + self._eps)
         if log_mean_probs.dtype != self._prob_total.dtype:
             log_mean_probs = log_mean_probs.to(self._prob_total)
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/gan/utils.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/gan/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
     def __init__(
         self,
         num_features: Optional[int],
         feature_extractor: Optional[torch.nn.Module],
         output_transform: Callable = lambda x: x,
         device: Union[str, torch.device] = torch.device("cpu"),
     ) -> None:
-
         if num_features is None:
             raise ValueError("Argument num_features must be provided, if feature_extractor is specified.")
 
         if feature_extractor is None:
             feature_extractor = torch.nn.Identity()
 
         if num_features <= 0:
@@ -74,28 +73,26 @@
 
         self._num_features = num_features
         self._feature_extractor = feature_extractor.to(device)
 
         super(_BaseInceptionMetric, self).__init__(output_transform=output_transform, device=device)
 
     def _check_feature_shapes(self, samples: torch.Tensor) -> None:
-
         if samples.dim() != 2:
             raise ValueError(f"feature_extractor output must be a tensor of dim 2, got: {samples.dim()}")
 
         if samples.shape[0] == 0:
             raise ValueError(f"Batch size should be greater than one, got: {samples.shape[0]}")
 
         if samples.shape[1] != self._num_features:
             raise ValueError(
                 f"num_features returned by feature_extractor should be {self._num_features}, got: {samples.shape[1]}"
             )
 
     def _extract_features(self, inputs: torch.Tensor) -> torch.Tensor:
-
         inputs = inputs.detach()
 
         if inputs.device != torch.device(self._device):
             inputs = inputs.to(self._device)
 
         with torch.no_grad():
             outputs = self._feature_extractor(inputs).to(self._device, dtype=torch.float64)
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/loss.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/mean_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/mean_pairwise_distance.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/mean_pairwise_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/mean_squared_error.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/metric.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -480,20 +480,20 @@
         from ignite.metrics.metrics_lambda import MetricsLambda
 
         return MetricsLambda(lambda x, y: x * y, other, self)
 
     def __pow__(self, other: Any) -> "MetricsLambda":
         from ignite.metrics.metrics_lambda import MetricsLambda
 
-        return MetricsLambda(lambda x, y: x ** y, self, other)
+        return MetricsLambda(lambda x, y: x**y, self, other)
 
     def __rpow__(self, other: Any) -> "MetricsLambda":
         from ignite.metrics.metrics_lambda import MetricsLambda
 
-        return MetricsLambda(lambda x, y: x ** y, other, self)
+        return MetricsLambda(lambda x, y: x**y, other, self)
 
     def __mod__(self, other: Any) -> "MetricsLambda":
         from ignite.metrics.metrics_lambda import MetricsLambda
 
         return MetricsLambda(lambda x, y: x % y, self, other)
 
     def __truediv__(self, other: Any) -> "MetricsLambda":
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/metrics_lambda.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/metrics_lambda.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/multilabel_confusion_matrix.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/multilabel_confusion_matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,12 +160,12 @@
         valid_types = (torch.uint8, torch.int8, torch.int16, torch.int32, torch.int64)
         if y_pred.dtype not in valid_types:
             raise ValueError(f"y_pred must be of any type: {valid_types}")
 
         if y.dtype not in valid_types:
             raise ValueError(f"y must be of any type: {valid_types}")
 
-        if not torch.equal(y_pred, y_pred ** 2):
+        if not torch.equal(y_pred, y_pred**2):
             raise ValueError("y_pred must be a binary tensor")
 
-        if not torch.equal(y, y ** 2):
+        if not torch.equal(y, y**2):
             raise ValueError("y must be a binary tensor")
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/nlp/bleu.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/nlp/bleu.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 
     @staticmethod
     def smooth2(numerators: torch.Tensor, denominators: torch.Tensor) -> Sequence[float]:
         return _Smoother._smooth2(numerators, denominators)
 
     @staticmethod
     def _smooth2(numerators: torch.Tensor, denominators: torch.Tensor) -> Sequence[float]:
-
         return [
             (n.item() + 1) / (d.item() + 1) if i != 0 else n.item() / d.item()
             for i, (n, d) in enumerate(zip(numerators, denominators))
         ]
 
     @staticmethod
     def no_smooth(numerators: torch.Tensor, denominators: torch.Tensor) -> Sequence[float]:
@@ -153,15 +152,14 @@
     def _n_gram_counter(
         self,
         references: Sequence[Sequence[Sequence[Any]]],
         candidates: Sequence[Sequence[Any]],
         p_numerators: torch.Tensor,
         p_denominators: torch.Tensor,
     ) -> Tuple[int, int]:
-
         if len(references) != len(candidates):
             raise ValueError(
                 f"nb of candidates should be equal to nb of reference lists ({len(candidates)} != "
                 f"{len(references)})"
             )
 
         hyp_lengths = 0
@@ -183,15 +181,14 @@
             ref_lengths += _closest_ref_length(refs, len(hyp))
 
         return hyp_lengths, ref_lengths
 
     def _brevity_penalty_smoothing(
         self, p_numerators: torch.Tensor, p_denominators: torch.Tensor, hyp_length_sum: int, ref_length_sum: int
     ) -> float:
-
         # Returns 0 if there's no matching n-grams
         # We only need to check for p_numerators[1] == 0, since if there's
         # no unigrams, there won't be any higher order ngrams.
         if p_numerators[1] == 0:
             return 0
 
         # If no smoother, returns 0 if there's at least one a not matching n-grams]
@@ -212,15 +209,14 @@
         gm = bp * math.exp(math.fsum(s))
         return gm
 
     def _sentence_bleu(self, references: Sequence[Sequence[Any]], candidates: Sequence[Any]) -> float:
         return self._corpus_bleu([references], [candidates])
 
     def _corpus_bleu(self, references: Sequence[Sequence[Sequence[Any]]], candidates: Sequence[Sequence[Any]]) -> float:
-
         p_numerators: torch.Tensor = torch.zeros(self.ngrams_order + 1)
         p_denominators: torch.Tensor = torch.zeros(self.ngrams_order + 1)
 
         hyp_length_sum, ref_length_sum = self._n_gram_counter(
             references=references, candidates=candidates, p_numerators=p_numerators, p_denominators=p_denominators
         )
         bleu_score = self._brevity_penalty_smoothing(
@@ -230,15 +226,14 @@
             ref_length_sum=ref_length_sum,
         )
 
         return bleu_score
 
     @reinit__is_reduced
     def reset(self) -> None:
-
         if self.average == "macro":
             self._sum_of_bleu = torch.tensor(0.0, dtype=torch.double, device=self._device)
             self._num_sentences = 0
 
         if self.average == "micro":
             self.p_numerators = torch.zeros(self.ngrams_order + 1)
             self.p_denominators = torch.zeros(self.ngrams_order + 1)
@@ -266,15 +261,14 @@
         if self._num_sentences == 0:
             raise NotComputableError("Bleu must have at least one example before it can be computed.")
 
         return self._sum_of_bleu / self._num_sentences
 
     @sync_all_reduce("p_numerators", "p_denominators", "hyp_length_sum", "ref_length_sum")
     def _compute_micro(self) -> float:
-
         bleu_score = self._brevity_penalty_smoothing(
             p_numerators=self.p_numerators,
             p_denominators=self.p_denominators,
             hyp_length_sum=self.hyp_length_sum,
             ref_length_sum=self.ref_length_sum,
         )
         return bleu_score
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/nlp/rouge.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/nlp/rouge.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/nlp/utils.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/precision.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/precision.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     def __init__(
         self,
         output_transform: Callable = lambda x: x,
         average: Optional[Union[bool, str]] = False,
         is_multilabel: bool = False,
         device: Union[str, torch.device] = torch.device("cpu"),
     ):
-
         if not (average is None or isinstance(average, bool) or average in ["macro", "micro", "weighted", "samples"]):
             raise ValueError(
                 "Argument average should be None or a boolean or one of values"
                 " 'macro', 'micro', 'weighted' and 'samples'."
             )
 
         if average is True:
@@ -55,15 +54,14 @@
                 "`y` and `y_pred` should be of dtype long when entry type is binary and average!=False", RuntimeWarning
             )
 
     def _prepare_output(self, output: Sequence[torch.Tensor]) -> Sequence[torch.Tensor]:
         y_pred, y = output[0].detach(), output[1].detach()
 
         if self._type == "binary" or self._type == "multiclass":
-
             num_classes = 2 if self._type == "binary" else y_pred.size(1)
             if self._type == "multiclass" and y.max() + 1 > num_classes:
                 raise ValueError(
                     f"y_pred contains less classes than y. Number of predicted classes is {num_classes}"
                     f" and element in y has invalid class = {y.max().item() + 1}."
                 )
             y = y.view(-1)
@@ -84,15 +82,14 @@
         y = y.to(dtype=torch.float64, device=self._device)
         correct = y * y_pred
 
         return y_pred, y, correct
 
     @reinit__is_reduced
     def reset(self) -> None:
-
         # `numerator`, `denominator` and `weight` are three variables chosen to be abstract
         # representatives of the ones that are measured for cases with different `average` parameters.
         # `weight` is only used when `average='weighted'`. Actual value of these three variables is
         # as follows.
         #
         # average='samples':
         #   numerator (torch.Tensor): sum of metric value for samples
@@ -119,15 +116,14 @@
         self._weight: Union[int, torch.Tensor] = 0
         self._updated = False
 
         super(_BasePrecisionRecall, self).reset()
 
     @sync_all_reduce("_numerator", "_denominator")
     def compute(self) -> Union[torch.Tensor, float]:
-
         # Return value of the metric for `average` options `'weighted'` and `'macro'` is computed as follows.
         #
         # .. math:: \text{Precision/Recall} = \frac{ numerator }{ denominator } \cdot weight
         #
         # wherein `weight` is the internal variable `weight` for `'weighted'` option and :math:`1/C`
         # for the `macro` one. :math:`C` is the number of classes/labels.
         #
@@ -372,25 +368,22 @@
     @reinit__is_reduced
     def update(self, output: Sequence[torch.Tensor]) -> None:
         self._check_shape(output)
         self._check_type(output)
         y_pred, y, correct = self._prepare_output(output)
 
         if self._average == "samples":
-
             all_positives = y_pred.sum(dim=1)
             true_positives = correct.sum(dim=1)
             self._numerator += torch.sum(true_positives / (all_positives + self.eps))
             self._denominator += y.size(0)
         elif self._average == "micro":
-
             self._denominator += y_pred.sum()
             self._numerator += correct.sum()
         else:  # _average in [False, None, 'macro', 'weighted']
-
             self._denominator += y_pred.sum(dim=0)
             self._numerator += correct.sum(dim=0)
 
             if self._average == "weighted":
                 self._weight += y.sum(dim=0)
 
         self._updated = True
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/psnr.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/psnr.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     @reinit__is_reduced
     def update(self, output: Sequence[torch.Tensor]) -> None:
         self._check_shape_dtype(output)
         y_pred, y = output[0].detach(), output[1].detach()
 
         dim = tuple(range(1, y.ndim))
         mse_error = torch.pow(y_pred.double() - y.view_as(y_pred).double(), 2).mean(dim=dim)
-        self._sum_of_batchwise_psnr += torch.sum(10.0 * torch.log10(self.data_range ** 2 / (mse_error + 1e-10))).to(
+        self._sum_of_batchwise_psnr += torch.sum(10.0 * torch.log10(self.data_range**2 / (mse_error + 1e-10))).to(
             device=self._device
         )
         self._num_examples += y.shape[0]
 
     @sync_all_reduce("_sum_of_batchwise_psnr", "_num_examples")
     def compute(self) -> float:
         if self._num_examples == 0:
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/recall.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/recall.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,25 +217,22 @@
     @reinit__is_reduced
     def update(self, output: Sequence[torch.Tensor]) -> None:
         self._check_shape(output)
         self._check_type(output)
         _, y, correct = self._prepare_output(output)
 
         if self._average == "samples":
-
             actual_positives = y.sum(dim=1)
             true_positives = correct.sum(dim=1)
             self._numerator += torch.sum(true_positives / (actual_positives + self.eps))
             self._denominator += y.size(0)
         elif self._average == "micro":
-
             self._denominator += y.sum()
             self._numerator += correct.sum()
         else:  # _average in [False, 'macro', 'weighted']
-
             self._denominator += y.sum(dim=0)
             self._numerator += correct.sum(dim=0)
 
             if self._average == "weighted":
                 self._weight += y.sum(dim=0)
 
         self._updated = True
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/root_mean_squared_error.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/root_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/running_average.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/running_average.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/ssim.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/ssim.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/metrics/top_k_categorical_accuracy.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/metrics/top_k_categorical_accuracy.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/ignite/utils.py` & `pytorch-ignite-0.5.0.dev20230429/ignite/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,21 +178,19 @@
     if distributed_rank is None:
         import ignite.distributed as idist
 
         distributed_rank = idist.get_rank()
 
     # Remove previous handlers
     if distributed_rank > 0 or reset:
-
         if logger.hasHandlers():
             for h in list(logger.handlers):
                 logger.removeHandler(h)
 
     if distributed_rank > 0:
-
         # Add null handler to avoid multiple parallel messages
         logger.addHandler(logging.NullHandler())
 
     # Keep the existing configuration if not reset
     if existing and not reset:
         return logger
 
@@ -250,15 +248,14 @@
     except ImportError:
         pass
 
 
 def deprecated(
     deprecated_in: str, removed_in: str = "", reasons: Tuple[str, ...] = (), raise_exception: bool = False
 ) -> Callable:
-
     F = TypeVar("F", bound=Callable[..., Any])
 
     def decorator(func: F) -> F:
         func_doc = func.__doc__ if func.__doc__ else ""
         deprecation_warning = (
             f"This function has been deprecated since version {deprecated_in}"
             + (f" and will be removed in version {removed_in}" if removed_in else "")
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/pyproject.toml` & `pytorch-ignite-0.5.0.dev20230429/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/pytorch_ignite.egg-info/PKG-INFO` & `pytorch-ignite-0.5.0.dev20230429/pytorch_ignite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-ignite
-Version: 0.5.0.dev20230428
+Version: 0.5.0.dev20230429
 Summary: A lightweight library to help with training neural networks in PyTorch.
 Home-page: https://github.com/pytorch/ignite
 Author: PyTorch Core Team
 Author-email: soumith@pytorch.org
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pytorch-ignite-0.5.0.dev20230428/pytorch_ignite.egg-info/SOURCES.txt` & `pytorch-ignite-0.5.0.dev20230429/pytorch_ignite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/setup.cfg` & `pytorch-ignite-0.5.0.dev20230429/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230428/setup.py` & `pytorch-ignite-0.5.0.dev20230429/setup.py`

 * *Files identical despite different names*


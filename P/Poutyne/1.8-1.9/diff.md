# Comparing `tmp/Poutyne-1.8.tar.gz` & `tmp/Poutyne-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Poutyne-1.8.tar", last modified: Fri Dec 17 18:16:23 2021, max compression
+gzip compressed data, was "Poutyne-1.9.tar", last modified: Fri Feb 18 22:48:55 2022, max compression
```

## Comparing `Poutyne-1.8.tar` & `Poutyne-1.9.tar`

### file list

```diff
@@ -1,113 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:23.872880 Poutyne-1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2021-12-17 18:16:14.000000 Poutyne-1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14478 2021-12-17 18:16:23.872880 Poutyne-1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:23.860880 Poutyne-1.8/Poutyne.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14478 2021-12-17 18:16:23.000000 Poutyne-1.8/Poutyne.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3714 2021-12-17 18:16:23.000000 Poutyne-1.8/Poutyne.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-17 18:16:23.000000 Poutyne-1.8/Poutyne.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-12-17 18:16:23.000000 Poutyne-1.8/Poutyne.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-12-17 18:16:23.000000 Poutyne-1.8/Poutyne.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11469 2021-12-17 18:16:14.000000 Poutyne-1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:23.860880 Poutyne-1.8/poutyne/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:23.864880 Poutyne-1.8/poutyne/framework/
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:23.864880 Poutyne-1.8/poutyne/framework/callbacks/
--rw-r--r--   0 runner    (1001) docker     (121)      514 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2047 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/best_model_restore.py
--rw-r--r--   0 runner    (1001) docker     (121)    14478 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     4819 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/clip_grad.py
--rw-r--r--   0 runner    (1001) docker     (121)    13879 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/color_formatting.py
--rw-r--r--   0 runner    (1001) docker     (121)     3047 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/delay.py
--rw-r--r--   0 runner    (1001) docker     (121)     4233 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/earlystopping.py
--rw-r--r--   0 runner    (1001) docker     (121)     6958 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/gradient_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     5057 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/lambda_.py
--rw-r--r--   0 runner    (1001) docker     (121)     8274 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     3196 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)     9402 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     4788 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/notification.py
--rw-r--r--   0 runner    (1001) docker     (121)     9518 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/periodic.py
--rw-r--r--   0 runner    (1001) docker     (121)     9284 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/policies.py
--rw-r--r--   0 runner    (1001) docker     (121)    13949 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/progress.py
--rw-r--r--   0 runner    (1001) docker     (121)     3262 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (121)      454 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/terminate_on_nan.py
--rw-r--r--   0 runner    (1001) docker     (121)     8702 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/callbacks/tracker.py
--rw-r--r--   0 runner    (1001) docker     (121)    53044 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/experiment.py
--rw-r--r--   0 runner    (1001) docker     (121)     6564 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/iterators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:23.864880 Poutyne-1.8/poutyne/framework/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)      237 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7842 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/metrics/batch_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/metrics/batch_metrics_pytorch_registering.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:23.868880 Poutyne-1.8/poutyne/framework/metrics/epoch_metrics/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/metrics/epoch_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      905 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/metrics/epoch_metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    14569 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/metrics/epoch_metrics/fscores.py
--rw-r--r--   0 runner    (1001) docker     (121)     4335 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/metrics/epoch_metrics/sklearn_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1831 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/metrics/metric_argument_indexing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2438 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/metrics/metrics_registering.py
--rw-r--r--   0 runner    (1001) docker     (121)     2325 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    79768 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/model.py
--rw-r--r--   0 runner    (1001) docker     (121)    61661 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/model_bundle.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/framework/warning_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:23.868880 Poutyne-1.8/poutyne/layers/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      607 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/layers/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8421 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     5286 2021-12-17 18:16:15.000000 Poutyne-1.8/poutyne/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-12-17 18:16:23.000000 Poutyne-1.8/poutyne/version.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-12-17 18:16:15.000000 Poutyne-1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-12-17 18:16:23.872880 Poutyne-1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3070 2021-12-17 18:16:15.000000 Poutyne-1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:23.868880 Poutyne-1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      200 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/context.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:23.868880 Poutyne-1.8/tests/framework/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:23.868880 Poutyne-1.8/tests/framework/callbacks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2771 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/callbacks/test_best_model_restore.py
--rw-r--r--   0 runner    (1001) docker     (121)     7493 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/callbacks/test_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     5222 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/callbacks/test_delay.py
--rw-r--r--   0 runner    (1001) docker     (121)     3041 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/callbacks/test_earlystopping.py
--rw-r--r--   0 runner    (1001) docker     (121)     3866 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/callbacks/test_gradient_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     4880 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/callbacks/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (121)     8230 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/callbacks/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     2372 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/callbacks/test_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)     4389 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/callbacks/test_lr_scheduler_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)    14534 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/callbacks/test_mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     4530 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/callbacks/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (121)     3229 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/callbacks/test_optimizer_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     9738 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/callbacks/test_periodic.py
--rw-r--r--   0 runner    (1001) docker     (121)     5650 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/callbacks/test_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)    11839 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/callbacks/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (121)     6800 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/callbacks/test_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (121)    13438 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/callbacks/test_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:23.868880 Poutyne-1.8/tests/framework/experiment/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14515 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/experiment/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (121)    14626 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/experiment/test_model_bundle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:23.872880 Poutyne-1.8/tests/framework/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15665 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/metrics/test_batch_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)    10479 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/metrics/test_fscores.py
--rw-r--r--   0 runner    (1001) docker     (121)    11755 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/metrics/test_metrics_model_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)     6201 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/metrics/test_sklearn_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:23.872880 Poutyne-1.8/tests/framework/model/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7711 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/model/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3654 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/model/test_dict_output.py
--rw-r--r--   0 runner    (1001) docker     (121)    51337 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/model/test_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/model/test_model_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)    30736 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/model/test_model_progress.py
--rw-r--r--   0 runner    (1001) docker     (121)     5165 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/model/test_multi_dict_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     9996 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/model/test_multi_gpu.py
--rw-r--r--   0 runner    (1001) docker     (121)     8840 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/model/test_multi_input.py
--rw-r--r--   0 runner    (1001) docker     (121)     6286 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/model/test_multi_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     7860 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/model/test_multi_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     2648 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/framework/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     7904 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)    10749 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2021-12-17 18:16:15.000000 Poutyne-1.8/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 22:48:55.804492 Poutyne-1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-02-18 22:48:44.000000 Poutyne-1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    14478 2022-02-18 22:48:55.804492 Poutyne-1.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 22:48:55.784492 Poutyne-1.9/Poutyne.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    14478 2022-02-18 22:48:55.000000 Poutyne-1.9/Poutyne.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-02-18 22:48:55.000000 Poutyne-1.9/Poutyne.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-18 22:48:55.000000 Poutyne-1.9/Poutyne.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2022-02-18 22:48:55.000000 Poutyne-1.9/Poutyne.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-18 22:48:55.000000 Poutyne-1.9/Poutyne.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11445 2022-02-18 22:48:44.000000 Poutyne-1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 22:48:55.784492 Poutyne-1.9/poutyne/
+-rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 22:48:55.788492 Poutyne-1.9/poutyne/framework/
+-rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 22:48:55.792492 Poutyne-1.9/poutyne/framework/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2914 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/best_model_restore.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15214 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5687 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2236 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/clip_grad.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14747 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/color_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3866 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/delay.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5052 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/earlystopping.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7826 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/gradient_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9711 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/gradient_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5925 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/lambda_.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9641 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4064 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10211 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5655 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/notification.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11150 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10150 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14817 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/progress.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4130 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1322 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/callbacks/terminate_on_nan.py
+-rw-r--r--   0 runner    (1001) docker     (121)      945 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8038 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/iterators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 22:48:55.792492 Poutyne-1.9/poutyne/framework/metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8710 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/metrics/batch_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/metrics/batch_metrics_pytorch_registering.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 22:48:55.792492 Poutyne-1.9/poutyne/framework/metrics/epoch_metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)      976 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/metrics/epoch_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2007 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/metrics/epoch_metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18193 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/metrics/epoch_metrics/fscores.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5149 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/metrics/epoch_metrics/sklearn_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2699 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/metrics/metric_argument_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4173 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/metrics/metrics_registering.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3464 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    86792 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    63595 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/model_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1705 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      910 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/framework/warning_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 22:48:55.792492 Poutyne-1.9/poutyne/layers/
+-rw-r--r--   0 runner    (1001) docker     (121)      923 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/layers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9289 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6555 2022-02-18 22:48:44.000000 Poutyne-1.9/poutyne/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-02-18 22:48:55.000000 Poutyne-1.9/poutyne/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-02-18 22:48:44.000000 Poutyne-1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-02-18 22:48:55.804492 Poutyne-1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3086 2022-02-18 22:48:44.000000 Poutyne-1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 22:48:55.792492 Poutyne-1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      867 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/context.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 22:48:55.796492 Poutyne-1.9/tests/framework/
+-rw-r--r--   0 runner    (1001) docker     (121)      867 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 22:48:55.800492 Poutyne-1.9/tests/framework/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (121)      867 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4042 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_best_model_restore.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_callback_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8361 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3731 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_color_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6432 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_delay.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4573 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_earlystopping.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7776 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_gradient_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5748 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11879 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3238 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5257 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_lr_scheduler_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19775 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7104 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_optimizer_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13358 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6518 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12707 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7668 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2703 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_terminate_on_nan.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15748 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/callbacks/test_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 22:48:55.800492 Poutyne-1.9/tests/framework/experiment/
+-rw-r--r--   0 runner    (1001) docker     (121)      867 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5282 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/experiment/test_checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15060 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/experiment/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6065 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/experiment/test_is_better_than.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2902 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/experiment/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/experiment/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 22:48:55.800492 Poutyne-1.9/tests/framework/metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)      867 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16533 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/metrics/test_batch_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15334 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/metrics/test_fscores.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17153 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/metrics/test_metrics_model_integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7069 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/metrics/test_sklearn_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 22:48:55.804492 Poutyne-1.9/tests/framework/model/
+-rw-r--r--   0 runner    (1001) docker     (121)      867 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8441 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4522 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/model/test_dict_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)    57025 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/model/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3128 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/model/test_model_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31604 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/model/test_model_progress.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6033 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/model/test_multi_dict_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10864 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/model/test_multi_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9708 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/model/test_multi_input.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7154 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/model/test_multi_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8728 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/model/test_multi_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3516 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/framework/tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8813 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15511 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-02-18 22:48:44.000000 Poutyne-1.9/tests/utils.py
```

### Comparing `Poutyne-1.8/LICENSE` & `Poutyne-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Poutyne-1.8/PKG-INFO` & `Poutyne-1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: Poutyne
-Version: 1.8
+Version: 1.9
 Summary: A simplified framework and utilities for PyTorch.
 Home-page: https://poutyne.org
 Author: Frédérik Paradis
 Author-email: fredy_14@live.fr
 License: LGPLv3
-Download-URL: https://github.com/GRAAL-Research/poutyne/archive/v1.8.zip
+Download-URL: https://github.com/GRAAL-Research/poutyne/archive/v1.9.zip
 Description: ![Poutyne Logo](https://raw.githubusercontent.com/GRAAL-Research/poutyne/master/docs/source/_static/logos/poutyne-dark.png)
         
         [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](http://www.gnu.org/licenses/lgpl-3.0)
         [![Continuous Integration](https://github.com/GRAAL-Research/poutyne/workflows/Continuous%20Integration/badge.svg)](https://github.com/GRAAL-Research/poutyne/actions?query=workflow%3A%22Continuous+Integration%22+branch%3Amaster)
+        [![codecov](https://codecov.io/gh/GRAAL-Research/poutyne/branch/master/graph/badge.svg?token=H8D1nZ1wTR)](https://codecov.io/gh/GRAAL-Research/poutyne)
         
         ## Here is Poutyne.
         
         Poutyne is a simplified framework for [PyTorch](https://pytorch.org/) and handles much of the boilerplating code needed to train neural networks.
         
         Use Poutyne to:
         - Train models easily.
@@ -48,14 +49,15 @@
         
         ```python
         # Import the Poutyne Model and define a toy dataset
         from poutyne import Model
         import torch
         import torch.nn as nn
         import numpy as np
+        import torchmetrics
         
         num_features = 20
         num_classes = 5
         hidden_state_size = 100
         
         num_train_samples = 800
         train_x = np.random.randn(num_train_samples, num_features).astype('float32')
@@ -86,17 +88,22 @@
             nn.Linear(hidden_state_size, num_classes)
         )
         ```
         
         You can now use Poutyne's model to train your network easily:
         
         ```python
-        model = Model(network, 'sgd', 'cross_entropy',
-                      batch_metrics=['accuracy'], epoch_metrics=['f1'],
-                      device=device)
+        model = Model(
+            network,
+            'sgd',
+            'cross_entropy',
+            batch_metrics=['accuracy'],
+            epoch_metrics=['f1', torchmetrics.AUROC(num_classes=num_classes)],
+            device=device
+        )
         model.fit(
             train_x, train_y,
             validation_data=(valid_x, valid_y),
             epochs=5,
             batch_size=32
         )
         ```
@@ -113,34 +120,30 @@
         
         ```python
         predictions = model.predict(test_x)
         ```
         
         [See the complete code here.](https://github.com/GRAAL-Research/poutyne/blob/master/examples/basic_random_classification.py) Also, [see this](https://github.com/GRAAL-Research/poutyne/blob/master/examples/basic_random_regression.py) for an example for regression that again also uses [epoch metrics](http://poutyne.org/metrics.html#epoch-metrics).
         
-        One of the strengths Poutyne are [callbacks](https://poutyne.org/callbacks.html). They allow you to save checkpoints, log training statistics and more. See this [notebook](https://github.com/GRAAL-Research/poutyne/blob/master/examples/introduction_pytorch_poutyne.ipynb) for an introduction to callbacks. In that vein, Poutyne also offers an [Experiment class](https://poutyne.org/experiment.html) that offers automatic checkpointing, logging and more using callbacks under the hood. Here is an example of usage.
+        One of the strengths Poutyne are [callbacks](https://poutyne.org/callbacks.html). They allow you to save checkpoints, log training statistics and more. See this [notebook](https://github.com/GRAAL-Research/poutyne/blob/master/examples/introduction_pytorch_poutyne.ipynb) for an introduction to callbacks. In that vein, Poutyne also offers an [ModelBundle class](https://poutyne.org/experiment.html#poutyne.ModelBundle) that offers automatic checkpointing, logging and more using callbacks under the hood. Here is an example of usage.
         
         ```python
-        from poutyne import Experiment, TensorDataset
-        from torch.utils.data import DataLoader
-        
-        # We need to use dataloaders (i.e. an iterable of batches) with Experiment
-        train_loader = DataLoader(TensorDataset(train_x, train_y), batch_size=32)
-        valid_loader = DataLoader(TensorDataset(valid_x, valid_y), batch_size=32)
-        test_loader = DataLoader(TensorDataset(test_x, test_y), batch_size=32)
+        from poutyne import ModelBundle
         
-        # Everything is saved in ./expt/my_classification_network
-        expt = Experiment('./expt/my_classification_network', network, device=device, optimizer='sgd', task='classif')
+        # Everything is saved in ./saves/my_classification_network
+        model_bundle = ModelBundle.from_network(
+            './saves/my_classification_network', network, optimizer='sgd', task='classif', device=device
+        )
         
-        expt.train(train_loader, valid_loader, epochs=5)
+        model_bundle.train_data(train_x, train_y, validation_data=(valid_x, valid_y), epochs=5)
         
-        expt.test(test_loader)
+        model_bundle.test_data(test_x, test_y)
         ```
         
-        [See the complete code here.](https://github.com/GRAAL-Research/poutyne/blob/master/examples/basic_random_classification_with_experiment.py) Also, [see this](https://github.com/GRAAL-Research/poutyne/blob/master/examples/basic_random_regression_with_experiment.py) for an example for regression that again also uses [epoch metrics](http://poutyne.org/metrics.html#epoch-metrics).
+        [See the complete code here.](https://github.com/GRAAL-Research/poutyne/blob/master/examples/basic_random_classification_with_model_bundle.py) Also, [see this](https://github.com/GRAAL-Research/poutyne/blob/master/examples/basic_random_regression_with_model_bundle.py) for an example for regression that again also uses [epoch metrics](http://poutyne.org/metrics.html#epoch-metrics).
         
         
         ------------------
         
         ## Installation
         
         Before installing Poutyne, you must have the latest version of [PyTorch](https://pytorch.org/) in your environment.
```

### Comparing `Poutyne-1.8/Poutyne.egg-info/PKG-INFO` & `Poutyne-1.9/Poutyne.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: Poutyne
-Version: 1.8
+Version: 1.9
 Summary: A simplified framework and utilities for PyTorch.
 Home-page: https://poutyne.org
 Author: Frédérik Paradis
 Author-email: fredy_14@live.fr
 License: LGPLv3
-Download-URL: https://github.com/GRAAL-Research/poutyne/archive/v1.8.zip
+Download-URL: https://github.com/GRAAL-Research/poutyne/archive/v1.9.zip
 Description: ![Poutyne Logo](https://raw.githubusercontent.com/GRAAL-Research/poutyne/master/docs/source/_static/logos/poutyne-dark.png)
         
         [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](http://www.gnu.org/licenses/lgpl-3.0)
         [![Continuous Integration](https://github.com/GRAAL-Research/poutyne/workflows/Continuous%20Integration/badge.svg)](https://github.com/GRAAL-Research/poutyne/actions?query=workflow%3A%22Continuous+Integration%22+branch%3Amaster)
+        [![codecov](https://codecov.io/gh/GRAAL-Research/poutyne/branch/master/graph/badge.svg?token=H8D1nZ1wTR)](https://codecov.io/gh/GRAAL-Research/poutyne)
         
         ## Here is Poutyne.
         
         Poutyne is a simplified framework for [PyTorch](https://pytorch.org/) and handles much of the boilerplating code needed to train neural networks.
         
         Use Poutyne to:
         - Train models easily.
@@ -48,14 +49,15 @@
         
         ```python
         # Import the Poutyne Model and define a toy dataset
         from poutyne import Model
         import torch
         import torch.nn as nn
         import numpy as np
+        import torchmetrics
         
         num_features = 20
         num_classes = 5
         hidden_state_size = 100
         
         num_train_samples = 800
         train_x = np.random.randn(num_train_samples, num_features).astype('float32')
@@ -86,17 +88,22 @@
             nn.Linear(hidden_state_size, num_classes)
         )
         ```
         
         You can now use Poutyne's model to train your network easily:
         
         ```python
-        model = Model(network, 'sgd', 'cross_entropy',
-                      batch_metrics=['accuracy'], epoch_metrics=['f1'],
-                      device=device)
+        model = Model(
+            network,
+            'sgd',
+            'cross_entropy',
+            batch_metrics=['accuracy'],
+            epoch_metrics=['f1', torchmetrics.AUROC(num_classes=num_classes)],
+            device=device
+        )
         model.fit(
             train_x, train_y,
             validation_data=(valid_x, valid_y),
             epochs=5,
             batch_size=32
         )
         ```
@@ -113,34 +120,30 @@
         
         ```python
         predictions = model.predict(test_x)
         ```
         
         [See the complete code here.](https://github.com/GRAAL-Research/poutyne/blob/master/examples/basic_random_classification.py) Also, [see this](https://github.com/GRAAL-Research/poutyne/blob/master/examples/basic_random_regression.py) for an example for regression that again also uses [epoch metrics](http://poutyne.org/metrics.html#epoch-metrics).
         
-        One of the strengths Poutyne are [callbacks](https://poutyne.org/callbacks.html). They allow you to save checkpoints, log training statistics and more. See this [notebook](https://github.com/GRAAL-Research/poutyne/blob/master/examples/introduction_pytorch_poutyne.ipynb) for an introduction to callbacks. In that vein, Poutyne also offers an [Experiment class](https://poutyne.org/experiment.html) that offers automatic checkpointing, logging and more using callbacks under the hood. Here is an example of usage.
+        One of the strengths Poutyne are [callbacks](https://poutyne.org/callbacks.html). They allow you to save checkpoints, log training statistics and more. See this [notebook](https://github.com/GRAAL-Research/poutyne/blob/master/examples/introduction_pytorch_poutyne.ipynb) for an introduction to callbacks. In that vein, Poutyne also offers an [ModelBundle class](https://poutyne.org/experiment.html#poutyne.ModelBundle) that offers automatic checkpointing, logging and more using callbacks under the hood. Here is an example of usage.
         
         ```python
-        from poutyne import Experiment, TensorDataset
-        from torch.utils.data import DataLoader
-        
-        # We need to use dataloaders (i.e. an iterable of batches) with Experiment
-        train_loader = DataLoader(TensorDataset(train_x, train_y), batch_size=32)
-        valid_loader = DataLoader(TensorDataset(valid_x, valid_y), batch_size=32)
-        test_loader = DataLoader(TensorDataset(test_x, test_y), batch_size=32)
+        from poutyne import ModelBundle
         
-        # Everything is saved in ./expt/my_classification_network
-        expt = Experiment('./expt/my_classification_network', network, device=device, optimizer='sgd', task='classif')
+        # Everything is saved in ./saves/my_classification_network
+        model_bundle = ModelBundle.from_network(
+            './saves/my_classification_network', network, optimizer='sgd', task='classif', device=device
+        )
         
-        expt.train(train_loader, valid_loader, epochs=5)
+        model_bundle.train_data(train_x, train_y, validation_data=(valid_x, valid_y), epochs=5)
         
-        expt.test(test_loader)
+        model_bundle.test_data(test_x, test_y)
         ```
         
-        [See the complete code here.](https://github.com/GRAAL-Research/poutyne/blob/master/examples/basic_random_classification_with_experiment.py) Also, [see this](https://github.com/GRAAL-Research/poutyne/blob/master/examples/basic_random_regression_with_experiment.py) for an example for regression that again also uses [epoch metrics](http://poutyne.org/metrics.html#epoch-metrics).
+        [See the complete code here.](https://github.com/GRAAL-Research/poutyne/blob/master/examples/basic_random_classification_with_model_bundle.py) Also, [see this](https://github.com/GRAAL-Research/poutyne/blob/master/examples/basic_random_regression_with_model_bundle.py) for an example for regression that again also uses [epoch metrics](http://poutyne.org/metrics.html#epoch-metrics).
         
         
         ------------------
         
         ## Installation
         
         Before installing Poutyne, you must have the latest version of [PyTorch](https://pytorch.org/) in your environment.
```

### Comparing `Poutyne-1.8/Poutyne.egg-info/SOURCES.txt` & `Poutyne-1.9/Poutyne.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -25,25 +25,25 @@
 poutyne/framework/callbacks/callbacks.py
 poutyne/framework/callbacks/checkpoint.py
 poutyne/framework/callbacks/clip_grad.py
 poutyne/framework/callbacks/color_formatting.py
 poutyne/framework/callbacks/delay.py
 poutyne/framework/callbacks/earlystopping.py
 poutyne/framework/callbacks/gradient_logger.py
+poutyne/framework/callbacks/gradient_tracker.py
 poutyne/framework/callbacks/lambda_.py
 poutyne/framework/callbacks/logger.py
 poutyne/framework/callbacks/lr_scheduler.py
 poutyne/framework/callbacks/mlflow_logger.py
 poutyne/framework/callbacks/notification.py
 poutyne/framework/callbacks/periodic.py
 poutyne/framework/callbacks/policies.py
 poutyne/framework/callbacks/progress.py
 poutyne/framework/callbacks/progress_bar.py
 poutyne/framework/callbacks/terminate_on_nan.py
-poutyne/framework/callbacks/tracker.py
 poutyne/framework/metrics/__init__.py
 poutyne/framework/metrics/batch_metrics.py
 poutyne/framework/metrics/batch_metrics_pytorch_registering.py
 poutyne/framework/metrics/metric_argument_indexing.py
 poutyne/framework/metrics/metrics_registering.py
 poutyne/framework/metrics/utils.py
 poutyne/framework/metrics/epoch_metrics/__init__.py
@@ -54,36 +54,43 @@
 poutyne/layers/utils.py
 tests/__init__.py
 tests/context.py
 tests/test_plotting.py
 tests/test_utils.py
 tests/utils.py
 tests/framework/__init__.py
+tests/framework/base.py
 tests/framework/tools.py
 tests/framework/callbacks/__init__.py
 tests/framework/callbacks/test_best_model_restore.py
+tests/framework/callbacks/test_callback_list.py
 tests/framework/callbacks/test_checkpoint.py
+tests/framework/callbacks/test_color_formatting.py
 tests/framework/callbacks/test_delay.py
 tests/framework/callbacks/test_earlystopping.py
 tests/framework/callbacks/test_gradient_logger.py
 tests/framework/callbacks/test_lambda.py
 tests/framework/callbacks/test_logger.py
 tests/framework/callbacks/test_lr_scheduler.py
 tests/framework/callbacks/test_lr_scheduler_checkpoint.py
 tests/framework/callbacks/test_mlflow_logger.py
 tests/framework/callbacks/test_notification.py
 tests/framework/callbacks/test_optimizer_checkpoint.py
 tests/framework/callbacks/test_periodic.py
 tests/framework/callbacks/test_policies.py
 tests/framework/callbacks/test_progress.py
 tests/framework/callbacks/test_progress_bar.py
+tests/framework/callbacks/test_terminate_on_nan.py
 tests/framework/callbacks/test_tracker.py
 tests/framework/experiment/__init__.py
+tests/framework/experiment/test_checkpointing.py
 tests/framework/experiment/test_experiment.py
-tests/framework/experiment/test_model_bundle.py
+tests/framework/experiment/test_is_better_than.py
+tests/framework/experiment/test_tasks.py
+tests/framework/experiment/utils.py
 tests/framework/metrics/__init__.py
 tests/framework/metrics/test_batch_metrics.py
 tests/framework/metrics/test_fscores.py
 tests/framework/metrics/test_metrics_model_integration.py
 tests/framework/metrics/test_sklearn_metrics.py
 tests/framework/model/__init__.py
 tests/framework/model/base.py
```

### Comparing `Poutyne-1.8/README.md` & `Poutyne-1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ![Poutyne Logo](https://raw.githubusercontent.com/GRAAL-Research/poutyne/master/docs/source/_static/logos/poutyne-dark.png)
 
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](http://www.gnu.org/licenses/lgpl-3.0)
 [![Continuous Integration](https://github.com/GRAAL-Research/poutyne/workflows/Continuous%20Integration/badge.svg)](https://github.com/GRAAL-Research/poutyne/actions?query=workflow%3A%22Continuous+Integration%22+branch%3Amaster)
+[![codecov](https://codecov.io/gh/GRAAL-Research/poutyne/branch/master/graph/badge.svg?token=H8D1nZ1wTR)](https://codecov.io/gh/GRAAL-Research/poutyne)
 
 ## Here is Poutyne.
 
 Poutyne is a simplified framework for [PyTorch](https://pytorch.org/) and handles much of the boilerplating code needed to train neural networks.
 
 Use Poutyne to:
 - Train models easily.
@@ -39,14 +40,15 @@
 
 ```python
 # Import the Poutyne Model and define a toy dataset
 from poutyne import Model
 import torch
 import torch.nn as nn
 import numpy as np
+import torchmetrics
 
 num_features = 20
 num_classes = 5
 hidden_state_size = 100
 
 num_train_samples = 800
 train_x = np.random.randn(num_train_samples, num_features).astype('float32')
@@ -77,17 +79,22 @@
     nn.Linear(hidden_state_size, num_classes)
 )
 ```
 
 You can now use Poutyne's model to train your network easily:
 
 ```python
-model = Model(network, 'sgd', 'cross_entropy',
-              batch_metrics=['accuracy'], epoch_metrics=['f1'],
-              device=device)
+model = Model(
+    network,
+    'sgd',
+    'cross_entropy',
+    batch_metrics=['accuracy'],
+    epoch_metrics=['f1', torchmetrics.AUROC(num_classes=num_classes)],
+    device=device
+)
 model.fit(
     train_x, train_y,
     validation_data=(valid_x, valid_y),
     epochs=5,
     batch_size=32
 )
 ```
@@ -104,34 +111,30 @@
 
 ```python
 predictions = model.predict(test_x)
 ```
 
 [See the complete code here.](https://github.com/GRAAL-Research/poutyne/blob/master/examples/basic_random_classification.py) Also, [see this](https://github.com/GRAAL-Research/poutyne/blob/master/examples/basic_random_regression.py) for an example for regression that again also uses [epoch metrics](http://poutyne.org/metrics.html#epoch-metrics).
 
-One of the strengths Poutyne are [callbacks](https://poutyne.org/callbacks.html). They allow you to save checkpoints, log training statistics and more. See this [notebook](https://github.com/GRAAL-Research/poutyne/blob/master/examples/introduction_pytorch_poutyne.ipynb) for an introduction to callbacks. In that vein, Poutyne also offers an [Experiment class](https://poutyne.org/experiment.html) that offers automatic checkpointing, logging and more using callbacks under the hood. Here is an example of usage.
+One of the strengths Poutyne are [callbacks](https://poutyne.org/callbacks.html). They allow you to save checkpoints, log training statistics and more. See this [notebook](https://github.com/GRAAL-Research/poutyne/blob/master/examples/introduction_pytorch_poutyne.ipynb) for an introduction to callbacks. In that vein, Poutyne also offers an [ModelBundle class](https://poutyne.org/experiment.html#poutyne.ModelBundle) that offers automatic checkpointing, logging and more using callbacks under the hood. Here is an example of usage.
 
 ```python
-from poutyne import Experiment, TensorDataset
-from torch.utils.data import DataLoader
-
-# We need to use dataloaders (i.e. an iterable of batches) with Experiment
-train_loader = DataLoader(TensorDataset(train_x, train_y), batch_size=32)
-valid_loader = DataLoader(TensorDataset(valid_x, valid_y), batch_size=32)
-test_loader = DataLoader(TensorDataset(test_x, test_y), batch_size=32)
+from poutyne import ModelBundle
 
-# Everything is saved in ./expt/my_classification_network
-expt = Experiment('./expt/my_classification_network', network, device=device, optimizer='sgd', task='classif')
+# Everything is saved in ./saves/my_classification_network
+model_bundle = ModelBundle.from_network(
+    './saves/my_classification_network', network, optimizer='sgd', task='classif', device=device
+)
 
-expt.train(train_loader, valid_loader, epochs=5)
+model_bundle.train_data(train_x, train_y, validation_data=(valid_x, valid_y), epochs=5)
 
-expt.test(test_loader)
+model_bundle.test_data(test_x, test_y)
 ```
 
-[See the complete code here.](https://github.com/GRAAL-Research/poutyne/blob/master/examples/basic_random_classification_with_experiment.py) Also, [see this](https://github.com/GRAAL-Research/poutyne/blob/master/examples/basic_random_regression_with_experiment.py) for an example for regression that again also uses [epoch metrics](http://poutyne.org/metrics.html#epoch-metrics).
+[See the complete code here.](https://github.com/GRAAL-Research/poutyne/blob/master/examples/basic_random_classification_with_model_bundle.py) Also, [see this](https://github.com/GRAAL-Research/poutyne/blob/master/examples/basic_random_regression_with_model_bundle.py) for an example for regression that again also uses [epoch metrics](http://poutyne.org/metrics.html#epoch-metrics).
 
 
 ------------------
 
 ## Installation
 
 Before installing Poutyne, you must have the latest version of [PyTorch](https://pytorch.org/) in your environment.
```

### Comparing `Poutyne-1.8/poutyne/framework/callbacks/callbacks.py` & `Poutyne-1.9/poutyne/framework/callbacks/callbacks.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,19 +16,36 @@
 Copyright (c) 2017, Microsoft, Inc.
 All rights reserved.
 
 All other contributions:
 Copyright (c) 2015 - 2017, the respective contributors.
 All rights reserved.
 
+Copyright (c) 2022 Poutyne.
+
 Each contributor holds copyright over their respective contributions. The project versioning (Git)
-records all such contribution source information.
+records all such contribution source information on the Poutyne and Keras repository.
 
 LICENSE
 
+The LGPLv3 License
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+
+
 The MIT License (MIT)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software without restriction,
 including without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -38,14 +55,15 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
+
 from typing import Dict, List
 
 
 class Callback:
     # pylint: disable=too-many-public-methods
     """
     Attributes:
```

### Comparing `Poutyne-1.8/poutyne/framework/callbacks/color_formatting.py` & `Poutyne-1.9/poutyne/framework/callbacks/color_formatting.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 import math
 import sys
 import time
 import warnings
 from typing import Dict, Union
 
 from poutyne import is_in_jupyter_notebook
```

### Comparing `Poutyne-1.8/poutyne/framework/callbacks/earlystopping.py` & `Poutyne-1.9/poutyne/framework/callbacks/earlystopping.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-The source code of this file was copied from the Keras project, and has been modified.
+The source code of this file was copied from the Keras project, and has been modified. All modifications
+made from the original source code are under the LGPLv3 license.
 
 COPYRIGHT
 
 All contributions by François Chollet:
 Copyright (c) 2015, François Chollet.
 All rights reserved.
 
@@ -15,19 +16,36 @@
 Copyright (c) 2017, Microsoft, Inc.
 All rights reserved.
 
 All other contributions:
 Copyright (c) 2015 - 2017, the respective contributors.
 All rights reserved.
 
+Copyright (c) 2022 Poutyne.
+
 Each contributor holds copyright over their respective contributions. The project versioning (Git)
-records all such contribution source information.
+records all such contribution source information on the Poutyne and Keras repository.
 
 LICENSE
 
+The LGPLv3 License
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+
+
 The MIT License (MIT)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software without restriction,
 including without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -37,14 +55,15 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
+
 from typing import Dict
 
 import numpy as np
 
 from .callbacks import Callback
```

### Comparing `Poutyne-1.8/poutyne/framework/callbacks/gradient_logger.py` & `Poutyne-1.9/poutyne/framework/callbacks/gradient_logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 import os
 from typing import Dict, List, Union, Optional, TextIO
 import csv
 
 import torch
 
 from ._utils import atomic_lambda_save
```

### Comparing `Poutyne-1.8/poutyne/framework/callbacks/logger.py` & `Poutyne-1.9/poutyne/framework/callbacks/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 import csv
 import os
 from typing import Dict, Optional, TextIO
 
 from ._utils import atomic_lambda_save
 from .callbacks import Callback
 
@@ -175,50 +194,60 @@
 
 class TensorBoardLogger(Logger):
     """
     Callback that outputs the result of each epoch_number or batch into a Tensorboard experiment folder.
 
     Args:
         writer (~torch.utils.tensorboard.writer.SummaryWriter): The tensorboard writer.
+        split_train_val (bool): Whether to put each training and validation metric in the same graphs.
+            (Default = False)
 
     Example:
         Using TensorBoardLogger::
 
             from torch.utils.tensorboard import SummaryWriter
             from poutyne import Model, TensorBoardLogger
 
             writer = SummaryWriter('runs')
             tb_logger = TensorBoardLogger(writer)
 
             model = Model(...)
             model.fit_generator(..., callbacks=[tb_logger])
     """
 
-    def __init__(self, writer):
+    def __init__(self, writer, split_train_val: bool = False):
         super().__init__(batch_granularity=False)
         self.writer = writer
+        self.split_train_val = split_train_val
 
     def _on_train_batch_end_write(self, batch_number: int, logs):
         """
         We don't handle tensorboard writing on batch granularity
         """
         pass
 
     def _on_epoch_end_write(self, epoch_number: int, logs: dict):
-        grouped_items = {}
-        for k, v in logs.items():
-            if 'val_' in k:
-                primary_key = k[4:]
-                if primary_key not in grouped_items:
-                    grouped_items[primary_key] = {}
-                grouped_items[k[4:]][k] = v
-            else:
-                if k not in grouped_items:
-                    grouped_items[k] = {}
-                grouped_items[k][k] = v
-        for k, v in grouped_items.items():
-            self.writer.add_scalars(k, v, epoch_number)
         lr = self._get_current_learning_rates()
-        self.writer.add_scalars('lr', lr, epoch_number)
+
+        if not self.split_train_val:
+            grouped_items = {}
+            for k, v in logs.items():
+                if 'val_' in k:
+                    primary_key = k[4:]
+                    if primary_key not in grouped_items:
+                        grouped_items[primary_key] = {}
+                    grouped_items[k[4:]][k] = v
+                else:
+                    if k not in grouped_items:
+                        grouped_items[k] = {}
+                    grouped_items[k][k] = v
+
+            for k, v in grouped_items.items():
+                self.writer.add_scalars(k, v, epoch_number)
+            self.writer.add_scalars('lr', lr, epoch_number)
+        else:
+            metrics = {**logs, **lr}
+            for metric_name, metric_value in metrics.items():
+                self.writer.add_scalar(metric_name, metric_value, epoch_number)
 
     def _on_train_end_write(self, logs: Dict):
         self.writer.close()
```

### Comparing `Poutyne-1.8/poutyne/framework/callbacks/lr_scheduler.py` & `Poutyne-1.9/poutyne/framework/callbacks/lr_scheduler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 import inspect
 import sys
 from typing import Dict, BinaryIO
 
 import torch.optim.lr_scheduler
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler
```

### Comparing `Poutyne-1.8/poutyne/framework/callbacks/mlflow_logger.py` & `Poutyne-1.9/poutyne/framework/callbacks/mlflow_logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 # pylint: disable=line-too-long, pointless-string-statement
 import os
 import warnings
 from typing import Dict, Union, Mapping, Sequence
 
 from . import Logger
 
@@ -20,115 +39,113 @@
 
 class MLFlowLogger(Logger):
     """
     MLflow logger to manage logging of experiments parameters, metrics update, models log and other information. The
     logger will log all run into the same experiment.
 
     Args:
-        experiment_name (str): The name of the experiment. Name must be unique and are case sensitive.
+        experiment_name (str): The name of the experiment. The name must be unique and are case-sensitive.
         tracking_uri (Union[str, None]): Either the URI tracking path (for server tracking) of the absolute path to
             the directory to save the files (for file store). For example: ``http://<ip address>:<port>``
             (remote server) or ``/home/<user>/mlflow-server`` (local server).
             If None, will use the default MLflow file tracking URI ``"./mlruns"``.
         batch_granularity (bool): Whether to also output the result of each batch in addition to the epochs.
             (Default value = False)
 
     Example:
         Using file store::
 
             mlflow_logger = MLFlowLogger(experiment_name="experiment", tracking_uri="/absolute/path/to/directory")
             mlflow_logger.log_config_params(config_params=cfg_dict) # logging the config dictionary
 
-            # our Poutyne experiment
-            experiment = Experiment(directory=saving_directory, network=network, device=device, optimizer=optimizer,
-                            loss_function=cross_entropy_loss, batch_metrics=[accuracy])
+            # our Poutyne model bundle
+            model_bundle = ModelBundle.from_network(directory=saving_directory, network=network, optimizer=optimizer,
+                                                    loss_function=cross_entropy_loss, batch_metrics=[accuracy],
+                                                    device=device)
 
             # Using the MLflow logger callback during training
-            experiment.train(train_generator=train_loader, valid_generator=valid_loader, epochs=1,
-                             seed=42, callbacks=[mlflow_logger])
+            model_bundle.train(train_generator=train_loader, valid_generator=valid_loader, epochs=1,
+                               seed=42, callbacks=[mlflow_logger])
 
         Using server tracking::
 
             mlflow_logger = MLFlowLogger(experiment_name="experiment", tracking_uri="http://IP_ADDRESS:PORT")
             mlflow_logger.log_config_params(config_params=cfg_dict) # logging the config dictionary
 
-            # our Poutyne experiment
-            experiment = Experiment(directory=saving_directory, network=network, device=device, optimizer=optimizer,
-                            loss_function=cross_entropy_loss, batch_metrics=[accuracy])
+            # our Poutyne model bundle
+            model_bundle = ModelBundle.from_network(directory=saving_directory, network=network, optimizer=optimizer,
+                                                    loss_function=cross_entropy_loss, batch_metrics=[accuracy],
+                                                    device=device)
 
             # Using the MLflow logger callback during training
-            experiment.train(train_generator=train_loader, valid_generator=valid_loader, epochs=1,
-                             seed=42, callbacks=[mlflow_logger])
+            model_bundle.train(train_generator=train_loader, valid_generator=valid_loader, epochs=1,
+                               seed=42, callbacks=[mlflow_logger])
     """
 
     def __init__(
         self, experiment_name: str, tracking_uri: Union[str, None] = None, batch_granularity: bool = False
     ) -> None:
         super().__init__(batch_granularity=batch_granularity)
         if mlflow is None:
             raise ImportError("Mlflow needs to be installed to use this callback.")
 
         self.tracking = tracking_uri
 
-        self._working_directory = os.getcwd()  # for Git
+        self._working_directory = os.getcwd()  # For Git hash monitoring.
 
         self.ml_flow_client = MlflowClient(tracking_uri=self.tracking)
 
         self._handle_experiment_id(experiment_name)
         self.run_id = self.ml_flow_client.create_run(experiment_id=self.experiment_id).info.run_id
 
         self._log_git_version()
 
-        self._status = "FAILED"  # base case is a failure
+        self._status = "FAILED"  # Base case is a failure.
 
-    def log_config_params(self, config_params: Union[Mapping, Sequence]) -> None:
+    def log_config_params(self, config_params: Mapping) -> None:
         """
         Args:
-            config_params (Union[Mapping, Sequence]):
+            config_params (Mapping):
                 The config parameters of the training to log, such as number of epoch, loss function, optimizer etc.
         """
-        if isinstance(config_params, Mapping):
-            for param_name, element in config_params.items():
-                self._log_config_write(param_name, element)
-        else:  # equivalent to "if isinstance(config_params, Sequence):"
-            for idx, element in enumerate(config_params):
-                self._log_config_write(str(idx), element)
+        for param_name, element in config_params.items():
+            self._log_config_write(param_name, element)
 
     def log_param(self, param_name: str, value: Union[str, float]) -> None:
         """
         Log the value of a parameter into the experiment.
 
         Args:
             param_name (str): The name of the parameter.
-            value (Union[str, float]: The value of the parameter.
+            value (Union[str, float]): The value of the parameter.
 
         """
         self.ml_flow_client.log_param(run_id=self.run_id, key=param_name, value=value)
 
     def log_metric(self, metric_name: str, value: float, step: Union[int, None] = None) -> None:
         """
         Log the value of a metric into the experiment.
 
         Args:
             metric_name (str): The name of the metric.
             value (float): The value of the metric.
-            step (Union[int, None]): The step when the metric was compute (Default = None).
+            step (Union[int, None]): The step when the metric was computed (Default = None).
         """
         self.ml_flow_client.log_metric(run_id=self.run_id, key=metric_name, value=value, step=step)
 
     def _log_config_write(self, parent_name: str, element: Union[int, float, str, Mapping, Sequence]) -> None:
         """
         Log the config parameters when it's a mapping or a sequence of elements.
         """
         if isinstance(element, Mapping):
             for key, value in element.items():
-                # We recursively open the element (Dict format type)
+                # We recursively open the element (Dict format type).
                 self._log_config_write(f"{parent_name}.{key}", value)
         elif isinstance(element, Sequence) and not isinstance(element, str):
-            # Since str are sequence we negate it to be log in the else
+            # Since str are sequence we negate it to be logged in the else.
             for idx, value in enumerate(element):
                 self._log_config_write(f"{parent_name}.{idx}", value)
         else:
             self.log_param(parent_name, element)
 
     def _on_train_batch_end_write(self, batch_number: int, logs: Dict) -> None:
         """
@@ -159,39 +176,39 @@
         """
         Log the last epoch batch and epoch metric.
         """
         last_epoch = self.params["epochs"]
         self.log_metric("last-epoch", last_epoch)
 
     def on_test_begin(self, logs: Dict):
-        self._status = "FAILED"  # to change status from FINISHED to FAILED (base case) if trained before
+        self._status = "FAILED"  # To change status from FINISHED to FAILED (base case) if trained before.
         self._status_handling()
 
     def on_test_end(self, logs: Dict):
         """
         Log the test results.
         """
-        if len(logs) > 0:  # to manage failure of the test loop
+        if len(logs) > 0:  # To manage failure of the test loop.
             self._on_test_end_write(logs)
             self._status = "FINISHED"
 
         mlflow.end_run()
         self._status_handling()
 
     def _on_test_end_write(self, logs: Dict) -> None:
         for key, value in logs.items():
             self.log_metric(key, value)
 
     def _status_handling(self):
-        # we set_terminated the run to get the finishing status (FINISHED or FAILED)
+        # We set_terminated the run to get the finishing status (FINISHED or FAILED)
         self.ml_flow_client.set_terminated(self.run_id, status=self._status)
 
     def _handle_experiment_id(self, experiment_name):
         """
-        Handle if the experiment name already exist to grad the id and append new experiment to it.
+        Handle the existing experiment name to grab the id and append a new experiment to it.
         """
         try:
             self.experiment_id = self.ml_flow_client.create_experiment(experiment_name, self.tracking)
         except MlflowException:
             self.experiment_id = self.ml_flow_client.get_experiment_by_name(experiment_name).experiment_id
 
     def _log_git_version(self):
@@ -200,15 +217,15 @@
         """
         source_version = _get_git_commit(self._working_directory)
         if source_version is not None:
             self.ml_flow_client.set_tag(self.run_id, "mlflow.source.git.commit", source_version)
 
 
 """
-The source code of the function _get_git_commit was inspired from the MLflow project
+The source code of the function _get_git_commit was inspired by the MLflow project
 (https://github.com/mlflow/mlflow/blob/7fde53e497c50b4eb4da1e9988710695b8c2e093/mlflow/tracking/context/git_context.py#L11),
 and has been modified. All modifications made from the original source code are under the LGPLv3 license.
 
 COPYRIGHT
 
 All contributions by MLflow:
 Copyright (c) 2020, MLFlow.
```

### Comparing `Poutyne-1.8/poutyne/framework/callbacks/notification.py` & `Poutyne-1.9/poutyne/framework/callbacks/notification.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 from abc import ABC, abstractmethod
 from typing import Dict, Union
 
 from . import Callback
 
 
 class Notificator(ABC):
@@ -100,13 +119,13 @@
 
     def on_test_end(self, logs: Dict) -> None:
         """
         Send the message to the channel 'End of the testing' or
         'End of the testing for the experiment experiment_name' if an experiment name is given.
         """
 
-        message = f"Here the epoch metrics: \n{self._format_logs(logs)}"
+        message = f"Here the test metrics: \n{self._format_logs(logs)}"
         self.notificator.send_notification(message, subject=f"End of the testing{self.experiment_name_msg}.")
 
     @staticmethod
     def _format_logs(logs: Dict) -> str:
         return " ".join([f"{key}: {value}\n" for key, value in logs.items()])
```

### Comparing `Poutyne-1.8/poutyne/framework/callbacks/periodic.py` & `Poutyne-1.9/poutyne/framework/callbacks/periodic.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,19 +16,36 @@
 Copyright (c) 2017, Microsoft, Inc.
 All rights reserved.
 
 All other contributions:
 Copyright (c) 2015 - 2017, the respective contributors.
 All rights reserved.
 
+Copyright (c) 2022 Poutyne.
+
 Each contributor holds copyright over their respective contributions. The project versioning (Git)
-records all such contribution source information.
+records all such contribution source information on the Poutyne and Keras repository.
 
 LICENSE
 
+The LGPLv3 License
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+
+
 The MIT License (MIT)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software without restriction,
 including without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -38,33 +55,35 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
+
 import os
 import warnings
 from typing import IO, Dict, Optional, Callable
+from abc import ABC, abstractmethod
 
 from ._utils import atomic_lambda_save
 from .callbacks import Callback
 
 
-class PeriodicSaveCallback(Callback):
+class PeriodicSaveCallback(ABC, Callback):
     """
-    Write a file (or checkpoint) after every epoch. `filename` can contain named formatting options,
-    which will be filled the value of `epoch` and keys in `logs` (passed in `on_epoch_end`). For
-    example: if `filename` is `weights.{epoch:02d}-{val_loss:.2f}.txt`, then `save_file()` will be
+    Write a file (or checkpoint) after every epoch. ``filename`` can contain named formatting options,
+    which will be filled the value of ``epoch`` and keys in ``logs`` (passed in ``on_epoch_end``). For
+    example: if ``filename`` is ``weights.{epoch:02d}-{val_loss:.2f}.txt``, then ``save_file()`` will be
     called with a file descriptor for a file with the epoch number and the validation loss in the
     filename.
 
     By default, the file is written atomically to the specified filename so that the training can
     be killed and restarted later using the same filename for periodic file saving. To do so, a
-    temporary file is created with the name of `filename + '.tmp'` and is then moved to the final
+    temporary file is created with the name of ``filename + '.tmp'`` and is then moved to the final
     destination after the checkpoint is done. The ``temporary_filename`` argument allows to change the
     path of this temporary file.
 
     Args:
         filename (str): Path to save the model file.
         monitor (str): Quantity to monitor.
             (Default value = 'val_loss')
@@ -105,15 +124,15 @@
         restore_best: bool = False,
         period: int = 1,
         verbose: bool = False,
         temporary_filename: Optional[str] = None,
         atomic_write: bool = True,
         open_mode: str = 'wb',
         read_mode: str = 'rb',
-    ):
+    ) -> None:
         super().__init__()
         self.filename = filename
         self.monitor = monitor
         self.verbose = verbose
         self.save_best_only = save_best_only
         self.keep_only_last_best = keep_only_last_best
         self.restore_best = restore_best
@@ -136,58 +155,78 @@
                 self.current_best = float('Inf')
             elif mode == 'max':
                 self.monitor_op = lambda x, y: x > y
                 self.current_best = -float('Inf')
 
         self.period = period
 
-    def save_file(self, fd: IO, epoch_number: int, logs: Dict):
-        raise NotImplementedError
+    @abstractmethod
+    def save_file(self, fd: IO, epoch_number: int, logs: Dict) -> None:
+        """
+        Abstract method that is called every time a save needs to be done.
+
+        Args:
+            fd (IO): The descriptor of the file in which to write.
+            epoch_number (int): The epoch number.
+            logs (Dict): Dictionary passed on epoch end.
+        """
+        pass
 
-    def _save_file(self, filename: str, epoch_number: int, logs: Dict):
+    def _save_file(self, filename: str, epoch_number: int, logs: Dict) -> None:
         atomic_lambda_save(
             filename,
             self.save_file,
             (epoch_number, logs),
             temporary_filename=self.temporary_filename,
             open_mode=self.open_mode,
             atomic=self.atomic_write,
         )
 
-    def on_epoch_end(self, epoch_number: int, logs: Dict):
+    def on_epoch_end(self, epoch_number: int, logs: Dict) -> None:
         filename = self.filename.format_map(logs)
 
         if self.save_best_only:
-            if self.monitor_op(logs[self.monitor], self.current_best):
-                old_best = self.current_best
-                self.current_best = logs[self.monitor]
-                old_best_filename = self.best_filename
-                self.best_filename = filename
-
-                if self.verbose:
-                    print(
-                        f'Epoch {epoch_number:d}: {self.monitor} improved from {old_best:0.5f} '
-                        f'to {self.current_best:0.5f}, saving file to {self.best_filename}'
-                    )
-                self._save_file(self.best_filename, epoch_number, logs)
-                if (
-                    self.keep_only_last_best
-                    and self.best_filename != old_best_filename
-                    and old_best_filename is not None
-                ):
-                    os.remove(old_best_filename)
+            if self.monitor in logs:
+                if self.monitor_op(logs[self.monitor], self.current_best):
+                    old_best = self.current_best
+                    self.current_best = logs[self.monitor]
+                    old_best_filename = self.best_filename
+                    self.best_filename = filename
+
+                    if self.verbose:
+                        print(
+                            f'Epoch {epoch_number:d}: {self.monitor} improved from {old_best:0.5f} '
+                            f'to {self.current_best:0.5f}, saving file to {self.best_filename}'
+                        )
+                    self._save_file(self.best_filename, epoch_number, logs)
+                    if (
+                        self.keep_only_last_best
+                        and self.best_filename != old_best_filename
+                        and old_best_filename is not None
+                    ):
+                        os.remove(old_best_filename)
+            else:
+                raise KeyError(f"The monitored metric name {self.monitor} is not found in computed metrics.")
         elif epoch_number % self.period == 0:
             if self.verbose:
                 print(f'Epoch {epoch_number:d}: saving file to {filename}')
             self._save_file(filename, epoch_number, logs)
 
-    def restore(self, fd: IO):
-        raise NotImplementedError
+    @abstractmethod
+    def restore(self, fd: IO) -> None:
+        """
+        Abstract method that is called when a save needs to be restored. This happens at the end of the training when
+        ``restore_best`` is true.
+
+        Args:
+            fd (IO): The descriptor of the file to read.
+        """
+        pass
 
-    def on_train_end(self, logs: Dict):
+    def on_train_end(self, logs: Dict) -> None:
         if self.restore_best:
             if self.best_filename is not None:
                 if self.verbose:
                     print(f'Restoring data from {self.best_filename}')
                 # pylint: disable=unspecified-encoding
                 open_kwargs = dict(encoding='utf-8') if 'b' not in self.read_mode else {}
                 with open(self.best_filename, self.read_mode, **open_kwargs) as fd:
@@ -207,18 +246,18 @@
         restore (Callable[[fd], None]): The lambda that will be called with a file descriptor to restore
             the state if necessary.
 
     See:
         :class:`~poutyne.PeriodicSaveCallback`
     """
 
-    def __init__(self, func: Callable, *args, restore: Optional[Callable] = None, **kwargs):
+    def __init__(self, func: Callable, *args, restore: Optional[Callable] = None, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.func = func
         self._restore = restore
 
-    def save_file(self, fd: IO, epoch_number: int, logs: Dict):
+    def save_file(self, fd: IO, epoch_number: int, logs: Dict) -> None:
         self.func(fd, epoch_number, logs)
 
-    def restore(self, fd: IO):
+    def restore(self, fd: IO) -> None:
         if self._restore is not None:
             self._restore(fd)
```

### Comparing `Poutyne-1.8/poutyne/framework/callbacks/policies.py` & `Poutyne-1.9/poutyne/framework/callbacks/policies.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 import contextlib
 from collections import OrderedDict
 from itertools import islice, chain
 from math import cos, pi
 from typing import Dict, List, Tuple, Optional
 
 try:
@@ -201,15 +220,15 @@
     Returns:
         A list of configured :class:`~poutyne.Phase` instances.
 
     References:
         `SGDR: Stochastic Gradient Descent with Warm Restarts
         <https://arxiv.org/abs/1608.03983>`_
     """
-    steps = [base_cycle_length * (cycle_mult ** i) for i in range(cycles)]
+    steps = [base_cycle_length * (cycle_mult**i) for i in range(cycles)]
     return [Phase(lr=cosinespace(lr[0], lr[1], step)) for step in steps]
 
 
 ###############################################################################
 class OptimizerPolicy(Callback):
     """
     Combine different :class:`~poutyne.Phase` instances
```

### Comparing `Poutyne-1.8/poutyne/framework/callbacks/progress.py` & `Poutyne-1.9/poutyne/framework/callbacks/progress.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 import itertools
 from typing import Dict, Callable
 
 from .callbacks import Callback
 from .color_formatting import ColorProgress
```

### Comparing `Poutyne-1.8/poutyne/framework/callbacks/progress_bar.py` & `Poutyne-1.9/poutyne/framework/callbacks/progress_bar.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 import math
 from typing import Optional
 
 BAR_EIGHTHS_CHARACTERS = [" ", "\u258f", "\u258e", "\u258d", "\u258c", "\u258b", "\u258a", "\u2589"]
 
 
 class ProgressBar:
```

### Comparing `Poutyne-1.8/poutyne/framework/callbacks/tracker.py` & `Poutyne-1.9/poutyne/framework/callbacks/gradient_tracker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 from typing import Dict, List, Tuple, Iterable
 
 import numpy as np
 import torch
 
 from .callbacks import Callback
 
@@ -9,17 +28,20 @@
 class WeightsGradientsStatsTracker:
     """
     The weights' gradient statistic tracker will estimate the absolute mean (i.e. the mean of the absolute values of
     the weights' gradients), running absolute mean variance (i.e. the variance of the absolute mean), min, absolute min,
      max and absolute max per layer. The tracker is using the `Welford's online algorithm
      <https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance#Welford's_online_algorithm>`_
     to estimate the running mean and running variance of the absolute weights' gradients.
+
+    Args:
+        number_layers (int): The number of layers to track stats on.
     """
 
-    def __init__(self, number_layers) -> None:
+    def __init__(self, number_layers: int) -> None:
         self.number_layers = number_layers
 
         self.reset()
 
     def batch_statistic_upgrade(self, named_parameters: Iterable[Tuple[str, torch.nn.parameter.Parameter]]) -> None:
         """
         Accumulate the running absolute mean, running absolute mean variance, min, absolute min, max ant the absolute
@@ -114,38 +136,38 @@
         self.running_min = np.zeros([self.number_layers], dtype="float32")
         self.running_abs_min = np.zeros([self.number_layers], dtype="float32")
         self.running_max = np.zeros([self.number_layers], dtype="float32")
         self.running_abs_max = np.zeros([self.number_layers], dtype="float32")
         self.count = 1
 
 
-class Tracker(Callback):
+class GradientTracker(Callback):
     def __init__(self, keep_bias: bool = False) -> None:
         super().__init__()
 
         self.keep_bias = keep_bias
         self.layer_names = []
         self.number_layers = 0
 
         self.tracker = None
 
-    def on_train_batch_end(self, batch_number: int, logs: Dict):
+    def on_train_batch_end(self, batch_number: int, logs: Dict) -> None:
         # pylint: disable=unused-argument
         named_parameters = ((n, p) for n, p in self.model.network.named_parameters() if self._keep_layer(p, n))
         self.tracker.batch_statistic_upgrade(named_parameters)
 
-    def on_train_begin(self, logs: Dict):
+    def on_train_begin(self, logs: Dict) -> None:
         for layer_name, layer_params in self.model.network.named_parameters():
             self._update_layers_to_track(layer_name, layer_params)
         self.tracker = WeightsGradientsStatsTracker(self.number_layers)
 
-    def on_epoch_end(self, epoch_number: int, logs: Dict):
+    def on_epoch_end(self, epoch_number: int, logs: Dict) -> None:
         self._on_epoch_end_log(epoch_number, logs)
 
-    def _on_epoch_end_log(self, epoch_number: int, logs: Dict):
+    def _on_epoch_end_log(self, epoch_number: int, logs: Dict) -> None:
         """
         The method to define the behavior of the logging tracker.
 
         Args:
             epoch_number (int): The epoch number.
             logs (Dict): The epoch logs dictionary.
         """
@@ -153,22 +175,22 @@
 
     def _update_layers_to_track(self, layer_name: str, layer_params: torch.nn.parameter.Parameter):
         if self._keep_layer(layer_params, layer_name):
             self.layer_names.append(layer_name)
 
         self.number_layers = len(self.layer_names)
 
-    def _keep_layer(self, layer_params: torch.nn.parameter.Parameter, layer_name: str):
+    def _keep_layer(self, layer_params: torch.nn.parameter.Parameter, layer_name: str) -> bool:
         layer_require_grad = layer_params.requires_grad
         if self.keep_bias:
             return layer_require_grad
         return layer_require_grad and ("bias" not in layer_name)
 
 
-class TensorBoardGradientTracker(Tracker):
+class TensorBoardGradientTracker(GradientTracker):
     """
     Wrapper to track the statistics of the weights' gradient per layer and log them in TensorBoard per epoch.
 
     Args:
         writer (~torch.utils.tensorboard.writer.SummaryWriter): The TensorBoard writer.
         keep_bias (bool): Either or not to log the bias of the network.
```

### Comparing `Poutyne-1.8/poutyne/framework/experiment.py` & `Poutyne-1.9/poutyne/framework/model_bundle.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 # pylint: disable=too-many-lines
 import os
 import warnings
 from typing import Union, Callable, List, Dict, Tuple, Any
 
 try:
     import pandas as pd
@@ -33,169 +52,22 @@
     PeriodicSaveLambda,
     AtomicCSVLogger,
     TensorBoardLogger,
     BestModelRestore,
 )
 
 
-class Experiment:
+class ModelBundle:
     """
-    The Experiment class provides a straightforward experimentation tool for efficient and entirely
+    The :class:`~poutyne.ModelBundle` class provides a straightforward experimentation tool for efficient and entirely
     customizable finetuning of the whole neural network training procedure with PyTorch. The
-    ``Experiment`` object takes care of the training and testing processes while also managing to
-    keep traces of all pertinent information via the automatic logging option.
-
-    Args:
-        directory (str): Path to the experiment's working directory. Will be used for automatic logging.
-        network (torch.nn.Module): A PyTorch network.
-        device (Union[torch.torch.device, List[torch.torch.device], str, None]): The device to which the model is sent
-            or for multi-GPUs, the list of devices to which the model is to be sent. When using a string for a multiple
-            GPUs, the option is "all", for "take them all." By default, the current device is used as the main one.
-            If None, the model will be kept on its current device.
-            (Default value = None)
-        logging (bool): Whether or not to log the experiment's progress. If true, various logging
-            callbacks will be inserted to output training and testing stats as well as to save model checkpoints,
-            for example, automatically. See :func:`~Experiment.train()` and :func:`~Experiment.test()` for more details.
-            (Default value = True)
-        optimizer (Union[torch.optim.Optimizer, str]): If Pytorch Optimizer, must already be initialized.
-            If str, should be the optimizer's name in Pytorch (i.e. 'Adam' for torch.optim.Adam).
-            (Default value = 'sgd')
-        loss_function(Union[Callable, str], optional) It can be any PyTorch
-            loss layer or custom loss function. It can also be a string with the same name as a PyTorch
-            loss function (either the functional or object name). The loss function must have the signature
-            ``loss_function(input, target)`` where ``input`` is the prediction of the network and ``target``
-            is the ground truth. If ``None``, will default to, in priority order, either the model's own
-            loss function or the default loss function associated with the ``task``.
-            (Default value = None)
-        batch_metrics (list): List of functions with the same signature as the loss function. Each metric
-            can be any PyTorch loss function. It can also be a string with the same name as a PyTorch
-            loss function (either the functional or object name). Furthermore, see :ref:`batch metrics`
-            for supplementary available batch metrics. 'accuracy' (or just 'acc') is an often used metric.
-            Each metric function is called on each batch of the optimization and on the validation batches
-            at the end of the epoch.
-            (Default value = None)
-        epoch_metrics (list): List of functions with the same signature as :class:`~poutyne.EpochMetric`.
-            See :ref:`epoch metrics` for available epoch metrics. (Default value = None)
-        monitoring (bool): Whether or not to monitor the training. If True will track the best epoch.
-            If False, ``monitor_metric`` and ``monitor_mode`` are not used, and when testing, the last epoch is used to
-            test the model instead of the best epoch.
-            (Default value = True)
-        monitor_metric (str, optional): Which metric to consider for best model performance calculation. Should be in
-            the format '{metric_name}' or 'val_{metric_name}' (i.e. 'val_loss'). If None, will follow the value
-            suggested by ``task`` or default to 'val_loss'. If ``monitoring`` is set to False, will be ignore.
-
-            .. warning:: If you do not plan on using a validation set, you must set the monitor metric to another
-                value.
-        monitor_mode (str, optional): Which mode, either 'min' or 'max', should be used when considering the
-            ``monitor_metric`` value. If None, will follow the value suggested by ``task`` or default to 'min'.
-            If ``monitoring`` is set to False, will be ignore.
-        task (str, optional): Any str beginning with either 'classif' or 'reg'. Specifying a ``task``
-            can assign default values to the ``loss_function``, ``batch_metrics``, ``monitor_mode`` and
-            ``monitor_mode``. For ``task`` that begins with 'reg', the only default value is the loss function
-            that is the mean squared error. When beginning with 'classif', the default loss function is the
-            cross-entropy loss. The default batch metrics will be the accuracy, the default epoch metrics will be
-            the F1 score and the default monitoring will be set on 'val_acc' with a 'max' mode.
-            (Default value = None)
-
-    Examples:
-        Using a PyTorch DataLoader, on classification task with SGD optimizer::
-
-            import torch
-            from torch.utils.data import DataLoader, TensorDataset
-            from poutyne import Experiment
-
-            num_features = 20
-            num_classes = 5
-
-            # Our training dataset with 800 samples.
-            num_train_samples = 800
-            train_x = torch.rand(num_train_samples, num_features)
-            train_y = torch.randint(num_classes, (num_train_samples, ), dtype=torch.long)
-            train_dataset = TensorDataset(train_x, train_y)
-            train_generator = DataLoader(train_dataset, batch_size=32)
-
-            # Our validation dataset with 200 samples.
-            num_valid_samples = 200
-            valid_x = torch.rand(num_valid_samples, num_features)
-            valid_y = torch.randint(num_classes, (num_valid_samples, ), dtype=torch.long)
-            valid_dataset = TensorDataset(valid_x, valid_y)
-            valid_generator = DataLoader(valid_dataset, batch_size=32)
-
-            # Our network
-            pytorch_network = torch.nn.Linear(num_features, num_train_samples)
-
-            # Initialization of our experimentation and network training
-            exp = Experiment('./simple_example',
-                             pytorch_network,
-                             optimizer='sgd',
-                             task='classif')
-            exp.train(train_generator, valid_generator, epochs=5)
-
-    The above code will yield an output similar to the below lines. Note the automatic checkpoint saving
-    in the experiment directory when the monitored metric improved.
-
-    .. code-block:: none
-
-            Epoch 1/5 0.09s Step 25/25: loss: 6.351375, acc: 1.375000, val_loss: 6.236106, val_acc: 5.000000
-            Epoch 1: val_acc improved from -inf to 5.00000, saving file to ./simple_example/checkpoint_epoch_1.ckpt
-            Epoch 2/5 0.10s Step 25/25: loss: 6.054254, acc: 14.000000, val_loss: 5.944495, val_acc: 19.500000
-            Epoch 2: val_acc improved from 5.00000 to 19.50000, saving file to ./simple_example/checkpoint_epoch_2.ckpt
-            Epoch 3/5 0.09s Step 25/25: loss: 5.759377, acc: 22.875000, val_loss: 5.655412, val_acc: 21.000000
-            Epoch 3: val_acc improved from 19.50000 to 21.00000, saving file to ./simple_example/checkpoint_epoch_3.ckpt
-            ...
-
-    Training can now easily be resumed from the best checkpoint::
-
-            exp.train(train_generator, valid_generator, epochs=10)
-
-    .. code-block:: none
-
-            Restoring model from ./simple_example/checkpoint_epoch_3.ckpt
-            Loading weights from ./simple_example/checkpoint.ckpt and starting at epoch 6.
-            Loading optimizer state from ./simple_example/checkpoint.optim and starting at epoch 6.
-            Epoch 6/10 0.16s Step 25/25: loss: 4.897135, acc: 22.875000, val_loss: 4.813141, val_acc: 20.500000
-            Epoch 7/10 0.10s Step 25/25: loss: 4.621514, acc: 22.625000, val_loss: 4.545359, val_acc: 20.500000
-            Epoch 8/10 0.24s Step 25/25: loss: 4.354721, acc: 23.625000, val_loss: 4.287117, val_acc: 20.500000
-            ...
-
-    Testing is also very intuitive::
-
-            exp.test(test_generator)
-
-    .. code-block:: none
-
-            Restoring model from ./simple_example/checkpoint_epoch_9.ckpt
-            Found best checkpoint at epoch: 9
-            lr: 0.01, loss: 4.09892, acc: 23.625, val_loss: 4.04057, val_acc: 21.5
-            On best model: test_loss: 4.06664, test_acc: 17.5
-
-
-    Finally, all the pertinent metrics specified to the Experiment at each epoch are stored in a specific logging
-    file, found here at './simple_example/log.tsv'.
-
-    .. code-block:: none
-
-            epoch	time	            lr	    loss	            acc	    val_loss	        val_acc
-            1	    0.0721172170015052	0.01	6.351375141143799	1.375	6.23610631942749	5.0
-            2	    0.0298177790245972	0.01	6.054253826141357	14.000	5.94449516296386	19.5
-            3	    0.0637106419890187	0.01	5.759376544952392	22.875	5.65541223526001	21.0
-            ...
-
-    Also, we could use more than one GPU (on a single node) by using the device argument
-
-    .. code-block:: none
-
-            # Initialization of our experimentation and network training
-            exp = Experiment('./simple_example',
-                             pytorch_network,
-                             optimizer='sgd',
-                             task='classif',
-                             device="all")
-            exp.train(train_generator, valid_generator, epochs=5)
+    :class:`~poutyne.ModelBundle` object takes care of the training and testing processes while also managing to keep
+    traces of all pertinent information via the automatic logging option.
 
+    Use ``ModelBundle.from_*`` methods to instanciate a :class:`~poutyne.ModelBundle`.
     """
 
     BEST_CHECKPOINT_FILENAME = 'checkpoint_epoch_{epoch}.ckpt'
     MODEL_CHECKPOINT_FILENAME = 'checkpoint.ckpt'
     OPTIMIZER_CHECKPOINT_FILENAME = 'checkpoint.optim'
     LOG_FILENAME = 'log.tsv'
     TENSORBOARD_DIRECTORY = 'tensorboard'
@@ -203,119 +75,467 @@
     LR_SCHEDULER_FILENAME = 'lr_sched_%d.lrsched'
     PLOTS_DIRECTORY = 'plots'
     TEST_LOG_FILENAME = '{name}_log.tsv'
 
     def __init__(
         self,
         directory: str,
+        model: Model,
+        *,
+        logging: bool = True,
+        monitoring: bool = True,
+        monitor_metric: Union[str, None] = None,
+        monitor_mode: Union[str, None] = None,
+        _is_direct=True,
+    ) -> None:
+        if _is_direct:
+            raise TypeError("Create a ModelBundle with ModelBundle.from_* methods.")
+
+        if pd is None:
+            raise ImportError("pandas needs to be installed to use the class ModelBundle.")
+
+        self.directory = directory
+        self.model = model
+        self.logging = logging
+
+        self.monitoring = monitoring
+        self.monitor_metric = monitor_metric
+        self.monitor_mode = monitor_mode
+
+        self.set_paths()
+
+    @classmethod
+    def from_network(
+        cls,
+        directory: str,
         network: torch.nn.Module,
         *,
         device: Union[torch.device, List[torch.device], List[str], None, str] = None,
         logging: bool = True,
         optimizer: Union[torch.optim.Optimizer, str] = 'sgd',
         loss_function: Union[Callable, str] = None,
         batch_metrics: Union[List, None] = None,
         epoch_metrics: Union[List, None] = None,
+        torch_metrics: Union[List, None] = None,
         monitoring: bool = True,
         monitor_metric: Union[str, None] = None,
         monitor_mode: Union[str, None] = None,
         task: Union[str, None] = None,
-    ) -> None:
-        if pd is None:
-            raise ImportError("pandas needs to be installed to use the class Experiment.")
+    ):
+        # pylint: disable=line-too-long
+        """
+        Instanciate a :class:`~poutyne.ModelBundle` from a PyTorch :class:`~torch.nn.Module` instance.
 
-        self.directory = directory
-        self.logging = logging
+        Args:
+            directory (str): Path to the model bundle's working directory. Will be used for automatic logging.
+            network (torch.nn.Module): A PyTorch network.
+            device (Union[torch.torch.device, List[torch.torch.device], str, None]): The device to which the model is
+                sent or for multi-GPUs, the list of devices to which the model is to be sent. When using a string for a
+                multiple GPUs, the option is "all", for "take them all." By default, the current device is used as the
+                main one. If None, the model will be kept on its current device.
+                (Default value = None)
+            logging (bool): Whether or not to log the model bundle's progress. If true, various logging
+                callbacks will be inserted to output training and testing stats as well as to save model checkpoints,
+                for example, automatically. See :func:`~ModelBundle.train()` and :func:`~ModelBundle.test()` for more
+                details. (Default value = True)
+            optimizer (Union[torch.optim.Optimizer, str]): If Pytorch Optimizer, must already be initialized.
+                If str, should be the optimizer's name in Pytorch (i.e. 'Adam' for torch.optim.Adam).
+                (Default value = 'sgd')
+            loss_function(Union[Callable, str], optional) It can be any PyTorch
+                loss layer or custom loss function. It can also be a string with the same name as a PyTorch
+                loss function (either the functional or object name). The loss function must have the signature
+                ``loss_function(input, target)`` where ``input`` is the prediction of the network and ``target``
+                is the ground truth. If ``None``, will default to, in priority order, either the model's own
+                loss function or the default loss function associated with the ``task``.
+                (Default value = None)
+            batch_metrics (list): List of functions with the same signature as the loss function. Each metric
+                can be any PyTorch loss function. It can also be a string with the same name as a PyTorch
+                loss function (either the functional or object name). Furthermore, see :ref:`batch metrics`
+                for supplementary available batch metrics. 'accuracy' (or just 'acc') is an often used metric.
+                Each metric function is called on each batch of the optimization and on the validation batches
+                at the end of the epoch.
+                (Default value = None)
+            epoch_metrics (list): List of objects with the same signature as either :class:`~poutyne.EpochMetric` or
+                :class:`torchmetrics.Metric <torchmetrics.Metric>`.
+                See :ref:`epoch metrics` and the
+                `TorchMetrics documentation <https://torchmetrics.readthedocs.io/en/latest/references/modules.html>`__
+                for available epoch metrics. (Default value = None)
+            torch_metrics (list): List of `TorchMetrics <https://torchmetrics.readthedocs.io/>`__  objects.
+                List of objects with the same signature as :class:`torchmetrics.Metric <torchmetrics.Metric>`.
+                See
+                `TorchMetrics documentation <https://torchmetrics.readthedocs.io/en/latest/references/modules.html>`__
+                for available torch metrics. (Default value = None)
+
+                .. warning:: When using this argument, the torch metrics are computed at each batch. This
+                    can significantly slow down the compuations depending on the metrics used. In such case, we advise
+                    to use them as epoch metrics instead.
+            monitoring (bool): Whether or not to monitor the training. If True will track the best epoch.
+                If False, ``monitor_metric`` and ``monitor_mode`` are not used, and when testing, the last epoch is used
+                to test the model instead of the best epoch.
+                (Default value = True)
+            monitor_metric (str, optional): Which metric to consider for best model performance calculation. Should be
+                in the format '{metric_name}' or 'val_{metric_name}' (i.e. 'val_loss'). If None, will follow the value
+                suggested by ``task`` or default to 'val_loss'. If ``monitoring`` is set to False, will be ignore.
+
+                .. warning:: If you do not plan on using a validation set, you must set the monitor metric to another
+                    value.
+            monitor_mode (str, optional): Which mode, either 'min' or 'max', should be used when considering the
+                ``monitor_metric`` value. If None, will follow the value suggested by ``task`` or default to 'min'.
+                If ``monitoring`` is set to False, will be ignore.
+            task (str, optional): Any str beginning with either 'classif' or 'reg'. Specifying a ``task``
+                can assign default values to the ``loss_function``, ``batch_metrics``, ``monitor_mode`` and
+                ``monitor_mode``. For ``task`` that begins with 'reg', the only default value is the loss function
+                that is the mean squared error. When beginning with 'classif', the default loss function is the
+                cross-entropy loss. The default batch metrics will be the accuracy, the default epoch metrics will be
+                the F1 score and the default monitoring will be set on 'val_acc' with a 'max' mode.
+                (Default value = None)
+
+        Examples:
+            Using a PyTorch DataLoader, on classification task with SGD optimizer::
+
+                import torch
+                from torch.utils.data import DataLoader, TensorDataset
+                from poutyne import ModelBundle
+
+                num_features = 20
+                num_classes = 5
+
+                # Our training dataset with 800 samples.
+                num_train_samples = 800
+                train_x = torch.rand(num_train_samples, num_features)
+                train_y = torch.randint(num_classes, (num_train_samples, ), dtype=torch.long)
+                train_dataset = TensorDataset(train_x, train_y)
+                train_generator = DataLoader(train_dataset, batch_size=32)
+
+                # Our validation dataset with 200 samples.
+                num_valid_samples = 200
+                valid_x = torch.rand(num_valid_samples, num_features)
+                valid_y = torch.randint(num_classes, (num_valid_samples, ), dtype=torch.long)
+                valid_dataset = TensorDataset(valid_x, valid_y)
+                valid_generator = DataLoader(valid_dataset, batch_size=32)
+
+                # Our network
+                pytorch_network = torch.nn.Linear(num_features, num_train_samples)
+
+                # Initialization of our experimentation and network training
+                exp = ModelBundle.from_network('./simple_example',
+                                               pytorch_network,
+                                               optimizer='sgd',
+                                               task='classif')
+                exp.train(train_generator, valid_generator, epochs=5)
+
+        The above code will yield an output similar to the below lines. Note the automatic checkpoint saving
+        in the model bundle directory when the monitored metric improved.
+
+        .. code-block:: none
+
+                Epoch 1/5 0.09s Step 25/25: loss: 6.351375, acc: 1.375000, val_loss: 6.236106, val_acc: 5.000000
+                Epoch 1: val_acc improved from -inf to 5.00000, saving file to ./simple_example/checkpoint_epoch_1.ckpt
+                Epoch 2/5 0.10s Step 25/25: loss: 6.054254, acc: 14.000000, val_loss: 5.944495, val_acc: 19.500000
+                Epoch 2: val_acc improved from 5.00000 to 19.50000, saving file to ./simple_example/checkpoint_epoch_2.ckpt
+                Epoch 3/5 0.09s Step 25/25: loss: 5.759377, acc: 22.875000, val_loss: 5.655412, val_acc: 21.000000
+                Epoch 3: val_acc improved from 19.50000 to 21.00000, saving file to ./simple_example/checkpoint_epoch_3.ckpt
+                ...
+
+        Training can now easily be resumed from the best checkpoint::
+
+                exp.train(train_generator, valid_generator, epochs=10)
+
+        .. code-block:: none
 
+                Restoring model from ./simple_example/checkpoint_epoch_3.ckpt
+                Loading weights from ./simple_example/checkpoint.ckpt and starting at epoch 6.
+                Loading optimizer state from ./simple_example/checkpoint.optim and starting at epoch 6.
+                Epoch 6/10 0.16s Step 25/25: loss: 4.897135, acc: 22.875000, val_loss: 4.813141, val_acc: 20.500000
+                Epoch 7/10 0.10s Step 25/25: loss: 4.621514, acc: 22.625000, val_loss: 4.545359, val_acc: 20.500000
+                Epoch 8/10 0.24s Step 25/25: loss: 4.354721, acc: 23.625000, val_loss: 4.287117, val_acc: 20.500000
+                ...
+
+        Testing is also very intuitive::
+
+                exp.test(test_generator)
+
+        .. code-block:: none
+
+                Restoring model from ./simple_example/checkpoint_epoch_9.ckpt
+                Found best checkpoint at epoch: 9
+                lr: 0.01, loss: 4.09892, acc: 23.625, val_loss: 4.04057, val_acc: 21.5
+                On best model: test_loss: 4.06664, test_acc: 17.5
+
+
+        Finally, all the pertinent metrics specified to the ModelBundle at each epoch are stored in a specific logging
+        file, found here at './simple_example/log.tsv'.
+
+        .. code-block:: none
+
+                epoch	time	            lr	    loss	            acc	    val_loss	        val_acc
+                1	    0.0721172170015052	0.01	6.351375141143799	1.375	6.23610631942749	5.0
+                2	    0.0298177790245972	0.01	6.054253826141357	14.000	5.94449516296386	19.5
+                3	    0.0637106419890187	0.01	5.759376544952392	22.875	5.65541223526001	21.0
+                ...
+
+        Also, we could use more than one GPU (on a single node) by using the device argument
+
+        .. code-block:: none
+
+                # Initialization of our experimentation and network training
+                exp = ModelBundle.from_network('./simple_example',
+                                               pytorch_network,
+                                               optimizer='sgd',
+                                               task='classif',
+                                               device="all")
+                exp.train(train_generator, valid_generator, epochs=5)
+
+        """
         if task is not None and not task.startswith('classif') and not task.startswith('reg'):
             raise ValueError(f"Invalid task '{task}'")
 
         batch_metrics = [] if batch_metrics is None else batch_metrics
         epoch_metrics = [] if epoch_metrics is None else epoch_metrics
 
-        loss_function = self._get_loss_function(loss_function, network, task)
-        batch_metrics = self._get_batch_metrics(batch_metrics, network, task)
-        epoch_metrics = self._get_epoch_metrics(epoch_metrics, network, task)
+        loss_function = cls._get_loss_function(loss_function, network, task)
+        batch_metrics = cls._get_batch_metrics(batch_metrics, network, task)
+        epoch_metrics = cls._get_epoch_metrics(epoch_metrics, network, task)
 
-        self.monitoring = monitoring
-        self.monitor_metric = None
-        self.monitor_mode = None
-        if self.monitoring:
-            self._set_monitor(monitor_metric, monitor_mode, task)
+        monitoring, monitor_metric, monitor_mode = cls._get_monitoring_config(
+            monitoring, monitor_metric, monitor_mode, task
+        )
 
-        self.model = Model(
-            network, optimizer, loss_function, batch_metrics=batch_metrics, epoch_metrics=epoch_metrics, device=device
+        model = Model(
+            network,
+            optimizer,
+            loss_function,
+            batch_metrics=batch_metrics,
+            epoch_metrics=epoch_metrics,
+            torch_metrics=torch_metrics,
+            device=device,
         )
 
-        self.best_checkpoint_filename = self.get_path(Experiment.BEST_CHECKPOINT_FILENAME)
-        self.model_checkpoint_filename = self.get_path(Experiment.MODEL_CHECKPOINT_FILENAME)
-        self.optimizer_checkpoint_filename = self.get_path(Experiment.OPTIMIZER_CHECKPOINT_FILENAME)
-        self.log_filename = self.get_path(Experiment.LOG_FILENAME)
-        self.tensorboard_directory = self.get_path(Experiment.TENSORBOARD_DIRECTORY)
-        self.epoch_filename = self.get_path(Experiment.EPOCH_FILENAME)
-        self.lr_scheduler_filename = self.get_path(Experiment.LR_SCHEDULER_FILENAME)
-        self.plots_directory = self.get_path(Experiment.PLOTS_DIRECTORY)
-        self.test_log_filename = self.get_path(Experiment.TEST_LOG_FILENAME)
+        return ModelBundle(
+            directory,
+            model,
+            logging=logging,
+            monitoring=monitoring,
+            monitor_metric=monitor_metric,
+            monitor_mode=monitor_mode,
+            _is_direct=False,
+        )
+
+    @classmethod
+    def from_model(
+        cls,
+        directory: str,
+        model: Model,
+        *,
+        logging: bool = True,
+        monitoring: bool = True,
+        monitor_metric: Union[str, None] = None,
+        monitor_mode: Union[str, None] = None,
+    ):
+        # pylint: disable=line-too-long
+        """
+        Instanciate a :class:`~poutyne.ModelBundle` from a :class:`~poutyne.Model` instance.
+
+        Args:
+            directory (str): Path to the model bundle's working directory. Will be used for automatic logging.
+            model (poutyne.Model): A Model instance..
+            logging (bool): Whether or not to log the model bundle's progress. If true, various logging
+                callbacks will be inserted to output training and testing stats as well as to save model checkpoints,
+                for example, automatically. See :func:`~ModelBundle.train()` and :func:`~ModelBundle.test()` for more
+                details. (Default value = True)
+            monitoring (bool): Whether or not to monitor the training. If True will track the best epoch.
+                If False, ``monitor_metric`` and ``monitor_mode`` are not used, and when testing, the last epoch is used
+                to test the model instead of the best epoch.
+                (Default value = True)
+            monitor_metric (str, optional): Which metric to consider for best model performance calculation. Should be
+                in the format '{metric_name}' or 'val_{metric_name}' (i.e. 'val_loss'). If None, will follow the value
+                suggested by ``task`` or default to 'val_loss'. If ``monitoring`` is set to False, will be ignore.
+
+                .. warning:: If you do not plan on using a validation set, you must set the monitor metric to another
+                    value.
+            monitor_mode (str, optional): Which mode, either 'min' or 'max', should be used when considering the
+                ``monitor_metric`` value. If None, will follow the value suggested by ``task`` or default to 'min'.
+                If ``monitoring`` is set to False, will be ignore.
+
+        Examples:
+            Using a PyTorch DataLoader, on classification task with SGD optimizer::
+
+                import torch
+                from torch.utils.data import DataLoader, TensorDataset
+                from poutyne import Model, ModelBundle
+
+                num_features = 20
+                num_classes = 5
+
+                # Our training dataset with 800 samples.
+                num_train_samples = 800
+                train_x = torch.rand(num_train_samples, num_features)
+                train_y = torch.randint(num_classes, (num_train_samples, ), dtype=torch.long)
+                train_dataset = TensorDataset(train_x, train_y)
+                train_generator = DataLoader(train_dataset, batch_size=32)
+
+                # Our validation dataset with 200 samples.
+                num_valid_samples = 200
+                valid_x = torch.rand(num_valid_samples, num_features)
+                valid_y = torch.randint(num_classes, (num_valid_samples, ), dtype=torch.long)
+                valid_dataset = TensorDataset(valid_x, valid_y)
+                valid_generator = DataLoader(valid_dataset, batch_size=32)
+
+                # Our network
+                pytorch_network = torch.nn.Linear(num_features, num_train_samples)
+
+                model = Model(pytorch_network, 'sgd', 'crossentropy', batch_metrics=['accuracy'])
+
+                # Initialization of our experimentation and network training
+                exp = ModelBundle.from_model('./simple_example', model)
+                exp.train(train_generator, valid_generator, epochs=5)
+
+        The above code will yield an output similar to the below lines. Note the automatic checkpoint saving
+        in the model bundle directory when the monitored metric improved.
+
+        .. code-block:: none
+
+                Epoch 1/5 0.09s Step 25/25: loss: 6.351375, acc: 1.375000, val_loss: 6.236106, val_acc: 5.000000
+                Epoch 1: val_acc improved from -inf to 5.00000, saving file to ./simple_example/checkpoint_epoch_1.ckpt
+                Epoch 2/5 0.10s Step 25/25: loss: 6.054254, acc: 14.000000, val_loss: 5.944495, val_acc: 19.500000
+                Epoch 2: val_acc improved from 5.00000 to 19.50000, saving file to ./simple_example/checkpoint_epoch_2.ckpt
+                Epoch 3/5 0.09s Step 25/25: loss: 5.759377, acc: 22.875000, val_loss: 5.655412, val_acc: 21.000000
+                Epoch 3: val_acc improved from 19.50000 to 21.00000, saving file to ./simple_example/checkpoint_epoch_3.ckpt
+                ...
+
+        Training can now easily be resumed from the best checkpoint::
+
+                exp.train(train_generator, valid_generator, epochs=10)
+
+        .. code-block:: none
+
+                Restoring model from ./simple_example/checkpoint_epoch_3.ckpt
+                Loading weights from ./simple_example/checkpoint.ckpt and starting at epoch 6.
+                Loading optimizer state from ./simple_example/checkpoint.optim and starting at epoch 6.
+                Epoch 6/10 0.16s Step 25/25: loss: 4.897135, acc: 22.875000, val_loss: 4.813141, val_acc: 20.500000
+                Epoch 7/10 0.10s Step 25/25: loss: 4.621514, acc: 22.625000, val_loss: 4.545359, val_acc: 20.500000
+                Epoch 8/10 0.24s Step 25/25: loss: 4.354721, acc: 23.625000, val_loss: 4.287117, val_acc: 20.500000
+                ...
+
+        Testing is also very intuitive::
+
+                exp.test(test_generator)
+
+        .. code-block:: none
+
+                Restoring model from ./simple_example/checkpoint_epoch_9.ckpt
+                Found best checkpoint at epoch: 9
+                lr: 0.01, loss: 4.09892, acc: 23.625, val_loss: 4.04057, val_acc: 21.5
+                On best model: test_loss: 4.06664, test_acc: 17.5
+
+
+        Finally, all the pertinent metrics specified to the ModelBundle at each epoch are stored in a specific logging
+        file, found here at './simple_example/log.tsv'.
+
+        .. code-block:: none
+
+                epoch	time	            lr	    loss	            acc	    val_loss	        val_acc
+                1	    0.0721172170015052	0.01	6.351375141143799	1.375	6.23610631942749	5.0
+                2	    0.0298177790245972	0.01	6.054253826141357	14.000	5.94449516296386	19.5
+                3	    0.0637106419890187	0.01	5.759376544952392	22.875	5.65541223526001	21.0
+                ...
+        """
+        monitoring, monitor_metric, monitor_mode = cls._get_monitoring_config(monitoring, monitor_metric, monitor_mode)
+
+        return ModelBundle(
+            directory,
+            model,
+            logging=logging,
+            monitoring=monitoring,
+            monitor_metric=monitor_metric,
+            monitor_mode=monitor_mode,
+            _is_direct=False,
+        )
+
+    def set_paths(self):
+        self.best_checkpoint_filename = self.get_path(ModelBundle.BEST_CHECKPOINT_FILENAME)
+        self.model_checkpoint_filename = self.get_path(ModelBundle.MODEL_CHECKPOINT_FILENAME)
+        self.optimizer_checkpoint_filename = self.get_path(ModelBundle.OPTIMIZER_CHECKPOINT_FILENAME)
+        self.log_filename = self.get_path(ModelBundle.LOG_FILENAME)
+        self.tensorboard_directory = self.get_path(ModelBundle.TENSORBOARD_DIRECTORY)
+        self.epoch_filename = self.get_path(ModelBundle.EPOCH_FILENAME)
+        self.lr_scheduler_filename = self.get_path(ModelBundle.LR_SCHEDULER_FILENAME)
+        self.plots_directory = self.get_path(ModelBundle.PLOTS_DIRECTORY)
+        self.test_log_filename = self.get_path(ModelBundle.TEST_LOG_FILENAME)
 
     def get_path(self, *paths: str) -> str:
         """
-        Returns the path inside the experiment directory.
+        Returns the path inside the model bundle directory.
         """
         return os.path.join(self.directory, *paths)
 
+    @classmethod
     def _get_loss_function(
-        self, loss_function: Union[Callable, str], network: torch.nn.Module, task: Union[str, None]
+        cls, loss_function: Union[Callable, str], network: torch.nn.Module, task: Union[str, None]
     ) -> Union[Callable, str]:
         if loss_function is None:
             if hasattr(network, 'loss_function'):
                 return network.loss_function
             if task is not None:
                 if task.startswith('classif'):
                     return 'cross_entropy'
                 if task.startswith('reg'):
                     return 'mse'
         return loss_function
 
+    @classmethod
     def _get_batch_metrics(
-        self, batch_metrics: Union[List, None], network: torch.nn.Module, task: Union[str, None]
+        cls, batch_metrics: Union[List, None], network: torch.nn.Module, task: Union[str, None]
     ) -> Union[List, None]:
         if batch_metrics is None or len(batch_metrics) == 0:
             if hasattr(network, 'batch_metrics'):
                 return network.batch_metrics
             if task is not None and task.startswith('classif'):
                 return ['accuracy']
         return batch_metrics
 
-    def _get_epoch_metrics(
-        self, epoch_metrics: Union[List, None], network, task: Union[str, None]
-    ) -> Union[List, None]:
+    @classmethod
+    def _get_epoch_metrics(cls, epoch_metrics: Union[List, None], network, task: Union[str, None]) -> Union[List, None]:
         if epoch_metrics is None or len(epoch_metrics) == 0:
             if hasattr(network, 'epoch_metrics'):
                 return network.epoch_metrics
             if task is not None and task.startswith('classif'):
                 return ['f1']
         return epoch_metrics
 
-    def _set_monitor(
-        self, monitor_metric: Union[str, None], monitor_mode: Union[str, None], task: Union[str, None]
+    @classmethod
+    def _get_monitoring_config(
+        cls,
+        monitoring: bool,
+        monitor_metric: Union[str, None],
+        monitor_mode: Union[str, None],
+        task: Union[str, None] = None,
     ) -> None:
+        if not monitoring:
+            return False, None, None
+
         if monitor_mode is not None and monitor_mode not in ['min', 'max']:
             raise ValueError(f"Invalid mode '{monitor_mode}'")
 
-        self.monitor_metric = 'val_loss'
-        self.monitor_mode = 'min'
-        if monitor_metric is not None:
-            self.monitor_metric = monitor_metric
-            if monitor_mode is not None:
-                self.monitor_mode = monitor_mode
-        elif task is not None and task.startswith('classif'):
-            self.monitor_metric = 'val_acc'
-            self.monitor_mode = 'max'
+        if monitor_metric is None:
+            if task is not None and task.startswith('classif'):
+                monitor_metric = 'val_acc'
+                monitor_mode = 'max'
+            else:
+                monitor_metric = 'val_loss'
+
+        if monitor_mode is None:
+            monitor_mode = 'min'
+
+        return True, monitor_metric, monitor_mode
 
     def get_stats(self):
+        if not os.path.isfile(self.log_filename):
+            raise ValueError("There are no logs available. Did you forget to train with logging enabled?")
+
         return pd.read_csv(self.log_filename, sep='\t')
 
     def get_best_epoch_stats(self) -> Dict:
         """
         Returns all computed statistics corresponding to the best epoch according to the
         ``monitor_metric`` and ``monitor_mode`` attributes.
 
@@ -395,26 +615,26 @@
 
         return initial_epoch
 
     def _init_model_restoring_callbacks(
         self, initial_epoch: int, keep_only_last_best: bool, save_every_epoch: bool
     ) -> List:
         callbacks = []
-        best_checkpoint = ModelCheckpoint(
-            self.best_checkpoint_filename,
-            monitor=self.monitor_metric,
-            mode=self.monitor_mode,
-            keep_only_last_best=keep_only_last_best,
-            save_best_only=not save_every_epoch,
-            restore_best=not save_every_epoch,
-            verbose=not save_every_epoch,
-        )
-        callbacks.append(best_checkpoint)
-
-        if save_every_epoch:
+        if not save_every_epoch:
+            best_checkpoint = ModelCheckpoint(
+                self.best_checkpoint_filename,
+                monitor=self.monitor_metric,
+                mode=self.monitor_mode,
+                keep_only_last_best=keep_only_last_best,
+                save_best_only=True,
+                restore_best=True,
+                verbose=True,
+            )
+            callbacks.append(best_checkpoint)
+        else:
             best_restore = BestModelRestore(monitor=self.monitor_metric, mode=self.monitor_mode, verbose=True)
             callbacks.append(best_restore)
 
         if initial_epoch > 1:
             # We set the current best metric score in the ModelCheckpoint so that
             # it does not save checkpoint it would not have saved if the
             # optimization was not stopped.
@@ -470,44 +690,38 @@
 
     def train(self, train_generator, valid_generator=None, **kwargs) -> List[Dict]:
         """
         Trains or finetunes the model on a dataset using a generator. If a previous training already occurred
         and lasted a total of `n_previous` epochs, then the model's weights will be set to the last checkpoint and the
         training will be resumed for epochs range (`n_previous`, `epochs`].
 
-        If the Experiment has logging enabled (i.e. self.logging is True), numerous callbacks will be automatically
+        If the ModelBundle has logging enabled (i.e. self.logging is True), numerous callbacks will be automatically
         included. Notably, two :class:`~poutyne.ModelCheckpoint` objects will take care of saving the last and every
         new best (according to monitor mode) model weights in appropriate checkpoint files.
         :class:`~poutyne.OptimizerCheckpoint` and :class:`~poutyne.LRSchedulerCheckpoint` will also respectively
         handle the saving of the optimizer and LR scheduler's respective states for future retrieval. Moreover, a
         :class:`~poutyne.AtomicCSVLogger` will save all available epoch statistics in an output .tsv file. Lastly, a
         :class:`~poutyne.TensorBoardLogger` handles automatic TensorBoard logging of various neural network
         statistics.
 
-        .. warning:: With **Jupyter Notebooks in Firefox**, if ``colorama`` is installed and colors are enabled (as it
-            is by default), a great number of epochs and steps per epoch can cause a spike in memory usage in Firefox.
-            The problem does not occur in Google Chrome/Chromium. To avoid this problem, you can disable the colors by
-            passing ``progress_options={'coloring': False}``. See
-            `this Github issue for details <https://github.com/jupyter/notebook/issues/5897>`__.
-
         Args:
             train_generator: Generator-like object for the training set. See :func:`~Model.fit_generator()`
                 for details on the types of generators supported.
             valid_generator (optional): Generator-like object for the validation set. See
                 :func:`~Model.fit_generator()` for details on the types of generators supported.
                 (Default value = None)
             callbacks (List[~poutyne.Callback]): List of callbacks that will be called during
                 training. These callbacks are added after those used in this method (see above). This allows to assume
                 that they are called after those.
                 (Default value = None)
             lr_schedulers: List of learning rate schedulers. (Default value = None)
             keep_only_last_best (bool): Whether only the last saved best checkpoint is kept. Applies only when
                  `save_every_epoch` is false.
                  (Default value = False)
-            save_every_epoch (bool, optional): Whether or not to save the experiment model's weights after
+            save_every_epoch (bool, optional): Whether or not to save the model bundle's model's weights after
                 every epoch.
                 (Default value = False)
             disable_tensorboard (bool, optional): Whether or not to disable the automatic tensorboard logging
                 callbacks.
                 (Default value = False)
             seed (int, optional): Seed used to make the sampling deterministic.
                 (Default value = 42)
@@ -520,15 +734,15 @@
 
     def train_dataset(self, train_dataset, valid_dataset=None, **kwargs) -> List[Dict]:
         """
         Trains or finetunes the model on a dataset. If a previous training already occurred
         and lasted a total of `n_previous` epochs, then the model's weights will be set to the last checkpoint and the
         training will be resumed for epochs range (`n_previous`, `epochs`].
 
-        If the Experiment has logging enabled (i.e. self.logging is True), numerous callbacks will be automatically
+        If the ModelBundle has logging enabled (i.e. self.logging is True), numerous callbacks will be automatically
         included. Notably, two :class:`~poutyne.ModelCheckpoint` objects will take care of saving the last and every
         new best (according to monitor mode) model weights in appropriate checkpoint files.
         :class:`~poutyne.OptimizerCheckpoint` and :class:`~poutyne.LRSchedulerCheckpoint` will also respectively
         handle the saving of the optimizer and LR scheduler's respective states for future retrieval. Moreover, a
         :class:`~poutyne.AtomicCSVLogger` will save all available epoch statistics in an output .tsv file. Lastly, a
         :class:`~poutyne.TensorBoardLogger` handles automatic TensorBoard logging of various neural network
         statistics.
@@ -540,15 +754,15 @@
                 training. These callbacks are added after those used in this method (see above). This allows to assume
                 that they are called after those.
                 (Default value = None)
             lr_schedulers: List of learning rate schedulers. (Default value = None)
             keep_only_last_best (bool): Whether only the last saved best checkpoint is kept. Applies only when
                  `save_every_epoch` is false.
                  (Default value = False)
-            save_every_epoch (bool, optional): Whether or not to save the experiment model's weights after
+            save_every_epoch (bool, optional): Whether or not to save the model bundle's model's weights after
                 every epoch.
                 (Default value = False)
             disable_tensorboard (bool, optional): Whether or not to disable the automatic tensorboard logging
                 callbacks.
                 (Default value = False)
             seed (int, optional): Seed used to make the sampling deterministic.
                 (Default value = 42)
@@ -561,15 +775,15 @@
 
     def train_data(self, x, y, validation_data=None, **kwargs) -> List[Dict]:
         """
         Trains or finetunes the model on data under the form of NumPy arrays or torch tensors. If a previous
         training already occurred and lasted a total of `n_previous` epochs, then the model's weights will be set to the
         last checkpoint and the training will be resumed for epochs range (`n_previous`, `epochs`].
 
-        If the Experiment has logging enabled (i.e. self.logging is True), numerous callbacks will be automatically
+        If the ModelBundle has logging enabled (i.e. self.logging is True), numerous callbacks will be automatically
         included. Notably, two :class:`~poutyne.ModelCheckpoint` objects will take care of saving the last and every
         new best (according to monitor mode) model weights in appropriate checkpoint files.
         :class:`~poutyne.OptimizerCheckpoint` and :class:`~poutyne.LRSchedulerCheckpoint` will also respectively
         handle the saving of the optimizer and LR scheduler's respective states for future retrieval. Moreover, a
         :class:`~poutyne.AtomicCSVLogger` will save all available epoch statistics in an output .tsv file. Lastly, a
         :class:`~poutyne.TensorBoardLogger` handles automatic TensorBoard logging of various neural network
         statistics.
@@ -590,15 +804,15 @@
                 training. These callbacks are added after those used in this method (see above). This allows to assume
                 that they are called after those.
                 (Default value = None)
             lr_schedulers: List of learning rate schedulers. (Default value = None)
             keep_only_last_best (bool): Whether only the last saved best checkpoint is kept. Applies only when
                  `save_every_epoch` is false.
                  (Default value = False)
-            save_every_epoch (bool, optional): Whether or not to save the experiment model's weights after
+            save_every_epoch (bool, optional): Whether or not to save the model bundle's model's weights after
                 every epoch.
                 (Default value = False)
             disable_tensorboard (bool, optional): Whether or not to disable the automatic tensorboard logging
                 callbacks.
                 (Default value = False)
             seed (int, optional): Seed used to make the sampling deterministic.
                 (Default value = 42)
@@ -638,14 +852,25 @@
 
             expt_callbacks += [AtomicCSVLogger(self.log_filename, separator='\t', append=initial_epoch != 1)]
 
             if self.monitoring:
                 expt_callbacks += self._init_model_restoring_callbacks(
                     initial_epoch, keep_only_last_best, save_every_epoch
                 )
+
+            if save_every_epoch:
+                expt_callbacks += [
+                    ModelCheckpoint(
+                        self.best_checkpoint_filename,
+                        save_best_only=False,
+                        restore_best=False,
+                        verbose=False,
+                    )
+                ]
+
             expt_callbacks += [ModelCheckpoint(self.model_checkpoint_filename, verbose=False)]
             expt_callbacks += [OptimizerCheckpoint(self.optimizer_checkpoint_filename, verbose=False)]
 
             # We save the last epoch number after the end of the epoch so that the
             # _load_epoch_state() knows which epoch to restart the optimization.
             expt_callbacks += [
                 PeriodicSaveLambda(lambda fd, epoch, logs: print(epoch, file=fd), self.epoch_filename, open_mode='w')
@@ -749,17 +974,14 @@
         ckpt_filename = self.best_checkpoint_filename.format(epoch=best_epoch)
 
         if verbose:
             print(f"Found best checkpoint at epoch: {best_epoch}")
             self._print_epoch_stats(best_epoch_stats)
             print(f"Loading checkpoint {ckpt_filename}")
 
-        if not os.path.isfile(ckpt_filename):
-            raise ValueError(f"No checkpoint found for epoch {best_epoch}")
-
         return best_epoch_stats, self.model.load_weights(ckpt_filename, strict=strict)
 
     def _load_last_checkpoint(self, *, verbose: bool = False, strict: bool = True) -> None:
         history = self.get_stats()
         epoch_stats = history.iloc[-1:]
 
         if verbose:
@@ -775,15 +997,15 @@
         return self.model.load_weights(path, strict=strict)
 
     def test(self, test_generator, **kwargs):
         """
         Computes and returns the loss and the metrics of the model on a given test examples
         generator.
 
-        If the Experiment has logging enabled (i.e. self.logging is True), a checkpoint (the best one by default)
+        If the ModelBundle has logging enabled (i.e. self.logging is True), a checkpoint (the best one by default)
         is loaded and test and validation statistics are saved in a specific test output .tsv file. Otherwise, the
         current weights of the network is used for testing and statistics are only shown in the standard output.
 
         Args:
             test_generator: Generator-like object for the test set. See :func:`~Model.fit_generator()` for
                 details on the types of generators supported.
             checkpoint (Union[str, int]): Which model checkpoint weights to load for the test evaluation.
@@ -796,28 +1018,28 @@
 
                 This argument has no effect when logging is disabled. (Default value = 'best')
             seed (int, optional): Seed used to make the sampling deterministic.
                 (Default value = 42)
             name (str): Prefix of the test log file. (Default value = 'test')
             kwargs: Any keyword arguments to pass to :func:`~Model.evaluate_generator()`.
 
-        If the Experiment has logging enabled (i.e. self.logging is True), one callback will be automatically
+        If the ModelBundle has logging enabled (i.e. self.logging is True), one callback will be automatically
         included to save the test metrics. Moreover, a :class:`~poutyne.AtomicCSVLogger` will save the test
         metrics in an output .tsv file.
 
         Returns:
             dict sorting of all the test metrics values by their names.
         """
         return self._test(self.model.evaluate_generator, test_generator, **kwargs)
 
     def test_dataset(self, test_dataset, **kwargs) -> Dict:
         """
         Computes and returns the loss and the metrics of the model on a given test dataset.
 
-        If the Experiment has logging enabled (i.e. self.logging is True), a checkpoint (the best one by default)
+        If the ModelBundle has logging enabled (i.e. self.logging is True), a checkpoint (the best one by default)
         is loaded and test and validation statistics are saved in a specific test output .tsv file. Otherwise, the
         current weights of the network is used for testing and statistics are only shown in the standard output.
 
         Args:
             test_dataset (~torch.utils.data.Dataset): Test dataset.
             checkpoint (Union[str, int]): Which model checkpoint weights to load for the test evaluation.
 
@@ -829,28 +1051,28 @@
 
                 This argument has no effect when logging is disabled. (Default value = 'best')
             seed (int, optional): Seed used to make the sampling deterministic.
                 (Default value = 42)
             name (str): Prefix of the test log file. (Default value = 'test')
             kwargs: Any keyword arguments to pass to :func:`~Model.evaluate_dataset()`.
 
-        If the Experiment has logging enabled (i.e. self.logging is True), one callback will be automatically
+        If the ModelBundle has logging enabled (i.e. self.logging is True), one callback will be automatically
         included to save the test metrics. Moreover, a :class:`~poutyne.AtomicCSVLogger` will save the test
         metrics in an output .tsv file.
 
         Returns:
             dict sorting of all the test metrics values by their names.
         """
         return self._test(self.model.evaluate_dataset, test_dataset, **kwargs)
 
     def test_data(self, x, y, **kwargs) -> Dict:
         """
         Computes and returns the loss and the metrics of the model on a given test dataset.
 
-        If the Experiment has logging enabled (i.e. self.logging is True), a checkpoint (the best one by default)
+        If the ModelBundle has logging enabled (i.e. self.logging is True), a checkpoint (the best one by default)
         is loaded and test and validation statistics are saved in a specific test output .tsv file. Otherwise, the
         current weights of the network is used for testing and statistics are only shown in the standard output.
 
         Args:
             x (Union[~torch.Tensor, ~numpy.ndarray] or Union[tuple, list] of Union[~torch.Tensor, ~numpy.ndarray]):
                 Input to the model. Union[Tensor, ndarray] if the model has a single input.
                 Union[tuple, list] of Union[Tensor, ndarray] if the model has multiple inputs.
@@ -867,15 +1089,15 @@
                   ``torch.save(a_pytorch_network.state_dict(), "./a_path.p")``).
 
                 This argument has no effect when logging is disabled. (Default value = 'best')
             seed (int, optional): Seed used to make the sampling deterministic.
                 (Default value = 42)
             name (str): Prefix of the test log file. (Default value = 'test')
             kwargs: Any keyword arguments to pass to :func:`~Model.evaluate()`.
-        If the Experiment has logging enabled (i.e. self.logging is True), one callback will be automatically
+        If the ModelBundle has logging enabled (i.e. self.logging is True), one callback will be automatically
         included to save the test metrics. Moreover, a :class:`~poutyne.AtomicCSVLogger` will save the test
         metrics in an output .tsv file.
 
         Returns:
             dict sorting of all the test metrics values by their names.
         """
         return self._test(self.model.evaluate, x, y, **kwargs)
@@ -990,54 +1212,54 @@
 
         Returns:
             Return the predictions in the format outputted by the model.
         """
         return self._predict(self.model.predict, x, **kwargs)
 
     def _predict(
-        self, evaluate_func: Callable, *args, verbose=True, checkpoint: Union[str, int] = 'best', **kwargs
+        self, predict_func: Callable, *args, verbose=True, checkpoint: Union[str, int] = 'best', **kwargs
     ) -> Any:
         if self.logging:
             if not self.monitoring and checkpoint == 'best':
                 checkpoint = 'last'
             self.load_checkpoint(checkpoint, verbose=verbose)
 
-        ret = evaluate_func(*args, verbose=verbose, **kwargs)
+        ret = predict_func(*args, verbose=verbose, **kwargs)
         return ret
 
-    def is_better_than(self, another_experiment) -> bool:
+    def is_better_than(self, another_model_bundle) -> bool:
         """
-        Compare the results of the Experiment with another experiment. To compare, both Experiments need to be
+        Compare the results of the ModelBundle with another model bundle. To compare, both ModelBundles need to be
         logged, monitor the same metric and the same monitor mode ("min" or "max").
 
         Args:
-            another_experiment (~poutyne. Experiment): Another Poutyne experiment to compare results with.
+            another_model_bundle (~poutyne.ModelBundle): Another Poutyne model bundle to compare results with.
 
         Return:
-            Whether the Experiment is better than the Experiment to compare with.
+            Whether the ModelBundle is better than the ModelBundle to compare with.
         """
         if not self.logging:
-            raise ValueError("The experiment is not logged.")
-        if not another_experiment.logging:
-            raise ValueError("The experiment to compare to is not logged.")
+            raise ValueError("The model bundle is not logged.")
+        if not another_model_bundle.logging:
+            raise ValueError("The model bundle to compare to is not logged.")
 
-        if self.monitor_metric != another_experiment.monitor_metric:
-            raise ValueError("The monitored metric is not the same between the two experiment.")
+        if self.monitor_metric != another_model_bundle.monitor_metric:
+            raise ValueError("The monitored metric is not the same between the two model bundles.")
         monitored_metric = self.monitor_metric
 
-        if self.monitor_mode != another_experiment.monitor_mode:
-            raise ValueError("The monitored mode is not the same between the two experiment.")
+        if self.monitor_mode != another_model_bundle.monitor_mode:
+            raise ValueError("The monitored mode is not the same between the two model bundles.")
         monitor_mode = self.monitor_mode
 
         checkpoint = 'best' if self.monitoring else 'last'
         self_stats = self.load_checkpoint(checkpoint, verbose=False)
         self_monitored_metric = self_stats[monitored_metric]
         self_monitored_metric_value = self_monitored_metric.item()
 
-        other_checkpoint = 'best' if another_experiment.monitoring else 'last'
+        other_checkpoint = 'best' if another_model_bundle.monitoring else 'last'
         other_stats = self.load_checkpoint(other_checkpoint, verbose=False)
         other_monitored_metric = other_stats[monitored_metric]
         other_monitored_metric_value = other_monitored_metric.item()
 
         if monitor_mode == 'min':
             is_better_than = self_monitored_metric_value < other_monitored_metric_value
         else:
```

### Comparing `Poutyne-1.8/poutyne/framework/metrics/batch_metrics.py` & `Poutyne-1.9/poutyne/framework/metrics/batch_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 # Because nn.Module has the abstract method _forward_unimplemented
 # pylint: disable=abstract-method
 import torch.nn as nn
 
 from .metrics_registering import register_batch_metric, register_batch_metric_function
```

### Comparing `Poutyne-1.8/poutyne/framework/metrics/epoch_metrics/fscores.py` & `Poutyne-1.9/poutyne/framework/metrics/epoch_metrics/fscores.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,29 @@
 """
-The source code of this file was copied from the AllenNLP project, and has been modified.
+The source code of this file was copied from the AllenNLP project, and has been modified. All modifications
+made from the original source code are under the LGPLv3 license.
+
+
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information on the Poutyne and AllenNLP repository.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+
 
 Copyright 2019 AllenNLP
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
@@ -11,14 +31,15 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
+
 from typing import Optional, Union, List, Tuple
 import torch
 from .base import EpochMetric
 from ..metrics_registering import register_epoch_metric
 
 
 class FBeta(EpochMetric):
@@ -72,35 +93,40 @@
             ``'micro'``:
                 Calculate metrics globally by counting the total true positives,
                 false negatives and false positives.
             ``'macro'``:
                 Calculate metrics for each label, and find their unweighted mean.
                 This does not take label imbalance into account.
 
-            (Default value = 'micro')
+            (Default value = 'macro')
         beta (float):
             The strength of recall versus precision in the F-score. (Default value = 1.0)
         pos_label (int):
-            The class with respect to which the metric is computed when `average == 'binary'`. Otherwise, this
+            The class with respect to which the metric is computed when ``average == 'binary'``. Otherwise, this
             argument has no effect. (Default value = 1)
         ignore_index (int): Specifies a target value that is ignored. This also works in combination with
             a mask if provided. (Default value = -100)
+        threshold (float): Threshold for when there is a single score for each prediction. If a sigmoid output is used,
+            this should be between 0 and 1. A suggested value would be 0.5. If a logits output is used, the threshold
+            would be between -inf and inf. The suggested default value is 0 as to give a probability of 0.5 if a sigmoid
+            output were used. (Default = 0)
         names (Optional[Union[str, List[str]]]): The names associated to the metrics. It is a string when
             a single metric is requested. It is a list of 3 strings if all metrics are requested.
             (Default value = None)
     """
 
     def __init__(
         self,
         *,
         metric: Optional[str] = None,
         average: Union[str, int] = 'macro',
         beta: float = 1.0,
         pos_label: int = 1,
         ignore_index: int = -100,
+        threshold: float = 0.0,
         names: Optional[Union[str, List[str]]] = None,
     ) -> None:
         super().__init__()
         self.metric_options = ('fscore', 'precision', 'recall')
         if metric is not None and metric not in self.metric_options:
             raise ValueError(f"`metric` has to be one of {self.metric_options}.")
 
@@ -116,14 +142,15 @@
         self._label = None
         if isinstance(average, int):
             self._label = average
         elif average == 'binary':
             self._label = pos_label
         self._beta = beta
         self.ignore_index = ignore_index
+        self.threshold = threshold
         self.__name__ = self._get_names(names)
 
         # statistics
         # the total number of true positive instances under each class
         # Shape: (num_classes, )
         self.register_buffer('_true_positive_sum', None)
         # the total number of instances
@@ -174,29 +201,36 @@
             y_true (Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]):
                 Ground truths. A tensor of the integer class label of shape (batch_size, ...). It must
                 be the same shape as the ``y_pred`` tensor without the ``num_classes`` dimension.
                 It can also be a tuple with two tensors of the same shape, the first being the
                 ground truths and the second being a mask.
         """
 
-        mask = 1
         if isinstance(y_true, tuple):
             y_true, mask = y_true
-            mask = mask.byte()
+            mask = mask.bool()
+        else:
+            mask = torch.ones_like(y_true).bool()
 
         if self.ignore_index is not None:
-            mask *= (y_true != self.ignore_index).byte()
+            mask *= y_true != self.ignore_index
 
-        if not torch.is_tensor(mask):
-            mask = torch.ones_like(y_true, dtype=torch.bool)
+        if y_pred.shape[0] == 1:
+            y_pred, y_true, mask = (
+                y_pred.squeeze().unsqueeze(0),
+                y_true.squeeze().unsqueeze(0),
+                mask.squeeze().unsqueeze(0),
+            )
         else:
-            mask = mask.bool()
+            y_pred, y_true, mask = y_pred.squeeze(), y_true.squeeze(), mask.squeeze()
+
+        num_classes = 2
+        if y_pred.shape != y_true.shape:
+            num_classes = y_pred.size(1)
 
-        # Calculate true_positive_sum, true_negative_sum, pred_sum, true_sum
-        num_classes = y_pred.size(1)
         if (y_true >= num_classes).any():
             raise ValueError(
                 f"A gold label passed to FBetaMeasure contains an id >= {num_classes}, the number of classes."
             )
 
         if self._average == 'binary' and num_classes > 2:
             raise ValueError("When `average` is binary, the number of prediction scores must be 2.")
@@ -207,15 +241,18 @@
             self._true_positive_sum = torch.zeros(num_classes, device=y_pred.device)
             self._true_sum = torch.zeros(num_classes, device=y_pred.device)
             self._pred_sum = torch.zeros(num_classes, device=y_pred.device)
             self._total_sum = torch.zeros(num_classes, device=y_pred.device)
 
         y_true = y_true.float()
 
-        argmax_y_pred = y_pred.argmax(1).float()
+        if y_pred.shape != y_true.shape:
+            argmax_y_pred = y_pred.argmax(1).float()
+        else:
+            argmax_y_pred = (y_pred > self.threshold).float()
         true_positives = (y_true == argmax_y_pred) * mask
         true_positives_bins = y_true[true_positives]
 
         # Watch it:
         # The total numbers of true positives under all _predicted_ classes are zeros.
         if true_positives_bins.shape[0] == 0:
             true_positive_sum = torch.zeros(num_classes, device=y_pred.device)
@@ -254,15 +291,15 @@
         true_sum = self._true_sum
 
         if self._average == 'micro':
             tp_sum = tp_sum.sum()
             pred_sum = pred_sum.sum()
             true_sum = true_sum.sum()
 
-        beta2 = self._beta ** 2
+        beta2 = self._beta**2
         # Finally, we have all our sufficient statistics.
         precision = _prf_divide(tp_sum, pred_sum)
         recall = _prf_divide(tp_sum, true_sum)
         fscore = (1 + beta2) * precision * recall / (beta2 * precision + recall)
         fscore[tp_sum == 0] = 0.0
 
         if self._average == 'macro':
@@ -294,15 +331,15 @@
 
 
 @register_epoch_metric
 class F1(FBeta):
     """
     Alias class for :class:`~poutyne.FBeta` where ``metric == 'fscore'`` and ``beta == 1``.
 
-    Possible string name in :class:`batch_metrics argument <poutyne.Model>`:
+    Possible string name in :class:`epoch_metrics argument <poutyne.Model>`:
         - ``'f1'``
 
     Keys in :class:`logs<poutyne.Callback>` dictionary of callbacks:
         - Train: ``'fscore_{average}'``
         - Validation: ``'val_fscore_{average}'``
 
         where ``{average}`` is replaced by the value of the respective parameter.
@@ -311,47 +348,101 @@
     def __init__(self, average='macro'):
         super().__init__(metric='fscore', average=average, beta=1)
 
 
 @register_epoch_metric
 class Precision(FBeta):
     """
-    Alias class for :class:`~poutyne.FBeta` where ``metric == 'precision'`` and ``beta == 1``.
+    Alias class for :class:`~poutyne.FBeta` where ``metric == 'precision'``.
 
-    Possible string name in :class:`batch_metrics argument <poutyne.Model>`:
+    Possible string name in :class:`epoch_metrics argument <poutyne.Model>`:
         - ``'precision'``
 
     Keys in :class:`logs<poutyne.Callback>` dictionary of callbacks:
         - Train: ``'precision_{average}'``
         - Validation: ``'val_precision_{average}'``
 
         where ``{average}`` is replaced by the value of the respective parameter.
     """
 
     def __init__(self, average='macro'):
-        super().__init__(metric='precision', average=average, beta=1)
+        super().__init__(metric='precision', average=average)
 
 
 @register_epoch_metric
 class Recall(FBeta):
     """
-    Alias class for :class:`~poutyne.FBeta` where ``metric == 'recall'`` and ``beta == 1``.
+    Alias class for :class:`~poutyne.FBeta` where ``metric == 'recall'``.
 
-    Possible string name in :class:`batch_metrics argument <poutyne.Model>`:
+    Possible string name in :class:`epoch_metrics argument <poutyne.Model>`:
         - ``'recall'``
 
     Keys in :class:`logs<poutyne.Callback>` dictionary of callbacks:
         - Train: ``'recall_{average}'``
         - Validation: ``'val_recall_{average}'``
 
         where ``{average}`` is replaced by the value of the respective parameter.
     """
 
     def __init__(self, average='macro'):
-        super().__init__(metric='recall', average=average, beta=1)
+        super().__init__(metric='recall', average=average)
+
+
+@register_epoch_metric('binaryf1', 'binf1')
+class BinaryF1(FBeta):
+    """
+    Alias class for :class:`~poutyne.FBeta` where ``metric == 'fscore'``, ``average='binary'`` and ``beta == 1``.
+
+    Possible string name in :class:`epoch_metrics argument <poutyne.Model>`:
+        - ``'binary_f1'``
+        - ``'bin_f1'``
+
+    Keys in :class:`logs<poutyne.Callback>` dictionary of callbacks:
+        - Train: ``'bin_fscore'``
+        - Validation: ``'val_bin_fscore'``
+    """
+
+    def __init__(self, threshold=0.0):
+        super().__init__(metric='fscore', average='binary', beta=1, threshold=threshold, names='bin_fscore')
+
+
+@register_epoch_metric('binaryprecision', 'binprecision')
+class BinaryPrecision(FBeta):
+    """
+    Alias class for :class:`~poutyne.FBeta` where ``metric == 'precision'`` and ``average='binary'``.
+
+    Possible string name in :class:`epoch_metrics argument <poutyne.Model>`:
+        - ``'binary_precision'``
+        - ``'bin_precision'``
+
+    Keys in :class:`logs<poutyne.Callback>` dictionary of callbacks:
+        - Train: ``'bin_precision'``
+        - Validation: ``'val_bin_precision'``
+    """
+
+    def __init__(self, threshold=0.0):
+        super().__init__(metric='precision', average='binary', threshold=threshold, names='bin_precision')
+
+
+@register_epoch_metric('binaryrecall', 'binrecall')
+class BinaryRecall(FBeta):
+    """
+    Alias class for :class:`~poutyne.FBeta` where ``metric == 'recall'`` and ``average='binary'``.
+
+    Possible string name in :class:`epoch_metrics argument <poutyne.Model>`:
+        - ``'binary_recall'``
+        - ``'bin_recall'``
+
+    Keys in :class:`logs<poutyne.Callback>` dictionary of callbacks:
+        - Train: ``'bin_recall'``
+        - Validation: ``'val_bin_recall'``
+    """
+
+    def __init__(self, threshold=0.0):
+        super().__init__(metric='recall', average='binary', threshold=threshold, names='bin_recall')
 
 
 def _prf_divide(numerator, denominator):
     """Performs division and handles divide-by-zero.
 
     On zero-division, sets the corresponding result elements to zero.
     """
```

### Comparing `Poutyne-1.8/poutyne/framework/metrics/epoch_metrics/sklearn_metrics.py` & `Poutyne-1.9/poutyne/framework/metrics/epoch_metrics/sklearn_metrics.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 from typing import Optional, Union, List, Callable, Dict, Tuple
 import numpy as np
 import torch
 from .base import EpochMetric
 
 
 class SKLearnMetrics(EpochMetric):
@@ -79,15 +98,14 @@
             y_true, sample_weight = y_true
             self.sample_weight_list.append(sample_weight.cpu().numpy())
         self.y_true_list.append(y_true.cpu().numpy())
 
     def get_metric(self) -> Dict:
         """
         Returns the metrics as a dictionary with the names as keys.
-        Note: This will reset the epoch metric value.
         """
         sample_weight = None
         if len(self.sample_weight_list) != 0:
             sample_weight = np.concatenate(self.sample_weight_list)
         y_pred = np.concatenate(self.y_pred_list)
         y_true = np.concatenate(self.y_true_list)
```

### Comparing `Poutyne-1.8/poutyne/framework/model.py` & `Poutyne-1.9/poutyne/framework/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,39 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 # pylint: disable=too-many-lines,too-many-public-methods
 import contextlib
 import numbers
 import timeit
 import warnings
 from collections import defaultdict
 from typing import Iterable, Mapping, List, Union, Any, Tuple
 
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.optim as optim
+from torch.nn.utils.rnn import PackedSequence
 from torch.utils.data import DataLoader
 
 from poutyne import torch_to_numpy, numpy_to_torch, torch_to
 from .callbacks import CallbackList, ProgressionCallback, Callback
 from .iterators import EpochIterator, _get_step_iterator, StepIterator
 from .metrics import get_epoch_metric
 from .metrics import get_loss_or_metric, get_callables_and_names, rename_doubles, flatten_metric_names
@@ -43,16 +63,28 @@
         batch_metrics (list): List of functions with the same signature as the loss function. Each metric
             can be any PyTorch loss function. It can also be a string with the same name as a PyTorch
             loss function (either the functional or object name). Furthermore, see :ref:`batch metrics`
             for supplementary available batch metrics. 'accuracy' (or just 'acc') is an often used metric.
             Each metric function is called on each batch of the optimization and on the validation batches
             at the end of the epoch.
             (Default value = None)
-        epoch_metrics (list): List of functions with the same signature as :class:`~poutyne.EpochMetric`.
-            See :ref:`epoch metrics` for available epoch metrics. (Default value = None)
+        epoch_metrics (list): List of objects with the same signature as either :class:`~poutyne.EpochMetric` or
+            :class:`torchmetrics.Metric <torchmetrics.Metric>`.
+            See :ref:`epoch metrics` and the
+            `TorchMetrics documentation <https://torchmetrics.readthedocs.io/en/latest/references/modules.html>`__ for
+            available epoch metrics.
+            (Default value = None)
+        torch_metrics (list): List of `TorchMetrics <https://torchmetrics.readthedocs.io/>`__  objects.
+            List of objects with the same signature as :class:`torchmetrics.Metric <torchmetrics.Metric>`.
+            See `TorchMetrics documentation <https://torchmetrics.readthedocs.io/en/latest/references/modules.html>`__
+            for available torch metrics. (Default value = None)
+
+            .. warning:: When using this argument, the torch metrics are computed at each batch. This
+                can significantly slow down the compuations depending on the metrics used. In such case, we advise to
+                use them as epoch metrics instead.
         device (Union[torch.torch.device, List[torch.torch.device]]): The device to which the network is
             sent or the list of device to which the network is sent. See :func:`~Model.to()` for details.
 
     Note:
         The name of each batch and epoch metric can be change by passing a tuple ``(name, metric)`` instead
         of simply the metric function or object, where ``name`` is the alternative name of the metric.
         Batch and epoch metrics can return multiple metrics (e.g. an epoch metric could return an F1-score
@@ -137,30 +169,44 @@
             Epoch 1/5 0.05s Step 25/25: loss: 6.752676, acc: 0.000000, val_loss: 6.575071, val_acc: 0.000000
             Epoch 2/5 0.03s Step 25/25: loss: 6.454859, acc: 0.125000, val_loss: 6.279577, val_acc: 0.000000
             Epoch 3/5 0.03s Step 25/25: loss: 6.158523, acc: 2.125000, val_loss: 5.985811, val_acc: 9.500000
             ...
 
     """
 
-    def __init__(self, network, optimizer, loss_function, *, batch_metrics=None, epoch_metrics=None, device=None):
+    def __init__(
+        self,
+        network,
+        optimizer,
+        loss_function,
+        *,
+        batch_metrics=None,
+        epoch_metrics=None,
+        torch_metrics=None,
+        device=None,
+    ):
         if not isinstance(network, nn.Module):
             raise ValueError(f"network should be of type derived from nn.Module, received {type(network)}.")
 
         if optimizer is not None and not isinstance(optimizer, (optim.Optimizer, str, dict)):
             raise ValueError(f"optimizer should be of type derived from optim.Optimizer, received {type(optimizer)}.")
 
         batch_metrics = [] if batch_metrics is None else batch_metrics
         epoch_metrics = [] if epoch_metrics is None else epoch_metrics
+        torch_metrics = [] if torch_metrics is None else torch_metrics
 
         self.network = network
         self.optimizer = get_optimizer(optimizer, self.network)
+
         self.loss_function = get_loss_or_metric(loss_function)
+        if isinstance(self.loss_function, tuple):
+            self.loss_function = self.loss_function[1]
 
         self._check_network_optimizer_parameters_match()
-        self._set_metrics_attributes(batch_metrics, epoch_metrics)
+        self._set_metrics_attributes(batch_metrics, epoch_metrics, torch_metrics)
 
         self.device = None
         self.other_device = None
 
         if device is not None:
             self.to(device)
 
@@ -172,30 +218,40 @@
                     if param not in param_set:
                         raise ValueError(
                             "All parameters in the optimizer should be part of the network. "
                             "This is so to insure that weights checkpointing and the likes "
                             "actually consider all parameters."
                         )
 
-    def _set_metrics_attributes(self, batch_metrics, epoch_metrics):
+    def _set_metrics_attributes(self, batch_metrics, epoch_metrics, torch_metrics):
         batch_metrics = list(map(get_loss_or_metric, batch_metrics))
         self.batch_metrics, batch_metrics_names = get_callables_and_names(batch_metrics)
 
         epoch_metrics = list(map(get_epoch_metric, epoch_metrics))
         self.epoch_metrics, epoch_metrics_names = get_callables_and_names(epoch_metrics)
 
-        self.original_batch_metrics_names, self.original_epoch_metrics_names = batch_metrics_names, epoch_metrics_names
-        batch_metrics_names, epoch_metrics_names = rename_doubles(batch_metrics_names, epoch_metrics_names)
+        self.torch_metrics, torch_metrics_names = get_callables_and_names(torch_metrics)
+
+        self.original_batch_metrics_names, self.original_epoch_metrics_names, self.original_torch_metrics_names = (
+            batch_metrics_names,
+            epoch_metrics_names,
+            torch_metrics_names,
+        )
+        batch_metrics_names, epoch_metrics_names, torch_metrics_names = rename_doubles(
+            batch_metrics_names, epoch_metrics_names, torch_metrics_names
+        )
 
         self.unflatten_batch_metrics_names = batch_metrics_names
         self.unflatten_epoch_metrics_names = epoch_metrics_names
+        self.unflatten_torch_metrics_names = torch_metrics_names
 
         self.batch_metrics_names = flatten_metric_names(batch_metrics_names)
         self.epoch_metrics_names = flatten_metric_names(epoch_metrics_names)
-        self.metrics_names = self.batch_metrics_names + self.epoch_metrics_names
+        self.torch_metrics_names = flatten_metric_names(torch_metrics_names)
+        self.metrics_names = self.batch_metrics_names + self.epoch_metrics_names + self.torch_metrics_names
 
     @contextlib.contextmanager
     def _set_training_mode(self, training):
         old_training = self.network.training
         self.network.train(training)
         with torch.set_grad_enabled(training):
             yield
@@ -530,14 +586,15 @@
             epochs=epochs,
             steps_per_epoch=steps_per_epoch,
             validation_steps=validation_steps,
             initial_epoch=initial_epoch,
             callback=callback_list,
             batch_metrics_names=self.batch_metrics_names,
             epoch_metrics_names=self.epoch_metrics_names,
+            torch_metrics_names=self.torch_metrics_names,
         )
 
         if batches_per_step > 1:
             self._fit_generator_n_batches_per_step(epoch_iterator, callback_list, batches_per_step)
         else:
             self._fit_generator_one_batch_per_step(epoch_iterator, callback_list)
 
@@ -549,103 +606,116 @@
 
             with self._set_training_mode(True):
                 for step, (x, y) in train_step_iterator:
                     step.size = self.get_batch_size(x, y)
 
                     examples_in_step += step.size
 
-                    step.loss, step.metrics, did_backprop, _ = self._fit_batch_n_batches_per_step(
+                    (
+                        step.loss,
+                        step.batch_metrics,
+                        step.torch_metrics,
+                        did_backprop,
+                        _,
+                    ) = self._fit_batch_n_batches_per_step(
                         x, y, batches_per_step, examples_in_step, callback=callback_list, step=step
                     )
 
                     if did_backprop:
                         examples_in_step = 0
 
             if not did_backprop:
                 # Did not step after last batch
                 self._adjust_step_size(examples_in_step)
                 self.optimizer.step()
 
             train_step_iterator.epoch_metrics = self._get_epoch_metrics()
+            train_step_iterator.torch_metrics = self._get_torch_metrics()
 
-            if valid_step_iterator is not None:
-                valid_begin_time = timeit.default_timer()
-
-                callback_list.on_valid_begin({})
-                self._validate(valid_step_iterator)
-
-                valid_step_iterator.epoch_metrics = self._get_epoch_metrics()
-                valid_total_time = timeit.default_timer() - valid_begin_time
-
-                valid_metrics_log = {'time': valid_total_time}
-                valid_metrics_log.update(valid_step_iterator.metrics_logs)
-
-                callback_list.on_valid_end(valid_metrics_log)
+            self._run_validation(valid_step_iterator, callback_list)
 
     def _fit_batch_n_batches_per_step(
-        self, x, y, batches_per_step, examples_in_step, *, callback=Callback(), step=None, return_pred=False
+        self,
+        x,
+        y,
+        batches_per_step,
+        examples_in_step,
+        *,
+        callback=Callback(),
+        step=None,
+        return_pred=False,
+        convert_to_numpy=True,
     ):
         # pylint: disable=too-many-locals
         zero_all_gradients = (step.number - 1) % batches_per_step == 0
         do_backprop = step.number % batches_per_step == 0
 
         if zero_all_gradients:
             self.optimizer.zero_grad()
 
-        loss_tensor, metrics, pred_y = self._compute_loss_and_metrics(
-            x, y, return_loss_tensor=True, return_pred=return_pred
+        loss_tensor, batch_metrics, torch_metrics, pred_y = self._compute_loss_and_metrics(
+            x, y, return_loss_tensor=True, return_pred=return_pred, convert_to_numpy=convert_to_numpy
         )
 
         adjusted_loss_tensor = loss_tensor * step.size
         adjusted_loss_tensor.backward()
 
         callback.on_backward_end(step)
 
         if do_backprop:
             self._adjust_step_size(examples_in_step)
             self.optimizer.step()
 
         loss = float(loss_tensor)
-        return loss, metrics, do_backprop, pred_y
+        return loss, batch_metrics, torch_metrics, do_backprop, pred_y
 
     def _fit_generator_one_batch_per_step(self, epoch_iterator, callback_list):
         for train_step_iterator, valid_step_iterator in epoch_iterator:
             with self._set_training_mode(True):
                 for step, (x, y) in train_step_iterator:
-                    step.loss, step.metrics, _ = self._fit_batch(x, y, callback=callback_list, step=step.number)
+                    step.loss, step.batch_metrics, step.torch_metrics, _ = self._fit_batch(
+                        x, y, callback=callback_list, step=step.number
+                    )
                     step.size = self.get_batch_size(x, y)
 
             train_step_iterator.epoch_metrics = self._get_epoch_metrics()
+            train_step_iterator.torch_metrics = self._get_torch_metrics()
 
-            if valid_step_iterator is not None:
-                callback_list.on_valid_begin({})
-                valid_begin_time = timeit.default_timer()
-                self._validate(valid_step_iterator)
-
-                valid_step_iterator.epoch_metrics = self._get_epoch_metrics()
-                valid_total_time = timeit.default_timer() - valid_begin_time
-
-                valid_metrics_log = {'time': valid_total_time}
-                valid_metrics_log.update(valid_step_iterator.metrics_logs)
+            self._run_validation(valid_step_iterator, callback_list)
 
-                callback_list.on_valid_end(valid_metrics_log)
-
-    def _fit_batch(self, x, y, *, callback=Callback(), step=None, return_pred=False):
+    def _fit_batch(self, x, y, *, callback=Callback(), step=None, return_pred=False, convert_to_numpy=True):
         self.optimizer.zero_grad()
 
-        loss_tensor, metrics, pred_y = self._compute_loss_and_metrics(
-            x, y, return_loss_tensor=True, return_pred=return_pred
+        loss_tensor, batch_metrics, torch_metrics, pred_y = self._compute_loss_and_metrics(
+            x, y, return_loss_tensor=True, return_pred=return_pred, convert_to_numpy=convert_to_numpy
         )
 
         loss_tensor.backward()
         callback.on_backward_end(step)
         self.optimizer.step()
 
         loss = float(loss_tensor)
-        return loss, metrics, pred_y
+        return loss, batch_metrics, torch_metrics, pred_y
+
+    def _run_validation(self, valid_step_iterator, callback_list):
+        if valid_step_iterator is not None:
+            valid_begin_time = timeit.default_timer()
+
+            callback_list.on_valid_begin({})
+            self._validate(valid_step_iterator)
+
+            valid_step_iterator.epoch_metrics = self._get_epoch_metrics()
+            valid_step_iterator.torch_metrics = self._get_torch_metrics()
+
+            valid_total_time = timeit.default_timer() - valid_begin_time
+
+            valid_metrics_log = {'time': valid_total_time}
+            valid_metrics_log.update(valid_step_iterator.metrics_logs)
+
+            callback_list.on_valid_end(valid_metrics_log)
 
     def _adjust_step_size(self, examples_in_step):
         for param in self.network.parameters():
             if param.grad is not None:
                 param.grad /= examples_in_step
 
     def _process_input(self, *args):
@@ -658,28 +728,34 @@
         if y is not None:
             x, y = self._process_input(x, y)
         else:
             x = self._process_input(x)
 
         x = x if isinstance(x, (tuple, list)) else (x,)
 
+        # We return PackedSequence in a tuple since it is a namedtuple, thus an iterator object and
+        # would break later when we call self.network(*x) since it will iterate over the PackedSequence named attribute.
+        x = (x,) if isinstance(x, PackedSequence) else x
+
         return (x, y) if y is not None else x
 
-    def train_on_batch(self, x, y, return_pred=False, return_dict_format=False):
+    def train_on_batch(self, x, y, *, return_pred=False, return_dict_format=False, convert_to_numpy=True):
         """
         Trains the network for the batch ``(x, y)`` and computes the loss and the metrics, and
         optionally returns the predictions.
 
         Args:
             x: Input data as a batch.
             y: Target data as a batch.
             return_pred (bool, optional): Whether to return the predictions.
                 (Default value = False)
             return_dict_format (bool, optional): Whether to return the loss and metrics in a dict format or not.
                 (Default value = False)
+            convert_to_numpy (bool, optional): Whether to convert the predictions into Numpy Arrays when ``return_pred``
+                is true. (Default value = True)
 
         Returns:
             Float ``loss`` if no metrics were specified and ``return_pred`` is false.
 
             Otherwise, tuple ``(loss, metrics)`` if ``return_pred`` is false.
             ``metrics`` is a Numpy array of size ``n``, where ``n`` is the
             number of metrics if ``n > 1``. If ``n == 1``, then ``metrics`` is a
@@ -693,22 +769,26 @@
             dictionary.
         """
         if self.optimizer is None:
             raise ValueError("Impossible to fit when optimizer is None.")
 
         with self._set_training_mode(True):
             self._transfer_optimizer_state_to_right_device()
-            loss, metrics, pred_y = self._fit_batch(x, y, return_pred=return_pred)
+            loss, batch_metrics, torch_metrics, pred_y = self._fit_batch(
+                x, y, return_pred=return_pred, convert_to_numpy=convert_to_numpy
+            )
 
         if return_dict_format:
             logs = dict(loss=loss)
-            logs.update(zip(self.batch_metrics_names, metrics))
+            logs.update(zip(self.batch_metrics_names, batch_metrics))
+            logs.update(zip(self.torch_metrics_names, torch_metrics))
 
             return self._format_truth_pred_return((logs,), pred_y, return_pred)
 
+        metrics = np.concatenate((batch_metrics, torch_metrics))
         return self._format_loss_metrics_return(loss, metrics, pred_y, return_pred)
 
     def _format_loss_metrics_return(self, loss, metrics, pred_y, return_pred, true_y=None, return_ground_truth=False):
         # pylint: disable=too-many-arguments
         ret = (loss,)
 
         ret += tuple(metrics.tolist()) if len(metrics) <= 1 else (metrics,)
@@ -726,14 +806,15 @@
         return init[0] if len(init) == 1 else init
 
     def predict(
         self,
         x,
         *,
         batch_size=32,
+        convert_to_numpy=True,
         verbose=True,
         progress_options: Union[dict, None] = None,
         callbacks=None,
         dataloader_kwargs=None,
     ) -> Any:
         """
         Returns the predictions of the network given a dataset ``x``, where the tensors are
@@ -741,14 +822,16 @@
 
         Args:
             x (Union[~torch.Tensor, ~numpy.ndarray] or Union[tuple, list] of Union[~torch.Tensor, ~numpy.ndarray]):
                 Input to the model. Union[Tensor, ndarray] if the model has a single input.
                 Union[tuple, list] of Union[Tensor, ndarray] if the model has multiple inputs.
             batch_size (int): Number of samples given to the network at one time.
                 (Default value = 32)
+            concatenate_returns (bool, optional): Whether to concatenate the predictions when returning them.
+                (Default value = True)
             verbose (bool): Whether to display the progress of the evaluation.
                 (Default value = True)
             progress_options (dict, optional): Keyword arguments to pass to the default progression callback used
                 in Poutyne (See :class:`~poutyne.ProgressionCallback` for the available arguments).
                 (Default value = None, meaning default color setting and progress bar)
             callbacks (List[~poutyne.Callback]): List of callbacks that will be called during
                 testing. (Default value = None)
@@ -760,14 +843,15 @@
         """
         x = x if isinstance(x, (tuple, list)) else (x,)
         dataset = self._dataset_from_data(x)
         return self.predict_dataset(
             dataset,
             batch_size=batch_size,
             concatenate_returns=True,
+            convert_to_numpy=convert_to_numpy,
             dataloader_kwargs=dataloader_kwargs,
             verbose=verbose,
             progress_options=progress_options,
             callbacks=callbacks,
         )
 
     def predict_dataset(
@@ -775,14 +859,15 @@
         dataset,
         *,
         batch_size=32,
         steps=None,
         has_ground_truth=False,
         return_ground_truth=False,
         concatenate_returns=True,
+        convert_to_numpy=True,
         num_workers=0,
         collate_fn=None,
         verbose=True,
         progress_options: Union[dict, None] = None,
         callbacks=None,
         dataloader_kwargs=None,
     ) -> Any:
@@ -800,14 +885,16 @@
             has_ground_truth (bool, optional): Whether the generator yields the target ``y``.  Automatically
                 set to true if `return_ground_truth` is true. (Default value = False)
             return_ground_truth (bool, optional): Whether to return the ground truths. If true, automatically
                 set `has_ground_truth` to true. (Default value = False)
             concatenate_returns (bool, optional): Whether to concatenate the predictions
                 or the ground truths when returning them. See :func:`predict_generator()`
                 for details. (Default value = True)
+            concatenate_returns (bool, optional): Whether to concatenate the predictions
+                or the ground truths when returning them. (Default value = True)
             num_workers (int, optional): how many subprocesses to use for data loading.
                 ``0`` means that the data will be loaded in the main process.
                 (Default value = 0)
             collate_fn (Callable, optional): merges a list of samples to form a mini-batch of Tensor(s).
                 Used when using batched loading from a map-style dataset.
             verbose (bool): Whether to display the progress of the evaluation.
                 (Default value = True)
@@ -841,27 +928,29 @@
         generator = DataLoader(dataset, **dataloader_kwargs)
         return self.predict_generator(
             generator,
             steps=steps,
             has_ground_truth=has_ground_truth,
             return_ground_truth=return_ground_truth,
             concatenate_returns=concatenate_returns,
+            convert_to_numpy=convert_to_numpy,
             verbose=verbose,
             progress_options=progress_options,
             callbacks=callbacks,
         )
 
     def predict_generator(
         self,
         generator,
         *,
         steps=None,
         has_ground_truth=False,
         return_ground_truth=False,
         concatenate_returns=True,
+        convert_to_numpy=True,
         verbose=True,
         progress_options: Union[dict, None] = None,
         callbacks=None,
     ) -> Any:
         """
         Returns the predictions of the network given batches of samples ``x``, where the tensors are
         converted into Numpy arrays.
@@ -875,14 +964,16 @@
                 (Defaults the number of steps needed to see the entire dataset)
             has_ground_truth (bool, optional): Whether the generator yields the target ``y``.  Automatically
                 set to true if `return_ground_truth` is true. (Default value = False)
             return_ground_truth (bool, optional): Whether to return the ground truths. If true, automatically
                 set `has_ground_truth` to true. (Default value = False)
             concatenate_returns (bool, optional): Whether to concatenate the predictions
                 or the ground truths when returning them. (Default value = True)
+            convert_to_numpy (bool, optional): Whether to convert the predictions or ground truths into Numpy Arrays.
+                (Default value = True)
             verbose (bool): Whether to display the progress of the evaluation.
                 (Default value = True)
             progress_options (dict, optional): Keyword arguments to pass to the default progression callback used
                 in Poutyne (See :class:`~poutyne.ProgressionCallback` for the available arguments).
                 (Default value = None, meaning default color setting and progress bar)
             callbacks (List[~poutyne.Callback]): List of callbacks that will be called during
                 testing. (Default value = None)
@@ -919,17 +1010,19 @@
             for step, batch in _get_step_iterator(steps, generator):
                 callback_list.on_predict_batch_begin(step, {})
 
                 if has_ground_truth:
                     x, y = self.preprocess_input(*batch)
                 else:
                     x = self.preprocess_input(batch)
-                pred_y.append(torch_to_numpy(self.network(*x)))
+
+                batch_pred = self.network(*x)
+                pred_y.append(torch_to_numpy(batch_pred) if convert_to_numpy else batch_pred)
                 if return_ground_truth:
-                    true_y.append(torch_to_numpy(y))
+                    true_y.append(torch_to_numpy(y) if convert_to_numpy else y)
 
                 batch_end_time = timeit.default_timer()
                 batch_total_time = batch_end_time - time_since_last_batch
                 time_since_last_batch = batch_end_time
 
                 callback_list.on_predict_batch_end(step, {'batch': step, 'time': batch_total_time})
 
@@ -940,37 +1033,41 @@
 
         callback_list.on_predict_end({'time': timeit.default_timer() - predict_begin_time})
 
         if return_ground_truth:
             return pred_y, true_y
         return pred_y
 
-    def predict_on_batch(self, x) -> Any:
+    def predict_on_batch(self, x, *, convert_to_numpy=True) -> Any:
         """
         Returns the predictions of the network given a batch ``x``, where the tensors are converted
         into Numpy arrays.
 
         Args:
             x: Input data as a batch.
+            convert_to_numpy (bool, optional): Whether to convert the predictions into Numpy Arrays.
+                (Default value = True)
 
         Returns:
             Return the predictions in the format outputted by the model.
         """
         with self._set_training_mode(False):
             x = self.preprocess_input(x)
-            return torch_to_numpy(self.network(*x))
+            y_pred = self.network(*x)
+            return torch_to_numpy(y_pred) if convert_to_numpy else y_pred
 
     def evaluate(
         self,
         x,
         y,
         *,
         batch_size=32,
         return_pred=False,
         return_dict_format=False,
+        convert_to_numpy=True,
         callbacks=None,
         verbose=True,
         progress_options: Union[dict, None] = None,
         dataloader_kwargs=None,
     ) -> Tuple:
         """
         Computes the loss and the metrics of the network on batches of samples and optionally
@@ -986,14 +1083,16 @@
                 Union[tuple, list] of Union[Tensor, ndarray] if the model has multiple outputs.
             batch_size (int): Number of samples given to the network at one time.
                 (Default value = 32)
             return_pred (bool, optional): Whether to return the predictions.
                 (Default value = False)
             return_dict_format (bool, optional): Whether to return the loss and metrics in a dict format or not.
                 (Default value = False)
+            convert_to_numpy (bool, optional): Whether to convert the predictions into Numpy Arrays when ``return_pred``
+                is true. (Default value = True)
             callbacks (List[~poutyne.Callback]): List of callbacks that will be called during
                 testing. (Default value = None)
             verbose (bool): Whether to display the progress of the evaluation.
                 (Default value = True)
             progress_options (dict, optional): Keyword arguments to pass to the default progression callback used
                 in Poutyne (See :class:`~poutyne.ProgressionCallback` for the available arguments).
                 (Default value = None, meaning default color setting and progress bar)
@@ -1021,14 +1120,15 @@
         dataset = self._dataset_from_data((x, y))
         return self.evaluate_dataset(
             dataset,
             batch_size=batch_size,
             return_pred=return_pred,
             return_dict_format=return_dict_format,
             concatenate_returns=True,
+            convert_to_numpy=convert_to_numpy,
             callbacks=callbacks,
             verbose=verbose,
             progress_options=progress_options,
             dataloader_kwargs=dataloader_kwargs,
         )
 
     def evaluate_dataset(
@@ -1037,21 +1137,23 @@
         *,
         batch_size=32,
         steps=None,
         return_pred=False,
         return_ground_truth=False,
         return_dict_format=False,
         concatenate_returns=True,
+        convert_to_numpy=True,
         callbacks=None,
         num_workers=0,
         collate_fn=None,
         dataloader_kwargs=None,
         verbose=True,
         progress_options: Union[dict, None] = None,
     ) -> Tuple:
+        # pylint: disable=too-many-locals
         """
         Computes the loss and the metrics of the network on batches of samples and optionally
         returns the predictions.
 
         Args:
             dataset (~torch.utils.data.Dataset): Dataset.
             batch_size (int): Number of samples given to the network at one time.
@@ -1062,14 +1164,16 @@
                 (Default value = False)
             return_ground_truth (bool, optional): Whether to return the ground truths.
                 (Default value = False)
             return_dict_format (bool, optional): Whether to return the loss and metrics in a dict format or not.
                 (Default value = False)
             concatenate_returns (bool, optional): Whether to concatenate the predictions
                 or the ground truths when returning them. (Default value = True)
+            convert_to_numpy (bool, optional): Whether to convert the predictions or ground truths into Numpy Arrays
+                when ``return_pred`` or ``return_ground_truth`` are true. (Default value = True)
             callbacks (List[~poutyne.Callback]): List of callbacks that will be called during
                 testing. (Default value = None)
             num_workers (int, optional): how many subprocesses to use for data loading.
                 ``0`` means that the data will be loaded in the main process.
                 (Default value = 0)
             collate_fn (Callable, optional): merges a list of samples to form a mini-batch of Tensor(s).
                 Used when using batched loading from a map-style dataset.
@@ -1114,28 +1218,30 @@
         return self.evaluate_generator(
             generator,
             steps=steps,
             return_pred=return_pred,
             return_ground_truth=return_ground_truth,
             return_dict_format=return_dict_format,
             concatenate_returns=concatenate_returns,
+            convert_to_numpy=convert_to_numpy,
             callbacks=callbacks,
             verbose=verbose,
             progress_options=progress_options,
         )
 
     def evaluate_generator(
         self,
         generator,
         *,
         steps=None,
         return_pred=False,
         return_ground_truth=False,
         return_dict_format=False,
         concatenate_returns=True,
+        convert_to_numpy=True,
         verbose=True,
         progress_options: Union[dict, None] = None,
         callbacks=None,
     ) -> Tuple:
         # pylint: disable=too-many-locals
         """
         Computes the loss and the metrics of the network on batches of samples and optionally returns
@@ -1148,14 +1254,16 @@
                 (Defaults the number of steps needed to see the entire dataset)
             return_pred (bool, optional): Whether to return the predictions.
                 (Default value = False)
             return_ground_truth (bool, optional): Whether to return the ground truths.
                 (Default value = False)
             return_dict_format (bool, optional): Whether to return the loss and metrics in a dict format or not.
                 (Default value = False)
+            convert_to_numpy (bool, optional): Whether to convert the predictions or ground truths into Numpy Arrays
+                when ``return_pred`` or ``return_ground_truth`` are true. (Default value = True)
             concatenate_returns (bool, optional): Whether to concatenate the predictions
                 or the ground truths when returning them. (Default value = True)
             verbose (bool): Whether to display the progress of the evaluation.
                 (Default value = True)
             progress_options (dict, optional): Keyword arguments to pass to the default progression callback used
                 in Poutyne (See :class:`~poutyne.ProgressionCallback` for the available arguments).
                 (Default value = None, meaning default color setting and progress bar)
@@ -1255,23 +1363,33 @@
         callback_list = CallbackList(callbacks)
         callback_list.set_model(self)
 
         callback_list.set_params({'steps': steps})
         callback_list.on_test_begin({})
 
         step_iterator = StepIterator(
-            generator, steps, self.batch_metrics_names, self.epoch_metrics_names, callback_list, mode="test"
+            generator,
+            steps,
+            self.batch_metrics_names,
+            self.epoch_metrics_names,
+            self.torch_metrics_names,
+            callback_list,
+            mode="test",
         )
 
         test_begin_time = timeit.default_timer()
         loss, batch_metrics, pred_y, true_y = self._validate(
-            step_iterator, return_pred=return_pred, return_ground_truth=return_ground_truth
+            step_iterator,
+            return_pred=return_pred,
+            return_ground_truth=return_ground_truth,
+            convert_to_numpy=convert_to_numpy,
         )
 
         step_iterator.epoch_metrics = self._get_epoch_metrics()
+        step_iterator.torch_metrics = self._get_torch_metrics()
         test_total_time = timeit.default_timer() - test_begin_time
 
         if return_pred and concatenate_returns:
             pred_y = _concat(pred_y)
         if return_ground_truth and concatenate_returns:
             true_y = _concat(true_y)
 
@@ -1279,29 +1397,31 @@
         test_metrics_log.update(step_iterator.metrics_logs)
 
         callback_list.on_test_end(test_metrics_log)
 
         if return_dict_format:
             return self._format_truth_pred_return((test_metrics_log,), pred_y, return_pred, true_y, return_ground_truth)
 
-        metrics = np.concatenate((batch_metrics, step_iterator.epoch_metrics))
+        metrics = np.concatenate((batch_metrics, step_iterator.epoch_metrics, step_iterator.torch_metrics))
         return self._format_loss_metrics_return(loss, metrics, pred_y, return_pred, true_y, return_ground_truth)
 
-    def evaluate_on_batch(self, x, y, *, return_pred=False, return_dict_format=False) -> Tuple:
+    def evaluate_on_batch(self, x, y, *, return_pred=False, return_dict_format=False, convert_to_numpy=True) -> Tuple:
         """
         Computes the loss and the metrics of the network on a single batch of samples and optionally
         returns the predictions.
 
         Args:
             x: Input data as a batch.
             y: Target data as a batch.
             return_pred (bool, optional): Whether to return the predictions for ``batch``.
                 (Default value = False)
             return_dict_format (bool, optional): Whether to return the loss and metrics in a dict format or not.
                 (Default value = False)
+            convert_to_numpy (bool, optional): Whether to convert the predictions into Numpy Arrays when ``return_pred``
+                is true. (Default value = True)
 
         Returns:
             Tuple ``(loss, metrics, pred_y)`` where specific elements are omitted if not
             applicable. If only loss is applicable, then it is returned as a float.
 
             `metrics`` is a Numpy array of size ``n``, where ``n`` is the
             number of metrics if ``n > 1``. If ``n == 1``, then ``metrics`` is a
@@ -1310,71 +1430,94 @@
             If ``return_pred`` is True, ``pred_y`` is the list of the predictions
             of each batch with tensors converted into Numpy arrays. It is otherwise omitted.
 
             If ``return_dict_format`` is True, then ``loss, metrics`` are replaced by a
             dictionary.
         """
         with self._set_training_mode(False):
-            loss, metrics, pred_y = self._compute_loss_and_metrics(x, y, return_pred=return_pred)
+            loss, batch_metrics, torch_metrics, pred_y = self._compute_loss_and_metrics(
+                x, y, return_pred=return_pred, convert_to_numpy=convert_to_numpy
+            )
 
         if return_dict_format:
             logs = dict(loss=loss)
-            logs.update(zip(self.batch_metrics_names, metrics))
+            logs.update(zip(self.batch_metrics_names, batch_metrics))
+            logs.update(zip(self.torch_metrics_names, torch_metrics))
 
             return self._format_truth_pred_return((logs,), pred_y, return_pred)
 
+        metrics = np.concatenate((batch_metrics, torch_metrics))
         return self._format_loss_metrics_return(loss, metrics, pred_y, return_pred)
 
-    def _validate(self, step_iterator, return_pred=False, return_ground_truth=False):
+    def _validate(self, step_iterator, return_pred=False, return_ground_truth=False, convert_to_numpy=True):
         pred_list = None
         true_list = None
         if return_pred:
             pred_list = []
         if return_ground_truth:
             true_list = []
 
         with self._set_training_mode(False):
             for step, (x, y) in step_iterator:
-                step.loss, step.metrics, pred_y = self._compute_loss_and_metrics(x, y, return_pred=return_pred)
+                step.loss, step.batch_metrics, step.torch_metrics, pred_y = self._compute_loss_and_metrics(
+                    x,
+                    y,
+                    return_pred=return_pred,
+                    convert_to_numpy=convert_to_numpy,
+                )
                 if return_pred:
                     pred_list.append(pred_y)
                 if return_ground_truth:
-                    true_list.append(torch_to_numpy(y))
+                    true_list.append(torch_to_numpy(y) if convert_to_numpy else y)
 
                 step.size = self.get_batch_size(x, y)
 
         return step_iterator.loss, step_iterator.batch_metrics, pred_list, true_list
 
-    def _compute_loss_and_metrics(self, x, y, return_loss_tensor=False, return_pred=False):
+    def _compute_loss_and_metrics(self, x, y, *, return_loss_tensor=False, return_pred=False, convert_to_numpy=True):
         x, y = self.preprocess_input(x, y)
         if self.other_device is not None:
             pred_y = torch.nn.parallel.data_parallel(self.network, x, [self.device] + self.other_device)
         else:
             pred_y = self.network(*x)
         loss = self.loss_function(pred_y, y)
         if not return_loss_tensor:
             loss = float(loss)
         with torch.no_grad():
-            metrics = self._compute_batch_metrics(pred_y, y)
+            batch_metrics, torch_metrics = self._compute_batch_and_torch_metrics(pred_y, y)
             for epoch_metric in self.epoch_metrics:
-                epoch_metric(pred_y, y)
+                epoch_metric.update(pred_y, y)
+
+        if return_pred:
+            pred_y = torch_to_numpy(pred_y) if convert_to_numpy else pred_y
+        else:
+            pred_y = None
 
-        pred_y = torch_to_numpy(pred_y) if return_pred else None
-        return loss, metrics, pred_y
+        return loss, batch_metrics, torch_metrics, pred_y
 
-    def _compute_batch_metrics(self, pred_y, y):
-        metrics = [metric(pred_y, y) for metric in self.batch_metrics]
-        return self._compute_metric_array(metrics, self.original_batch_metrics_names)
+    def _compute_batch_and_torch_metrics(self, pred_y, y):
+        batch_metrics = [metric(pred_y, y) for metric in self.batch_metrics]
+        torch_metrics = [metric(pred_y, y) for metric in self.torch_metrics]
+        return (
+            self._compute_metric_array(batch_metrics, self.original_batch_metrics_names),
+            self._compute_metric_array(torch_metrics, self.original_torch_metrics_names),
+        )
 
     def _get_epoch_metrics(self):
-        metrics = [epoch_metric.get_metric() for epoch_metric in self.epoch_metrics]
+        metrics = [epoch_metric.compute() for epoch_metric in self.epoch_metrics]
         for epoch_metric in self.epoch_metrics:
             epoch_metric.reset()
         return self._compute_metric_array(metrics, self.original_epoch_metrics_names)
 
+    def _get_torch_metrics(self):
+        metrics = [torch_metric.compute() for torch_metric in self.torch_metrics]
+        for torch_metric in self.torch_metrics:
+            torch_metric.reset()
+        return self._compute_metric_array(metrics, self.original_torch_metrics_names)
+
     def _compute_metric_array(self, metrics_list, names_list):
         def _get_metric(names, metrics):
             names = [names] if isinstance(names, str) else names
             values = None
             if (torch.is_tensor(metrics) or isinstance(metrics, np.ndarray)) and len(metrics.shape) == 0:
                 values = [float(metrics)]
             elif isinstance(metrics, Mapping):
@@ -1700,12 +1843,12 @@
         self._transfer_loss_and_metrics_modules_to_right_device()
         return self
 
     def _transfer_loss_and_metrics_modules_to_right_device(self):
         if isinstance(self.loss_function, torch.nn.Module):
             self.loss_function.to(self.device)
 
-        for metric in self.batch_metrics + self.epoch_metrics:
+        for metric in self.batch_metrics + self.epoch_metrics + self.torch_metrics:
             if isinstance(metric, torch.nn.Module):
                 metric.to(self.device)
 
         return self
```

### Comparing `Poutyne-1.8/poutyne/plotting.py` & `Poutyne-1.9/poutyne/plotting.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 import os
 import itertools
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 try:
     import matplotlib.pyplot as plt
     from matplotlib.ticker import MaxNLocator
```

### Comparing `Poutyne-1.8/poutyne/utils.py` & `Poutyne-1.9/poutyne/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,32 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 # -*- coding: utf-8 -*-
 import random
+
 import numpy as np
 import torch
+from torch.nn.utils.rnn import PackedSequence
 from torch.utils.data import Dataset
 
 
 def torch_to_numpy(obj, copy=False):
     """
     Convert to Numpy arrays all tensors inside a Python object composed of the supported types.
 
@@ -63,30 +84,37 @@
     """
     fn = lambda t: func(t) if torch.is_tensor(t) else t
     return _apply(obj, fn)
 
 
 def _apply(obj, func):
     if isinstance(obj, (list, tuple)):
+        if isinstance(obj, PackedSequence):
+            return type(obj)(
+                *(_apply(getattr(obj, el), func) if el != "batch_sizes" else getattr(obj, el) for el in obj._fields)
+            )
         return type(obj)(_apply(el, func) for el in obj)
     if isinstance(obj, dict):
         return {k: _apply(el, func) for k, el in obj.items()}
     return func(obj)
 
 
 def _concat(obj):
-    if isinstance(obj[0], (list, tuple)):
-        return type(obj[0])(_concat(ele) for ele in zip(*obj))
-    if isinstance(obj[0], dict):
+    first_item = obj[0]
+    if isinstance(first_item, (list, tuple)):
+        return type(first_item)(_concat(ele) for ele in zip(*obj))
+    if isinstance(first_item, dict):
         concat_dict = {}
-        for key in obj[0].keys():
+        for key in first_item.keys():
             concat_dict[key] = _concat([o[key] for o in obj])
         return concat_dict
-    if isinstance(obj[0], np.ndarray) and obj[0].shape != ():
+    if isinstance(first_item, np.ndarray) and len(first_item.shape) != 0:
         return np.concatenate(obj)
+    if torch.is_tensor(first_item) and len(first_item.shape) != 0:
+        return torch.cat(obj)
     return obj
 
 
 def numpy_to_torch(obj):
     """
     Convert to tensors all Numpy arrays inside a Python object composed of the supported types.
```

### Comparing `Poutyne-1.8/setup.py` & `Poutyne-1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             'Programming Language :: Python :: 3.9',
             'Topic :: Software Development :: Libraries',
             'Topic :: Software Development :: Libraries :: Python Modules',
             'Topic :: Scientific/Engineering',
             'Topic :: Scientific/Engineering :: Artificial Intelligence',
         ],
         packages=packages,
-        install_requires=['numpy', 'torch'],
+        install_requires=['numpy', 'torch', 'torchmetrics'],
         python_requires='>=3.6.1',
         description='A simplified framework and utilities for PyTorch.',
         long_description=readme,
         long_description_content_type='text/markdown',
         extras_require={
             "colorama": "colorama>=0.4.3",
             "scikit-learn": "scikit-learn>=0.23.2",
```

### Comparing `Poutyne-1.8/tests/framework/callbacks/test_checkpoint.py` & `Poutyne-1.9/tests/framework/callbacks/test_checkpoint.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 import os
 
 import unittest
 from unittest import TestCase
 
 from tempfile import TemporaryDirectory
```

### Comparing `Poutyne-1.8/tests/framework/callbacks/test_delay.py` & `Poutyne-1.9/tests/framework/callbacks/test_delay.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,34 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 import unittest
 from unittest import TestCase
 from unittest.mock import MagicMock, call, ANY
 
 import torch
 import torch.nn as nn
 
-from poutyne import Model, DelayCallback, Callback
+from poutyne import Model, DelayCallback, Callback, CallbackList
 from tests.framework.tools import some_data_generator
 
 
 class DelayCallbackTest(TestCase):
     epochs = 10
     steps_per_epoch = 5
     batch_size = 20
@@ -71,14 +90,21 @@
 
     def test_batch_delay_at_begin_of_epoch(self):
         self._test_batch_delay(epoch_delay=5, batch_in_epoch_delay=0)
 
     def test_batch_delay_when_no_delay(self):
         self._test_batch_delay(epoch_delay=0, batch_in_epoch_delay=0)
 
+    def test_proper_init_with_callback_element(self):
+        delay_callback = DelayCallback([self.mock_callback])
+        self.assertTrue(isinstance(delay_callback.callbacks, CallbackList))
+
+        delay_callback = DelayCallback(self.mock_callback)
+        self.assertTrue(isinstance(delay_callback.callbacks, CallbackList))
+
     def _test_batch_delay(self, epoch_delay, batch_in_epoch_delay):
         batch_delay = epoch_delay * DelayCallbackTest.steps_per_epoch + batch_in_epoch_delay
         delay_callback = DelayCallback(self.mock_callback, batch_delay=batch_delay)
         train_generator = some_data_generator(DelayCallbackTest.batch_size)
         valid_generator = some_data_generator(DelayCallbackTest.batch_size)
         self.model.fit_generator(
             train_generator,
```

### Comparing `Poutyne-1.8/tests/framework/callbacks/test_lambda.py` & `Poutyne-1.9/tests/framework/callbacks/test_lambda.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 from unittest.mock import Mock, call
 
 import torch
 import torch.nn as nn
 
 from poutyne import Model, LambdaCallback, Callback
 from tests.framework.tools import some_data_tensor_generator
```

### Comparing `Poutyne-1.8/tests/framework/callbacks/test_logger.py` & `Poutyne-1.9/tests/framework/callbacks/test_logger.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 import csv
 import os
 from tempfile import TemporaryDirectory
 from unittest import TestCase, skipIf, main
 from unittest.mock import MagicMock, call
 
 import torch
@@ -207,9 +226,80 @@
 
 
 @skipIf(TorchSummaryWriter is None, "Unable to import SummaryWriter from torch")
 class TorchTensorboardLoggerTest(BaseTensorBoardLoggerTest, TestCase):
     SummaryWriter = TorchSummaryWriter
 
 
+class BaseTensorBoardLoggerWithSplitTrainValTest:
+    SummaryWriter = None
+    batch_size = 20
+    lr = 1e-3
+    num_epochs = 10
+
+    def setUp(self):
+        torch.manual_seed(42)
+        self.pytorch_network = nn.Linear(1, 1)
+        self.loss_function = nn.MSELoss()
+        self.optimizer = torch.optim.SGD(self.pytorch_network.parameters(), lr=BaseTensorBoardLoggerTest.lr)
+        self.model = Model(self.pytorch_network, self.optimizer, self.loss_function)
+        self.temp_dir_obj = TemporaryDirectory()
+        # pylint: disable=not-callable
+        self.writer = self.SummaryWriter(self.temp_dir_obj.name)
+        self.writer.add_scalar = MagicMock()
+
+    def tearDown(self):
+        self.temp_dir_obj.cleanup()
+
+    def test_logging(self):
+        train_gen = some_data_generator(20)
+        valid_gen = some_data_generator(20)
+        logger = TensorBoardLogger(self.writer, split_train_val=True)
+        history = self.model.fit_generator(
+            train_gen, valid_gen, epochs=self.num_epochs, steps_per_epoch=5, callbacks=[logger]
+        )
+        self._test_logging(history)
+
+    def test_multiple_learning_rates(self):
+        train_gen = some_data_generator(20)
+        valid_gen = some_data_generator(20)
+        logger = TensorBoardLogger(self.writer, split_train_val=True)
+        lrs = [BaseCSVLoggerTest.lr, BaseCSVLoggerTest.lr / 2]
+        optimizer = torch.optim.SGD(
+            [dict(params=[self.pytorch_network.weight], lr=lrs[0]), dict(params=[self.pytorch_network.bias], lr=lrs[1])]
+        )
+        model = Model(self.pytorch_network, optimizer, self.loss_function)
+        history = model.fit_generator(
+            train_gen, valid_gen, epochs=self.num_epochs, steps_per_epoch=5, callbacks=[logger]
+        )
+        self._test_logging(history, lrs=lrs)
+
+    def _test_logging(self, history, lrs=None):
+        if lrs is None:
+            lrs = [BaseCSVLoggerTest.lr]
+
+        calls = []
+        for h in history:
+            for k, v in h.items():
+                calls.append(call(k, v, h['epoch']))
+
+            if len(lrs) == 1:
+                calls.append(call('lr', self.lr, h['epoch']))
+            else:
+                for i, lr in enumerate(lrs):
+                    calls.append(call(f'lr_group_{i}', lr, h['epoch']))
+
+        self.writer.add_scalar.assert_has_calls(calls, any_order=True)
+
+
+@skipIf(XSummaryWriter is None, "Needs tensorboardX to run this test")
+class TensorboardXLoggerWithSplitTrainValTest(BaseTensorBoardLoggerWithSplitTrainValTest, TestCase):
+    SummaryWriter = XSummaryWriter
+
+
+@skipIf(TorchSummaryWriter is None, "Unable to import SummaryWriter from torch")
+class TorchTensorboardLoggerWithSplitTrainValTest(BaseTensorBoardLoggerWithSplitTrainValTest, TestCase):
+    SummaryWriter = TorchSummaryWriter
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `Poutyne-1.8/tests/framework/callbacks/test_mlflow_logger.py` & `Poutyne-1.9/tests/framework/callbacks/test_mlflow_logger.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,41 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 import os
+from typing import List, Dict
 from typing import Mapping, Sequence
 from unittest import TestCase
 from unittest.mock import patch, MagicMock, call
 
 import git
+import torch
+import torch.nn as nn
 from mlflow.exceptions import MlflowException
 from omegaconf import DictConfig
 
+from poutyne import Model
 from poutyne.framework.callbacks.mlflow_logger import _get_git_commit, MLFlowLogger
+from tests.framework.tools import SomeDataGeneratorWithLen
 
 a_git_commit = "9bff900c30e80c3a35388d3e617db5b7a64c9afd"
 mlflow_default_git_commit_tag = "mlflow.source.git.commit"
 
 
 class MLFlowLoggerTest(TestCase):
     def setUp(self) -> None:
@@ -26,30 +50,37 @@
 
         self.experiment_mock = MagicMock()
         self.experiment_mock.return_value = self.a_experiment_id
 
         self.run_mock = MagicMock()
         self.run_mock.return_value.info.run_id = self.a_run_id
 
-        self.epochs = 1
+        self.num_epochs = 2
+        self.steps_per_epoch = 5
+        self.batch_size = 32
         self.a_log = {"metric_1": 1, "metric_2": 2}
 
         self.settings_in_dict = {"param_1": 1, "param_2": 2, "param_3": "value"}
-        self.settings_in_dictconfig_no_sequence = DictConfig(
+        self.settings_in_dict_config_no_sequence = DictConfig(
             {'param_dict': {'param_1': 1}, 'param_dict_2': {'param_2"': 2, 'param_3"': 3}, 'param': 'value'}
         )
-        self.settings_in_dictconfig_with_sequence = DictConfig(
+        self.settings_in_dict_config_with_sequence = DictConfig(
             {
                 'param_dict': {'param_1': 1},
                 'param_dict_2': {'param_2"': 2, 'param_3"': 3},
                 'param': 'value',
                 'a_list_param': [0, 1],
             }
         )
 
+    @patch("poutyne.framework.mlflow_logger.mlflow", None)
+    def test_whenMLFowNotInstalled_thenRaiseImportError(self):
+        with self.assertRaises(ImportError):
+            MLFlowLogger(self.a_experiment_name)
+
     @patch("poutyne.framework.mlflow_logger._get_git_commit", MagicMock())
     def test_whenNewExperiment_givenAMLFlowInstantiation_thenCreateNewExperiment(self):
         with patch("poutyne.framework.mlflow_logger.MlflowClient") as ml_flow_client_patch:
             ml_flow_client_patch.return_value.create_experiment = self.experiment_mock
 
             MLFlowLogger(self.a_experiment_name)
 
@@ -71,15 +102,15 @@
                 call().create_experiment(self.a_experiment_name, self.none_tracking_uri),
                 call().get_experiment_by_name(self.a_experiment_name),
             ]
 
             ml_flow_client_patch.assert_has_calls(create_experiment_calls)
 
     @patch("poutyne.framework.mlflow_logger._get_git_commit", MagicMock())
-    def test_whenCorrectSettings_givenAMLFlowInstantiation_thenMLflowClientIsProperlySet(self):
+    def test_whenCorrectSettings_givenAMLFlowInstantiation_thenMLFlowClientIsProperlySet(self):
         with patch("poutyne.framework.mlflow_logger.MlflowClient") as ml_flow_client_patch:
             ml_flow_client_patch.return_value.create_experiment = self.experiment_mock
             ml_flow_client_patch.return_value.create_run = self.run_mock
 
             mlflow_logger = MLFlowLogger(self.a_experiment_name)
 
             settings_calls = [
@@ -153,54 +184,54 @@
     @patch("poutyne.framework.mlflow_logger._get_git_commit", MagicMock())
     def test_whenLogConfigParamsAConfigDict_givenAMLFlowCallback_thenLogParams(self):
         with patch("poutyne.framework.mlflow_logger.MlflowClient") as ml_flow_client_patch:
             ml_flow_client_patch.return_value.create_experiment = self.experiment_mock
             ml_flow_client_patch.return_value.create_run = self.run_mock
 
             mlflow_logger = MLFlowLogger(self.a_experiment_name)
-            mlflow_logger.log_config_params(self.settings_in_dictconfig_no_sequence)
+            mlflow_logger.log_config_params(self.settings_in_dict_config_no_sequence)
 
-            ml_flow_client_calls = self._populate_calls_from_dict(self.settings_in_dictconfig_no_sequence)
+            ml_flow_client_calls = self._populate_calls_from_dict(self.settings_in_dict_config_no_sequence)
             ml_flow_client_patch.assert_has_calls(ml_flow_client_calls)
 
     @patch("poutyne.framework.mlflow_logger._get_git_commit", MagicMock())
     def test_whenLogConfigParamsAConfigDictWithSequence_givenAMLFlowCallback_thenLogParams(self):
         with patch("poutyne.framework.mlflow_logger.MlflowClient") as ml_flow_client_patch:
             ml_flow_client_patch.return_value.create_experiment = self.experiment_mock
             ml_flow_client_patch.return_value.create_run = self.run_mock
 
             mlflow_logger = MLFlowLogger(self.a_experiment_name)
-            mlflow_logger.log_config_params(self.settings_in_dictconfig_with_sequence)
+            mlflow_logger.log_config_params(self.settings_in_dict_config_with_sequence)
 
-            ml_flow_client_calls = self._populate_calls_from_dict(self.settings_in_dictconfig_with_sequence)
+            ml_flow_client_calls = self._populate_calls_from_dict(self.settings_in_dict_config_with_sequence)
             ml_flow_client_patch.assert_has_calls(ml_flow_client_calls)
 
     @patch("poutyne.framework.mlflow_logger._get_git_commit", MagicMock())
     def test_whenOnTrainEndSuccess_givenAMLFlowCallback_thenLogLastEpochNumber(self):
         with patch("poutyne.framework.mlflow_logger.MlflowClient") as ml_flow_client_patch:
             ml_flow_client_patch.return_value.create_experiment = self.experiment_mock
             ml_flow_client_patch.return_value.create_run = self.run_mock
 
             mlflow_logger = MLFlowLogger(self.a_experiment_name)
-            mlflow_logger.set_params({"epochs": self.epochs})
+            mlflow_logger.set_params({"epochs": self.num_epochs})
             mlflow_logger.on_train_end(self.a_log)
 
             ml_flow_client_calls = [
-                call().log_metric(run_id=self.a_run_id, key='last-epoch', value=self.epochs, step=None)
+                call().log_metric(run_id=self.a_run_id, key='last-epoch', value=self.num_epochs, step=None)
             ]
             ml_flow_client_patch.assert_has_calls(ml_flow_client_calls)
 
     @patch("poutyne.framework.mlflow_logger._get_git_commit", MagicMock())
     def test_whenOnTrainEndSuccess_givenAMLFlowCallback_thenHasSuccessTerminatedStatus(self):
         with patch("poutyne.framework.mlflow_logger.MlflowClient") as ml_flow_client_patch:
             ml_flow_client_patch.return_value.create_experiment = self.experiment_mock
             ml_flow_client_patch.return_value.create_run = self.run_mock
 
             mlflow_logger = MLFlowLogger(self.a_experiment_name)
-            mlflow_logger.set_params({"epochs": self.epochs})
+            mlflow_logger.set_params({"epochs": self.num_epochs})
             mlflow_logger.on_train_end(self.a_log)
 
             ml_flow_client_calls = [call().set_terminated(self.a_run_id, status="FINISHED")]
             ml_flow_client_patch.assert_has_calls(ml_flow_client_calls)
 
     @patch("poutyne.framework.mlflow_logger._get_git_commit", MagicMock())
     def test_whenOnTestFailure_givenAMLFlowCallback_thenHasFailureTerminatedStatus(self):
@@ -218,23 +249,77 @@
     @patch("poutyne.framework.mlflow_logger._get_git_commit", MagicMock())
     def test_whenOnTestSuccess_givenAMLFlowCallback_thenHasSuccessTerminatedStatus(self):
         with patch("poutyne.framework.mlflow_logger.MlflowClient") as ml_flow_client_patch:
             ml_flow_client_patch.return_value.create_experiment = self.experiment_mock
             ml_flow_client_patch.return_value.create_run = self.run_mock
 
             mlflow_logger = MLFlowLogger(self.a_experiment_name)
-            mlflow_logger.set_params({"epochs": self.epochs})
+            mlflow_logger.set_params({"epochs": self.num_epochs})
             mlflow_logger.on_train_end(self.a_log)
             mlflow_logger.on_test_begin({})  # since we change status at the start of testing
             mlflow_logger.on_test_end(self.a_log)
 
             ml_flow_client_calls = [call().set_terminated(self.a_run_id, status="FINISHED")]
             ml_flow_client_patch.assert_has_calls(ml_flow_client_calls)
 
-    def _populate_calls_from_dict(self, config_dict):
+    @patch("poutyne.framework.mlflow_logger._get_git_commit", MagicMock())
+    def test_integration_train(self):
+        with patch("poutyne.framework.mlflow_logger.MlflowClient") as ml_flow_client_patch:
+            ml_flow_client_patch.return_value.create_experiment = self.experiment_mock
+            ml_flow_client_patch.return_value.create_run = self.run_mock
+
+            mlflow_logger = MLFlowLogger(self.a_experiment_name)
+
+            torch.manual_seed(42)
+            a_pytorch_network = nn.Linear(1, 1)
+            a_loss_function = nn.MSELoss()
+            an_optimizer = torch.optim.Adam(a_pytorch_network.parameters(), lr=1e-3)
+            model = Model(a_pytorch_network, an_optimizer, a_loss_function)
+
+            train_generator = SomeDataGeneratorWithLen(self.batch_size, 10, 0)
+            valid_generator = SomeDataGeneratorWithLen(self.batch_size, 10, 0)
+            logs = model.fit_generator(
+                train_generator,
+                valid_generator,
+                epochs=self.num_epochs,
+                steps_per_epoch=self.steps_per_epoch,
+                callbacks=[mlflow_logger],
+            )
+
+            ml_flow_client_calls = self._populate_calls_from_logs(logs)
+            ml_flow_client_patch.assert_has_calls(ml_flow_client_calls)
+
+    @patch("poutyne.framework.mlflow_logger._get_git_commit", MagicMock())
+    def test_integration_train_batch_granularity(self):
+        with patch("poutyne.framework.mlflow_logger.MlflowClient") as ml_flow_client_patch:
+            ml_flow_client_patch.return_value.create_experiment = self.experiment_mock
+            ml_flow_client_patch.return_value.create_run = self.run_mock
+
+            mlflow_logger = MLFlowLogger(self.a_experiment_name, batch_granularity=True)
+
+            torch.manual_seed(42)
+            a_pytorch_network = nn.Linear(1, 1)
+            a_loss_function = nn.MSELoss()
+            an_optimizer = torch.optim.Adam(a_pytorch_network.parameters(), lr=1e-3)
+            model = Model(a_pytorch_network, an_optimizer, a_loss_function)
+
+            train_generator = SomeDataGeneratorWithLen(self.batch_size, 10, 0)
+            valid_generator = SomeDataGeneratorWithLen(self.batch_size, 10, 0)
+            a_num_epoch = 2
+            model.fit_generator(
+                train_generator,
+                valid_generator,
+                epochs=a_num_epoch,
+                steps_per_epoch=self.steps_per_epoch,
+                callbacks=[mlflow_logger],
+            )
+
+            self._assert_has_granularity_calls(ml_flow_client_patch)
+
+    def _populate_calls_from_dict(self, config_dict: Dict) -> List:
         ml_flow_client_calls = []
         for key, value in config_dict.items():
             if isinstance(value, Mapping):
                 for key_lower, value_lower in value.items():
                     good_key = f"{key}.{key_lower}"
                     ml_flow_client_calls.append(call().log_param(run_id=self.a_run_id, key=good_key, value=value_lower))
             elif isinstance(value, Sequence) and not isinstance(value, str):
@@ -243,14 +328,40 @@
                     ml_flow_client_calls.append(
                         (call().log_param(run_id=self.a_run_id, key=good_key, value=value_lower))
                     )
             else:
                 ml_flow_client_calls.append(call().log_param(run_id=self.a_run_id, key=key, value=value))
         return ml_flow_client_calls
 
+    def _populate_calls_from_logs(self, logs: Dict) -> List:
+        ml_flow_client_calls = []
+        for epoch_num, epoch_log in enumerate(logs):
+            epoch_log.pop("epoch")
+            for key, value in epoch_log.items():
+                ml_flow_client_calls.append(
+                    call().log_metric(run_id=self.a_run_id, key=key, value=value, step=epoch_num + 1)
+                )  # +1 for enumerate
+        ml_flow_client_calls.append(
+            call().log_metric(run_id=self.a_run_id, key="last-epoch", value=self.num_epochs, step=None)
+        )
+        ml_flow_client_calls.append(call().set_terminated(self.a_run_id, status='FINISHED'))
+        return ml_flow_client_calls
+
+    def _assert_has_granularity_calls(self, ml_flow_client_patch):
+        for _ in range(1, self.num_epochs):
+            for step_number in range(1, self.steps_per_epoch):
+                ml_flow_client_step_calls = []
+                ml_flow_client_step_calls.append(
+                    call().log_metric(run_id=self.a_run_id, key='batch', value=step_number, step=step_number)
+                )
+                ml_flow_client_step_calls.append(
+                    call().log_metric(run_id=self.a_run_id, key='size', value=self.batch_size, step=step_number)
+                )
+                ml_flow_client_patch.assert_has_calls(ml_flow_client_step_calls)
+
 
 class GetGitCommitTest(TestCase):
     def setUp(self) -> None:
         self.a_fake_path = "a_fake_path"
         self.a_wrong_path = "/a_wrong_path"
         self.a_git_sha = a_git_commit
```

### Comparing `Poutyne-1.8/tests/framework/callbacks/test_periodic.py` & `Poutyne-1.9/tests/framework/callbacks/test_periodic.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,37 @@
-import os
-from typing import Dict, IO
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
 
-import unittest
-from unittest import TestCase
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
 
+import os
+import unittest
 from tempfile import TemporaryDirectory
+from typing import Dict, IO
+from unittest import TestCase
+from unittest.mock import MagicMock, call
 
 import torch
 import torch.nn as nn
 
-from poutyne import Model, PeriodicSaveCallback
+from poutyne import Model, PeriodicSaveCallback, PeriodicSaveLambda
 from tests.framework.tools import some_data_generator
 
 
 class PeriodicEpochSave(PeriodicSaveCallback):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, open_mode='w', read_mode='r', **kwargs)
         self.epoch_number = None
@@ -43,14 +61,42 @@
 
     def test_integration(self):
         train_gen = some_data_generator(PeriodicSaveTest.batch_size)
         valid_gen = some_data_generator(PeriodicSaveTest.batch_size)
         saver = PeriodicEpochSave(self.save_filename, monitor='val_loss', verbose=True, save_best_only=True)
         self.model.fit_generator(train_gen, valid_gen, epochs=10, steps_per_epoch=5, callbacks=[saver])
 
+    def test_mode_not_min_max_raise_error(self):
+        with self.assertRaises(ValueError):
+            invalid_mode = "a_mode"
+            PeriodicEpochSave(
+                self.save_filename, monitor='val_loss', verbose=True, save_best_only=True, mode=invalid_mode
+            )
+
+    def test_incorrect_monitored_metric_name_raise_key_error(self):
+        invalid_monitor_metric_name = "invalid_monitor_metric_name"
+        periodic_epoch_save = PeriodicEpochSave(
+            self.save_filename, monitor=invalid_monitor_metric_name, verbose=True, save_best_only=True
+        )
+
+        an_epoch_number = 1
+        a_log_dict = {"epoch": 1, 'acc': 1.0, 'another_metric_name': 1.0}
+        with self.assertRaises(KeyError):
+            periodic_epoch_save.on_epoch_end(an_epoch_number, a_log_dict)
+
+    def test_integration_correct_monitored_metric_name(self):
+        correct_monitor_metric_name = "val_loss"
+        periodic_epoch_save = PeriodicEpochSave(
+            self.save_filename, monitor=correct_monitor_metric_name, verbose=True, save_best_only=True
+        )
+
+        an_epoch_number = 1
+        a_log_dict = {"epoch": 1, 'acc': 1.0, 'val_loss': 1.0}
+        periodic_epoch_save.on_epoch_end(an_epoch_number, a_log_dict)
+
     def test_integration_with_keep_only_last_best(self):
         train_gen = some_data_generator(PeriodicSaveTest.batch_size)
         valid_gen = some_data_generator(PeriodicSaveTest.batch_size)
         saver = PeriodicEpochSave(
             self.save_filename, monitor='val_loss', verbose=True, save_best_only=True, keep_only_last_best=True
         )
         self.model.fit_generator(train_gen, valid_gen, epochs=10, steps_per_epoch=5, callbacks=[saver])
@@ -166,14 +212,20 @@
             PeriodicEpochSave(
                 self.save_filename, monitor='val_loss', verbose=True, save_best_only=False, restore_best=True
             )
 
         with self.assertRaises(ValueError):
             PeriodicEpochSave(self.save_filename, monitor='val_loss', verbose=True, restore_best=True)
 
+    def test_on_train_end_with_restore_best_without_training_raise_warning(self):
+        checkpointer = PeriodicEpochSave(self.save_filename, monitor='val_loss', save_best_only=True, restore_best=True)
+        a_log = {}
+        with self.assertWarns(UserWarning):
+            checkpointer.on_train_end(a_log)
+
     def _test_saver_with_val_losses(self, saver, val_losses, has_checkpoints, keep_only_last_best=False):
         generator = some_data_generator(PeriodicSaveTest.batch_size)
 
         best_checkpoint_filenames = []
         saver.set_params({'epochs': len(val_losses), 'steps': 1})
         saver.set_model(self.model)
         saver.on_train_begin({})
@@ -210,9 +262,40 @@
         loss.backward()
 
         self.optimizer.step()
 
         return float(loss)
 
 
+class PeriodicSaveLambdaTest(TestCase):
+    def setUp(self) -> None:
+        self.a_filename = "a_file_name"
+
+    def test_given_a_fun_save_file_use_function(self):
+        a_function_mock = MagicMock()
+
+        periodic_save_lambda = PeriodicSaveLambda(filename=self.a_filename, func=a_function_mock)
+        a_file_descriptor_mock = MagicMock()
+        a_epoch_number = 1
+        a_log = {}
+
+        periodic_save_lambda.save_file(a_file_descriptor_mock, a_epoch_number, a_log)
+        a_function_mock.assert_has_calls([call(a_file_descriptor_mock, a_epoch_number, a_log)])
+
+    def test_restore_use_lambda_function(self):
+        a_function_mock = MagicMock()
+
+        a_restore_mock_function = MagicMock()
+        a_restore_function = lambda x: a_restore_mock_function(2)
+
+        periodic_save_lambda = PeriodicSaveLambda(
+            filename=self.a_filename, func=a_function_mock, restore=a_restore_function
+        )
+        a_file_descriptor_mock = MagicMock()
+        periodic_save_lambda.restore(a_file_descriptor_mock)
+
+        a_restore_mock_function.assert_called()
+        a_restore_mock_function.assert_has_calls([call(2)])
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Poutyne-1.8/tests/framework/callbacks/test_progress.py` & `Poutyne-1.9/tests/framework/callbacks/test_progress.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 from typing import List, Union
 from unittest import TestCase
 from unittest.mock import patch, MagicMock, call
 
 from poutyne import ProgressionCallback
```

### Comparing `Poutyne-1.8/tests/framework/callbacks/test_tracker.py` & `Poutyne-1.9/tests/framework/callbacks/test_tracker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,43 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 import math
 from tempfile import TemporaryDirectory
 from unittest import TestCase, skipIf
 from unittest.mock import MagicMock, call, ANY
 
+
 import torch
 import torch.nn as nn
 
 from tests.framework.tools import some_data_generator
 
 try:
     from torch.utils.tensorboard import SummaryWriter
 except ImportError:
     SummaryWriter = None
 
-from poutyne import Model, TensorBoardGradientTracker, WeightsGradientsStatsTracker, Tracker
-
-
-class TrackerTest(TestCase):
-    def test_keep_good_layer(self):
-        # pylint: disable=protected-access
-        tracker = Tracker(keep_bias=False)
-        layer_to_keep_params = MagicMock()
-        layer_to_keep_params.requires_grad = True
-        self.assertTrue(tracker._keep_layer(layer_to_keep_params, "fake_layer_name_to_keep"))
-        self.assertFalse(tracker._keep_layer(layer_to_keep_params, "bias_name_not_to_keep"))
-
-        layer_not_to_keep_params = MagicMock()
-        layer_not_to_keep_params.requires_grad = False
-        self.assertFalse(tracker._keep_layer(layer_not_to_keep_params, "fake_layer_name_not_to_keep"))
-        self.assertFalse(tracker._keep_layer(layer_not_to_keep_params, "bias_name_not_to_keep"))
-
-        tracker = Tracker(keep_bias=True)
-        layer_to_keep_params = MagicMock()
-        layer_to_keep_params.requires_grad = True
-        self.assertTrue(tracker._keep_layer(layer_to_keep_params, "fake_layer_name_to_keep"))
-        self.assertTrue(tracker._keep_layer(layer_to_keep_params, "bias_name_to_keep"))
-
-        layer_not_to_keep_params = MagicMock()
-        layer_not_to_keep_params.requires_grad = False
-        self.assertFalse(tracker._keep_layer(layer_not_to_keep_params, "fake_layer_name_not_to_keep"))
-        self.assertFalse(tracker._keep_layer(layer_not_to_keep_params, "bias_name_not_to_keep"))
+from poutyne import Model, TensorBoardGradientTracker, WeightsGradientsStatsTracker, GradientTracker
 
 
 class GradientStatsTrackerTest(TestCase):
     def setUp(self):
         self.tracker = WeightsGradientsStatsTracker(number_layers=2)
 
         self.absolute_min_both_layer = 0.00
@@ -172,14 +166,67 @@
     def _test_stats(self, expected, actual):
         self.assertEqual(len(expected), len(actual))
         self.assertEqual(expected.keys(), actual.keys())
         for expected_value, actual_value in zip(expected.values(), actual.values()):
             self.assertAlmostEqual(float(expected_value), float(actual_value), places=3)
 
 
+class GradientTrackerTest(TestCase):
+    def test_keep_good_layer(self):
+        # pylint: disable=protected-access
+        gradient_tracker = GradientTracker(keep_bias=False)
+        layer_to_keep_params = MagicMock()
+        layer_to_keep_params.requires_grad = True
+        self.assertTrue(gradient_tracker._keep_layer(layer_to_keep_params, "fake_layer_name_to_keep"))
+        self.assertFalse(gradient_tracker._keep_layer(layer_to_keep_params, "bias_name_not_to_keep"))
+
+        layer_not_to_keep_params = MagicMock()
+        layer_not_to_keep_params.requires_grad = False
+        self.assertFalse(gradient_tracker._keep_layer(layer_not_to_keep_params, "fake_layer_name_not_to_keep"))
+        self.assertFalse(gradient_tracker._keep_layer(layer_not_to_keep_params, "bias_name_not_to_keep"))
+
+        gradient_tracker = GradientTracker(keep_bias=True)
+        layer_to_keep_params = MagicMock()
+        layer_to_keep_params.requires_grad = True
+        self.assertTrue(gradient_tracker._keep_layer(layer_to_keep_params, "fake_layer_name_to_keep"))
+        self.assertTrue(gradient_tracker._keep_layer(layer_to_keep_params, "bias_name_to_keep"))
+
+        layer_not_to_keep_params = MagicMock()
+        layer_not_to_keep_params.requires_grad = False
+        self.assertFalse(gradient_tracker._keep_layer(layer_not_to_keep_params, "fake_layer_name_not_to_keep"))
+        self.assertFalse(gradient_tracker._keep_layer(layer_not_to_keep_params, "bias_name_not_to_keep"))
+
+    def test_integration(self):
+        train_gen = some_data_generator(20)
+        valid_gen = some_data_generator(20)
+        torch.manual_seed(42)
+        self.pytorch_network = nn.Linear(1, 1)
+        self.loss_function = nn.MSELoss()
+        self.optimizer = torch.optim.SGD(self.pytorch_network.parameters(), lr=1e-3)
+        device = torch.device("cpu")
+        self.model = Model(self.pytorch_network, self.optimizer, self.loss_function, device=device)
+        gradient_tracker = GradientTracker()
+
+        self.model.fit_generator(train_gen, valid_gen, epochs=10, steps_per_epoch=5, callbacks=[gradient_tracker])
+
+    @skipIf(not torch.cuda.is_available(), "no gpu available")
+    def test_integration_on_gpu(self):
+        train_gen = some_data_generator(20)
+        valid_gen = some_data_generator(20)
+        torch.manual_seed(42)
+        self.pytorch_network = nn.Linear(1, 1)
+        self.loss_function = nn.MSELoss()
+        self.optimizer = torch.optim.SGD(self.pytorch_network.parameters(), lr=1e-3)
+        device = torch.device("cuda:0")
+        self.model = Model(self.pytorch_network, self.optimizer, self.loss_function, device=device)
+        gradient_tracker = GradientTracker()
+
+        self.model.fit_generator(train_gen, valid_gen, epochs=10, steps_per_epoch=5, callbacks=[gradient_tracker])
+
+
 @skipIf(SummaryWriter is None, "Unable to import SummaryWriter from torch")
 class TensorBoardGradientTrackerTest(TestCase):
     batch_size = 20
     lr = 1e-3
     num_epochs = 10
 
     def setUp(self):
```

### Comparing `Poutyne-1.8/tests/framework/experiment/test_model_bundle.py` & `Poutyne-1.9/tests/framework/experiment/test_experiment.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,137 +1,277 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 import os
 from tempfile import TemporaryDirectory
 from unittest import TestCase
-from unittest.mock import patch, MagicMock
 
+import numpy as np
 import torch
-from pandas import DataFrame, Series
+import pandas as pd
 from torch import nn
 from torch.utils.data import TensorDataset
 
-from poutyne import ModelBundle
+# pylint: disable=no-name-in-module
+from poutyne import Experiment, ExponentialLR
 from tests.framework.tools import SomeDataGeneratorWithLen
+from tests.framework.experiment.utils import ConstantMetric, ConstantMetricCallback
 
 
-class ModelBundleTest(TestCase):
-    NUM_EPOCHS = 5
+class BaseExperimentTest:
+    # pylint: disable=no-member
+    NUM_EPOCHS = None
+    METRIC_VALUES = None
+    CHECKPOINT_EPOCHS = None
+    NO_CHECKPOINT_EPOCHS = None
+    MONITOR_MODE = None
 
     def setUp(self):
         self.temp_dir_obj = TemporaryDirectory()
         self.test_checkpoints_path = os.path.join(self.temp_dir_obj.name, 'expt')
 
-        self.test_experiment = ModelBundle.from_network(
+        self.metric = ConstantMetric()
+        self.metric_callback = ConstantMetricCallback(self.METRIC_VALUES, self.metric)
+
+        self.test_experiment = Experiment(
             self.test_checkpoints_path,
             nn.Linear(1, 1),
             optimizer='sgd',
             loss_function='mse',
-            monitor_metric="loss",
-            monitor_mode="min",
+            batch_metrics=[self.metric],
+            monitor_metric="const",
+            monitor_mode=self.MONITOR_MODE,
         )
-        self.ckpt_1_path = os.path.join(self.test_checkpoints_path, "checkpoint_epoch_1.ckpt")
+        self.checkpoint_paths = [
+            os.path.join(self.test_checkpoints_path, f"checkpoint_epoch_{epoch}.ckpt")
+            for epoch in self.CHECKPOINT_EPOCHS
+        ]
+        self.no_checkpoint_paths = [
+            os.path.join(self.test_checkpoints_path, f"checkpoint_epoch_{epoch}.ckpt")
+            for epoch in self.NO_CHECKPOINT_EPOCHS
+        ]
         self.ckpt_last_path = os.path.join(self.test_checkpoints_path, "checkpoint.ckpt")
         self.optim_ckpt_path = os.path.join(self.test_checkpoints_path, "checkpoint.optim")
+        self.first_lr_scheduler_ckpt_path = os.path.join(self.test_checkpoints_path, "lr_sched_0.lrsched")
+        self.second_lr_scheduler_ckpt_path = os.path.join(self.test_checkpoints_path, "lr_sched_1.lrsched")
         self.tsv_log_path = os.path.join(self.test_checkpoints_path, "log.tsv")
         self.tsv_test_log_path = os.path.join(self.test_checkpoints_path, "test_log.tsv")
         self.epoch_file_path = os.path.join(self.test_checkpoints_path, "last.epoch")
-        self.time_metric_plot_png_file_path = os.path.join(self.test_checkpoints_path, "plots", 'time.png')
-        self.time_metric_plot_pdf_file_path = os.path.join(self.test_checkpoints_path, "plots", 'time.pdf')
-        self.loss_metric_plot_png_file_path = os.path.join(self.test_checkpoints_path, "plots", 'loss.png')
-        self.loss_metric_plot_pdf_file_path = os.path.join(self.test_checkpoints_path, "plots", 'loss.pdf')
+        self.time_metric_plot_png_file_path = os.path.join(self.test_checkpoints_path, "plots", "time.png")
+        self.time_metric_plot_pdf_file_path = os.path.join(self.test_checkpoints_path, "plots", "time.pdf")
+        self.loss_metric_plot_png_file_path = os.path.join(self.test_checkpoints_path, "plots", "loss.png")
+        self.loss_metric_plot_pdf_file_path = os.path.join(self.test_checkpoints_path, "plots", "loss.pdf")
 
     def tearDown(self):
         self.temp_dir_obj.cleanup()
 
     def test_integration_train(self):
         train_generator = SomeDataGeneratorWithLen(32, 10, 0)
         valid_generator = SomeDataGeneratorWithLen(32, 10, 0)
-        logs = self.test_experiment.train(train_generator, valid_generator, epochs=ModelBundleTest.NUM_EPOCHS)
+        logs = self.test_experiment.train(
+            train_generator, valid_generator, epochs=self.NUM_EPOCHS, callbacks=[self.metric_callback]
+        )
         self._test_train_integration(logs)
 
+    def test_integration_train_with_lr_scheduler(self):
+        lr_scheduler = ExponentialLR(0.9)
+
+        train_generator = SomeDataGeneratorWithLen(32, 10, 0)
+        valid_generator = SomeDataGeneratorWithLen(32, 10, 0)
+        logs = self.test_experiment.train(
+            train_generator,
+            valid_generator,
+            epochs=self.NUM_EPOCHS,
+            callbacks=[self.metric_callback],
+            lr_schedulers=[lr_scheduler],
+        )
+        self._test_train_integration(logs, num_lr_schedulers=1)
+
+    def test_integration_train_with_two_lr_schedulers(self):
+        lr_schedulers = [ExponentialLR(0.9), ExponentialLR(0.8)]
+
+        train_generator = SomeDataGeneratorWithLen(32, 10, 0)
+        valid_generator = SomeDataGeneratorWithLen(32, 10, 0)
+        logs = self.test_experiment.train(
+            train_generator,
+            valid_generator,
+            epochs=self.NUM_EPOCHS,
+            callbacks=[self.metric_callback],
+            lr_schedulers=lr_schedulers,
+        )
+        self._test_train_integration(logs, num_lr_schedulers=2)
+
     def test_integration_train_dataset(self):
         train_dataset = TensorDataset(torch.rand(32 * 10, 1), torch.rand(32 * 10, 1))
         valid_dataset = TensorDataset(torch.rand(32 * 10, 1), torch.rand(32 * 10, 1))
-        logs = self.test_experiment.train_dataset(train_dataset, valid_dataset, epochs=ModelBundleTest.NUM_EPOCHS)
+        logs = self.test_experiment.train_dataset(
+            train_dataset, valid_dataset, epochs=self.NUM_EPOCHS, callbacks=[self.metric_callback]
+        )
         self._test_train_integration(logs)
 
     def test_integration_train_data(self):
         train_x, train_y = torch.rand(32 * 10, 1), torch.rand(32 * 10, 1)
         validation_data = torch.rand(32 * 10, 1), torch.rand(32 * 10, 1)
-        logs = self.test_experiment.train_data(train_x, train_y, validation_data, epochs=ModelBundleTest.NUM_EPOCHS)
+        logs = self.test_experiment.train_data(
+            train_x, train_y, validation_data, epochs=self.NUM_EPOCHS, callbacks=[self.metric_callback]
+        )
         self._test_train_integration(logs)
 
     def test_train_resume(self):
         train_generator = SomeDataGeneratorWithLen(32, 10, 0)
         valid_generator = SomeDataGeneratorWithLen(32, 10, 0)
-        logs = self.test_experiment.train(train_generator, valid_generator, epochs=ModelBundleTest.NUM_EPOCHS)
-        self._test_train_integration(logs)
+        lr_schedulers = [ExponentialLR(0.9), ExponentialLR(0.8)]
+        logs = self.test_experiment.train(
+            train_generator,
+            valid_generator,
+            epochs=self.NUM_EPOCHS,
+            callbacks=[self.metric_callback],
+            lr_schedulers=lr_schedulers,
+        )
+        self._test_train_integration(logs, num_lr_schedulers=2)
 
-        epochs = ModelBundleTest.NUM_EPOCHS + 10
-        logs = self.test_experiment.train(train_generator, valid_generator, epochs=epochs)
-        self._test_train_integration(logs, epochs=epochs, initial_epoch=ModelBundleTest.NUM_EPOCHS + 1)
+        epochs = self.NUM_EPOCHS + 10
+        logs = self.test_experiment.train(train_generator, valid_generator, epochs=epochs, lr_schedulers=lr_schedulers)
+        self._test_train_integration(logs, epochs=epochs, initial_epoch=self.NUM_EPOCHS + 1, num_lr_schedulers=2)
 
     def test_train_no_log(self):
-        test_experiment = ModelBundle.from_network(
+        self._test_train_no_log(0)
+
+    def test_train_no_log_with_lr_scheduler(self):
+        self._test_train_no_log(1)
+
+    def test_train_no_log_with_two_lr_schedulers(self):
+        self._test_train_no_log(2)
+
+    def _test_train_no_log(self, num_lr_schedulers):
+        lr_schedulers = None
+        if num_lr_schedulers >= 1:
+            lr_schedulers = [ExponentialLR(0.9 - 0.1 * i) for i in range(num_lr_schedulers)]
+        test_experiment = Experiment(
             self.test_checkpoints_path,
             nn.Linear(1, 1),
             optimizer='sgd',
             loss_function='mse',
-            monitor_metric="loss",
-            monitor_mode="min",
+            batch_metrics=[self.metric],
+            monitor_metric="const",
+            monitor_mode=self.MONITOR_MODE,
             logging=False,
         )
         train_generator = SomeDataGeneratorWithLen(32, 10, 0)
         valid_generator = SomeDataGeneratorWithLen(32, 10, 0)
-        logs = test_experiment.train(train_generator, valid_generator, epochs=ModelBundleTest.NUM_EPOCHS)
+        logs = test_experiment.train(
+            train_generator,
+            valid_generator,
+            epochs=self.NUM_EPOCHS,
+            callbacks=[self.metric_callback],
+            lr_schedulers=lr_schedulers,
+        )
 
         self.assertFalse(os.path.isdir(self.test_checkpoints_path))
-        self.assertFalse(os.path.isfile(self.ckpt_1_path))
+        for path in self.checkpoint_paths:
+            self.assertFalse(os.path.isfile(path))
+        for path in self.no_checkpoint_paths:
+            self.assertFalse(os.path.isfile(path))
         self.assertFalse(os.path.isfile(self.ckpt_last_path))
         self.assertFalse(os.path.isfile(self.optim_ckpt_path))
         self.assertFalse(os.path.isfile(self.tsv_log_path))
         self.assertFalse(os.path.isfile(self.epoch_file_path))
         self.assertFalse(os.path.isfile(self.tsv_test_log_path))
         self.assertFalse(os.path.isfile(self.time_metric_plot_png_file_path))
         self.assertFalse(os.path.isfile(self.time_metric_plot_pdf_file_path))
         self.assertFalse(os.path.isfile(self.loss_metric_plot_png_file_path))
         self.assertFalse(os.path.isfile(self.loss_metric_plot_pdf_file_path))
+        self.assertFalse(os.path.isfile(self.first_lr_scheduler_ckpt_path))
+        self.assertFalse(os.path.isfile(self.second_lr_scheduler_ckpt_path))
 
-        self.assertEqual(len(logs), ModelBundleTest.NUM_EPOCHS)
+        self.assertEqual(len(logs), self.NUM_EPOCHS)
         for i, log in enumerate(logs, 1):
             self.assertIn('epoch', log)
             self.assertEqual(log['epoch'], i)
             self.assertIn('loss', log)
             self.assertIn('val_loss', log)
             self.assertIn('time', log)
 
-    def _test_train_integration(self, logs, epochs=NUM_EPOCHS, initial_epoch=1):
+    def _test_train_integration(self, logs, epochs=None, initial_epoch=1, num_lr_schedulers=0):
+        if epochs is None:
+            epochs = self.NUM_EPOCHS
+
         self.assertTrue(os.path.isdir(self.test_checkpoints_path))
-        self.assertTrue(os.path.isfile(self.ckpt_1_path))
+        for path in self.checkpoint_paths:
+            self.assertTrue(os.path.isfile(path))
+        for path in self.no_checkpoint_paths:
+            self.assertFalse(os.path.isfile(path))
         self.assertTrue(os.path.isfile(self.ckpt_last_path))
         self.assertTrue(os.path.isfile(self.optim_ckpt_path))
         self.assertTrue(os.path.isfile(self.tsv_log_path))
         self.assertTrue(os.path.isfile(self.epoch_file_path))
         self.assertTrue(os.path.isfile(self.time_metric_plot_png_file_path))
         self.assertTrue(os.path.isfile(self.time_metric_plot_pdf_file_path))
         self.assertTrue(os.path.isfile(self.loss_metric_plot_png_file_path))
         self.assertTrue(os.path.isfile(self.loss_metric_plot_pdf_file_path))
         self.assertFalse(os.path.isfile(self.tsv_test_log_path))
+        if num_lr_schedulers >= 1:
+            self.assertTrue(os.path.isfile(self.first_lr_scheduler_ckpt_path))
+        else:
+            self.assertFalse(os.path.isfile(self.first_lr_scheduler_ckpt_path))
+        if num_lr_schedulers >= 2:
+            self.assertTrue(os.path.isfile(self.second_lr_scheduler_ckpt_path))
+        else:
+            self.assertFalse(os.path.isfile(self.second_lr_scheduler_ckpt_path))
 
         self.assertEqual(len(logs), epochs - initial_epoch + 1)
         for i, log in enumerate(logs, initial_epoch):
             self.assertIn('epoch', log)
             self.assertEqual(log['epoch'], i)
             self.assertIn('loss', log)
             self.assertIn('val_loss', log)
             self.assertIn('time', log)
 
         with open(self.epoch_file_path, 'r', encoding='utf-8') as fd:
             epoch = int(fd.read())
         self.assertEqual(epoch, epochs)
 
+        actual_stats = pd.read_csv(self.tsv_log_path, sep='\t')
+        pd.testing.assert_frame_equal(self.test_experiment.get_stats(), actual_stats)
+
+        actual_logs = actual_stats.drop(columns=['lr'])
+        actual_logs = actual_logs[actual_logs['epoch'] >= initial_epoch].reset_index(drop=True)
+        expected_logs = pd.DataFrame(logs)
+        pd.testing.assert_frame_equal(expected_logs, actual_logs)
+
+    def test_get_saved_epochs(self):
+        train_generator = SomeDataGeneratorWithLen(32, 10, 0)
+        valid_generator = SomeDataGeneratorWithLen(32, 10, 0)
+        self.test_experiment.train(
+            train_generator, valid_generator, epochs=self.NUM_EPOCHS, callbacks=[self.metric_callback]
+        )
+        actual_saved_epochs = self.test_experiment.get_saved_epochs()
+
+        self.assertEqual(self.CHECKPOINT_EPOCHS, actual_saved_epochs['epoch'].tolist())
+
+        stats = self.test_experiment.get_stats()
+        expected_saved_epochs = stats[stats['epoch'].isin(self.CHECKPOINT_EPOCHS)]
+        pd.testing.assert_frame_equal(expected_saved_epochs, actual_saved_epochs)
+
     def test_integration_test(self):
         self._train_expt()
         generator = SomeDataGeneratorWithLen(32, 10, 0)
         logs = self.test_experiment.test(generator)
         self._test_test_integration(logs)
 
     def test_integration_test_dataset(self):
@@ -142,175 +282,69 @@
 
     def test_integration_test_data(self):
         self._train_expt()
         x, y = torch.rand(32 * 10, 1), torch.rand(32 * 10, 1)
         log = self.test_experiment.test_data(x, y)
         self._test_test_integration(log)
 
-    def _train_expt(self):
-        train_generator = SomeDataGeneratorWithLen(32, 10, 0)
-        valid_generator = SomeDataGeneratorWithLen(32, 10, 0)
-        self.test_experiment.train(train_generator, valid_generator, epochs=ModelBundleTest.NUM_EPOCHS)
+    def test_test_with_return_dict_format_to_False_raises_exception(self):
+        self._train_expt()
+        generator = SomeDataGeneratorWithLen(32, 10, 0)
+        with self.assertRaises(ValueError):
+            self.test_experiment.test(generator, return_dict_format=False)
 
     def _test_test_integration(self, log):
         self.assertTrue(os.path.isfile(self.tsv_test_log_path))
 
         self.assertIn('test_loss', log)
         self.assertIn('time', log)
 
-    def setUpTwoModelBundle(self, a_params=None, b_params=None):
-        self.test_checkpoints_path_b = os.path.join(self.temp_dir_obj.name, 'expt_b')
-        self.test_checkpoints_path_a = os.path.join(self.temp_dir_obj.name, 'expt_a')
-
-        if a_params is None:
-            a_params = {}
-
-        self.test_experiment_a = ModelBundle.from_network(self.test_checkpoints_path_a, nn.Linear(1, 1), **a_params)
-
-        if b_params is None:
-            b_params = {}
-
-        self.test_experiment_b = ModelBundle.from_network(self.test_checkpoints_path_b, nn.Linear(1, 1), **b_params)
-
-    def test_givenAIsSmallerThanBMinMonitoring_thenReturnTrue(self):
-        self.setUpTwoModelBundle()
-
-        with patch.object(ModelBundle, "load_checkpoint") as load_checkpoint_mock:
-            mocked_stats = MagicMock(spec=DataFrame)
-            series_mock = MagicMock(spec=Series)
-            series_mock.item.side_effect = [[1], [2]]  # The monitored metric values
-            mocked_stats.__getitem__.return_value = series_mock
-            load_checkpoint_mock.return_value = mocked_stats
-
-            self.assertTrue(self.test_experiment_a.is_better_than(self.test_experiment_b))
-
-    def test_givenAIsGreaterThanBMinMonitoring_thenReturnFalse(self):
-        self.setUpTwoModelBundle()
-
-        with patch.object(ModelBundle, "load_checkpoint") as load_checkpoint_mock:
-            mocked_stats = MagicMock(spec=DataFrame)
-            series_mock = MagicMock(spec=Series)
-            series_mock.item.side_effect = [[2], [1]]  # The monitored metric values
-            mocked_stats.__getitem__.return_value = series_mock
-            load_checkpoint_mock.return_value = mocked_stats
-
-            self.assertFalse(self.test_experiment_a.is_better_than(self.test_experiment_b))
-
-    def test_givenAIsSmallerThanBMaxMonitoring_thenReturnFalse(self):
-        # We need to specify the metric for the mode to be properly set to "max"
-        params = {"monitor_mode": "max", "monitor_metric": "loss"}
-        self.setUpTwoModelBundle(a_params=params, b_params=params)
-
-        with patch.object(ModelBundle, "load_checkpoint") as load_checkpoint_mock:
-            mocked_stats = MagicMock(spec=DataFrame)
-            series_mock = MagicMock(spec=Series)
-            series_mock.item.side_effect = [[1], [2]]  # The monitored metric values
-            mocked_stats.__getitem__.return_value = series_mock
-            load_checkpoint_mock.return_value = mocked_stats
-
-            self.assertFalse(self.test_experiment_a.is_better_than(self.test_experiment_b))
-
-    def test_givenAIsGreaterThanBMaxMonitoring_thenReturnTrue(self):
-        # We need to specify the metric for the mode to be properly set to "max"
-        params = {"monitor_mode": "max", "monitor_metric": "loss"}
-        self.setUpTwoModelBundle(a_params=params, b_params=params)
-
-        with patch.object(ModelBundle, "load_checkpoint") as load_checkpoint_mock:
-            mocked_stats = MagicMock(spec=DataFrame)
-            series_mock = MagicMock(spec=Series)
-            series_mock.item.side_effect = [[2], [1]]  # The monitored metric values
-            mocked_stats.__getitem__.return_value = series_mock
-            load_checkpoint_mock.return_value = mocked_stats
-
-            self.assertTrue(self.test_experiment_a.is_better_than(self.test_experiment_b))
-
-    def test_givenSomeModelBundleNotLogging_thenRaiseValueError(self):
-        params_a = {"logging": False}
-        params_b = {"logging": True}
-        self.setUpTwoModelBundle(a_params=params_a, b_params=params_b)
-        with self.assertRaises(ValueError):
-            self.test_experiment_a.is_better_than(self.test_experiment_b)
-
-        params_a = {"logging": True}
-        params_b = {"logging": False}
-        self.setUpTwoModelBundle(a_params=params_a, b_params=params_b)
-        with self.assertRaises(ValueError):
-            self.test_experiment_a.is_better_than(self.test_experiment_b)
+    def test_infer(self):
+        self._train_expt()
+        num_steps = 10
+        generator = SomeDataGeneratorWithLen(32, 10, 0)
+        generator = (x for x, _ in generator)
+        pred_y = self.test_experiment.infer(generator, steps=num_steps)
+        self.assertEqual(type(pred_y), np.ndarray)
+        self.assertEqual(pred_y.shape, (320, 1))
 
-        params = {"logging": False}
-        self.setUpTwoModelBundle(a_params=params, b_params=params)
-        with self.assertRaises(ValueError):
-            self.test_experiment_a.is_better_than(self.test_experiment_b)
+    def test_infer_dataset(self):
+        self._train_expt()
+        dataset = TensorDataset(torch.rand(32 * 10, 1))
+        pred_y = self.test_experiment.infer_dataset(dataset)
+        self.assertEqual(type(pred_y), np.ndarray)
+        self.assertEqual(pred_y.shape, (320, 1))
 
-    def test_givenDifferentMonitorMetric_thenRaiseValueError(self):
-        params_a = {"monitor_metric": "loss"}
-        params_b = {"monitor_metric": "acc"}
-        self.setUpTwoModelBundle(a_params=params_a, b_params=params_b)
-        with self.assertRaises(ValueError):
-            self.test_experiment_a.is_better_than(self.test_experiment_b)
+    def test_infer_data(self):
+        self._train_expt()
+        x = torch.rand(32 * 10, 1)
+        pred_y = self.test_experiment.infer_data(x)
+        self.assertEqual(type(pred_y), np.ndarray)
+        self.assertEqual(pred_y.shape, (320, 1))
 
-    def test_givenDifferentMonitorMode_thenRaiseValueError(self):
-        # We need to specify the metric for the mode to be properly set to "max"
-        params_a = {"monitor_mode": "max", "monitor_metric": "loss"}
-        params_b = {"monitor_mode": "min"}
-        self.setUpTwoModelBundle(a_params=params_a, b_params=params_b)
+    def test_infer_data_without_training(self):
+        x = torch.rand(32 * 10, 1)
         with self.assertRaises(ValueError):
-            self.test_experiment_a.is_better_than(self.test_experiment_b)
-
-
-class ModelBundleCheckpointLoadingTest(TestCase):
-    def setUp(self):
-        self.temp_dir_obj = TemporaryDirectory()
-        self.test_checkpoints_path = self.temp_dir_obj.name
-        self.ckpt_1_path = os.path.join(self.test_checkpoints_path, "checkpoint_epoch_1.ckpt")
-        self.ckpt_last_path = os.path.join(self.test_checkpoints_path, "checkpoint.ckpt")
-
-        expt = ModelBundle.from_network(
-            self.test_checkpoints_path,
-            nn.Linear(1, 1),
-            optimizer='sgd',
-            loss_function='mse',
-            monitor_metric="loss",
-            monitor_mode="min",
-        )
-        train_generator = SomeDataGeneratorWithLen(2, 32, 0)
-        expt.train(train_generator, epochs=1)
-
-        self.test_experiment = ModelBundle.from_network(
-            self.test_checkpoints_path,
-            nn.Linear(1, 1),
-            optimizer='sgd',
-            loss_function='mse',
-            monitor_metric="loss",
-            monitor_mode="min",
-        )
-
-    def tearDown(self):
-        self.temp_dir_obj.cleanup()
+            self.test_experiment.infer_data(x)
 
-    def test_load_checkpoint_with_int(self):
-        self.test_experiment.load_checkpoint(1)
-
-        self.assertEqual(
-            self.test_experiment.model.network.state_dict(), torch.load(self.ckpt_1_path, map_location="cpu")
-        )
-
-    def test_load_checkpoint_best(self):
-        self.test_experiment.load_checkpoint("best")
-
-        self.assertEqual(
-            self.test_experiment.model.network.state_dict(), torch.load(self.ckpt_1_path, map_location="cpu")
+    def _train_expt(self):
+        train_generator = SomeDataGeneratorWithLen(32, 10, 0)
+        valid_generator = SomeDataGeneratorWithLen(32, 10, 0)
+        self.test_experiment.train(
+            train_generator, valid_generator, epochs=self.NUM_EPOCHS, callbacks=[self.metric_callback]
         )
 
-    def test_load_checkpoint_last(self):
-        self.test_experiment.load_checkpoint("last")
 
-        self.assertEqual(
-            self.test_experiment.model.network.state_dict(), torch.load(self.ckpt_last_path, map_location="cpu")
-        )
+class MonitorMinExperimentTest(BaseExperimentTest, TestCase):
+    NUM_EPOCHS = 5
+    METRIC_VALUES = [9, 3, 6, 2, 3]
+    CHECKPOINT_EPOCHS = [1, 2, 4]
+    NO_CHECKPOINT_EPOCHS = [3, 5]
+    MONITOR_MODE = "min"
 
-    def test_load_checkpoint_path_state_dict(self):
-        cpkt_path = os.path.join(self.test_checkpoints_path, "test_model_weights_state_dict.p")
-        torch.save(torch.load(self.ckpt_1_path, map_location="cpu"), cpkt_path)  # change the ckpt path
-        self.test_experiment.load_checkpoint(cpkt_path)
 
-        self.assertEqual(self.test_experiment.model.network.state_dict(), torch.load(cpkt_path, map_location="cpu"))
+class MonitorMaxExperimentTest(BaseExperimentTest, TestCase):
+    NUM_EPOCHS = 5
+    METRIC_VALUES = [4, 3, 6, 2, 7]
+    CHECKPOINT_EPOCHS = [1, 3, 5]
+    NO_CHECKPOINT_EPOCHS = [2, 4]
+    MONITOR_MODE = "max"
```

### Comparing `Poutyne-1.8/tests/framework/metrics/test_batch_metrics.py` & `Poutyne-1.9/tests/framework/metrics/test_batch_metrics.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 from unittest import TestCase, skipIf
 
 import numpy as np
 import torch
 
 from poutyne import Accuracy, BinaryAccuracy, TopKAccuracy, acc, bin_acc, topk
```

### Comparing `Poutyne-1.8/tests/framework/metrics/test_fscores.py` & `Poutyne-1.9/tests/framework/metrics/test_fscores.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,29 @@
 """
-The source code of this file was copied from the AllenNLP project, and has been modified.
+The source code of this file was copied from the AllenNLP project, and has been modified. All modifications
+made from the original source code are under the LGPLv3 license.
+
+
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information on the Poutyne and AllenNLP repository.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+
 
 Copyright 2019 AllenNLP
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
@@ -17,16 +37,17 @@
 """
 
 # pylint: disable=protected-access
 from unittest import TestCase
 
 import numpy
 import torch
+import torch.nn as nn
 
-from poutyne import FBeta
+from poutyne import FBeta, Model
 
 
 class FBetaTest(TestCase):
     def setUp(self):
         # [0, 1, 1, 1, 3, 1]
         self.predictions = torch.Tensor(
             [
@@ -232,7 +253,95 @@
         self.assertEqual('f', fbeta.__name__)
         fbeta = FBeta(average='macro', names=['f', "p", "r"])
         self.assertEqual(["f", "p", "r"], fbeta.__name__)
         fbeta = FBeta(average='binary')
         self.assertEqual(['fscore_binary_1', 'precision_binary_1', 'recall_binary_1'], fbeta.__name__)
         fbeta = FBeta(average='binary', pos_label=0)
         self.assertEqual(['fscore_binary_0', 'precision_binary_0', 'recall_binary_0'], fbeta.__name__)
+
+    def test_predefined_names(self):
+        epoch_metrics = [
+            'f1',
+            'precision',
+            'recall',
+            'binaryf1',
+            'binf1',
+            'binaryprecision',
+            'binprecision',
+            'binaryrecall',
+            'binrecall',
+        ]
+        fmetric = ['fscore', 'precision', 'recall', 'fscore', 'fscore', 'precision', 'precision', 'recall', 'recall']
+        average = ['macro', 'macro', 'macro', 'binary', 'binary', 'binary', 'binary', 'binary', 'binary']
+        names = [
+            'fscore_macro',
+            'precision_macro',
+            'recall_macro',
+            'bin_fscore1',
+            'bin_fscore2',
+            'bin_precision1',
+            'bin_precision2',
+            'bin_recall1',
+            'bin_recall2',
+        ]
+        model = Model(nn.Linear(10, 2), 'sgd', 'cross_entropy', epoch_metrics=epoch_metrics)
+        actual_fmetric = [epoch_metric._metric for epoch_metric in model.epoch_metrics]
+        actual_average = [epoch_metric._average for epoch_metric in model.epoch_metrics]
+        self.assertEqual(fmetric, actual_fmetric)
+        self.assertEqual(average, actual_average)
+        self.assertEqual(names, model.epoch_metrics_names)
+
+
+class FBetaBinaryTest(TestCase):
+    def setUp(self):
+        # [0, 1, 1, 1, 0, 1]
+        self.predictions = torch.Tensor([[0.35, 0.25], [0.1, 0.6], [0.1, 0.6], [0.1, 0.5], [0.2, 0.1], [0.1, 0.6]])
+        self.targets = torch.Tensor([0, 0, 1, 0, 1, 0])
+
+        # detailed target state
+        self.pred_sum = [2, 4]
+        self.true_sum = [4, 2]
+        self.true_positive_sum = [1, 1]
+        self.true_negative_sum = [1, 1]
+        self.total_sum = [6, 6]
+
+        desired_precision = 0.25
+        desired_recall = 0.5
+        desired_fscore = (
+            (2 * desired_precision * desired_recall) / (desired_precision + desired_recall)
+            if desired_precision + desired_recall != 0.0
+            else 0.0
+        )
+        self.output = [desired_fscore, desired_precision, desired_recall]
+
+    def test_fbeta_binary(self):
+        fbeta = FBeta(average='binary')
+        fbeta(self.predictions, self.targets)
+
+        # check state
+        numpy.testing.assert_almost_equal(fbeta._pred_sum.tolist(), self.pred_sum)
+        numpy.testing.assert_almost_equal(fbeta._true_sum.tolist(), self.true_sum)
+        numpy.testing.assert_almost_equal(fbeta._true_positive_sum.tolist(), self.true_positive_sum)
+        numpy.testing.assert_almost_equal(fbeta._total_sum.tolist(), self.total_sum)
+        numpy.testing.assert_almost_equal(fbeta.get_metric(), self.output)
+
+    def test_fbeta_binary_one_dim_pred(self):
+        fbeta = FBeta(average='binary')
+        fbeta(self.predictions[:, 1:] - self.predictions[:, 0:1], self.targets)
+
+        # check state
+        numpy.testing.assert_almost_equal(fbeta._pred_sum.tolist(), self.pred_sum)
+        numpy.testing.assert_almost_equal(fbeta._true_sum.tolist(), self.true_sum)
+        numpy.testing.assert_almost_equal(fbeta._true_positive_sum.tolist(), self.true_positive_sum)
+        numpy.testing.assert_almost_equal(fbeta._total_sum.tolist(), self.total_sum)
+        numpy.testing.assert_almost_equal(fbeta.get_metric(), self.output)
+
+    def test_fbeta_binary_zero_dim_pred(self):
+        fbeta = FBeta(average='binary')
+        fbeta(self.predictions[:, 1] - self.predictions[:, 0], self.targets)
+
+        # check state
+        numpy.testing.assert_almost_equal(fbeta._pred_sum.tolist(), self.pred_sum)
+        numpy.testing.assert_almost_equal(fbeta._true_sum.tolist(), self.true_sum)
+        numpy.testing.assert_almost_equal(fbeta._true_positive_sum.tolist(), self.true_positive_sum)
+        numpy.testing.assert_almost_equal(fbeta._total_sum.tolist(), self.total_sum)
+        numpy.testing.assert_almost_equal(fbeta.get_metric(), self.output)
```

### Comparing `Poutyne-1.8/tests/framework/metrics/test_metrics_model_integration.py` & `Poutyne-1.9/tests/framework/metrics/test_metrics_model_integration.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,56 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 # pylint: disable=unused-argument
 
 # Bug with PyTorch source code makes torch.tensor as not callable for pylint.
 # pylint: disable=not-callable
 import os
 import unittest
 from unittest import skipIf
 from unittest.mock import ANY
 import numpy as np
 import torch
 import torch.nn as nn
+import torchmetrics
+
+from poutyne import Model, EpochMetric, rename_doubles, register_epoch_metric_class, unregister_epoch_metric
 
-from poutyne import Model, EpochMetric, rename_doubles
+
+class MyConstTorchMetric(torchmetrics.Metric):
+    def __init__(self, value=0):
+        super().__init__()
+        self.value = value
+
+    def update(self, preds: torch.Tensor, target: torch.Tensor):
+        pass
+
+    def compute(self):
+        return self.value
 
 
 class ConstEpochMetric(EpochMetric):
-    def __init__(self, value):
+    def __init__(self, value=0):
         super().__init__()
         self.value = value
 
     def forward(self, y_pred, y_true):
         pass
 
     def get_metric(self):
@@ -47,14 +79,15 @@
     def const_batch_metric(y_pred, y_true):
         return value
 
     return const_batch_metric
 
 
 class MetricsModelIntegrationTest(unittest.TestCase):
+    # pylint: disable=too-many-public-methods
     epochs = 2
     steps_per_epoch = 3
     batch_size = 10
 
     cuda_device = int(os.environ.get('CUDA_DEVICE', 0))
 
     def setUp(self):
@@ -208,14 +241,75 @@
         )
         self._test_history(model, self.metric_names, self.metric_values)
 
     def test_batch_metrics_with_str_str_tuple(self):
         model = Model(self.pytorch_network, self.optimizer, self.loss_function, batch_metrics=['mse', ('mse2', 'mse')])
         self._test_history(model, ['mse', 'mse2'], [ANY, ANY])
 
+    def test_epoch_metrics_registered_with_unique_name(self):
+        names = register_epoch_metric_class(SomeMetricName, names=['some1', 'some2'], unique_name='unique_some')
+        model = Model(
+            self.pytorch_network, self.optimizer, self.loss_function, epoch_metrics=['some2', ('something', 'some1')]
+        )
+        self._test_history(model, ['unique_some', 'something'], [0.0, 0.0])
+        unregister_epoch_metric(names)
+
+    def test_torchmetrics_handling(self):
+        expected_names = ['r2_score', 'spearman_corr_coef']
+        model = Model(
+            self.pytorch_network,
+            self.optimizer,
+            self.loss_function,
+            torch_metrics=[torchmetrics.R2Score(), torchmetrics.SpearmanCorrCoef()],
+        )
+        self._test_history(model, expected_names, [ANY, ANY])
+
+    def test_repeated_torch_metrics_handling(self):
+        expected_names = ['my_const_torch_metric1', 'my_const_torch_metric2']
+        model = Model(
+            self.pytorch_network,
+            self.optimizer,
+            self.loss_function,
+            torch_metrics=[MyConstTorchMetric(1), MyConstTorchMetric(2)],
+        )
+        self._test_history(model, expected_names, [1, 2])
+
+    def test_repeated_torch_metrics_handling_with_different_names(self):
+        expected_names = ['metric1', 'metric2']
+        model = Model(
+            self.pytorch_network,
+            self.optimizer,
+            self.loss_function,
+            torch_metrics=[('metric1', MyConstTorchMetric(1)), ('metric2', MyConstTorchMetric(2))],
+        )
+        self._test_history(model, expected_names, [1, 2])
+
+    def test_use_torch_metrics_as_epoch_metrics(self):
+        expected_names = ['metric1', 'metric2']
+        model = Model(
+            self.pytorch_network,
+            self.optimizer,
+            self.loss_function,
+            epoch_metrics=[('metric1', MyConstTorchMetric(1)), ('metric2', MyConstTorchMetric(2))],
+        )
+        self._test_history(model, expected_names, [1, 2])
+
+    @skipIf(not torch.cuda.is_available(), "no gpu available")
+    def test_torch_metrics_on_gpu(self):
+        with torch.cuda.device(MetricsModelIntegrationTest.cuda_device):
+            expected_names = ['r2_score', 'spearman_corr_coef']
+            model = Model(
+                self.pytorch_network,
+                self.optimizer,
+                self.loss_function,
+                torch_metrics=[torchmetrics.R2Score(), torchmetrics.SpearmanCorrCoef()],
+            )
+            model.cuda()
+            self._test_history(model, expected_names, [ANY, ANY])
+
     def _test_history(self, model, names, values):
         history = model.fit(
             self.train_x,
             self.train_y,
             validation_data=(self.valid_x, self.valid_y),
             batch_size=MetricsModelIntegrationTest.batch_size,
             epochs=MetricsModelIntegrationTest.epochs,
@@ -223,70 +317,103 @@
         for logs in history:
             for name, value in zip(names, values):
                 self.assertIn(name, logs)
                 self.assertEqual(value, logs[name])
                 self.assertIn('val_' + name, logs)
                 self.assertEqual(value, logs['val_' + name])
 
+    def test_epoch_metrics_with_str_str_tuple(self):
+        dataset_size = MetricsModelIntegrationTest.batch_size * MetricsModelIntegrationTest.steps_per_epoch
+        torch.manual_seed(42)
+        train_x = torch.rand(dataset_size, 1)
+        train_y = torch.randint(10, (dataset_size,))
+        valid_x = torch.rand(dataset_size, 1)
+        valid_y = torch.randint(10, (dataset_size,))
+
+        model = Model(nn.Linear(1, 10), 'sgd', 'cross_entropy', epoch_metrics=['f1', ('f1_2', 'f1')])
+        names = ['fscore_macro', 'f1_2']
+        history = model.fit(
+            train_x,
+            train_y,
+            validation_data=(valid_x, valid_y),
+            batch_size=MetricsModelIntegrationTest.batch_size,
+            epochs=MetricsModelIntegrationTest.epochs,
+        )
+        for logs in history:
+            for name in names:
+                self.assertIn(name, logs)
+                self.assertEqual(ANY, logs[name])
+                self.assertIn('val_' + name, logs)
+                self.assertEqual(ANY, logs['val_' + name])
+
 
 class MetricsRenamingTest(unittest.TestCase):
     def test_batch_metrics(self):
-        actual = rename_doubles(['a', 'a'], [])
-        expected = ['a1', 'a2'], []
+        actual = rename_doubles(['a', 'a'], [], [])
+        expected = ['a1', 'a2'], [], []
         self.assertEqual(expected, actual)
 
-        actual = rename_doubles(['a', 'b', 'a', 'a', 'c', 'd'], [])
-        expected = ['a1', 'b', 'a2', 'a3', 'c', 'd'], []
+        actual = rename_doubles(['a', 'b', 'a', 'a', 'c', 'd'], [], [])
+        expected = ['a1', 'b', 'a2', 'a3', 'c', 'd'], [], []
         self.assertEqual(expected, actual)
 
     def test_epoch_metrics(self):
-        actual = rename_doubles([], ['a', 'a'])
-        expected = [], ['a1', 'a2']
+        actual = rename_doubles([], ['a', 'a'], [])
+        expected = [], ['a1', 'a2'], []
+        self.assertEqual(expected, actual)
+
+        actual = rename_doubles([], ['a', 'b', 'a', 'a', 'c', 'd'], [])
+        expected = [], ['a1', 'b', 'a2', 'a3', 'c', 'd'], []
+        self.assertEqual(expected, actual)
+
+    def test_torch_metrics(self):
+        actual = rename_doubles([], [], ['a', 'a'])
+        expected = [], [], ['a1', 'a2']
         self.assertEqual(expected, actual)
 
-        actual = rename_doubles([], ['a', 'b', 'a', 'a', 'c', 'd'])
-        expected = [], ['a1', 'b', 'a2', 'a3', 'c', 'd']
+        actual = rename_doubles([], [], ['a', 'b', 'a', 'a', 'c', 'd'])
+        expected = [], [], ['a1', 'b', 'a2', 'a3', 'c', 'd']
         self.assertEqual(expected, actual)
 
-    def test_batch_epoch_metrics(self):
-        actual = rename_doubles(['a', 'b', 'c'], ['d', 'a', 'e', 'a'])
-        expected = ['a1', 'b', 'c'], ['d', 'a2', 'e', 'a3']
+    def test_batch_epoch_torch_metrics(self):
+        actual = rename_doubles(['a', 'b', 'c'], ['d', 'a', 'e', 'a'], ['f', 'a', 'g'])
+        expected = ['a1', 'b', 'c'], ['d', 'a2', 'e', 'a3'], ['f', 'a4', 'g']
         self.assertEqual(expected, actual)
 
-        actual = rename_doubles(['a', 'b', 'c', 'b'], ['d', 'a', 'e', 'a', 'e'])
-        expected = ['a1', 'b1', 'c', 'b2'], ['d', 'a2', 'e1', 'a3', 'e2']
+        actual = rename_doubles(['a', 'b', 'c', 'b'], ['d', 'a', 'e', 'a', 'e'], ['f', 'a'])
+        expected = ['a1', 'b1', 'c', 'b2'], ['d', 'a2', 'e1', 'a3', 'e2'], ['f', 'a4']
         self.assertEqual(expected, actual)
 
-        actual = rename_doubles(['a', 'b', 'c'], ['d', 'a', 'e', 'a', 'e'])
-        expected = ['a1', 'b', 'c'], ['d', 'a2', 'e1', 'a3', 'e2']
+        actual = rename_doubles(['a', 'b', 'c'], ['d', 'a', 'e', 'a', 'e'], ['f', 'a'])
+        expected = ['a1', 'b', 'c'], ['d', 'a2', 'e1', 'a3', 'e2'], ['f', 'a4']
         self.assertEqual(expected, actual)
 
     def test_nested_batch_metrics(self):
-        actual = rename_doubles([['a', 'a']], [])
-        expected = [['a1', 'a2']], []
+        actual = rename_doubles([['a', 'a']], [], [])
+        expected = [['a1', 'a2']], [], []
         self.assertEqual(expected, actual)
 
-        actual = rename_doubles([['a', 'b'], 'b'], [])
-        expected = [['a', 'b1'], 'b2'], []
+        actual = rename_doubles([['a', 'b'], 'b'], [], [])
+        expected = [['a', 'b1'], 'b2'], [], []
         self.assertEqual(expected, actual)
 
     def test_nested_epoch_metrics(self):
-        actual = rename_doubles([], [['a', 'a']])
-        expected = [], [['a1', 'a2']]
+        actual = rename_doubles([], [['a', 'a']], [])
+        expected = [], [['a1', 'a2']], []
         self.assertEqual(expected, actual)
 
-        actual = rename_doubles([], [['a', 'b'], 'b'])
-        expected = [], [['a', 'b1'], 'b2']
+        actual = rename_doubles([], [['a', 'b'], 'b'], [])
+        expected = [], [['a', 'b1'], 'b2'], []
         self.assertEqual(expected, actual)
 
     def test_nested_batch_epoch_metrics(self):
-        actual = rename_doubles([['a']], [['a']])
-        expected = [['a1']], [['a2']]
+        actual = rename_doubles([['a']], [['a']], [])
+        expected = [['a1']], [['a2']], []
         self.assertEqual(expected, actual)
 
-        actual = rename_doubles([['a', 'b']], [['c', 'a']])
-        expected = [['a1', 'b']], [['c', 'a2']]
+        actual = rename_doubles([['a', 'b']], [['c', 'a']], [])
+        expected = [['a1', 'b']], [['c', 'a2']], []
         self.assertEqual(expected, actual)
 
-        actual = rename_doubles(['a', 'b', ['b', 'a'], 'c', 'a', 'd'], ['e', ['c', 'a'], 'f', 'a'])
-        expected = ['a1', 'b1', ['b2', 'a2'], 'c1', 'a3', 'd'], ['e', ['c2', 'a4'], 'f', 'a5']
+        actual = rename_doubles(['a', 'b', ['b', 'a'], 'c', 'a', 'd'], ['e', ['c', 'a'], 'f', 'a'], [])
+        expected = ['a1', 'b1', ['b2', 'a2'], 'c1', 'a3', 'd'], ['e', ['c2', 'a4'], 'f', 'a5'], []
         self.assertEqual(expected, actual)
```

### Comparing `Poutyne-1.8/tests/framework/metrics/test_sklearn_metrics.py` & `Poutyne-1.9/tests/framework/metrics/test_sklearn_metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 from unittest import TestCase, skipIf
 from itertools import repeat
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
```

### Comparing `Poutyne-1.8/tests/framework/model/test_model.py` & `Poutyne-1.9/tests/framework/model/test_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,39 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 # pylint: disable=too-many-locals,too-many-lines
 
 import warnings
 from collections import OrderedDict
 from math import ceil
 from unittest import skipIf, main
 from unittest.mock import MagicMock, ANY
 
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
+from torch.nn.utils.rnn import PackedSequence
 from torch.utils.data import DataLoader, Dataset
 
 from poutyne import Model, warning_settings, TensorDataset
 from tests.framework.tools import (
     some_data_tensor_generator,
     SomeDataGeneratorUsingStopIteration,
     SomeDataGeneratorWithLen,
@@ -23,14 +43,15 @@
     repeat_batch_metric,
     some_metric_1_value,
     some_metric_2_value,
     repeat_batch_metric_value,
     some_constant_epoch_metric_value,
     SomeEpochMetric,
 )
+from tests.utils import populate_packed_sequence
 from .base import ModelFittingTestCase
 
 warning_settings['concatenate_returns'] = 'ignore'
 
 
 def some_ndarray_generator(batch_size):
     while True:
@@ -519,14 +540,24 @@
     def test_evaluate_with_pred(self):
         x = torch.rand(ModelTest.evaluate_dataset_len, 1)
         y = torch.rand(ModelTest.evaluate_dataset_len, 1)
         # We also test the unpacking.
         _, _, pred_y = self.model.evaluate(x, y, batch_size=ModelTest.batch_size, return_pred=True)
         self.assertEqual(pred_y.shape, (ModelTest.evaluate_dataset_len, 1))
 
+    def test_evaluate_with_pred_without_convert_to_numpy(self):
+        x = torch.rand(ModelTest.evaluate_dataset_len, 1)
+        y = torch.rand(ModelTest.evaluate_dataset_len, 1)
+        # We also test the unpacking.
+        _, _, pred_y = self.model.evaluate(
+            x, y, batch_size=ModelTest.batch_size, return_pred=True, convert_to_numpy=False
+        )
+        self.assertTrue(torch.is_tensor(pred_y))
+        self.assertEqual(pred_y.shape, (ModelTest.evaluate_dataset_len, 1))
+
     def test_evaluate_with_callback(self):
         x = torch.rand(ModelTest.evaluate_dataset_len, 1)
         y = torch.rand(ModelTest.evaluate_dataset_len, 1)
         # We also test the unpacking.
         _, _, pred_y = self.model.evaluate(
             x, y, batch_size=ModelTest.batch_size, return_pred=True, callbacks=[self.mock_callback]
         )
@@ -632,14 +663,32 @@
 
         self._test_return_dict_logs(logs)
         self.assertEqual(type(pred_y), np.ndarray)
         self.assertEqual(type(true_y), np.ndarray)
         self.assertEqual(pred_y.shape, (num_steps * ModelTest.batch_size, 1))
         self.assertEqual(true_y.shape, (num_steps * ModelTest.batch_size, 1))
 
+    def test_evaluate_generator_with_return_dict_and_pred_and_ground_truth_without_convert_to_numpy(self):
+        num_steps = 10
+        generator = some_data_tensor_generator(ModelTest.batch_size)
+        logs, pred_y, true_y = self.model.evaluate_generator(
+            generator,
+            steps=num_steps,
+            return_dict_format=True,
+            return_pred=True,
+            return_ground_truth=True,
+            convert_to_numpy=False,
+        )
+
+        self._test_return_dict_logs(logs)
+        self.assertTrue(torch.is_tensor(pred_y))
+        self.assertTrue(torch.is_tensor(true_y))
+        self.assertEqual(pred_y.shape, (num_steps * ModelTest.batch_size, 1))
+        self.assertEqual(true_y.shape, (num_steps * ModelTest.batch_size, 1))
+
     def test_evaluate_generator_with_ground_truth(self):
         num_steps = 10
         generator = some_data_tensor_generator(ModelTest.batch_size)
         loss, metrics, pred_y, true_y = self.model.evaluate_generator(
             generator, steps=num_steps, return_pred=True, return_ground_truth=True
         )
         self.assertEqual(type(loss), float)
@@ -754,25 +803,41 @@
     def test_evaluate_on_batch_with_return_dict_and_pred(self):
         x = torch.rand(ModelTest.batch_size, 1)
         y = torch.rand(ModelTest.batch_size, 1)
         logs, pred_y = self.model.evaluate_on_batch(x, y, return_dict_format=True, return_pred=True)
         self.assertEqual(set(logs.keys()), set(['loss'] + self.batch_metrics_names))
         self.assertEqual(pred_y.shape, (ModelTest.batch_size, 1))
 
+    def test_evaluate_on_batch_with_return_dict_and_pred_without_convert_to_numpy(self):
+        x = torch.rand(ModelTest.batch_size, 1)
+        y = torch.rand(ModelTest.batch_size, 1)
+        logs, pred_y = self.model.evaluate_on_batch(
+            x, y, return_dict_format=True, return_pred=True, convert_to_numpy=False
+        )
+        self.assertEqual(set(logs.keys()), set(['loss'] + self.batch_metrics_names))
+        self.assertTrue(torch.is_tensor(pred_y))
+        self.assertEqual(pred_y.shape, (ModelTest.batch_size, 1))
+
     def test_predict(self):
         x = torch.rand(ModelTest.evaluate_dataset_len, 1)
         pred_y = self.model.predict(x, batch_size=ModelTest.batch_size)
         self.assertEqual(pred_y.shape, (ModelTest.evaluate_dataset_len, 1))
 
     def test_predict_with_np_array(self):
         x = np.random.rand(ModelTest.evaluate_dataset_len, 1).astype(np.float32)
         pred_y = self.model.predict(x, batch_size=ModelTest.batch_size)
         self.assertEqual(type(pred_y), np.ndarray)
         self.assertEqual(pred_y.shape, (ModelTest.evaluate_dataset_len, 1))
 
+    def test_predict_without_convert_to_numpy(self):
+        x = torch.rand(ModelTest.evaluate_dataset_len, 1)
+        pred_y = self.model.predict(x, batch_size=ModelTest.batch_size, convert_to_numpy=False)
+        self.assertTrue(torch.is_tensor(pred_y))
+        self.assertEqual(pred_y.shape, (ModelTest.evaluate_dataset_len, 1))
+
     def test_predict_data_loader(self):
         x = torch.rand(ModelTest.evaluate_dataset_len, 1)
         generator = DataLoader(x, ModelTest.batch_size)
         pred_y = self.model.predict_generator(generator)
         self.assertEqual(type(pred_y), np.ndarray)
         self.assertEqual(pred_y.shape, (ModelTest.evaluate_dataset_len, 1))
 
@@ -807,14 +872,26 @@
         pred_y, true_y = self.model.predict_generator(generator, steps=num_steps, return_ground_truth=True)
 
         self.assertEqual(type(pred_y), np.ndarray)
         self.assertEqual(type(true_y), np.ndarray)
         self.assertEqual(pred_y.shape, (num_steps * ModelTest.batch_size, 1))
         self.assertEqual(true_y.shape, (num_steps * ModelTest.batch_size, 1))
 
+    def test_predict_generator_with_ground_truth_tensor_without_convert_to_numpy(self):
+        num_steps = 10
+        generator = some_data_tensor_generator(ModelTest.batch_size)
+        pred_y, true_y = self.model.predict_generator(
+            generator, steps=num_steps, return_ground_truth=True, convert_to_numpy=False
+        )
+
+        self.assertTrue(torch.is_tensor(pred_y))
+        self.assertTrue(torch.is_tensor(true_y))
+        self.assertEqual(pred_y.shape, (num_steps * ModelTest.batch_size, 1))
+        self.assertEqual(true_y.shape, (num_steps * ModelTest.batch_size, 1))
+
     def test_predict_generator_with_ground_truth_and_no_concatenation(self):
         num_steps = 10
         generator = some_data_tensor_generator(ModelTest.batch_size)
         pred_y, true_y = self.model.predict_generator(
             generator, steps=num_steps, return_ground_truth=True, concatenate_returns=False
         )
 
@@ -833,14 +910,20 @@
         self.assertEqual(pred_y.shape, (ModelTest.batch_size, 1))
 
     def test_ndarray_predict_on_batch(self):
         x = np.random.rand(ModelTest.batch_size, 1).astype(np.float32)
         pred_y = self.model.predict_on_batch(x)
         self.assertEqual(pred_y.shape, (ModelTest.batch_size, 1))
 
+    def test_predict_on_batch_without_convert_to_numpy(self):
+        x = torch.rand(ModelTest.batch_size, 1)
+        pred_y = self.model.predict_on_batch(x, convert_to_numpy=False)
+        self.assertTrue(torch.is_tensor(pred_y))
+        self.assertEqual(pred_y.shape, (ModelTest.batch_size, 1))
+
     @skipIf(not torch.cuda.is_available(), "no gpu available")
     def test_cpu_cuda(self):
         train_generator = some_data_tensor_generator(ModelTest.batch_size)
         valid_generator = some_data_tensor_generator(ModelTest.batch_size)
 
         self._capture_output()
 
@@ -1014,18 +1097,14 @@
             self.pytorch_network,
             'sgd',
             'cross_entropy',
             batch_metrics=self.batch_metrics,
             epoch_metrics=self.epoch_metrics,
         )
 
-    def assertStdoutContains(self, values):
-        for value in values:
-            self.assertIn(value, self.test_out.getvalue().strip())
-
     def test_fitting_mnist(self):
         logs = self.model.fit_dataset(
             self.train_dataset,
             self.valid_dataset,
             epochs=ModelTest.epochs,
             steps_per_epoch=ModelTest.steps_per_epoch,
             validation_steps=ModelTest.steps_per_epoch,
@@ -1128,14 +1207,32 @@
 
         self.assertEqual(type(pred_y), np.ndarray)
         self.assertEqual(type(true_y), np.ndarray)
         self.assertEqual(pred_y.shape, (num_steps * ModelTest.batch_size, 10))
         self.assertEqual(true_y.shape, (num_steps * ModelTest.batch_size,))
         self._test_return_dict_logs(logs)
 
+    def test_evaluate_dataset_with_return_dict_and_pred_and_ground_truth_without_convert_to_numpy(self):
+        num_steps = 10
+        logs, pred_y, true_y = self.model.evaluate_dataset(
+            self.test_dataset,
+            batch_size=ModelTest.batch_size,
+            steps=num_steps,
+            return_dict_format=True,
+            return_pred=True,
+            return_ground_truth=True,
+            convert_to_numpy=False,
+        )
+
+        self.assertTrue(torch.is_tensor(pred_y))
+        self.assertTrue(torch.is_tensor(true_y))
+        self.assertEqual(pred_y.shape, (num_steps * ModelTest.batch_size, 10))
+        self.assertEqual(true_y.shape, (num_steps * ModelTest.batch_size,))
+        self._test_return_dict_logs(logs)
+
     def test_evaluate_dataset_with_ground_truth(self):
         num_steps = 10
         loss, metrics, pred_y, true_y = self.model.evaluate_dataset(
             self.test_dataset,
             batch_size=ModelTest.batch_size,
             steps=num_steps,
             return_pred=True,
@@ -1183,14 +1280,29 @@
         )
 
         self.assertEqual(type(pred_y), np.ndarray)
         self.assertEqual(type(true_y), np.ndarray)
         self.assertEqual(pred_y.shape, (num_steps * ModelTest.batch_size, 10))
         self.assertEqual(true_y.shape, (num_steps * ModelTest.batch_size,))
 
+    def test_predict_dataset_with_ground_truth_without_convert_to_numpy(self):
+        num_steps = 10
+        pred_y, true_y = self.model.predict_dataset(
+            self.test_dataset,
+            batch_size=ModelTest.batch_size,
+            steps=num_steps,
+            return_ground_truth=True,
+            convert_to_numpy=False,
+        )
+
+        self.assertTrue(torch.is_tensor(pred_y))
+        self.assertTrue(torch.is_tensor(true_y))
+        self.assertEqual(pred_y.shape, (num_steps * ModelTest.batch_size, 10))
+        self.assertEqual(true_y.shape, (num_steps * ModelTest.batch_size,))
+
     def test_predict_dataset_with_ground_truth_and_no_concatenation(self):
         num_steps = 10
         pred_y, true_y = self.model.predict_dataset(
             self.test_dataset,
             batch_size=ModelTest.batch_size,
             steps=num_steps,
             return_ground_truth=True,
@@ -1202,10 +1314,22 @@
             self.assertEqual(type(pred), np.ndarray)
             self.assertEqual(pred.shape, (ModelTest.batch_size, 10))
         self.assertEqual(type(true_y), list)
         for true in true_y:
             self.assertEqual(type(true), np.ndarray)
             self.assertEqual(true.shape, (ModelTest.batch_size,))
 
+    def test_preprocess_input_with_packed_sequence_return_packed_sequence_in_tuple(self):
+        x = MagicMock(spec=PackedSequence)
+
+        actual_x = self.model.preprocess_input(x)
+        self.assertTrue(isinstance(actual_x, tuple))
+
+    def test_preprocess_input_integration_with_packed_sequence(self):
+        pack_padded_sequences_vectors = populate_packed_sequence()
+
+        actual_x = self.model.preprocess_input(pack_padded_sequences_vectors)
+        self.assertTrue(isinstance(actual_x[0], PackedSequence))
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `Poutyne-1.8/tests/framework/model/test_model_progress.py` & `Poutyne-1.9/tests/framework/model/test_model_progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 from unittest import skipIf
 
 import torch
 import torch.nn as nn
 from torch.utils.data import DataLoader
 
 from poutyne import Model, TensorDataset
```

### Comparing `Poutyne-1.8/tests/framework/model/test_multi_dict_io.py` & `Poutyne-1.9/tests/framework/model/test_multi_dict_io.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 # Because nn.Module has the abstract method _forward_unimplemented
 # pylint: disable=abstract-method
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
```

### Comparing `Poutyne-1.8/tests/framework/model/test_multi_gpu.py` & `Poutyne-1.9/tests/framework/model/test_multi_gpu.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 # pylint: disable=unused-argument
 import os
 from unittest import skipIf
 
 import torch
 from torch import nn
```

### Comparing `Poutyne-1.8/tests/framework/model/test_multi_input.py` & `Poutyne-1.9/tests/framework/model/test_multi_input.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 import numpy as np
 import torch
 import torch.nn as nn
 from torch.utils.data import DataLoader
 
 from poutyne import Model, warning_settings, TensorDataset
```

### Comparing `Poutyne-1.8/tests/framework/model/test_multi_io.py` & `Poutyne-1.9/tests/framework/model/test_multi_io.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 import numpy as np
 import torch
 import torch.nn as nn
 
 from poutyne import Model, warning_settings
 
 from .base import ModelFittingTestCase, MultiIOModel
```

### Comparing `Poutyne-1.8/tests/framework/model/test_multi_output.py` & `Poutyne-1.9/tests/framework/model/test_multi_output.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 import numpy as np
 import torch
 import torch.nn as nn
 from torch.utils.data import DataLoader
 
 from poutyne import Model, warning_settings, TensorDataset
```

### Comparing `Poutyne-1.8/tests/test_plotting.py` & `Poutyne-1.9/tests/test_plotting.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,40 @@
+"""
+Copyright (c) 2022 Poutyne and all respective contributors.
+
+Each contributor holds copyright over their respective contributions. The project versioning (Git)
+records all such contribution source information.
+
+This file is part of Poutyne.
+
+Poutyne is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+Poutyne is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
+of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License along with Poutyne. If not, see
+<https://www.gnu.org/licenses/>.
+"""
+
 import os
 from io import BytesIO
 from tempfile import TemporaryDirectory
 from unittest import TestCase
+import matplotlib as mpl
 import matplotlib.pyplot as plt
 from matplotlib.figure import Figure
 from matplotlib.axes import Axes
 from PIL import Image
 
 from poutyne import plot_history, plot_metric
 
+mpl.use('Agg')
+
 
 class PlotHistoryTest(TestCase):
     HISTORY = [
         {'epoch': 1, 'time': 6.2788, 'loss': 0.3683, 'acc': 88.2645, 'val_loss': 0.0984, 'val_acc': 97.0833},
         {'epoch': 2, 'time': 6.2570, 'loss': 0.1365, 'acc': 95.9166, 'val_loss': 0.0680, 'val_acc': 97.9916},
         {'epoch': 3, 'time': 6.3314, 'loss': 0.1057, 'acc': 96.8458, 'val_loss': 0.0531, 'val_acc': 98.4916},
         {'epoch': 4, 'time': 6.2574, 'loss': 0.0874, 'acc': 97.2937, 'val_loss': 0.0521, 'val_acc': 98.4166},
```


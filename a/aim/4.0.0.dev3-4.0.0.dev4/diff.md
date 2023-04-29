# Comparing `tmp/aim-4.0.0.dev3.tar.gz` & `tmp/aim-4.0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aim-4.0.0.dev3.tar", last modified: Mon Apr 10 17:48:51 2023, max compression
+gzip compressed data, was "aim-4.0.0.dev4.tar", last modified: Sat Apr 29 15:33:52 2023, max compression
```

## Comparing `aim-4.0.0.dev3.tar` & `aim-4.0.0.dev4.tar`

### file list

```diff
@@ -1,460 +1,479 @@
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:51.002742 aim-4.0.0.dev3/
--rw-r--r--   0 github     (503) staff       (20)    11347 2022-08-06 00:13:01.000000 aim-4.0.0.dev3/LICENSE
--rw-r--r--   0 github     (503) staff       (20)      185 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/MANIFEST.in
--rw-r--r--   0 github     (503) staff       (20)    37846 2023-04-10 17:48:51.002914 aim-4.0.0.dev3/PKG-INFO
--rw-r--r--   0 github     (503) staff       (20)    37159 2023-04-06 20:09:56.000000 aim-4.0.0.dev3/README.md
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.920046 aim-4.0.0.dev3/aim/
--rw-r--r--   0 github     (503) staff       (20)       10 2023-04-10 17:48:41.000000 aim-4.0.0.dev3/aim/VERSION
--rw-r--r--   0 github     (503) staff       (20)      825 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/__about__.py
--rw-r--r--   0 github     (503) staff       (20)      377 2023-02-01 20:08:30.000000 aim-4.0.0.dev3/aim/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      183 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/__version__.py
--rw-r--r--   0 github     (503) staff       (20)      100 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/acme.py
--rw-r--r--   0 github     (503) staff       (20)       96 2022-05-06 13:59:46.000000 aim-4.0.0.dev3/aim/catboost.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.921952 aim-4.0.0.dev3/aim/cli/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1323 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/cli/cli.py
--rw-r--r--   0 github     (503) staff       (20)      166 2022-06-17 00:13:19.000000 aim-4.0.0.dev3/aim/cli/configs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.922333 aim-4.0.0.dev3/aim/cli/convert/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/convert/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2998 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/cli/convert/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.923311 aim-4.0.0.dev3/aim/cli/convert/processors/
--rw-r--r--   0 github     (503) staff       (20)      113 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/cli/convert/processors/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5914 2022-09-01 19:23:53.000000 aim-4.0.0.dev3/aim/cli/convert/processors/mlflow.py
--rw-r--r--   0 github     (503) staff       (20)    10372 2022-08-06 00:13:01.000000 aim-4.0.0.dev3/aim/cli/convert/processors/tensorboard.py
--rw-r--r--   0 github     (503) staff       (20)     6816 2023-01-04 20:08:59.000000 aim-4.0.0.dev3/aim/cli/convert/processors/wandb.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.923653 aim-4.0.0.dev3/aim/cli/init/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/init/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1592 2023-03-24 14:18:45.000000 aim-4.0.0.dev3/aim/cli/init/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.923999 aim-4.0.0.dev3/aim/cli/manager/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/manager/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3382 2022-08-11 13:58:02.000000 aim-4.0.0.dev3/aim/cli/manager/manager.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.924341 aim-4.0.0.dev3/aim/cli/reindex/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/reindex/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      736 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/cli/reindex/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.924958 aim-4.0.0.dev3/aim/cli/runs/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/runs/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     6621 2023-03-24 14:18:45.000000 aim-4.0.0.dev3/aim/cli/runs/commands.py
--rw-r--r--   0 github     (503) staff       (20)     2570 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/cli/runs/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.925329 aim-4.0.0.dev3/aim/cli/server/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/server/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3709 2023-03-24 14:18:45.000000 aim-4.0.0.dev3/aim/cli/server/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.925658 aim-4.0.0.dev3/aim/cli/storage/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-06-17 00:13:19.000000 aim-4.0.0.dev3/aim/cli/storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     7537 2023-03-24 14:18:45.000000 aim-4.0.0.dev3/aim/cli/storage/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.926011 aim-4.0.0.dev3/aim/cli/telemetry/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/cli/telemetry/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      305 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/cli/telemetry/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.926634 aim-4.0.0.dev3/aim/cli/up/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/up/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5953 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/cli/up/commands.py
--rw-r--r--   0 github     (503) staff       (20)     1446 2022-06-21 18:01:08.000000 aim-4.0.0.dev3/aim/cli/up/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.927090 aim-4.0.0.dev3/aim/cli/upgrade/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.927833 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/
--rw-r--r--   0 github     (503) staff       (20)      258 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      734 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/configs.py
--rw-r--r--   0 github     (503) staff       (20)      448 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/metric_artifact.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.928496 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      263 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/base_pb2.py
--rw-r--r--   0 github     (503) staff       (20)      267 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/metric_pb2.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.928979 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v3/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v3/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3396 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v3/base_pb2.py
--rw-r--r--   0 github     (503) staff       (20)     1919 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v3/metric_pb2.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.929408 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v4/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v4/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1111 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v4/base_pb2.py
--rw-r--r--   0 github     (503) staff       (20)      969 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v4/metric_pb2.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.930388 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/
--rw-r--r--   0 github     (503) staff       (20)        1 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1722 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/metric.py
--rw-r--r--   0 github     (503) staff       (20)     3722 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/repo.py
--rw-r--r--   0 github     (503) staff       (20)     4062 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/run.py
--rw-r--r--   0 github     (503) staff       (20)     1357 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/trace.py
--rw-r--r--   0 github     (503) staff       (20)     1211 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/utils.py
--rw-r--r--   0 github     (503) staff       (20)     6635 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/upgrade/utils.py
--rw-r--r--   0 github     (503) staff       (20)      370 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.930628 aim-4.0.0.dev3/aim/cli/version/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/version/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      149 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/cli/version/commands.py
--rw-r--r--   0 github     (503) staff       (20)     9960 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/cli/watcher_cli.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.931264 aim-4.0.0.dev3/aim/ext/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.931537 aim-4.0.0.dev3/aim/ext/cleanup/
--rw-r--r--   0 github     (503) staff       (20)     3579 2022-11-12 00:14:35.000000 aim-4.0.0.dev3/aim/ext/cleanup/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2021 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/ext/exception_resistant.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.931952 aim-4.0.0.dev3/aim/ext/notebook/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/notebook/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     7314 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/notebook/notebook.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.934341 aim-4.0.0.dev3/aim/ext/notifier/
--rw-r--r--   0 github     (503) staff       (20)      589 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      305 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/base_notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1858 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/ext/notifier/config.py
--rw-r--r--   0 github     (503) staff       (20)      361 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/config_default.json
--rw-r--r--   0 github     (503) staff       (20)       70 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/config_empty.json
--rw-r--r--   0 github     (503) staff       (20)      522 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/logging_notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1428 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1158 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/notifier_builder.py
--rw-r--r--   0 github     (503) staff       (20)      524 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/slack_notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1034 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/utils.py
--rw-r--r--   0 github     (503) staff       (20)      862 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/notifier/workplace_notifier.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.935698 aim-4.0.0.dev3/aim/ext/resource/
--rw-r--r--   0 github     (503) staff       (20)       92 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/resource/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      100 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/resource/configs.py
--rw-r--r--   0 github     (503) staff       (20)      726 2022-05-16 21:25:24.000000 aim-4.0.0.dev3/aim/ext/resource/log.py
--rw-r--r--   0 github     (503) staff       (20)     6700 2023-01-04 20:08:59.000000 aim-4.0.0.dev3/aim/ext/resource/stat.py
--rw-r--r--   0 github     (503) staff       (20)     7511 2023-01-04 20:08:59.000000 aim-4.0.0.dev3/aim/ext/resource/tracker.py
--rw-r--r--   0 github     (503) staff       (20)       56 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/resource/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.935961 aim-4.0.0.dev3/aim/ext/sshfs/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/sshfs/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     7768 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/sshfs/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.936228 aim-4.0.0.dev3/aim/ext/task_queue/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/task_queue/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2069 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/task_queue/queue.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.936951 aim-4.0.0.dev3/aim/ext/tensorboard_tracker/
--rw-r--r--   0 github     (503) staff       (20)       48 2023-01-04 20:08:59.000000 aim-4.0.0.dev3/aim/ext/tensorboard_tracker/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      919 2023-01-04 20:08:59.000000 aim-4.0.0.dev3/aim/ext/tensorboard_tracker/run.py
--rw-r--r--   0 github     (503) staff       (20)     7201 2023-01-04 20:08:59.000000 aim-4.0.0.dev3/aim/ext/tensorboard_tracker/tracker.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.940530 aim-4.0.0.dev3/aim/ext/transport/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/transport/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    13282 2023-04-06 20:09:56.000000 aim-4.0.0.dev3/aim/ext/transport/client.py
--rw-r--r--   0 github     (503) staff       (20)      563 2023-04-06 20:09:56.000000 aim-4.0.0.dev3/aim/ext/transport/config.py
--rw-r--r--   0 github     (503) staff       (20)     3298 2023-01-23 20:08:00.000000 aim-4.0.0.dev3/aim/ext/transport/handlers.py
--rw-r--r--   0 github     (503) staff       (20)     5555 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/health.py
--rw-r--r--   0 github     (503) staff       (20)     5616 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/heartbeat.py
--rw-r--r--   0 github     (503) staff       (20)     3347 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/message_utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.941787 aim-4.0.0.dev3/aim/ext/transport/proto/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      245 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/health_pb2.py
--rw-r--r--   0 github     (503) staff       (20)     3991 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/health_pb2_grpc.py
--rw-r--r--   0 github     (503) staff       (20)      259 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/remote_router_pb2.py
--rw-r--r--   0 github     (503) staff       (20)     8855 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/remote_router_pb2_grpc.py
--rw-r--r--   0 github     (503) staff       (20)      263 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/remote_tracking_pb2.py
--rw-r--r--   0 github     (503) staff       (20)     9444 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/remote_tracking_pb2_grpc.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.942697 aim-4.0.0.dev3/aim/ext/transport/proto/v3/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/v3/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     6195 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/v3/health_pb2.py
--rw-r--r--   0 github     (503) staff       (20)    25245 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/v3/remote_router_pb2.py
--rw-r--r--   0 github     (503) staff       (20)    37567 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/v3/remote_tracking_pb2.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.943550 aim-4.0.0.dev3/aim/ext/transport/proto/v4/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/v4/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1749 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/v4/health_pb2.py
--rw-r--r--   0 github     (503) staff       (20)     4280 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/v4/remote_router_pb2.py
--rw-r--r--   0 github     (503) staff       (20)     5662 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/proto/v4/remote_tracking_pb2.py
--rw-r--r--   0 github     (503) staff       (20)      428 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/ext/transport/remote_resource.py
--rw-r--r--   0 github     (503) staff       (20)     8078 2023-01-23 10:30:27.000000 aim-4.0.0.dev3/aim/ext/transport/remote_tracking.py
--rw-r--r--   0 github     (503) staff       (20)     3637 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/router.py
--rw-r--r--   0 github     (503) staff       (20)     3728 2022-11-18 00:13:03.000000 aim-4.0.0.dev3/aim/ext/transport/rpc_queue.py
--rw-r--r--   0 github     (503) staff       (20)     4609 2023-01-23 10:30:27.000000 aim-4.0.0.dev3/aim/ext/transport/server.py
--rw-r--r--   0 github     (503) staff       (20)     3419 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/ext/transport/worker.py
--rw-r--r--   0 github     (503) staff       (20)     2103 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/ext/utils.py
--rw-r--r--   0 github     (503) staff       (20)       92 2022-09-25 12:02:15.000000 aim-4.0.0.dev3/aim/fastai.py
--rw-r--r--   0 github     (503) staff       (20)      127 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/hf_dataset.py
--rw-r--r--   0 github     (503) staff       (20)      105 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/hugging_face.py
--rw-r--r--   0 github     (503) staff       (20)      103 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/keras.py
--rw-r--r--   0 github     (503) staff       (20)      103 2022-08-20 12:34:00.000000 aim-4.0.0.dev3/aim/keras_tuner.py
--rw-r--r--   0 github     (503) staff       (20)       98 2022-05-06 13:59:46.000000 aim-4.0.0.dev3/aim/lightgbm.py
--rw-r--r--   0 github     (503) staff       (20)       97 2022-10-04 00:16:28.000000 aim-4.0.0.dev3/aim/mxnet.py
--rw-r--r--   0 github     (503) staff       (20)       98 2022-11-12 00:14:35.000000 aim-4.0.0.dev3/aim/optuna.py
--rw-r--r--   0 github     (503) staff       (20)       99 2022-11-12 00:14:35.000000 aim-4.0.0.dev3/aim/paddle.py
--rw-r--r--   0 github     (503) staff       (20)       93 2023-01-31 20:08:25.000000 aim-4.0.0.dev3/aim/prophet.py
--rw-r--r--   0 github     (503) staff       (20)      115 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/pytorch.py
--rw-r--r--   0 github     (503) staff       (20)      107 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/pytorch_ignite.py
--rw-r--r--   0 github     (503) staff       (20)      113 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/pytorch_lightning.py
--rw-r--r--   0 github     (503) staff       (20)       87 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/aim/sb3.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.952455 aim-4.0.0.dev3/aim/sdk/
--rw-r--r--   0 github     (503) staff       (20)      915 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.956451 aim-4.0.0.dev3/aim/sdk/adapters/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/adapters/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2609 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/acme.py
--rw-r--r--   0 github     (503) staff       (20)     3371 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/catboost.py
--rw-r--r--   0 github     (503) staff       (20)     5510 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/fastai.py
--rw-r--r--   0 github     (503) staff       (20)     5664 2023-03-24 14:18:45.000000 aim-4.0.0.dev3/aim/sdk/adapters/hugging_face.py
--rw-r--r--   0 github     (503) staff       (20)     2579 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/keras.py
--rw-r--r--   0 github     (503) staff       (20)     1128 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/adapters/keras_mixins.py
--rw-r--r--   0 github     (503) staff       (20)     2805 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/keras_tuner.py
--rw-r--r--   0 github     (503) staff       (20)     3266 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/lightgbm.py
--rw-r--r--   0 github     (503) staff       (20)     8261 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/mxnet.py
--rw-r--r--   0 github     (503) staff       (20)     7159 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/optuna.py
--rw-r--r--   0 github     (503) staff       (20)     3495 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/paddle.py
--rw-r--r--   0 github     (503) staff       (20)     2911 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/prophet.py
--rw-r--r--   0 github     (503) staff       (20)     2458 2022-07-09 00:13:12.000000 aim-4.0.0.dev3/aim/sdk/adapters/pytorch.py
--rw-r--r--   0 github     (503) staff       (20)     9025 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/pytorch_ignite.py
--rw-r--r--   0 github     (503) staff       (20)     5837 2023-03-24 14:18:45.000000 aim-4.0.0.dev3/aim/sdk/adapters/pytorch_lightning.py
--rw-r--r--   0 github     (503) staff       (20)     4533 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/sb3.py
--rw-r--r--   0 github     (503) staff       (20)     2600 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/tensorflow.py
--rw-r--r--   0 github     (503) staff       (20)     2934 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/adapters/xgboost.py
--rw-r--r--   0 github     (503) staff       (20)     5138 2023-03-16 00:07:12.000000 aim-4.0.0.dev3/aim/sdk/base_run.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.957257 aim-4.0.0.dev3/aim/sdk/callbacks/
--rw-r--r--   0 github     (503) staff       (20)      196 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/callbacks/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1493 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/callbacks/caller.py
--rw-r--r--   0 github     (503) staff       (20)      495 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/callbacks/events.py
--rw-r--r--   0 github     (503) staff       (20)     1416 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/callbacks/helpers.py
--rw-r--r--   0 github     (503) staff       (20)      253 2022-09-26 00:13:35.000000 aim-4.0.0.dev3/aim/sdk/configs.py
--rw-r--r--   0 github     (503) staff       (20)       22 2022-11-24 20:09:30.000000 aim-4.0.0.dev3/aim/sdk/data_version.py
--rw-r--r--   0 github     (503) staff       (20)      145 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/errors.py
--rw-r--r--   0 github     (503) staff       (20)     4990 2023-01-23 20:08:00.000000 aim-4.0.0.dev3/aim/sdk/index_manager.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.958300 aim-4.0.0.dev3/aim/sdk/legacy/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/legacy/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      288 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/legacy/deprecation_warning.py
--rw-r--r--   0 github     (503) staff       (20)       94 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/legacy/flush.py
--rw-r--r--   0 github     (503) staff       (20)      185 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/legacy/init.py
--rw-r--r--   0 github     (503) staff       (20)      702 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/legacy/select.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.958782 aim-4.0.0.dev3/aim/sdk/legacy/session/
--rw-r--r--   0 github     (503) staff       (20)       67 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/legacy/session/__init__.py
--rw-r--r--   0 github     (503) staff       (20)       30 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/legacy/session/configs.py
--rw-r--r--   0 github     (503) staff       (20)     4277 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/legacy/session/session.py
--rw-r--r--   0 github     (503) staff       (20)      410 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/legacy/track.py
--rw-r--r--   0 github     (503) staff       (20)     6513 2023-02-01 20:08:30.000000 aim-4.0.0.dev3/aim/sdk/lock_manager.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.959117 aim-4.0.0.dev3/aim/sdk/logging/
--rw-r--r--   0 github     (503) staff       (20)       61 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/logging/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1863 2023-02-03 15:21:38.000000 aim-4.0.0.dev3/aim/sdk/logging/log_record.py
--rw-r--r--   0 github     (503) staff       (20)      954 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/maintenance_run.py
--rw-r--r--   0 github     (503) staff       (20)     3397 2023-03-16 00:07:12.000000 aim-4.0.0.dev3/aim/sdk/num_utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.960264 aim-4.0.0.dev3/aim/sdk/objects/
--rw-r--r--   0 github     (503) staff       (20)      214 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/objects/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3264 2022-11-11 08:24:45.000000 aim-4.0.0.dev3/aim/sdk/objects/audio.py
--rw-r--r--   0 github     (503) staff       (20)     4232 2023-01-04 20:08:59.000000 aim-4.0.0.dev3/aim/sdk/objects/distribution.py
--rw-r--r--   0 github     (503) staff       (20)     2885 2023-01-04 20:08:59.000000 aim-4.0.0.dev3/aim/sdk/objects/figure.py
--rw-r--r--   0 github     (503) staff       (20)     9914 2023-03-03 20:09:01.000000 aim-4.0.0.dev3/aim/sdk/objects/image.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.960591 aim-4.0.0.dev3/aim/sdk/objects/io/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/objects/io/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    21094 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/objects/io/wavfile.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.961665 aim-4.0.0.dev3/aim/sdk/objects/plugins/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/objects/plugins/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1983 2023-01-23 20:08:00.000000 aim-4.0.0.dev3/aim/sdk/objects/plugins/dvc_metadata.py
--rw-r--r--   0 github     (503) staff       (20)     3648 2023-02-02 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/objects/plugins/hf_datasets_metadata.py
--rw-r--r--   0 github     (503) staff       (20)     1272 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/objects/plugins/hub_dataset.py
--rw-r--r--   0 github     (503) staff       (20)      694 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/objects/text.py
--rw-r--r--   0 github     (503) staff       (20)     6048 2022-09-01 19:23:53.000000 aim-4.0.0.dev3/aim/sdk/query_utils.py
--rw-r--r--   0 github     (503) staff       (20)     1050 2023-01-23 10:30:27.000000 aim-4.0.0.dev3/aim/sdk/remote_repo_proxy.py
--rw-r--r--   0 github     (503) staff       (20)     2171 2023-01-23 10:30:27.000000 aim-4.0.0.dev3/aim/sdk/remote_run_reporter.py
--rw-r--r--   0 github     (503) staff       (20)    34519 2023-03-03 20:09:01.000000 aim-4.0.0.dev3/aim/sdk/repo.py
--rw-r--r--   0 github     (503) staff       (20)     1022 2023-03-16 00:07:12.000000 aim-4.0.0.dev3/aim/sdk/repo_utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.962310 aim-4.0.0.dev3/aim/sdk/reporter/
--rw-r--r--   0 github     (503) staff       (20)    31012 2023-01-23 20:08:00.000000 aim-4.0.0.dev3/aim/sdk/reporter/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1832 2023-01-23 10:30:27.000000 aim-4.0.0.dev3/aim/sdk/reporter/file_manager.py
--rw-r--r--   0 github     (503) staff       (20)    30774 2023-03-16 00:07:12.000000 aim-4.0.0.dev3/aim/sdk/run.py
--rw-r--r--   0 github     (503) staff       (20)    13171 2023-02-03 15:21:38.000000 aim-4.0.0.dev3/aim/sdk/run_status_watcher.py
--rw-r--r--   0 github     (503) staff       (20)    12970 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/sequence.py
--rw-r--r--   0 github     (503) staff       (20)     9944 2022-07-21 10:42:47.000000 aim-4.0.0.dev3/aim/sdk/sequence_collection.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.963838 aim-4.0.0.dev3/aim/sdk/sequences/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/sequences/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      458 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/sequences/audio_sequence.py
--rw-r--r--   0 github     (503) staff       (20)      408 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/sequences/distribution_sequence.py
--rw-r--r--   0 github     (503) staff       (20)      452 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/sequences/figure_sequence.py
--rw-r--r--   0 github     (503) staff       (20)      482 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/sequences/image_sequence.py
--rw-r--r--   0 github     (503) staff       (20)     3936 2022-07-09 00:13:12.000000 aim-4.0.0.dev3/aim/sdk/sequences/metric.py
--rw-r--r--   0 github     (503) staff       (20)      458 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/sequences/text_sequence.py
--rw-r--r--   0 github     (503) staff       (20)    10545 2022-09-25 12:02:15.000000 aim-4.0.0.dev3/aim/sdk/tracker.py
--rw-r--r--   0 github     (503) staff       (20)     2202 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/sdk/training_flow.py
--rw-r--r--   0 github     (503) staff       (20)      159 2022-06-18 00:13:24.000000 aim-4.0.0.dev3/aim/sdk/types.py
--rw-r--r--   0 github     (503) staff       (20)     2940 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/sdk/uri_service.py
--rw-r--r--   0 github     (503) staff       (20)     4046 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/sdk/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.976271 aim-4.0.0.dev3/aim/storage/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   439810 2023-04-10 17:48:47.000000 aim-4.0.0.dev3/aim/storage/arrayview.cpp
--rw-r--r--   0 github     (503) staff       (20)      278 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/arrayview.pxd
--rw-r--r--   0 github     (503) staff       (20)     2649 2022-06-15 14:05:59.000000 aim-4.0.0.dev3/aim/storage/arrayview.py
--rw-r--r--   0 github     (503) staff       (20)   844368 2023-04-10 17:48:47.000000 aim-4.0.0.dev3/aim/storage/container.cpp
--rw-r--r--   0 github     (503) staff       (20)      951 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/container.pxd
--rw-r--r--   0 github     (503) staff       (20)    10477 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/container.py
--rw-r--r--   0 github     (503) staff       (20)   912217 2023-04-10 17:48:48.000000 aim-4.0.0.dev3/aim/storage/containertreeview.cpp
--rw-r--r--   0 github     (503) staff       (20)      313 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/containertreeview.pxd
--rw-r--r--   0 github     (503) staff       (20)     6026 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/storage/containertreeview.py
--rw-r--r--   0 github     (503) staff       (20)     1212 2022-06-15 14:05:59.000000 aim-4.0.0.dev3/aim/storage/context.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.977728 aim-4.0.0.dev3/aim/storage/encoding/
--rw-r--r--   0 github     (503) staff       (20)   148655 2023-04-10 17:48:48.000000 aim-4.0.0.dev3/aim/storage/encoding/__init__.cpp
--rw-r--r--   0 github     (503) staff       (20)      155 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/encoding/__init__.pxd
--rw-r--r--   0 github     (503) staff       (20)       95 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/encoding/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   378105 2023-04-10 17:48:48.000000 aim-4.0.0.dev3/aim/storage/encoding/encoding.cpp
--rw-r--r--   0 github     (503) staff       (20)      507 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/encoding/encoding.pxd
--rw-r--r--   0 github     (503) staff       (20)     7373 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/encoding/encoding.pyx
--rw-r--r--   0 github     (503) staff       (20)   353597 2023-04-10 17:48:48.000000 aim-4.0.0.dev3/aim/storage/encoding/encoding_native.cpp
--rw-r--r--   0 github     (503) staff       (20)      930 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/encoding/encoding_native.pxd
--rw-r--r--   0 github     (503) staff       (20)     5974 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/encoding/encoding_native.pyx
--rw-r--r--   0 github     (503) staff       (20)      337 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/env.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.979081 aim-4.0.0.dev3/aim/storage/hashing/
--rw-r--r--   0 github     (503) staff       (20)   141729 2023-04-10 17:48:48.000000 aim-4.0.0.dev3/aim/storage/hashing/__init__.cpp
--rw-r--r--   0 github     (503) staff       (20)       85 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/hashing/__init__.pxd
--rw-r--r--   0 github     (503) staff       (20)       50 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/hashing/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   205598 2023-04-10 17:48:48.000000 aim-4.0.0.dev3/aim/storage/hashing/c_hash.cpp
--rw-r--r--   0 github     (503) staff       (20)      151 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/hashing/c_hash.pxd
--rw-r--r--   0 github     (503) staff       (20)     1077 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/hashing/c_hash.pyx
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.979189 aim-4.0.0.dev3/aim/storage/hashing/hash/
--rw-r--r--   0 github     (503) staff       (20)     1412 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/hashing/hash/hash.h
--rw-r--r--   0 github     (503) staff       (20)   392224 2023-04-10 17:48:48.000000 aim-4.0.0.dev3/aim/storage/hashing/hashing.cpp
--rw-r--r--   0 github     (503) staff       (20)     1009 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/hashing/hashing.pxd
--rw-r--r--   0 github     (503) staff       (20)     5562 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/storage/hashing/hashing.py
--rw-r--r--   0 github     (503) staff       (20)   672756 2023-04-10 17:48:48.000000 aim-4.0.0.dev3/aim/storage/inmemorytreeview.cpp
--rw-r--r--   0 github     (503) staff       (20)      196 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/inmemorytreeview.pxd
--rw-r--r--   0 github     (503) staff       (20)     4341 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/storage/inmemorytreeview.py
--rw-r--r--   0 github     (503) staff       (20)     1322 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/storage/lock_proxy.py
--rw-r--r--   0 github     (503) staff       (20)     6344 2023-04-06 20:09:56.000000 aim-4.0.0.dev3/aim/storage/locking.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.981488 aim-4.0.0.dev3/aim/storage/migrations/
--rw-r--r--   0 github     (503) staff       (20)       38 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/README
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2218 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/alembic.ini
--rw-r--r--   0 github     (503) staff       (20)     2215 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/alembic_dev.ini
--rw-r--r--   0 github     (503) staff       (20)     2339 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/env.py
--rw-r--r--   0 github     (503) staff       (20)      494 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/script.py.mako
--rw-r--r--   0 github     (503) staff       (20)      965 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.982665 aim-4.0.0.dev3/aim/storage/migrations/versions/
--rw-r--r--   0 github     (503) staff       (20)     2841 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/versions/1ecf8222220d_initial_schema.py
--rw-r--r--   0 github     (503) staff       (20)      658 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/versions/3c4f22db7a46_run_end_time.py
--rw-r--r--   0 github     (503) staff       (20)     1475 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/storage/migrations/versions/46b89d830ad8_.py
--rw-r--r--   0 github     (503) staff       (20)      653 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/versions/9ba30ab3b2b4_.py
--rw-r--r--   0 github     (503) staff       (20)     1516 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/versions/b07e7b07c8ce_.py
--rw-r--r--   0 github     (503) staff       (20)      789 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/migrations/versions/fbfe5c4702fb_soft_delete.py
--rw-r--r--   0 github     (503) staff       (20)     1650 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/object.py
--rw-r--r--   0 github     (503) staff       (20)   959785 2023-04-10 17:48:49.000000 aim-4.0.0.dev3/aim/storage/prefixview.cpp
--rw-r--r--   0 github     (503) staff       (20)      770 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/prefixview.pxd
--rw-r--r--   0 github     (503) staff       (20)    11248 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/prefixview.py
--rw-r--r--   0 github     (503) staff       (20)    11648 2022-06-15 14:05:59.000000 aim-4.0.0.dev3/aim/storage/proxy.py
--rw-r--r--   0 github     (503) staff       (20)     4816 2022-07-21 10:42:47.000000 aim-4.0.0.dev3/aim/storage/query.py
--rw-r--r--   0 github     (503) staff       (20)  1056280 2023-04-10 17:48:49.000000 aim-4.0.0.dev3/aim/storage/rockscontainer.cpp
--rw-r--r--   0 github     (503) staff       (20)    18514 2023-01-23 20:08:00.000000 aim-4.0.0.dev3/aim/storage/rockscontainer.pyx
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.983441 aim-4.0.0.dev3/aim/storage/structured/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/structured/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3183 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/structured/db.py
--rw-r--r--   0 github     (503) staff       (20)     5355 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/storage/structured/entities.py
--rw-r--r--   0 github     (503) staff       (20)     2959 2022-11-12 00:14:35.000000 aim-4.0.0.dev3/aim/storage/structured/proxy.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.984595 aim-4.0.0.dev3/aim/storage/structured/sql_engine/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/structured/sql_engine/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    19882 2023-01-25 20:08:55.000000 aim-4.0.0.dev3/aim/storage/structured/sql_engine/entities.py
--rw-r--r--   0 github     (503) staff       (20)     3484 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/structured/sql_engine/factory.py
--rw-r--r--   0 github     (503) staff       (20)     4888 2022-11-25 20:09:54.000000 aim-4.0.0.dev3/aim/storage/structured/sql_engine/models.py
--rw-r--r--   0 github     (503) staff       (20)     4811 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/structured/sql_engine/utils.py
--rw-r--r--   0 github     (503) staff       (20)   697830 2023-04-10 17:48:49.000000 aim-4.0.0.dev3/aim/storage/treearrayview.cpp
--rw-r--r--   0 github     (503) staff       (20)      251 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/treearrayview.pxd
--rw-r--r--   0 github     (503) staff       (20)     3033 2022-08-02 09:43:44.000000 aim-4.0.0.dev3/aim/storage/treearrayview.py
--rw-r--r--   0 github     (503) staff       (20)   722166 2023-04-10 17:48:49.000000 aim-4.0.0.dev3/aim/storage/treeutils.cpp
--rw-r--r--   0 github     (503) staff       (20)     8365 2022-06-15 14:05:59.000000 aim-4.0.0.dev3/aim/storage/treeutils.pyx
--rw-r--r--   0 github     (503) staff       (20)      707 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/treeutils_non_native.py
--rw-r--r--   0 github     (503) staff       (20)   515752 2023-04-10 17:48:49.000000 aim-4.0.0.dev3/aim/storage/treeview.cpp
--rw-r--r--   0 github     (503) staff       (20)      311 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/treeview.pxd
--rw-r--r--   0 github     (503) staff       (20)     2765 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/storage/treeview.py
--rw-r--r--   0 github     (503) staff       (20)     8241 2023-02-27 08:16:06.000000 aim-4.0.0.dev3/aim/storage/treeviewproxy.py
--rw-r--r--   0 github     (503) staff       (20)     1357 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/types.py
--rw-r--r--   0 github     (503) staff       (20)   812526 2023-04-10 17:48:49.000000 aim-4.0.0.dev3/aim/storage/union.cpp
--rw-r--r--   0 github     (503) staff       (20)     7919 2023-01-23 20:08:00.000000 aim-4.0.0.dev3/aim/storage/union.pyx
--rw-r--r--   0 github     (503) staff       (20)   810540 2023-04-10 17:48:50.000000 aim-4.0.0.dev3/aim/storage/utils.cpp
--rw-r--r--   0 github     (503) staff       (20)      469 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/utils.pxd
--rw-r--r--   0 github     (503) staff       (20)     2102 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/storage/utils.py
--rw-r--r--   0 github     (503) staff       (20)      119 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/tensorflow.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.985324 aim-4.0.0.dev3/aim/utils/
--rw-r--r--   0 github     (503) staff       (20)       84 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/aim/utils/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1209 2023-02-01 20:08:30.000000 aim-4.0.0.dev3/aim/utils/deprecation.py
--rw-r--r--   0 github     (503) staff       (20)     4728 2023-02-27 08:16:06.000000 aim-4.0.0.dev3/aim/utils/tracking.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.986193 aim-4.0.0.dev3/aim/web/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.987139 aim-4.0.0.dev3/aim/web/api/
--rw-r--r--   0 github     (503) staff       (20)     3504 2023-01-23 10:30:27.000000 aim-4.0.0.dev3/aim/web/api/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.987988 aim-4.0.0.dev3/aim/web/api/dashboard_apps/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/dashboard_apps/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      939 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/dashboard_apps/models.py
--rw-r--r--   0 github     (503) staff       (20)      542 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/dashboard_apps/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)      445 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/dashboard_apps/serializers.py
--rw-r--r--   0 github     (503) staff       (20)     2974 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/dashboard_apps/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.988889 aim-4.0.0.dev3/aim/web/api/dashboards/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/dashboards/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      667 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/dashboards/models.py
--rw-r--r--   0 github     (503) staff       (20)      652 2022-10-06 00:17:33.000000 aim-4.0.0.dev3/aim/web/api/dashboards/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)      775 2022-10-06 00:17:33.000000 aim-4.0.0.dev3/aim/web/api/dashboards/serializers.py
--rw-r--r--   0 github     (503) staff       (20)     3341 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/dashboards/views.py
--rw-r--r--   0 github     (503) staff       (20)      820 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/db.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.989400 aim-4.0.0.dev3/aim/web/api/experiments/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/experiments/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      974 2022-11-24 20:09:30.000000 aim-4.0.0.dev3/aim/web/api/experiments/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)     8931 2023-01-19 20:08:35.000000 aim-4.0.0.dev3/aim/web/api/experiments/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.990242 aim-4.0.0.dev3/aim/web/api/projects/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/projects/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      735 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/projects/project.py
--rw-r--r--   0 github     (503) staff       (20)      943 2022-10-06 00:17:33.000000 aim-4.0.0.dev3/aim/web/api/projects/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)     5200 2023-01-24 20:09:40.000000 aim-4.0.0.dev3/aim/web/api/projects/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.991757 aim-4.0.0.dev3/aim/web/api/runs/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/runs/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    12969 2022-07-21 10:42:47.000000 aim-4.0.0.dev3/aim/web/api/runs/object_api_utils.py
--rw-r--r--   0 github     (503) staff       (20)     6683 2022-07-21 10:42:47.000000 aim-4.0.0.dev3/aim/web/api/runs/object_views.py
--rw-r--r--   0 github     (503) staff       (20)     4420 2022-12-23 10:19:51.000000 aim-4.0.0.dev3/aim/web/api/runs/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)    16029 2023-04-06 20:09:56.000000 aim-4.0.0.dev3/aim/web/api/runs/utils.py
--rw-r--r--   0 github     (503) staff       (20)    12258 2023-04-06 20:09:56.000000 aim-4.0.0.dev3/aim/web/api/runs/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.992319 aim-4.0.0.dev3/aim/web/api/tags/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/tags/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      871 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/tags/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)     4272 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/tags/views.py
--rw-r--r--   0 github     (503) staff       (20)     1169 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/api/utils.py
--rw-r--r--   0 github     (503) staff       (20)     1589 2022-05-16 21:25:24.000000 aim-4.0.0.dev3/aim/web/api/views.py
--rw-r--r--   0 github     (503) staff       (20)      508 2022-08-11 13:58:02.000000 aim-4.0.0.dev3/aim/web/configs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.992494 aim-4.0.0.dev3/aim/web/middlewares/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/middlewares/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.992857 aim-4.0.0.dev3/aim/web/middlewares/profiler/
--rw-r--r--   0 github     (503) staff       (20)       81 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/middlewares/profiler/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3654 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/middlewares/profiler/profiler.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.993713 aim-4.0.0.dev3/aim/web/migrations/
--rw-r--r--   0 github     (503) staff       (20)       38 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/migrations/README
--rw-r--r--   0 github     (503) staff       (20)      810 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/migrations/alembic.ini
--rw-r--r--   0 github     (503) staff       (20)      807 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/migrations/alembic_dev.ini
--rw-r--r--   0 github     (503) staff       (20)     2792 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/migrations/env.py
--rw-r--r--   0 github     (503) staff       (20)      494 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/migrations/script.py.mako
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.994443 aim-4.0.0.dev3/aim/web/migrations/versions/
--rw-r--r--   0 github     (503) staff       (20)     2183 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/migrations/versions/11672b13f92c_.py
--rw-r--r--   0 github     (503) staff       (20)     1545 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/migrations/versions/517a45b2e62c_.py
--rw-r--r--   0 github     (503) staff       (20)     5592 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/migrations/versions/5ae8371b7481_.py
--rw-r--r--   0 github     (503) staff       (20)     7262 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/migrations/versions/73a3d004c227_.py
--rw-r--r--   0 github     (503) staff       (20)       55 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/run.py
--rw-r--r--   0 github     (503) staff       (20)     3055 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/web/utils.py
--rw-r--r--   0 github     (503) staff       (20)       96 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/aim/xgboost.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.921023 aim-4.0.0.dev3/aim.egg-info/
--rw-r--r--   0 github     (503) staff       (20)    37846 2023-04-10 17:48:50.000000 aim-4.0.0.dev3/aim.egg-info/PKG-INFO
--rw-r--r--   0 github     (503) staff       (20)    11901 2023-04-10 17:48:50.000000 aim-4.0.0.dev3/aim.egg-info/SOURCES.txt
--rw-r--r--   0 github     (503) staff       (20)        1 2023-04-10 17:48:50.000000 aim-4.0.0.dev3/aim.egg-info/dependency_links.txt
--rw-r--r--   0 github     (503) staff       (20)      102 2023-04-10 17:48:50.000000 aim-4.0.0.dev3/aim.egg-info/entry_points.txt
--rw-r--r--   0 github     (503) staff       (20)      422 2023-04-10 17:48:50.000000 aim-4.0.0.dev3/aim.egg-info/requires.txt
--rw-r--r--   0 github     (503) staff       (20)       28 2023-04-10 17:48:50.000000 aim-4.0.0.dev3/aim.egg-info/top_level.txt
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.912416 aim-4.0.0.dev3/performance_tests/
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.995532 aim-4.0.0.dev3/performance_tests/sdk/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/performance_tests/sdk/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      469 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/performance_tests/sdk/queries.py
--rw-r--r--   0 github     (503) staff       (20)     1199 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/performance_tests/sdk/test_data_collection.py
--rw-r--r--   0 github     (503) staff       (20)     1134 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/performance_tests/sdk/test_query.py
--rw-r--r--   0 github     (503) staff       (20)     1881 2022-06-18 00:13:24.000000 aim-4.0.0.dev3/performance_tests/sdk/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.996390 aim-4.0.0.dev3/performance_tests/storage/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/performance_tests/storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      678 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/performance_tests/storage/test_container_open.py
--rw-r--r--   0 github     (503) staff       (20)      690 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/performance_tests/storage/test_iterative_access.py
--rw-r--r--   0 github     (503) staff       (20)      802 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/performance_tests/storage/test_random_access.py
--rw-r--r--   0 github     (503) staff       (20)     1262 2022-06-18 00:13:24.000000 aim-4.0.0.dev3/performance_tests/storage/utils.py
--rw-r--r--   0 github     (503) staff       (20)       84 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/pyproject.toml
--rw-r--r--   0 github     (503) staff       (20)      336 2023-04-10 17:48:51.003221 aim-4.0.0.dev3/setup.cfg
--rw-r--r--   0 github     (503) staff       (20)     6716 2023-03-02 20:49:40.000000 aim-4.0.0.dev3/setup.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.912679 aim-4.0.0.dev3/tests/
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.998347 aim-4.0.0.dev3/tests/api/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/tests/api/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5155 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/tests/api/test_dashboards_api.py
--rw-r--r--   0 github     (503) staff       (20)     4335 2022-09-25 12:02:15.000000 aim-4.0.0.dev3/tests/api/test_project_api.py
--rw-r--r--   0 github     (503) staff       (20)    10653 2023-01-23 10:30:27.000000 aim-4.0.0.dev3/tests/api/test_run_api.py
--rw-r--r--   0 github     (503) staff       (20)    21533 2023-01-23 10:30:27.000000 aim-4.0.0.dev3/tests/api/test_run_images_api.py
--rw-r--r--   0 github     (503) staff       (20)    12787 2023-01-23 10:30:27.000000 aim-4.0.0.dev3/tests/api/test_structured_data_api.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:50.999118 aim-4.0.0.dev3/tests/integrations/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/tests/integrations/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1167 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/tests/integrations/test_dvc_metadata.py
--rw-r--r--   0 github     (503) staff       (20)     1093 2023-01-13 20:10:23.000000 aim-4.0.0.dev3/tests/integrations/test_hf_datasets.py
--rw-r--r--   0 github     (503) staff       (20)      961 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/tests/integrations/test_hub_dataset.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:51.001562 aim-4.0.0.dev3/tests/sdk/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/tests/sdk/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2312 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/tests/sdk/test_image_construction.py
--rw-r--r--   0 github     (503) staff       (20)     2665 2022-09-25 12:02:15.000000 aim-4.0.0.dev3/tests/sdk/test_resource_tracker.py
--rw-r--r--   0 github     (503) staff       (20)     1022 2022-11-01 00:13:35.000000 aim-4.0.0.dev3/tests/sdk/test_run_apis.py
--rw-r--r--   0 github     (503) staff       (20)     1147 2022-09-01 19:23:53.000000 aim-4.0.0.dev3/tests/sdk/test_run_creation_checks.py
--rw-r--r--   0 github     (503) staff       (20)     1661 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/tests/sdk/test_run_finalization_time.py
--rw-r--r--   0 github     (503) staff       (20)     1214 2022-11-01 00:13:35.000000 aim-4.0.0.dev3/tests/sdk/test_run_metric_types.py
--rw-r--r--   0 github     (503) staff       (20)     4631 2022-09-25 12:02:15.000000 aim-4.0.0.dev3/tests/sdk/test_run_track_type_checking.py
--rw-r--r--   0 github     (503) staff       (20)    10444 2022-09-25 12:02:15.000000 aim-4.0.0.dev3/tests/sdk/test_run_write_container_data.py
--rw-r--r--   0 github     (503) staff       (20)     4517 2022-06-01 01:05:15.000000 aim-4.0.0.dev3/tests/sdk/test_utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-10 17:48:51.002535 aim-4.0.0.dev3/tests/storage/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev3/tests/storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5677 2022-09-25 12:02:15.000000 aim-4.0.0.dev3/tests/storage/test_query.py
--rw-r--r--   0 github     (503) staff       (20)     1482 2022-06-18 00:13:24.000000 aim-4.0.0.dev3/tests/storage/test_query_with_epoch_none.py
--rw-r--r--   0 github     (503) staff       (20)     1342 2022-09-25 12:02:15.000000 aim-4.0.0.dev3/tests/storage/test_structured_db.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.951090 aim-4.0.0.dev4/
+-rw-r--r--   0 github     (503) staff       (20)    11347 2022-08-06 00:13:01.000000 aim-4.0.0.dev4/LICENSE
+-rw-r--r--   0 github     (503) staff       (20)      185 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/MANIFEST.in
+-rw-r--r--   0 github     (503) staff       (20)    38879 2023-04-29 15:33:52.951264 aim-4.0.0.dev4/PKG-INFO
+-rw-r--r--   0 github     (503) staff       (20)    38192 2023-04-28 20:15:40.000000 aim-4.0.0.dev4/README.md
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.868392 aim-4.0.0.dev4/aim/
+-rw-r--r--   0 github     (503) staff       (20)        9 2023-04-29 15:33:43.000000 aim-4.0.0.dev4/aim/VERSION
+-rw-r--r--   0 github     (503) staff       (20)      825 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/__about__.py
+-rw-r--r--   0 github     (503) staff       (20)      377 2023-02-01 20:08:30.000000 aim-4.0.0.dev4/aim/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      183 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/__version__.py
+-rw-r--r--   0 github     (503) staff       (20)      100 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/acme.py
+-rw-r--r--   0 github     (503) staff       (20)       96 2022-05-06 13:59:46.000000 aim-4.0.0.dev4/aim/catboost.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.870341 aim-4.0.0.dev4/aim/cli/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1323 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/cli/cli.py
+-rw-r--r--   0 github     (503) staff       (20)      166 2022-06-17 00:13:19.000000 aim-4.0.0.dev4/aim/cli/configs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.870679 aim-4.0.0.dev4/aim/cli/convert/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/convert/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2998 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/cli/convert/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.871684 aim-4.0.0.dev4/aim/cli/convert/processors/
+-rw-r--r--   0 github     (503) staff       (20)      113 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/cli/convert/processors/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     5914 2022-09-01 19:23:53.000000 aim-4.0.0.dev4/aim/cli/convert/processors/mlflow.py
+-rw-r--r--   0 github     (503) staff       (20)    10372 2022-08-06 00:13:01.000000 aim-4.0.0.dev4/aim/cli/convert/processors/tensorboard.py
+-rw-r--r--   0 github     (503) staff       (20)     6816 2023-01-04 20:08:59.000000 aim-4.0.0.dev4/aim/cli/convert/processors/wandb.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.872020 aim-4.0.0.dev4/aim/cli/init/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/init/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1592 2023-03-24 14:18:45.000000 aim-4.0.0.dev4/aim/cli/init/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.872373 aim-4.0.0.dev4/aim/cli/manager/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/manager/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3382 2022-08-11 13:58:02.000000 aim-4.0.0.dev4/aim/cli/manager/manager.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.872736 aim-4.0.0.dev4/aim/cli/reindex/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/reindex/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      736 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/cli/reindex/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.873365 aim-4.0.0.dev4/aim/cli/runs/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/runs/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     6621 2023-03-24 14:18:45.000000 aim-4.0.0.dev4/aim/cli/runs/commands.py
+-rw-r--r--   0 github     (503) staff       (20)     2570 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/cli/runs/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.873697 aim-4.0.0.dev4/aim/cli/server/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/server/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3709 2023-03-24 14:18:45.000000 aim-4.0.0.dev4/aim/cli/server/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.874000 aim-4.0.0.dev4/aim/cli/storage/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-06-17 00:13:19.000000 aim-4.0.0.dev4/aim/cli/storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     7537 2023-03-24 14:18:45.000000 aim-4.0.0.dev4/aim/cli/storage/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.874345 aim-4.0.0.dev4/aim/cli/telemetry/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/cli/telemetry/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      305 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/cli/telemetry/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.875058 aim-4.0.0.dev4/aim/cli/up/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/up/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     5953 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/cli/up/commands.py
+-rw-r--r--   0 github     (503) staff       (20)     1446 2022-06-21 18:01:08.000000 aim-4.0.0.dev4/aim/cli/up/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.875721 aim-4.0.0.dev4/aim/cli/upgrade/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.876494 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/
+-rw-r--r--   0 github     (503) staff       (20)      258 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      734 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/configs.py
+-rw-r--r--   0 github     (503) staff       (20)      448 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/metric_artifact.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.877138 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      263 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/base_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)      267 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/metric_pb2.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.877591 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v3/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v3/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3396 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v3/base_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)     1919 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v3/metric_pb2.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.877984 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v4/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v4/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1111 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v4/base_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)      969 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v4/metric_pb2.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.878979 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/
+-rw-r--r--   0 github     (503) staff       (20)        1 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1722 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/metric.py
+-rw-r--r--   0 github     (503) staff       (20)     3722 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/repo.py
+-rw-r--r--   0 github     (503) staff       (20)     4062 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/run.py
+-rw-r--r--   0 github     (503) staff       (20)     1357 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/trace.py
+-rw-r--r--   0 github     (503) staff       (20)     1211 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/utils.py
+-rw-r--r--   0 github     (503) staff       (20)     6635 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/utils.py
+-rw-r--r--   0 github     (503) staff       (20)      370 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.879237 aim-4.0.0.dev4/aim/cli/version/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/version/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      149 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/version/commands.py
+-rw-r--r--   0 github     (503) staff       (20)     9960 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/cli/watcher_cli.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.879813 aim-4.0.0.dev4/aim/ext/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.880086 aim-4.0.0.dev4/aim/ext/cleanup/
+-rw-r--r--   0 github     (503) staff       (20)     3579 2022-11-12 00:14:35.000000 aim-4.0.0.dev4/aim/ext/cleanup/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2021 2023-03-02 20:49:40.000000 aim-4.0.0.dev4/aim/ext/exception_resistant.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.880442 aim-4.0.0.dev4/aim/ext/notebook/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/notebook/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     7314 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/notebook/notebook.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.882468 aim-4.0.0.dev4/aim/ext/notifier/
+-rw-r--r--   0 github     (503) staff       (20)      589 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      305 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/base_notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1858 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/ext/notifier/config.py
+-rw-r--r--   0 github     (503) staff       (20)      361 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/config_default.json
+-rw-r--r--   0 github     (503) staff       (20)       70 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/config_empty.json
+-rw-r--r--   0 github     (503) staff       (20)      522 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/logging_notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1428 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1158 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/notifier_builder.py
+-rw-r--r--   0 github     (503) staff       (20)      524 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/slack_notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1034 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/utils.py
+-rw-r--r--   0 github     (503) staff       (20)      862 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/workplace_notifier.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.883736 aim-4.0.0.dev4/aim/ext/resource/
+-rw-r--r--   0 github     (503) staff       (20)       92 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/resource/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      100 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/resource/configs.py
+-rw-r--r--   0 github     (503) staff       (20)      726 2022-05-16 21:25:24.000000 aim-4.0.0.dev4/aim/ext/resource/log.py
+-rw-r--r--   0 github     (503) staff       (20)     6700 2023-01-04 20:08:59.000000 aim-4.0.0.dev4/aim/ext/resource/stat.py
+-rw-r--r--   0 github     (503) staff       (20)     7511 2023-01-04 20:08:59.000000 aim-4.0.0.dev4/aim/ext/resource/tracker.py
+-rw-r--r--   0 github     (503) staff       (20)       56 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/resource/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.883998 aim-4.0.0.dev4/aim/ext/sshfs/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/sshfs/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     7768 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/sshfs/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.884288 aim-4.0.0.dev4/aim/ext/task_queue/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/task_queue/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2069 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/task_queue/queue.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.884937 aim-4.0.0.dev4/aim/ext/tensorboard_tracker/
+-rw-r--r--   0 github     (503) staff       (20)       48 2023-01-04 20:08:59.000000 aim-4.0.0.dev4/aim/ext/tensorboard_tracker/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      919 2023-01-04 20:08:59.000000 aim-4.0.0.dev4/aim/ext/tensorboard_tracker/run.py
+-rw-r--r--   0 github     (503) staff       (20)     7201 2023-01-04 20:08:59.000000 aim-4.0.0.dev4/aim/ext/tensorboard_tracker/tracker.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.888986 aim-4.0.0.dev4/aim/ext/transport/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/transport/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    13282 2023-04-06 20:09:56.000000 aim-4.0.0.dev4/aim/ext/transport/client.py
+-rw-r--r--   0 github     (503) staff       (20)      563 2023-04-06 20:09:56.000000 aim-4.0.0.dev4/aim/ext/transport/config.py
+-rw-r--r--   0 github     (503) staff       (20)     3298 2023-01-23 20:08:00.000000 aim-4.0.0.dev4/aim/ext/transport/handlers.py
+-rw-r--r--   0 github     (503) staff       (20)     5555 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/health.py
+-rw-r--r--   0 github     (503) staff       (20)     5616 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/heartbeat.py
+-rw-r--r--   0 github     (503) staff       (20)     3347 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/message_utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.890766 aim-4.0.0.dev4/aim/ext/transport/proto/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      245 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/health_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)     3991 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/health_pb2_grpc.py
+-rw-r--r--   0 github     (503) staff       (20)      259 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/remote_router_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)     8855 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/remote_router_pb2_grpc.py
+-rw-r--r--   0 github     (503) staff       (20)      263 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/remote_tracking_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)     9444 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/remote_tracking_pb2_grpc.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.891721 aim-4.0.0.dev4/aim/ext/transport/proto/v3/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/v3/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     6195 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/v3/health_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)    25245 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/v3/remote_router_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)    37567 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/v3/remote_tracking_pb2.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.892484 aim-4.0.0.dev4/aim/ext/transport/proto/v4/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/v4/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1749 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/v4/health_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)     4280 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/v4/remote_router_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)     5662 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/v4/remote_tracking_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)      428 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/transport/remote_resource.py
+-rw-r--r--   0 github     (503) staff       (20)     8078 2023-01-23 10:30:27.000000 aim-4.0.0.dev4/aim/ext/transport/remote_tracking.py
+-rw-r--r--   0 github     (503) staff       (20)     3637 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/router.py
+-rw-r--r--   0 github     (503) staff       (20)     3728 2022-11-18 00:13:03.000000 aim-4.0.0.dev4/aim/ext/transport/rpc_queue.py
+-rw-r--r--   0 github     (503) staff       (20)     4609 2023-01-23 10:30:27.000000 aim-4.0.0.dev4/aim/ext/transport/server.py
+-rw-r--r--   0 github     (503) staff       (20)     3419 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/worker.py
+-rw-r--r--   0 github     (503) staff       (20)     2103 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/utils.py
+-rw-r--r--   0 github     (503) staff       (20)       92 2022-09-25 12:02:15.000000 aim-4.0.0.dev4/aim/fastai.py
+-rw-r--r--   0 github     (503) staff       (20)      127 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/hf_dataset.py
+-rw-r--r--   0 github     (503) staff       (20)      105 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/hugging_face.py
+-rw-r--r--   0 github     (503) staff       (20)      103 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/keras.py
+-rw-r--r--   0 github     (503) staff       (20)      103 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/keras_tuner.py
+-rw-r--r--   0 github     (503) staff       (20)       98 2022-05-06 13:59:46.000000 aim-4.0.0.dev4/aim/lightgbm.py
+-rw-r--r--   0 github     (503) staff       (20)       97 2022-10-04 00:16:28.000000 aim-4.0.0.dev4/aim/mxnet.py
+-rw-r--r--   0 github     (503) staff       (20)       98 2022-11-12 00:14:35.000000 aim-4.0.0.dev4/aim/optuna.py
+-rw-r--r--   0 github     (503) staff       (20)       99 2022-11-12 00:14:35.000000 aim-4.0.0.dev4/aim/paddle.py
+-rw-r--r--   0 github     (503) staff       (20)       93 2023-01-31 20:08:25.000000 aim-4.0.0.dev4/aim/prophet.py
+-rw-r--r--   0 github     (503) staff       (20)      115 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/pytorch.py
+-rw-r--r--   0 github     (503) staff       (20)      107 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/pytorch_ignite.py
+-rw-r--r--   0 github     (503) staff       (20)      113 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/pytorch_lightning.py
+-rw-r--r--   0 github     (503) staff       (20)       87 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/sb3.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.899412 aim-4.0.0.dev4/aim/sdk/
+-rw-r--r--   0 github     (503) staff       (20)      915 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.903019 aim-4.0.0.dev4/aim/sdk/adapters/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/adapters/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3521 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/acme.py
+-rw-r--r--   0 github     (503) staff       (20)     4648 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/catboost.py
+-rw-r--r--   0 github     (503) staff       (20)     6461 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/fastai.py
+-rw-r--r--   0 github     (503) staff       (20)     6610 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/hugging_face.py
+-rw-r--r--   0 github     (503) staff       (20)     3438 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/keras.py
+-rw-r--r--   0 github     (503) staff       (20)     1086 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/keras_mixins.py
+-rw-r--r--   0 github     (503) staff       (20)     3718 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/keras_tuner.py
+-rw-r--r--   0 github     (503) staff       (20)     3810 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/lightgbm.py
+-rw-r--r--   0 github     (503) staff       (20)     9022 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/mxnet.py
+-rw-r--r--   0 github     (503) staff       (20)     7300 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/optuna.py
+-rw-r--r--   0 github     (503) staff       (20)     3576 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/paddle.py
+-rw-r--r--   0 github     (503) staff       (20)     3772 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/prophet.py
+-rw-r--r--   0 github     (503) staff       (20)     2436 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/pytorch.py
+-rw-r--r--   0 github     (503) staff       (20)     9518 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/pytorch_ignite.py
+-rw-r--r--   0 github     (503) staff       (20)     6871 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/pytorch_lightning.py
+-rw-r--r--   0 github     (503) staff       (20)     4711 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/sb3.py
+-rw-r--r--   0 github     (503) staff       (20)     3459 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/tensorflow.py
+-rw-r--r--   0 github     (503) staff       (20)     3836 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/xgboost.py
+-rw-r--r--   0 github     (503) staff       (20)     5138 2023-03-16 00:07:12.000000 aim-4.0.0.dev4/aim/sdk/base_run.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.903811 aim-4.0.0.dev4/aim/sdk/callbacks/
+-rw-r--r--   0 github     (503) staff       (20)      196 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/callbacks/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1493 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/callbacks/caller.py
+-rw-r--r--   0 github     (503) staff       (20)      495 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/callbacks/events.py
+-rw-r--r--   0 github     (503) staff       (20)     1416 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/callbacks/helpers.py
+-rw-r--r--   0 github     (503) staff       (20)      253 2022-09-26 00:13:35.000000 aim-4.0.0.dev4/aim/sdk/configs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.905841 aim-4.0.0.dev4/aim/sdk/core/
+-rw-r--r--   0 github     (503) staff       (20)      263 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     9802 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/collections.py
+-rw-r--r--   0 github     (503) staff       (20)      519 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/constants.py
+-rw-r--r--   0 github     (503) staff       (20)    10813 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/container.py
+-rw-r--r--   0 github     (503) staff       (20)      561 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/exceptions.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.906253 aim-4.0.0.dev4/aim/sdk/core/interfaces/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/interfaces/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1247 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/interfaces/container.py
+-rw-r--r--   0 github     (503) staff       (20)     2255 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/interfaces/sequence.py
+-rw-r--r--   0 github     (503) staff       (20)      873 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/object.py
+-rw-r--r--   0 github     (503) staff       (20)     2805 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/query_utils.py
+-rw-r--r--   0 github     (503) staff       (20)     5286 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/repo.py
+-rw-r--r--   0 github     (503) staff       (20)     9304 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/sequence.py
+-rw-r--r--   0 github     (503) staff       (20)     3534 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/type_utils.py
+-rw-r--r--   0 github     (503) staff       (20)      205 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/utils.py
+-rw-r--r--   0 github     (503) staff       (20)       22 2022-11-24 20:09:30.000000 aim-4.0.0.dev4/aim/sdk/data_version.py
+-rw-r--r--   0 github     (503) staff       (20)      145 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/errors.py
+-rw-r--r--   0 github     (503) staff       (20)     4994 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/index_manager.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.907280 aim-4.0.0.dev4/aim/sdk/legacy/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/legacy/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      288 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/legacy/deprecation_warning.py
+-rw-r--r--   0 github     (503) staff       (20)       94 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/legacy/flush.py
+-rw-r--r--   0 github     (503) staff       (20)      185 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/legacy/init.py
+-rw-r--r--   0 github     (503) staff       (20)      702 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/legacy/select.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.907764 aim-4.0.0.dev4/aim/sdk/legacy/session/
+-rw-r--r--   0 github     (503) staff       (20)       67 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/legacy/session/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)       30 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/legacy/session/configs.py
+-rw-r--r--   0 github     (503) staff       (20)     4277 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/legacy/session/session.py
+-rw-r--r--   0 github     (503) staff       (20)      410 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/legacy/track.py
+-rw-r--r--   0 github     (503) staff       (20)     6513 2023-02-01 20:08:30.000000 aim-4.0.0.dev4/aim/sdk/lock_manager.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.908081 aim-4.0.0.dev4/aim/sdk/logging/
+-rw-r--r--   0 github     (503) staff       (20)       61 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/logging/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1863 2023-02-03 15:21:38.000000 aim-4.0.0.dev4/aim/sdk/logging/log_record.py
+-rw-r--r--   0 github     (503) staff       (20)      954 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/maintenance_run.py
+-rw-r--r--   0 github     (503) staff       (20)     3397 2023-03-16 00:07:12.000000 aim-4.0.0.dev4/aim/sdk/num_utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.909644 aim-4.0.0.dev4/aim/sdk/objects/
+-rw-r--r--   0 github     (503) staff       (20)      214 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/objects/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3264 2022-11-11 08:24:45.000000 aim-4.0.0.dev4/aim/sdk/objects/audio.py
+-rw-r--r--   0 github     (503) staff       (20)     4232 2023-01-04 20:08:59.000000 aim-4.0.0.dev4/aim/sdk/objects/distribution.py
+-rw-r--r--   0 github     (503) staff       (20)     2885 2023-01-04 20:08:59.000000 aim-4.0.0.dev4/aim/sdk/objects/figure.py
+-rw-r--r--   0 github     (503) staff       (20)     9914 2023-03-03 20:09:01.000000 aim-4.0.0.dev4/aim/sdk/objects/image.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.910009 aim-4.0.0.dev4/aim/sdk/objects/io/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/objects/io/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    21094 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/objects/io/wavfile.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.911089 aim-4.0.0.dev4/aim/sdk/objects/plugins/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/objects/plugins/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1983 2023-01-23 20:08:00.000000 aim-4.0.0.dev4/aim/sdk/objects/plugins/dvc_metadata.py
+-rw-r--r--   0 github     (503) staff       (20)     3648 2023-02-02 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/objects/plugins/hf_datasets_metadata.py
+-rw-r--r--   0 github     (503) staff       (20)     1272 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/objects/plugins/hub_dataset.py
+-rw-r--r--   0 github     (503) staff       (20)      694 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/objects/text.py
+-rw-r--r--   0 github     (503) staff       (20)     6048 2022-09-01 19:23:53.000000 aim-4.0.0.dev4/aim/sdk/query_utils.py
+-rw-r--r--   0 github     (503) staff       (20)     1050 2023-01-23 10:30:27.000000 aim-4.0.0.dev4/aim/sdk/remote_repo_proxy.py
+-rw-r--r--   0 github     (503) staff       (20)     2171 2023-01-23 10:30:27.000000 aim-4.0.0.dev4/aim/sdk/remote_run_reporter.py
+-rw-r--r--   0 github     (503) staff       (20)    34518 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/repo.py
+-rw-r--r--   0 github     (503) staff       (20)     1022 2023-03-16 00:07:12.000000 aim-4.0.0.dev4/aim/sdk/repo_utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.911754 aim-4.0.0.dev4/aim/sdk/reporter/
+-rw-r--r--   0 github     (503) staff       (20)    31012 2023-01-23 20:08:00.000000 aim-4.0.0.dev4/aim/sdk/reporter/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1832 2023-01-23 10:30:27.000000 aim-4.0.0.dev4/aim/sdk/reporter/file_manager.py
+-rw-r--r--   0 github     (503) staff       (20)    30870 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/run.py
+-rw-r--r--   0 github     (503) staff       (20)    13171 2023-02-03 15:21:38.000000 aim-4.0.0.dev4/aim/sdk/run_status_watcher.py
+-rw-r--r--   0 github     (503) staff       (20)    12970 2023-03-02 20:49:40.000000 aim-4.0.0.dev4/aim/sdk/sequence.py
+-rw-r--r--   0 github     (503) staff       (20)     9975 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/sequence_collection.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.913159 aim-4.0.0.dev4/aim/sdk/sequences/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/sequences/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      458 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/sequences/audio_sequence.py
+-rw-r--r--   0 github     (503) staff       (20)      408 2023-03-02 20:49:40.000000 aim-4.0.0.dev4/aim/sdk/sequences/distribution_sequence.py
+-rw-r--r--   0 github     (503) staff       (20)      452 2023-03-02 20:49:40.000000 aim-4.0.0.dev4/aim/sdk/sequences/figure_sequence.py
+-rw-r--r--   0 github     (503) staff       (20)      482 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/sequences/image_sequence.py
+-rw-r--r--   0 github     (503) staff       (20)     3936 2022-07-09 00:13:12.000000 aim-4.0.0.dev4/aim/sdk/sequences/metric.py
+-rw-r--r--   0 github     (503) staff       (20)      458 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/sequences/text_sequence.py
+-rw-r--r--   0 github     (503) staff       (20)    10545 2022-09-25 12:02:15.000000 aim-4.0.0.dev4/aim/sdk/tracker.py
+-rw-r--r--   0 github     (503) staff       (20)     2202 2023-03-02 20:49:40.000000 aim-4.0.0.dev4/aim/sdk/training_flow.py
+-rw-r--r--   0 github     (503) staff       (20)      159 2022-06-18 00:13:24.000000 aim-4.0.0.dev4/aim/sdk/types.py
+-rw-r--r--   0 github     (503) staff       (20)     2940 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/uri_service.py
+-rw-r--r--   0 github     (503) staff       (20)     4046 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.925774 aim-4.0.0.dev4/aim/storage/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   439810 2023-04-29 15:33:49.000000 aim-4.0.0.dev4/aim/storage/arrayview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      278 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/arrayview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     2649 2022-06-15 14:05:59.000000 aim-4.0.0.dev4/aim/storage/arrayview.py
+-rw-r--r--   0 github     (503) staff       (20)   844368 2023-04-29 15:33:49.000000 aim-4.0.0.dev4/aim/storage/container.cpp
+-rw-r--r--   0 github     (503) staff       (20)      951 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/container.pxd
+-rw-r--r--   0 github     (503) staff       (20)    10477 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/container.py
+-rw-r--r--   0 github     (503) staff       (20)   912217 2023-04-29 15:33:50.000000 aim-4.0.0.dev4/aim/storage/containertreeview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      313 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/containertreeview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     6026 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/storage/containertreeview.py
+-rw-r--r--   0 github     (503) staff       (20)     1825 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/storage/context.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.927198 aim-4.0.0.dev4/aim/storage/encoding/
+-rw-r--r--   0 github     (503) staff       (20)   148655 2023-04-29 15:33:50.000000 aim-4.0.0.dev4/aim/storage/encoding/__init__.cpp
+-rw-r--r--   0 github     (503) staff       (20)      155 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/encoding/__init__.pxd
+-rw-r--r--   0 github     (503) staff       (20)       95 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/encoding/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   378105 2023-04-29 15:33:50.000000 aim-4.0.0.dev4/aim/storage/encoding/encoding.cpp
+-rw-r--r--   0 github     (503) staff       (20)      507 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/encoding/encoding.pxd
+-rw-r--r--   0 github     (503) staff       (20)     7373 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/encoding/encoding.pyx
+-rw-r--r--   0 github     (503) staff       (20)   353597 2023-04-29 15:33:50.000000 aim-4.0.0.dev4/aim/storage/encoding/encoding_native.cpp
+-rw-r--r--   0 github     (503) staff       (20)      930 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/encoding/encoding_native.pxd
+-rw-r--r--   0 github     (503) staff       (20)     5974 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/encoding/encoding_native.pyx
+-rw-r--r--   0 github     (503) staff       (20)      337 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/env.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.928546 aim-4.0.0.dev4/aim/storage/hashing/
+-rw-r--r--   0 github     (503) staff       (20)   141729 2023-04-29 15:33:50.000000 aim-4.0.0.dev4/aim/storage/hashing/__init__.cpp
+-rw-r--r--   0 github     (503) staff       (20)       85 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/hashing/__init__.pxd
+-rw-r--r--   0 github     (503) staff       (20)       50 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/hashing/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   205598 2023-04-29 15:33:50.000000 aim-4.0.0.dev4/aim/storage/hashing/c_hash.cpp
+-rw-r--r--   0 github     (503) staff       (20)      151 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/hashing/c_hash.pxd
+-rw-r--r--   0 github     (503) staff       (20)     1077 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/hashing/c_hash.pyx
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.928654 aim-4.0.0.dev4/aim/storage/hashing/hash/
+-rw-r--r--   0 github     (503) staff       (20)     1412 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/hashing/hash/hash.h
+-rw-r--r--   0 github     (503) staff       (20)   392224 2023-04-29 15:33:50.000000 aim-4.0.0.dev4/aim/storage/hashing/hashing.cpp
+-rw-r--r--   0 github     (503) staff       (20)     1009 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/hashing/hashing.pxd
+-rw-r--r--   0 github     (503) staff       (20)     5562 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/storage/hashing/hashing.py
+-rw-r--r--   0 github     (503) staff       (20)   672756 2023-04-29 15:33:50.000000 aim-4.0.0.dev4/aim/storage/inmemorytreeview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      196 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/inmemorytreeview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     4341 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/storage/inmemorytreeview.py
+-rw-r--r--   0 github     (503) staff       (20)     1322 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/storage/lock_proxy.py
+-rw-r--r--   0 github     (503) staff       (20)     6344 2023-04-06 20:09:56.000000 aim-4.0.0.dev4/aim/storage/locking.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.930046 aim-4.0.0.dev4/aim/storage/migrations/
+-rw-r--r--   0 github     (503) staff       (20)       38 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/README
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2218 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/alembic.ini
+-rw-r--r--   0 github     (503) staff       (20)     2215 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/alembic_dev.ini
+-rw-r--r--   0 github     (503) staff       (20)     2339 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/env.py
+-rw-r--r--   0 github     (503) staff       (20)      494 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/script.py.mako
+-rw-r--r--   0 github     (503) staff       (20)      965 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.931198 aim-4.0.0.dev4/aim/storage/migrations/versions/
+-rw-r--r--   0 github     (503) staff       (20)     2841 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/versions/1ecf8222220d_initial_schema.py
+-rw-r--r--   0 github     (503) staff       (20)      658 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/versions/3c4f22db7a46_run_end_time.py
+-rw-r--r--   0 github     (503) staff       (20)     1475 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/storage/migrations/versions/46b89d830ad8_.py
+-rw-r--r--   0 github     (503) staff       (20)      653 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/versions/9ba30ab3b2b4_.py
+-rw-r--r--   0 github     (503) staff       (20)     1516 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/versions/b07e7b07c8ce_.py
+-rw-r--r--   0 github     (503) staff       (20)      789 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/versions/fbfe5c4702fb_soft_delete.py
+-rw-r--r--   0 github     (503) staff       (20)     1657 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/storage/object.py
+-rw-r--r--   0 github     (503) staff       (20)   959785 2023-04-29 15:33:51.000000 aim-4.0.0.dev4/aim/storage/prefixview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      770 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/prefixview.pxd
+-rw-r--r--   0 github     (503) staff       (20)    11248 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/prefixview.py
+-rw-r--r--   0 github     (503) staff       (20)    11648 2022-06-15 14:05:59.000000 aim-4.0.0.dev4/aim/storage/proxy.py
+-rw-r--r--   0 github     (503) staff       (20)     4937 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/storage/query.py
+-rw-r--r--   0 github     (503) staff       (20)  1056280 2023-04-29 15:33:51.000000 aim-4.0.0.dev4/aim/storage/rockscontainer.cpp
+-rw-r--r--   0 github     (503) staff       (20)    18514 2023-01-23 20:08:00.000000 aim-4.0.0.dev4/aim/storage/rockscontainer.pyx
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.931939 aim-4.0.0.dev4/aim/storage/structured/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/structured/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3183 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/structured/db.py
+-rw-r--r--   0 github     (503) staff       (20)     5355 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/storage/structured/entities.py
+-rw-r--r--   0 github     (503) staff       (20)     2959 2022-11-12 00:14:35.000000 aim-4.0.0.dev4/aim/storage/structured/proxy.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.933165 aim-4.0.0.dev4/aim/storage/structured/sql_engine/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/structured/sql_engine/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    19882 2023-01-25 20:08:55.000000 aim-4.0.0.dev4/aim/storage/structured/sql_engine/entities.py
+-rw-r--r--   0 github     (503) staff       (20)     3484 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/structured/sql_engine/factory.py
+-rw-r--r--   0 github     (503) staff       (20)     4888 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/storage/structured/sql_engine/models.py
+-rw-r--r--   0 github     (503) staff       (20)     4811 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/structured/sql_engine/utils.py
+-rw-r--r--   0 github     (503) staff       (20)   697830 2023-04-29 15:33:51.000000 aim-4.0.0.dev4/aim/storage/treearrayview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      251 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/treearrayview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     3033 2022-08-02 09:43:44.000000 aim-4.0.0.dev4/aim/storage/treearrayview.py
+-rw-r--r--   0 github     (503) staff       (20)   722166 2023-04-29 15:33:51.000000 aim-4.0.0.dev4/aim/storage/treeutils.cpp
+-rw-r--r--   0 github     (503) staff       (20)     8365 2022-06-15 14:05:59.000000 aim-4.0.0.dev4/aim/storage/treeutils.pyx
+-rw-r--r--   0 github     (503) staff       (20)      707 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/treeutils_non_native.py
+-rw-r--r--   0 github     (503) staff       (20)   515752 2023-04-29 15:33:51.000000 aim-4.0.0.dev4/aim/storage/treeview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      311 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/treeview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     2765 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/storage/treeview.py
+-rw-r--r--   0 github     (503) staff       (20)     8241 2023-02-27 08:16:06.000000 aim-4.0.0.dev4/aim/storage/treeviewproxy.py
+-rw-r--r--   0 github     (503) staff       (20)     1357 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/types.py
+-rw-r--r--   0 github     (503) staff       (20)   812526 2023-04-29 15:33:51.000000 aim-4.0.0.dev4/aim/storage/union.cpp
+-rw-r--r--   0 github     (503) staff       (20)     7919 2023-01-23 20:08:00.000000 aim-4.0.0.dev4/aim/storage/union.pyx
+-rw-r--r--   0 github     (503) staff       (20)   810540 2023-04-29 15:33:52.000000 aim-4.0.0.dev4/aim/storage/utils.cpp
+-rw-r--r--   0 github     (503) staff       (20)      469 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/utils.pxd
+-rw-r--r--   0 github     (503) staff       (20)     2102 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/utils.py
+-rw-r--r--   0 github     (503) staff       (20)      119 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/tensorflow.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.933815 aim-4.0.0.dev4/aim/utils/
+-rw-r--r--   0 github     (503) staff       (20)       84 2023-03-02 20:49:40.000000 aim-4.0.0.dev4/aim/utils/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1209 2023-02-01 20:08:30.000000 aim-4.0.0.dev4/aim/utils/deprecation.py
+-rw-r--r--   0 github     (503) staff       (20)     4728 2023-02-27 08:16:06.000000 aim-4.0.0.dev4/aim/utils/tracking.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.934668 aim-4.0.0.dev4/aim/web/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.935577 aim-4.0.0.dev4/aim/web/api/
+-rw-r--r--   0 github     (503) staff       (20)     3616 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/web/api/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.936488 aim-4.0.0.dev4/aim/web/api/dashboard_apps/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/dashboard_apps/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      939 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/dashboard_apps/models.py
+-rw-r--r--   0 github     (503) staff       (20)      542 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/dashboard_apps/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)      445 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/dashboard_apps/serializers.py
+-rw-r--r--   0 github     (503) staff       (20)     2974 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/dashboard_apps/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.937349 aim-4.0.0.dev4/aim/web/api/dashboards/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/dashboards/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      667 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/dashboards/models.py
+-rw-r--r--   0 github     (503) staff       (20)      652 2022-10-06 00:17:33.000000 aim-4.0.0.dev4/aim/web/api/dashboards/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)      775 2022-10-06 00:17:33.000000 aim-4.0.0.dev4/aim/web/api/dashboards/serializers.py
+-rw-r--r--   0 github     (503) staff       (20)     3341 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/dashboards/views.py
+-rw-r--r--   0 github     (503) staff       (20)      820 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/db.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.937863 aim-4.0.0.dev4/aim/web/api/experiments/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/experiments/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      974 2022-11-24 20:09:30.000000 aim-4.0.0.dev4/aim/web/api/experiments/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)     8931 2023-01-19 20:08:35.000000 aim-4.0.0.dev4/aim/web/api/experiments/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.938676 aim-4.0.0.dev4/aim/web/api/projects/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/projects/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      740 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/web/api/projects/project.py
+-rw-r--r--   0 github     (503) staff       (20)      943 2022-10-06 00:17:33.000000 aim-4.0.0.dev4/aim/web/api/projects/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)     5200 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/web/api/projects/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.939011 aim-4.0.0.dev4/aim/web/api/queries/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/web/api/queries/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2770 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/web/api/queries/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.940347 aim-4.0.0.dev4/aim/web/api/runs/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/runs/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    12969 2022-07-21 10:42:47.000000 aim-4.0.0.dev4/aim/web/api/runs/object_api_utils.py
+-rw-r--r--   0 github     (503) staff       (20)     7642 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/web/api/runs/object_views.py
+-rw-r--r--   0 github     (503) staff       (20)     4420 2022-12-23 10:19:51.000000 aim-4.0.0.dev4/aim/web/api/runs/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)    16029 2023-04-06 20:09:56.000000 aim-4.0.0.dev4/aim/web/api/runs/utils.py
+-rw-r--r--   0 github     (503) staff       (20)    13619 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/web/api/runs/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.940900 aim-4.0.0.dev4/aim/web/api/tags/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/tags/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      871 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/tags/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)     4272 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/tags/views.py
+-rw-r--r--   0 github     (503) staff       (20)     1169 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/utils.py
+-rw-r--r--   0 github     (503) staff       (20)     1589 2022-05-16 21:25:24.000000 aim-4.0.0.dev4/aim/web/api/views.py
+-rw-r--r--   0 github     (503) staff       (20)      508 2022-08-11 13:58:02.000000 aim-4.0.0.dev4/aim/web/configs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.941056 aim-4.0.0.dev4/aim/web/middlewares/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/middlewares/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.941420 aim-4.0.0.dev4/aim/web/middlewares/profiler/
+-rw-r--r--   0 github     (503) staff       (20)       81 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/middlewares/profiler/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3654 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/middlewares/profiler/profiler.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.942337 aim-4.0.0.dev4/aim/web/migrations/
+-rw-r--r--   0 github     (503) staff       (20)       38 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/migrations/README
+-rw-r--r--   0 github     (503) staff       (20)      810 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/migrations/alembic.ini
+-rw-r--r--   0 github     (503) staff       (20)      807 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/migrations/alembic_dev.ini
+-rw-r--r--   0 github     (503) staff       (20)     2792 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/migrations/env.py
+-rw-r--r--   0 github     (503) staff       (20)      494 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/migrations/script.py.mako
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.943023 aim-4.0.0.dev4/aim/web/migrations/versions/
+-rw-r--r--   0 github     (503) staff       (20)     2183 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/migrations/versions/11672b13f92c_.py
+-rw-r--r--   0 github     (503) staff       (20)     1545 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/migrations/versions/517a45b2e62c_.py
+-rw-r--r--   0 github     (503) staff       (20)     5592 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/migrations/versions/5ae8371b7481_.py
+-rw-r--r--   0 github     (503) staff       (20)     7262 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/migrations/versions/73a3d004c227_.py
+-rw-r--r--   0 github     (503) staff       (20)       55 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/run.py
+-rw-r--r--   0 github     (503) staff       (20)     3055 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/utils.py
+-rw-r--r--   0 github     (503) staff       (20)       96 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/xgboost.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.869331 aim-4.0.0.dev4/aim.egg-info/
+-rw-r--r--   0 github     (503) staff       (20)    38879 2023-04-29 15:33:52.000000 aim-4.0.0.dev4/aim.egg-info/PKG-INFO
+-rw-r--r--   0 github     (503) staff       (20)    12349 2023-04-29 15:33:52.000000 aim-4.0.0.dev4/aim.egg-info/SOURCES.txt
+-rw-r--r--   0 github     (503) staff       (20)        1 2023-04-29 15:33:52.000000 aim-4.0.0.dev4/aim.egg-info/dependency_links.txt
+-rw-r--r--   0 github     (503) staff       (20)      102 2023-04-29 15:33:52.000000 aim-4.0.0.dev4/aim.egg-info/entry_points.txt
+-rw-r--r--   0 github     (503) staff       (20)      422 2023-04-29 15:33:52.000000 aim-4.0.0.dev4/aim.egg-info/requires.txt
+-rw-r--r--   0 github     (503) staff       (20)       28 2023-04-29 15:33:52.000000 aim-4.0.0.dev4/aim.egg-info/top_level.txt
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.860730 aim-4.0.0.dev4/performance_tests/
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.943993 aim-4.0.0.dev4/performance_tests/sdk/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/performance_tests/sdk/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      469 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/performance_tests/sdk/queries.py
+-rw-r--r--   0 github     (503) staff       (20)     1199 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/performance_tests/sdk/test_data_collection.py
+-rw-r--r--   0 github     (503) staff       (20)     1134 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/performance_tests/sdk/test_query.py
+-rw-r--r--   0 github     (503) staff       (20)     1881 2022-06-18 00:13:24.000000 aim-4.0.0.dev4/performance_tests/sdk/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.944874 aim-4.0.0.dev4/performance_tests/storage/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/performance_tests/storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      678 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/performance_tests/storage/test_container_open.py
+-rw-r--r--   0 github     (503) staff       (20)      690 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/performance_tests/storage/test_iterative_access.py
+-rw-r--r--   0 github     (503) staff       (20)      802 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/performance_tests/storage/test_random_access.py
+-rw-r--r--   0 github     (503) staff       (20)     1262 2022-06-18 00:13:24.000000 aim-4.0.0.dev4/performance_tests/storage/utils.py
+-rw-r--r--   0 github     (503) staff       (20)       84 2023-03-02 20:49:40.000000 aim-4.0.0.dev4/pyproject.toml
+-rw-r--r--   0 github     (503) staff       (20)      336 2023-04-29 15:33:52.951584 aim-4.0.0.dev4/setup.cfg
+-rw-r--r--   0 github     (503) staff       (20)     6716 2023-03-02 20:49:40.000000 aim-4.0.0.dev4/setup.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.861007 aim-4.0.0.dev4/tests/
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.947152 aim-4.0.0.dev4/tests/api/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/tests/api/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     5155 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/tests/api/test_dashboards_api.py
+-rw-r--r--   0 github     (503) staff       (20)     4335 2022-09-25 12:02:15.000000 aim-4.0.0.dev4/tests/api/test_project_api.py
+-rw-r--r--   0 github     (503) staff       (20)    10653 2023-01-23 10:30:27.000000 aim-4.0.0.dev4/tests/api/test_run_api.py
+-rw-r--r--   0 github     (503) staff       (20)    21533 2023-01-23 10:30:27.000000 aim-4.0.0.dev4/tests/api/test_run_images_api.py
+-rw-r--r--   0 github     (503) staff       (20)    12787 2023-01-23 10:30:27.000000 aim-4.0.0.dev4/tests/api/test_structured_data_api.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.948024 aim-4.0.0.dev4/tests/integrations/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/tests/integrations/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1167 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/tests/integrations/test_dvc_metadata.py
+-rw-r--r--   0 github     (503) staff       (20)     1093 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/tests/integrations/test_hf_datasets.py
+-rw-r--r--   0 github     (503) staff       (20)      961 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/tests/integrations/test_hub_dataset.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.950228 aim-4.0.0.dev4/tests/sdk/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/tests/sdk/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2312 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/tests/sdk/test_image_construction.py
+-rw-r--r--   0 github     (503) staff       (20)     2665 2022-09-25 12:02:15.000000 aim-4.0.0.dev4/tests/sdk/test_resource_tracker.py
+-rw-r--r--   0 github     (503) staff       (20)     1022 2022-11-01 00:13:35.000000 aim-4.0.0.dev4/tests/sdk/test_run_apis.py
+-rw-r--r--   0 github     (503) staff       (20)     1147 2022-09-01 19:23:53.000000 aim-4.0.0.dev4/tests/sdk/test_run_creation_checks.py
+-rw-r--r--   0 github     (503) staff       (20)     1661 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/tests/sdk/test_run_finalization_time.py
+-rw-r--r--   0 github     (503) staff       (20)     1214 2022-11-01 00:13:35.000000 aim-4.0.0.dev4/tests/sdk/test_run_metric_types.py
+-rw-r--r--   0 github     (503) staff       (20)     4631 2022-09-25 12:02:15.000000 aim-4.0.0.dev4/tests/sdk/test_run_track_type_checking.py
+-rw-r--r--   0 github     (503) staff       (20)    10444 2022-09-25 12:02:15.000000 aim-4.0.0.dev4/tests/sdk/test_run_write_container_data.py
+-rw-r--r--   0 github     (503) staff       (20)     4517 2022-06-01 01:05:15.000000 aim-4.0.0.dev4/tests/sdk/test_utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.950944 aim-4.0.0.dev4/tests/storage/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/tests/storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     5677 2022-09-25 12:02:15.000000 aim-4.0.0.dev4/tests/storage/test_query.py
+-rw-r--r--   0 github     (503) staff       (20)     1482 2022-06-18 00:13:24.000000 aim-4.0.0.dev4/tests/storage/test_query_with_epoch_none.py
+-rw-r--r--   0 github     (503) staff       (20)     1342 2022-09-25 12:02:15.000000 aim-4.0.0.dev4/tests/storage/test_structured_db.py
```

### Comparing `aim-4.0.0.dev3/LICENSE` & `aim-4.0.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/PKG-INFO` & `aim-4.0.0.dev4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,40 @@
-Metadata-Version: 2.1
-Name: aim
-Version: 4.0.0.dev3
-Summary: A super-easy way to record, search and compare AI experiments.
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
   <table>
     <tbody>
       <tr>
         <td>Drop a star to support Aim ⭐</td>
         <td>
           <a href="https://community.aimstack.io/">Join Aim discord community</a>
           <img width="20px" src="https://user-images.githubusercontent.com/13848158/226759622-063b725d-8b3e-4c75-80c7-11fb04b7adf5.png">
         </td>
-        <td><a href="#-aim-40">🔮 Aim 4.0 - COMING SOON!!</a></td>
+      </tr>
+      <tr>
+        <td colspan="2"><p align="center"><a href="#-aim-40">🔮 Aim 4.0 - COMING SOON!!</a></p></td>
       </tr>
     </tbody>
   </table>
 </div>
 
+<br />
+
 <div align="center">
   <img src="https://user-images.githubusercontent.com/13848158/225620298-9f9293e9-a138-41fd-bd77-21d53d0490b7.png">
   <h3>
     An easy-to-use & supercharged open-source AI metadata tracker. 
   </h3>
   
-  Aim logs all your AI metadata(**experiments**, **prompts**, etc), enables a UI to compare & observe them and SDK to query them programmatically.
+  Aim logs all your AI metadata, enables a UI to observe/compare them, and an SDK to query them programmatically.
+  
+  <p align="center">
+    <strong>Learn more:</strong> </br>
+    <a href="#experiment-tracking-with-aim">Experiment tracking with Aim</a> </br>
+    <a href="#ai-systems-and-agents-tracing-with-Aim">AI agents tracing with Aim</a>
+  </p>
+  
 </div>
 
 <br/>
 
 <div align="center">
   
   [![Discord Server](https://dcbadge.vercel.app/api/server/zXq2NfVdtF?compact=true&style=flat)](https://community.aimstack.io/)
@@ -109,15 +103,15 @@
 <p align="center">
   AimStack offers enterprise support that's beyond core Aim. Contact via <a href="mailto:hello@aimstack.io">hello@aimstack.io</a> e-mail.
 </p>
 
 ---
 
 <h3 align="center">
-  <a href="#-about"><b>About</b></a> &bull;
+  <a href="#ℹ️-about"><b>About</b></a> &bull;
   <a href="#-demos"><b>Demos</b></a> &bull;
   <a href="#-ecosystem"><b>Ecosystem</b></a> &bull;
   <a href="#-quick-start"><b>Quick Start</b></a> &bull;
   <a href="https://github.com/aimhubio/aim/tree/main/examples"><b>Examples</b></a> &bull;
   <a href="https://aimstack.readthedocs.io/en/latest/"><b>Documentation</b></a> &bull;
   <a href="#-community"><b>Community</b></a> &bull;
   <a href="https://aimstack.io/blog"><b>Blog</b></a> &bull;
@@ -125,32 +119,62 @@
 </h3>  
 
 ---
 
 # ℹ️ About
 
 Aim is an open-source, self-hosted AI Metadata tracking tool designed to handle 100,000s of tracked metadata sequences.
-Two most famous AI metadata applications are: experiment tracking and prompt engineering.
 
-Aim provides a performant and beautiful UI for exploring and comparing training runs, prompt sessions.
+Aim provides a performant and beautiful UI for exploring and comparing metadata such as training runs or agents executions.
 Additionally, its SDK enables programmatic access to tracked metadata — perfect for automations and Jupyter Notebook analysis.
 
 <p align="center">
   <strong>Aim's mission is to democratize AI dev tools 🎯 </strong>
 </p>
 
 <div align="center">
   <img src="https://user-images.githubusercontent.com/13848158/226426018-f7c11c9b-78d9-4ee4-b292-df28b3e8eaa6.jpg" height="140" />
   <img src="https://user-images.githubusercontent.com/13848158/226426005-f7e83923-0f92-44a4-88e4-1735a3d3e119.jpg" height="140" />
   <img src="https://user-images.githubusercontent.com/13848158/226426015-4f1122d8-c96a-443f-8698-3db942b1972a.jpg" height="140" />
 </div>
 
 </br>
 
-<div align="center">
+### AI systems and agents tracing with Aim
+
+<div align="left">
+  <table>
+    <tbody>
+      <tr>
+        <th>Log Inputs, Outputs and Actions of Executions 🤖</th>
+        <th>Visualize & Compare Executions Steps via UI 🔍</th>
+      </tr>
+      <tr>
+        <td>
+          <ul>
+            <li>Track all the inputs, outputs of LLMs and tools</li>
+            <li>Capture terminal output of executions</li>
+            <li>Get notified on executions progress and finish</li>
+            </ul>
+          </td>
+        <td>
+          <ul>
+            <li>Deep dive into single execution steps</li>
+            <li>Compare executions side-by-side</li>
+            <li>View previous exectutions terminal outputs</li>
+          </ul>
+        </td>
+      </tr>
+    </tbody>
+  </table>
+</div>
+
+### Experiment tracking with Aim
+
+<div align="left">
   <table>
     <tbody>
       <tr>
         <th>Log Metadata Across Your ML Pipeline 💾</th>
         <th>Visualize & Compare Metadata via UI 📊</th>
       </tr>
       <tr>
@@ -378,15 +402,15 @@
 
 </br>
 
 **Training run comparison**
 
 Order of magnitude faster training run comparison with Aim
 - The tracked params are first class citizens at Aim. You can search, group, aggregate via params - deeply explore all the tracked data (metrics, params, images) on the UI.
-- With tensorboard the users are forced to record those parameters in the training run name to be able to search and compare. This causes a super-tedius comparison experience and usability issues on the UI when there are many experiments and params. **TensorBoard doesn't have features to group, aggregate the metrics**
+- With tensorboard the users are forced to record those parameters in the training run name to be able to search and compare. This causes a super-tedius comparison experience and usability issues on the UI when there are many experiments and params. **TensorBoard doesn't have features to group, aggregate the metrics**.
 
 **Scalability**
 
 - Aim is built to handle 1000s of training runs - both on the backend and on the UI.
 - TensorBoard becomes really slow and hard to use when a few hundred training runs are queried / compared.
 
 **Beloved TB visualizations to be added on Aim**
@@ -403,20 +427,20 @@
 
 </br>
 
 MLFlow is an end-to-end ML Lifecycle tool.
 Aim is focused on training tracking.
 The main differences of Aim and MLflow are around the UI scalability and run comparison features.
 
-Aim and MLflow are a perfect match - check out the [aimlflow](https://github.com/aimhubio/aimlflow) - the tool that enables Aim supoerpowers on Mlflow.
+Aim and MLflow are a perfect match - check out the [aimlflow](https://github.com/aimhubio/aimlflow) - the tool that enables Aim superpowers on MLflow.
 
 **Run comparison**
 
-- Aim treats tracked parameters as first-class citizens. Users can query runs, metrics, images and filter using the params.
-- MLFlow does have a search by tracked config, but there are no grouping, aggregation, subplotting by hyparparams and other comparison features available.
+- Aim treats tracked parameters as first-class citizens. Users can query runs, metrics, images, and filter using the params.
+- MLFlow does have a search by tracked config, but there are no grouping, aggregation, subplotting by hyperparams and other comparison features available.
 
 **UI Scalability**
 
 - Aim UI can handle several thousands of metrics at the same time smoothly with 1000s of steps. It may get shaky when you explore 1000s of metrics with 10000s of steps each. But we are constantly optimizing!
 - MLflow UI becomes slow to use when there are a few hundreds of runs.
 
 </details>
@@ -427,15 +451,15 @@
 </summary>
 
 </br>
 
 Hosted vs self-hosted
 
 - Weights and Biases is a hosted closed-source MLOps platform.
-- Aim is self-hosted, free and open-source experiment tracking tool.
+- Aim is self-hosted, free, and open-source experiment tracking tool.
 
 </details>
 
 # 🛣️ Roadmap
 
 ## Detailed milestones
```

#### html2text {}

```diff
@@ -1,27 +1,18 @@
-Metadata-Version: 2.1 Name: aim Version: 4.0.0.dev3 Summary: A super-easy way
-to record, search and compare AI experiments. Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
-Python: >=3.7.0 Description-Content-Type: text/markdown License-File: LICENSE
-                       Join_Aim_discord_community
-                       [https://user-
-Drop a star to support images.githubusercontent.com/ ð®_Aim_4.0_-_COMING
-Aim â­             13848158/226759622-063b725d-  SOON!!
-                       8b3e-4c75-80c7-
-                       11fb04b7adf5.png]
+                               Join_Aim_discord_community [https://user-
+Drop a star to support Aim â­images.githubusercontent.com/13848158/226759622-
+                               063b725d-8b3e-4c75-80c7-11fb04b7adf5.png]
+                         ð®_Aim_4.0_-_COMING_SOON!!
+
  [https://user-images.githubusercontent.com/13848158/225620298-9f9293e9-a138-
                           41fd-bd77-21d53d0490b7.png]
    **** An easy-to-use & supercharged open-source AI metadata tracker. ****
-Aim logs all your AI metadata(**experiments**, **prompts**, etc), enables a UI
-       to compare & observe them and SDK to query them programmatically.
+Aim logs all your AI metadata, enables a UI to observe/compare them, and an SDK
+                        to query them programmatically.
+     Learn more:  Experiment_tracking_with_Aim  AI_agents_tracing_with_Aim
 
            [![Discord Server](https://dcbadge.vercel.app/api/server/
 zXq2NfVdtF?compact=true&style=flat)](https://community.aimstack.io/) [![Twitter
 Follow](https://img.shields.io/twitter/follow/aimstackio?style=social)](https:/
    /twitter.com/aimstackio) [![Medium](https://img.shields.io/badge/Medium-
 12100E?style=flat&logo=medium&logoColor=white)](https://medium.com/aimstack) [!
  [Platform Support](https://img.shields.io/badge/platform-Linux%20%7C%20macOS-
@@ -82,25 +73,35 @@
 
     AimStack offers enterprise support that's beyond core Aim. Contact via
                            hello@aimstack.io e-mail.
 ---
    **** About • Demos • Ecosystem • Quick_Start • Examples • Documentation •
                      Community • Blog • COMING_SOON!! ****
 --- # â¹ï¸ About Aim is an open-source, self-hosted AI Metadata tracking tool
-designed to handle 100,000s of tracked metadata sequences. Two most famous AI
-metadata applications are: experiment tracking and prompt engineering. Aim
-provides a performant and beautiful UI for exploring and comparing training
-runs, prompt sessions. Additionally, its SDK enables programmatic access to
-tracked metadata â perfect for automations and Jupyter Notebook analysis.
+designed to handle 100,000s of tracked metadata sequences. Aim provides a
+performant and beautiful UI for exploring and comparing metadata such as
+training runs or agents executions. Additionally, its SDK enables programmatic
+access to tracked metadata â perfect for automations and Jupyter Notebook
+analysis.
                Aim's mission is to democratize AI dev tools ð¯
  [https://user-images.githubusercontent.com/13848158/226426018-f7c11c9b-78d9-
     4ee4-b292-df28b3e8eaa6.jpg] [https://user-images.githubusercontent.com/
   13848158/226426005-f7e83923-0f92-44a4-88e4-1735a3d3e119.jpg] [https://user-
    images.githubusercontent.com/13848158/226426015-4f1122d8-c96a-443f-8698-
                                3db942b1972a.jpg]
+ ### AI systems and agents tracing with Aim
+Log Inputs, Outputs and Actions of     Visualize & Compare Executions Steps via
+Executions ð¤                    UI ð
+    * Track all the inputs, outputs of     * Deep dive into single execution
+      LLMs and tools                         steps
+    * Capture terminal output of           * Compare executions side-by-side
+      executions                           * View previous exectutions terminal
+    * Get notified on executions             outputs
+      progress and finish
+### Experiment tracking with Aim
 Log Metadata Across Your ML Pipeline  Visualize & Compare Metadata via UI ð
 ð¾
     * ML experiments and any metadata
       tracking                            * Metadata visualization via Aim
     * Integration with popular ML           Explorers
       frameworks                          * Grouping and aggregation
     * Easy migration from other           * Querying using Python expressions
@@ -211,33 +212,33 @@
 comparison** Order of magnitude faster training run comparison with Aim - The
 tracked params are first class citizens at Aim. You can search, group,
 aggregate via params - deeply explore all the tracked data (metrics, params,
 images) on the UI. - With tensorboard the users are forced to record those
 parameters in the training run name to be able to search and compare. This
 causes a super-tedius comparison experience and usability issues on the UI when
 there are many experiments and params. **TensorBoard doesn't have features to
-group, aggregate the metrics** **Scalability** - Aim is built to handle 1000s
+group, aggregate the metrics**. **Scalability** - Aim is built to handle 1000s
 of training runs - both on the backend and on the UI. - TensorBoard becomes
 really slow and hard to use when a few hundred training runs are queried /
 compared. **Beloved TB visualizations to be added on Aim** - Embedding
 projector. - Neural network visualization.    MLflow vs Aim   MLFlow is an end-
 to-end ML Lifecycle tool. Aim is focused on training tracking. The main
 differences of Aim and MLflow are around the UI scalability and run comparison
 features. Aim and MLflow are a perfect match - check out the [aimlflow](https:/
-/github.com/aimhubio/aimlflow) - the tool that enables Aim supoerpowers on
-Mlflow. **Run comparison** - Aim treats tracked parameters as first-class
-citizens. Users can query runs, metrics, images and filter using the params. -
+/github.com/aimhubio/aimlflow) - the tool that enables Aim superpowers on
+MLflow. **Run comparison** - Aim treats tracked parameters as first-class
+citizens. Users can query runs, metrics, images, and filter using the params. -
 MLFlow does have a search by tracked config, but there are no grouping,
-aggregation, subplotting by hyparparams and other comparison features
+aggregation, subplotting by hyperparams and other comparison features
 available. **UI Scalability** - Aim UI can handle several thousands of metrics
 at the same time smoothly with 1000s of steps. It may get shaky when you
 explore 1000s of metrics with 10000s of steps each. But we are constantly
 optimizing! - MLflow UI becomes slow to use when there are a few hundreds of
 runs.    Weights and Biases vs Aim   Hosted vs self-hosted - Weights and Biases
-is a hosted closed-source MLOps platform. - Aim is self-hosted, free and open-
+is a hosted closed-source MLOps platform. - Aim is self-hosted, free, and open-
 source experiment tracking tool.  # ð£ï¸ Roadmap ## Detailed milestones The
 [Aim product roadmap](https://github.com/orgs/aimhubio/projects/3) :sparkle: -
 The `Backlog` contains the issues we are going to choose from and prioritize
 weekly - The issues are mainly prioritized by the highly-requested features ##
 High-level roadmap The high-level features we are going to work on the next few
 months: **In progress** - [ ] Aim SDK low-level interface - [ ] Dashboards â
 customizable layouts with embedded explorers - [ ] Ergonomic UI kit - [ ] Text
```

### Comparing `aim-4.0.0.dev3/README.md` & `aim-4.0.0.dev4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,57 @@
+Metadata-Version: 2.1
+Name: aim
+Version: 4.0.0.dev4
+Summary: A super-easy way to record, search and compare AI experiments.
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
   <table>
     <tbody>
       <tr>
         <td>Drop a star to support Aim ⭐</td>
         <td>
           <a href="https://community.aimstack.io/">Join Aim discord community</a>
           <img width="20px" src="https://user-images.githubusercontent.com/13848158/226759622-063b725d-8b3e-4c75-80c7-11fb04b7adf5.png">
         </td>
-        <td><a href="#-aim-40">🔮 Aim 4.0 - COMING SOON!!</a></td>
+      </tr>
+      <tr>
+        <td colspan="2"><p align="center"><a href="#-aim-40">🔮 Aim 4.0 - COMING SOON!!</a></p></td>
       </tr>
     </tbody>
   </table>
 </div>
 
+<br />
+
 <div align="center">
   <img src="https://user-images.githubusercontent.com/13848158/225620298-9f9293e9-a138-41fd-bd77-21d53d0490b7.png">
   <h3>
     An easy-to-use & supercharged open-source AI metadata tracker. 
   </h3>
   
-  Aim logs all your AI metadata(**experiments**, **prompts**, etc), enables a UI to compare & observe them and SDK to query them programmatically.
+  Aim logs all your AI metadata, enables a UI to observe/compare them, and an SDK to query them programmatically.
+  
+  <p align="center">
+    <strong>Learn more:</strong> </br>
+    <a href="#experiment-tracking-with-aim">Experiment tracking with Aim</a> </br>
+    <a href="#ai-systems-and-agents-tracing-with-Aim">AI agents tracing with Aim</a>
+  </p>
+  
 </div>
 
 <br/>
 
 <div align="center">
   
   [![Discord Server](https://dcbadge.vercel.app/api/server/zXq2NfVdtF?compact=true&style=flat)](https://community.aimstack.io/)
@@ -92,15 +120,15 @@
 <p align="center">
   AimStack offers enterprise support that's beyond core Aim. Contact via <a href="mailto:hello@aimstack.io">hello@aimstack.io</a> e-mail.
 </p>
 
 ---
 
 <h3 align="center">
-  <a href="#-about"><b>About</b></a> &bull;
+  <a href="#ℹ️-about"><b>About</b></a> &bull;
   <a href="#-demos"><b>Demos</b></a> &bull;
   <a href="#-ecosystem"><b>Ecosystem</b></a> &bull;
   <a href="#-quick-start"><b>Quick Start</b></a> &bull;
   <a href="https://github.com/aimhubio/aim/tree/main/examples"><b>Examples</b></a> &bull;
   <a href="https://aimstack.readthedocs.io/en/latest/"><b>Documentation</b></a> &bull;
   <a href="#-community"><b>Community</b></a> &bull;
   <a href="https://aimstack.io/blog"><b>Blog</b></a> &bull;
@@ -108,32 +136,62 @@
 </h3>  
 
 ---
 
 # ℹ️ About
 
 Aim is an open-source, self-hosted AI Metadata tracking tool designed to handle 100,000s of tracked metadata sequences.
-Two most famous AI metadata applications are: experiment tracking and prompt engineering.
 
-Aim provides a performant and beautiful UI for exploring and comparing training runs, prompt sessions.
+Aim provides a performant and beautiful UI for exploring and comparing metadata such as training runs or agents executions.
 Additionally, its SDK enables programmatic access to tracked metadata — perfect for automations and Jupyter Notebook analysis.
 
 <p align="center">
   <strong>Aim's mission is to democratize AI dev tools 🎯 </strong>
 </p>
 
 <div align="center">
   <img src="https://user-images.githubusercontent.com/13848158/226426018-f7c11c9b-78d9-4ee4-b292-df28b3e8eaa6.jpg" height="140" />
   <img src="https://user-images.githubusercontent.com/13848158/226426005-f7e83923-0f92-44a4-88e4-1735a3d3e119.jpg" height="140" />
   <img src="https://user-images.githubusercontent.com/13848158/226426015-4f1122d8-c96a-443f-8698-3db942b1972a.jpg" height="140" />
 </div>
 
 </br>
 
-<div align="center">
+### AI systems and agents tracing with Aim
+
+<div align="left">
+  <table>
+    <tbody>
+      <tr>
+        <th>Log Inputs, Outputs and Actions of Executions 🤖</th>
+        <th>Visualize & Compare Executions Steps via UI 🔍</th>
+      </tr>
+      <tr>
+        <td>
+          <ul>
+            <li>Track all the inputs, outputs of LLMs and tools</li>
+            <li>Capture terminal output of executions</li>
+            <li>Get notified on executions progress and finish</li>
+            </ul>
+          </td>
+        <td>
+          <ul>
+            <li>Deep dive into single execution steps</li>
+            <li>Compare executions side-by-side</li>
+            <li>View previous exectutions terminal outputs</li>
+          </ul>
+        </td>
+      </tr>
+    </tbody>
+  </table>
+</div>
+
+### Experiment tracking with Aim
+
+<div align="left">
   <table>
     <tbody>
       <tr>
         <th>Log Metadata Across Your ML Pipeline 💾</th>
         <th>Visualize & Compare Metadata via UI 📊</th>
       </tr>
       <tr>
@@ -361,15 +419,15 @@
 
 </br>
 
 **Training run comparison**
 
 Order of magnitude faster training run comparison with Aim
 - The tracked params are first class citizens at Aim. You can search, group, aggregate via params - deeply explore all the tracked data (metrics, params, images) on the UI.
-- With tensorboard the users are forced to record those parameters in the training run name to be able to search and compare. This causes a super-tedius comparison experience and usability issues on the UI when there are many experiments and params. **TensorBoard doesn't have features to group, aggregate the metrics**
+- With tensorboard the users are forced to record those parameters in the training run name to be able to search and compare. This causes a super-tedius comparison experience and usability issues on the UI when there are many experiments and params. **TensorBoard doesn't have features to group, aggregate the metrics**.
 
 **Scalability**
 
 - Aim is built to handle 1000s of training runs - both on the backend and on the UI.
 - TensorBoard becomes really slow and hard to use when a few hundred training runs are queried / compared.
 
 **Beloved TB visualizations to be added on Aim**
@@ -386,20 +444,20 @@
 
 </br>
 
 MLFlow is an end-to-end ML Lifecycle tool.
 Aim is focused on training tracking.
 The main differences of Aim and MLflow are around the UI scalability and run comparison features.
 
-Aim and MLflow are a perfect match - check out the [aimlflow](https://github.com/aimhubio/aimlflow) - the tool that enables Aim supoerpowers on Mlflow.
+Aim and MLflow are a perfect match - check out the [aimlflow](https://github.com/aimhubio/aimlflow) - the tool that enables Aim superpowers on MLflow.
 
 **Run comparison**
 
-- Aim treats tracked parameters as first-class citizens. Users can query runs, metrics, images and filter using the params.
-- MLFlow does have a search by tracked config, but there are no grouping, aggregation, subplotting by hyparparams and other comparison features available.
+- Aim treats tracked parameters as first-class citizens. Users can query runs, metrics, images, and filter using the params.
+- MLFlow does have a search by tracked config, but there are no grouping, aggregation, subplotting by hyperparams and other comparison features available.
 
 **UI Scalability**
 
 - Aim UI can handle several thousands of metrics at the same time smoothly with 1000s of steps. It may get shaky when you explore 1000s of metrics with 10000s of steps each. But we are constantly optimizing!
 - MLflow UI becomes slow to use when there are a few hundreds of runs.
 
 </details>
@@ -410,15 +468,15 @@
 </summary>
 
 </br>
 
 Hosted vs self-hosted
 
 - Weights and Biases is a hosted closed-source MLOps platform.
-- Aim is self-hosted, free and open-source experiment tracking tool.
+- Aim is self-hosted, free, and open-source experiment tracking tool.
 
 </details>
 
 # 🛣️ Roadmap
 
 ## Detailed milestones
```

#### html2text {}

```diff
@@ -1,18 +1,27 @@
-                       Join_Aim_discord_community
-                       [https://user-
-Drop a star to support images.githubusercontent.com/ ð®_Aim_4.0_-_COMING
-Aim â­             13848158/226759622-063b725d-  SOON!!
-                       8b3e-4c75-80c7-
-                       11fb04b7adf5.png]
+Metadata-Version: 2.1 Name: aim Version: 4.0.0.dev4 Summary: A super-easy way
+to record, search and compare AI experiments. Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
+Python: >=3.7.0 Description-Content-Type: text/markdown License-File: LICENSE
+                               Join_Aim_discord_community [https://user-
+Drop a star to support Aim â­images.githubusercontent.com/13848158/226759622-
+                               063b725d-8b3e-4c75-80c7-11fb04b7adf5.png]
+                         ð®_Aim_4.0_-_COMING_SOON!!
+
  [https://user-images.githubusercontent.com/13848158/225620298-9f9293e9-a138-
                           41fd-bd77-21d53d0490b7.png]
    **** An easy-to-use & supercharged open-source AI metadata tracker. ****
-Aim logs all your AI metadata(**experiments**, **prompts**, etc), enables a UI
-       to compare & observe them and SDK to query them programmatically.
+Aim logs all your AI metadata, enables a UI to observe/compare them, and an SDK
+                        to query them programmatically.
+     Learn more:  Experiment_tracking_with_Aim  AI_agents_tracing_with_Aim
 
            [![Discord Server](https://dcbadge.vercel.app/api/server/
 zXq2NfVdtF?compact=true&style=flat)](https://community.aimstack.io/) [![Twitter
 Follow](https://img.shields.io/twitter/follow/aimstackio?style=social)](https:/
    /twitter.com/aimstackio) [![Medium](https://img.shields.io/badge/Medium-
 12100E?style=flat&logo=medium&logoColor=white)](https://medium.com/aimstack) [!
  [Platform Support](https://img.shields.io/badge/platform-Linux%20%7C%20macOS-
@@ -73,25 +82,35 @@
 
     AimStack offers enterprise support that's beyond core Aim. Contact via
                            hello@aimstack.io e-mail.
 ---
    **** About • Demos • Ecosystem • Quick_Start • Examples • Documentation •
                      Community • Blog • COMING_SOON!! ****
 --- # â¹ï¸ About Aim is an open-source, self-hosted AI Metadata tracking tool
-designed to handle 100,000s of tracked metadata sequences. Two most famous AI
-metadata applications are: experiment tracking and prompt engineering. Aim
-provides a performant and beautiful UI for exploring and comparing training
-runs, prompt sessions. Additionally, its SDK enables programmatic access to
-tracked metadata â perfect for automations and Jupyter Notebook analysis.
+designed to handle 100,000s of tracked metadata sequences. Aim provides a
+performant and beautiful UI for exploring and comparing metadata such as
+training runs or agents executions. Additionally, its SDK enables programmatic
+access to tracked metadata â perfect for automations and Jupyter Notebook
+analysis.
                Aim's mission is to democratize AI dev tools ð¯
  [https://user-images.githubusercontent.com/13848158/226426018-f7c11c9b-78d9-
     4ee4-b292-df28b3e8eaa6.jpg] [https://user-images.githubusercontent.com/
   13848158/226426005-f7e83923-0f92-44a4-88e4-1735a3d3e119.jpg] [https://user-
    images.githubusercontent.com/13848158/226426015-4f1122d8-c96a-443f-8698-
                                3db942b1972a.jpg]
+ ### AI systems and agents tracing with Aim
+Log Inputs, Outputs and Actions of     Visualize & Compare Executions Steps via
+Executions ð¤                    UI ð
+    * Track all the inputs, outputs of     * Deep dive into single execution
+      LLMs and tools                         steps
+    * Capture terminal output of           * Compare executions side-by-side
+      executions                           * View previous exectutions terminal
+    * Get notified on executions             outputs
+      progress and finish
+### Experiment tracking with Aim
 Log Metadata Across Your ML Pipeline  Visualize & Compare Metadata via UI ð
 ð¾
     * ML experiments and any metadata
       tracking                            * Metadata visualization via Aim
     * Integration with popular ML           Explorers
       frameworks                          * Grouping and aggregation
     * Easy migration from other           * Querying using Python expressions
@@ -202,33 +221,33 @@
 comparison** Order of magnitude faster training run comparison with Aim - The
 tracked params are first class citizens at Aim. You can search, group,
 aggregate via params - deeply explore all the tracked data (metrics, params,
 images) on the UI. - With tensorboard the users are forced to record those
 parameters in the training run name to be able to search and compare. This
 causes a super-tedius comparison experience and usability issues on the UI when
 there are many experiments and params. **TensorBoard doesn't have features to
-group, aggregate the metrics** **Scalability** - Aim is built to handle 1000s
+group, aggregate the metrics**. **Scalability** - Aim is built to handle 1000s
 of training runs - both on the backend and on the UI. - TensorBoard becomes
 really slow and hard to use when a few hundred training runs are queried /
 compared. **Beloved TB visualizations to be added on Aim** - Embedding
 projector. - Neural network visualization.    MLflow vs Aim   MLFlow is an end-
 to-end ML Lifecycle tool. Aim is focused on training tracking. The main
 differences of Aim and MLflow are around the UI scalability and run comparison
 features. Aim and MLflow are a perfect match - check out the [aimlflow](https:/
-/github.com/aimhubio/aimlflow) - the tool that enables Aim supoerpowers on
-Mlflow. **Run comparison** - Aim treats tracked parameters as first-class
-citizens. Users can query runs, metrics, images and filter using the params. -
+/github.com/aimhubio/aimlflow) - the tool that enables Aim superpowers on
+MLflow. **Run comparison** - Aim treats tracked parameters as first-class
+citizens. Users can query runs, metrics, images, and filter using the params. -
 MLFlow does have a search by tracked config, but there are no grouping,
-aggregation, subplotting by hyparparams and other comparison features
+aggregation, subplotting by hyperparams and other comparison features
 available. **UI Scalability** - Aim UI can handle several thousands of metrics
 at the same time smoothly with 1000s of steps. It may get shaky when you
 explore 1000s of metrics with 10000s of steps each. But we are constantly
 optimizing! - MLflow UI becomes slow to use when there are a few hundreds of
 runs.    Weights and Biases vs Aim   Hosted vs self-hosted - Weights and Biases
-is a hosted closed-source MLOps platform. - Aim is self-hosted, free and open-
+is a hosted closed-source MLOps platform. - Aim is self-hosted, free, and open-
 source experiment tracking tool.  # ð£ï¸ Roadmap ## Detailed milestones The
 [Aim product roadmap](https://github.com/orgs/aimhubio/projects/3) :sparkle: -
 The `Backlog` contains the issues we are going to choose from and prioritize
 weekly - The issues are mainly prioritized by the highly-requested features ##
 High-level roadmap The high-level features we are going to work on the next few
 months: **In progress** - [ ] Aim SDK low-level interface - [ ] Dashboards â
 customizable layouts with embedded explorers - [ ] Ergonomic UI kit - [ ] Text
```

### Comparing `aim-4.0.0.dev3/aim/__about__.py` & `aim-4.0.0.dev4/aim/__about__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/cli.py` & `aim-4.0.0.dev4/aim/cli/cli.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/convert/commands.py` & `aim-4.0.0.dev4/aim/cli/convert/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/convert/processors/mlflow.py` & `aim-4.0.0.dev4/aim/cli/convert/processors/mlflow.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/convert/processors/tensorboard.py` & `aim-4.0.0.dev4/aim/cli/convert/processors/tensorboard.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/convert/processors/wandb.py` & `aim-4.0.0.dev4/aim/cli/convert/processors/wandb.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/init/commands.py` & `aim-4.0.0.dev4/aim/cli/init/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/manager/manager.py` & `aim-4.0.0.dev4/aim/cli/manager/manager.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/reindex/commands.py` & `aim-4.0.0.dev4/aim/cli/reindex/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/runs/commands.py` & `aim-4.0.0.dev4/aim/cli/runs/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/runs/utils.py` & `aim-4.0.0.dev4/aim/cli/runs/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/server/commands.py` & `aim-4.0.0.dev4/aim/cli/server/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/storage/commands.py` & `aim-4.0.0.dev4/aim/cli/storage/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/up/commands.py` & `aim-4.0.0.dev4/aim/cli/up/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/up/utils.py` & `aim-4.0.0.dev4/aim/cli/up/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/configs.py` & `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/configs.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v3/base_pb2.py` & `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v3/base_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v3/metric_pb2.py` & `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v3/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v4/base_pb2.py` & `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v4/base_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/proto/v4/metric_pb2.py` & `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v4/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/metric.py` & `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/metric.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/repo.py` & `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/repo.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/run.py` & `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/trace.py` & `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/trace.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/upgrade/_legacy_repo/repo/utils.py` & `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/upgrade/utils.py` & `aim-4.0.0.dev4/aim/cli/upgrade/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/cli/watcher_cli.py` & `aim-4.0.0.dev4/aim/cli/watcher_cli.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/cleanup/__init__.py` & `aim-4.0.0.dev4/aim/ext/cleanup/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/exception_resistant.py` & `aim-4.0.0.dev4/aim/ext/exception_resistant.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/notebook/notebook.py` & `aim-4.0.0.dev4/aim/ext/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/notifier/__init__.py` & `aim-4.0.0.dev4/aim/ext/notifier/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/notifier/config.py` & `aim-4.0.0.dev4/aim/ext/notifier/config.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/notifier/logging_notifier.py` & `aim-4.0.0.dev4/aim/ext/notifier/logging_notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/notifier/notifier.py` & `aim-4.0.0.dev4/aim/ext/notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/notifier/notifier_builder.py` & `aim-4.0.0.dev4/aim/ext/notifier/notifier_builder.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/notifier/slack_notifier.py` & `aim-4.0.0.dev4/aim/ext/notifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/notifier/utils.py` & `aim-4.0.0.dev4/aim/ext/notifier/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/notifier/workplace_notifier.py` & `aim-4.0.0.dev4/aim/ext/notifier/workplace_notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/resource/log.py` & `aim-4.0.0.dev4/aim/ext/resource/log.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/resource/stat.py` & `aim-4.0.0.dev4/aim/ext/resource/stat.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/resource/tracker.py` & `aim-4.0.0.dev4/aim/ext/resource/tracker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/sshfs/utils.py` & `aim-4.0.0.dev4/aim/ext/sshfs/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/task_queue/queue.py` & `aim-4.0.0.dev4/aim/ext/task_queue/queue.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/tensorboard_tracker/run.py` & `aim-4.0.0.dev4/aim/ext/tensorboard_tracker/run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/tensorboard_tracker/tracker.py` & `aim-4.0.0.dev4/aim/ext/tensorboard_tracker/tracker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/client.py` & `aim-4.0.0.dev4/aim/ext/transport/client.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/config.py` & `aim-4.0.0.dev4/aim/ext/transport/config.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/handlers.py` & `aim-4.0.0.dev4/aim/ext/transport/handlers.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/health.py` & `aim-4.0.0.dev4/aim/ext/transport/health.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/heartbeat.py` & `aim-4.0.0.dev4/aim/ext/transport/heartbeat.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/message_utils.py` & `aim-4.0.0.dev4/aim/ext/transport/message_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/proto/health_pb2_grpc.py` & `aim-4.0.0.dev4/aim/ext/transport/proto/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/proto/remote_router_pb2_grpc.py` & `aim-4.0.0.dev4/aim/ext/transport/proto/remote_router_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/proto/remote_tracking_pb2_grpc.py` & `aim-4.0.0.dev4/aim/ext/transport/proto/remote_tracking_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/proto/v3/health_pb2.py` & `aim-4.0.0.dev4/aim/ext/transport/proto/v3/health_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/proto/v3/remote_router_pb2.py` & `aim-4.0.0.dev4/aim/ext/transport/proto/v3/remote_router_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/proto/v3/remote_tracking_pb2.py` & `aim-4.0.0.dev4/aim/ext/transport/proto/v3/remote_tracking_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/proto/v4/health_pb2.py` & `aim-4.0.0.dev4/aim/ext/transport/proto/v4/health_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/proto/v4/remote_router_pb2.py` & `aim-4.0.0.dev4/aim/ext/transport/proto/v4/remote_router_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/proto/v4/remote_tracking_pb2.py` & `aim-4.0.0.dev4/aim/ext/transport/proto/v4/remote_tracking_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/remote_tracking.py` & `aim-4.0.0.dev4/aim/ext/transport/remote_tracking.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/router.py` & `aim-4.0.0.dev4/aim/ext/transport/router.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/rpc_queue.py` & `aim-4.0.0.dev4/aim/ext/transport/rpc_queue.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/server.py` & `aim-4.0.0.dev4/aim/ext/transport/server.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/transport/worker.py` & `aim-4.0.0.dev4/aim/ext/transport/worker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/ext/utils.py` & `aim-4.0.0.dev4/aim/ext/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/__init__.py` & `aim-4.0.0.dev4/aim/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/adapters/acme.py` & `aim-4.0.0.dev4/aim/sdk/adapters/acme.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 from typing import Optional, Dict
 from aim.sdk.run import Run
 from aim.ext.resource.configs import DEFAULT_SYSTEM_TRACKING_INT
 from acme.utils.loggers.base import Logger, LoggingData
 
 
 class AimCallback:
+    """
+    AimCallback callback class.
+
+    Args:
+        repo (:obj:`str`, optional): Aim repository path or Repo object to which Run object is bound.
+            If skipped, default Repo is used.
+        experiment_name (:obj:`str`, optional): Sets Run's `experiment` property. 'default' if not specified.
+            Can be used later to query runs/sequences.
+        system_tracking_interval (:obj:`int`, optional): Sets the tracking interval in seconds for system usage
+            metrics (CPU, Memory, etc.). Set to `None` to disable system metrics tracking.
+        log_system_params (:obj:`bool`, optional): Enable/Disable logging of system params such as installed packages,
+            git info, environment variables, etc.
+        capture_terminal_logs (:obj:`bool`, optional): Enable/Disable terminal stdout logging.
+        args (:obj:`dict`, optional): Arguments to set a run parameters
+    """
+
     def __init__(
         self,
         repo: Optional[str] = None,
         experiment_name: Optional[str] = None,
         system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
         log_system_params: Optional[bool] = True,
         capture_terminal_logs: Optional[bool] = True,
@@ -66,12 +82,12 @@
     def __init__(self, aim_run, logger_label, steps_key, task_id):
         self.aim_run = aim_run
         self.logger_label = logger_label
         self.steps_key = steps_key
         self.task_id = task_id
 
     def write(self, values: LoggingData):
-        self.aim_run.track(values, context={"logger_label": self.logger_label})
+        self.aim_run.track(values, context={'logger_label': self.logger_label})
 
     def close(self):
         if self.aim_run and self.aim_run.active:
             self.aim_run.close()
```

### Comparing `aim-4.0.0.dev3/aim/sdk/adapters/catboost.py` & `aim-4.0.0.dev4/aim/sdk/adapters/prophet.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,64 @@
-from sys import stdout
-from typing import Optional
+from typing import Any, Dict, Optional, TypeVar
 
 from aim import Run
 from aim.ext.resource import DEFAULT_SYSTEM_TRACKING_INT
+from aim.storage.types import AimObject
+
+Prophet = TypeVar('Prophet')
 
 
 class AimLogger:
+    """
+    AimLogger logger class.
+
+    Prophet doesn't have a callback system and isn't trained iteratively.
+    Thus, only the hyperparameters and user-provided metrics are logged.
 
-    def __init__(self, loss_function: Optional[str] = "Loss",
-                 repo: Optional[str] = None,
-                 experiment: Optional[str] = None,
-                 system_tracking_interval: Optional[int]
-                 = DEFAULT_SYSTEM_TRACKING_INT,
-                 log_system_params: Optional[bool] = True,
-                 capture_terminal_logs: Optional[bool] = True,
-                 log_cout=stdout):
-        super().__init__()
-        self._loss_function = loss_function
+    Args:
+        repo (:obj:`str`, optional): Aim repository path or Repo object to which Run object is bound.
+            If skipped, default Repo is used.
+        experiment_name (:obj:`str`, optional): Sets Run's `experiment` property. 'default' if not specified.
+            Can be used later to query runs/sequences.
+        system_tracking_interval (:obj:`int`, optional): Sets the tracking interval in seconds for system usage
+            metrics (CPU, Memory, etc.). Set to `None` to disable system metrics tracking.
+        log_system_params (:obj:`bool`, optional): Enable/Disable logging of system params such as installed packages,
+            git info, environment variables, etc.
+        capture_terminal_logs (:obj:`bool`, optional): Enable/Disable terminal stdout logging.
+        prophet_model (:obj: `Any`, optional): An instance of Prophet model.
+    """
+
+    def __init__(
+        self,
+        repo: Optional[str] = None,
+        experiment_name: Optional[str] = None,
+        system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
+        log_system_params: Optional[bool] = True,
+        capture_terminal_logs: Optional[bool] = True,
+        prophet_model: Prophet = None,
+    ):
         self._repo_path = repo
-        self._experiment = experiment
+        self._experiment = experiment_name
         self._system_tracking_interval = system_tracking_interval
         self._log_system_params = log_system_params
         self._capture_terminal_logs = capture_terminal_logs
         self._run = None
         self._run_hash = None
-        self._log_cout = log_cout
-
-        if log_cout is not None:
-            assert hasattr(log_cout, "write")
+        self.setup(prophet_model.__dict__)
 
     @property
     def experiment(self) -> Run:
         if not self._run:
             self.setup()
         return self._run
 
-    def setup(self):
+    def setup(self, hparams: Dict[str, Any]) -> None:
+        """
+        Sets up a Run and logs hyperparameters (this method is only used in the constructor).
+        """
         if self._run:
             return
         if self._run_hash:
             self._run = Run(
                 self._run_hash,
                 repo=self._repo_path,
                 system_tracking_interval=self._system_tracking_interval,
@@ -51,48 +70,29 @@
                 experiment=self._experiment,
                 system_tracking_interval=self._system_tracking_interval,
                 log_system_params=self._log_system_params,
                 capture_terminal_logs=self._capture_terminal_logs,
             )
             self._run_hash = self._run.hash
 
-    def _to_number(self, val):
-        try:
-            return float(val)
-        except ValueError:
-            return val
-
-    def write(self, log):
-        run = self.experiment
-
-        _log = log
-        log = log.strip().split()
-        if log:
-            if len(log) == 3 and log[1] == '=':
-                run[log[0]] = self._to_number(log[2])
-                return
-
-            value_learn = None
-            value_iter = None
-            value_test = None
-            value_best = None
-
-            if log[1] == 'learn:':
-                value_iter = int(log[0][:-1])
-                value_learn = self._to_number(log[2])
-                if log[3] == 'test:':
-                    value_test = self._to_number(log[4])
-                    if log[5] == 'best:':
-                        value_best = self._to_number(log[6])
-            if any((value_learn, value_test, value_best)):
-                if value_learn:
-                    run.track(value_learn, name=self._loss_function, step=value_iter, context={'log': 'learn'})
-                if value_test:
-                    run.track(value_test, name=self._loss_function, step=value_iter, context={'log': 'test'})
-                if value_best:
-                    run.track(value_best, name=self._loss_function, step=value_iter, context={'log': 'best'})
-            else:
-                # Unhandled or junky log
-                pass
+        for hparam, value in hparams.items():
+            self._run.set(hparam, value, strict=False)
 
-        if self._log_cout:
-            self._log_cout.write(_log)
+    def __del__(self) -> None:
+        if self._run and self._run.active:
+            self._run.close()
+
+    def track_metrics(
+        self,
+        metrics: Dict[str, float],
+        context: AimObject = None,
+    ) -> None:
+        """
+        Since Prophet doesn't compute loss during training,
+        only hyperparameters are logged by default.
+        This method can be used to log any user-provied metrics.
+        NOTE: if context is not provided, it's assumed all metrics are validation metrics.
+        """
+        if context is None:
+            context = {'subset': 'val'}
+        for metric, value in metrics.items():
+            self._run.track(value, name=metric, context=context)
```

### Comparing `aim-4.0.0.dev3/aim/sdk/adapters/fastai.py` & `aim-4.0.0.dev4/aim/sdk/adapters/fastai.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,21 +14,37 @@
         'Please install it with command: \n pip install fastai'
     )
 
 logger = getLogger(__name__)
 
 
 class AimCallback(Callback):
-    def __init__(self,
-                 repo: Optional[str] = None,
-                 experiment_name: Optional[str] = None,
-                 system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
-                 log_system_params: [bool] = True,
-                 capture_terminal_logs: Optional[bool] = True,
-                 ):
+    """
+    AimCallback callback class.
+
+    Args:
+        repo (:obj:`str`, optional): Aim repository path or Repo object to which Run object is bound.
+            If skipped, default Repo is used.
+        experiment_name (:obj:`str`, optional): Sets Run's `experiment` property. 'default' if not specified.
+            Can be used later to query runs/sequences.
+        system_tracking_interval (:obj:`int`, optional): Sets the tracking interval in seconds for system usage
+            metrics (CPU, Memory, etc.). Set to `None` to disable system metrics tracking.
+        log_system_params (:obj:`bool`, optional): Enable/Disable logging of system params such as installed packages,
+            git info, environment variables, etc.
+        capture_terminal_logs (:obj:`bool`, optional): Enable/Disable terminal stdout logging.
+    """
+
+    def __init__(
+        self,
+        repo: Optional[str] = None,
+        experiment_name: Optional[str] = None,
+        system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
+        log_system_params: Optional[bool] = True,
+        capture_terminal_logs: Optional[bool] = True,
+    ):
         store_attr()
         self.repo = repo
         self.experiment_name = experiment_name
         self.system_tracking_interval = system_tracking_interval
         self.log_system_params = log_system_params
         self.capture_terminal_logs = capture_terminal_logs
         self._run = None
@@ -73,15 +89,17 @@
             configs_log = self.gather_args()
             formatted_config = AimCallback.format_config(configs_log)
             self.setup(formatted_config)
 
     def after_batch(self):
         context = {'subset': 'train'} if self.training else {'subset': 'val'}
 
-        self._run.track(self.loss.item(), name='train_loss', step=self.train_iter, context=context)
+        self._run.track(
+            self.loss.item(), name='train_loss', step=self.train_iter, context=context
+        )
         for i, h in enumerate(self.opt.hypers):
             for k, v in h.items():
                 self._run.track(v, f'{k}_{i}', step=self.train_iter, context=context)
 
     def before_epoch(self):
         for metric in self.metrics:
             metric.reset()
@@ -92,25 +110,34 @@
                 self._run.track(value, name=name)
 
     def __del__(self):
         if self._run and self._run.active:
             self._run.close()
 
     def gather_args(self):
-        "Gather config parameters accessible to the learner"
+        'Gather config parameters accessible to the learner'
         # args stored by 'store_attr'
-        cb_args = {f'{cb}': getattr(cb, '__stored_args__', True) for cb in self.cbs if cb != self}
+        cb_args = {
+            f'{cb}': getattr(cb, '__stored_args__', True)
+            for cb in self.cbs
+            if cb != self
+        }
         args = {'Learner': self.learn, **cb_args}
         # input dim
         try:
             n_inp = self.dls.train.n_inp
             args['n_inp'] = n_inp
             xb = self.dls.valid.one_batch()[:n_inp]
-            args.update({f'input {n+1} dim {i+1}': d for n in range(n_inp)
-                        for i, d in enumerate(list(detuplify(xb[n]).shape))})
+            args.update(
+                {
+                    f'input {n+1} dim {i+1}': d
+                    for n in range(n_inp)
+                    for i, d in enumerate(list(detuplify(xb[n]).shape))
+                }
+            )
         except Exception:
             logger.warning('Failed to gather input dimensions')
         # other args
         with ignore_exceptions():
             args['batch_size'] = self.dls.bs
             args['batch_per_epoch'] = len(self.dls.train)
             args['model_parameters'] = total_params(self.model)[0]
@@ -121,15 +148,15 @@
             args['dls', 'after_item'] = f'{self.dls.after_item}'
             args['dls', 'before_batch'] = f'{self.dls.before_batch}'
             args['dls', 'after_batch'] = f'{self.dls.after_batch}'
         return args
 
     @classmethod
     def format_config(cls, config):
-        "Format config parameters for logging"
+        'Format config parameters for logging'
         for key, value in config.items():
             if isinstance(value, dict):
                 config[key] = AimCallback.format_config(value)
             else:
                 config[key] = AimCallback.format_config_value(value)
         return config
```

### Comparing `aim-4.0.0.dev3/aim/sdk/adapters/hugging_face.py` & `aim-4.0.0.dev4/aim/sdk/adapters/hugging_face.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,24 +15,39 @@
         'Please install it with command: \n pip install transformers'
     )
 
 logger = getLogger(__name__)
 
 
 class AimCallback(TrainerCallback):
+    """
+    AimCallback callback class.
+
+    Args:
+        repo (:obj:`str`, optional): Aim repository path or Repo object to which Run object is bound.
+            If skipped, default Repo is used.
+        experiment_name (:obj:`str`, optional): Sets Run's `experiment` property. 'default' if not specified.
+            Can be used later to query runs/sequences.
+        system_tracking_interval (:obj:`int`, optional): Sets the tracking interval in seconds for system usage
+            metrics (CPU, Memory, etc.). Set to `None` to disable system metrics tracking.
+        log_system_params (:obj:`bool`, optional): Enable/Disable logging of system params such as installed packages,
+            git info, environment variables, etc.
+        capture_terminal_logs (:obj:`bool`, optional): Enable/Disable terminal stdout logging.
+    """
+
     def __init__(
         self,
         repo: Optional[str] = None,
-        experiment: Optional[str] = None,
+        experiment_name: Optional[str] = None,
         system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
         log_system_params: Optional[bool] = True,
         capture_terminal_logs: Optional[bool] = True,
     ):
         self._repo_path = repo
-        self._experiment_name = experiment
+        self._experiment_name = experiment_name
         self._system_tracking_interval = system_tracking_interval
         self._log_system_params = log_system_params
         self._capture_terminal_logs = capture_terminal_logs
         self._run = None
         self._run_hash = None
         self._log_value_warned = False
 
@@ -65,16 +80,22 @@
                 self._run_hash = self._run.hash
 
         if args:
             combined_dict = {**args.to_sanitized_dict()}
             for key, value in combined_dict.items():
                 self._run.set(('hparams', key), value, strict=False)
         if model:
-            self._run.set('model', {**vars(model.config), 'num_labels': getattr(model, 'num_labels', None)},
-                          strict=False)
+            self._run.set(
+                'model',
+                {
+                    **vars(model.config),
+                    'num_labels': getattr(model, 'num_labels', None),
+                },
+                strict=False,
+            )
 
         # Store model configs as well
         # if hasattr(model, 'config') and model.config is not None:
         #     model_config = model.config.to_dict()
         #     self._run['model'] = model_config
 
     def on_train_begin(self, args, state, control, model=None, **kwargs):
```

### Comparing `aim-4.0.0.dev3/aim/sdk/adapters/keras.py` & `aim-4.0.0.dev4/aim/sdk/adapters/keras.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,51 +10,79 @@
     raise RuntimeError(
         'This contrib module requires keras to be installed. '
         'Please install it with command: \n pip install keras'
     )
 
 
 class AimCallback(TrackerKerasCallbackMetricsEpochEndMixin, Callback):
-    def __init__(self, repo: Optional[str] = None,
-                 experiment: Optional[str] = None,
-                 system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
-                 log_system_params: Optional[bool] = True,
-                 capture_terminal_logs: Optional[bool] = True):
+    """
+    AimCallback callback class.
+
+    Args:
+        repo (:obj:`str`, optional): Aim repository path or Repo object to which Run object is bound.
+            If skipped, default Repo is used.
+        experiment_name (:obj:`str`, optional): Sets Run's `experiment` property. 'default' if not specified.
+            Can be used later to query runs/sequences.
+        system_tracking_interval (:obj:`int`, optional): Sets the tracking interval in seconds for system usage
+            metrics (CPU, Memory, etc.). Set to `None` to disable system metrics tracking.
+        log_system_params (:obj:`bool`, optional): Enable/Disable logging of system params such as installed packages,
+            git info, environment variables, etc.
+        capture_terminal_logs (:obj:`bool`, optional): Enable/Disable terminal stdout logging.
+    """
+
+    def __init__(
+        self,
+        repo: Optional[str] = None,
+        experiment_name: Optional[str] = None,
+        system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
+        log_system_params: Optional[bool] = True,
+        capture_terminal_logs: Optional[bool] = True,
+    ):
         super(Callback, self).__init__()
 
         self._system_tracking_interval = system_tracking_interval
         self._log_system_params = log_system_params
         self._capture_terminal_logs = capture_terminal_logs
 
-        if repo is None and experiment is None:
-            self._run = Run(system_tracking_interval=self._system_tracking_interval,
-                            log_system_params=self._log_system_params,
-                            capture_terminal_logs=self._capture_terminal_logs,)
+        if repo is None and experiment_name is None:
+            self._run = Run(
+                system_tracking_interval=self._system_tracking_interval,
+                log_system_params=self._log_system_params,
+                capture_terminal_logs=self._capture_terminal_logs,
+            )
         else:
-            self._run = Run(repo=repo, experiment=experiment,
-                            system_tracking_interval=self._system_tracking_interval,
-                            log_system_params=self._log_system_params,
-                            capture_terminal_logs=self._capture_terminal_logs,)
+            self._run = Run(
+                repo=repo,
+                experiment=experiment_name,
+                system_tracking_interval=self._system_tracking_interval,
+                log_system_params=self._log_system_params,
+                capture_terminal_logs=self._capture_terminal_logs,
+            )
 
         self._run_hash = self._run.hash
         self._repo_path = repo
 
     @property
     def experiment(self) -> Run:
         if not self._run:
-            self._run = Run(self._run_hash,
-                            repo=self._repo_path,
-                            system_tracking_interval=self._system_tracking_interval,
-                            capture_terminal_logs=self._capture_terminal_logs,)
+            self._run = Run(
+                self._run_hash,
+                repo=self._repo_path,
+                system_tracking_interval=self._system_tracking_interval,
+                capture_terminal_logs=self._capture_terminal_logs,
+            )
         return self._run
 
     @classmethod
-    def metrics(cls, repo: Optional[str] = None,
-                experiment: Optional[str] = None,
-                run: Optional[Run] = None):
+    def metrics(
+        cls,
+        repo: Optional[str] = None,
+        experiment: Optional[str] = None,
+        run: Optional[Run] = None,
+    ):
         # Keep `metrics` method for backward compatibility
         return cls(repo, experiment, run)
 
     def close(self) -> None:
         if self._run:
             self._run.close()
             del self._run
```

### Comparing `aim-4.0.0.dev3/aim/sdk/adapters/keras_mixins.py` & `aim-4.0.0.dev4/aim/sdk/adapters/keras_mixins.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,20 +12,18 @@
 
     def _log_epoch_metrics(self, epoch, logs):
         if not logs:
             return
 
         track_func = self._run.track
 
-        train_logs = {k: v for k, v in logs.items() if
-                      not k.startswith('val_')}
+        train_logs = {k: v for k, v in logs.items() if not k.startswith('val_')}
         for name, value in train_logs.items():
             track_func(value, name=name, epoch=epoch, context={'subset': 'train'})
 
-        val_logs = {k: v for k, v in logs.items() if
-                    k.startswith('val_')}
+        val_logs = {k: v for k, v in logs.items() if k.startswith('val_')}
         for name, value in val_logs.items():
             track_func(value, name=name[4:], epoch=epoch, context={'subset': 'val'})
 
         lr = self._get_learning_rate()
         if lr is not None:
             track_func(lr, name='lr', epoch=epoch, context={'subset': 'train'})
```

### Comparing `aim-4.0.0.dev3/aim/sdk/adapters/lightgbm.py` & `aim-4.0.0.dev4/aim/sdk/adapters/lightgbm.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,27 +10,38 @@
         'This contrib module requires Lightgbm to be installed. '
         'Please install it with command: \n pip install lightgbm'
     )
 
 
 class AimCallback:
     """
-    Records evaluation data into Aim.
-    Similar to `lightgbm.record_evaluation` callback:
-    https://lightgbm.readthedocs.io/en/latest/pythonapi/lightgbm.record_evaluation.html
+    AimCallback callback class.
+
+    Args:
+        repo (:obj:`str`, optional): Aim repository path or Repo object to which Run object is bound.
+            If skipped, default Repo is used.
+        experiment_name (:obj:`str`, optional): Sets Run's `experiment` property. 'default' if not specified.
+            Can be used later to query runs/sequences.
+        system_tracking_interval (:obj:`int`, optional): Sets the tracking interval in seconds for system usage
+            metrics (CPU, Memory, etc.). Set to `None` to disable system metrics tracking.
+        log_system_params (:obj:`bool`, optional): Enable/Disable logging of system params such as installed packages,
+            git info, environment variables, etc.
+        capture_terminal_logs (:obj:`bool`, optional): Enable/Disable terminal stdout logging.
     """
 
-    def __init__(self, repo: Optional[str] = None,
-                 experiment: Optional[str] = None,
-                 system_tracking_interval: Optional[int]
-                 = DEFAULT_SYSTEM_TRACKING_INT,
-                 log_system_params: Optional[bool] = True,
-                 capture_terminal_logs: Optional[bool] = True,):
+    def __init__(
+        self,
+        repo: Optional[str] = None,
+        experiment_name: Optional[str] = None,
+        system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
+        log_system_params: Optional[bool] = True,
+        capture_terminal_logs: Optional[bool] = True,
+    ):
         self._repo_path = repo
-        self._experiment = experiment
+        self._experiment = experiment_name
         self._system_tracking_interval = system_tracking_interval
         self._log_system_params = log_system_params
         self._capture_terminal_logs = capture_terminal_logs
         self._run = None
         self._run_hash = None
 
         # callback parameters
@@ -59,38 +70,36 @@
                 experiment=self._experiment,
                 system_tracking_interval=self._system_tracking_interval,
                 log_system_params=self._log_system_params,
                 capture_terminal_logs=self._capture_terminal_logs,
             )
             self._run_hash = self._run.hash
 
-    def before_tracking(self, **kwargs):
-        """ Runs before tracking data """
-        pass
-
-    def after_tracking(self, **kwargs):
-        """ Runs after tracking data """
-        pass
-
     def __call__(self, env: CallbackEnv):
         if env.iteration == env.begin_iteration:
             self.setup()
 
         self.before_tracking(env=env)
 
         for item in env.evaluation_result_list:
             if len(item) == 4:
                 data_name, eval_name, result, _ = item
-                self._run.track(result, name=eval_name, context={'data_name': data_name})
+                self._run.track(
+                    result, name=eval_name, context={'data_name': data_name}
+                )
             else:
                 data_name, eval_name = item[1].split()
                 res_mean = item[2]
                 res_stdv = item[4]
-                self._run.track(res_mean, name=f'{eval_name}-mean', context={'data_name': data_name})
-                self._run.track(res_stdv, name=f'{eval_name}-stdv', context={'data_name': data_name})
+                self._run.track(
+                    res_mean, name=f'{eval_name}-mean', context={'data_name': data_name}
+                )
+                self._run.track(
+                    res_stdv, name=f'{eval_name}-stdv', context={'data_name': data_name}
+                )
 
         self.after_tracking(env=env)
 
     def close(self):
         if self._run:
             self._run.close()
             del self._run
```

### Comparing `aim-4.0.0.dev3/aim/sdk/adapters/mxnet.py` & `aim-4.0.0.dev4/aim/sdk/adapters/mxnet.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,63 @@
 import time
 import numpy as np
 from mxnet.gluon.contrib.estimator.utils import _check_metrics
-from mxnet.gluon.contrib.estimator import TrainBegin, TrainEnd, EpochBegin, EpochEnd, BatchBegin, BatchEnd, Estimator
+from mxnet.gluon.contrib.estimator import (
+    TrainBegin,
+    TrainEnd,
+    EpochBegin,
+    EpochEnd,
+    BatchBegin,
+    BatchEnd,
+    Estimator,
+)
 from typing import Optional, Union, Any, List
 from aim.sdk.run import Run
 from aim.ext.resource.configs import DEFAULT_SYSTEM_TRACKING_INT
 
 
-class AimLoggingHandler(TrainBegin, TrainEnd, EpochBegin, EpochEnd, BatchBegin, BatchEnd):
-    """Aim wrapper on top of the Mxnet Basic Logging Handler that applies to every Gluon estimator by default.
-    :py:class:`AimLoggingHandler` logs hyper-parameters, training statistics,
-    and other useful information during training
-    Parameters
-    ----------
-    log_interval: int or str, default 'epoch'
-        Logging interval during training.
-        log_interval='epoch': display metrics every epoch
-        log_interval=integer k: display metrics every interval of k batches
-    metrics : list of EvalMetrics
-        Metrics to be logged, logged at batch end, epoch end, train end.
-    priority : scalar, default np.Inf
-        Priority level of the AimLoggingHandler. Priority level is sorted in
-        ascending order. The lower the number is, the higher priority level the
-        handler is.
+class AimLoggingHandler(
+    TrainBegin, TrainEnd, EpochBegin, EpochEnd, BatchBegin, BatchEnd
+):
     """
+    AimLoggingHandler logging handler class.
 
-    def __init__(self, log_interval: Union[int, str] = 'epoch',
-                 repo: Optional[str] = None,
-                 experiment_name: Optional[str] = None,
-                 system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
-                 log_system_params: Optional[bool] = True,
-                 capture_terminal_logs: Optional[bool] = True,
-                 metrics: Optional[List[Any]] = None,
-                 priority=np.Inf,):
+    Args:
+        repo (:obj:`str`, optional): Aim repository path or Repo object to which Run object is bound.
+            If skipped, default Repo is used.
+        experiment_name (:obj:`str`, optional): Sets Run's `experiment` property. 'default' if not specified.
+            Can be used later to query runs/sequences.
+        system_tracking_interval (:obj:`int`, optional): Sets the tracking interval in seconds for system usage
+            metrics (CPU, Memory, etc.). Set to `None` to disable system metrics tracking.
+        log_system_params (:obj:`bool`, optional): Enable/Disable logging of system params such as installed packages,
+            git info, environment variables, etc.
+        capture_terminal_logs (:obj:`bool`, optional): Enable/Disable terminal stdout logging.
+        log_interval: (:obj:`int` or `str`) default: 'epoch': Logging interval during training.
+            log_interval='epoch': display metrics every epoch
+            log_interval=integer k: display metrics every interval of k batches
+        metrics: (:obj:`list`, optional): Metrics to be logged, logged at batch end, epoch end, train end.
+        priority: (:obj:`float`, optional), default np.Inf:  Priority level of the AimLoggingHandler.
+            Priority level is sorted in ascending order.
+            The lower the number is, the higher priority level the handler is.
+    """
+
+    def __init__(
+        self,
+        repo: Optional[str] = None,
+        experiment_name: Optional[str] = None,
+        system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
+        log_system_params: Optional[bool] = True,
+        capture_terminal_logs: Optional[bool] = True,
+        log_interval: Union[int, str] = 'epoch',
+        metrics: Optional[List[Any]] = None,
+        priority=np.Inf,
+    ):
         super().__init__()
         if not isinstance(log_interval, int) and log_interval != 'epoch':
-            raise ValueError("log_interval must be either an integer or string 'epoch'")
+            raise ValueError('log_interval must be either an integer or string "epoch"')
 
         self.metrics = _check_metrics(metrics)
         self.batch_index = 0
         self.current_epoch = 0
         self.processed_samples = 0
         # logging handler need to be called at last to make sure all states are updated
         # it will also shut down logging at train end
@@ -57,71 +75,81 @@
 
     def train_begin(self, estimator: Optional[Estimator], *args, **kwargs):
         self.train_start = time.time()
         trainer = estimator.trainer
         optimizer = trainer.optimizer.__class__.__name__
         lr = trainer.learning_rate
 
-        estimator.logger.info("Training begin: using optimizer %s "
-                              "with current learning rate %.4f ",
-                              optimizer, lr)
+        estimator.logger.info(
+            'Training begin: using optimizer %s ' 'with current learning rate %.4f ',
+            optimizer,
+            lr,
+        )
         if estimator.max_epoch:
-            estimator.logger.info("Train for %d epochs.", estimator.max_epoch)
+            estimator.logger.info('Train for %d epochs.', estimator.max_epoch)
         else:
-            estimator.logger.info("Train for %d batches.", estimator.max_batch)
+            estimator.logger.info('Train for %d batches.', estimator.max_batch)
         # reset all counters
         self.current_epoch = 0
         self.batch_index = 0
         self.processed_samples = 0
         self.log_interval_time = 0
 
         params = {
-            "arch": estimator.net.name,
-            "loss": estimator.loss.name,
-            "optimizer": optimizer,
-            "lr": lr,
-            "max_epoch": estimator.max_epoch,
-            "max_batch": estimator.max_batch
+            'arch': estimator.net.name,
+            'loss': estimator.loss.name,
+            'optimizer': optimizer,
+            'lr': lr,
+            'max_epoch': estimator.max_epoch,
+            'max_batch': estimator.max_batch,
         }
 
         self.setup(estimator, params)
 
     def train_end(self, estimator: Optional[Estimator], *args, **kwargs):
         train_time = time.time() - self.train_start
-        msg = 'Train finished using total %ds with %d epochs. ' % (train_time, self.current_epoch)
+        msg = 'Train finished using total %ds with %d epochs. ' % (
+            train_time,
+            self.current_epoch,
+        )
         # log every result in train stats including train/validation loss & metrics
         for metric in self.metrics:
             name, value = metric.get()
             msg += '%s: %.4f, ' % (name, value)
         estimator.logger.info(msg.rstrip(', '))
 
     def epoch_begin(self, estimator: Optional[Estimator], *args, **kwargs):
         if isinstance(self.log_interval, int) or self.log_interval == 'epoch':
             is_training = False
             for metric in self.metrics:
                 if 'training' in metric.name:
                     is_training = True
             self.epoch_start = time.time()
             if is_training:
-                estimator.logger.info("[Epoch %d] Begin, current learning rate: %.4f",
-                                      self.current_epoch, estimator.trainer.learning_rate)
+                estimator.logger.info(
+                    '[Epoch %d] Begin, current learning rate: %.4f',
+                    self.current_epoch,
+                    estimator.trainer.learning_rate,
+                )
             else:
-                estimator.logger.info("Validation Begin")
+                estimator.logger.info('Validation Begin')
 
     def epoch_end(self, estimator: Optional[Estimator], *args, **kwargs):
         if isinstance(self.log_interval, int) or self.log_interval == 'epoch':
             epoch_time = time.time() - self.epoch_start
             msg = '[Epoch %d] Finished in %.3fs, ' % (self.current_epoch, epoch_time)
             for metric in self.metrics:
                 name, value = metric.get()
                 msg += '%s: %.4f, ' % (name, value)
 
-                context_name, metric_name = name.split(" ")
+                context_name, metric_name = name.split(' ')
                 context = {'subset': context_name}
-                self._run.track(value, metric_name, step=self.batch_index, context=context)
+                self._run.track(
+                    value, metric_name, step=self.batch_index, context=context
+                )
             estimator.logger.info(msg.rstrip(', '))
         self.current_epoch += 1
         self.batch_index = 0
 
     def batch_begin(self, estimator: Optional[Estimator], *args, **kwargs):
         if isinstance(self.log_interval, int):
             self.batch_start = time.time()
@@ -137,17 +165,19 @@
                 msg += 'time/interval: %.3fs ' % self.log_interval_time
                 self.log_interval_time = 0
                 for metric in self.metrics:
                     # only log current training loss & metric after each interval
                     name, value = metric.get()
                     msg += '%s: %.4f, ' % (name, value)
 
-                    context_name, metric_name = name.split(" ")
+                    context_name, metric_name = name.split(' ')
                     context = {'subset': context_name}
-                    self._run.track(value, metric_name, step=self.batch_index, context=context)
+                    self._run.track(
+                        value, metric_name, step=self.batch_index, context=context
+                    )
                 estimator.logger.info(msg.rstrip(', '))
         self.batch_index += 1
 
     @property
     def experiment(self) -> Run:
         if not self._run:
             self.setup()
```

### Comparing `aim-4.0.0.dev3/aim/sdk/adapters/optuna.py` & `aim-4.0.0.dev4/aim/sdk/adapters/optuna.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,68 +8,58 @@
 
 
 with try_import() as _imports:
     from aim.sdk.run import Run
     from aim.ext.resource.configs import DEFAULT_SYSTEM_TRACKING_INT
 
 
-@experimental_class("2.9.0")
+@experimental_class('2.9.0')
 class AimCallback:
-    """Callback to track Optuna trials with Aim.
-
-    This callback enables tracking of Optuna study in Aim.
-    The study is tracked as a single experiment run,
-    where all suggested hyperparameters and optimized metrics
-    are logged and plotted as a function of optimizer steps.
-
-    .. note::
-        Users who want to run multiple Optuna studies within the same process
-        should call ``close()`` method between subsequent calls to
-        ``study.optimize()``. Calling ``close()`` method is not necessary
-        if you are running one Optuna study per process.
-
-    .. note::
-        To ensure correct trial order in Aim, this callback
-        should only be used with ``study.optimize(n_jobs=1)``.
-
+    """
+    AimCallback callback class.
 
     Args:
-        metric_name:
-            Name assigned to optimized metric. In case of multi-objective optimization,
-            list of names can be passed. Those names will be assigned
+        repo (:obj:`str`, optional): Aim repository path or Repo object to which Run object is bound.
+            If skipped, default Repo is used.
+        experiment_name (:obj:`str`, optional): Sets Run's `experiment` property. 'default' if not specified.
+            Can be used later to query runs/sequences.
+        system_tracking_interval (:obj:`int`, optional): Sets the tracking interval in seconds for system usage
+            metrics (CPU, Memory, etc.). Set to `None` to disable system metrics tracking.
+        log_system_params (:obj:`bool`, optional): Enable/Disable logging of system params such as installed packages,
+            git info, environment variables, etc.
+        capture_terminal_logs (:obj:`bool`, optional): Enable/Disable terminal stdout logging.
+        metric_name (:obj:`str`, optional): Name assigned to optimized metric.
+            In case of multi-objective optimization, list of names can be passed. Those names will be assigned
             to metrics in the order returned by objective function.
             If single name is provided, or this argument is left to default value,
             it will be broadcasted to each objective with a number suffix in order
             returned by objective function e.g. two objectives and default metric name
             will be logged as ``value_0`` and ``value_1``. The number of metrics must be
             the same as the number of values objective function returns.
-        as_multirun:
-            Creates new runs for each trial and sets the metrics as run parametrs.
+        as_multirun (:obj:`bool`, optional): Creates new runs for each trial and sets the metrics as run parametrs.
             Useful for exploring parameters in Aim UI
             (for more: https://aimstack.readthedocs.io/en/latest/ui/pages/explorers.html#params-explorer).
             If is false then all of the stats are tracked in a single run as Aim metrics.
-
     """
 
     def __init__(
         self,
-        metric_name: Union[str, Sequence[str]] = "value",
-        as_multirun: bool = False,
         repo: Optional[str] = None,
         experiment_name: Optional[str] = None,
         system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
         log_system_params: Optional[bool] = True,
         capture_terminal_logs: Optional[bool] = True,
+        metric_name: Union[str, Sequence[str]] = 'value',
+        as_multirun: bool = False,
     ) -> None:
-
         _imports.check()
 
         if not isinstance(metric_name, Sequence):
             raise TypeError(
-                f"Expected metric_name to be string or sequence of strings, got {type(metric_name)}."
+                f'Expected metric_name to be string or sequence of strings, got {type(metric_name)}.'
             )
 
         self._metric_name = metric_name
         self._as_multirun = as_multirun
         self._repo_path = repo
         self._experiment_name = experiment_name
         self._system_tracking_interval = system_tracking_interval
@@ -77,49 +67,50 @@
         self._capture_terminal_logs = capture_terminal_logs
         self._run = None
         self._run_hash = None
 
         if not self._as_multirun:
             self.setup()
 
-    def __call__(self, study: optuna.study.Study, trial: optuna.trial.FrozenTrial) -> None:
-
+    def __call__(
+        self, study: optuna.study.Study, trial: optuna.trial.FrozenTrial
+    ) -> None:
         if isinstance(self._metric_name, str):
             if len(trial.values) > 1:
                 # Broadcast default name for multi-objective optimization.
-                names = [f"{self._metric_name}_{i}" for i in range(len(trial.values))]
+                names = [f'{self._metric_name}_{i}' for i in range(len(trial.values))]
             else:
                 names = [self._metric_name]
         else:
             if len(self._metric_name) != len(trial.values):
                 raise ValueError(
-                    "Running multi-objective optimization "
-                    f"with {len(trial.values)} objective values, but {len(self._metric_name)} names specified. "
-                    "Match objective values and names, or use default broadcasting."
+                    'Running multi-objective optimization '
+                    f'with {len(trial.values)} objective values, but {len(self._metric_name)} names specified. '
+                    'Match objective values and names, or use default broadcasting.'
                 )
             else:
                 names = self._metric_name
 
         metrics = {name: value for name, value in zip(names, trial.values)}
 
         if self._as_multirun:
-            metrics["trial_number"] = trial.number
+            metrics['trial_number'] = trial.number
 
-        attributes = {"direction": [d.name for d in study.directions]}
+        attributes = {'direction': [d.name for d in study.directions]}
 
         step = trial.number if self._run else None
 
         if not self._run:
             self.setup()
-            self._run.name = f"trial-{trial.number}"
+            self._run.name = f'trial-{trial.number}'
 
         for key, value in attributes.items():
             self._run.set(('hparams', key), value, strict=False)
 
-        self._run.set("study_name", study.study_name)
+        self._run.set('study_name', study.study_name)
 
         if self._as_multirun:
             for key, value in trial.params.items():
                 self._run.set(('hparams', key), value, strict=False)
 
             for key, value in metrics.items():
                 self._run.set(key, value, strict=False)
@@ -162,15 +153,15 @@
 
     def close(self) -> None:
         if self._run:
             self._run.close()
             self._run = None
             self._run_hash = None
 
-    @experimental_func("3.0.0")
+    @experimental_func('3.0.0')
     def track_in_aim(self) -> Callable:
         """Decorator for using Aim for tracking inside the objective function.
 
         All the metrics from inside the objective function will be logged into the same run
         which stores the parameters for a given trial.
 
         Returns:
@@ -178,11 +169,13 @@
         """
 
         def decorator(func: ObjectiveFuncType) -> ObjectiveFuncType:
             @functools.wraps(func)
             def wrapper(trial: optuna.trial.Trial) -> Union[float, Sequence[float]]:
                 if not self._run:
                     self.setup()
-                    self._run.name = f"trial-{trial.number}"
+                    self._run.name = f'trial-{trial.number}'
                 return func(trial)
+
             return wrapper
+
         return decorator
```

### Comparing `aim-4.0.0.dev3/aim/sdk/adapters/paddle.py` & `aim-4.0.0.dev4/aim/sdk/adapters/paddle.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,21 +13,25 @@
             If skipped, default Repo is used.
         experiment_name (:obj:`str`, optional): Sets Run's `experiment` property. 'default' if not specified.
             Can be used later to query runs/sequences.
         system_tracking_interval (:obj:`int`, optional): Sets the tracking interval in seconds for system usage
             metrics (CPU, Memory, etc.). Set to `None` to disable system metrics tracking.
         log_system_params (:obj:`bool`, optional): Enable/Disable logging of system params such as installed packages,
             git info, environment variables, etc.
+        capture_terminal_logs (:obj:`bool`, optional): Enable/Disable terminal stdout logging.
     """
 
-    def __init__(self, repo: Optional[str] = None,
-                 experiment_name: Optional[str] = None,
-                 system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
-                 log_system_params: Optional[bool] = True,
-                 capture_terminal_logs: Optional[bool] = True,):
+    def __init__(
+        self,
+        repo: Optional[str] = None,
+        experiment_name: Optional[str] = None,
+        system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
+        log_system_params: Optional[bool] = True,
+        capture_terminal_logs: Optional[bool] = True,
+    ):
         self.repo = repo
         self.experiment_name = experiment_name
         self.system_tracking_interval = system_tracking_interval
         self.log_system_params = log_system_params
         self.capture_terminal_logs = capture_terminal_logs
         self._run = None
         self._run_hash = None
@@ -47,15 +51,15 @@
 
     def _track(self, logs, context, step=None):
         for k, v in logs.items():
             if isinstance(v, list):
                 if len(v) == 1:
                     v = v[0]
                 else:
-                    raise NotImplementedError(f"number of items in {k} are more than 1")
+                    raise NotImplementedError(f'number of items in {k} are more than 1')
             self._run.track(v, k, step=step, context=context, epoch=self.epoch)
 
     @property
     def experiment(self):
         if not self._run:
             self.setup()
         return self._run
```

### Comparing `aim-4.0.0.dev3/aim/sdk/adapters/pytorch.py` & `aim-4.0.0.dev4/aim/sdk/adapters/pytorch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 def track_params_dists(model, run):
     from aim import Distribution
+
     data_hist = get_model_layers(model, 'data')
 
     for name, params in data_hist.items():
         if 'weight' in params:
             run.track(
                 Distribution(params['weight']),
                 name=name,
                 context={
                     'type': 'data',
                     'params': 'weights',
-                }
+                },
             )
         if 'bias' in params:
             run.track(
                 Distribution(params['bias']),
                 name=name,
                 context={
                     'type': 'data',
                     'params': 'biases',
-                }
+                },
             )
 
 
 def track_gradients_dists(model, run):
     from aim import Distribution
+
     grad_hist = get_model_layers(model, 'grad')
 
     for name, params in grad_hist.items():
         if 'weight' in params:
             run.track(
                 Distribution(params['weight']),
                 name=name,
                 context={
                     'type': 'gradients',
                     'params': 'weights',
-                }
+                },
             )
         if 'bias' in params:
             run.track(
                 Distribution(params['bias']),
                 name=name,
                 context={
                     'type': 'gradients',
                     'params': 'biases',
-                }
+                },
             )
 
 
 def get_model_layers(model, dt, parent_name=None):
     layers = {}
     for name, m in model.named_children():
-        layer_name = '{}__{}'.format(parent_name, name) \
-            if parent_name \
-            else name
+        layer_name = '{}__{}'.format(parent_name, name) if parent_name else name
         layer_name += '.{}'.format(type(m).__name__)
 
         if len(list(m.named_children())):
             layers.update(get_model_layers(m, dt, layer_name))
         else:
             layers[layer_name] = {}
             weight = None
```

### Comparing `aim-4.0.0.dev3/aim/sdk/adapters/pytorch_ignite.py` & `aim-4.0.0.dev4/aim/sdk/adapters/pytorch_ignite.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,60 +7,71 @@
     from torch.optim import Optimizer
 except ImportError:
     raise RuntimeError(
         'This contrib module requires PyTorch to be installed. '
         'Please install it with command: \n pip install torch'
     )
 try:
-    from ignite.contrib.handlers.base_logger import BaseLogger, BaseOptimizerParamsHandler, BaseOutputHandler
+    from ignite.contrib.handlers.base_logger import (
+        BaseLogger,
+        BaseOptimizerParamsHandler,
+        BaseOutputHandler,
+    )
     from ignite.engine import Engine, Events
 except ImportError:
     raise RuntimeError(
         'This contrib module requires PyTorch Ignite to be installed. '
         'Please install it with command: \n pip install pytorch-ignite'
     )
 
 
 class AimLogger(BaseLogger):
     """
-        `Aim` tracking client handler to log parameters and metrics during the training
-        and validation.
+    AimLogger logger class.
 
-        Args:
-            repo: Aim repository path
-            experiment: Aim run's experiment name
-            train_metric_prefix: prefix to identify training metrics
-            val_metric_prefix: prefix to identify validation metrics
-            test_metric_prefix: prefix to identify test metrics
-            system_tracking_interval: sets the tracking interval in seconds
-                for system usage metrics (CPU, Memory, etc.)
-            log_system_params: flag to enable system params logging, True by default
+    Args:
+        repo (:obj:`str`, optional): Aim repository path or Repo object to which Run object is bound.
+            If skipped, default Repo is used.
+        experiment_name (:obj:`str`, optional): Sets Run's `experiment` property. 'default' if not specified.
+            Can be used later to query runs/sequences.
+        system_tracking_interval (:obj:`int`, optional): Sets the tracking interval in seconds for system usage
+            metrics (CPU, Memory, etc.). Set to `None` to disable system metrics tracking.
+        log_system_params (:obj:`bool`, optional): Enable/Disable logging of system params such as installed packages,
+            git info, environment variables, etc.
+        capture_terminal_logs (:obj:`bool`, optional): Enable/Disable terminal stdout logging.
+        train_metric_prefix (:obj:`str`, optional): Training metric prefix.
+        val_metric_prefix (:obj:`str`, optional): validation metric prefix.
+        test_metric_prefix (:obj:`str`, optional): testing metric prefix.
+        context (:obj:`dict`, optional): Initial context to use for adding metric context.
     """
-    def __init__(self,
-                 repo: Optional[str] = None,
-                 experiment: Optional[str] = None,
-                 train_metric_prefix: Optional[str] = 'train_',
-                 val_metric_prefix: Optional[str] = 'val_',
-                 test_metric_prefix: Optional[str] = 'test_',
-                 system_tracking_interval: Optional[int]
-                 = DEFAULT_SYSTEM_TRACKING_INT,
-                 log_system_params: Optional[bool] = True,
-                 capture_terminal_logs: Optional[bool] = True,
-                 ):
+
+    def __init__(
+        self,
+        repo: Optional[str] = None,
+        experiment_name: Optional[str] = None,
+        system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
+        log_system_params: Optional[bool] = True,
+        capture_terminal_logs: Optional[bool] = True,
+        train_metric_prefix: Optional[str] = 'train_',
+        val_metric_prefix: Optional[str] = 'val_',
+        test_metric_prefix: Optional[str] = 'test_',
+        context: Optional[Dict[str, Any]] = {},
+    ):
         super().__init__()
 
-        self._experiment_name = experiment
         self._repo_path = repo
+        self._experiment_name = experiment_name
+        self._system_tracking_interval = system_tracking_interval
+        self._log_system_params = log_system_params
+        self._capture_terminal_logs = capture_terminal_logs
 
         self._train_metric_prefix = train_metric_prefix
         self._val_metric_prefix = val_metric_prefix
         self._test_metric_prefix = test_metric_prefix
-        self._system_tracking_interval = system_tracking_interval
-        self._log_system_params = log_system_params
-        self._capture_terminal_logs = capture_terminal_logs
+        self._context = context
 
         self._run = None
         self._run_hash = None
 
     @property
     def experiment(self) -> Run:
         if self._run is None:
@@ -92,31 +103,28 @@
             # Convert to primitives
             if isinstance(params, Container):
                 params = OmegaConf.to_container(params, resolve=True)
 
         for key, value in params.items():
             self.experiment.set(('hparams', key), value, strict=False)
 
-    def log_metrics(self, metrics: Dict[str, float],
-                    step: Optional[int] = None):
+    def log_metrics(self, metrics: Dict[str, float], step: Optional[int] = None):
         for k, v in metrics.items():
             name = k
             context = {}
-            if self._train_metric_prefix \
-                    and name.startswith(self._train_metric_prefix):
+            if self._train_metric_prefix and name.startswith(self._train_metric_prefix):
                 name = name[len(self._train_metric_prefix):]
                 context['subset'] = 'train'
-            elif self._test_metric_prefix \
-                    and name.startswith(self._test_metric_prefix):
+            elif self._test_metric_prefix and name.startswith(self._test_metric_prefix):
                 name = name[len(self._test_metric_prefix):]
                 context['subset'] = 'test'
-            elif self._val_metric_prefix \
-                    and name.startswith(self._val_metric_prefix):
+            elif self._val_metric_prefix and name.startswith(self._val_metric_prefix):
                 name = name[len(self._val_metric_prefix):]
                 context['subset'] = 'val'
+            context.update(self._context)
             self.experiment.track(v, step=step, name=name, context=context)
 
     @property
     def save_dir(self) -> str:
         return self.experiment.repo.path
 
     @property
@@ -132,55 +140,59 @@
             self._run.close()
             del self._run
             self._run = None
 
     def __del__(self):
         self.close()
 
-    def _create_output_handler(self, *args: Any, **kwargs: Any) -> "OutputHandler":
+    def _create_output_handler(self, *args: Any, **kwargs: Any) -> 'OutputHandler':
         return OutputHandler(*args, **kwargs)
 
-    def _create_opt_params_handler(self, *args: Any, **kwargs: Any) -> "OptimizerParamsHandler":
+    def _create_opt_params_handler(
+        self, *args: Any, **kwargs: Any
+    ) -> 'OptimizerParamsHandler':
         return OptimizerParamsHandler(*args, **kwargs)
 
 
 class OutputHandler(BaseOutputHandler):
     """Helper handler to log engine's output and/or metrics.
 
-        Args:
-            tag: common title for all produced plots. For example, 'training'
-            metric_names: list of metric names to plot or a string "all" to plot all available
-                metrics.
-            output_transform: output transform function to prepare `engine.state.output` as a number.
-                For example, `output_transform = lambda output: output`
-                This function can also return a dictionary, e.g `{'loss': loss1, 'another_loss': loss2}` to label
-                the plot with corresponding keys.
-            global_step_transform: global step transform function to output a desired global step.
-                Input of the function is `(engine, event_name)`. Output of function should be an integer.
-                Default is None, global_step based on attached engine. If provided,
-                uses function output as global_step. To setup global step from another engine, please use
-                :meth:`~ignite.contrib.handlers.mlflow_logger.global_step_from_engine`.
-            state_attributes: list of attributes of the ``trainer.state`` to plot.
+    Args:
+        tag: common title for all produced plots. For example, 'training'
+        metric_names: list of metric names to plot or a string "all" to plot all available
+            metrics.
+        output_transform: output transform function to prepare `engine.state.output` as a number.
+            For example, `output_transform = lambda output: output`
+            This function can also return a dictionary, e.g `{'loss': loss1, 'another_loss': loss2}` to label
+            the plot with corresponding keys.
+        global_step_transform: global step transform function to output a desired global step.
+            Input of the function is `(engine, event_name)`. Output of function should be an integer.
+            Default is None, global_step based on attached engine. If provided,
+            uses function output as global_step. To setup global step from another engine, please use
+            :meth:`~ignite.contrib.handlers.mlflow_logger.global_step_from_engine`.
+        state_attributes: list of attributes of the ``trainer.state`` to plot.
     """
+
     def __init__(
         self,
         tag: str,
         metric_names: Optional[Union[str, List[str]]] = None,
         output_transform: Optional[Callable] = None,
         global_step_transform: Optional[Callable] = None,
         state_attributes: Optional[List[str]] = None,
     ) -> None:
         super(OutputHandler, self).__init__(
             tag, metric_names, output_transform, global_step_transform, state_attributes
         )
 
-    def __call__(self, engine: Engine, logger: AimLogger, event_name: Union[str, Events]) -> None:
-
+    def __call__(
+        self, engine: Engine, logger: AimLogger, event_name: Union[str, Events]
+    ) -> None:
         if not isinstance(logger, AimLogger):
-            raise TypeError('Handler \'OutputHandler\' works only with AimLogger')
+            raise TypeError('Handler "OutputHandler" works only with AimLogger')
 
         rendered_metrics = self._setup_output_metrics_state_attrs(engine)
 
         global_step = self.global_step_transform(engine, event_name)  # type: ignore[misc]
 
         if not isinstance(global_step, int):
             raise TypeError(
@@ -195,28 +207,35 @@
 
         logger.log_metrics(metrics, step=global_step)
 
 
 class OptimizerParamsHandler(BaseOptimizerParamsHandler):
     """Helper handler to log optimizer parameters
 
-        Args:
-            optimizer: torch optimizer or any object with attribute ``param_groups``
-                as a sequence.
-            param_name: parameter name
-            tag: common title for all produced plots. For example, 'generator'
+    Args:
+        optimizer: torch optimizer or any object with attribute ``param_groups``
+            as a sequence.
+        param_name: parameter name
+        tag: common title for all produced plots. For example, 'generator'
     """
-    def __init__(self, optimizer: Optimizer, param_name: str = 'lr', tag: Optional[str] = None):
+
+    def __init__(
+        self, optimizer: Optimizer, param_name: str = 'lr', tag: Optional[str] = None
+    ):
         super(OptimizerParamsHandler, self).__init__(optimizer, param_name, tag)
 
-    def __call__(self, engine: Engine, logger: AimLogger, event_name: Union[str, Events]) -> None:
+    def __call__(
+        self, engine: Engine, logger: AimLogger, event_name: Union[str, Events]
+    ) -> None:
         if not isinstance(logger, AimLogger):
             raise TypeError('Handler OptimizerParamsHandler works only with AimLogger')
 
         global_step = engine.state.get_event_attrib_value(event_name)
         tag_prefix = f'{self.tag}_' if self.tag else ''
         params = {
-            f'{tag_prefix}{self.param_name}_group_{i}': float(param_group[self.param_name])
+            f'{tag_prefix}{self.param_name}_group_{i}': float(
+                param_group[self.param_name]
+            )
             for i, param_group in enumerate(self.optimizer.param_groups)
         }
 
         logger.log_metrics(params, step=global_step)
```

### Comparing `aim-4.0.0.dev3/aim/sdk/adapters/pytorch_lightning.py` & `aim-4.0.0.dev4/aim/sdk/adapters/pytorch_lightning.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from argparse import Namespace
 
 import packaging.version
 
 try:
     import pytorch_lightning as pl
 
-    if packaging.version.parse(pl.__version__) < packaging.version.parse("1.7"):
+    if packaging.version.parse(pl.__version__) < packaging.version.parse('1.7'):
         from pytorch_lightning.loggers.base import (
             LightningLoggerBase as Logger,
             rank_zero_experiment,
         )
     else:
         from pytorch_lightning.loggers.logger import (
             Logger,
@@ -28,43 +28,64 @@
 from aim.sdk.run import Run
 from aim.sdk.repo import Repo
 from aim.sdk.utils import clean_repo_path, get_aim_repo_name
 from aim.ext.resource.configs import DEFAULT_SYSTEM_TRACKING_INT
 
 
 class AimLogger(Logger):
-    def __init__(self,
-                 repo: Optional[str] = None,
-                 experiment: Optional[str] = None,
-                 train_metric_prefix: Optional[str] = 'train_',
-                 val_metric_prefix: Optional[str] = 'val_',
-                 test_metric_prefix: Optional[str] = 'test_',
-                 system_tracking_interval: Optional[int]
-                 = DEFAULT_SYSTEM_TRACKING_INT,
-                 log_system_params: Optional[bool] = True,
-                 capture_terminal_logs: Optional[bool] = True,
-                 run_name: Optional[str] = None,
-                 run_hash: Optional[str] = None,
-                 ):
+    """
+    AimLogger logger class.
+
+    Args:
+        repo (:obj:`str`, optional): Aim repository path or Repo object to which Run object is bound.
+            If skipped, default Repo is used.
+        experiment_name (:obj:`str`, optional): Sets Run's `experiment` property. 'default' if not specified.
+            Can be used later to query runs/sequences.
+        system_tracking_interval (:obj:`int`, optional): Sets the tracking interval in seconds for system usage
+            metrics (CPU, Memory, etc.). Set to `None` to disable system metrics tracking.
+        log_system_params (:obj:`bool`, optional): Enable/Disable logging of system params such as installed packages,
+            git info, environment variables, etc.
+        capture_terminal_logs (:obj:`bool`, optional): Enable/Disable terminal stdout logging.
+        train_metric_prefix (:obj:`str`, optional): Training metric prefix.
+        val_metric_prefix (:obj:`str`, optional): validation metric prefix.
+        test_metric_prefix (:obj:`str`, optional): testing metric prefix.
+        run_name (:obj:`str`, optional): Aim run name, for reusing the specified run.
+        run_hash (:obj:`str`, optional): Aim run hash, for reusing the specified run.
+    """
+
+    def __init__(
+        self,
+        repo: Optional[str] = None,
+        experiment_name: Optional[str] = None,
+        system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
+        log_system_params: Optional[bool] = True,
+        capture_terminal_logs: Optional[bool] = True,
+        train_metric_prefix: Optional[str] = 'train_',
+        val_metric_prefix: Optional[str] = 'val_',
+        test_metric_prefix: Optional[str] = 'test_',
+        run_name: Optional[str] = None,
+        run_hash: Optional[str] = None,
+    ):
         super().__init__()
 
-        self._experiment_name = experiment
-        self._run_name = run_name
         self._repo_path = repo
+        self._experiment_name = experiment_name
+        self._system_tracking_interval = system_tracking_interval
+        self._log_system_params = log_system_params
+        self._capture_terminal_logs = capture_terminal_logs
 
         self._train_metric_prefix = train_metric_prefix
         self._val_metric_prefix = val_metric_prefix
         self._test_metric_prefix = test_metric_prefix
-        self._system_tracking_interval = system_tracking_interval
-        self._log_system_params = log_system_params
-        self._capture_terminal_logs = capture_terminal_logs
 
-        self._run = None
+        self._run_name = run_name
         self._run_hash = run_hash
 
+        self._run = None
+
     @staticmethod
     def _convert_params(params: Union[Dict[str, Any], Namespace]) -> Dict[str, Any]:
         # in case converting from namespace
         if isinstance(params, Namespace):
             params = vars(params)
 
         if params is None:
@@ -77,15 +98,15 @@
     def experiment(self) -> Run:
         if self._run is None:
             if self._run_hash:
                 self._run = Run(
                     self._run_hash,
                     repo=self._repo_path,
                     system_tracking_interval=self._system_tracking_interval,
-                    capture_terminal_logs=self._capture_terminal_logs
+                    capture_terminal_logs=self._capture_terminal_logs,
                 )
                 if self._run_name is not None:
                     self._run.name = self._run_name
             else:
                 self._run = Run(
                     repo=self._repo_path,
                     experiment=self._experiment_name,
@@ -110,39 +131,34 @@
             if OmegaConf.is_config(params):
                 params = OmegaConf.to_container(params, resolve=True)
 
         for key, value in params.items():
             self.experiment.set(('hparams', key), value, strict=False)
 
     @rank_zero_only
-    def log_metrics(self, metrics: Dict[str, float],
-                    step: Optional[int] = None):
-        assert rank_zero_only.rank == 0, \
-            'experiment tried to log from global_rank != 0'
+    def log_metrics(self, metrics: Dict[str, float], step: Optional[int] = None):
+        assert rank_zero_only.rank == 0, 'experiment tried to log from global_rank != 0'
 
-        metric_items: Dict[str: Any] = {k: v for k, v in metrics.items()}
+        metric_items: Dict[str:Any] = {k: v for k, v in metrics.items()}
 
         if 'epoch' in metric_items:
             epoch: int = metric_items.pop('epoch')
         else:
             epoch = None
 
         for k, v in metric_items.items():
             name = k
             context = {}
-            if self._train_metric_prefix \
-                    and name.startswith(self._train_metric_prefix):
+            if self._train_metric_prefix and name.startswith(self._train_metric_prefix):
                 name = name[len(self._train_metric_prefix):]
                 context['subset'] = 'train'
-            elif self._test_metric_prefix \
-                    and name.startswith(self._test_metric_prefix):
+            elif self._test_metric_prefix and name.startswith(self._test_metric_prefix):
                 name = name[len(self._test_metric_prefix):]
                 context['subset'] = 'test'
-            elif self._val_metric_prefix \
-                    and name.startswith(self._val_metric_prefix):
+            elif self._val_metric_prefix and name.startswith(self._val_metric_prefix):
                 name = name[len(self._val_metric_prefix):]
                 context['subset'] = 'val'
             self.experiment.track(v, name=name, step=step, epoch=epoch, context=context)
 
     @rank_zero_only
     def finalize(self, status: str = '') -> None:
         super().finalize(status)
```

### Comparing `aim-4.0.0.dev3/aim/sdk/adapters/sb3.py` & `aim-4.0.0.dev4/aim/sdk/adapters/sb3.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,81 +13,80 @@
 
 
 class AimOutputFormat(KVWriter):
     """
     Track key/value pairs into Aim run.
     """
 
-    def __init__(
-        self,
-        aim_callback
-    ):
+    def __init__(self, aim_callback):
         self.aim_callback = aim_callback
 
     def write(
         self,
         key_values: Dict[str, Any],
         key_excluded: Dict[str, Union[str, Tuple[str, ...]]],
         step: int = 0,
     ) -> None:
         for (key, value), (_, excluded) in zip(
             sorted(key_values.items()), sorted(key_excluded.items())
         ):
-
             if excluded is not None:
                 continue
 
             if isinstance(value, np.ScalarType):
                 if not isinstance(value, str):
                     tag, key = key.split('/')
                     if tag in ['train', 'valid']:
                         context = {'subset': tag}
                     else:
                         context = {'tag': tag}
 
-                    self.aim_callback.experiment.track(value, key, step=step, context=context)
+                    self.aim_callback.experiment.track(
+                        value, key, step=step, context=context
+                    )
 
 
 class AimCallback(BaseCallback):
     """
-    AimCallback callback function.
+    AimCallback callback class.
 
     Args:
         repo (:obj:`str`, optional): Aim repository path or Repo object to which Run object is bound.
             If skipped, default Repo is used.
         experiment_name (:obj:`str`, optional): Sets Run's `experiment` property. 'default' if not specified.
             Can be used later to query runs/sequences.
         system_tracking_interval (:obj:`int`, optional): Sets the tracking interval in seconds for system usage
             metrics (CPU, Memory, etc.). Set to `None` to disable system metrics tracking.
         log_system_params (:obj:`bool`, optional): Enable/Disable logging of system params such as installed packages,
             git info, environment variables, etc.
+        capture_terminal_logs (:obj:`bool`, optional): Enable/Disable terminal stdout logging.
+        verbose (:obj:`bool`, optional): Enable/Disable verbose
     """
 
     def __init__(
         self,
         repo: Optional[str] = None,
         experiment_name: Optional[str] = None,
         system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
         log_system_params: Optional[bool] = True,
         capture_terminal_logs: Optional[bool] = True,
         verbose: int = 0,
     ) -> None:
-
         super().__init__(verbose)
 
         self.repo = repo
         self.experiment_name = experiment_name
         self.system_tracking_interval = system_tracking_interval
         self.log_system_params = log_system_params
         self.capture_terminal_logs = capture_terminal_logs
         self._run = None
         self._run_hash = None
 
     def _init_callback(self) -> None:
-        args = {"algo": type(self.model).__name__}
+        args = {'algo': type(self.model).__name__}
         for key in self.model.__dict__:
             if type(self.model.__dict__[key]) in [float, int, str]:
                 args[key] = self.model.__dict__[key]
             else:
                 args[key] = str(self.model.__dict__[key])
 
         self.setup(args=args)
```

### Comparing `aim-4.0.0.dev3/aim/sdk/adapters/tensorflow.py` & `aim-4.0.0.dev4/aim/sdk/adapters/tensorflow.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,51 +10,79 @@
     raise RuntimeError(
         'This contrib module requires tensorflow to be installed. '
         'Please install it with command: \n pip install tensorflow'
     )
 
 
 class AimCallback(TrackerKerasCallbackMetricsEpochEndMixin, Callback):
-    def __init__(self, repo: Optional[str] = None,
-                 experiment: Optional[str] = None,
-                 system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
-                 log_system_params: Optional[bool] = True,
-                 capture_terminal_logs: Optional[bool] = True,):
+    """
+    AimCallback callback class.
+
+    Args:
+        repo (:obj:`str`, optional): Aim repository path or Repo object to which Run object is bound.
+            If skipped, default Repo is used.
+        experiment_name (:obj:`str`, optional): Sets Run's `experiment` property. 'default' if not specified.
+            Can be used later to query runs/sequences.
+        system_tracking_interval (:obj:`int`, optional): Sets the tracking interval in seconds for system usage
+            metrics (CPU, Memory, etc.). Set to `None` to disable system metrics tracking.
+        log_system_params (:obj:`bool`, optional): Enable/Disable logging of system params such as installed packages,
+            git info, environment variables, etc.
+        capture_terminal_logs (:obj:`bool`, optional): Enable/Disable terminal stdout logging.
+    """
+
+    def __init__(
+        self,
+        repo: Optional[str] = None,
+        experiment_name: Optional[str] = None,
+        system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
+        log_system_params: Optional[bool] = True,
+        capture_terminal_logs: Optional[bool] = True,
+    ):
         super(Callback, self).__init__()
 
         self._system_tracking_interval = system_tracking_interval
         self._log_system_params = log_system_params
         self._capture_terminal_logs = capture_terminal_logs
 
-        if repo is None and experiment is None:
-            self._run = Run(system_tracking_interval=self._system_tracking_interval,
-                            log_system_params=self._log_system_params,
-                            capture_terminal_logs=self._capture_terminal_logs,)
+        if repo is None and experiment_name is None:
+            self._run = Run(
+                system_tracking_interval=self._system_tracking_interval,
+                log_system_params=self._log_system_params,
+                capture_terminal_logs=self._capture_terminal_logs,
+            )
         else:
-            self._run = Run(repo=repo, experiment=experiment,
-                            system_tracking_interval=self._system_tracking_interval,
-                            log_system_params=self._log_system_params,
-                            capture_terminal_logs=self._capture_terminal_logs,)
+            self._run = Run(
+                repo=repo,
+                experiment=experiment_name,
+                system_tracking_interval=self._system_tracking_interval,
+                log_system_params=self._log_system_params,
+                capture_terminal_logs=self._capture_terminal_logs,
+            )
 
         self._run_hash = self._run.hash
         self._repo_path = repo
 
     @property
     def experiment(self) -> Run:
         if not self._run:
-            self._run = Run(self._run_hash,
-                            repo=self._repo_path,
-                            system_tracking_interval=self._system_tracking_interval,
-                            capture_terminal_logs=self._capture_terimanl_logs)
+            self._run = Run(
+                self._run_hash,
+                repo=self._repo_path,
+                system_tracking_interval=self._system_tracking_interval,
+                capture_terminal_logs=self._capture_terimanl_logs,
+            )
         return self._run
 
     @classmethod
-    def metrics(cls, repo: Optional[str] = None,
-                experiment: Optional[str] = None,
-                run: Optional[Run] = None):
+    def metrics(
+        cls,
+        repo: Optional[str] = None,
+        experiment: Optional[str] = None,
+        run: Optional[Run] = None,
+    ):
         # Keep `metrics` method for backward compatibility
         return cls(repo, experiment, run)
 
     def close(self) -> None:
         if self._run:
             self._run.close()
             del self._run
```

### Comparing `aim-4.0.0.dev3/aim/sdk/adapters/xgboost.py` & `aim-4.0.0.dev4/aim/sdk/adapters/xgboost.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,24 +9,40 @@
     raise RuntimeError(
         'This contrib module requires XGBoost to be installed. '
         'Please install it with command: \n pip install xgboost'
     )
 
 
 class AimCallback(TrainingCallback):
+    """
+    AimCallback callback class.
 
-    def __init__(self, repo: Optional[str] = None,
-                 experiment: Optional[str] = None,
-                 system_tracking_interval: Optional[int]
-                 = DEFAULT_SYSTEM_TRACKING_INT,
-                 log_system_params: Optional[bool] = True,
-                 capture_terminal_logs: Optional[bool] = True,):
+    Args:
+        repo (:obj:`str`, optional): Aim repository path or Repo object to which Run object is bound.
+            If skipped, default Repo is used.
+        experiment_name (:obj:`str`, optional): Sets Run's `experiment` property. 'default' if not specified.
+            Can be used later to query runs/sequences.
+        system_tracking_interval (:obj:`int`, optional): Sets the tracking interval in seconds for system usage
+            metrics (CPU, Memory, etc.). Set to `None` to disable system metrics tracking.
+        log_system_params (:obj:`bool`, optional): Enable/Disable logging of system params such as installed packages,
+            git info, environment variables, etc.
+        capture_terminal_logs (:obj:`bool`, optional): Enable/Disable terminal stdout logging.
+    """
+
+    def __init__(
+        self,
+        repo: Optional[str] = None,
+        experiment_name: Optional[str] = None,
+        system_tracking_interval: Optional[int] = DEFAULT_SYSTEM_TRACKING_INT,
+        log_system_params: Optional[bool] = True,
+        capture_terminal_logs: Optional[bool] = True,
+    ):
         super().__init__()
         self._repo_path = repo
-        self._experiment = experiment
+        self._experiment = experiment_name
         self._system_tracking_interval = system_tracking_interval
         self._log_system_params = log_system_params
         self._capture_terminal_logs = capture_terminal_logs
         self._run = None
         self._run_hash = None
 
     @property
@@ -68,17 +84,21 @@
                 stdv: Optional[float] = None
                 if isinstance(log[-1], tuple):
                     score = log[-1][0]
                     stdv = log[-1][1]
                 else:
                     score = log[-1]
 
-                self._run.track(score, step=0, name=metric_name, context={'stdv': False})
+                self._run.track(
+                    score, step=0, name=metric_name, context={'stdv': False}
+                )
                 if stdv is not None:
-                    self._run.track(score, step=0, name=metric_name, context={'stdv': True})
+                    self._run.track(
+                        score, step=0, name=metric_name, context={'stdv': True}
+                    )
 
         return False
 
     def after_training(self, model):
         self.close()
         return model
```

### Comparing `aim-4.0.0.dev3/aim/sdk/base_run.py` & `aim-4.0.0.dev4/aim/sdk/base_run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/callbacks/caller.py` & `aim-4.0.0.dev4/aim/sdk/callbacks/caller.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/callbacks/helpers.py` & `aim-4.0.0.dev4/aim/sdk/callbacks/helpers.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/index_manager.py` & `aim-4.0.0.dev4/aim/sdk/index_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     def index(self, run_hash) -> bool:
         try:
             index = self.repo._get_index_tree('meta', timeout=10).view(())
             meta_tree = self.repo.request_tree(
                 'meta', run_hash, read_only=True, from_union=False, no_cache=True).subtree('meta')
             meta_run_tree = meta_tree.subtree('chunks').subtree(run_hash)
             meta_run_tree.finalize(index=index)
-            if meta_run_tree['end_time'] is None:
+            if meta_run_tree.get('end_time') is None:
                 index['meta', 'chunks', run_hash, 'end_time'] = datetime.datetime.now(pytz.utc).timestamp()
             return True
         except TimeoutError:
             logger.warning(f'Cannot index Run {run_hash}. Index is locked.')
             return False
         except Exception as e:
             logger.warning(f'Failed to index Run {run_hash}. {e}')
```

### Comparing `aim-4.0.0.dev3/aim/sdk/legacy/select.py` & `aim-4.0.0.dev4/aim/sdk/legacy/select.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/legacy/session/session.py` & `aim-4.0.0.dev4/aim/sdk/legacy/session/session.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/lock_manager.py` & `aim-4.0.0.dev4/aim/sdk/lock_manager.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/logging/log_record.py` & `aim-4.0.0.dev4/aim/sdk/logging/log_record.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/maintenance_run.py` & `aim-4.0.0.dev4/aim/sdk/maintenance_run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/num_utils.py` & `aim-4.0.0.dev4/aim/sdk/num_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/objects/audio.py` & `aim-4.0.0.dev4/aim/sdk/objects/audio.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/objects/distribution.py` & `aim-4.0.0.dev4/aim/sdk/objects/distribution.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/objects/figure.py` & `aim-4.0.0.dev4/aim/sdk/objects/figure.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/objects/image.py` & `aim-4.0.0.dev4/aim/sdk/objects/image.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/objects/io/wavfile.py` & `aim-4.0.0.dev4/aim/sdk/objects/io/wavfile.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/objects/plugins/dvc_metadata.py` & `aim-4.0.0.dev4/aim/sdk/objects/plugins/dvc_metadata.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/objects/plugins/hf_datasets_metadata.py` & `aim-4.0.0.dev4/aim/sdk/objects/plugins/hf_datasets_metadata.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/objects/plugins/hub_dataset.py` & `aim-4.0.0.dev4/aim/sdk/objects/plugins/hub_dataset.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/objects/text.py` & `aim-4.0.0.dev4/aim/sdk/objects/text.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/query_utils.py` & `aim-4.0.0.dev4/aim/sdk/query_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/remote_repo_proxy.py` & `aim-4.0.0.dev4/aim/sdk/remote_repo_proxy.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/remote_run_reporter.py` & `aim-4.0.0.dev4/aim/sdk/remote_run_reporter.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/repo.py` & `aim-4.0.0.dev4/aim/sdk/repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         Returns:
             :obj:`Repo` object.
         """
         if not path.startswith('ssh://') and not cls.is_remote_path(path):
             path = clean_repo_path(path)
         repo = cls._pool.get(path)
         if repo is None:
-            repo = Repo(path, read_only=read_only, init=init)
+            repo = cls(path, read_only=read_only, init=init)
             cls._pool[path] = repo
         return repo
 
     @classmethod
     def exists(cls, path: str) -> bool:
         """Check Aim repository existence.
```

### Comparing `aim-4.0.0.dev3/aim/sdk/repo_utils.py` & `aim-4.0.0.dev4/aim/sdk/repo_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/reporter/__init__.py` & `aim-4.0.0.dev4/aim/sdk/reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/reporter/file_manager.py` & `aim-4.0.0.dev4/aim/sdk/reporter/file_manager.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/run.py` & `aim-4.0.0.dev4/aim/sdk/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -810,14 +810,15 @@
          experiment (:obj:`str`, optional): Sets Run's `experiment` property. 'default' if not specified.
             Can be used later to query runs/sequences.
          force_resume (:obj:`bool`, optional): Forcefully resume stalled Run.
          system_tracking_interval (:obj:`int`, optional): Sets the tracking interval in seconds for system usage
             metrics (CPU, Memory, etc.). Set to `None` to disable system metrics tracking.
          log_system_params (:obj:`bool`, optional): Enable/Disable logging of system params such as installed packages,
             git info, environment variables, etc.
+         capture_terminal_logs (:obj:`bool`, optional): Enable/Disable terminal stdout logging.
     """
 
     @noexcept
     def __init__(self, run_hash: Optional[str] = None, *,
                  repo: Optional[Union[str, 'Repo', pathlib.Path]] = None,
                  read_only: bool = False,
                  experiment: Optional[str] = None,
```

### Comparing `aim-4.0.0.dev3/aim/sdk/run_status_watcher.py` & `aim-4.0.0.dev4/aim/sdk/run_status_watcher.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/sequence.py` & `aim-4.0.0.dev4/aim/sdk/sequence.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/sequence_collection.py` & `aim-4.0.0.dev4/aim/sdk/sequence_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Iterator
 from typing import TYPE_CHECKING
 from tqdm import tqdm
 
 from aim.sdk.sequence import Sequence
 from aim.sdk.types import QueryReportMode
 from aim.sdk.query_utils import RunView, SequenceView
-from aim.storage.query import RestrictedPythonQuery
+from aim.storage.query import LegacyRestrictedPythonQuery as RestrictedPythonQuery
 
 
 if TYPE_CHECKING:
     from aim.sdk.run import Run
     from aim.sdk.repo import Repo
     from pandas import DataFrame
```

### Comparing `aim-4.0.0.dev3/aim/sdk/sequences/metric.py` & `aim-4.0.0.dev4/aim/sdk/sequences/metric.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/tracker.py` & `aim-4.0.0.dev4/aim/sdk/tracker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/training_flow.py` & `aim-4.0.0.dev4/aim/sdk/training_flow.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/uri_service.py` & `aim-4.0.0.dev4/aim/sdk/uri_service.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/sdk/utils.py` & `aim-4.0.0.dev4/aim/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/arrayview.cpp` & `aim-4.0.0.dev4/aim/storage/arrayview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.arrayview",
         "sources": [
             "aim/storage/arrayview.py"
         ]
     },
     "module_name": "aim.storage.arrayview"
```

### Comparing `aim-4.0.0.dev3/aim/storage/arrayview.py` & `aim-4.0.0.dev4/aim/storage/arrayview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/container.cpp` & `aim-4.0.0.dev4/aim/storage/container.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.container",
         "sources": [
             "aim/storage/container.py"
         ]
     },
     "module_name": "aim.storage.container"
```

### Comparing `aim-4.0.0.dev3/aim/storage/container.pxd` & `aim-4.0.0.dev4/aim/storage/container.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/container.py` & `aim-4.0.0.dev4/aim/storage/container.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/containertreeview.cpp` & `aim-4.0.0.dev4/aim/storage/containertreeview.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.containertreeview",
         "sources": [
             "aim/storage/containertreeview.py"
         ]
     },
     "module_name": "aim.storage.containertreeview"
```

### Comparing `aim-4.0.0.dev3/aim/storage/containertreeview.py` & `aim-4.0.0.dev4/aim/storage/containertreeview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/encoding/__init__.cpp` & `aim-4.0.0.dev4/aim/storage/encoding/__init__.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.encoding",
         "sources": [
             "aim/storage/encoding/__init__.py"
         ]
     },
     "module_name": "aim.storage.encoding"
```

### Comparing `aim-4.0.0.dev3/aim/storage/encoding/encoding.cpp` & `aim-4.0.0.dev4/aim/storage/encoding/encoding.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.encoding.encoding",
         "sources": [
             "aim/storage/encoding/encoding.pyx"
         ]
     },
     "module_name": "aim.storage.encoding.encoding"
```

### Comparing `aim-4.0.0.dev3/aim/storage/encoding/encoding.pyx` & `aim-4.0.0.dev4/aim/storage/encoding/encoding.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/encoding/encoding_native.cpp` & `aim-4.0.0.dev4/aim/storage/encoding/encoding_native.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.encoding.encoding_native",
         "sources": [
             "aim/storage/encoding/encoding_native.pyx"
         ]
     },
     "module_name": "aim.storage.encoding.encoding_native"
```

### Comparing `aim-4.0.0.dev3/aim/storage/encoding/encoding_native.pxd` & `aim-4.0.0.dev4/aim/storage/encoding/encoding_native.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/encoding/encoding_native.pyx` & `aim-4.0.0.dev4/aim/storage/encoding/encoding_native.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/hashing/__init__.cpp` & `aim-4.0.0.dev4/aim/storage/hashing/__init__.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,22 @@
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
             "aim/storage/hashing",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.hashing",
         "sources": [
             "aim/storage/hashing/__init__.py"
         ]
     },
     "module_name": "aim.storage.hashing"
```

### Comparing `aim-4.0.0.dev3/aim/storage/hashing/c_hash.cpp` & `aim-4.0.0.dev4/aim/storage/hashing/c_hash.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,23 +14,23 @@
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
             "aim/storage/hashing",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "language_level": "3",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.hashing.c_hash",
         "sources": [
             "aim/storage/hashing/c_hash.pyx"
         ]
     },
     "module_name": "aim.storage.hashing.c_hash"
```

### Comparing `aim-4.0.0.dev3/aim/storage/hashing/c_hash.pyx` & `aim-4.0.0.dev4/aim/storage/hashing/c_hash.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/hashing/hash/hash.h` & `aim-4.0.0.dev4/aim/storage/hashing/hash/hash.h`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/hashing/hashing.cpp` & `aim-4.0.0.dev4/aim/storage/hashing/hashing.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,22 @@
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
             "aim/storage/hashing",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.hashing.hashing",
         "sources": [
             "aim/storage/hashing/hashing.py"
         ]
     },
     "module_name": "aim.storage.hashing.hashing"
```

### Comparing `aim-4.0.0.dev3/aim/storage/hashing/hashing.pxd` & `aim-4.0.0.dev4/aim/storage/hashing/hashing.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/hashing/hashing.py` & `aim-4.0.0.dev4/aim/storage/hashing/hashing.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/inmemorytreeview.cpp` & `aim-4.0.0.dev4/aim/storage/inmemorytreeview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.inmemorytreeview",
         "sources": [
             "aim/storage/inmemorytreeview.py"
         ]
     },
     "module_name": "aim.storage.inmemorytreeview"
```

### Comparing `aim-4.0.0.dev3/aim/storage/inmemorytreeview.py` & `aim-4.0.0.dev4/aim/storage/inmemorytreeview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/lock_proxy.py` & `aim-4.0.0.dev4/aim/storage/lock_proxy.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/locking.py` & `aim-4.0.0.dev4/aim/storage/locking.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/migrations/alembic.ini` & `aim-4.0.0.dev4/aim/storage/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/migrations/alembic_dev.ini` & `aim-4.0.0.dev4/aim/storage/migrations/alembic_dev.ini`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/migrations/env.py` & `aim-4.0.0.dev4/aim/storage/migrations/env.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/migrations/utils.py` & `aim-4.0.0.dev4/aim/storage/migrations/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/migrations/versions/1ecf8222220d_initial_schema.py` & `aim-4.0.0.dev4/aim/storage/migrations/versions/1ecf8222220d_initial_schema.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/migrations/versions/3c4f22db7a46_run_end_time.py` & `aim-4.0.0.dev4/aim/storage/migrations/versions/3c4f22db7a46_run_end_time.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/migrations/versions/46b89d830ad8_.py` & `aim-4.0.0.dev4/aim/storage/migrations/versions/46b89d830ad8_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/migrations/versions/9ba30ab3b2b4_.py` & `aim-4.0.0.dev4/aim/storage/migrations/versions/9ba30ab3b2b4_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/migrations/versions/b07e7b07c8ce_.py` & `aim-4.0.0.dev4/aim/storage/migrations/versions/b07e7b07c8ce_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/migrations/versions/fbfe5c4702fb_soft_delete.py` & `aim-4.0.0.dev4/aim/storage/migrations/versions/fbfe5c4702fb_soft_delete.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/object.py` & `aim-4.0.0.dev4/aim/storage/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         return decorator
 
     @staticmethod
     def by_name(name: str):
         return CustomObject.registry[name]
 
     @classmethod
-    def get_typename(cls):
+    def get_typename(cls) -> str:
         # TODO [AT, MV] check AIM_NAME to have python type name format (f.e. "aim.sdk.Image" but not "abc//}?")
         return cls.AIM_NAME
 
     def __new__(cls, *args, **kwargs):
         obj = super().__new__(cls)
         obj.storage = kwargs.get('_storage', InMemoryTreeView(container={}))
         return obj
```

### Comparing `aim-4.0.0.dev3/aim/storage/prefixview.cpp` & `aim-4.0.0.dev4/aim/storage/prefixview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.prefixview",
         "sources": [
             "aim/storage/prefixview.py"
         ]
     },
     "module_name": "aim.storage.prefixview"
```

### Comparing `aim-4.0.0.dev3/aim/storage/prefixview.pxd` & `aim-4.0.0.dev4/aim/storage/prefixview.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/prefixview.py` & `aim-4.0.0.dev4/aim/storage/prefixview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/proxy.py` & `aim-4.0.0.dev4/aim/storage/proxy.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/query.py` & `aim-4.0.0.dev4/aim/storage/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -159,34 +159,40 @@
 
     __slots__ = ('_checker', 'run_metadata_cache')
 
     allowed_params = {'run', 'metric', 'images', 'audios', 'distributions', 'figures', 'texts'}
 
     def __init__(
         self,
-        query: str
+        query: str,
     ):
-        stripped_query = strip_query(query)
-        expr = query_add_default_expr(stripped_query)
+        expr = self.query_expression(query)
         super().__init__(expr=expr)
         self._checker = compile_checker(expr)
         self.run_metadata_cache = None
 
     def __bool__(
         self
     ) -> bool:
         return bool(self.expr)
 
     def check(
         self,
         **params
     ) -> bool:
-        # prevent possible messing with globals
-        assert set(params.keys()).issubset(self.allowed_params)
-
         # TODO enforce immutable
         try:
             namespace = dict(**params, **restricted_globals)
             return eval(self._checker, restricted_globals, namespace)
         except BaseException as e:
             logger.warning('query failed, %s', e)
             return False
+
+    @classmethod
+    def query_expression(cls, query: str) -> str:
+        return strip_query(query)
+
+
+class LegacyRestrictedPythonQuery(RestrictedPythonQuery):
+    @classmethod
+    def query_expression(cls, query: str) -> str:
+        return query_add_default_expr(strip_query(query))
```

### Comparing `aim-4.0.0.dev3/aim/storage/rockscontainer.cpp` & `aim-4.0.0.dev4/aim/storage/rockscontainer.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.rockscontainer",
         "sources": [
             "aim/storage/rockscontainer.pyx"
         ]
     },
     "module_name": "aim.storage.rockscontainer"
```

### Comparing `aim-4.0.0.dev3/aim/storage/rockscontainer.pyx` & `aim-4.0.0.dev4/aim/storage/rockscontainer.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/structured/db.py` & `aim-4.0.0.dev4/aim/storage/structured/db.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/structured/entities.py` & `aim-4.0.0.dev4/aim/storage/structured/entities.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/structured/proxy.py` & `aim-4.0.0.dev4/aim/storage/structured/proxy.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/structured/sql_engine/entities.py` & `aim-4.0.0.dev4/aim/storage/structured/sql_engine/entities.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/structured/sql_engine/factory.py` & `aim-4.0.0.dev4/aim/storage/structured/sql_engine/factory.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/structured/sql_engine/models.py` & `aim-4.0.0.dev4/aim/storage/structured/sql_engine/models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/structured/sql_engine/utils.py` & `aim-4.0.0.dev4/aim/storage/structured/sql_engine/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/treearrayview.cpp` & `aim-4.0.0.dev4/aim/storage/treearrayview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.treearrayview",
         "sources": [
             "aim/storage/treearrayview.py"
         ]
     },
     "module_name": "aim.storage.treearrayview"
```

### Comparing `aim-4.0.0.dev3/aim/storage/treearrayview.py` & `aim-4.0.0.dev4/aim/storage/treearrayview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/treeutils.cpp` & `aim-4.0.0.dev4/aim/storage/treeutils.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.treeutils",
         "sources": [
             "aim/storage/treeutils.pyx"
         ]
     },
     "module_name": "aim.storage.treeutils"
```

### Comparing `aim-4.0.0.dev3/aim/storage/treeutils.pyx` & `aim-4.0.0.dev4/aim/storage/treeutils.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/treeutils_non_native.py` & `aim-4.0.0.dev4/aim/storage/treeutils_non_native.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/treeview.cpp` & `aim-4.0.0.dev4/aim/storage/treeview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.treeview",
         "sources": [
             "aim/storage/treeview.py"
         ]
     },
     "module_name": "aim.storage.treeview"
```

### Comparing `aim-4.0.0.dev3/aim/storage/treeview.py` & `aim-4.0.0.dev4/aim/storage/treeview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/treeviewproxy.py` & `aim-4.0.0.dev4/aim/storage/treeviewproxy.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/types.py` & `aim-4.0.0.dev4/aim/storage/types.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/union.cpp` & `aim-4.0.0.dev4/aim/storage/union.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.union",
         "sources": [
             "aim/storage/union.pyx"
         ]
     },
     "module_name": "aim.storage.union"
```

### Comparing `aim-4.0.0.dev3/aim/storage/union.pyx` & `aim-4.0.0.dev4/aim/storage/union.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/storage/utils.cpp` & `aim-4.0.0.dev4/aim/storage/utils.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-4ipj6rc2/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.utils",
         "sources": [
             "aim/storage/utils.py"
         ]
     },
     "module_name": "aim.storage.utils"
```

### Comparing `aim-4.0.0.dev3/aim/storage/utils.py` & `aim-4.0.0.dev4/aim/storage/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/utils/deprecation.py` & `aim-4.0.0.dev4/aim/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/utils/tracking.py` & `aim-4.0.0.dev4/aim/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/__init__.py` & `aim-4.0.0.dev4/aim/web/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     from aim.web.api.runs.views import runs_router
     from aim.web.api.runs.views import add_api_routes
     from aim.web.api.tags.views import tags_router
     from aim.web.api.experiments.views import experiment_router
     from aim.web.api.dashboard_apps.views import dashboard_apps_router
     from aim.web.api.dashboards.views import dashboards_router
     from aim.web.api.projects.views import projects_router
+    from aim.web.api.queries.views import query_router
     from aim.web.api.views import statics_router
     from aim.web.configs import AIM_UI_BASE_PATH
 
     from aim.web.api.projects.project import Project
     from aim.sdk.index_manager import RepoIndexManager
 
     # The indexing thread has to run in the same process as the uvicorn app itself.
@@ -80,14 +81,15 @@
 
     api_app.include_router(dashboard_apps_router, prefix='/apps')
     api_app.include_router(dashboards_router, prefix='/dashboards')
     api_app.include_router(experiment_router, prefix='/experiments')
     api_app.include_router(projects_router, prefix='/projects')
     api_app.include_router(runs_router, prefix='/runs')
     api_app.include_router(tags_router, prefix='/tags')
+    api_app.include_router(query_router, prefix='/data')
 
     base_path = os.environ.get(AIM_UI_BASE_PATH, '')
 
     app.mount(f'{base_path}/api', api_app)
     static_files_app = FastAPI()
 
     static_files_app.include_router(statics_router)
```

### Comparing `aim-4.0.0.dev3/aim/web/api/dashboard_apps/models.py` & `aim-4.0.0.dev4/aim/web/api/dashboard_apps/models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/dashboard_apps/pydantic_models.py` & `aim-4.0.0.dev4/aim/web/api/dashboard_apps/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/dashboard_apps/views.py` & `aim-4.0.0.dev4/aim/web/api/dashboard_apps/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/dashboards/models.py` & `aim-4.0.0.dev4/aim/web/api/dashboards/models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/dashboards/pydantic_models.py` & `aim-4.0.0.dev4/aim/web/api/dashboards/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/dashboards/serializers.py` & `aim-4.0.0.dev4/aim/web/api/dashboards/serializers.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/dashboards/views.py` & `aim-4.0.0.dev4/aim/web/api/dashboards/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/db.py` & `aim-4.0.0.dev4/aim/web/api/db.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/experiments/pydantic_models.py` & `aim-4.0.0.dev4/aim/web/api/experiments/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/experiments/views.py` & `aim-4.0.0.dev4/aim/web/api/experiments/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/projects/project.py` & `aim-4.0.0.dev4/aim/web/api/projects/project.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from aim.sdk.repo import Repo
+from aim.sdk.core.repo import Repo
 from aim.sdk.configs import get_aim_repo_name
 from aim.web.utils import get_root_path
 
 
 class Project:
     def __init__(self):
         root_path = get_root_path()
```

### Comparing `aim-4.0.0.dev3/aim/web/api/projects/pydantic_models.py` & `aim-4.0.0.dev4/aim/web/api/projects/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/projects/views.py` & `aim-4.0.0.dev4/aim/web/api/projects/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/runs/object_api_utils.py` & `aim-4.0.0.dev4/aim/web/api/runs/object_api_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/runs/object_views.py` & `aim-4.0.0.dev4/aim/web/api/runs/object_views.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,14 +38,45 @@
 
     @staticmethod
     def check_density(density):
         if density <= 0:
             raise HTTPException(status_code=400, detail='Density must be greater than 0.')
 
     @classmethod
+    def sequence_search_fn(cls,
+                           repo,
+                           query: str,
+                           skip_system: Optional[bool] = True,
+                           record_range: Optional[str] = '', record_density: Optional[int] = 50,
+                           index_range: Optional[str] = '', index_density: Optional[int] = 5,
+                           report_progress: Optional[bool] = True,
+                           x_timezone_offset: int = Header(default=0),):
+        assert issubclass(cls.sequence_type, Sequence)
+
+        record_range = checked_range(record_range)
+        index_range = checked_range(index_range)
+        CustomObjectApiConfig.check_density(record_density)
+        CustomObjectApiConfig.check_density(index_density)
+
+        # TODO [MV, AT]: move to `repo.py` when `SELECT` statements are introduced
+        repo._prepare_runs_cache()
+        query_iterator = QuerySequenceCollection(repo=repo,
+                                                 seq_cls=cls.sequence_type,
+                                                 query=query,
+                                                 report_mode=QueryReportMode.PROGRESS_TUPLE,
+                                                 timezone_offset=x_timezone_offset)
+
+        api = CustomObjectApi(cls.sequence_type.sequence_name(), resolve_blobs=cls.resolve_blobs)
+        api.set_dump_data_fn(cls.dump_record_fn)
+        api.set_trace_collection(query_iterator)
+        api.set_ranges(record_range, record_density, index_range, index_density)
+        streamer = api.search_result_streamer(skip_system, report_progress)
+        return StreamingResponse(streamer)
+
+    @classmethod
     def register_endpoints(cls, router):
         assert issubclass(cls.sequence_type, Sequence)
         seq_name = cls.sequence_type.sequence_name()
 
         # search API
         search_endpoint = f'/search/{seq_name}/'
 
@@ -56,33 +87,19 @@
                              record_range: Optional[str] = '', record_density: Optional[int] = 50,
                              index_range: Optional[str] = '', index_density: Optional[int] = 5,
                              report_progress: Optional[bool] = True,
                              x_timezone_offset: int = Header(default=0),):
             # search Sequence API
             repo = get_project_repo()
             query = checked_query(q)
-            record_range = checked_range(record_range)
-            index_range = checked_range(index_range)
-            CustomObjectApiConfig.check_density(record_density)
-            CustomObjectApiConfig.check_density(index_density)
-
-            # TODO [MV, AT]: move to `repo.py` when `SELECT` statements are introduced
-            repo._prepare_runs_cache()
-            query_iterator = QuerySequenceCollection(repo=repo,
-                                                     seq_cls=cls.sequence_type,
-                                                     query=query,
-                                                     report_mode=QueryReportMode.PROGRESS_TUPLE,
-                                                     timezone_offset=x_timezone_offset)
-
-            api = CustomObjectApi(seq_name, resolve_blobs=cls.resolve_blobs)
-            api.set_dump_data_fn(cls.dump_record_fn)
-            api.set_trace_collection(query_iterator)
-            api.set_ranges(record_range, record_density, index_range, index_density)
-            streamer = api.search_result_streamer(skip_system, report_progress)
-            return StreamingResponse(streamer)
+            return cls.sequence_search_fn(repo, query,
+                                          skip_system=skip_system,
+                                          record_range=record_range, record_density=record_density,
+                                          index_range=index_range, index_density=index_density,
+                                          report_progress=report_progress, x_timezone_offset=x_timezone_offset)
 
         # run sequence batch API
         sequence_batch_endpoint = f'/{{run_id}}/{seq_name}/get-batch/'
 
         @router.post(sequence_batch_endpoint, response_model=List[ObjectSequenceBaseView])
         async def sequence_batch_api(run_id: str,
                                      requested_traces: RunTracesBatchApiIn,
```

### Comparing `aim-4.0.0.dev3/aim/web/api/runs/pydantic_models.py` & `aim-4.0.0.dev4/aim/web/api/runs/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/runs/utils.py` & `aim-4.0.0.dev4/aim/web/api/runs/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/runs/views.py` & `aim-4.0.0.dev4/aim/web/api/runs/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,82 +51,111 @@
 
 runs_router = APIRouter()
 
 # static msgs
 NOTE_NOT_FOUND = 'Note with id {id} is not found in this run.'
 
 
-@runs_router.get('/search/run/', response_model=RunSearchApiOut,
-                 responses={400: {'model': QuerySyntaxErrorOut}})
-async def run_search_api(q: Optional[str] = '',
-                         limit: Optional[int] = 0,
-                         offset: Optional[str] = None,
-                         skip_system: Optional[bool] = True,
-                         report_progress: Optional[bool] = True,
-                         exclude_params: Optional[bool] = False,
-                         exclude_traces: Optional[bool] = False,
-                         x_timezone_offset: int = Header(default=0),):
-    from aim.sdk.sequence_collection import QueryRunSequenceCollection
-    repo = get_project_repo()
-    query = checked_query(q)
+def runs_search_fn(repo,
+                   query: str,
+                   *,
+                   limit: Optional[int] = 0,
+                   offset: Optional[str] = None,
+                   skip_system: Optional[bool] = True,
+                   report_progress: Optional[bool] = True,
+                   exclude_params: Optional[bool] = False,
+                   exclude_traces: Optional[bool] = False,
+                   x_timezone_offset: int = Header(default=0)):
 
+    from aim.sdk.sequence_collection import QueryRunSequenceCollection
     repo._prepare_runs_cache()
     runs = QueryRunSequenceCollection(repo=repo,
                                       query=query,
                                       paginated=bool(limit),
                                       offset=offset,
                                       report_mode=QueryReportMode.PROGRESS_TUPLE,
                                       timezone_offset=x_timezone_offset)
 
     streamer = run_search_result_streamer(runs, limit,
                                           skip_system, report_progress,
                                           exclude_params, exclude_traces)
     return StreamingResponse(streamer)
 
 
+@runs_router.get('/search/run/', response_model=RunSearchApiOut,
+                 responses={400: {'model': QuerySyntaxErrorOut}})
+async def run_search_api(q: Optional[str] = '',
+                         limit: Optional[int] = 0,
+                         offset: Optional[str] = None,
+                         skip_system: Optional[bool] = True,
+                         report_progress: Optional[bool] = True,
+                         exclude_params: Optional[bool] = False,
+                         exclude_traces: Optional[bool] = False,
+                         x_timezone_offset: int = Header(default=0),):
+    repo = get_project_repo()
+    query = checked_query(q)
+
+    return runs_search_fn(repo, query,
+                          limit=limit, offset=offset, skip_system=skip_system,
+                          report_progress=report_progress, exclude_params=exclude_params,
+                          exclude_traces=exclude_traces, x_timezone_offset=x_timezone_offset)
+
+
 @runs_router.post('/search/metric/align/', response_model=RunMetricCustomAlignApiOut)
 async def run_metric_custom_align_api(request_data: MetricAlignApiIn):
     repo = get_project_repo()
     x_axis_metric_name = request_data.align_by
     requested_runs = request_data.runs
 
     streamer = custom_aligned_metrics_streamer(requested_runs, x_axis_metric_name, repo)
     return StreamingResponse(streamer)
 
 
-@runs_router.get('/search/metric/', response_model=RunMetricSearchApiOut,
-                 responses={400: {'model': QuerySyntaxErrorOut}})
-async def run_metric_search_api(q: Optional[str] = '',
-                                p: Optional[int] = 50,
-                                x_axis: Optional[str] = None,
-                                skip_system: Optional[bool] = True,
-                                report_progress: Optional[bool] = True,
-                                x_timezone_offset: int = Header(default=0),):
+def metrics_search_fn(repo,
+                      query: str,
+                      *,
+                      p: Optional[int] = 50,
+                      x_axis: Optional[str] = None,
+                      skip_system: Optional[bool] = True,
+                      report_progress: Optional[bool] = True,
+                      x_timezone_offset: int = Header(default=0),):
     from aim.sdk.sequences.metric import Metric
     from aim.sdk.sequence_collection import QuerySequenceCollection
 
     steps_num = p
 
     if x_axis:
         x_axis = x_axis.strip()
 
-    repo = get_project_repo()
-    query = checked_query(q)
-
     repo._prepare_runs_cache()
     traces = QuerySequenceCollection(repo=repo,
                                      seq_cls=Metric,
                                      query=query,
                                      report_mode=QueryReportMode.PROGRESS_TUPLE,
                                      timezone_offset=x_timezone_offset,)
 
     streamer = metric_search_result_streamer(traces, skip_system, steps_num, x_axis, report_progress)
     return StreamingResponse(streamer)
 
 
+@runs_router.get('/search/metric/', response_model=RunMetricSearchApiOut,
+                 responses={400: {'model': QuerySyntaxErrorOut}})
+async def run_metric_search_api(q: Optional[str] = '',
+                                p: Optional[int] = 50,
+                                x_axis: Optional[str] = None,
+                                skip_system: Optional[bool] = True,
+                                report_progress: Optional[bool] = True,
+                                x_timezone_offset: int = Header(default=0),):
+    repo = get_project_repo()
+    query = checked_query(q)
+    return metrics_search_fn(repo, query,
+                             p=p, x_axis=x_axis, skip_system=skip_system,
+                             report_progress=report_progress, x_timezone_offset=x_timezone_offset)
+
+
 @runs_router.get('/active/', response_model=RunActiveOut)
 async def get_active_runs_api(report_progress: Optional[bool] = True):
     repo = get_project_repo()
     repo._prepare_runs_cache()
 
     streamer = run_active_result_streamer(repo)
```

### Comparing `aim-4.0.0.dev3/aim/web/api/tags/pydantic_models.py` & `aim-4.0.0.dev4/aim/web/api/tags/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/tags/views.py` & `aim-4.0.0.dev4/aim/web/api/tags/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/utils.py` & `aim-4.0.0.dev4/aim/web/api/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/api/views.py` & `aim-4.0.0.dev4/aim/web/api/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/middlewares/profiler/profiler.py` & `aim-4.0.0.dev4/aim/web/middlewares/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/migrations/alembic.ini` & `aim-4.0.0.dev4/aim/web/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/migrations/alembic_dev.ini` & `aim-4.0.0.dev4/aim/web/migrations/alembic_dev.ini`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/migrations/env.py` & `aim-4.0.0.dev4/aim/web/migrations/env.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/migrations/versions/11672b13f92c_.py` & `aim-4.0.0.dev4/aim/web/migrations/versions/11672b13f92c_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/migrations/versions/517a45b2e62c_.py` & `aim-4.0.0.dev4/aim/web/migrations/versions/517a45b2e62c_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/migrations/versions/5ae8371b7481_.py` & `aim-4.0.0.dev4/aim/web/migrations/versions/5ae8371b7481_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/migrations/versions/73a3d004c227_.py` & `aim-4.0.0.dev4/aim/web/migrations/versions/73a3d004c227_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim/web/utils.py` & `aim-4.0.0.dev4/aim/web/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/aim.egg-info/PKG-INFO` & `aim-4.0.0.dev4/aim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aim
-Version: 4.0.0.dev3
+Version: 4.0.0.dev4
 Summary: A super-easy way to record, search and compare AI experiments.
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,27 +20,38 @@
     <tbody>
       <tr>
         <td>Drop a star to support Aim ⭐</td>
         <td>
           <a href="https://community.aimstack.io/">Join Aim discord community</a>
           <img width="20px" src="https://user-images.githubusercontent.com/13848158/226759622-063b725d-8b3e-4c75-80c7-11fb04b7adf5.png">
         </td>
-        <td><a href="#-aim-40">🔮 Aim 4.0 - COMING SOON!!</a></td>
+      </tr>
+      <tr>
+        <td colspan="2"><p align="center"><a href="#-aim-40">🔮 Aim 4.0 - COMING SOON!!</a></p></td>
       </tr>
     </tbody>
   </table>
 </div>
 
+<br />
+
 <div align="center">
   <img src="https://user-images.githubusercontent.com/13848158/225620298-9f9293e9-a138-41fd-bd77-21d53d0490b7.png">
   <h3>
     An easy-to-use & supercharged open-source AI metadata tracker. 
   </h3>
   
-  Aim logs all your AI metadata(**experiments**, **prompts**, etc), enables a UI to compare & observe them and SDK to query them programmatically.
+  Aim logs all your AI metadata, enables a UI to observe/compare them, and an SDK to query them programmatically.
+  
+  <p align="center">
+    <strong>Learn more:</strong> </br>
+    <a href="#experiment-tracking-with-aim">Experiment tracking with Aim</a> </br>
+    <a href="#ai-systems-and-agents-tracing-with-Aim">AI agents tracing with Aim</a>
+  </p>
+  
 </div>
 
 <br/>
 
 <div align="center">
   
   [![Discord Server](https://dcbadge.vercel.app/api/server/zXq2NfVdtF?compact=true&style=flat)](https://community.aimstack.io/)
@@ -109,15 +120,15 @@
 <p align="center">
   AimStack offers enterprise support that's beyond core Aim. Contact via <a href="mailto:hello@aimstack.io">hello@aimstack.io</a> e-mail.
 </p>
 
 ---
 
 <h3 align="center">
-  <a href="#-about"><b>About</b></a> &bull;
+  <a href="#ℹ️-about"><b>About</b></a> &bull;
   <a href="#-demos"><b>Demos</b></a> &bull;
   <a href="#-ecosystem"><b>Ecosystem</b></a> &bull;
   <a href="#-quick-start"><b>Quick Start</b></a> &bull;
   <a href="https://github.com/aimhubio/aim/tree/main/examples"><b>Examples</b></a> &bull;
   <a href="https://aimstack.readthedocs.io/en/latest/"><b>Documentation</b></a> &bull;
   <a href="#-community"><b>Community</b></a> &bull;
   <a href="https://aimstack.io/blog"><b>Blog</b></a> &bull;
@@ -125,32 +136,62 @@
 </h3>  
 
 ---
 
 # ℹ️ About
 
 Aim is an open-source, self-hosted AI Metadata tracking tool designed to handle 100,000s of tracked metadata sequences.
-Two most famous AI metadata applications are: experiment tracking and prompt engineering.
 
-Aim provides a performant and beautiful UI for exploring and comparing training runs, prompt sessions.
+Aim provides a performant and beautiful UI for exploring and comparing metadata such as training runs or agents executions.
 Additionally, its SDK enables programmatic access to tracked metadata — perfect for automations and Jupyter Notebook analysis.
 
 <p align="center">
   <strong>Aim's mission is to democratize AI dev tools 🎯 </strong>
 </p>
 
 <div align="center">
   <img src="https://user-images.githubusercontent.com/13848158/226426018-f7c11c9b-78d9-4ee4-b292-df28b3e8eaa6.jpg" height="140" />
   <img src="https://user-images.githubusercontent.com/13848158/226426005-f7e83923-0f92-44a4-88e4-1735a3d3e119.jpg" height="140" />
   <img src="https://user-images.githubusercontent.com/13848158/226426015-4f1122d8-c96a-443f-8698-3db942b1972a.jpg" height="140" />
 </div>
 
 </br>
 
-<div align="center">
+### AI systems and agents tracing with Aim
+
+<div align="left">
+  <table>
+    <tbody>
+      <tr>
+        <th>Log Inputs, Outputs and Actions of Executions 🤖</th>
+        <th>Visualize & Compare Executions Steps via UI 🔍</th>
+      </tr>
+      <tr>
+        <td>
+          <ul>
+            <li>Track all the inputs, outputs of LLMs and tools</li>
+            <li>Capture terminal output of executions</li>
+            <li>Get notified on executions progress and finish</li>
+            </ul>
+          </td>
+        <td>
+          <ul>
+            <li>Deep dive into single execution steps</li>
+            <li>Compare executions side-by-side</li>
+            <li>View previous exectutions terminal outputs</li>
+          </ul>
+        </td>
+      </tr>
+    </tbody>
+  </table>
+</div>
+
+### Experiment tracking with Aim
+
+<div align="left">
   <table>
     <tbody>
       <tr>
         <th>Log Metadata Across Your ML Pipeline 💾</th>
         <th>Visualize & Compare Metadata via UI 📊</th>
       </tr>
       <tr>
@@ -378,15 +419,15 @@
 
 </br>
 
 **Training run comparison**
 
 Order of magnitude faster training run comparison with Aim
 - The tracked params are first class citizens at Aim. You can search, group, aggregate via params - deeply explore all the tracked data (metrics, params, images) on the UI.
-- With tensorboard the users are forced to record those parameters in the training run name to be able to search and compare. This causes a super-tedius comparison experience and usability issues on the UI when there are many experiments and params. **TensorBoard doesn't have features to group, aggregate the metrics**
+- With tensorboard the users are forced to record those parameters in the training run name to be able to search and compare. This causes a super-tedius comparison experience and usability issues on the UI when there are many experiments and params. **TensorBoard doesn't have features to group, aggregate the metrics**.
 
 **Scalability**
 
 - Aim is built to handle 1000s of training runs - both on the backend and on the UI.
 - TensorBoard becomes really slow and hard to use when a few hundred training runs are queried / compared.
 
 **Beloved TB visualizations to be added on Aim**
@@ -403,20 +444,20 @@
 
 </br>
 
 MLFlow is an end-to-end ML Lifecycle tool.
 Aim is focused on training tracking.
 The main differences of Aim and MLflow are around the UI scalability and run comparison features.
 
-Aim and MLflow are a perfect match - check out the [aimlflow](https://github.com/aimhubio/aimlflow) - the tool that enables Aim supoerpowers on Mlflow.
+Aim and MLflow are a perfect match - check out the [aimlflow](https://github.com/aimhubio/aimlflow) - the tool that enables Aim superpowers on MLflow.
 
 **Run comparison**
 
-- Aim treats tracked parameters as first-class citizens. Users can query runs, metrics, images and filter using the params.
-- MLFlow does have a search by tracked config, but there are no grouping, aggregation, subplotting by hyparparams and other comparison features available.
+- Aim treats tracked parameters as first-class citizens. Users can query runs, metrics, images, and filter using the params.
+- MLFlow does have a search by tracked config, but there are no grouping, aggregation, subplotting by hyperparams and other comparison features available.
 
 **UI Scalability**
 
 - Aim UI can handle several thousands of metrics at the same time smoothly with 1000s of steps. It may get shaky when you explore 1000s of metrics with 10000s of steps each. But we are constantly optimizing!
 - MLflow UI becomes slow to use when there are a few hundreds of runs.
 
 </details>
@@ -427,15 +468,15 @@
 </summary>
 
 </br>
 
 Hosted vs self-hosted
 
 - Weights and Biases is a hosted closed-source MLOps platform.
-- Aim is self-hosted, free and open-source experiment tracking tool.
+- Aim is self-hosted, free, and open-source experiment tracking tool.
 
 </details>
 
 # 🛣️ Roadmap
 
 ## Detailed milestones
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: aim Version: 4.0.0.dev3 Summary: A super-easy way
+Metadata-Version: 2.1 Name: aim Version: 4.0.0.dev4 Summary: A super-easy way
 to record, search and compare AI experiments. Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
 Python: >=3.7.0 Description-Content-Type: text/markdown License-File: LICENSE
-                       Join_Aim_discord_community
-                       [https://user-
-Drop a star to support images.githubusercontent.com/ ð®_Aim_4.0_-_COMING
-Aim â­             13848158/226759622-063b725d-  SOON!!
-                       8b3e-4c75-80c7-
-                       11fb04b7adf5.png]
+                               Join_Aim_discord_community [https://user-
+Drop a star to support Aim â­images.githubusercontent.com/13848158/226759622-
+                               063b725d-8b3e-4c75-80c7-11fb04b7adf5.png]
+                         ð®_Aim_4.0_-_COMING_SOON!!
+
  [https://user-images.githubusercontent.com/13848158/225620298-9f9293e9-a138-
                           41fd-bd77-21d53d0490b7.png]
    **** An easy-to-use & supercharged open-source AI metadata tracker. ****
-Aim logs all your AI metadata(**experiments**, **prompts**, etc), enables a UI
-       to compare & observe them and SDK to query them programmatically.
+Aim logs all your AI metadata, enables a UI to observe/compare them, and an SDK
+                        to query them programmatically.
+     Learn more:  Experiment_tracking_with_Aim  AI_agents_tracing_with_Aim
 
            [![Discord Server](https://dcbadge.vercel.app/api/server/
 zXq2NfVdtF?compact=true&style=flat)](https://community.aimstack.io/) [![Twitter
 Follow](https://img.shields.io/twitter/follow/aimstackio?style=social)](https:/
    /twitter.com/aimstackio) [![Medium](https://img.shields.io/badge/Medium-
 12100E?style=flat&logo=medium&logoColor=white)](https://medium.com/aimstack) [!
  [Platform Support](https://img.shields.io/badge/platform-Linux%20%7C%20macOS-
@@ -82,25 +82,35 @@
 
     AimStack offers enterprise support that's beyond core Aim. Contact via
                            hello@aimstack.io e-mail.
 ---
    **** About • Demos • Ecosystem • Quick_Start • Examples • Documentation •
                      Community • Blog • COMING_SOON!! ****
 --- # â¹ï¸ About Aim is an open-source, self-hosted AI Metadata tracking tool
-designed to handle 100,000s of tracked metadata sequences. Two most famous AI
-metadata applications are: experiment tracking and prompt engineering. Aim
-provides a performant and beautiful UI for exploring and comparing training
-runs, prompt sessions. Additionally, its SDK enables programmatic access to
-tracked metadata â perfect for automations and Jupyter Notebook analysis.
+designed to handle 100,000s of tracked metadata sequences. Aim provides a
+performant and beautiful UI for exploring and comparing metadata such as
+training runs or agents executions. Additionally, its SDK enables programmatic
+access to tracked metadata â perfect for automations and Jupyter Notebook
+analysis.
                Aim's mission is to democratize AI dev tools ð¯
  [https://user-images.githubusercontent.com/13848158/226426018-f7c11c9b-78d9-
     4ee4-b292-df28b3e8eaa6.jpg] [https://user-images.githubusercontent.com/
   13848158/226426005-f7e83923-0f92-44a4-88e4-1735a3d3e119.jpg] [https://user-
    images.githubusercontent.com/13848158/226426015-4f1122d8-c96a-443f-8698-
                                3db942b1972a.jpg]
+ ### AI systems and agents tracing with Aim
+Log Inputs, Outputs and Actions of     Visualize & Compare Executions Steps via
+Executions ð¤                    UI ð
+    * Track all the inputs, outputs of     * Deep dive into single execution
+      LLMs and tools                         steps
+    * Capture terminal output of           * Compare executions side-by-side
+      executions                           * View previous exectutions terminal
+    * Get notified on executions             outputs
+      progress and finish
+### Experiment tracking with Aim
 Log Metadata Across Your ML Pipeline  Visualize & Compare Metadata via UI ð
 ð¾
     * ML experiments and any metadata
       tracking                            * Metadata visualization via Aim
     * Integration with popular ML           Explorers
       frameworks                          * Grouping and aggregation
     * Easy migration from other           * Querying using Python expressions
@@ -211,33 +221,33 @@
 comparison** Order of magnitude faster training run comparison with Aim - The
 tracked params are first class citizens at Aim. You can search, group,
 aggregate via params - deeply explore all the tracked data (metrics, params,
 images) on the UI. - With tensorboard the users are forced to record those
 parameters in the training run name to be able to search and compare. This
 causes a super-tedius comparison experience and usability issues on the UI when
 there are many experiments and params. **TensorBoard doesn't have features to
-group, aggregate the metrics** **Scalability** - Aim is built to handle 1000s
+group, aggregate the metrics**. **Scalability** - Aim is built to handle 1000s
 of training runs - both on the backend and on the UI. - TensorBoard becomes
 really slow and hard to use when a few hundred training runs are queried /
 compared. **Beloved TB visualizations to be added on Aim** - Embedding
 projector. - Neural network visualization.    MLflow vs Aim   MLFlow is an end-
 to-end ML Lifecycle tool. Aim is focused on training tracking. The main
 differences of Aim and MLflow are around the UI scalability and run comparison
 features. Aim and MLflow are a perfect match - check out the [aimlflow](https:/
-/github.com/aimhubio/aimlflow) - the tool that enables Aim supoerpowers on
-Mlflow. **Run comparison** - Aim treats tracked parameters as first-class
-citizens. Users can query runs, metrics, images and filter using the params. -
+/github.com/aimhubio/aimlflow) - the tool that enables Aim superpowers on
+MLflow. **Run comparison** - Aim treats tracked parameters as first-class
+citizens. Users can query runs, metrics, images, and filter using the params. -
 MLFlow does have a search by tracked config, but there are no grouping,
-aggregation, subplotting by hyparparams and other comparison features
+aggregation, subplotting by hyperparams and other comparison features
 available. **UI Scalability** - Aim UI can handle several thousands of metrics
 at the same time smoothly with 1000s of steps. It may get shaky when you
 explore 1000s of metrics with 10000s of steps each. But we are constantly
 optimizing! - MLflow UI becomes slow to use when there are a few hundreds of
 runs.    Weights and Biases vs Aim   Hosted vs self-hosted - Weights and Biases
-is a hosted closed-source MLOps platform. - Aim is self-hosted, free and open-
+is a hosted closed-source MLOps platform. - Aim is self-hosted, free, and open-
 source experiment tracking tool.  # ð£ï¸ Roadmap ## Detailed milestones The
 [Aim product roadmap](https://github.com/orgs/aimhubio/projects/3) :sparkle: -
 The `Backlog` contains the issues we are going to choose from and prioritize
 weekly - The issues are mainly prioritized by the highly-requested features ##
 High-level roadmap The high-level features we are going to work on the next few
 months: **In progress** - [ ] Aim SDK low-level interface - [ ] Dashboards â
 customizable layouts with embedded explorers - [ ] Ergonomic UI kit - [ ] Text
```

### Comparing `aim-4.0.0.dev3/aim.egg-info/SOURCES.txt` & `aim-4.0.0.dev4/aim.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -183,14 +183,28 @@
 aim/sdk/adapters/sb3.py
 aim/sdk/adapters/tensorflow.py
 aim/sdk/adapters/xgboost.py
 aim/sdk/callbacks/__init__.py
 aim/sdk/callbacks/caller.py
 aim/sdk/callbacks/events.py
 aim/sdk/callbacks/helpers.py
+aim/sdk/core/__init__.py
+aim/sdk/core/collections.py
+aim/sdk/core/constants.py
+aim/sdk/core/container.py
+aim/sdk/core/exceptions.py
+aim/sdk/core/object.py
+aim/sdk/core/query_utils.py
+aim/sdk/core/repo.py
+aim/sdk/core/sequence.py
+aim/sdk/core/type_utils.py
+aim/sdk/core/utils.py
+aim/sdk/core/interfaces/__init__.py
+aim/sdk/core/interfaces/container.py
+aim/sdk/core/interfaces/sequence.py
 aim/sdk/legacy/__init__.py
 aim/sdk/legacy/deprecation_warning.py
 aim/sdk/legacy/flush.py
 aim/sdk/legacy/init.py
 aim/sdk/legacy/select.py
 aim/sdk/legacy/track.py
 aim/sdk/legacy/session/__init__.py
@@ -325,14 +339,16 @@
 aim/web/api/experiments/__init__.py
 aim/web/api/experiments/pydantic_models.py
 aim/web/api/experiments/views.py
 aim/web/api/projects/__init__.py
 aim/web/api/projects/project.py
 aim/web/api/projects/pydantic_models.py
 aim/web/api/projects/views.py
+aim/web/api/queries/__init__.py
+aim/web/api/queries/views.py
 aim/web/api/runs/__init__.py
 aim/web/api/runs/object_api_utils.py
 aim/web/api/runs/object_views.py
 aim/web/api/runs/pydantic_models.py
 aim/web/api/runs/utils.py
 aim/web/api/runs/views.py
 aim/web/api/tags/__init__.py
```

### Comparing `aim-4.0.0.dev3/performance_tests/sdk/test_data_collection.py` & `aim-4.0.0.dev4/performance_tests/sdk/test_data_collection.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/performance_tests/sdk/test_query.py` & `aim-4.0.0.dev4/performance_tests/sdk/test_query.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/performance_tests/sdk/utils.py` & `aim-4.0.0.dev4/performance_tests/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/performance_tests/storage/test_container_open.py` & `aim-4.0.0.dev4/performance_tests/storage/test_container_open.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/performance_tests/storage/test_iterative_access.py` & `aim-4.0.0.dev4/performance_tests/storage/test_iterative_access.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/performance_tests/storage/test_random_access.py` & `aim-4.0.0.dev4/performance_tests/storage/test_random_access.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/performance_tests/storage/utils.py` & `aim-4.0.0.dev4/performance_tests/storage/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/setup.py` & `aim-4.0.0.dev4/setup.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/api/test_dashboards_api.py` & `aim-4.0.0.dev4/tests/api/test_dashboards_api.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/api/test_project_api.py` & `aim-4.0.0.dev4/tests/api/test_project_api.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/api/test_run_api.py` & `aim-4.0.0.dev4/tests/api/test_run_api.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/api/test_run_images_api.py` & `aim-4.0.0.dev4/tests/api/test_run_images_api.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/api/test_structured_data_api.py` & `aim-4.0.0.dev4/tests/api/test_structured_data_api.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/integrations/test_dvc_metadata.py` & `aim-4.0.0.dev4/tests/integrations/test_dvc_metadata.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/integrations/test_hf_datasets.py` & `aim-4.0.0.dev4/tests/integrations/test_hf_datasets.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/integrations/test_hub_dataset.py` & `aim-4.0.0.dev4/tests/integrations/test_hub_dataset.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/sdk/test_image_construction.py` & `aim-4.0.0.dev4/tests/sdk/test_image_construction.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/sdk/test_resource_tracker.py` & `aim-4.0.0.dev4/tests/sdk/test_resource_tracker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/sdk/test_run_apis.py` & `aim-4.0.0.dev4/tests/sdk/test_run_apis.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/sdk/test_run_creation_checks.py` & `aim-4.0.0.dev4/tests/sdk/test_run_creation_checks.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/sdk/test_run_finalization_time.py` & `aim-4.0.0.dev4/tests/sdk/test_run_finalization_time.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/sdk/test_run_metric_types.py` & `aim-4.0.0.dev4/tests/sdk/test_run_metric_types.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/sdk/test_run_track_type_checking.py` & `aim-4.0.0.dev4/tests/sdk/test_run_track_type_checking.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/sdk/test_run_write_container_data.py` & `aim-4.0.0.dev4/tests/sdk/test_run_write_container_data.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/sdk/test_utils.py` & `aim-4.0.0.dev4/tests/sdk/test_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/storage/test_query.py` & `aim-4.0.0.dev4/tests/storage/test_query.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/storage/test_query_with_epoch_none.py` & `aim-4.0.0.dev4/tests/storage/test_query_with_epoch_none.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev3/tests/storage/test_structured_db.py` & `aim-4.0.0.dev4/tests/storage/test_structured_db.py`

 * *Files identical despite different names*


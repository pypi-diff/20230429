# Comparing `tmp/ultralytics-8.0.9.tar.gz` & `tmp/ultralytics-8.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics-8.0.9.tar", last modified: Wed Jan 18 08:36:22 2023, max compression
+gzip compressed data, was "ultralytics-8.0.90.tar", last modified: Sat Apr 29 18:18:51 2023, max compression
```

## Comparing `ultralytics-8.0.9.tar` & `ultralytics-8.0.90.tar`

### file list

```diff
@@ -1,140 +1,179 @@
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.378065 ultralytics-8.0.9/
--rw-r--r--   0 glennjocher   (501) staff       (20)     5613 2023-01-17 13:35:22.000000 ultralytics-8.0.9/CONTRIBUTING.md
--rw-r--r--   0 glennjocher   (501) staff       (20)    35149 2023-01-17 13:35:22.000000 ultralytics-8.0.9/LICENSE
--rw-r--r--   0 glennjocher   (501) staff       (20)      140 2023-01-17 13:35:22.000000 ultralytics-8.0.9/MANIFEST.in
--rw-r--r--   0 glennjocher   (501) staff       (20)    23762 2023-01-18 08:36:22.378177 ultralytics-8.0.9/PKG-INFO
--rw-r--r--   0 glennjocher   (501) staff       (20)    22374 2023-01-18 08:17:00.000000 ultralytics-8.0.9/README.md
--rw-r--r--   0 glennjocher   (501) staff       (20)    20431 2023-01-17 22:00:59.000000 ultralytics-8.0.9/README.zh-CN.md
--rw-r--r--   0 glennjocher   (501) staff       (20)     1189 2023-01-17 21:37:01.000000 ultralytics-8.0.9/requirements.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)      702 2023-01-18 08:36:22.378608 ultralytics-8.0.9/setup.cfg
--rw-r--r--   0 glennjocher   (501) staff       (20)     2520 2023-01-17 22:00:59.000000 ultralytics-8.0.9/setup.py
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.354642 ultralytics-8.0.9/ultralytics/
--rw-r--r--   0 glennjocher   (501) staff       (20)      299 2023-01-18 08:33:56.000000 ultralytics-8.0.9/ultralytics/__init__.py
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.356672 ultralytics-8.0.9/ultralytics/hub/
--rw-r--r--   0 glennjocher   (501) staff       (20)     4465 2023-01-18 07:33:38.000000 ultralytics-8.0.9/ultralytics/hub/__init__.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     2483 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/hub/auth.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     4655 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/hub/session.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     6660 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/hub/utils.py
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.350419 ultralytics-8.0.9/ultralytics/models/
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.357623 ultralytics-8.0.9/ultralytics/models/v3/
--rw-r--r--   0 glennjocher   (501) staff       (20)     1434 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v3/yolov3-spp.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1135 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1425 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v3/yolov3.yaml
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.358685 ultralytics-8.0.9/ultralytics/models/v5/
--rw-r--r--   0 glennjocher   (501) staff       (20)     1267 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v5/yolov5l.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1269 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v5/yolov5m.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1269 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v5/yolov5n.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1270 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v5/yolov5s.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1269 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v5/yolov5x.yaml
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.360012 ultralytics-8.0.9/ultralytics/models/v8/
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.361106 ultralytics-8.0.9/ultralytics/models/v8/cls/
--rw-r--r--   0 glennjocher   (501) staff       (20)      629 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v8/cls/yolov8l-cls.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)      629 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v8/cls/yolov8m-cls.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)      629 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v8/cls/yolov8n-cls.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)      629 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v8/cls/yolov8s-cls.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)      629 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v8/cls/yolov8x-cls.yaml
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.362256 ultralytics-8.0.9/ultralytics/models/v8/seg/
--rw-r--r--   0 glennjocher   (501) staff       (20)     1209 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v8/seg/yolov8l-seg.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1209 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v8/seg/yolov8m-seg.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1213 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v8/seg/yolov8n-seg.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1213 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v8/seg/yolov8s-seg.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1209 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v8/seg/yolov8x-seg.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1199 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v8/yolov8l.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1199 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v8/yolov8m.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1203 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v8/yolov8n.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1203 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v8/yolov8s.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1199 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v8/yolov8x.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1569 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/models/v8/yolov8x6.yaml
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.363349 ultralytics-8.0.9/ultralytics/nn/
--rw-r--r--   0 glennjocher   (501) staff       (20)        0 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/nn/__init__.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    20525 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/nn/autobackend.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    11853 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/nn/autoshape.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    18358 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/nn/modules.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    18651 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/nn/tasks.py
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.363820 ultralytics-8.0.9/ultralytics/yolo/
--rw-r--r--   0 glennjocher   (501) staff       (20)       59 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/__init__.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     5956 2023-01-18 08:03:25.000000 ultralytics-8.0.9/ultralytics/yolo/cli.py
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.364604 ultralytics-8.0.9/ultralytics/yolo/configs/
--rw-r--r--   0 glennjocher   (501) staff       (20)     1212 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/configs/__init__.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     5470 2023-01-17 14:57:21.000000 ultralytics-8.0.9/ultralytics/yolo/configs/default.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     3760 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/configs/hydra_patch.py
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.366253 ultralytics-8.0.9/ultralytics/yolo/data/
--rw-r--r--   0 glennjocher   (501) staff       (20)      262 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/__init__.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    30711 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/augment.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     8547 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/base.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     4967 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/build.py
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.367178 ultralytics-8.0.9/ultralytics/yolo/data/dataloaders/
--rw-r--r--   0 glennjocher   (501) staff       (20)        0 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/dataloaders/__init__.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    13173 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/dataloaders/stream_loaders.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    17247 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/dataloaders/v5augmentations.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    55344 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/dataloaders/v5loader.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     9605 2023-01-18 07:19:48.000000 ultralytics-8.0.9/ultralytics/yolo/data/dataset.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     1330 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/dataset_wrappers.py
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.370185 ultralytics-8.0.9/ultralytics/yolo/data/datasets/
--rw-r--r--   0 glennjocher   (501) staff       (20)     2728 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/datasets/Argoverse.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1880 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)    18866 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/datasets/ImageNet.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     9200 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/datasets/Objects365.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     2336 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/datasets/SKU-110K.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     3488 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/datasets/VOC.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     2966 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/datasets/VisDrone.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     2485 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/datasets/coco.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1862 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/datasets/coco128-seg.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1846 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/datasets/coco128.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1797 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/datasets/coco8-seg.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     1777 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/datasets/coco8.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)     5165 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/datasets/xView.yaml
--rw-r--r--   0 glennjocher   (501) staff       (20)    13304 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/data/utils.py
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.371597 ultralytics-8.0.9/ultralytics/yolo/engine/
--rw-r--r--   0 glennjocher   (501) staff       (20)        0 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/engine/__init__.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    40297 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/engine/exporter.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     9078 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/engine/model.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    13261 2023-01-17 22:00:59.000000 ultralytics-8.0.9/ultralytics/yolo/engine/predictor.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     9580 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/engine/results.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    25807 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/engine/trainer.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     8999 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/engine/validator.py
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.374329 ultralytics-8.0.9/ultralytics/yolo/utils/
--rw-r--r--   0 glennjocher   (501) staff       (20)    15731 2023-01-18 08:33:56.000000 ultralytics-8.0.9/ultralytics/yolo/utils/__init__.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     3010 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/utils/autobatch.py
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.375451 ultralytics-8.0.9/ultralytics/yolo/utils/callbacks/
--rw-r--r--   0 glennjocher   (501) staff       (20)       63 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/utils/callbacks/__init__.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     3182 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/utils/callbacks/base.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     1872 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/utils/callbacks/clearml.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     1596 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/utils/callbacks/comet.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     2584 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/utils/callbacks/hub.py
--rw-r--r--   0 glennjocher   (501) staff       (20)      723 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/utils/callbacks/tensorboard.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    10817 2023-01-18 08:21:26.000000 ultralytics-8.0.9/ultralytics/yolo/utils/checks.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     2278 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/utils/dist.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     6625 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/utils/downloads.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     3818 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/utils/files.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    11360 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/utils/instance.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     2261 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/utils/loss.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    22673 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/utils/metrics.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    28031 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/utils/ops.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    14641 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/utils/plotting.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     9580 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/utils/tal.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    15783 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/utils/torch_utils.py
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.375655 ultralytics-8.0.9/ultralytics/yolo/v8/
--rw-r--r--   0 glennjocher   (501) staff       (20)      220 2023-01-17 22:00:59.000000 ultralytics-8.0.9/ultralytics/yolo/v8/__init__.py
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.376424 ultralytics-8.0.9/ultralytics/yolo/v8/classify/
--rw-r--r--   0 glennjocher   (501) staff       (20)      274 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/v8/classify/__init__.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     2832 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/v8/classify/predict.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     6144 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/v8/classify/train.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     2126 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/v8/classify/val.py
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.377152 ultralytics-8.0.9/ultralytics/yolo/v8/detect/
--rw-r--r--   0 glennjocher   (501) staff       (20)      175 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/v8/detect/__init__.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     3929 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/v8/detect/predict.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     9553 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/v8/detect/train.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    11868 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/v8/detect/val.py
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.377898 ultralytics-8.0.9/ultralytics/yolo/v8/segment/
--rw-r--r--   0 glennjocher   (501) staff       (20)      184 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/v8/segment/__init__.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     4710 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/v8/segment/predict.py
--rw-r--r--   0 glennjocher   (501) staff       (20)     6948 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/v8/segment/train.py
--rw-r--r--   0 glennjocher   (501) staff       (20)    12343 2023-01-17 13:35:22.000000 ultralytics-8.0.9/ultralytics/yolo/v8/segment/val.py
-drwxr-xr-x   0 glennjocher   (501) staff       (20)        0 2023-01-18 08:36:22.355654 ultralytics-8.0.9/ultralytics.egg-info/
--rw-r--r--   0 glennjocher   (501) staff       (20)    23762 2023-01-18 08:36:22.000000 ultralytics-8.0.9/ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 glennjocher   (501) staff       (20)     4111 2023-01-18 08:36:22.000000 ultralytics-8.0.9/ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)        1 2023-01-18 08:36:22.000000 ultralytics-8.0.9/ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)      103 2023-01-18 08:36:22.000000 ultralytics-8.0.9/ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)      372 2023-01-18 08:36:22.000000 ultralytics-8.0.9/ultralytics.egg-info/requires.txt
--rw-r--r--   0 glennjocher   (501) staff       (20)       12 2023-01-18 08:36:22.000000 ultralytics-8.0.9/ultralytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.539567 ultralytics-8.0.90/
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-29 18:17:10.000000 ultralytics-8.0.90/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-29 18:17:10.000000 ultralytics-8.0.90/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-29 18:17:10.000000 ultralytics-8.0.90/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-04-29 18:18:51.539567 ultralytics-8.0.90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-04-29 18:17:10.000000 ultralytics-8.0.90/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23225 2023-04-29 18:17:10.000000 ultralytics-8.0.90/README.zh-CN.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-29 18:17:10.000000 ultralytics-8.0.90/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-29 18:18:51.539567 ultralytics-8.0.90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-29 18:17:10.000000 ultralytics-8.0.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.519567 ultralytics-8.0.90/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-29 18:17:10.000000 ultralytics-8.0.90/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-29 18:17:10.000000 ultralytics-8.0.90/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-29 18:17:10.000000 ultralytics-8.0.90/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.519567 ultralytics-8.0.90/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.523567 ultralytics-8.0.90/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.523567 ultralytics-8.0.90/ultralytics/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/datasets/xView.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.523567 ultralytics-8.0.90/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.519567 ultralytics-8.0.90/ultralytics/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.523567 ultralytics-8.0.90/ultralytics/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.523567 ultralytics-8.0.90/ultralytics/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.527567 ultralytics-8.0.90/ultralytics/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.527567 ultralytics-8.0.90/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24243 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/nn/autobackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/nn/autoshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25079 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/nn/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27170 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.527567 ultralytics-8.0.90/ultralytics/tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.527567 ultralytics-8.0.90/ultralytics/tracker/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/cfg/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/cfg/bytetrack.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/track.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.527567 ultralytics-8.0.90/ultralytics/tracker/trackers/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/trackers/byte_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.527567 ultralytics-8.0.90/ultralytics/tracker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/tracker/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.527567 ultralytics-8.0.90/ultralytics/vit/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.527567 ultralytics-8.0.90/ultralytics/vit/sam/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/autosize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.531567 ultralytics-8.0.90/ultralytics/vit/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22502 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15281 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/modules/mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/modules/prompt_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/vit/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.531567 ultralytics-8.0.90/ultralytics/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.531567 ultralytics-8.0.90/ultralytics/yolo/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)    17675 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/cfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.531567 ultralytics-8.0.90/ultralytics/yolo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33512 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.531567 ultralytics-8.0.90/ultralytics/yolo/data/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/dataloaders/stream_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/dataloaders/v5augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51260 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/dataloaders/v5loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.531567 ultralytics-8.0.90/ultralytics/yolo/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40265 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16049 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20388 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.535567 ultralytics-8.0.90/ultralytics/yolo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    27960 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.535567 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41829 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28191 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20019 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.535567 ultralytics-8.0.90/ultralytics/yolo/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.535567 ultralytics-8.0.90/ultralytics/yolo/v8/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.539567 ultralytics-8.0.90/ultralytics/yolo/v8/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12195 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/detect/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.539567 ultralytics-8.0.90/ultralytics/yolo/v8/pose/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.539567 ultralytics-8.0.90/ultralytics/yolo/v8/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-04-29 18:17:10.000000 ultralytics-8.0.90/ultralytics/yolo/v8/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:18:51.523567 ultralytics-8.0.90/ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25796 2023-04-29 18:18:51.000000 ultralytics-8.0.90/ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-29 18:18:51.000000 ultralytics-8.0.90/ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:18:51.000000 ultralytics-8.0.90/ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-29 18:18:51.000000 ultralytics-8.0.90/ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-29 18:18:51.000000 ultralytics-8.0.90/ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 18:18:51.000000 ultralytics-8.0.90/ultralytics.egg-info/top_level.txt
```

### Comparing `ultralytics-8.0.9/CONTRIBUTING.md` & `ultralytics-8.0.90/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,26 +55,28 @@
 <p align="center"><img width="751" alt="Screenshot 2022-08-29 at 22 47 03" src="https://user-images.githubusercontent.com/26833433/187296922-545c5498-f64a-4d8c-8300-5fa764360da6.png"></p>
 
 - ✅ Reduce changes to the absolute **minimum** required for your bug fix or feature addition. _"It is not daily increase
   but daily decrease, hack away the unessential. The closer to the source, the less wastage there is."_  — Bruce Lee
 
 ### Docstrings
 
-Not all functions or classes require docstrings but when they do, we follow [google-stlye docstrings format](https://google.github.io/styleguide/pyguide.html#38-comments-and-docstrings). Here is an example:
+Not all functions or classes require docstrings but when they do, we
+follow [google-style docstrings format](https://google.github.io/styleguide/pyguide.html#38-comments-and-docstrings).
+Here is an example:
 
 ```python
 """
-   What the function does - performs nms on given detection predictions
+   What the function does. Performs NMS on given detection predictions.
 
     Args:
         arg1: The description of the 1st argument
         arg2: The description of the 2nd argument
 
     Returns:
-        What the function returns. Empty if nothing is returned
+        What the function returns. Empty if nothing is returned.
 
     Raises:
         Exception Class: When and why this exception can be raised by the function.
 """
 ```
 
 ## Submitting a Bug Report 🐛
@@ -106,8 +108,8 @@
 **Bug Report** [template](https://github.com/ultralytics/ultralytics/issues/new/choose) and providing
 a [minimum reproducible example](https://stackoverflow.com/help/minimal-reproducible-example) to help us better
 understand and diagnose your problem.
 
 ## License
 
 By contributing, you agree that your contributions will be licensed under
-the [GPL-3.0 license](https://choosealicense.com/licenses/gpl-3.0/)
+the [AGPL-3.0 license](https://choosealicense.com/licenses/agpl-3.0/)
```

### Comparing `ultralytics-8.0.9/LICENSE` & `ultralytics-8.0.90/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,70 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
 
  Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
                             Preamble
 
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
+  The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
 
   The licenses for most software and other practical works are designed
 to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
+our General Public Licenses are intended to guarantee your freedom to
 share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
+software for all its users.
 
   When we speak of free software, we are referring to freedom, not
 price.  Our General Public Licenses are designed to make sure that you
 have the freedom to distribute copies of free software (and charge for
 them if you wish), that you receive source code or can get it if you
 want it, that you can change the software or use pieces of it in new
 free programs, and that you know you can do these things.
 
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
+  Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+  A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate.  Many developers of free software are heartened and
+encouraged by the resulting cooperation.  However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+  The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community.  It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server.  Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+  An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals.  This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing under
+this license.
 
   The precise terms and conditions for copying, distribution and
 modification follow.
 
                        TERMS AND CONDITIONS
 
   0. Definitions.
 
-  "This License" refers to version 3 of the GNU General Public License.
+  "This License" refers to version 3 of the GNU Affero General Public License.
 
   "Copyright" also means copyright-like laws that apply to other kinds of
 works, such as semiconductor masks.
 
   "The Program" refers to any copyrightable work licensed under this
 License.  Each licensee is addressed as "you".  "Licensees" and
 "recipients" may be individuals or organizations.
@@ -545,43 +533,53 @@
 covered work so as to satisfy simultaneously your obligations under this
 License and any other pertinent obligations, then as a consequence you may
 not convey it at all.  For example, if you agree to terms that obligate you
 to collect a royalty for further conveying from those to whom you convey
 the Program, the only way you could satisfy both those terms and this
 License would be to refrain entirely from conveying the Program.
 
-  13. Use with the GNU Affero General Public License.
+  13. Remote Network Interaction; Use with the GNU General Public License.
+
+  Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your version
+supports such interaction) an opportunity to receive the Corresponding
+Source of your version by providing access to the Corresponding Source
+from a network server at no charge, through some standard or customary
+means of facilitating copying of software.  This Corresponding Source
+shall include the Corresponding Source for any work covered by version 3
+of the GNU General Public License that is incorporated pursuant to the
+following paragraph.
 
   Notwithstanding any other provision of this License, you have
 permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
+under version 3 of the GNU General Public License into a single
 combined work, and to convey the resulting work.  The terms of this
 License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
 
   14. Revised Versions of this License.
 
   The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
+the GNU Affero General Public License from time to time.  Such new versions
+will be similar in spirit to the present version, but may differ in detail to
 address new problems or concerns.
 
   Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
+Program specifies that a certain numbered version of the GNU Affero General
 Public License "or any later version" applies to it, you have the
 option of following the terms and conditions either of that numbered
 version or of any later version published by the Free Software
 Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
+GNU Affero General Public License, you may choose any version ever published
 by the Free Software Foundation.
 
   If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
+versions of the GNU Affero General Public License can be used, that proxy's
 public statement of acceptance of a version permanently authorizes you
 to choose that version for the Program.
 
   Later license versions may give you additional or different
 permissions.  However, no additional obligations are imposed on any
 author or copyright holder as a result of your choosing to follow a
 later version.
@@ -631,44 +629,33 @@
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
     <one line to give the program's name and a brief idea of what it does.>
     Copyright (C) <year>  <name of author>
 
     This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
+    it under the terms of the GNU Affero General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
+    GNU Affero General Public License for more details.
 
-    You should have received a copy of the GNU General Public License
+    You should have received a copy of the GNU Affero General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
+  If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source.  For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code.  There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for the
+specific requirements.
 
   You should also get your employer (if you work as a programmer) or school,
 if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
+For more information on this, and how to apply and follow the GNU AGPL, see
 <https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `ultralytics-8.0.9/PKG-INFO` & `ultralytics-8.0.90/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.0.9
+Version: 8.0.90
 Summary: Ultralytics YOLOv8
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
-License: GPL-3.0
+License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/ultralytics
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7,<=3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: export
 License-File: LICENSE
 
 <div align="center">
   <p>
-    <a align="center" href="https://ultralytics.com/yolov8" target="_blank">
+    <a href="https://ultralytics.com/yolov8" target="_blank">
       <img width="100%" src="https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/banner-yolov8.png"></a>
   </p>
 
 [English](README.md) | [简体中文](README.zh-CN.md)
 <br>
 
 <div>
@@ -46,80 +50,54 @@
     <br>
     <a href="https://console.paperspace.com/github/ultralytics/ultralytics"><img src="https://assets.paperspace.io/img/gradient-badge.svg" alt="Run on Gradient"/></a>
     <a href="https://colab.research.google.com/github/ultralytics/ultralytics/blob/main/examples/tutorial.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>
     <a href="https://www.kaggle.com/ultralytics/yolov8"><img src="https://kaggle.com/static/images/open-in-kaggle.svg" alt="Open In Kaggle"></a>
   </div>
   <br>
 
-[Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics), developed by [Ultralytics](https://ultralytics.com),
-is a cutting-edge, state-of-the-art (SOTA) model that builds upon the success of previous YOLO versions and introduces
-new features and improvements to further boost performance and flexibility. YOLOv8 is designed to be fast, accurate, and
-easy to use, making it an excellent choice for a wide range of object detection, image segmentation and image
-classification tasks.
+[Ultralytics](https://ultralytics.com) [YOLOv8](https://github.com/ultralytics/ultralytics) is a cutting-edge, state-of-the-art (SOTA) model that builds upon the success of previous YOLO versions and introduces new features and improvements to further boost performance and flexibility. YOLOv8 is designed to be fast, accurate, and easy to use, making it an excellent choice for a wide range of object detection and tracking, instance segmentation, image classification and pose estimation tasks.
+
+We hope that the resources here will help you get the most out of YOLOv8. Please browse the YOLOv8 <a href="https://docs.ultralytics.com/">Docs</a> for details, raise an issue on <a href="https://github.com/ultralytics/ultralytics/issues/new/choose">GitHub</a> for support, and join our <a href="https://discord.gg/n6cFeSPZdD">Discord</a> community for questions and discussions!
 
 To request an Enterprise License please complete the form at [Ultralytics Licensing](https://ultralytics.com/license).
 
 <img width="100%" src="https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/yolo-comparison-plots.png"></a>
 
 <div align="center">
-    <a href="https://github.com/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://www.linkedin.com/company/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://twitter.com/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://www.producthunt.com/@glenn_jocher" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-producthunt.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://youtube.com/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://www.facebook.com/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-facebook.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://www.instagram.com/ultralytics/" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="2%" alt="" /></a>
-  </div>
+  <a href="https://github.com/ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://www.linkedin.com/company/ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://twitter.com/ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://youtube.com/ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://www.tiktok.com/@ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-tiktok.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://www.instagram.com/ultralytics/" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://discord.gg/n6cFeSPZdD" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/blob/main/social/logo-social-discord.png" width="2%" alt="" /></a>
 </div>
-
-## <div align="center">Ultralytics Live Session</div>
-
-<div align="center">
-
-[Ultralytics Live Session 3](https://youtu.be/IPcpYO5ITa8) ✨ is here! Join us on January 24th at 18 CET as we dive into
-the latest advancements in YOLOv8, and demonstrate how to use this cutting-edge, SOTA model to improve your object
-detection, instance segmentation, and image classification projects. See firsthand how YOLOv8's speed, accuracy, and
-ease of use make it a top choice for professionals and researchers alike.
-
-In addition to learning about the exciting new features and improvements of Ultralytics YOLOv8, you will also have the
-opportunity to ask questions and interact with our team during the live Q&A session. We encourage you to come prepared
-with any questions you may have.
-
-To join the webinar, visit our YouTube [Channel](https://www.youtube.com/@Ultralytics/streams) and turn on your
-notifications!
-
-<a align="center" href="https://youtu.be/IPcpYO5ITa8" target="_blank">
-<img width="80%" src="https://user-images.githubusercontent.com/107626595/212887899-e94b006c-5192-40fa-8b24-7b5428e065e8.png"></a>
 </div>
 
 ## <div align="center">Documentation</div>
 
-See below for a quickstart installation and usage example, and see the [YOLOv8 Docs](https://docs.ultralytics.com) for
-full documentation on training, validation, prediction and deployment.
+See below for a quickstart installation and usage example, and see the [YOLOv8 Docs](https://docs.ultralytics.com) for full documentation on training, validation, prediction and deployment.
 
 <details open>
 <summary>Install</summary>
 
-Pip install the ultralytics package including
-all [requirements.txt](https://github.com/ultralytics/ultralytics/blob/main/requirements.txt) in a
-[**3.10>=Python>=3.7**](https://www.python.org/) environment, including
-[**PyTorch>=1.7**](https://pytorch.org/get-started/locally/).
+Pip install the ultralytics package including all [requirements](https://github.com/ultralytics/ultralytics/blob/main/requirements.txt) in a [**Python>=3.7**](https://www.python.org/) environment with [**PyTorch>=1.7**](https://pytorch.org/get-started/locally/).
 
 ```bash
 pip install ultralytics
 ```
 
 </details>
 
@@ -127,199 +105,194 @@
 <summary>Usage</summary>
 
 #### CLI
 
 YOLOv8 may be used directly in the Command Line Interface (CLI) with a `yolo` command:
 
 ```bash
-yolo predict model=yolov8n.pt source="https://ultralytics.com/images/bus.jpg"
+yolo predict model=yolov8n.pt source='https://ultralytics.com/images/bus.jpg'
 ```
 
-`yolo` can be used for a variety of tasks and modes and accepts additional arguments, i.e. `imgsz=640`. See the YOLOv8
-[CLI Docs](https://docs.ultralytics.com/cli) for examples.
+`yolo` can be used for a variety of tasks and modes and accepts additional arguments, i.e. `imgsz=640`. See the YOLOv8 [CLI Docs](https://docs.ultralytics.com/usage/cli) for examples.
 
 #### Python
 
-YOLOv8 may also be used directly in a Python environment, and accepts the
-same [arguments](https://docs.ultralytics.com/config/) as in the CLI example above:
+YOLOv8 may also be used directly in a Python environment, and accepts the same [arguments](https://docs.ultralytics.com/usage/cfg/) as in the CLI example above:
 
 ```python
 from ultralytics import YOLO
 
 # Load a model
 model = YOLO("yolov8n.yaml")  # build a new model from scratch
 model = YOLO("yolov8n.pt")  # load a pretrained model (recommended for training)
 
 # Use the model
-results = model.train(data="coco128.yaml", epochs=3)  # train the model
-results = model.val()  # evaluate model performance on the validation set
+model.train(data="coco128.yaml", epochs=3)  # train the model
+metrics = model.val()  # evaluate model performance on the validation set
 results = model("https://ultralytics.com/images/bus.jpg")  # predict on an image
 success = model.export(format="onnx")  # export the model to ONNX format
 ```
 
-[Models](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) download automatically from the latest
-Ultralytics [release](https://github.com/ultralytics/assets/releases). See
-YOLOv8 [Python Docs](https://docs.ultralytics.com/python) for more examples.
-
-#### Known Issues / TODOs
-
-We are still working on several parts of YOLOv8! We aim to have these completed soon to bring the YOLOv8 feature set up
-to par with YOLOv5, including export and inference to all the same formats. We are also writing a YOLOv8 paper which we
-will submit to [arxiv.org](https://arxiv.org) once complete.
-
-- [ ] TensorFlow exports
-- [ ] DDP resume
-- [ ] [arxiv.org](https://arxiv.org) paper
+[Models](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) download automatically from the latest Ultralytics [release](https://github.com/ultralytics/assets/releases). See YOLOv8 [Python Docs](https://docs.ultralytics.com/usage/python) for more examples.
 
 </details>
 
 ## <div align="center">Models</div>
 
-All YOLOv8 pretrained models are available here. Detection and Segmentation models are pretrained on the COCO dataset,
-while Classification models are pretrained on the ImageNet dataset.
+All YOLOv8 pretrained models are available here. Detect, Segment and Pose models are pretrained on the [COCO](https://github.com/ultralytics/ultralytics/blob/main/ultralytics/datasets/coco.yaml) dataset, while Classify models are pretrained on the [ImageNet](https://github.com/ultralytics/ultralytics/blob/main/ultralytics/datasets/ImageNet.yaml) dataset.
 
-[Models](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) download automatically from the latest
-Ultralytics [release](https://github.com/ultralytics/assets/releases) on first use.
+[Models](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) download automatically from the latest Ultralytics [release](https://github.com/ultralytics/assets/releases) on first use.
 
 <details open><summary>Detection</summary>
 
-See [Detection Docs](https://docs.ultralytics.com/tasks/detection/) for usage examples with these models.
+See [Detection Docs](https://docs.ultralytics.com/tasks/detect/) for usage examples with these models.
 
 | Model                                                                                | size<br><sup>(pixels) | mAP<sup>val<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |
 | ------------------------------------------------------------------------------------ | --------------------- | -------------------- | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
 | [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n.pt) | 640                   | 37.3                 | 80.4                           | 0.99                                | 3.2                | 8.7               |
 | [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s.pt) | 640                   | 44.9                 | 128.4                          | 1.20                                | 11.2               | 28.6              |
 | [YOLOv8m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m.pt) | 640                   | 50.2                 | 234.7                          | 1.83                                | 25.9               | 78.9              |
 | [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l.pt) | 640                   | 52.9                 | 375.2                          | 2.39                                | 43.7               | 165.2             |
 | [YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x.pt) | 640                   | 53.9                 | 479.1                          | 3.53                                | 68.2               | 257.8             |
 
 - **mAP<sup>val</sup>** values are for single-model single-scale on [COCO val2017](http://cocodataset.org) dataset.
   <br>Reproduce by `yolo val detect data=coco.yaml device=0`
-- **Speed** averaged over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/)
-  instance.
-  <br>Reproduce by `yolo val detect data=coco128.yaml batch=1 device=0/cpu`
+- **Speed** averaged over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) instance.
+  <br>Reproduce by `yolo val detect data=coco128.yaml batch=1 device=0|cpu`
 
 </details>
 
 <details><summary>Segmentation</summary>
 
-See [Segmentation Docs](https://docs.ultralytics.com/tasks/segmentation/) for usage examples with these models.
+See [Segmentation Docs](https://docs.ultralytics.com/tasks/segment/) for usage examples with these models.
 
-| Model                                                                                    | size<br><sup>(pixels) | mAP<sup>box<br>50-95 | mAP<sup>mask<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |
-| ---------------------------------------------------------------------------------------- | --------------------- | -------------------- | --------------------- | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
-| [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640                   | 36.7                 | 30.5                  | 96.1                           | 1.21                                | 3.4                | 12.6              |
-| [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-seg.pt) | 640                   | 44.6                 | 36.8                  | 155.7                          | 1.47                                | 11.8               | 42.6              |
-| [YOLOv8m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-seg.pt) | 640                   | 49.9                 | 40.8                  | 317.0                          | 2.18                                | 27.3               | 110.2             |
-| [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-seg.pt) | 640                   | 52.3                 | 42.6                  | 572.4                          | 2.79                                | 46.0               | 220.5             |
-| [YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-seg.pt) | 640                   | 53.4                 | 43.4                  | 712.1                          | 4.02                                | 71.8               | 344.1             |
+| Model                                                                                        | size<br><sup>(pixels) | mAP<sup>box<br>50-95 | mAP<sup>mask<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |
+| -------------------------------------------------------------------------------------------- | --------------------- | -------------------- | --------------------- | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
+| [YOLOv8n-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640                   | 36.7                 | 30.5                  | 96.1                           | 1.21                                | 3.4                | 12.6              |
+| [YOLOv8s-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-seg.pt) | 640                   | 44.6                 | 36.8                  | 155.7                          | 1.47                                | 11.8               | 42.6              |
+| [YOLOv8m-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-seg.pt) | 640                   | 49.9                 | 40.8                  | 317.0                          | 2.18                                | 27.3               | 110.2             |
+| [YOLOv8l-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-seg.pt) | 640                   | 52.3                 | 42.6                  | 572.4                          | 2.79                                | 46.0               | 220.5             |
+| [YOLOv8x-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-seg.pt) | 640                   | 53.4                 | 43.4                  | 712.1                          | 4.02                                | 71.8               | 344.1             |
 
 - **mAP<sup>val</sup>** values are for single-model single-scale on [COCO val2017](http://cocodataset.org) dataset.
   <br>Reproduce by `yolo val segment data=coco.yaml device=0`
-- **Speed** averaged over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/)
-  instance.
-  <br>Reproduce by `yolo val segment data=coco128-seg.yaml batch=1 device=0/cpu`
+- **Speed** averaged over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) instance.
+  <br>Reproduce by `yolo val segment data=coco128-seg.yaml batch=1 device=0|cpu`
 
 </details>
 
 <details><summary>Classification</summary>
 
-See [Classification Docs](https://docs.ultralytics.com/tasks/classification/) for usage examples with these models.
+See [Classification Docs](https://docs.ultralytics.com/tasks/classify/) for usage examples with these models.
 
-| Model                                                                                    | size<br><sup>(pixels) | acc<br><sup>top1 | acc<br><sup>top5 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) at 640 |
-| ---------------------------------------------------------------------------------------- | --------------------- | ---------------- | ---------------- | ------------------------------ | ----------------------------------- | ------------------ | ------------------------ |
-| [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-cls.pt) | 224                   | 66.6             | 87.0             | 12.9                           | 0.31                                | 2.7                | 4.3                      |
-| [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-cls.pt) | 224                   | 72.3             | 91.1             | 23.4                           | 0.35                                | 6.4                | 13.5                     |
-| [YOLOv8m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-cls.pt) | 224                   | 76.4             | 93.2             | 85.4                           | 0.62                                | 17.0               | 42.7                     |
-| [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-cls.pt) | 224                   | 78.0             | 94.1             | 163.0                          | 0.87                                | 37.5               | 99.7                     |
-| [YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-cls.pt) | 224                   | 78.4             | 94.3             | 232.0                          | 1.01                                | 57.4               | 154.8                    |
+| Model                                                                                        | size<br><sup>(pixels) | acc<br><sup>top1 | acc<br><sup>top5 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) at 640 |
+| -------------------------------------------------------------------------------------------- | --------------------- | ---------------- | ---------------- | ------------------------------ | ----------------------------------- | ------------------ | ------------------------ |
+| [YOLOv8n-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-cls.pt) | 224                   | 66.6             | 87.0             | 12.9                           | 0.31                                | 2.7                | 4.3                      |
+| [YOLOv8s-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-cls.pt) | 224                   | 72.3             | 91.1             | 23.4                           | 0.35                                | 6.4                | 13.5                     |
+| [YOLOv8m-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-cls.pt) | 224                   | 76.4             | 93.2             | 85.4                           | 0.62                                | 17.0               | 42.7                     |
+| [YOLOv8l-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-cls.pt) | 224                   | 78.0             | 94.1             | 163.0                          | 0.87                                | 37.5               | 99.7                     |
+| [YOLOv8x-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-cls.pt) | 224                   | 78.4             | 94.3             | 232.0                          | 1.01                                | 57.4               | 154.8                    |
 
 - **acc** values are model accuracies on the [ImageNet](https://www.image-net.org/) dataset validation set.
   <br>Reproduce by `yolo val classify data=path/to/ImageNet device=0`
-- **Speed** averaged over ImageNet val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/)
-  instance.
-  <br>Reproduce by `yolo val classify data=path/to/ImageNet batch=1 device=0/cpu`
+- **Speed** averaged over ImageNet val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) instance.
+  <br>Reproduce by `yolo val classify data=path/to/ImageNet batch=1 device=0|cpu`
+
+</details>
+
+<details><summary>Pose</summary>
+
+See [Pose Docs](https://docs.ultralytics.com/tasks/pose) for usage examples with these models.
+
+| Model                                                                                                | size<br><sup>(pixels) | mAP<sup>pose<br>50-95 | mAP<sup>pose<br>50 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |
+| ---------------------------------------------------------------------------------------------------- | --------------------- | --------------------- | ------------------ | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
+| [YOLOv8n-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-pose.pt)       | 640                   | 50.4                  | 80.1               | 131.8                          | 1.18                                | 3.3                | 9.2               |
+| [YOLOv8s-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-pose.pt)       | 640                   | 60.0                  | 86.2               | 233.2                          | 1.42                                | 11.6               | 30.2              |
+| [YOLOv8m-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-pose.pt)       | 640                   | 65.0                  | 88.8               | 456.3                          | 2.00                                | 26.4               | 81.0              |
+| [YOLOv8l-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-pose.pt)       | 640                   | 67.6                  | 90.0               | 784.5                          | 2.59                                | 44.4               | 168.6             |
+| [YOLOv8x-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-pose.pt)       | 640                   | 69.2                  | 90.2               | 1607.1                         | 3.73                                | 69.4               | 263.2             |
+| [YOLOv8x-pose-p6](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-pose-p6.pt) | 1280                  | 71.6                  | 91.2               | 4088.7                         | 10.04                               | 99.1               | 1066.4            |
+
+- **mAP<sup>val</sup>** values are for single-model single-scale on [COCO Keypoints val2017](http://cocodataset.org)
+  dataset.
+  <br>Reproduce by `yolo val pose data=coco-pose.yaml device=0`
+- **Speed** averaged over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) instance.
+  <br>Reproduce by `yolo val pose data=coco8-pose.yaml batch=1 device=0|cpu`
 
 </details>
 
 ## <div align="center">Integrations</div>
 
 <br>
-<a align="center" href="https://bit.ly/ultralytics_hub" target="_blank">
+<a href="https://bit.ly/ultralytics_hub" target="_blank">
 <img width="100%" src="https://github.com/ultralytics/assets/raw/main/yolov8/banner-integrations.png"></a>
 <br>
 <br>
 
 <div align="center">
   <a href="https://roboflow.com/?ref=ultralytics">
-    <img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-roboflow.png" width="10%" /></a>
+    <img src="https://github.com/ultralytics/assets/raw/main/partners/logo-roboflow.png" width="10%" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="15%" height="0" alt="" />
   <a href="https://cutt.ly/yolov5-readme-clearml">
-    <img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-clearml.png" width="10%" /></a>
+    <img src="https://github.com/ultralytics/assets/raw/main/partners/logo-clearml.png" width="10%" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="15%" height="0" alt="" />
-  <a href="https://bit.ly/yolov5-readme-comet">
-    <img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-comet.png" width="10%" /></a>
+  <a href="https://bit.ly/yolov8-readme-comet">
+    <img src="https://github.com/ultralytics/assets/raw/main/partners/logo-comet.png" width="10%" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="15%" height="0" alt="" />
   <a href="https://bit.ly/yolov5-neuralmagic">
-    <img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-neuralmagic.png" width="10%" /></a>
+    <img src="https://github.com/ultralytics/assets/raw/main/partners/logo-neuralmagic.png" width="10%" /></a>
 </div>
 
-|                                                           Roboflow                                                           |                                                            ClearML ⭐ NEW                                                            |                                                                        Comet ⭐ NEW                                                                         |                                           Neural Magic ⭐ NEW                                           |
-| :--------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------: |
-| Label and export your custom datasets directly to YOLOv8 for training with [Roboflow](https://roboflow.com/?ref=ultralytics) | Automatically track, visualize and even remotely train YOLOv8 using [ClearML](https://cutt.ly/yolov5-readme-clearml) (open-source!) | Free forever, [Comet](https://bit.ly/yolov5-readme-comet2) lets you save YOLOv8 models, resume training, and interactively visualize and debug predictions | Run YOLOv8 inference up to 6x faster with [Neural Magic DeepSparse](https://bit.ly/yolov5-neuralmagic) |
+|                                                           Roboflow                                                           |                                                            ClearML ⭐ NEW                                                            |                                                                        Comet ⭐ NEW                                                                        |                                           Neural Magic ⭐ NEW                                           |
+| :--------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------: |
+| Label and export your custom datasets directly to YOLOv8 for training with [Roboflow](https://roboflow.com/?ref=ultralytics) | Automatically track, visualize and even remotely train YOLOv8 using [ClearML](https://cutt.ly/yolov5-readme-clearml) (open-source!) | Free forever, [Comet](https://bit.ly/yolov8-readme-comet) lets you save YOLOv8 models, resume training, and interactively visualize and debug predictions | Run YOLOv8 inference up to 6x faster with [Neural Magic DeepSparse](https://bit.ly/yolov5-neuralmagic) |
 
 ## <div align="center">Ultralytics HUB</div>
 
-[Ultralytics HUB](https://bit.ly/ultralytics_hub) is our ⭐ **NEW** no-code solution to visualize datasets, train YOLOv8
-🚀 models, and deploy to the real world in a seamless experience. Get started for **Free** now! Also run YOLOv8 models on
-your iOS or Android device by downloading the [Ultralytics App](https://ultralytics.com/app_install)!
+Experience seamless AI with [Ultralytics HUB](https://bit.ly/ultralytics_hub) ⭐, the all-in-one solution for data visualization, YOLOv5 and YOLOv8 🚀 model training and deployment, without any coding. Transform images into actionable insights and bring your AI visions to life with ease using our cutting-edge platform and user-friendly [Ultralytics App](https://ultralytics.com/app_install). Start your journey for **Free** now!
 
-<a align="center" href="https://bit.ly/ultralytics_hub" target="_blank">
+<a href="https://bit.ly/ultralytics_hub" target="_blank">
 <img width="100%" src="https://github.com/ultralytics/assets/raw/main/im/ultralytics-hub.png"></a>
 
 ## <div align="center">Contribute</div>
 
-We love your input! YOLOv5 and YOLOv8 would not be possible without help from our community. Please see
-our [Contributing Guide](CONTRIBUTING.md) to get started, and fill out
-our [Survey](https://ultralytics.com/survey?utm_source=github&utm_medium=social&utm_campaign=Survey) to send us feedback
-on your experience. Thank you 🙏 to all our contributors!
+We love your input! YOLOv5 and YOLOv8 would not be possible without help from our community. Please see our [Contributing Guide](https://docs.ultralytics.com/help/contributing) to get started, and fill out our [Survey](https://ultralytics.com/survey?utm_source=github&utm_medium=social&utm_campaign=Survey) to send us feedback on your experience. Thank you 🙏 to all our contributors!
 
 <!-- SVG image from https://opencollective.com/ultralytics/contributors.svg?width=990 -->
 
-<a href="https://github.com/ultralytics/ultralytics/graphs/contributors"><img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/image-contributors-1280.png"/></a>
+<a href="https://github.com/ultralytics/yolov5/graphs/contributors">
+<img width="100%" src="https://github.com/ultralytics/assets/raw/main/im/image-contributors.png"></a>
 
 ## <div align="center">License</div>
 
 YOLOv8 is available under two different licenses:
 
-- **GPL-3.0 License**: See [LICENSE](https://github.com/ultralytics/ultralytics/blob/main/LICENSE) file for details.
-- **Enterprise License**: Provides greater flexibility for commercial product development without the open-source
-  requirements of GPL-3.0. Typical use cases are embedding Ultralytics software and AI models in commercial products and
-  applications. Request an Enterprise License at [Ultralytics Licensing](https://ultralytics.com/license).
+- **AGPL-3.0 License**: See [LICENSE](https://github.com/ultralytics/ultralytics/blob/main/LICENSE) file for details.
+- **Enterprise License**: Provides greater flexibility for commercial product development without the open-source requirements of AGPL-3.0. Typical use cases are embedding Ultralytics software and AI models in commercial products and applications. Request an Enterprise License at [Ultralytics Licensing](https://ultralytics.com/license).
 
 ## <div align="center">Contact</div>
 
-For YOLOv8 bugs and feature requests please visit [GitHub Issues](https://github.com/ultralytics/ultralytics/issues).
-For professional support please [Contact Us](https://ultralytics.com/contact).
+For YOLOv8 bug reports and feature requests please visit [GitHub Issues](https://github.com/ultralytics/ultralytics/issues), and join our [Discord](https://discord.gg/n6cFeSPZdD) community for questions and discussions!
 
 <br>
 <div align="center">
   <a href="https://github.com/ultralytics" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
   <a href="https://www.linkedin.com/company/ultralytics" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
   <a href="https://twitter.com/ultralytics" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
-  <a href="https://www.producthunt.com/@glenn_jocher" style="text-decoration:none;">
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-producthunt.png" width="3%" alt="" /></a>
-  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
   <a href="https://youtube.com/ultralytics" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
-  <a href="https://www.facebook.com/ultralytics" style="text-decoration:none;">
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-facebook.png" width="3%" alt="" /></a>
+  <a href="https://www.tiktok.com/@ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-tiktok.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
   <a href="https://www.instagram.com/ultralytics/" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="3%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
+  <a href="https://discord.gg/n6cFeSPZdD" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/blob/main/social/logo-social-discord.png" width="3%" alt="" /></a>
 </div>
```

#### html2text {}

```diff
@@ -1,99 +1,85 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.0.9 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.0.90 Summary: Ultralytics
 YOLOv8 Home-page: https://github.com/ultralytics/ultralytics Author:
-Ultralytics Author-email: hello@ultralytics.com License: GPL-3.0 Project-URL:
+Ultralytics Author-email: hello@ultralytics.com License: AGPL-3.0 Project-URL:
 Bug Reports, https://github.com/ultralytics/ultralytics/issues Project-URL:
 Funding, https://ultralytics.com Project-URL: Source, https://github.com/
 ultralytics/ultralytics Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Science/
-Research Classifier: License :: OSI Approved :: GNU General Public License v3
-(GPLv3) Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Topic :: Software Development
+Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: GNU Affero General
+Public License v3 or later (AGPLv3+) Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Scientific/
 Engineering :: Image Recognition Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS Classifier: Operating System :: Microsoft
-:: Windows Requires-Python: >=3.7,<=3.11 Description-Content-Type: text/
-markdown Provides-Extra: dev License-File: LICENSE
+:: Windows Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: export License-File: LICENSE
    [https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/banner-
                                   yolov8.png]
             [English](README.md) | [ç®ä½ä¸­æ](README.zh-CN.md)
               [Ultralytics_CI] [YOLOv8_Citation] [Docker_Pulls]
               [Run_on_Gradient] [Open_In_Colab] [Open_In_Kaggle]
 
-[Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics), developed by
- [Ultralytics](https://ultralytics.com), is a cutting-edge, state-of-the-art
-    (SOTA) model that builds upon the success of previous YOLO versions and
-   introduces new features and improvements to further boost performance and
- flexibility. YOLOv8 is designed to be fast, accurate, and easy to use, making
-it an excellent choice for a wide range of object detection, image segmentation
-    and image classification tasks. To request an Enterprise License please
-complete the form at [Ultralytics Licensing](https://ultralytics.com/license).
-    [https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/yolo-
-                             comparison-plots.png]
+[Ultralytics](https://ultralytics.com) [YOLOv8](https://github.com/ultralytics/
+ultralytics) is a cutting-edge, state-of-the-art (SOTA) model that builds upon
+     the success of previous YOLO versions and introduces new features and
+ improvements to further boost performance and flexibility. YOLOv8 is designed
+to be fast, accurate, and easy to use, making it an excellent choice for a wide
+     range of object detection and tracking, instance segmentation, image
+classification and pose estimation tasks. We hope that the resources here will
+help you get the most out of YOLOv8. Please browse the YOLOv8 Docs for details,
+   raise an issue on GitHub for support, and join our Discord community for
+questions and discussions! To request an Enterprise License please complete the
+  form at [Ultralytics Licensing](https://ultralytics.com/license). [https://
+   raw.githubusercontent.com/ultralytics/assets/main/yolov8/yolo-comparison-
+                                  plots.png]
 
 ##
-                           Ultralytics Live Session
-[Ultralytics Live Session 3](https://youtu.be/IPcpYO5ITa8) â¨ is here! Join us
- on January 24th at 18 CET as we dive into the latest advancements in YOLOv8,
-and demonstrate how to use this cutting-edge, SOTA model to improve your object
-   detection, instance segmentation, and image classification projects. See
- firsthand how YOLOv8's speed, accuracy, and ease of use make it a top choice
-  for professionals and researchers alike. In addition to learning about the
-  exciting new features and improvements of Ultralytics YOLOv8, you will also
-  have the opportunity to ask questions and interact with our team during the
-live Q&A session. We encourage you to come prepared with any questions you may
-have. To join the webinar, visit our YouTube [Channel](https://www.youtube.com/
-     @Ultralytics/streams) and turn on your notifications! [https://user-
-   images.githubusercontent.com/107626595/212887899-e94b006c-5192-40fa-8b24-
-                               7b5428e065e8.png]
-##
                                  Documentation
 See below for a quickstart installation and usage example, and see the [YOLOv8
 Docs](https://docs.ultralytics.com) for full documentation on training,
 validation, prediction and deployment.  Install Pip install the ultralytics
-package including all [requirements.txt](https://github.com/ultralytics/
-ultralytics/blob/main/requirements.txt) in a [**3.10>=Python>=3.7**](https://
-www.python.org/) environment, including [**PyTorch>=1.7**](https://pytorch.org/
-get-started/locally/). ```bash pip install ultralytics ```   Usage #### CLI
-YOLOv8 may be used directly in the Command Line Interface (CLI) with a `yolo`
-command: ```bash yolo predict model=yolov8n.pt source="https://ultralytics.com/
-images/bus.jpg" ``` `yolo` can be used for a variety of tasks and modes and
-accepts additional arguments, i.e. `imgsz=640`. See the YOLOv8 [CLI Docs]
-(https://docs.ultralytics.com/cli) for examples. #### Python YOLOv8 may also be
+package including all [requirements](https://github.com/ultralytics/
+ultralytics/blob/main/requirements.txt) in a [**Python>=3.7**](https://
+www.python.org/) environment with [**PyTorch>=1.7**](https://pytorch.org/get-
+started/locally/). ```bash pip install ultralytics ```   Usage #### CLI YOLOv8
+may be used directly in the Command Line Interface (CLI) with a `yolo` command:
+```bash yolo predict model=yolov8n.pt source='https://ultralytics.com/images/
+bus.jpg' ``` `yolo` can be used for a variety of tasks and modes and accepts
+additional arguments, i.e. `imgsz=640`. See the YOLOv8 [CLI Docs](https://
+docs.ultralytics.com/usage/cli) for examples. #### Python YOLOv8 may also be
 used directly in a Python environment, and accepts the same [arguments](https:/
-/docs.ultralytics.com/config/) as in the CLI example above: ```python from
+/docs.ultralytics.com/usage/cfg/) as in the CLI example above: ```python from
 ultralytics import YOLO # Load a model model = YOLO("yolov8n.yaml") # build a
 new model from scratch model = YOLO("yolov8n.pt") # load a pretrained model
-(recommended for training) # Use the model results = model.train
-(data="coco128.yaml", epochs=3) # train the model results = model.val() #
-evaluate model performance on the validation set results = model("https://
-ultralytics.com/images/bus.jpg") # predict on an image success = model.export
-(format="onnx") # export the model to ONNX format ``` [Models](https://
-github.com/ultralytics/ultralytics/tree/main/ultralytics/models) download
-automatically from the latest Ultralytics [release](https://github.com/
-ultralytics/assets/releases). See YOLOv8 [Python Docs](https://
-docs.ultralytics.com/python) for more examples. #### Known Issues / TODOs We
-are still working on several parts of YOLOv8! We aim to have these completed
-soon to bring the YOLOv8 feature set up to par with YOLOv5, including export
-and inference to all the same formats. We are also writing a YOLOv8 paper which
-we will submit to [arxiv.org](https://arxiv.org) once complete. - [ ]
-TensorFlow exports - [ ] DDP resume - [ ] [arxiv.org](https://arxiv.org) paper
-##
+(recommended for training) # Use the model model.train(data="coco128.yaml",
+epochs=3) # train the model metrics = model.val() # evaluate model performance
+on the validation set results = model("https://ultralytics.com/images/bus.jpg")
+# predict on an image success = model.export(format="onnx") # export the model
+to ONNX format ``` [Models](https://github.com/ultralytics/ultralytics/tree/
+main/ultralytics/models) download automatically from the latest Ultralytics
+[release](https://github.com/ultralytics/assets/releases). See YOLOv8 [Python
+Docs](https://docs.ultralytics.com/usage/python) for more examples.  ##
                                     Models
-All YOLOv8 pretrained models are available here. Detection and Segmentation
-models are pretrained on the COCO dataset, while Classification models are
-pretrained on the ImageNet dataset. [Models](https://github.com/ultralytics/
-ultralytics/tree/main/ultralytics/models) download automatically from the
-latest Ultralytics [release](https://github.com/ultralytics/assets/releases) on
-first use. Detection See [Detection Docs](https://docs.ultralytics.com/tasks/
-detection/) for usage examples with these models. | Model | size
+All YOLOv8 pretrained models are available here. Detect, Segment and Pose
+models are pretrained on the [COCO](https://github.com/ultralytics/ultralytics/
+blob/main/ultralytics/datasets/coco.yaml) dataset, while Classify models are
+pretrained on the [ImageNet](https://github.com/ultralytics/ultralytics/blob/
+main/ultralytics/datasets/ImageNet.yaml) dataset. [Models](https://github.com/
+ultralytics/ultralytics/tree/main/ultralytics/models) download automatically
+from the latest Ultralytics [release](https://github.com/ultralytics/assets/
+releases) on first use. Detection See [Detection Docs](https://
+docs.ultralytics.com/tasks/detect/) for usage examples with these models. |
+Model | size
 (pixels) | mAPval
 50-95 | Speed
 CPU ONNX
 (ms) | Speed
 A100 TensorRT
 (ms) | params
 (M) | FLOPs
@@ -110,119 +96,151 @@
 | 165.2 | | [YOLOv8x](https://github.com/ultralytics/assets/releases/download/
 v0.0.0/yolov8x.pt) | 640 | 53.9 | 479.1 | 3.53 | 68.2 | 257.8 | - **mAPval**
 values are for single-model single-scale on [COCO val2017](http://
 cocodataset.org) dataset.
 Reproduce by `yolo val detect data=coco.yaml device=0` - **Speed** averaged
 over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/
 instance-types/p4/) instance.
-Reproduce by `yolo val detect data=coco128.yaml batch=1 device=0/cpu`
+Reproduce by `yolo val detect data=coco128.yaml batch=1 device=0|cpu`
 Segmentation See [Segmentation Docs](https://docs.ultralytics.com/tasks/
-segmentation/) for usage examples with these models. | Model | size
+segment/) for usage examples with these models. | Model | size
 (pixels) | mAPbox
 50-95 | mAPmask
 50-95 | Speed
 CPU ONNX
 (ms) | Speed
 A100 TensorRT
 (ms) | params
 (M) | FLOPs
 (B) | | -----------------------------------------------------------------------
------------------ | --------------------- | -------------------- | ------------
---------- | ------------------------------ | ----------------------------------
-- | ------------------ | ----------------- | | [YOLOv8n](https://github.com/
-ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640 | 36.7 | 30.5
-| 96.1 | 1.21 | 3.4 | 12.6 | | [YOLOv8s](https://github.com/ultralytics/assets/
-releases/download/v0.0.0/yolov8s-seg.pt) | 640 | 44.6 | 36.8 | 155.7 | 1.47 |
-11.8 | 42.6 | | [YOLOv8m](https://github.com/ultralytics/assets/releases/
-download/v0.0.0/yolov8m-seg.pt) | 640 | 49.9 | 40.8 | 317.0 | 2.18 | 27.3 |
-110.2 | | [YOLOv8l](https://github.com/ultralytics/assets/releases/download/
-v0.0.0/yolov8l-seg.pt) | 640 | 52.3 | 42.6 | 572.4 | 2.79 | 46.0 | 220.5 | |
-[YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/
-yolov8x-seg.pt) | 640 | 53.4 | 43.4 | 712.1 | 4.02 | 71.8 | 344.1 | -
-**mAPval** values are for single-model single-scale on [COCO val2017](http://
-cocodataset.org) dataset.
+--------------------- | --------------------- | -------------------- | --------
+------------- | ------------------------------ | ------------------------------
+----- | ------------------ | ----------------- | | [YOLOv8n-seg](https://
+github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640 |
+36.7 | 30.5 | 96.1 | 1.21 | 3.4 | 12.6 | | [YOLOv8s-seg](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8s-seg.pt) | 640 | 44.6 | 36.8
+| 155.7 | 1.47 | 11.8 | 42.6 | | [YOLOv8m-seg](https://github.com/ultralytics/
+assets/releases/download/v0.0.0/yolov8m-seg.pt) | 640 | 49.9 | 40.8 | 317.0 |
+2.18 | 27.3 | 110.2 | | [YOLOv8l-seg](https://github.com/ultralytics/assets/
+releases/download/v0.0.0/yolov8l-seg.pt) | 640 | 52.3 | 42.6 | 572.4 | 2.79 |
+46.0 | 220.5 | | [YOLOv8x-seg](https://github.com/ultralytics/assets/releases/
+download/v0.0.0/yolov8x-seg.pt) | 640 | 53.4 | 43.4 | 712.1 | 4.02 | 71.8 |
+344.1 | - **mAPval** values are for single-model single-scale on [COCO val2017]
+(http://cocodataset.org) dataset.
 Reproduce by `yolo val segment data=coco.yaml device=0` - **Speed** averaged
 over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/
 instance-types/p4/) instance.
-Reproduce by `yolo val segment data=coco128-seg.yaml batch=1 device=0/cpu`
+Reproduce by `yolo val segment data=coco128-seg.yaml batch=1 device=0|cpu`
 Classification See [Classification Docs](https://docs.ultralytics.com/tasks/
-classification/) for usage examples with these models. | Model | size
+classify/) for usage examples with these models. | Model | size
 (pixels) | acc
 top1 | acc
 top5 | Speed
 CPU ONNX
 (ms) | Speed
 A100 TensorRT
 (ms) | params
 (M) | FLOPs
 (B) at 640 | | ----------------------------------------------------------------
------------------------- | --------------------- | ---------------- | ---------
-------- | ------------------------------ | ----------------------------------
-- | ------------------ | ------------------------ | | [YOLOv8n](https://
+---------------------------- | --------------------- | ---------------- | -----
+----------- | ------------------------------ | --------------------------------
+--- | ------------------ | ------------------------ | | [YOLOv8n-cls](https://
 github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-cls.pt) | 224 |
-66.6 | 87.0 | 12.9 | 0.31 | 2.7 | 4.3 | | [YOLOv8s](https://github.com/
+66.6 | 87.0 | 12.9 | 0.31 | 2.7 | 4.3 | | [YOLOv8s-cls](https://github.com/
 ultralytics/assets/releases/download/v0.0.0/yolov8s-cls.pt) | 224 | 72.3 | 91.1
-| 23.4 | 0.35 | 6.4 | 13.5 | | [YOLOv8m](https://github.com/ultralytics/assets/
-releases/download/v0.0.0/yolov8m-cls.pt) | 224 | 76.4 | 93.2 | 85.4 | 0.62 |
-17.0 | 42.7 | | [YOLOv8l](https://github.com/ultralytics/assets/releases/
-download/v0.0.0/yolov8l-cls.pt) | 224 | 78.0 | 94.1 | 163.0 | 0.87 | 37.5 |
-99.7 | | [YOLOv8x](https://github.com/ultralytics/assets/releases/download/
-v0.0.0/yolov8x-cls.pt) | 224 | 78.4 | 94.3 | 232.0 | 1.01 | 57.4 | 154.8 | -
-**acc** values are model accuracies on the [ImageNet](https://www.image-
-net.org/) dataset validation set.
+| 23.4 | 0.35 | 6.4 | 13.5 | | [YOLOv8m-cls](https://github.com/ultralytics/
+assets/releases/download/v0.0.0/yolov8m-cls.pt) | 224 | 76.4 | 93.2 | 85.4 |
+0.62 | 17.0 | 42.7 | | [YOLOv8l-cls](https://github.com/ultralytics/assets/
+releases/download/v0.0.0/yolov8l-cls.pt) | 224 | 78.0 | 94.1 | 163.0 | 0.87 |
+37.5 | 99.7 | | [YOLOv8x-cls](https://github.com/ultralytics/assets/releases/
+download/v0.0.0/yolov8x-cls.pt) | 224 | 78.4 | 94.3 | 232.0 | 1.01 | 57.4 |
+154.8 | - **acc** values are model accuracies on the [ImageNet](https://
+www.image-net.org/) dataset validation set.
 Reproduce by `yolo val classify data=path/to/ImageNet device=0` - **Speed**
 averaged over ImageNet val images using an [Amazon EC2 P4d](https://
 aws.amazon.com/ec2/instance-types/p4/) instance.
-Reproduce by `yolo val classify data=path/to/ImageNet batch=1 device=0/cpu`  ##
+Reproduce by `yolo val classify data=path/to/ImageNet batch=1 device=0|cpu`
+Pose See [Pose Docs](https://docs.ultralytics.com/tasks/pose) for usage
+examples with these models. | Model | size
+(pixels) | mAPpose
+50-95 | mAPpose
+50 | Speed
+CPU ONNX
+(ms) | Speed
+A100 TensorRT
+(ms) | params
+(M) | FLOPs
+(B) | | -----------------------------------------------------------------------
+----------------------------- | --------------------- | --------------------- |
+------------------ | ------------------------------ | -------------------------
+---------- | ------------------ | ----------------- | | [YOLOv8n-pose](https://
+github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-pose.pt) | 640 |
+50.4 | 80.1 | 131.8 | 1.18 | 3.3 | 9.2 | | [YOLOv8s-pose](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8s-pose.pt) | 640 | 60.0 |
+86.2 | 233.2 | 1.42 | 11.6 | 30.2 | | [YOLOv8m-pose](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8m-pose.pt) | 640 | 65.0 |
+88.8 | 456.3 | 2.00 | 26.4 | 81.0 | | [YOLOv8l-pose](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8l-pose.pt) | 640 | 67.6 |
+90.0 | 784.5 | 2.59 | 44.4 | 168.6 | | [YOLOv8x-pose](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8x-pose.pt) | 640 | 69.2 |
+90.2 | 1607.1 | 3.73 | 69.4 | 263.2 | | [YOLOv8x-pose-p6](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8x-pose-p6.pt) | 1280 | 71.6 |
+91.2 | 4088.7 | 10.04 | 99.1 | 1066.4 | - **mAPval** values are for single-
+model single-scale on [COCO Keypoints val2017](http://cocodataset.org) dataset.
+
+Reproduce by `yolo val pose data=coco-pose.yaml device=0` - **Speed** averaged
+over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/
+instance-types/p4/) instance.
+Reproduce by `yolo val pose data=coco8-pose.yaml batch=1 device=0|cpu`  ##
                                  Integrations
 
 [https://github.com/ultralytics/assets/raw/main/yolov8/banner-integrations.png]
 
 
-      [https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-
- roboflow.png]  [https://github.com/ultralytics/yolov5/releases/download/v1.0/
- logo-clearml.png]  [https://github.com/ultralytics/yolov5/releases/download/
-v1.0/logo-comet.png]  [https://github.com/ultralytics/yolov5/releases/download/
-                          v1.0/logo-neuralmagic.png]
+ [https://github.com/ultralytics/assets/raw/main/partners/logo-roboflow.png]
+ [https://github.com/ultralytics/assets/raw/main/partners/logo-clearml.png]
+  [https://github.com/ultralytics/assets/raw/main/partners/logo-comet.png]
+[https://github.com/ultralytics/assets/raw/main/partners/logo-neuralmagic.png]
 | Roboflow | ClearML â­ NEW | Comet â­ NEW | Neural Magic â­ NEW | | :------
 -------------------------------------------------------------------------------
 -------------------------------------: | :-------------------------------------
 -------------------------------------------------------------------------------
 -------------: | :-------------------------------------------------------------
 -------------------------------------------------------------------------------
-------------: | :--------------------------------------------------------------
---------------------------------------: | | Label and export your custom
+-----------: | :---------------------------------------------------------------
+-------------------------------------: | | Label and export your custom
 datasets directly to YOLOv8 for training with [Roboflow](https://roboflow.com/
 ?ref=ultralytics) | Automatically track, visualize and even remotely train
 YOLOv8 using [ClearML](https://cutt.ly/yolov5-readme-clearml) (open-source!) |
-Free forever, [Comet](https://bit.ly/yolov5-readme-comet2) lets you save YOLOv8
+Free forever, [Comet](https://bit.ly/yolov8-readme-comet) lets you save YOLOv8
 models, resume training, and interactively visualize and debug predictions |
 Run YOLOv8 inference up to 6x faster with [Neural Magic DeepSparse](https://
 bit.ly/yolov5-neuralmagic) | ##
                                 Ultralytics HUB
-[Ultralytics HUB](https://bit.ly/ultralytics_hub) is our â­ **NEW** no-code
-solution to visualize datasets, train YOLOv8 ð models, and deploy to the
-real world in a seamless experience. Get started for **Free** now! Also run
-YOLOv8 models on your iOS or Android device by downloading the [Ultralytics
-App](https://ultralytics.com/app_install)! [https://github.com/ultralytics/
-assets/raw/main/im/ultralytics-hub.png] ##
+Experience seamless AI with [Ultralytics HUB](https://bit.ly/ultralytics_hub)
+â­, the all-in-one solution for data visualization, YOLOv5 and YOLOv8 ð
+model training and deployment, without any coding. Transform images into
+actionable insights and bring your AI visions to life with ease using our
+cutting-edge platform and user-friendly [Ultralytics App](https://
+ultralytics.com/app_install). Start your journey for **Free** now! [https://
+github.com/ultralytics/assets/raw/main/im/ultralytics-hub.png] ##
                                   Contribute
 We love your input! YOLOv5 and YOLOv8 would not be possible without help from
-our community. Please see our [Contributing Guide](CONTRIBUTING.md) to get
-started, and fill out our [Survey](https://ultralytics.com/
+our community. Please see our [Contributing Guide](https://
+docs.ultralytics.com/help/contributing) to get started, and fill out our
+[Survey](https://ultralytics.com/
 survey?utm_source=github&utm_medium=social&utm_campaign=Survey) to send us
 feedback on your experience. Thank you ð to all our contributors!  [https://
-github.com/ultralytics/yolov5/releases/download/v1.0/image-contributors-
-1280.png] ##
+github.com/ultralytics/assets/raw/main/im/image-contributors.png] ##
                                     License
-YOLOv8 is available under two different licenses: - **GPL-3.0 License**: See
+YOLOv8 is available under two different licenses: - **AGPL-3.0 License**: See
 [LICENSE](https://github.com/ultralytics/ultralytics/blob/main/LICENSE) file
 for details. - **Enterprise License**: Provides greater flexibility for
-commercial product development without the open-source requirements of GPL-3.0.
-Typical use cases are embedding Ultralytics software and AI models in
+commercial product development without the open-source requirements of AGPL-
+3.0. Typical use cases are embedding Ultralytics software and AI models in
 commercial products and applications. Request an Enterprise License at
 [Ultralytics Licensing](https://ultralytics.com/license). ##
                                     Contact
-For YOLOv8 bugs and feature requests please visit [GitHub Issues](https://
-github.com/ultralytics/ultralytics/issues). For professional support please
-[Contact Us](https://ultralytics.com/contact).
+For YOLOv8 bug reports and feature requests please visit [GitHub Issues](https:
+//github.com/ultralytics/ultralytics/issues), and join our [Discord](https://
+discord.gg/n6cFeSPZdD) community for questions and discussions!
```

### Comparing `ultralytics-8.0.9/README.md` & `ultralytics-8.0.90/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <div align="center">
   <p>
-    <a align="center" href="https://ultralytics.com/yolov8" target="_blank">
+    <a href="https://ultralytics.com/yolov8" target="_blank">
       <img width="100%" src="https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/banner-yolov8.png"></a>
   </p>
 
 [English](README.md) | [简体中文](README.zh-CN.md)
 <br>
 
 <div>
@@ -14,80 +14,54 @@
     <br>
     <a href="https://console.paperspace.com/github/ultralytics/ultralytics"><img src="https://assets.paperspace.io/img/gradient-badge.svg" alt="Run on Gradient"/></a>
     <a href="https://colab.research.google.com/github/ultralytics/ultralytics/blob/main/examples/tutorial.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>
     <a href="https://www.kaggle.com/ultralytics/yolov8"><img src="https://kaggle.com/static/images/open-in-kaggle.svg" alt="Open In Kaggle"></a>
   </div>
   <br>
 
-[Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics), developed by [Ultralytics](https://ultralytics.com),
-is a cutting-edge, state-of-the-art (SOTA) model that builds upon the success of previous YOLO versions and introduces
-new features and improvements to further boost performance and flexibility. YOLOv8 is designed to be fast, accurate, and
-easy to use, making it an excellent choice for a wide range of object detection, image segmentation and image
-classification tasks.
+[Ultralytics](https://ultralytics.com) [YOLOv8](https://github.com/ultralytics/ultralytics) is a cutting-edge, state-of-the-art (SOTA) model that builds upon the success of previous YOLO versions and introduces new features and improvements to further boost performance and flexibility. YOLOv8 is designed to be fast, accurate, and easy to use, making it an excellent choice for a wide range of object detection and tracking, instance segmentation, image classification and pose estimation tasks.
+
+We hope that the resources here will help you get the most out of YOLOv8. Please browse the YOLOv8 <a href="https://docs.ultralytics.com/">Docs</a> for details, raise an issue on <a href="https://github.com/ultralytics/ultralytics/issues/new/choose">GitHub</a> for support, and join our <a href="https://discord.gg/n6cFeSPZdD">Discord</a> community for questions and discussions!
 
 To request an Enterprise License please complete the form at [Ultralytics Licensing](https://ultralytics.com/license).
 
 <img width="100%" src="https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/yolo-comparison-plots.png"></a>
 
 <div align="center">
-    <a href="https://github.com/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://www.linkedin.com/company/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://twitter.com/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://www.producthunt.com/@glenn_jocher" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-producthunt.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://youtube.com/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://www.facebook.com/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-facebook.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://www.instagram.com/ultralytics/" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="2%" alt="" /></a>
-  </div>
+  <a href="https://github.com/ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://www.linkedin.com/company/ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://twitter.com/ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://youtube.com/ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://www.tiktok.com/@ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-tiktok.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://www.instagram.com/ultralytics/" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://discord.gg/n6cFeSPZdD" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/blob/main/social/logo-social-discord.png" width="2%" alt="" /></a>
 </div>
-
-## <div align="center">Ultralytics Live Session</div>
-
-<div align="center">
-
-[Ultralytics Live Session 3](https://youtu.be/IPcpYO5ITa8) ✨ is here! Join us on January 24th at 18 CET as we dive into
-the latest advancements in YOLOv8, and demonstrate how to use this cutting-edge, SOTA model to improve your object
-detection, instance segmentation, and image classification projects. See firsthand how YOLOv8's speed, accuracy, and
-ease of use make it a top choice for professionals and researchers alike.
-
-In addition to learning about the exciting new features and improvements of Ultralytics YOLOv8, you will also have the
-opportunity to ask questions and interact with our team during the live Q&A session. We encourage you to come prepared
-with any questions you may have.
-
-To join the webinar, visit our YouTube [Channel](https://www.youtube.com/@Ultralytics/streams) and turn on your
-notifications!
-
-<a align="center" href="https://youtu.be/IPcpYO5ITa8" target="_blank">
-<img width="80%" src="https://user-images.githubusercontent.com/107626595/212887899-e94b006c-5192-40fa-8b24-7b5428e065e8.png"></a>
 </div>
 
 ## <div align="center">Documentation</div>
 
-See below for a quickstart installation and usage example, and see the [YOLOv8 Docs](https://docs.ultralytics.com) for
-full documentation on training, validation, prediction and deployment.
+See below for a quickstart installation and usage example, and see the [YOLOv8 Docs](https://docs.ultralytics.com) for full documentation on training, validation, prediction and deployment.
 
 <details open>
 <summary>Install</summary>
 
-Pip install the ultralytics package including
-all [requirements.txt](https://github.com/ultralytics/ultralytics/blob/main/requirements.txt) in a
-[**3.10>=Python>=3.7**](https://www.python.org/) environment, including
-[**PyTorch>=1.7**](https://pytorch.org/get-started/locally/).
+Pip install the ultralytics package including all [requirements](https://github.com/ultralytics/ultralytics/blob/main/requirements.txt) in a [**Python>=3.7**](https://www.python.org/) environment with [**PyTorch>=1.7**](https://pytorch.org/get-started/locally/).
 
 ```bash
 pip install ultralytics
 ```
 
 </details>
 
@@ -95,199 +69,194 @@
 <summary>Usage</summary>
 
 #### CLI
 
 YOLOv8 may be used directly in the Command Line Interface (CLI) with a `yolo` command:
 
 ```bash
-yolo predict model=yolov8n.pt source="https://ultralytics.com/images/bus.jpg"
+yolo predict model=yolov8n.pt source='https://ultralytics.com/images/bus.jpg'
 ```
 
-`yolo` can be used for a variety of tasks and modes and accepts additional arguments, i.e. `imgsz=640`. See the YOLOv8
-[CLI Docs](https://docs.ultralytics.com/cli) for examples.
+`yolo` can be used for a variety of tasks and modes and accepts additional arguments, i.e. `imgsz=640`. See the YOLOv8 [CLI Docs](https://docs.ultralytics.com/usage/cli) for examples.
 
 #### Python
 
-YOLOv8 may also be used directly in a Python environment, and accepts the
-same [arguments](https://docs.ultralytics.com/config/) as in the CLI example above:
+YOLOv8 may also be used directly in a Python environment, and accepts the same [arguments](https://docs.ultralytics.com/usage/cfg/) as in the CLI example above:
 
 ```python
 from ultralytics import YOLO
 
 # Load a model
 model = YOLO("yolov8n.yaml")  # build a new model from scratch
 model = YOLO("yolov8n.pt")  # load a pretrained model (recommended for training)
 
 # Use the model
-results = model.train(data="coco128.yaml", epochs=3)  # train the model
-results = model.val()  # evaluate model performance on the validation set
+model.train(data="coco128.yaml", epochs=3)  # train the model
+metrics = model.val()  # evaluate model performance on the validation set
 results = model("https://ultralytics.com/images/bus.jpg")  # predict on an image
 success = model.export(format="onnx")  # export the model to ONNX format
 ```
 
-[Models](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) download automatically from the latest
-Ultralytics [release](https://github.com/ultralytics/assets/releases). See
-YOLOv8 [Python Docs](https://docs.ultralytics.com/python) for more examples.
-
-#### Known Issues / TODOs
-
-We are still working on several parts of YOLOv8! We aim to have these completed soon to bring the YOLOv8 feature set up
-to par with YOLOv5, including export and inference to all the same formats. We are also writing a YOLOv8 paper which we
-will submit to [arxiv.org](https://arxiv.org) once complete.
-
-- [ ] TensorFlow exports
-- [ ] DDP resume
-- [ ] [arxiv.org](https://arxiv.org) paper
+[Models](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) download automatically from the latest Ultralytics [release](https://github.com/ultralytics/assets/releases). See YOLOv8 [Python Docs](https://docs.ultralytics.com/usage/python) for more examples.
 
 </details>
 
 ## <div align="center">Models</div>
 
-All YOLOv8 pretrained models are available here. Detection and Segmentation models are pretrained on the COCO dataset,
-while Classification models are pretrained on the ImageNet dataset.
+All YOLOv8 pretrained models are available here. Detect, Segment and Pose models are pretrained on the [COCO](https://github.com/ultralytics/ultralytics/blob/main/ultralytics/datasets/coco.yaml) dataset, while Classify models are pretrained on the [ImageNet](https://github.com/ultralytics/ultralytics/blob/main/ultralytics/datasets/ImageNet.yaml) dataset.
 
-[Models](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) download automatically from the latest
-Ultralytics [release](https://github.com/ultralytics/assets/releases) on first use.
+[Models](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) download automatically from the latest Ultralytics [release](https://github.com/ultralytics/assets/releases) on first use.
 
 <details open><summary>Detection</summary>
 
-See [Detection Docs](https://docs.ultralytics.com/tasks/detection/) for usage examples with these models.
+See [Detection Docs](https://docs.ultralytics.com/tasks/detect/) for usage examples with these models.
 
 | Model                                                                                | size<br><sup>(pixels) | mAP<sup>val<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |
 | ------------------------------------------------------------------------------------ | --------------------- | -------------------- | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
 | [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n.pt) | 640                   | 37.3                 | 80.4                           | 0.99                                | 3.2                | 8.7               |
 | [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s.pt) | 640                   | 44.9                 | 128.4                          | 1.20                                | 11.2               | 28.6              |
 | [YOLOv8m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m.pt) | 640                   | 50.2                 | 234.7                          | 1.83                                | 25.9               | 78.9              |
 | [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l.pt) | 640                   | 52.9                 | 375.2                          | 2.39                                | 43.7               | 165.2             |
 | [YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x.pt) | 640                   | 53.9                 | 479.1                          | 3.53                                | 68.2               | 257.8             |
 
 - **mAP<sup>val</sup>** values are for single-model single-scale on [COCO val2017](http://cocodataset.org) dataset.
   <br>Reproduce by `yolo val detect data=coco.yaml device=0`
-- **Speed** averaged over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/)
-  instance.
-  <br>Reproduce by `yolo val detect data=coco128.yaml batch=1 device=0/cpu`
+- **Speed** averaged over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) instance.
+  <br>Reproduce by `yolo val detect data=coco128.yaml batch=1 device=0|cpu`
 
 </details>
 
 <details><summary>Segmentation</summary>
 
-See [Segmentation Docs](https://docs.ultralytics.com/tasks/segmentation/) for usage examples with these models.
+See [Segmentation Docs](https://docs.ultralytics.com/tasks/segment/) for usage examples with these models.
 
-| Model                                                                                    | size<br><sup>(pixels) | mAP<sup>box<br>50-95 | mAP<sup>mask<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |
-| ---------------------------------------------------------------------------------------- | --------------------- | -------------------- | --------------------- | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
-| [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640                   | 36.7                 | 30.5                  | 96.1                           | 1.21                                | 3.4                | 12.6              |
-| [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-seg.pt) | 640                   | 44.6                 | 36.8                  | 155.7                          | 1.47                                | 11.8               | 42.6              |
-| [YOLOv8m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-seg.pt) | 640                   | 49.9                 | 40.8                  | 317.0                          | 2.18                                | 27.3               | 110.2             |
-| [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-seg.pt) | 640                   | 52.3                 | 42.6                  | 572.4                          | 2.79                                | 46.0               | 220.5             |
-| [YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-seg.pt) | 640                   | 53.4                 | 43.4                  | 712.1                          | 4.02                                | 71.8               | 344.1             |
+| Model                                                                                        | size<br><sup>(pixels) | mAP<sup>box<br>50-95 | mAP<sup>mask<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |
+| -------------------------------------------------------------------------------------------- | --------------------- | -------------------- | --------------------- | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
+| [YOLOv8n-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640                   | 36.7                 | 30.5                  | 96.1                           | 1.21                                | 3.4                | 12.6              |
+| [YOLOv8s-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-seg.pt) | 640                   | 44.6                 | 36.8                  | 155.7                          | 1.47                                | 11.8               | 42.6              |
+| [YOLOv8m-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-seg.pt) | 640                   | 49.9                 | 40.8                  | 317.0                          | 2.18                                | 27.3               | 110.2             |
+| [YOLOv8l-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-seg.pt) | 640                   | 52.3                 | 42.6                  | 572.4                          | 2.79                                | 46.0               | 220.5             |
+| [YOLOv8x-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-seg.pt) | 640                   | 53.4                 | 43.4                  | 712.1                          | 4.02                                | 71.8               | 344.1             |
 
 - **mAP<sup>val</sup>** values are for single-model single-scale on [COCO val2017](http://cocodataset.org) dataset.
   <br>Reproduce by `yolo val segment data=coco.yaml device=0`
-- **Speed** averaged over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/)
-  instance.
-  <br>Reproduce by `yolo val segment data=coco128-seg.yaml batch=1 device=0/cpu`
+- **Speed** averaged over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) instance.
+  <br>Reproduce by `yolo val segment data=coco128-seg.yaml batch=1 device=0|cpu`
 
 </details>
 
 <details><summary>Classification</summary>
 
-See [Classification Docs](https://docs.ultralytics.com/tasks/classification/) for usage examples with these models.
+See [Classification Docs](https://docs.ultralytics.com/tasks/classify/) for usage examples with these models.
 
-| Model                                                                                    | size<br><sup>(pixels) | acc<br><sup>top1 | acc<br><sup>top5 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) at 640 |
-| ---------------------------------------------------------------------------------------- | --------------------- | ---------------- | ---------------- | ------------------------------ | ----------------------------------- | ------------------ | ------------------------ |
-| [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-cls.pt) | 224                   | 66.6             | 87.0             | 12.9                           | 0.31                                | 2.7                | 4.3                      |
-| [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-cls.pt) | 224                   | 72.3             | 91.1             | 23.4                           | 0.35                                | 6.4                | 13.5                     |
-| [YOLOv8m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-cls.pt) | 224                   | 76.4             | 93.2             | 85.4                           | 0.62                                | 17.0               | 42.7                     |
-| [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-cls.pt) | 224                   | 78.0             | 94.1             | 163.0                          | 0.87                                | 37.5               | 99.7                     |
-| [YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-cls.pt) | 224                   | 78.4             | 94.3             | 232.0                          | 1.01                                | 57.4               | 154.8                    |
+| Model                                                                                        | size<br><sup>(pixels) | acc<br><sup>top1 | acc<br><sup>top5 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) at 640 |
+| -------------------------------------------------------------------------------------------- | --------------------- | ---------------- | ---------------- | ------------------------------ | ----------------------------------- | ------------------ | ------------------------ |
+| [YOLOv8n-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-cls.pt) | 224                   | 66.6             | 87.0             | 12.9                           | 0.31                                | 2.7                | 4.3                      |
+| [YOLOv8s-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-cls.pt) | 224                   | 72.3             | 91.1             | 23.4                           | 0.35                                | 6.4                | 13.5                     |
+| [YOLOv8m-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-cls.pt) | 224                   | 76.4             | 93.2             | 85.4                           | 0.62                                | 17.0               | 42.7                     |
+| [YOLOv8l-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-cls.pt) | 224                   | 78.0             | 94.1             | 163.0                          | 0.87                                | 37.5               | 99.7                     |
+| [YOLOv8x-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-cls.pt) | 224                   | 78.4             | 94.3             | 232.0                          | 1.01                                | 57.4               | 154.8                    |
 
 - **acc** values are model accuracies on the [ImageNet](https://www.image-net.org/) dataset validation set.
   <br>Reproduce by `yolo val classify data=path/to/ImageNet device=0`
-- **Speed** averaged over ImageNet val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/)
-  instance.
-  <br>Reproduce by `yolo val classify data=path/to/ImageNet batch=1 device=0/cpu`
+- **Speed** averaged over ImageNet val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) instance.
+  <br>Reproduce by `yolo val classify data=path/to/ImageNet batch=1 device=0|cpu`
+
+</details>
+
+<details><summary>Pose</summary>
+
+See [Pose Docs](https://docs.ultralytics.com/tasks/pose) for usage examples with these models.
+
+| Model                                                                                                | size<br><sup>(pixels) | mAP<sup>pose<br>50-95 | mAP<sup>pose<br>50 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |
+| ---------------------------------------------------------------------------------------------------- | --------------------- | --------------------- | ------------------ | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
+| [YOLOv8n-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-pose.pt)       | 640                   | 50.4                  | 80.1               | 131.8                          | 1.18                                | 3.3                | 9.2               |
+| [YOLOv8s-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-pose.pt)       | 640                   | 60.0                  | 86.2               | 233.2                          | 1.42                                | 11.6               | 30.2              |
+| [YOLOv8m-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-pose.pt)       | 640                   | 65.0                  | 88.8               | 456.3                          | 2.00                                | 26.4               | 81.0              |
+| [YOLOv8l-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-pose.pt)       | 640                   | 67.6                  | 90.0               | 784.5                          | 2.59                                | 44.4               | 168.6             |
+| [YOLOv8x-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-pose.pt)       | 640                   | 69.2                  | 90.2               | 1607.1                         | 3.73                                | 69.4               | 263.2             |
+| [YOLOv8x-pose-p6](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-pose-p6.pt) | 1280                  | 71.6                  | 91.2               | 4088.7                         | 10.04                               | 99.1               | 1066.4            |
+
+- **mAP<sup>val</sup>** values are for single-model single-scale on [COCO Keypoints val2017](http://cocodataset.org)
+  dataset.
+  <br>Reproduce by `yolo val pose data=coco-pose.yaml device=0`
+- **Speed** averaged over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) instance.
+  <br>Reproduce by `yolo val pose data=coco8-pose.yaml batch=1 device=0|cpu`
 
 </details>
 
 ## <div align="center">Integrations</div>
 
 <br>
-<a align="center" href="https://bit.ly/ultralytics_hub" target="_blank">
+<a href="https://bit.ly/ultralytics_hub" target="_blank">
 <img width="100%" src="https://github.com/ultralytics/assets/raw/main/yolov8/banner-integrations.png"></a>
 <br>
 <br>
 
 <div align="center">
   <a href="https://roboflow.com/?ref=ultralytics">
-    <img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-roboflow.png" width="10%" /></a>
+    <img src="https://github.com/ultralytics/assets/raw/main/partners/logo-roboflow.png" width="10%" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="15%" height="0" alt="" />
   <a href="https://cutt.ly/yolov5-readme-clearml">
-    <img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-clearml.png" width="10%" /></a>
+    <img src="https://github.com/ultralytics/assets/raw/main/partners/logo-clearml.png" width="10%" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="15%" height="0" alt="" />
-  <a href="https://bit.ly/yolov5-readme-comet">
-    <img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-comet.png" width="10%" /></a>
+  <a href="https://bit.ly/yolov8-readme-comet">
+    <img src="https://github.com/ultralytics/assets/raw/main/partners/logo-comet.png" width="10%" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="15%" height="0" alt="" />
   <a href="https://bit.ly/yolov5-neuralmagic">
-    <img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-neuralmagic.png" width="10%" /></a>
+    <img src="https://github.com/ultralytics/assets/raw/main/partners/logo-neuralmagic.png" width="10%" /></a>
 </div>
 
-|                                                           Roboflow                                                           |                                                            ClearML ⭐ NEW                                                            |                                                                        Comet ⭐ NEW                                                                         |                                           Neural Magic ⭐ NEW                                           |
-| :--------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------: |
-| Label and export your custom datasets directly to YOLOv8 for training with [Roboflow](https://roboflow.com/?ref=ultralytics) | Automatically track, visualize and even remotely train YOLOv8 using [ClearML](https://cutt.ly/yolov5-readme-clearml) (open-source!) | Free forever, [Comet](https://bit.ly/yolov5-readme-comet2) lets you save YOLOv8 models, resume training, and interactively visualize and debug predictions | Run YOLOv8 inference up to 6x faster with [Neural Magic DeepSparse](https://bit.ly/yolov5-neuralmagic) |
+|                                                           Roboflow                                                           |                                                            ClearML ⭐ NEW                                                            |                                                                        Comet ⭐ NEW                                                                        |                                           Neural Magic ⭐ NEW                                           |
+| :--------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------: |
+| Label and export your custom datasets directly to YOLOv8 for training with [Roboflow](https://roboflow.com/?ref=ultralytics) | Automatically track, visualize and even remotely train YOLOv8 using [ClearML](https://cutt.ly/yolov5-readme-clearml) (open-source!) | Free forever, [Comet](https://bit.ly/yolov8-readme-comet) lets you save YOLOv8 models, resume training, and interactively visualize and debug predictions | Run YOLOv8 inference up to 6x faster with [Neural Magic DeepSparse](https://bit.ly/yolov5-neuralmagic) |
 
 ## <div align="center">Ultralytics HUB</div>
 
-[Ultralytics HUB](https://bit.ly/ultralytics_hub) is our ⭐ **NEW** no-code solution to visualize datasets, train YOLOv8
-🚀 models, and deploy to the real world in a seamless experience. Get started for **Free** now! Also run YOLOv8 models on
-your iOS or Android device by downloading the [Ultralytics App](https://ultralytics.com/app_install)!
+Experience seamless AI with [Ultralytics HUB](https://bit.ly/ultralytics_hub) ⭐, the all-in-one solution for data visualization, YOLOv5 and YOLOv8 🚀 model training and deployment, without any coding. Transform images into actionable insights and bring your AI visions to life with ease using our cutting-edge platform and user-friendly [Ultralytics App](https://ultralytics.com/app_install). Start your journey for **Free** now!
 
-<a align="center" href="https://bit.ly/ultralytics_hub" target="_blank">
+<a href="https://bit.ly/ultralytics_hub" target="_blank">
 <img width="100%" src="https://github.com/ultralytics/assets/raw/main/im/ultralytics-hub.png"></a>
 
 ## <div align="center">Contribute</div>
 
-We love your input! YOLOv5 and YOLOv8 would not be possible without help from our community. Please see
-our [Contributing Guide](CONTRIBUTING.md) to get started, and fill out
-our [Survey](https://ultralytics.com/survey?utm_source=github&utm_medium=social&utm_campaign=Survey) to send us feedback
-on your experience. Thank you 🙏 to all our contributors!
+We love your input! YOLOv5 and YOLOv8 would not be possible without help from our community. Please see our [Contributing Guide](https://docs.ultralytics.com/help/contributing) to get started, and fill out our [Survey](https://ultralytics.com/survey?utm_source=github&utm_medium=social&utm_campaign=Survey) to send us feedback on your experience. Thank you 🙏 to all our contributors!
 
 <!-- SVG image from https://opencollective.com/ultralytics/contributors.svg?width=990 -->
 
-<a href="https://github.com/ultralytics/ultralytics/graphs/contributors"><img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/image-contributors-1280.png"/></a>
+<a href="https://github.com/ultralytics/yolov5/graphs/contributors">
+<img width="100%" src="https://github.com/ultralytics/assets/raw/main/im/image-contributors.png"></a>
 
 ## <div align="center">License</div>
 
 YOLOv8 is available under two different licenses:
 
-- **GPL-3.0 License**: See [LICENSE](https://github.com/ultralytics/ultralytics/blob/main/LICENSE) file for details.
-- **Enterprise License**: Provides greater flexibility for commercial product development without the open-source
-  requirements of GPL-3.0. Typical use cases are embedding Ultralytics software and AI models in commercial products and
-  applications. Request an Enterprise License at [Ultralytics Licensing](https://ultralytics.com/license).
+- **AGPL-3.0 License**: See [LICENSE](https://github.com/ultralytics/ultralytics/blob/main/LICENSE) file for details.
+- **Enterprise License**: Provides greater flexibility for commercial product development without the open-source requirements of AGPL-3.0. Typical use cases are embedding Ultralytics software and AI models in commercial products and applications. Request an Enterprise License at [Ultralytics Licensing](https://ultralytics.com/license).
 
 ## <div align="center">Contact</div>
 
-For YOLOv8 bugs and feature requests please visit [GitHub Issues](https://github.com/ultralytics/ultralytics/issues).
-For professional support please [Contact Us](https://ultralytics.com/contact).
+For YOLOv8 bug reports and feature requests please visit [GitHub Issues](https://github.com/ultralytics/ultralytics/issues), and join our [Discord](https://discord.gg/n6cFeSPZdD) community for questions and discussions!
 
 <br>
 <div align="center">
   <a href="https://github.com/ultralytics" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
   <a href="https://www.linkedin.com/company/ultralytics" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
   <a href="https://twitter.com/ultralytics" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
-  <a href="https://www.producthunt.com/@glenn_jocher" style="text-decoration:none;">
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-producthunt.png" width="3%" alt="" /></a>
-  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
   <a href="https://youtube.com/ultralytics" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
-  <a href="https://www.facebook.com/ultralytics" style="text-decoration:none;">
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-facebook.png" width="3%" alt="" /></a>
+  <a href="https://www.tiktok.com/@ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-tiktok.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
   <a href="https://www.instagram.com/ultralytics/" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="3%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
+  <a href="https://discord.gg/n6cFeSPZdD" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/blob/main/social/logo-social-discord.png" width="3%" alt="" /></a>
 </div>
```

#### html2text {}

```diff
@@ -1,80 +1,64 @@
    [https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/banner-
                                   yolov8.png]
             [English](README.md) | [ç®ä½ä¸­æ](README.zh-CN.md)
               [Ultralytics_CI] [YOLOv8_Citation] [Docker_Pulls]
               [Run_on_Gradient] [Open_In_Colab] [Open_In_Kaggle]
 
-[Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics), developed by
- [Ultralytics](https://ultralytics.com), is a cutting-edge, state-of-the-art
-    (SOTA) model that builds upon the success of previous YOLO versions and
-   introduces new features and improvements to further boost performance and
- flexibility. YOLOv8 is designed to be fast, accurate, and easy to use, making
-it an excellent choice for a wide range of object detection, image segmentation
-    and image classification tasks. To request an Enterprise License please
-complete the form at [Ultralytics Licensing](https://ultralytics.com/license).
-    [https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/yolo-
-                             comparison-plots.png]
+[Ultralytics](https://ultralytics.com) [YOLOv8](https://github.com/ultralytics/
+ultralytics) is a cutting-edge, state-of-the-art (SOTA) model that builds upon
+     the success of previous YOLO versions and introduces new features and
+ improvements to further boost performance and flexibility. YOLOv8 is designed
+to be fast, accurate, and easy to use, making it an excellent choice for a wide
+     range of object detection and tracking, instance segmentation, image
+classification and pose estimation tasks. We hope that the resources here will
+help you get the most out of YOLOv8. Please browse the YOLOv8 Docs for details,
+   raise an issue on GitHub for support, and join our Discord community for
+questions and discussions! To request an Enterprise License please complete the
+  form at [Ultralytics Licensing](https://ultralytics.com/license). [https://
+   raw.githubusercontent.com/ultralytics/assets/main/yolov8/yolo-comparison-
+                                  plots.png]
 
 ##
-                           Ultralytics Live Session
-[Ultralytics Live Session 3](https://youtu.be/IPcpYO5ITa8) â¨ is here! Join us
- on January 24th at 18 CET as we dive into the latest advancements in YOLOv8,
-and demonstrate how to use this cutting-edge, SOTA model to improve your object
-   detection, instance segmentation, and image classification projects. See
- firsthand how YOLOv8's speed, accuracy, and ease of use make it a top choice
-  for professionals and researchers alike. In addition to learning about the
-  exciting new features and improvements of Ultralytics YOLOv8, you will also
-  have the opportunity to ask questions and interact with our team during the
-live Q&A session. We encourage you to come prepared with any questions you may
-have. To join the webinar, visit our YouTube [Channel](https://www.youtube.com/
-     @Ultralytics/streams) and turn on your notifications! [https://user-
-   images.githubusercontent.com/107626595/212887899-e94b006c-5192-40fa-8b24-
-                               7b5428e065e8.png]
-##
                                  Documentation
 See below for a quickstart installation and usage example, and see the [YOLOv8
 Docs](https://docs.ultralytics.com) for full documentation on training,
 validation, prediction and deployment.  Install Pip install the ultralytics
-package including all [requirements.txt](https://github.com/ultralytics/
-ultralytics/blob/main/requirements.txt) in a [**3.10>=Python>=3.7**](https://
-www.python.org/) environment, including [**PyTorch>=1.7**](https://pytorch.org/
-get-started/locally/). ```bash pip install ultralytics ```   Usage #### CLI
-YOLOv8 may be used directly in the Command Line Interface (CLI) with a `yolo`
-command: ```bash yolo predict model=yolov8n.pt source="https://ultralytics.com/
-images/bus.jpg" ``` `yolo` can be used for a variety of tasks and modes and
-accepts additional arguments, i.e. `imgsz=640`. See the YOLOv8 [CLI Docs]
-(https://docs.ultralytics.com/cli) for examples. #### Python YOLOv8 may also be
+package including all [requirements](https://github.com/ultralytics/
+ultralytics/blob/main/requirements.txt) in a [**Python>=3.7**](https://
+www.python.org/) environment with [**PyTorch>=1.7**](https://pytorch.org/get-
+started/locally/). ```bash pip install ultralytics ```   Usage #### CLI YOLOv8
+may be used directly in the Command Line Interface (CLI) with a `yolo` command:
+```bash yolo predict model=yolov8n.pt source='https://ultralytics.com/images/
+bus.jpg' ``` `yolo` can be used for a variety of tasks and modes and accepts
+additional arguments, i.e. `imgsz=640`. See the YOLOv8 [CLI Docs](https://
+docs.ultralytics.com/usage/cli) for examples. #### Python YOLOv8 may also be
 used directly in a Python environment, and accepts the same [arguments](https:/
-/docs.ultralytics.com/config/) as in the CLI example above: ```python from
+/docs.ultralytics.com/usage/cfg/) as in the CLI example above: ```python from
 ultralytics import YOLO # Load a model model = YOLO("yolov8n.yaml") # build a
 new model from scratch model = YOLO("yolov8n.pt") # load a pretrained model
-(recommended for training) # Use the model results = model.train
-(data="coco128.yaml", epochs=3) # train the model results = model.val() #
-evaluate model performance on the validation set results = model("https://
-ultralytics.com/images/bus.jpg") # predict on an image success = model.export
-(format="onnx") # export the model to ONNX format ``` [Models](https://
-github.com/ultralytics/ultralytics/tree/main/ultralytics/models) download
-automatically from the latest Ultralytics [release](https://github.com/
-ultralytics/assets/releases). See YOLOv8 [Python Docs](https://
-docs.ultralytics.com/python) for more examples. #### Known Issues / TODOs We
-are still working on several parts of YOLOv8! We aim to have these completed
-soon to bring the YOLOv8 feature set up to par with YOLOv5, including export
-and inference to all the same formats. We are also writing a YOLOv8 paper which
-we will submit to [arxiv.org](https://arxiv.org) once complete. - [ ]
-TensorFlow exports - [ ] DDP resume - [ ] [arxiv.org](https://arxiv.org) paper
-##
+(recommended for training) # Use the model model.train(data="coco128.yaml",
+epochs=3) # train the model metrics = model.val() # evaluate model performance
+on the validation set results = model("https://ultralytics.com/images/bus.jpg")
+# predict on an image success = model.export(format="onnx") # export the model
+to ONNX format ``` [Models](https://github.com/ultralytics/ultralytics/tree/
+main/ultralytics/models) download automatically from the latest Ultralytics
+[release](https://github.com/ultralytics/assets/releases). See YOLOv8 [Python
+Docs](https://docs.ultralytics.com/usage/python) for more examples.  ##
                                     Models
-All YOLOv8 pretrained models are available here. Detection and Segmentation
-models are pretrained on the COCO dataset, while Classification models are
-pretrained on the ImageNet dataset. [Models](https://github.com/ultralytics/
-ultralytics/tree/main/ultralytics/models) download automatically from the
-latest Ultralytics [release](https://github.com/ultralytics/assets/releases) on
-first use. Detection See [Detection Docs](https://docs.ultralytics.com/tasks/
-detection/) for usage examples with these models. | Model | size
+All YOLOv8 pretrained models are available here. Detect, Segment and Pose
+models are pretrained on the [COCO](https://github.com/ultralytics/ultralytics/
+blob/main/ultralytics/datasets/coco.yaml) dataset, while Classify models are
+pretrained on the [ImageNet](https://github.com/ultralytics/ultralytics/blob/
+main/ultralytics/datasets/ImageNet.yaml) dataset. [Models](https://github.com/
+ultralytics/ultralytics/tree/main/ultralytics/models) download automatically
+from the latest Ultralytics [release](https://github.com/ultralytics/assets/
+releases) on first use. Detection See [Detection Docs](https://
+docs.ultralytics.com/tasks/detect/) for usage examples with these models. |
+Model | size
 (pixels) | mAPval
 50-95 | Speed
 CPU ONNX
 (ms) | Speed
 A100 TensorRT
 (ms) | params
 (M) | FLOPs
@@ -91,119 +75,151 @@
 | 165.2 | | [YOLOv8x](https://github.com/ultralytics/assets/releases/download/
 v0.0.0/yolov8x.pt) | 640 | 53.9 | 479.1 | 3.53 | 68.2 | 257.8 | - **mAPval**
 values are for single-model single-scale on [COCO val2017](http://
 cocodataset.org) dataset.
 Reproduce by `yolo val detect data=coco.yaml device=0` - **Speed** averaged
 over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/
 instance-types/p4/) instance.
-Reproduce by `yolo val detect data=coco128.yaml batch=1 device=0/cpu`
+Reproduce by `yolo val detect data=coco128.yaml batch=1 device=0|cpu`
 Segmentation See [Segmentation Docs](https://docs.ultralytics.com/tasks/
-segmentation/) for usage examples with these models. | Model | size
+segment/) for usage examples with these models. | Model | size
 (pixels) | mAPbox
 50-95 | mAPmask
 50-95 | Speed
 CPU ONNX
 (ms) | Speed
 A100 TensorRT
 (ms) | params
 (M) | FLOPs
 (B) | | -----------------------------------------------------------------------
------------------ | --------------------- | -------------------- | ------------
---------- | ------------------------------ | ----------------------------------
-- | ------------------ | ----------------- | | [YOLOv8n](https://github.com/
-ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640 | 36.7 | 30.5
-| 96.1 | 1.21 | 3.4 | 12.6 | | [YOLOv8s](https://github.com/ultralytics/assets/
-releases/download/v0.0.0/yolov8s-seg.pt) | 640 | 44.6 | 36.8 | 155.7 | 1.47 |
-11.8 | 42.6 | | [YOLOv8m](https://github.com/ultralytics/assets/releases/
-download/v0.0.0/yolov8m-seg.pt) | 640 | 49.9 | 40.8 | 317.0 | 2.18 | 27.3 |
-110.2 | | [YOLOv8l](https://github.com/ultralytics/assets/releases/download/
-v0.0.0/yolov8l-seg.pt) | 640 | 52.3 | 42.6 | 572.4 | 2.79 | 46.0 | 220.5 | |
-[YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/
-yolov8x-seg.pt) | 640 | 53.4 | 43.4 | 712.1 | 4.02 | 71.8 | 344.1 | -
-**mAPval** values are for single-model single-scale on [COCO val2017](http://
-cocodataset.org) dataset.
+--------------------- | --------------------- | -------------------- | --------
+------------- | ------------------------------ | ------------------------------
+----- | ------------------ | ----------------- | | [YOLOv8n-seg](https://
+github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640 |
+36.7 | 30.5 | 96.1 | 1.21 | 3.4 | 12.6 | | [YOLOv8s-seg](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8s-seg.pt) | 640 | 44.6 | 36.8
+| 155.7 | 1.47 | 11.8 | 42.6 | | [YOLOv8m-seg](https://github.com/ultralytics/
+assets/releases/download/v0.0.0/yolov8m-seg.pt) | 640 | 49.9 | 40.8 | 317.0 |
+2.18 | 27.3 | 110.2 | | [YOLOv8l-seg](https://github.com/ultralytics/assets/
+releases/download/v0.0.0/yolov8l-seg.pt) | 640 | 52.3 | 42.6 | 572.4 | 2.79 |
+46.0 | 220.5 | | [YOLOv8x-seg](https://github.com/ultralytics/assets/releases/
+download/v0.0.0/yolov8x-seg.pt) | 640 | 53.4 | 43.4 | 712.1 | 4.02 | 71.8 |
+344.1 | - **mAPval** values are for single-model single-scale on [COCO val2017]
+(http://cocodataset.org) dataset.
 Reproduce by `yolo val segment data=coco.yaml device=0` - **Speed** averaged
 over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/
 instance-types/p4/) instance.
-Reproduce by `yolo val segment data=coco128-seg.yaml batch=1 device=0/cpu`
+Reproduce by `yolo val segment data=coco128-seg.yaml batch=1 device=0|cpu`
 Classification See [Classification Docs](https://docs.ultralytics.com/tasks/
-classification/) for usage examples with these models. | Model | size
+classify/) for usage examples with these models. | Model | size
 (pixels) | acc
 top1 | acc
 top5 | Speed
 CPU ONNX
 (ms) | Speed
 A100 TensorRT
 (ms) | params
 (M) | FLOPs
 (B) at 640 | | ----------------------------------------------------------------
------------------------- | --------------------- | ---------------- | ---------
-------- | ------------------------------ | ----------------------------------
-- | ------------------ | ------------------------ | | [YOLOv8n](https://
+---------------------------- | --------------------- | ---------------- | -----
+----------- | ------------------------------ | --------------------------------
+--- | ------------------ | ------------------------ | | [YOLOv8n-cls](https://
 github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-cls.pt) | 224 |
-66.6 | 87.0 | 12.9 | 0.31 | 2.7 | 4.3 | | [YOLOv8s](https://github.com/
+66.6 | 87.0 | 12.9 | 0.31 | 2.7 | 4.3 | | [YOLOv8s-cls](https://github.com/
 ultralytics/assets/releases/download/v0.0.0/yolov8s-cls.pt) | 224 | 72.3 | 91.1
-| 23.4 | 0.35 | 6.4 | 13.5 | | [YOLOv8m](https://github.com/ultralytics/assets/
-releases/download/v0.0.0/yolov8m-cls.pt) | 224 | 76.4 | 93.2 | 85.4 | 0.62 |
-17.0 | 42.7 | | [YOLOv8l](https://github.com/ultralytics/assets/releases/
-download/v0.0.0/yolov8l-cls.pt) | 224 | 78.0 | 94.1 | 163.0 | 0.87 | 37.5 |
-99.7 | | [YOLOv8x](https://github.com/ultralytics/assets/releases/download/
-v0.0.0/yolov8x-cls.pt) | 224 | 78.4 | 94.3 | 232.0 | 1.01 | 57.4 | 154.8 | -
-**acc** values are model accuracies on the [ImageNet](https://www.image-
-net.org/) dataset validation set.
+| 23.4 | 0.35 | 6.4 | 13.5 | | [YOLOv8m-cls](https://github.com/ultralytics/
+assets/releases/download/v0.0.0/yolov8m-cls.pt) | 224 | 76.4 | 93.2 | 85.4 |
+0.62 | 17.0 | 42.7 | | [YOLOv8l-cls](https://github.com/ultralytics/assets/
+releases/download/v0.0.0/yolov8l-cls.pt) | 224 | 78.0 | 94.1 | 163.0 | 0.87 |
+37.5 | 99.7 | | [YOLOv8x-cls](https://github.com/ultralytics/assets/releases/
+download/v0.0.0/yolov8x-cls.pt) | 224 | 78.4 | 94.3 | 232.0 | 1.01 | 57.4 |
+154.8 | - **acc** values are model accuracies on the [ImageNet](https://
+www.image-net.org/) dataset validation set.
 Reproduce by `yolo val classify data=path/to/ImageNet device=0` - **Speed**
 averaged over ImageNet val images using an [Amazon EC2 P4d](https://
 aws.amazon.com/ec2/instance-types/p4/) instance.
-Reproduce by `yolo val classify data=path/to/ImageNet batch=1 device=0/cpu`  ##
+Reproduce by `yolo val classify data=path/to/ImageNet batch=1 device=0|cpu`
+Pose See [Pose Docs](https://docs.ultralytics.com/tasks/pose) for usage
+examples with these models. | Model | size
+(pixels) | mAPpose
+50-95 | mAPpose
+50 | Speed
+CPU ONNX
+(ms) | Speed
+A100 TensorRT
+(ms) | params
+(M) | FLOPs
+(B) | | -----------------------------------------------------------------------
+----------------------------- | --------------------- | --------------------- |
+------------------ | ------------------------------ | -------------------------
+---------- | ------------------ | ----------------- | | [YOLOv8n-pose](https://
+github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-pose.pt) | 640 |
+50.4 | 80.1 | 131.8 | 1.18 | 3.3 | 9.2 | | [YOLOv8s-pose](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8s-pose.pt) | 640 | 60.0 |
+86.2 | 233.2 | 1.42 | 11.6 | 30.2 | | [YOLOv8m-pose](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8m-pose.pt) | 640 | 65.0 |
+88.8 | 456.3 | 2.00 | 26.4 | 81.0 | | [YOLOv8l-pose](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8l-pose.pt) | 640 | 67.6 |
+90.0 | 784.5 | 2.59 | 44.4 | 168.6 | | [YOLOv8x-pose](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8x-pose.pt) | 640 | 69.2 |
+90.2 | 1607.1 | 3.73 | 69.4 | 263.2 | | [YOLOv8x-pose-p6](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8x-pose-p6.pt) | 1280 | 71.6 |
+91.2 | 4088.7 | 10.04 | 99.1 | 1066.4 | - **mAPval** values are for single-
+model single-scale on [COCO Keypoints val2017](http://cocodataset.org) dataset.
+
+Reproduce by `yolo val pose data=coco-pose.yaml device=0` - **Speed** averaged
+over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/
+instance-types/p4/) instance.
+Reproduce by `yolo val pose data=coco8-pose.yaml batch=1 device=0|cpu`  ##
                                  Integrations
 
 [https://github.com/ultralytics/assets/raw/main/yolov8/banner-integrations.png]
 
 
-      [https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-
- roboflow.png]  [https://github.com/ultralytics/yolov5/releases/download/v1.0/
- logo-clearml.png]  [https://github.com/ultralytics/yolov5/releases/download/
-v1.0/logo-comet.png]  [https://github.com/ultralytics/yolov5/releases/download/
-                          v1.0/logo-neuralmagic.png]
+ [https://github.com/ultralytics/assets/raw/main/partners/logo-roboflow.png]
+ [https://github.com/ultralytics/assets/raw/main/partners/logo-clearml.png]
+  [https://github.com/ultralytics/assets/raw/main/partners/logo-comet.png]
+[https://github.com/ultralytics/assets/raw/main/partners/logo-neuralmagic.png]
 | Roboflow | ClearML â­ NEW | Comet â­ NEW | Neural Magic â­ NEW | | :------
 -------------------------------------------------------------------------------
 -------------------------------------: | :-------------------------------------
 -------------------------------------------------------------------------------
 -------------: | :-------------------------------------------------------------
 -------------------------------------------------------------------------------
-------------: | :--------------------------------------------------------------
---------------------------------------: | | Label and export your custom
+-----------: | :---------------------------------------------------------------
+-------------------------------------: | | Label and export your custom
 datasets directly to YOLOv8 for training with [Roboflow](https://roboflow.com/
 ?ref=ultralytics) | Automatically track, visualize and even remotely train
 YOLOv8 using [ClearML](https://cutt.ly/yolov5-readme-clearml) (open-source!) |
-Free forever, [Comet](https://bit.ly/yolov5-readme-comet2) lets you save YOLOv8
+Free forever, [Comet](https://bit.ly/yolov8-readme-comet) lets you save YOLOv8
 models, resume training, and interactively visualize and debug predictions |
 Run YOLOv8 inference up to 6x faster with [Neural Magic DeepSparse](https://
 bit.ly/yolov5-neuralmagic) | ##
                                 Ultralytics HUB
-[Ultralytics HUB](https://bit.ly/ultralytics_hub) is our â­ **NEW** no-code
-solution to visualize datasets, train YOLOv8 ð models, and deploy to the
-real world in a seamless experience. Get started for **Free** now! Also run
-YOLOv8 models on your iOS or Android device by downloading the [Ultralytics
-App](https://ultralytics.com/app_install)! [https://github.com/ultralytics/
-assets/raw/main/im/ultralytics-hub.png] ##
+Experience seamless AI with [Ultralytics HUB](https://bit.ly/ultralytics_hub)
+â­, the all-in-one solution for data visualization, YOLOv5 and YOLOv8 ð
+model training and deployment, without any coding. Transform images into
+actionable insights and bring your AI visions to life with ease using our
+cutting-edge platform and user-friendly [Ultralytics App](https://
+ultralytics.com/app_install). Start your journey for **Free** now! [https://
+github.com/ultralytics/assets/raw/main/im/ultralytics-hub.png] ##
                                   Contribute
 We love your input! YOLOv5 and YOLOv8 would not be possible without help from
-our community. Please see our [Contributing Guide](CONTRIBUTING.md) to get
-started, and fill out our [Survey](https://ultralytics.com/
+our community. Please see our [Contributing Guide](https://
+docs.ultralytics.com/help/contributing) to get started, and fill out our
+[Survey](https://ultralytics.com/
 survey?utm_source=github&utm_medium=social&utm_campaign=Survey) to send us
 feedback on your experience. Thank you ð to all our contributors!  [https://
-github.com/ultralytics/yolov5/releases/download/v1.0/image-contributors-
-1280.png] ##
+github.com/ultralytics/assets/raw/main/im/image-contributors.png] ##
                                     License
-YOLOv8 is available under two different licenses: - **GPL-3.0 License**: See
+YOLOv8 is available under two different licenses: - **AGPL-3.0 License**: See
 [LICENSE](https://github.com/ultralytics/ultralytics/blob/main/LICENSE) file
 for details. - **Enterprise License**: Provides greater flexibility for
-commercial product development without the open-source requirements of GPL-3.0.
-Typical use cases are embedding Ultralytics software and AI models in
+commercial product development without the open-source requirements of AGPL-
+3.0. Typical use cases are embedding Ultralytics software and AI models in
 commercial products and applications. Request an Enterprise License at
 [Ultralytics Licensing](https://ultralytics.com/license). ##
                                     Contact
-For YOLOv8 bugs and feature requests please visit [GitHub Issues](https://
-github.com/ultralytics/ultralytics/issues). For professional support please
-[Contact Us](https://ultralytics.com/contact).
+For YOLOv8 bug reports and feature requests please visit [GitHub Issues](https:
+//github.com/ultralytics/ultralytics/issues), and join our [Discord](https://
+discord.gg/n6cFeSPZdD) community for questions and discussions!
```

### Comparing `ultralytics-8.0.9/README.zh-CN.md` & `ultralytics-8.0.90/README.zh-CN.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,240 +1,260 @@
 <div align="center">
   <p>
-    <a align="center" href="https://ultralytics.com/yolov8" target="_blank">
-      <img width="850" src="https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/banner-yolov8.png"></a>
+    <a href="https://ultralytics.com/yolov8" target="_blank">
+      <img width="100%" src="https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/banner-yolov8.png"></a>
   </p>
 
 [English](README.md) | [简体中文](README.zh-CN.md)
 <br>
 
 <div>
     <a href="https://github.com/ultralytics/ultralytics/actions/workflows/ci.yaml"><img src="https://github.com/ultralytics/ultralytics/actions/workflows/ci.yaml/badge.svg" alt="Ultralytics CI"></a>
     <a href="https://zenodo.org/badge/latestdoi/264818686"><img src="https://zenodo.org/badge/264818686.svg" alt="YOLOv8 Citation"></a>
-    <a href="https://hub.docker.com/r/ultralytics/yolov5"><img src="https://img.shields.io/docker/pulls/ultralytics/yolov5?logo=docker" alt="Docker Pulls"></a>
+    <a href="https://hub.docker.com/r/ultralytics/ultralytics"><img src="https://img.shields.io/docker/pulls/ultralytics/ultralytics?logo=docker" alt="Docker Pulls"></a>
     <br>
     <a href="https://console.paperspace.com/github/ultralytics/ultralytics"><img src="https://assets.paperspace.io/img/gradient-badge.svg" alt="Run on Gradient"/></a>
     <a href="https://colab.research.google.com/github/ultralytics/ultralytics/blob/main/examples/tutorial.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>
     <a href="https://www.kaggle.com/ultralytics/yolov8"><img src="https://kaggle.com/static/images/open-in-kaggle.svg" alt="Open In Kaggle"></a>
   </div>
   <br>
 
-[Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics) 是由 [Ultralytics](https://ultralytics.com) 开发的一个前沿的 SOTA 模型。它在以前成功的 YOLO 版本基础上，引入了新的功能和改进，进一步提升了其性能和灵活性。YOLOv8 基于快速、准确和易于使用的设计理念，使其成为广泛的目标检测、图像分割和图像分类任务的绝佳选择。
+[Ultralytics](https://ultralytics.com) [YOLOv8](https://github.com/ultralytics/ultralytics) 是一款前沿、最先进（SOTA）的模型，基于先前 YOLO 版本的成功，引入了新功能和改进，进一步提升性能和灵活性。YOLOv8 设计快速、准确且易于使用，使其成为各种物体检测与跟踪、实例分割、图像分类和姿态估计任务的绝佳选择。
 
-如果要申请企业许可证，请填写 [Ultralytics 许可](https://ultralytics.com/license)。
+我们希望这里的资源能帮助您充分利用 YOLOv8。请浏览 YOLOv8 <a href="https://docs.ultralytics.com/">文档</a> 了解详细信息，在 <a href="https://github.com/ultralytics/ultralytics/issues/new/choose">GitHub</a> 上提交问题以获得支持，并加入我们的 <a href="https://discord.gg/n6cFeSPZdD">Discord</a> 社区进行问题和讨论！
+
+如需申请企业许可，请在 [Ultralytics Licensing](https://ultralytics.com/license) 处填写表格
+
+<img width="100%" src="https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/yolo-comparison-plots.png"></a>
 
 <div align="center">
-    <a href="https://github.com/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://www.linkedin.com/company/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://twitter.com/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://www.producthunt.com/@glenn_jocher" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-producthunt.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://youtube.com/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://www.facebook.com/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-facebook.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://www.instagram.com/ultralytics/" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="2%" alt="" /></a>
-  </div>
+  <a href="https://github.com/ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://www.linkedin.com/company/ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://twitter.com/ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://youtube.com/ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://www.tiktok.com/@ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-tiktok.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://www.instagram.com/ultralytics/" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://discord.gg/n6cFeSPZdD" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/blob/main/social/logo-social-discord.png" width="2%" alt="" /></a>
+</div>
 </div>
 
 ## <div align="center">文档</div>
 
-有关训练、测试和部署的完整文档见[YOLOv8 Docs](https://docs.ultralytics.com)。请参阅下面的快速入门示例。
+请参阅下面的快速安装和使用示例，以及 [YOLOv8 文档](https://docs.ultralytics.com) 上有关培训、验证、预测和部署的完整文档。
 
 <details open>
 <summary>安装</summary>
 
-Pip 安装包含所有 [requirements.txt](https://github.com/ultralytics/ultralytics/blob/main/requirements.txt) 的 ultralytics 包，环境要求 [**3.10>=Python>=3.7**](https://www.python.org/)，且 [**PyTorch>=1.7**](https://pytorch.org/get-started/locally/)。
+在一个 [**Python>=3.7**](https://www.python.org/) 环境中，使用 [**PyTorch>=1.7**](https://pytorch.org/get-started/locally/)，通过 pip 安装 ultralytics 软件包以及所有[依赖项](https://github.com/ultralytics/ultralytics/blob/main/requirements.txt)。
 
 ```bash
 pip install ultralytics
 ```
 
 </details>
 
 <details open>
-<summary>使用方法</summary>
+<summary>Usage</summary>
 
-YOLOv8 可以直接在命令行界面（CLI）中使用 `yolo` 命令运行：
+#### CLI
+
+YOLOv8 可以在命令行界面（CLI）中直接使用，只需输入 `yolo` 命令：
 
 ```bash
-yolo predict model=yolov8n.pt source="https://ultralytics.com/images/bus.jpg"
+yolo predict model=yolov8n.pt source='https://ultralytics.com/images/bus.jpg'
 ```
 
-`yolo`可以用于各种任务和模式，并接受额外的参数，例如 `imgsz=640`。参见 YOLOv8 [文档](https://docs.ultralytics.com)中可用`yolo`[参数](https://docs.ultralytics.com/config/)的完整列表。
+`yolo` 可用于各种任务和模式，并接受其他参数，例如 `imgsz=640`。查看 YOLOv8 [CLI 文档](https://docs.ultralytics.com/usage/cli)以获取示例。
 
-```bash
-yolo task=detect    mode=train    model=yolov8n.pt        args...
-          classify       predict        yolov8n-cls.yaml  args...
-          segment        val            yolov8n-seg.yaml  args...
-                         export         yolov8n.pt        format=onnx  args...
-```
+#### Python
 
-YOLOv8 也可以在 Python 环境中直接使用，并接受与上面 CLI 例子中相同的[参数](https://docs.ultralytics.com/config/)：
+YOLOv8 也可以在 Python 环境中直接使用，并接受与上述 CLI 示例中相同的[参数](https://docs.ultralytics.com/usage/cfg/)：
 
 ```python
 from ultralytics import YOLO
 
 # 加载模型
 model = YOLO("yolov8n.yaml")  # 从头开始构建新模型
-model = YOLO("yolov8n.pt")  # 加载预训练模型（推荐用于训练）
+model = YOLO("yolov8n.pt")  # 加载预训练模型（建议用于训练）
 
-# Use the model
-results = model.train(data="coco128.yaml", epochs=3)  # 训练模型
-results = model.val()  # 在验证集上评估模型性能
-results = model("https://ultralytics.com/images/bus.jpg")  # 预测图像
+# 使用模型
+model.train(data="coco128.yaml", epochs=3)  # 训练模型
+metrics = model.val()  # 在验证集上评估模型性能
+results = model("https://ultralytics.com/images/bus.jpg")  # 对图像进行预测
 success = model.export(format="onnx")  # 将模型导出为 ONNX 格式
 ```
 
-[模型](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) 会从 Ultralytics [发布页](https://github.com/ultralytics/ultralytics/releases) 自动下载。
-
-### 已知问题 / 待办事项
-
-我们仍在努力完善 YOLOv8 的几个部分！我们的目标是尽快完成这些工作，使 YOLOv8 的功能设置达到YOLOv5 的水平，包括对所有相同格式的导出和推理。我们还在写一篇 YOLOv8 的论文，一旦完成，我们将提交给 [arxiv.org](https://arxiv.org)。
-
-- [ ] TensorFlow 导出
-- [ ] DDP 恢复训练
-- [ ] [arxiv.org](https://arxiv.org) 论文
+[模型](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) 会自动从最新的 Ultralytics [发布版本](https://github.com/ultralytics/assets/releases)中下载。查看 YOLOv8 [Python 文档](https://docs.ultralytics.com/usage/python)以获取更多示例。
 
 </details>
 
 ## <div align="center">模型</div>
 
-所有 YOLOv8 的预训练模型都可以在这里找到。目标检测和分割模型是在 COCO 数据集上预训练的，而分类模型是在 ImageNet 数据集上预训练的。
+所有的 YOLOv8 预训练模型都可以在此找到。检测、分割和姿态模型在 [COCO](https://github.com/ultralytics/ultralytics/blob/main/ultralytics/datasets/coco.yaml) 数据集上进行预训练，而分类模型在 [ImageNet](https://github.com/ultralytics/ultralytics/blob/main/ultralytics/datasets/ImageNet.yaml) 数据集上进行预训练。
 
-第一次使用时，[模型](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) 会从 Ultralytics [发布页](https://github.com/ultralytics/ultralytics/releases) 自动下载。
+在首次使用时，[模型](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) 会自动从最新的 Ultralytics [发布版本](https://github.com/ultralytics/assets/releases)中下载。
 
-<details open><summary>目标检测</summary>
+<details open><summary>检测</summary>
 
-| 模型                                                                                   | 尺寸<br><sup>（像素） | mAP<sup>val<br>50-95 | 推理速度<br><sup>CPU ONNX<br>(ms) | 推理速度<br><sup>A100 TensorRT<br>(ms) | 参数量<br><sup>(M) | FLOPs<br><sup>(B) |
-| ------------------------------------------------------------------------------------ | --------------- | -------------------- | ----------------------------- | ---------------------------------- | --------------- | ----------------- |
-| [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n.pt) | 640             | 37.3                 | 80.4                          | 0.99                               | 3.2             | 8.7               |
-| [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s.pt) | 640             | 44.9                 | 128.4                         | 1.20                               | 11.2            | 28.6              |
-| [YOLOv8m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m.pt) | 640             | 50.2                 | 234.7                         | 1.83                               | 25.9            | 78.9              |
-| [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l.pt) | 640             | 52.9                 | 375.2                         | 2.39                               | 43.7            | 165.2             |
-| [YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x.pt) | 640             | 53.9                 | 479.1                         | 3.53                               | 68.2            | 257.8             |
+查看 [检测文档](https://docs.ultralytics.com/tasks/detect/) 以获取使用这些模型的示例。
 
-- **mAP<sup>val</sup>** 结果都在 [COCO val2017](http://cocodataset.org) 数据集上，使用单模型单尺度测试得到。
-  <br>复现命令 `yolo val detect data=coco.yaml device=0`
-- **推理速度**使用 COCO 验证集图片推理时间进行平均得到，测试环境使用 [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) 实例。
-  <br>复现命令 `yolo val detect data=coco128.yaml batch=1 device=0/cpu`
+| 模型                                                                                   | 尺寸<br><sup>(像素) | mAP<sup>val<br>50-95 | 速度<br><sup>CPU ONNX<br>(ms) | 速度<br><sup>A100 TensorRT<br>(ms) | 参数<br><sup>(M) | FLOPs<br><sup>(B) |
+| ------------------------------------------------------------------------------------ | --------------- | -------------------- | --------------------------- | -------------------------------- | -------------- | ----------------- |
+| [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n.pt) | 640             | 37.3                 | 80.4                        | 0.99                             | 3.2            | 8.7               |
+| [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s.pt) | 640             | 44.9                 | 128.4                       | 1.20                             | 11.2           | 28.6              |
+| [YOLOv8m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m.pt) | 640             | 50.2                 | 234.7                       | 1.83                             | 25.9           | 78.9              |
+| [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l.pt) | 640             | 52.9                 | 375.2                       | 2.39                             | 43.7           | 165.2             |
+| [YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x.pt) | 640             | 53.9                 | 479.1                       | 3.53                             | 68.2           | 257.8             |
+
+- **mAP<sup>val</sup>** 值是基于单模型单尺度在 [COCO val2017](http://cocodataset.org) 数据集上的结果。
+  <br>通过 `yolo val detect data=coco.yaml device=0` 复现
+- **速度** 是使用 [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) 实例对 COCO val 图像进行平均计算的。
+  <br>通过 `yolo val detect data=coco128.yaml batch=1 device=0|cpu` 复现
 
 </details>
 
-<details><summary>实例分割</summary>
+<details><summary>分割</summary>
 
-| 模型                                                                                       | 尺寸<br><sup>（像素） | mAP<sup>box<br>50-95 | mAP<sup>mask<br>50-95 | 推理速度<br><sup>CPU ONNX<br>(ms) | 推理速度<br><sup>A100 TensorRT<br>(ms) | 参数量<br><sup>(M) | FLOPs<br><sup>(B) |
-| ---------------------------------------------------------------------------------------- | --------------- | -------------------- | --------------------- | ----------------------------- | ---------------------------------- | --------------- | ----------------- |
-| [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640             | 36.7                 | 30.5                  | 96.1                          | 1.21                               | 3.4             | 12.6              |
-| [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-seg.pt) | 640             | 44.6                 | 36.8                  | 155.7                         | 1.47                               | 11.8            | 42.6              |
-| [YOLOv8m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-seg.pt) | 640             | 49.9                 | 40.8                  | 317.0                         | 2.18                               | 27.3            | 110.2             |
-| [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-seg.pt) | 640             | 52.3                 | 42.6                  | 572.4                         | 2.79                               | 46.0            | 220.5             |
-| [YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-seg.pt) | 640             | 53.4                 | 43.4                  | 712.1                         | 4.02                               | 71.8            | 344.1             |
+查看 [分割文档](https://docs.ultralytics.com/tasks/segment/) 以获取使用这些模型的示例。
 
-- **mAP<sup>val</sup>**  结果都在 [COCO val2017](http://cocodataset.org) 数据集上，使用单模型单尺度测试得到。
-  <br>复现命令 `yolo val segment data=coco.yaml device=0`
-- **推理速度**使用 COCO 验证集图片推理时间进行平均得到，测试环境使用 [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) 实例。
-  <br>复现命令 `yolo val segment data=coco128-seg.yaml batch=1 device=0/cpu`
+| 模型                                                                                           | 尺寸<br><sup>(像素) | mAP<sup>box<br>50-95 | mAP<sup>mask<br>50-95 | 速度<br><sup>CPU ONNX<br>(ms) | 速度<br><sup>A100 TensorRT<br>(ms) | 参数<br><sup>(M) | FLOPs<br><sup>(B) |
+| -------------------------------------------------------------------------------------------- | --------------- | -------------------- | --------------------- | --------------------------- | -------------------------------- | -------------- | ----------------- |
+| [YOLOv8n-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640             | 36.7                 | 30.5                  | 96.1                        | 1.21                             | 3.4            | 12.6              |
+| [YOLOv8s-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-seg.pt) | 640             | 44.6                 | 36.8                  | 155.7                       | 1.47                             | 11.8           | 42.6              |
+| [YOLOv8m-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-seg.pt) | 640             | 49.9                 | 40.8                  | 317.0                       | 2.18                             | 27.3           | 110.2             |
+| [YOLOv8l-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-seg.pt) | 640             | 52.3                 | 42.6                  | 572.4                       | 2.79                             | 46.0           | 220.5             |
+| [YOLOv8x-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-seg.pt) | 640             | 53.4                 | 43.4                  | 712.1                       | 4.02                             | 71.8           | 344.1             |
+
+- **mAP<sup>val</sup>** 值是基于单模型单尺度在 [COCO val2017](http://cocodataset.org) 数据集上的结果。
+  <br>通过 `yolo val segment data=coco.yaml device=0` 复现
+- **速度** 是使用 [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) 实例对 COCO val 图像进行平均计算的。
+  <br>通过 `yolo val segment data=coco128-seg.yaml batch=1 device=0|cpu` 复现
 
 </details>
 
 <details><summary>分类</summary>
 
-| 模型                                                                                       | 尺寸<br><sup>（像素） | acc<br><sup>top1 | acc<br><sup>top5 | 推理速度<br><sup>CPU ONNX<br>(ms) | 推理速度<br><sup>A100 TensorRT<br>(ms) | 参数量<br><sup>(M) | FLOPs<br><sup>(B) at 640 |
-| ---------------------------------------------------------------------------------------- | --------------- | ---------------- | ---------------- | ----------------------------- | ---------------------------------- | --------------- | ------------------------ |
-| [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-cls.pt) | 224             | 66.6             | 87.0             | 12.9                          | 0.31                               | 2.7             | 4.3                      |
-| [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-cls.pt) | 224             | 72.3             | 91.1             | 23.4                          | 0.35                               | 6.4             | 13.5                     |
-| [YOLOv8m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-cls.pt) | 224             | 76.4             | 93.2             | 85.4                          | 0.62                               | 17.0            | 42.7                     |
-| [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-cls.pt) | 224             | 78.0             | 94.1             | 163.0                         | 0.87                               | 37.5            | 99.7                     |
-| [YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-cls.pt) | 224             | 78.4             | 94.3             | 232.0                         | 1.01                               | 57.4            | 154.8                    |
-
-- **acc** 都在 [ImageNet](https://www.image-net.org/) 数据集上，使用单模型单尺度测试得到。
-  <br>复现命令 `yolo val classify data=path/to/ImageNet device=0`
-- **推理速度**使用 ImageNet 验证集图片推理时间进行平均得到，测试环境使用 [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) 实例。
-  <br>复现命令 `yolo val classify data=path/to/ImageNet batch=1 device=0/cpu`
+查看 [分类文档](https://docs.ultralytics.com/tasks/classify/) 以获取使用这些模型的示例。
+
+| 模型                                                                                           | 尺寸<br><sup>(像素) | acc<br><sup>top1 | acc<br><sup>top5 | 速度<br><sup>CPU ONNX<br>(ms) | 速度<br><sup>A100 TensorRT<br>(ms) | 参数<br><sup>(M) | FLOPs<br><sup>(B) at 640 |
+| -------------------------------------------------------------------------------------------- | --------------- | ---------------- | ---------------- | --------------------------- | -------------------------------- | -------------- | ------------------------ |
+| [YOLOv8n-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-cls.pt) | 224             | 66.6             | 87.0             | 12.9                        | 0.31                             | 2.7            | 4.3                      |
+| [YOLOv8s-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-cls.pt) | 224             | 72.3             | 91.1             | 23.4                        | 0.35                             | 6.4            | 13.5                     |
+| [YOLOv8m-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-cls.pt) | 224             | 76.4             | 93.2             | 85.4                        | 0.62                             | 17.0           | 42.7                     |
+| [YOLOv8l-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-cls.pt) | 224             | 78.0             | 94.1             | 163.0                       | 0.87                             | 37.5           | 99.7                     |
+| [YOLOv8x-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-cls.pt) | 224             | 78.4             | 94.3             | 232.0                       | 1.01                             | 57.4           | 154.8                    |
+
+- **acc** 值是模型在 [ImageNet](https://www.image-net.org/) 数据集验证集上的准确率。
+  <br>通过 `yolo val classify data=path/to/ImageNet device=0` 复现
+- **速度** 是使用 [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) 实例对 ImageNet val 图像进行平均计算的。
+  <br>通过 `yolo val classify data=path/to/ImageNet batch=1 device=0|cpu` 复现
 
 </details>
 
-## <div align="center">模块集成</div>
+<details><summary>姿态</summary>
+
+查看 [姿态文档](https://docs.ultralytics.com/tasks/) 以获取使用这些模型的示例。
+
+| 模型                                                                                                   | 尺寸<br><sup>(像素) | mAP<sup>pose<br>50-95 | mAP<sup>pose<br>50 | 速度<br><sup>CPU ONNX<br>(ms) | 速度<br><sup>A100 TensorRT<br>(ms) | 参数<br><sup>(M) | FLOPs<br><sup>(B) |
+| ---------------------------------------------------------------------------------------------------- | --------------- | --------------------- | ------------------ | --------------------------- | -------------------------------- | -------------- | ----------------- |
+| [YOLOv8n-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-pose.pt)       | 640             | 50.4                  | 80.1               | 131.8                       | 1.18                             | 3.3            | 9.2               |
+| [YOLOv8s-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-pose.pt)       | 640             | 60.0                  | 86.2               | 233.2                       | 1.42                             | 11.6           | 30.2              |
+| [YOLOv8m-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-pose.pt)       | 640             | 65.0                  | 88.8               | 456.3                       | 2.00                             | 26.4           | 81.0              |
+| [YOLOv8l-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-pose.pt)       | 640             | 67.6                  | 90.0               | 784.5                       | 2.59                             | 44.4           | 168.6             |
+| [YOLOv8x-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-pose.pt)       | 640             | 69.2                  | 90.2               | 1607.1                      | 3.73                             | 69.4           | 263.2             |
+| [YOLOv8x-pose-p6](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-pose-p6.pt) | 1280            | 71.6                  | 91.2               | 4088.7                      | 10.04                            | 99.1           | 1066.4            |
+
+- **mAP<sup>val</sup>** 值是基于单模型单尺度在 [COCO Keypoints val2017](http://cocodataset.org) 数据集上的结果。
+  <br>通过 `yolo val pose data=coco-pose.yaml device=0` 复现
+- **速度** 是使用 [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) 实例对 COCO val 图像进行平均计算的。
+  <br>通过 `yolo val pose data=coco8-pose.yaml batch=1 device=0|cpu` 复现
+
+</details>
+
+## <div align="center">集成</div>
 
 <br>
-<a align="center" href="https://bit.ly/ultralytics_hub" target="_blank">
+<a href="https://bit.ly/ultralytics_hub" target="_blank">
 <img width="100%" src="https://github.com/ultralytics/assets/raw/main/yolov8/banner-integrations.png"></a>
 <br>
 <br>
 
 <div align="center">
   <a href="https://roboflow.com/?ref=ultralytics">
-    <img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-roboflow.png" width="10%" /></a>
+    <img src="https://github.com/ultralytics/assets/raw/main/partners/logo-roboflow.png" width="10%" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="15%" height="0" alt="" />
   <a href="https://cutt.ly/yolov5-readme-clearml">
-    <img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-clearml.png" width="10%" /></a>
+    <img src="https://github.com/ultralytics/assets/raw/main/partners/logo-clearml.png" width="10%" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="15%" height="0" alt="" />
-  <a href="https://bit.ly/yolov5-readme-comet">
-    <img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-comet.png" width="10%" /></a>
+  <a href="https://bit.ly/yolov8-readme-comet">
+    <img src="https://github.com/ultralytics/assets/raw/main/partners/logo-comet.png" width="10%" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="15%" height="0" alt="" />
   <a href="https://bit.ly/yolov5-neuralmagic">
-    <img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-neuralmagic.png" width="10%" /></a>
+    <img src="https://github.com/ultralytics/assets/raw/main/partners/logo-neuralmagic.png" width="10%" /></a>
 </div>
 
-|                                      Roboflow                                      |                                 ClearML ⭐ 新                                 |                                     Comet ⭐ 新                                     |                                    Neural Magic ⭐ 新                                    |
-| :--------------------------------------------------------------------------------: | :-------------------------------------------------------------------------: | :-------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------: |
-| 将您的自定义数据集进行标注并直接导出到 YOLOv8 以进行训练 [Roboflow](https://roboflow.com/?ref=ultralytics) | 自动跟踪、可视化甚至远程训练 YOLOv8 [ClearML](https://cutt.ly/yolov5-readme-clearml)（开源！） | 永远免费，[Comet](https://bit.ly/yolov5-readme-comet)可让您保存 YOLOv8 模型、恢复训练以及交互式可视化和调试预测 | 使用 [Neural Magic DeepSparse](https://bit.ly/yolov5-neuralmagic)，运行 YOLOv8 推理的速度最高可提高6倍 |
+|                                      Roboflow                                      |                                 ClearML ⭐ NEW                                  |                                     Comet ⭐ NEW                                      |                                  Neural Magic ⭐ NEW                                   |
+| :--------------------------------------------------------------------------------: | :----------------------------------------------------------------------------: | :----------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------: |
+| 使用 [Roboflow](https://roboflow.com/?ref=ultralytics) 将您的自定义数据集直接标记并导出至 YOLOv8 进行训练 | 使用 [ClearML](https://cutt.ly/yolov5-readme-clearml)（开源！）自动跟踪、可视化，甚至远程训练 YOLOv8 | 免费且永久，[Comet](https://bit.ly/yolov8-readme-comet) 让您保存 YOLOv8 模型、恢复训练，并以交互式方式查看和调试预测 | 使用 [Neural Magic DeepSparse](https://bit.ly/yolov5-neuralmagic) 使 YOLOv8 推理速度提高多达 6 倍 |
 
 ## <div align="center">Ultralytics HUB</div>
 
-[Ultralytics HUB](https://bit.ly/ultralytics_hub) 是我们⭐ **新**的无代码解决方案，用于可视化数据集，训练 YOLOv8🚀 模型，并以无缝体验方式部署到现实世界。现在开始**免费**! 还可以通过下载 [Ultralytics App](https://ultralytics.com/app_install) 在你的 iOS 或 Android 设备上运行 YOLOv8 模型!
+体验 [Ultralytics HUB](https://bit.ly/ultralytics_hub) ⭐ 带来的无缝 AI，这是一个一体化解决方案，用于数据可视化、YOLOv5 和即将推出的 YOLOv8 🚀 模型训练和部署，无需任何编码。通过我们先进的平台和用户友好的 [Ultralytics 应用程序](https://ultralytics.com/app_install)，轻松将图像转化为可操作的见解，并实现您的 AI 愿景。现在就开始您的**免费**之旅！
 
-<a align="center" href="https://bit.ly/ultralytics_hub" target="_blank">
+<a href="https://bit.ly/ultralytics_hub" target="_blank">
 <img width="100%" src="https://github.com/ultralytics/assets/raw/main/im/ultralytics-hub.png"></a>
 
 ## <div align="center">贡献</div>
 
-我们喜欢您的意见或建议！我们希望尽可能简单和透明地为 YOLOv8 做出贡献。请看我们的 [贡献指南](CONTRIBUTING.md) ，并填写 [调查问卷](https://ultralytics.com/survey?utm_source=github&utm_medium=social&utm_campaign=Survey) 向我们发送您的体验反馈。感谢我们所有的贡献者！
+我们喜欢您的参与！没有社区的帮助，YOLOv5 和 YOLOv8 将无法实现。请参阅我们的[贡献指南](https://docs.ultralytics.com/help/contributing)以开始使用，并填写我们的[调查问卷](https://ultralytics.com/survey?utm_source=github&utm_medium=social&utm_campaign=Survey)向我们提供您的使用体验反馈。感谢所有贡献者的支持！🙏
 
 <!-- SVG image from https://opencollective.com/ultralytics/contributors.svg?width=990 -->
 
-<a href="https://github.com/ultralytics/ultralytics/graphs/contributors"><img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/image-contributors-1280.png"/></a>
+<a href="https://github.com/ultralytics/yolov5/graphs/contributors">
+<img width="100%" src="https://github.com/ultralytics/assets/raw/main/im/image-contributors.png"></a>
 
-## <div align="center">License</div>
+## <div align="center">许可证</div>
 
-- YOLOv8 在两种不同的 License 下可用：
-  - **GPL-3.0 License**： 查看 [License](https://github.com/ultralytics/ultralytics/blob/main/LICENSE) 文件的详细信息。
-  - **企业License**：在没有 GPL-3.0 开源要求的情况下为商业产品开发提供更大的灵活性。典型用例是将 Ultralytics 软件和 AI 模型嵌入到商业产品和应用程序中。在以下位置申请企业许可证 [Ultralytics 许可](https://ultralytics.com/license) 。
+YOLOv8 提供两种不同的许可证：
 
-## <div align="center">联系我们</div>
+- **AGPL-3.0 许可证**：详细信息请参阅 [LICENSE](https://github.com/ultralytics/ultralytics/blob/main/LICENSE) 文件。
+- **企业许可证**：为商业产品开发提供更大的灵活性，无需遵循 AGPL-3.0 的开源要求。典型的用例是将 Ultralytics 软件和 AI 模型嵌入商业产品和应用中。在 [Ultralytics 授权](https://ultralytics.com/license) 处申请企业许可证。
 
-若发现 YOLOv8 的 Bug 或有功能需求，请访问 [GitHub 问题](https://github.com/ultralytics/ultralytics/issues)。如需专业支持，请 [联系我们](https://ultralytics.com/contact)。
+## <div align="center">联系方式</div>
+
+对于 YOLOv8 的错误报告和功能请求，请访问 [GitHub Issues](https://github.com/ultralytics/ultralytics/issues)，并加入我们的 [Discord](https://discord.gg/n6cFeSPZdD) 社区进行问题和讨论！
 
 <br>
 <div align="center">
   <a href="https://github.com/ultralytics" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
   <a href="https://www.linkedin.com/company/ultralytics" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
   <a href="https://twitter.com/ultralytics" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
-  <a href="https://www.producthunt.com/@glenn_jocher" style="text-decoration:none;">
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-producthunt.png" width="3%" alt="" /></a>
-  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
   <a href="https://youtube.com/ultralytics" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
-  <a href="https://www.facebook.com/ultralytics" style="text-decoration:none;">
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-facebook.png" width="3%" alt="" /></a>
+  <a href="https://www.tiktok.com/@ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-tiktok.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
   <a href="https://www.instagram.com/ultralytics/" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="3%" alt="" /></a>
+  <a href="https://discord.gg/n6cFeSPZdD" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/blob/main/social/logo-social-discord.png" width="3%" alt="" /></a>
 </div>
```

#### html2text {}

```diff
@@ -1,191 +1,224 @@
    [https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/banner-
                                   yolov8.png]
             [English](README.md) | [ç®ä½ä¸­æ](README.zh-CN.md)
               [Ultralytics_CI] [YOLOv8_Citation] [Docker_Pulls]
               [Run_on_Gradient] [Open_In_Colab] [Open_In_Kaggle]
 
-   [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics) æ¯ç±
-     [Ultralytics](https://ultralytics.com) å¼åçä¸ä¸ªåæ²¿ç SOTA
-                      æ¨¡åãå®å¨ä»¥åæåç YOLO
-çæ¬åºç¡ä¸ï¼å¼å¥äºæ°çåè½åæ¹è¿ï¼è¿ä¸æ­¥æåäºå¶æ§è½åçµæ´»æ§ãYOLOv8
-åºäºå¿«éãåç¡®åæäºä½¿ç¨çè®¾è®¡çå¿µï¼ä½¿å¶æä¸ºå¹¿æ³çç®æ æ£æµãå¾ååå²åå¾ååç±»ä»»å¡çç»ä½³éæ©ã
-   å¦æè¦ç³è¯·ä¼ä¸è®¸å¯è¯ï¼è¯·å¡«å [Ultralytics è®¸å¯](https://
-                          ultralytics.com/license)ã
+[Ultralytics](https://ultralytics.com) [YOLOv8](https://github.com/ultralytics/
+ultralytics) æ¯ä¸æ¬¾åæ²¿ãæåè¿ï¼SOTAï¼çæ¨¡åï¼åºäºåå YOLO
+çæ¬çæåï¼å¼å¥äºæ°åè½åæ¹è¿ï¼è¿ä¸æ­¥æåæ§è½åçµæ´»æ§ãYOLOv8
+è®¾è®¡å¿«éãåç¡®ä¸æäºä½¿ç¨ï¼ä½¿å¶æä¸ºåç§ç©ä½æ£æµä¸è·è¸ªãå®ä¾åå²ãå¾ååç±»åå§¿æä¼°è®¡ä»»å¡çç»ä½³éæ©ã
+ æä»¬å¸æè¿éçèµæºè½å¸®å©æ¨ååå©ç¨ YOLOv8ãè¯·æµè§ YOLOv8
+                    ææ¡£ äºè§£è¯¦ç»ä¿¡æ¯ï¼å¨ GitHub
+          ä¸æäº¤é®é¢ä»¥è·å¾æ¯æï¼å¹¶å å¥æä»¬ç Discord
+ ç¤¾åºè¿è¡é®é¢åè®¨è®ºï¼ å¦éç³è¯·ä¼ä¸è®¸å¯ï¼è¯·å¨ [Ultralytics
+     Licensing](https://ultralytics.com/license) å¤å¡«åè¡¨æ ¼ [https://
+   raw.githubusercontent.com/ultralytics/assets/main/yolov8/yolo-comparison-
+                                  plots.png]
 
 ##
                                     ææ¡£
-æå³è®­ç»ãæµè¯åé¨ç½²çå®æ´ææ¡£è§[YOLOv8 Docs](https://
-docs.ultralytics.com)ãè¯·åéä¸é¢çå¿«éå¥é¨ç¤ºä¾ã  å®è£ Pip
-å®è£åå«ææ [requirements.txt](https://github.com/ultralytics/
-ultralytics/blob/main/requirements.txt) ç ultralytics åï¼ç¯å¢è¦æ±
-[**3.10>=Python>=3.7**](https://www.python.org/)ï¼ä¸ [**PyTorch>=1.7**]
-(https://pytorch.org/get-started/locally/)ã ```bash pip install ultralytics
-```   ä½¿ç¨æ¹æ³ YOLOv8 å¯ä»¥ç´æ¥å¨å½ä»¤è¡çé¢ï¼CLIï¼ä¸­ä½¿ç¨
-`yolo` å½ä»¤è¿è¡ï¼ ```bash yolo predict model=yolov8n.pt source="https://
-ultralytics.com/images/bus.jpg" ```
-`yolo`å¯ä»¥ç¨äºåç§ä»»å¡åæ¨¡å¼ï¼å¹¶æ¥åé¢å¤çåæ°ï¼ä¾å¦
-`imgsz=640`ãåè§ YOLOv8 [ææ¡£](https://
-docs.ultralytics.com)ä¸­å¯ç¨`yolo`[åæ°](https://docs.ultralytics.com/
-config/)çå®æ´åè¡¨ã ```bash yolo task=detect mode=train model=yolov8n.pt
-args... classify predict yolov8n-cls.yaml args... segment val yolov8n-seg.yaml
-args... export yolov8n.pt format=onnx args... ``` YOLOv8 ä¹å¯ä»¥å¨ Python
-ç¯å¢ä¸­ç´æ¥ä½¿ç¨ï¼å¹¶æ¥åä¸ä¸é¢ CLI ä¾å­ä¸­ç¸åç[åæ°]
-(https://docs.ultralytics.com/config/)ï¼ ```python from ultralytics import
+è¯·åéä¸é¢çå¿«éå®è£åä½¿ç¨ç¤ºä¾ï¼ä»¥å [YOLOv8 ææ¡£](https://
+docs.ultralytics.com)
+ä¸æå³å¹è®­ãéªè¯ãé¢æµåé¨ç½²çå®æ´ææ¡£ã  å®è£ å¨ä¸ä¸ª
+[**Python>=3.7**](https://www.python.org/) ç¯å¢ä¸­ï¼ä½¿ç¨
+[**PyTorch>=1.7**](https://pytorch.org/get-started/locally/)ï¼éè¿ pip
+å®è£ ultralytics è½¯ä»¶åä»¥åææ[ä¾èµé¡¹](https://github.com/
+ultralytics/ultralytics/blob/main/requirements.txt)ã ```bash pip install
+ultralytics ```   Usage #### CLI YOLOv8
+å¯ä»¥å¨å½ä»¤è¡çé¢ï¼CLIï¼ä¸­ç´æ¥ä½¿ç¨ï¼åªéè¾å¥ `yolo`
+å½ä»¤ï¼ ```bash yolo predict model=yolov8n.pt source='https://
+ultralytics.com/images/bus.jpg' ``` `yolo`
+å¯ç¨äºåç§ä»»å¡åæ¨¡å¼ï¼å¹¶æ¥åå¶ä»åæ°ï¼ä¾å¦
+`imgsz=640`ãæ¥ç YOLOv8 [CLI ææ¡£](https://docs.ultralytics.com/usage/
+cli)ä»¥è·åç¤ºä¾ã #### Python YOLOv8 ä¹å¯ä»¥å¨ Python
+ç¯å¢ä¸­ç´æ¥ä½¿ç¨ï¼å¹¶æ¥åä¸ä¸è¿° CLI ç¤ºä¾ä¸­ç¸åç[åæ°]
+(https://docs.ultralytics.com/usage/cfg/)ï¼ ```python from ultralytics import
 YOLO # å è½½æ¨¡å model = YOLO("yolov8n.yaml") # ä»å¤´å¼å§æå»ºæ°æ¨¡å
-model = YOLO("yolov8n.pt") # å è½½é¢è®­ç»æ¨¡åï¼æ¨èç¨äºè®­ç»ï¼ #
-Use the model results = model.train(data="coco128.yaml", epochs=3) #
-è®­ç»æ¨¡å results = model.val() # å¨éªè¯éä¸è¯ä¼°æ¨¡åæ§è½ results
-= model("https://ultralytics.com/images/bus.jpg") # é¢æµå¾å success =
-model.export(format="onnx") # å°æ¨¡åå¯¼åºä¸º ONNX æ ¼å¼ ``` [æ¨¡å]
-(https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models)
-ä¼ä» Ultralytics [åå¸é¡µ](https://github.com/ultralytics/ultralytics/
-releases) èªå¨ä¸è½½ã ### å·²ç¥é®é¢ / å¾åäºé¡¹
-æä»¬ä»å¨åªåå®å YOLOv8
-çå ä¸ªé¨åï¼æä»¬çç®æ æ¯å°½å¿«å®æè¿äºå·¥ä½ï¼ä½¿ YOLOv8
-çåè½è®¾ç½®è¾¾å°YOLOv5
-çæ°´å¹³ï¼åæ¬å¯¹ææç¸åæ ¼å¼çå¯¼åºåæ¨çãæä»¬è¿å¨åä¸ç¯
-YOLOv8 çè®ºæï¼ä¸æ¦å®æï¼æä»¬å°æäº¤ç» [arxiv.org](https://
-arxiv.org)ã - [ ] TensorFlow å¯¼åº - [ ] DDP æ¢å¤è®­ç» - [ ] [arxiv.org]
-(https://arxiv.org) è®ºæ  ##
+model = YOLO("yolov8n.pt") # å è½½é¢è®­ç»æ¨¡åï¼å»ºè®®ç¨äºè®­ç»ï¼ #
+ä½¿ç¨æ¨¡å model.train(data="coco128.yaml", epochs=3) # è®­ç»æ¨¡å metrics
+= model.val() # å¨éªè¯éä¸è¯ä¼°æ¨¡åæ§è½ results = model("https://
+ultralytics.com/images/bus.jpg") # å¯¹å¾åè¿è¡é¢æµ success = model.export
+(format="onnx") # å°æ¨¡åå¯¼åºä¸º ONNX æ ¼å¼ ``` [æ¨¡å](https://
+github.com/ultralytics/ultralytics/tree/main/ultralytics/models)
+ä¼èªå¨ä»ææ°ç Ultralytics [åå¸çæ¬](https://github.com/
+ultralytics/assets/releases)ä¸­ä¸è½½ãæ¥ç YOLOv8 [Python ææ¡£](https://
+docs.ultralytics.com/usage/python)ä»¥è·åæ´å¤ç¤ºä¾ã  ##
                                     æ¨¡å
-ææ YOLOv8
-çé¢è®­ç»æ¨¡åé½å¯ä»¥å¨è¿éæ¾å°ãç®æ æ£æµååå²æ¨¡åæ¯å¨
-COCO æ°æ®éä¸é¢è®­ç»çï¼èåç±»æ¨¡åæ¯å¨ ImageNet
-æ°æ®éä¸é¢è®­ç»çã ç¬¬ä¸æ¬¡ä½¿ç¨æ¶ï¼[æ¨¡å](https://github.com/
-ultralytics/ultralytics/tree/main/ultralytics/models) ä¼ä» Ultralytics
-[åå¸é¡µ](https://github.com/ultralytics/ultralytics/releases)
-èªå¨ä¸è½½ã ç®æ æ£æµ | æ¨¡å | å°ºå¯¸
-ï¼åç´ ï¼ | mAPval
-50-95 | æ¨çéåº¦
+ææç YOLOv8
+é¢è®­ç»æ¨¡åé½å¯ä»¥å¨æ­¤æ¾å°ãæ£æµãåå²åå§¿ææ¨¡åå¨ [COCO]
+(https://github.com/ultralytics/ultralytics/blob/main/ultralytics/datasets/
+coco.yaml) æ°æ®éä¸è¿è¡é¢è®­ç»ï¼èåç±»æ¨¡åå¨ [ImageNet](https://
+github.com/ultralytics/ultralytics/blob/main/ultralytics/datasets/
+ImageNet.yaml) æ°æ®éä¸è¿è¡é¢è®­ç»ã å¨é¦æ¬¡ä½¿ç¨æ¶ï¼[æ¨¡å]
+(https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models)
+ä¼èªå¨ä»ææ°ç Ultralytics [åå¸çæ¬](https://github.com/
+ultralytics/assets/releases)ä¸­ä¸è½½ã æ£æµ æ¥ç [æ£æµææ¡£](https://
+docs.ultralytics.com/tasks/detect/) ä»¥è·åä½¿ç¨è¿äºæ¨¡åçç¤ºä¾ã |
+æ¨¡å | å°ºå¯¸
+(åç´ ) | mAPval
+50-95 | éåº¦
 CPU ONNX
-(ms) | æ¨çéåº¦
+(ms) | éåº¦
 A100 TensorRT
-(ms) | åæ°é
+(ms) | åæ°
 (M) | FLOPs
 (B) | | -----------------------------------------------------------------------
 ------------- | --------------- | -------------------- | ----------------------
-------- | ---------------------------------- | --------------- | --------------
---- | | [YOLOv8n](https://github.com/ultralytics/assets/releases/download/
-v0.0.0/yolov8n.pt) | 640 | 37.3 | 80.4 | 0.99 | 3.2 | 8.7 | | [YOLOv8s](https:/
-/github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s.pt) | 640 |
-44.9 | 128.4 | 1.20 | 11.2 | 28.6 | | [YOLOv8m](https://github.com/ultralytics/
+----- | -------------------------------- | -------------- | ----------------- |
+| [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/
+yolov8n.pt) | 640 | 37.3 | 80.4 | 0.99 | 3.2 | 8.7 | | [YOLOv8s](https://
+github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s.pt) | 640 | 44.9
+| 128.4 | 1.20 | 11.2 | 28.6 | | [YOLOv8m](https://github.com/ultralytics/
 assets/releases/download/v0.0.0/yolov8m.pt) | 640 | 50.2 | 234.7 | 1.83 | 25.9
 | 78.9 | | [YOLOv8l](https://github.com/ultralytics/assets/releases/download/
 v0.0.0/yolov8l.pt) | 640 | 52.9 | 375.2 | 2.39 | 43.7 | 165.2 | | [YOLOv8x]
 (https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x.pt) |
-640 | 53.9 | 479.1 | 3.53 | 68.2 | 257.8 | - **mAPval** ç»æé½å¨ [COCO
-val2017](http://cocodataset.org)
-æ°æ®éä¸ï¼ä½¿ç¨åæ¨¡ååå°ºåº¦æµè¯å¾å°ã
-å¤ç°å½ä»¤ `yolo val detect data=coco.yaml device=0` - **æ¨çéåº¦**ä½¿ç¨
-COCO éªè¯éå¾çæ¨çæ¶é´è¿è¡å¹³åå¾å°ï¼æµè¯ç¯å¢ä½¿ç¨ [Amazon
-EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) å®ä¾ã
-å¤ç°å½ä»¤ `yolo val detect data=coco128.yaml batch=1 device=0/cpu`
-å®ä¾åå² | æ¨¡å | å°ºå¯¸
-ï¼åç´ ï¼ | mAPbox
+640 | 53.9 | 479.1 | 3.53 | 68.2 | 257.8 | - **mAPval**
+å¼æ¯åºäºåæ¨¡ååå°ºåº¦å¨ [COCO val2017](http://cocodataset.org)
+æ°æ®éä¸çç»æã
+éè¿ `yolo val detect data=coco.yaml device=0` å¤ç° - **éåº¦** æ¯ä½¿ç¨
+[Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) å®ä¾å¯¹ COCO
+val å¾åè¿è¡å¹³åè®¡ç®çã
+éè¿ `yolo val detect data=coco128.yaml batch=1 device=0|cpu` å¤ç°  åå²
+æ¥ç [åå²ææ¡£](https://docs.ultralytics.com/tasks/segment/
+) ä»¥è·åä½¿ç¨è¿äºæ¨¡åçç¤ºä¾ã | æ¨¡å | å°ºå¯¸
+(åç´ ) | mAPbox
 50-95 | mAPmask
-50-95 | æ¨çéåº¦
+50-95 | éåº¦
 CPU ONNX
-(ms) | æ¨çéåº¦
+(ms) | éåº¦
 A100 TensorRT
-(ms) | åæ°é
+(ms) | åæ°
 (M) | FLOPs
 (B) | | -----------------------------------------------------------------------
------------------ | --------------- | -------------------- | ------------------
---- | ----------------------------- | ---------------------------------- | ----
------------ | ----------------- | | [YOLOv8n](https://github.com/ultralytics/
-assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640 | 36.7 | 30.5 | 96.1 |
-1.21 | 3.4 | 12.6 | | [YOLOv8s](https://github.com/ultralytics/assets/releases/
-download/v0.0.0/yolov8s-seg.pt) | 640 | 44.6 | 36.8 | 155.7 | 1.47 | 11.8 |
-42.6 | | [YOLOv8m](https://github.com/ultralytics/assets/releases/download/
-v0.0.0/yolov8m-seg.pt) | 640 | 49.9 | 40.8 | 317.0 | 2.18 | 27.3 | 110.2 | |
-[YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/
-yolov8l-seg.pt) | 640 | 52.3 | 42.6 | 572.4 | 2.79 | 46.0 | 220.5 | | [YOLOv8x]
-(https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-seg.pt)
-| 640 | 53.4 | 43.4 | 712.1 | 4.02 | 71.8 | 344.1 | - **mAPval** ç»æé½å¨
-[COCO val2017](http://cocodataset.org)
-æ°æ®éä¸ï¼ä½¿ç¨åæ¨¡ååå°ºåº¦æµè¯å¾å°ã
-å¤ç°å½ä»¤ `yolo val segment data=coco.yaml device=0` -
-**æ¨çéåº¦**ä½¿ç¨ COCO
-éªè¯éå¾çæ¨çæ¶é´è¿è¡å¹³åå¾å°ï¼æµè¯ç¯å¢ä½¿ç¨ [Amazon EC2
-P4d](https://aws.amazon.com/ec2/instance-types/p4/) å®ä¾ã
-å¤ç°å½ä»¤ `yolo val segment data=coco128-seg.yaml batch=1 device=0/cpu`
-åç±» | æ¨¡å | å°ºå¯¸
-ï¼åç´ ï¼ | acc
+--------------------- | --------------- | -------------------- | --------------
+------- | --------------------------- | -------------------------------- | ----
+---------- | ----------------- | | [YOLOv8n-seg](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640 | 36.7 | 30.5
+| 96.1 | 1.21 | 3.4 | 12.6 | | [YOLOv8s-seg](https://github.com/ultralytics/
+assets/releases/download/v0.0.0/yolov8s-seg.pt) | 640 | 44.6 | 36.8 | 155.7 |
+1.47 | 11.8 | 42.6 | | [YOLOv8m-seg](https://github.com/ultralytics/assets/
+releases/download/v0.0.0/yolov8m-seg.pt) | 640 | 49.9 | 40.8 | 317.0 | 2.18 |
+27.3 | 110.2 | | [YOLOv8l-seg](https://github.com/ultralytics/assets/releases/
+download/v0.0.0/yolov8l-seg.pt) | 640 | 52.3 | 42.6 | 572.4 | 2.79 | 46.0 |
+220.5 | | [YOLOv8x-seg](https://github.com/ultralytics/assets/releases/
+download/v0.0.0/yolov8x-seg.pt) | 640 | 53.4 | 43.4 | 712.1 | 4.02 | 71.8 |
+344.1 | - **mAPval** å¼æ¯åºäºåæ¨¡ååå°ºåº¦å¨ [COCO val2017](http://
+cocodataset.org) æ°æ®éä¸çç»æã
+éè¿ `yolo val segment data=coco.yaml device=0` å¤ç° - **éåº¦** æ¯ä½¿ç¨
+[Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) å®ä¾å¯¹ COCO
+val å¾åè¿è¡å¹³åè®¡ç®çã
+éè¿ `yolo val segment data=coco128-seg.yaml batch=1 device=0|cpu` å¤ç°
+åç±» æ¥ç [åç±»ææ¡£](https://docs.ultralytics.com/tasks/classify/
+) ä»¥è·åä½¿ç¨è¿äºæ¨¡åçç¤ºä¾ã | æ¨¡å | å°ºå¯¸
+(åç´ ) | acc
 top1 | acc
-top5 | æ¨çéåº¦
+top5 | éåº¦
 CPU ONNX
-(ms) | æ¨çéåº¦
+(ms) | éåº¦
 A100 TensorRT
-(ms) | åæ°é
+(ms) | åæ°
 (M) | FLOPs
 (B) at 640 | | ----------------------------------------------------------------
------------------------- | --------------- | ---------------- | ---------------
-- | ----------------------------- | ---------------------------------- | ------
---------- | ------------------------ | | [YOLOv8n](https://github.com/
+---------------------------- | --------------- | ---------------- | -----------
+----- | --------------------------- | -------------------------------- | ------
+-------- | ------------------------ | | [YOLOv8n-cls](https://github.com/
 ultralytics/assets/releases/download/v0.0.0/yolov8n-cls.pt) | 224 | 66.6 | 87.0
-| 12.9 | 0.31 | 2.7 | 4.3 | | [YOLOv8s](https://github.com/ultralytics/assets/
-releases/download/v0.0.0/yolov8s-cls.pt) | 224 | 72.3 | 91.1 | 23.4 | 0.35 |
-6.4 | 13.5 | | [YOLOv8m](https://github.com/ultralytics/assets/releases/
-download/v0.0.0/yolov8m-cls.pt) | 224 | 76.4 | 93.2 | 85.4 | 0.62 | 17.0 | 42.7
-| | [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/
-yolov8l-cls.pt) | 224 | 78.0 | 94.1 | 163.0 | 0.87 | 37.5 | 99.7 | | [YOLOv8x]
-(https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-cls.pt)
-| 224 | 78.4 | 94.3 | 232.0 | 1.01 | 57.4 | 154.8 | - **acc** é½å¨ [ImageNet]
-(https://www.image-net.org/
-) æ°æ®éä¸ï¼ä½¿ç¨åæ¨¡ååå°ºåº¦æµè¯å¾å°ã
-å¤ç°å½ä»¤ `yolo val classify data=path/to/ImageNet device=0` -
-**æ¨çéåº¦**ä½¿ç¨ ImageNet
-éªè¯éå¾çæ¨çæ¶é´è¿è¡å¹³åå¾å°ï¼æµè¯ç¯å¢ä½¿ç¨ [Amazon EC2
-P4d](https://aws.amazon.com/ec2/instance-types/p4/) å®ä¾ã
-å¤ç°å½ä»¤ `yolo val classify data=path/to/ImageNet batch=1 device=0/cpu`  ##
-                                 æ¨¡åéæ
+| 12.9 | 0.31 | 2.7 | 4.3 | | [YOLOv8s-cls](https://github.com/ultralytics/
+assets/releases/download/v0.0.0/yolov8s-cls.pt) | 224 | 72.3 | 91.1 | 23.4 |
+0.35 | 6.4 | 13.5 | | [YOLOv8m-cls](https://github.com/ultralytics/assets/
+releases/download/v0.0.0/yolov8m-cls.pt) | 224 | 76.4 | 93.2 | 85.4 | 0.62 |
+17.0 | 42.7 | | [YOLOv8l-cls](https://github.com/ultralytics/assets/releases/
+download/v0.0.0/yolov8l-cls.pt) | 224 | 78.0 | 94.1 | 163.0 | 0.87 | 37.5 |
+99.7 | | [YOLOv8x-cls](https://github.com/ultralytics/assets/releases/download/
+v0.0.0/yolov8x-cls.pt) | 224 | 78.4 | 94.3 | 232.0 | 1.01 | 57.4 | 154.8 | -
+**acc** å¼æ¯æ¨¡åå¨ [ImageNet](https://www.image-net.org/
+) æ°æ®ééªè¯éä¸çåç¡®çã
+éè¿ `yolo val classify data=path/to/ImageNet device=0` å¤ç° - **éåº¦**
+æ¯ä½¿ç¨ [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/
+) å®ä¾å¯¹ ImageNet val å¾åè¿è¡å¹³åè®¡ç®çã
+éè¿ `yolo val classify data=path/to/ImageNet batch=1 device=0|cpu` å¤ç°
+å§¿æ æ¥ç [å§¿æææ¡£](https://docs.ultralytics.com/tasks/
+) ä»¥è·åä½¿ç¨è¿äºæ¨¡åçç¤ºä¾ã | æ¨¡å | å°ºå¯¸
+(åç´ ) | mAPpose
+50-95 | mAPpose
+50 | éåº¦
+CPU ONNX
+(ms) | éåº¦
+A100 TensorRT
+(ms) | åæ°
+(M) | FLOPs
+(B) | | -----------------------------------------------------------------------
+----------------------------- | --------------- | --------------------- | -----
+------------- | --------------------------- | -------------------------------
+- | -------------- | ----------------- | | [YOLOv8n-pose](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8n-pose.pt) | 640 | 50.4 |
+80.1 | 131.8 | 1.18 | 3.3 | 9.2 | | [YOLOv8s-pose](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8s-pose.pt) | 640 | 60.0 |
+86.2 | 233.2 | 1.42 | 11.6 | 30.2 | | [YOLOv8m-pose](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8m-pose.pt) | 640 | 65.0 |
+88.8 | 456.3 | 2.00 | 26.4 | 81.0 | | [YOLOv8l-pose](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8l-pose.pt) | 640 | 67.6 |
+90.0 | 784.5 | 2.59 | 44.4 | 168.6 | | [YOLOv8x-pose](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8x-pose.pt) | 640 | 69.2 |
+90.2 | 1607.1 | 3.73 | 69.4 | 263.2 | | [YOLOv8x-pose-p6](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8x-pose-p6.pt) | 1280 | 71.6 |
+91.2 | 4088.7 | 10.04 | 99.1 | 1066.4 | - **mAPval**
+å¼æ¯åºäºåæ¨¡ååå°ºåº¦å¨ [COCO Keypoints val2017](http://
+cocodataset.org) æ°æ®éä¸çç»æã
+éè¿ `yolo val pose data=coco-pose.yaml device=0` å¤ç° - **éåº¦**
+æ¯ä½¿ç¨ [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/
+) å®ä¾å¯¹ COCO val å¾åè¿è¡å¹³åè®¡ç®çã
+éè¿ `yolo val pose data=coco8-pose.yaml batch=1 device=0|cpu` å¤ç°  ##
+                                    éæ
 
 [https://github.com/ultralytics/assets/raw/main/yolov8/banner-integrations.png]
 
 
-      [https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-
- roboflow.png]  [https://github.com/ultralytics/yolov5/releases/download/v1.0/
- logo-clearml.png]  [https://github.com/ultralytics/yolov5/releases/download/
-v1.0/logo-comet.png]  [https://github.com/ultralytics/yolov5/releases/download/
-                          v1.0/logo-neuralmagic.png]
-| Roboflow | ClearML â­ æ° | Comet â­ æ° | Neural Magic â­ æ° | | :------
+ [https://github.com/ultralytics/assets/raw/main/partners/logo-roboflow.png]
+ [https://github.com/ultralytics/assets/raw/main/partners/logo-clearml.png]
+  [https://github.com/ultralytics/assets/raw/main/partners/logo-comet.png]
+[https://github.com/ultralytics/assets/raw/main/partners/logo-neuralmagic.png]
+| Roboflow | ClearML â­ NEW | Comet â­ NEW | Neural Magic â­ NEW | | :------
 --------------------------------------------------------------------------: | :
--------------------------------------------------------------------------: | :-
-------------------------------------------------------------------------------:
-| :----------------------------------------------------------------------------
---------: | | å°æ¨çèªå®ä¹æ°æ®éè¿è¡æ æ³¨å¹¶ç´æ¥å¯¼åºå° YOLOv8
-ä»¥è¿è¡è®­ç» [Roboflow](https://roboflow.com/?ref=ultralytics) |
-èªå¨è·è¸ªãå¯è§åçè³è¿ç¨è®­ç» YOLOv8 [ClearML](https://cutt.ly/
-yolov5-readme-clearml)ï¼å¼æºï¼ï¼ | æ°¸è¿åè´¹ï¼[Comet](https://bit.ly/
-yolov5-readme-comet)å¯è®©æ¨ä¿å­ YOLOv8
-æ¨¡åãæ¢å¤è®­ç»ä»¥åäº¤äºå¼å¯è§ååè°è¯é¢æµ | ä½¿ç¨ [Neural
-Magic DeepSparse](https://bit.ly/yolov5-neuralmagic)ï¼è¿è¡ YOLOv8
-æ¨ççéåº¦æé«å¯æé«6å | ##
+----------------------------------------------------------------------------: |
+:------------------------------------------------------------------------------
+----: | :----------------------------------------------------------------------
+-------------: | | ä½¿ç¨ [Roboflow](https://roboflow.com/?ref=ultralytics)
+å°æ¨çèªå®ä¹æ°æ®éç´æ¥æ è®°å¹¶å¯¼åºè³ YOLOv8 è¿è¡è®­ç» |
+ä½¿ç¨ [ClearML](https://cutt.ly/yolov5-readme-
+clearml)ï¼å¼æºï¼ï¼èªå¨è·è¸ªãå¯è§åï¼çè³è¿ç¨è®­ç» YOLOv8 |
+åè´¹ä¸æ°¸ä¹ï¼[Comet](https://bit.ly/yolov8-readme-comet) è®©æ¨ä¿å­
+YOLOv8 æ¨¡åãæ¢å¤è®­ç»ï¼å¹¶ä»¥äº¤äºå¼æ¹å¼æ¥çåè°è¯é¢æµ |
+ä½¿ç¨ [Neural Magic DeepSparse](https://bit.ly/yolov5-neuralmagic) ä½¿ YOLOv8
+æ¨çéåº¦æé«å¤è¾¾ 6 å | ##
                                 Ultralytics HUB
-[Ultralytics HUB](https://bit.ly/ultralytics_hub) æ¯æä»¬â­
-**æ°**çæ ä»£ç è§£å³æ¹æ¡ï¼ç¨äºå¯è§åæ°æ®éï¼è®­ç» YOLOv8ð
-æ¨¡åï¼å¹¶ä»¥æ ç¼ä½éªæ¹å¼é¨ç½²å°ç°å®ä¸çãç°å¨å¼å§**åè´¹**!
-è¿å¯ä»¥éè¿ä¸è½½ [Ultralytics App](https://ultralytics.com/app_install)
-å¨ä½ ç iOS æ Android è®¾å¤ä¸è¿è¡ YOLOv8 æ¨¡å! [https://github.com/
+ä½éª [Ultralytics HUB](https://bit.ly/ultralytics_hub) â­ å¸¦æ¥çæ ç¼
+AIï¼è¿æ¯ä¸ä¸ªä¸ä½åè§£å³æ¹æ¡ï¼ç¨äºæ°æ®å¯è§åãYOLOv5
+åå³å°æ¨åºç YOLOv8 ð
+æ¨¡åè®­ç»åé¨ç½²ï¼æ éä»»ä½ç¼ç ãéè¿æä»¬åè¿çå¹³å°åç¨æ·åå¥½ç
+[Ultralytics åºç¨ç¨åº](https://ultralytics.com/
+app_install)ï¼è½»æ¾å°å¾åè½¬åä¸ºå¯æä½çè§è§£ï¼å¹¶å®ç°æ¨ç AI
+æ¿æ¯ãç°å¨å°±å¼å§æ¨ç**åè´¹**ä¹æï¼ [https://github.com/
 ultralytics/assets/raw/main/im/ultralytics-hub.png] ##
                                     è´¡ç®
-æä»¬åæ¬¢æ¨çæè§æå»ºè®®ï¼æä»¬å¸æå°½å¯è½ç®ååéæå°ä¸º
-YOLOv8 ååºè´¡ç®ãè¯·çæä»¬ç [è´¡ç®æå](CONTRIBUTING.md)
-ï¼å¹¶å¡«å [è°æ¥é®å·](https://ultralytics.com/
-survey?utm_source=github&utm_medium=social&utm_campaign=Survey)
-åæä»¬åéæ¨çä½éªåé¦ãæè°¢æä»¬ææçè´¡ç®èï¼  [https:/
-/github.com/ultralytics/yolov5/releases/download/v1.0/image-contributors-
-1280.png] ##
-                                    License
-- YOLOv8 å¨ä¸¤ç§ä¸åç License ä¸å¯ç¨ï¼ - **GPL-3.0 License**ï¼
-æ¥ç [License](https://github.com/ultralytics/ultralytics/blob/main/LICENSE)
-æä»¶çè¯¦ç»ä¿¡æ¯ã - **ä¼ä¸License**ï¼å¨æ²¡æ GPL-3.0
-å¼æºè¦æ±çæåµä¸ä¸ºåä¸äº§åå¼åæä¾æ´å¤§ççµæ´»æ§ãå¸åç¨ä¾æ¯å°
-Ultralytics è½¯ä»¶å AI
-æ¨¡ååµå¥å°åä¸äº§åååºç¨ç¨åºä¸­ãå¨ä»¥ä¸ä½ç½®ç³è¯·ä¼ä¸è®¸å¯è¯
-[Ultralytics è®¸å¯](https://ultralytics.com/license) ã ##
-                                 èç³»æä»¬
-è¥åç° YOLOv8 ç Bug ææåè½éæ±ï¼è¯·è®¿é® [GitHub é®é¢](https:/
-/github.com/ultralytics/ultralytics/issues)ãå¦éä¸ä¸æ¯æï¼è¯·
-[èç³»æä»¬](https://ultralytics.com/contact)ã
+æä»¬åæ¬¢æ¨çåä¸ï¼æ²¡æç¤¾åºçå¸®å©ï¼YOLOv5 å YOLOv8
+å°æ æ³å®ç°ãè¯·åéæä»¬ç[è´¡ç®æå](https://
+docs.ultralytics.com/help/contributing)ä»¥å¼å§ä½¿ç¨ï¼å¹¶å¡«åæä»¬ç
+[è°æ¥é®å·](https://ultralytics.com/
+survey?utm_source=github&utm_medium=social&utm_campaign=Survey)åæä»¬æä¾æ¨çä½¿ç¨ä½éªåé¦ãæè°¢ææè´¡ç®èçæ¯æï¼ð
+[https://github.com/ultralytics/assets/raw/main/im/image-contributors.png] ##
+                                   è®¸å¯è¯
+YOLOv8 æä¾ä¸¤ç§ä¸åçè®¸å¯è¯ï¼ - **AGPL-3.0
+è®¸å¯è¯**ï¼è¯¦ç»ä¿¡æ¯è¯·åé [LICENSE](https://github.com/ultralytics/
+ultralytics/blob/main/LICENSE) æä»¶ã -
+**ä¼ä¸è®¸å¯è¯**ï¼ä¸ºåä¸äº§åå¼åæä¾æ´å¤§ççµæ´»æ§ï¼æ ééµå¾ª
+AGPL-3.0 çå¼æºè¦æ±ãå¸åçç¨ä¾æ¯å° Ultralytics è½¯ä»¶å AI
+æ¨¡ååµå¥åä¸äº§åååºç¨ä¸­ãå¨ [Ultralytics ææ](https://
+ultralytics.com/license) å¤ç³è¯·ä¼ä¸è®¸å¯è¯ã ##
+                                 èç³»æ¹å¼
+å¯¹äº YOLOv8 çéè¯¯æ¥åååè½è¯·æ±ï¼è¯·è®¿é® [GitHub Issues](https:
+//github.com/ultralytics/ultralytics/issues)ï¼å¹¶å å¥æä»¬ç [Discord]
+(https://discord.gg/n6cFeSPZdD) ç¤¾åºè¿è¡é®é¢åè®¨è®ºï¼
```

### Comparing `ultralytics-8.0.9/requirements.txt` & `ultralytics-8.0.90/requirements.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 # Ultralytics requirements
 # Usage: pip install -r requirements.txt
 
 # Base ----------------------------------------
-hydra-core>=1.2.0
 matplotlib>=3.2.2
-numpy>=1.18.5
-opencv-python>=4.1.1
+opencv-python>=4.6.0
 Pillow>=7.1.2
 PyYAML>=5.3.1
 requests>=2.23.0
 scipy>=1.4.1
 torch>=1.7.0
 torchvision>=0.8.1
 tqdm>=4.64.0
 
 # Logging -------------------------------------
-tensorboard>=2.4.1
+# tensorboard>=2.4.1
 # clearml
 # comet
 
 # Plotting ------------------------------------
 pandas>=1.1.4
 seaborn>=0.11.0
 
 # Export --------------------------------------
 # coremltools>=6.0  # CoreML export
 # onnx>=1.12.0  # ONNX export
-# onnx-simplifier>=0.4.1  # ONNX simplifier
+# onnxsim>=0.4.1  # ONNX simplifier
 # nvidia-pyindex  # TensorRT export
 # nvidia-tensorrt  # TensorRT export
 # scikit-learn==0.19.2  # CoreML quantization
 # tensorflow>=2.4.1  # TF exports (-cpu, -aarch64, -macos)
+# tflite-support
 # tensorflowjs>=3.9.0  # TF.js export
-# openvino-dev  # OpenVINO export
+# openvino-dev>=2022.3  # OpenVINO export
 
 # Extras --------------------------------------
-ipython  # interactive notebook
 psutil  # system utilization
 thop>=0.1.1  # FLOPs computation
+# ipython  # interactive notebook
 # albumentations>=1.0.3
 # pycocotools>=2.0.6  # COCO mAP
 # roboflow
-
-# HUB -----------------------------------------
-GitPython>=3.1.24
```

### Comparing `ultralytics-8.0.9/setup.cfg` & `ultralytics-8.0.90/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-license_file = LICENSE
+license_files = LICENSE
 description_file = README.md
 
 [tool:pytest]
 norecursedirs = 
 	.git
 	dist
 	build
@@ -15,27 +15,27 @@
 [flake8]
 max-line-length = 120
 exclude = .tox,*.egg,build,temp
 select = E,W,F
 doctests = True
 verbose = 2
 format = pylint
-ignore = E731,F405,E402,F401,W504,E127,E231,E501,F403
+ignore = E731,F405,E402,W504,E501
 
 [isort]
 line_length = 120
 multi_line_output = 0
 
 [yapf]
 based_on_style = pep8
 spaces_before_comment = 2
 COLUMN_LIMIT = 120
 COALESCE_BRACKETS = True
 SPACES_AROUND_POWER_OPERATOR = True
-SPACE_BETWEEN_ENDING_COMMA_AND_CLOSING_BRACKET = False
+SPACE_BETWEEN_ENDING_COMMA_AND_CLOSING_BRACKET = True
 SPLIT_BEFORE_CLOSING_BRACKET = False
 SPLIT_BEFORE_FIRST_ARGUMENT = False
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ultralytics-8.0.9/setup.py` & `ultralytics-8.0.90/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,67 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import re
 from pathlib import Path
 
 import pkg_resources as pkg
 from setuptools import find_packages, setup
 
 # Settings
 FILE = Path(__file__).resolve()
 PARENT = FILE.parent  # root directory
-README = (PARENT / "README.md").read_text(encoding="utf-8")
+README = (PARENT / 'README.md').read_text(encoding='utf-8')
 REQUIREMENTS = [f'{x.name}{x.specifier}' for x in pkg.parse_requirements((PARENT / 'requirements.txt').read_text())]
 PKG_REQUIREMENTS = ['sentry_sdk']  # pip-only requirements
 
 
 def get_version():
     file = PARENT / 'ultralytics/__init__.py'
-    return re.search(r'^__version__ = [\'"]([^\'"]*)[\'"]', file.read_text(encoding="utf-8"), re.M)[1]
+    return re.search(r'^__version__ = [\'"]([^\'"]*)[\'"]', file.read_text(encoding='utf-8'), re.M)[1]
 
 
 setup(
-    name="ultralytics",  # name of pypi package
+    name='ultralytics',  # name of pypi package
     version=get_version(),  # version of pypi package
-    python_requires=">=3.7,<=3.11",
-    license='GPL-3.0',
+    python_requires='>=3.7',
+    license='AGPL-3.0',
     description='Ultralytics YOLOv8',
     long_description=README,
-    long_description_content_type="text/markdown",
-    url="https://github.com/ultralytics/ultralytics",
+    long_description_content_type='text/markdown',
+    url='https://github.com/ultralytics/ultralytics',
     project_urls={
         'Bug Reports': 'https://github.com/ultralytics/ultralytics/issues',
         'Funding': 'https://ultralytics.com',
         'Source': 'https://github.com/ultralytics/ultralytics'},
-    author="Ultralytics",
+    author='Ultralytics',
     author_email='hello@ultralytics.com',
     packages=find_packages(),  # required
     include_package_data=True,
     install_requires=REQUIREMENTS + PKG_REQUIREMENTS,
     extras_require={
-        'dev':
-        ['check-manifest', 'pytest', 'pytest-cov', 'coverage', 'mkdocs', 'mkdocstrings[python]', 'mkdocs-material']},
+        'dev': [
+            'check-manifest', 'pytest', 'pytest-cov', 'coverage', 'mkdocs-material', 'mkdocstrings[python]',
+            'mkdocs-redirects'],
+        'export': ['coremltools>=6.0', 'openvino-dev>=2022.3', 'tensorflowjs'],  # automatically installs tensorflow
+    },
     classifiers=[
-        "Intended Audience :: Developers", "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)", "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7", "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9", "Programming Language :: Python :: 3.10",
-        "Topic :: Software Development", "Topic :: Scientific/Engineering",
-        "Topic :: Scientific/Engineering :: Artificial Intelligence",
-        "Topic :: Scientific/Engineering :: Image Recognition", "Operating System :: POSIX :: Linux",
-        "Operating System :: MacOS", "Operating System :: Microsoft :: Windows"],
-    keywords="machine-learning, deep-learning, vision, ML, DL, AI, YOLO, YOLOv3, YOLOv5, YOLOv8, HUB, Ultralytics",
+        'Development Status :: 4 - Beta',
+        'Intended Audience :: Developers',
+        'Intended Audience :: Education',
+        'Intended Audience :: Science/Research',
+        'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Topic :: Software Development',
+        'Topic :: Scientific/Engineering',
+        'Topic :: Scientific/Engineering :: Artificial Intelligence',
+        'Topic :: Scientific/Engineering :: Image Recognition',
+        'Operating System :: POSIX :: Linux',
+        'Operating System :: MacOS',
+        'Operating System :: Microsoft :: Windows', ],
+    keywords='machine-learning, deep-learning, vision, ML, DL, AI, YOLO, YOLOv3, YOLOv5, YOLOv8, HUB, Ultralytics',
     entry_points={
-        'console_scripts': ['yolo = ultralytics.yolo.cli:entrypoint', 'ultralytics = ultralytics.yolo.cli:entrypoint']})
+        'console_scripts': ['yolo = ultralytics.yolo.cfg:entrypoint', 'ultralytics = ultralytics.yolo.cfg:entrypoint']})
```

### Comparing `ultralytics-8.0.9/ultralytics/models/v3/yolov3-spp.yaml` & `ultralytics-8.0.90/ultralytics/models/v3/yolov3-spp.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
 # Parameters
 nc: 80  # number of classes
 depth_multiple: 1.0  # model depth multiple
 width_multiple: 1.0  # layer channel multiple
 
 # darknet53 backbone
```

### Comparing `ultralytics-8.0.9/ultralytics/models/v3/yolov3-tiny.yaml` & `ultralytics-8.0.90/ultralytics/models/v3/yolov3-tiny.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
 # Parameters
 nc: 80  # number of classes
 depth_multiple: 1.0  # model depth multiple
 width_multiple: 1.0  # layer channel multiple
 
 # YOLOv3-tiny backbone
```

### Comparing `ultralytics-8.0.9/ultralytics/models/v3/yolov3.yaml` & `ultralytics-8.0.90/ultralytics/models/v3/yolov3.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
 # Parameters
 nc: 80  # number of classes
 depth_multiple: 1.0  # model depth multiple
 width_multiple: 1.0  # layer channel multiple
 
 # darknet53 backbone
```

### Comparing `ultralytics-8.0.9/ultralytics/models/v5/yolov5l.yaml` & `ultralytics-8.0.90/ultralytics/models/v8/yolov8-p6.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,56 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
+# YOLOv8 object detection model with P3-P6 outputs. For Usage examples see https://docs.ultralytics.com/tasks/detect
 
 # Parameters
 nc: 80  # number of classes
-depth_multiple: 1.0  # model depth multiple
-width_multiple: 1.0  # layer channel multiple
+scales: # model compound scaling constants, i.e. 'model=yolov8n-p6.yaml' will call yolov8-p6.yaml with scale 'n'
+  # [depth, width, max_channels]
+  n: [0.33, 0.25, 1024]
+  s: [0.33, 0.50, 1024]
+  m: [0.67, 0.75, 768]
+  l: [1.00, 1.00, 512]
+  x: [1.00, 1.25, 512]
 
-# YOLOv5 v6.0 backbone
+# YOLOv8.0x6 backbone
 backbone:
-  # [from, number, module, args]
-  [[-1, 1, Conv, [64, 6, 2, 2]],  # 0-P1/2
-   [-1, 1, Conv, [128, 3, 2]],  # 1-P2/4
-   [-1, 3, C3, [128]],
-   [-1, 1, Conv, [256, 3, 2]],  # 3-P3/8
-   [-1, 6, C3, [256]],
-   [-1, 1, Conv, [512, 3, 2]],  # 5-P4/16
-   [-1, 9, C3, [512]],
-   [-1, 1, Conv, [1024, 3, 2]],  # 7-P5/32
-   [-1, 3, C3, [1024]],
-   [-1, 1, SPPF, [1024, 5]],  # 9
-  ]
+  # [from, repeats, module, args]
+  - [-1, 1, Conv, [64, 3, 2]]  # 0-P1/2
+  - [-1, 1, Conv, [128, 3, 2]]  # 1-P2/4
+  - [-1, 3, C2f, [128, True]]
+  - [-1, 1, Conv, [256, 3, 2]]  # 3-P3/8
+  - [-1, 6, C2f, [256, True]]
+  - [-1, 1, Conv, [512, 3, 2]]  # 5-P4/16
+  - [-1, 6, C2f, [512, True]]
+  - [-1, 1, Conv, [768, 3, 2]]  # 7-P5/32
+  - [-1, 3, C2f, [768, True]]
+  - [-1, 1, Conv, [1024, 3, 2]]  # 9-P6/64
+  - [-1, 3, C2f, [1024, True]]
+  - [-1, 1, SPPF, [1024, 5]]  # 11
 
-# YOLOv5 v6.0 head
+# YOLOv8.0x6 head
 head:
-  [[-1, 1, Conv, [512, 1, 1]],
-   [-1, 1, nn.Upsample, [None, 2, 'nearest']],
-   [[-1, 6], 1, Concat, [1]],  # cat backbone P4
-   [-1, 3, C3, [512, False]],  # 13
-
-   [-1, 1, Conv, [256, 1, 1]],
-   [-1, 1, nn.Upsample, [None, 2, 'nearest']],
-   [[-1, 4], 1, Concat, [1]],  # cat backbone P3
-   [-1, 3, C3, [256, False]],  # 17 (P3/8-small)
-
-   [-1, 1, Conv, [256, 3, 2]],
-   [[-1, 14], 1, Concat, [1]],  # cat head P4
-   [-1, 3, C3, [512, False]],  # 20 (P4/16-medium)
-
-   [-1, 1, Conv, [512, 3, 2]],
-   [[-1, 10], 1, Concat, [1]],  # cat head P5
-   [-1, 3, C3, [1024, False]],  # 23 (P5/32-large)
+  - [-1, 1, nn.Upsample, [None, 2, 'nearest']]
+  - [[-1, 8], 1, Concat, [1]]  # cat backbone P5
+  - [-1, 3, C2, [768, False]]  # 14
+
+  - [-1, 1, nn.Upsample, [None, 2, 'nearest']]
+  - [[-1, 6], 1, Concat, [1]]  # cat backbone P4
+  - [-1, 3, C2, [512, False]]  # 17
+
+  - [-1, 1, nn.Upsample, [None, 2, 'nearest']]
+  - [[-1, 4], 1, Concat, [1]]  # cat backbone P3
+  - [-1, 3, C2, [256, False]]  # 20 (P3/8-small)
+
+  - [-1, 1, Conv, [256, 3, 2]]
+  - [[-1, 17], 1, Concat, [1]]  # cat head P4
+  - [-1, 3, C2, [512, False]]  # 23 (P4/16-medium)
+
+  - [-1, 1, Conv, [512, 3, 2]]
+  - [[-1, 14], 1, Concat, [1]]  # cat head P5
+  - [-1, 3, C2, [768, False]]  # 26 (P5/32-large)
+
+  - [-1, 1, Conv, [768, 3, 2]]
+  - [[-1, 11], 1, Concat, [1]]  # cat head P6
+  - [-1, 3, C2, [1024, False]]  # 29 (P6/64-xlarge)
 
-   [[17, 20, 23], 1, Detect, [nc]],  # Detect(P3, P4, P5)
-  ]
+  - [[20, 23, 26, 29], 1, Detect, [nc]]  # Detect(P3, P4, P5, P6)
```

### Comparing `ultralytics-8.0.9/ultralytics/models/v5/yolov5m.yaml` & `ultralytics-8.0.90/ultralytics/models/v5/yolov5-p6.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,60 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
 # Parameters
 nc: 80  # number of classes
-depth_multiple: 0.67  # model depth multiple
-width_multiple: 0.75  # layer channel multiple
+scales: # model compound scaling constants, i.e. 'model=yolov5n-p6.yaml' will call yolov5-p6.yaml with scale 'n'
+  # [depth, width, max_channels]
+  n: [0.33, 0.25, 1024]
+  s: [0.33, 0.50, 1024]
+  m: [0.67, 0.75, 1024]
+  l: [1.00, 1.00, 1024]
+  x: [1.33, 1.25, 1024]
 
 # YOLOv5 v6.0 backbone
 backbone:
   # [from, number, module, args]
   [[-1, 1, Conv, [64, 6, 2, 2]],  # 0-P1/2
    [-1, 1, Conv, [128, 3, 2]],  # 1-P2/4
    [-1, 3, C3, [128]],
    [-1, 1, Conv, [256, 3, 2]],  # 3-P3/8
    [-1, 6, C3, [256]],
    [-1, 1, Conv, [512, 3, 2]],  # 5-P4/16
    [-1, 9, C3, [512]],
-   [-1, 1, Conv, [1024, 3, 2]],  # 7-P5/32
+   [-1, 1, Conv, [768, 3, 2]],  # 7-P5/32
+   [-1, 3, C3, [768]],
+   [-1, 1, Conv, [1024, 3, 2]],  # 9-P6/64
    [-1, 3, C3, [1024]],
-   [-1, 1, SPPF, [1024, 5]],  # 9
+   [-1, 1, SPPF, [1024, 5]],  # 11
   ]
 
 # YOLOv5 v6.0 head
 head:
-  [[-1, 1, Conv, [512, 1, 1]],
+  [[-1, 1, Conv, [768, 1, 1]],
+   [-1, 1, nn.Upsample, [None, 2, 'nearest']],
+   [[-1, 8], 1, Concat, [1]],  # cat backbone P5
+   [-1, 3, C3, [768, False]],  # 15
+
+   [-1, 1, Conv, [512, 1, 1]],
    [-1, 1, nn.Upsample, [None, 2, 'nearest']],
    [[-1, 6], 1, Concat, [1]],  # cat backbone P4
-   [-1, 3, C3, [512, False]],  # 13
+   [-1, 3, C3, [512, False]],  # 19
 
    [-1, 1, Conv, [256, 1, 1]],
    [-1, 1, nn.Upsample, [None, 2, 'nearest']],
    [[-1, 4], 1, Concat, [1]],  # cat backbone P3
-   [-1, 3, C3, [256, False]],  # 17 (P3/8-small)
+   [-1, 3, C3, [256, False]],  # 23 (P3/8-small)
 
    [-1, 1, Conv, [256, 3, 2]],
-   [[-1, 14], 1, Concat, [1]],  # cat head P4
-   [-1, 3, C3, [512, False]],  # 20 (P4/16-medium)
+   [[-1, 20], 1, Concat, [1]],  # cat head P4
+   [-1, 3, C3, [512, False]],  # 26 (P4/16-medium)
 
    [-1, 1, Conv, [512, 3, 2]],
-   [[-1, 10], 1, Concat, [1]],  # cat head P5
-   [-1, 3, C3, [1024, False]],  # 23 (P5/32-large)
+   [[-1, 16], 1, Concat, [1]],  # cat head P5
+   [-1, 3, C3, [768, False]],  # 29 (P5/32-large)
 
-   [[17, 20, 23], 1, Detect, [nc]],  # Detect(P3, P4, P5)
-  ]
+   [-1, 1, Conv, [768, 3, 2]],
+   [[-1, 12], 1, Concat, [1]],  # cat head P6
+   [-1, 3, C3, [1024, False]],  # 32 (P6/64-xlarge)
+
+   [[23, 26, 29, 32], 1, Detect, [nc]],  # Detect(P3, P4, P5, P6)
+  ]
```

### Comparing `ultralytics-8.0.9/ultralytics/models/v8/seg/yolov8m-seg.yaml` & `ultralytics-8.0.90/ultralytics/models/v8/yolov8-seg.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,46 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
+# YOLOv8-seg instance segmentation model. For Usage examples see https://docs.ultralytics.com/tasks/segment
 
 # Parameters
 nc: 80  # number of classes
-depth_multiple: 0.67  # scales module repeats
-width_multiple: 0.75  # scales convolution channels
+scales: # model compound scaling constants, i.e. 'model=yolov8n-seg.yaml' will call yolov8-seg.yaml with scale 'n'
+  # [depth, width, max_channels]
+  n: [0.33, 0.25, 1024]
+  s: [0.33, 0.50, 1024]
+  m: [0.67, 0.75, 768]
+  l: [1.00, 1.00, 512]
+  x: [1.00, 1.25, 512]
 
-# YOLOv8.0m backbone
+# YOLOv8.0n backbone
 backbone:
   # [from, repeats, module, args]
   - [-1, 1, Conv, [64, 3, 2]]  # 0-P1/2
   - [-1, 1, Conv, [128, 3, 2]]  # 1-P2/4
   - [-1, 3, C2f, [128, True]]
   - [-1, 1, Conv, [256, 3, 2]]  # 3-P3/8
   - [-1, 6, C2f, [256, True]]
   - [-1, 1, Conv, [512, 3, 2]]  # 5-P4/16
   - [-1, 6, C2f, [512, True]]
-  - [-1, 1, Conv, [768, 3, 2]]  # 7-P5/32
-  - [-1, 3, C2f, [768, True]]
-  - [-1, 1, SPPF, [768, 5]]  # 9
+  - [-1, 1, Conv, [1024, 3, 2]]  # 7-P5/32
+  - [-1, 3, C2f, [1024, True]]
+  - [-1, 1, SPPF, [1024, 5]]  # 9
 
-# YOLOv8.0m head
+# YOLOv8.0n head
 head:
   - [-1, 1, nn.Upsample, [None, 2, 'nearest']]
   - [[-1, 6], 1, Concat, [1]]  # cat backbone P4
-  - [-1, 3, C2f, [512]]  # 13
+  - [-1, 3, C2f, [512]]  # 12
 
   - [-1, 1, nn.Upsample, [None, 2, 'nearest']]
   - [[-1, 4], 1, Concat, [1]]  # cat backbone P3
-  - [-1, 3, C2f, [256]]  # 17 (P3/8-small)
+  - [-1, 3, C2f, [256]]  # 15 (P3/8-small)
 
   - [-1, 1, Conv, [256, 3, 2]]
   - [[-1, 12], 1, Concat, [1]]  # cat head P4
-  - [-1, 3, C2f, [512]]  # 20 (P4/16-medium)
+  - [-1, 3, C2f, [512]]  # 18 (P4/16-medium)
 
   - [-1, 1, Conv, [512, 3, 2]]
   - [[-1, 9], 1, Concat, [1]]  # cat head P5
-  - [-1, 3, C2f, [768]]  # 23 (P5/32-large)
+  - [-1, 3, C2f, [1024]]  # 21 (P5/32-large)
 
-  - [[15, 18, 21], 1, Segment, [nc, 32, 256]]  # Detect(P3, P4, P5)
+  - [[15, 18, 21], 1, Segment, [nc, 32, 256]]  # Segment(P3, P4, P5)
```

### Comparing `ultralytics-8.0.9/ultralytics/models/v8/seg/yolov8n-seg.yaml` & `ultralytics-8.0.90/ultralytics/models/v8/yolov8-p2.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,54 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
+# YOLOv8 object detection model with P2-P5 outputs. For Usage examples see https://docs.ultralytics.com/tasks/detect
 
 # Parameters
 nc: 80  # number of classes
-depth_multiple: 0.33  # scales module repeats
-width_multiple: 0.25  # scales convolution channels
+scales: # model compound scaling constants, i.e. 'model=yolov8n.yaml' will call yolov8.yaml with scale 'n'
+  # [depth, width, max_channels]
+  n: [0.33, 0.25, 1024]
+  s: [0.33, 0.50, 1024]
+  m: [0.67, 0.75, 768]
+  l: [1.00, 1.00, 512]
+  x: [1.00, 1.25, 512]
 
-# YOLOv8.0n backbone
+# YOLOv8.0 backbone
 backbone:
   # [from, repeats, module, args]
   - [-1, 1, Conv, [64, 3, 2]]  # 0-P1/2
   - [-1, 1, Conv, [128, 3, 2]]  # 1-P2/4
   - [-1, 3, C2f, [128, True]]
   - [-1, 1, Conv, [256, 3, 2]]  # 3-P3/8
   - [-1, 6, C2f, [256, True]]
   - [-1, 1, Conv, [512, 3, 2]]  # 5-P4/16
   - [-1, 6, C2f, [512, True]]
   - [-1, 1, Conv, [1024, 3, 2]]  # 7-P5/32
   - [-1, 3, C2f, [1024, True]]
   - [-1, 1, SPPF, [1024, 5]]  # 9
 
-# YOLOv8.0n head
+# YOLOv8.0-p2 head
 head:
   - [-1, 1, nn.Upsample, [None, 2, 'nearest']]
   - [[-1, 6], 1, Concat, [1]]  # cat backbone P4
-  - [-1, 3, C2f, [512]]  # 13
+  - [-1, 3, C2f, [512]]  # 12
 
   - [-1, 1, nn.Upsample, [None, 2, 'nearest']]
   - [[-1, 4], 1, Concat, [1]]  # cat backbone P3
-  - [-1, 3, C2f, [256]]  # 17 (P3/8-small)
+  - [-1, 3, C2f, [256]]  # 15 (P3/8-small)
+
+  - [-1, 1, nn.Upsample, [None, 2, 'nearest']]
+  - [[-1, 2], 1, Concat, [1]]  # cat backbone P2
+  - [-1, 3, C2f, [128]]  # 18 (P2/4-xsmall)
+
+  - [-1, 1, Conv, [128, 3, 2]]
+  - [[-1, 15], 1, Concat, [1]]  # cat head P3
+  - [-1, 3, C2f, [256]]  # 21 (P3/8-small)
 
   - [-1, 1, Conv, [256, 3, 2]]
   - [[-1, 12], 1, Concat, [1]]  # cat head P4
-  - [-1, 3, C2f, [512]]  # 20 (P4/16-medium)
+  - [-1, 3, C2f, [512]]  # 24 (P4/16-medium)
 
   - [-1, 1, Conv, [512, 3, 2]]
   - [[-1, 9], 1, Concat, [1]]  # cat head P5
-  - [-1, 3, C2f, [1024]]  # 23 (P5/32-large)
+  - [-1, 3, C2f, [1024]]  # 27 (P5/32-large)
 
-  - [[15, 18, 21], 1, Segment, [nc, 32, 256]]  # Detect(P3, P4, P5)
+  - [[18, 21, 24, 27], 1, Detect, [nc]]  # Detect(P2, P3, P4, P5)
```

### Comparing `ultralytics-8.0.9/ultralytics/models/v8/seg/yolov8s-seg.yaml` & `ultralytics-8.0.90/ultralytics/models/v5/yolov5.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,49 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
 # Parameters
 nc: 80  # number of classes
-depth_multiple: 0.33  # scales module repeats
-width_multiple: 0.50  # scales convolution channels
+scales: # model compound scaling constants, i.e. 'model=yolov5n.yaml' will call yolov5.yaml with scale 'n'
+  # [depth, width, max_channels]
+  n: [0.33, 0.25, 1024]
+  s: [0.33, 0.50, 1024]
+  m: [0.67, 0.75, 1024]
+  l: [1.00, 1.00, 1024]
+  x: [1.33, 1.25, 1024]
 
-# YOLOv8.0s backbone
+# YOLOv5 v6.0 backbone
 backbone:
-  # [from, repeats, module, args]
-  - [-1, 1, Conv, [64, 3, 2]]  # 0-P1/2
-  - [-1, 1, Conv, [128, 3, 2]]  # 1-P2/4
-  - [-1, 3, C2f, [128, True]]
-  - [-1, 1, Conv, [256, 3, 2]]  # 3-P3/8
-  - [-1, 6, C2f, [256, True]]
-  - [-1, 1, Conv, [512, 3, 2]]  # 5-P4/16
-  - [-1, 6, C2f, [512, True]]
-  - [-1, 1, Conv, [1024, 3, 2]]  # 7-P5/32
-  - [-1, 3, C2f, [1024, True]]
-  - [-1, 1, SPPF, [1024, 5]]  # 9
+  # [from, number, module, args]
+  [[-1, 1, Conv, [64, 6, 2, 2]],  # 0-P1/2
+   [-1, 1, Conv, [128, 3, 2]],  # 1-P2/4
+   [-1, 3, C3, [128]],
+   [-1, 1, Conv, [256, 3, 2]],  # 3-P3/8
+   [-1, 6, C3, [256]],
+   [-1, 1, Conv, [512, 3, 2]],  # 5-P4/16
+   [-1, 9, C3, [512]],
+   [-1, 1, Conv, [1024, 3, 2]],  # 7-P5/32
+   [-1, 3, C3, [1024]],
+   [-1, 1, SPPF, [1024, 5]],  # 9
+  ]
 
-# YOLOv8.0s head
+# YOLOv5 v6.0 head
 head:
-  - [-1, 1, nn.Upsample, [None, 2, 'nearest']]
-  - [[-1, 6], 1, Concat, [1]]  # cat backbone P4
-  - [-1, 3, C2f, [512]]  # 13
-
-  - [-1, 1, nn.Upsample, [None, 2, 'nearest']]
-  - [[-1, 4], 1, Concat, [1]]  # cat backbone P3
-  - [-1, 3, C2f, [256]]  # 17 (P3/8-small)
-
-  - [-1, 1, Conv, [256, 3, 2]]
-  - [[-1, 12], 1, Concat, [1]]  # cat head P4
-  - [-1, 3, C2f, [512]]  # 20 (P4/16-medium)
-
-  - [-1, 1, Conv, [512, 3, 2]]
-  - [[-1, 9], 1, Concat, [1]]  # cat head P5
-  - [-1, 3, C2f, [1024]]  # 23 (P5/32-large)
+  [[-1, 1, Conv, [512, 1, 1]],
+   [-1, 1, nn.Upsample, [None, 2, 'nearest']],
+   [[-1, 6], 1, Concat, [1]],  # cat backbone P4
+   [-1, 3, C3, [512, False]],  # 13
+
+   [-1, 1, Conv, [256, 1, 1]],
+   [-1, 1, nn.Upsample, [None, 2, 'nearest']],
+   [[-1, 4], 1, Concat, [1]],  # cat backbone P3
+   [-1, 3, C3, [256, False]],  # 17 (P3/8-small)
+
+   [-1, 1, Conv, [256, 3, 2]],
+   [[-1, 14], 1, Concat, [1]],  # cat head P4
+   [-1, 3, C3, [512, False]],  # 20 (P4/16-medium)
+
+   [-1, 1, Conv, [512, 3, 2]],
+   [[-1, 10], 1, Concat, [1]],  # cat head P5
+   [-1, 3, C3, [1024, False]],  # 23 (P5/32-large)
 
-  - [[15, 18, 21], 1, Segment, [nc, 32, 256]]  # Detect(P3, P4, P5)
+   [[17, 20, 23], 1, Detect, [nc]],  # Detect(P3, P4, P5)
+  ]
```

### Comparing `ultralytics-8.0.9/ultralytics/nn/autobackend.py` & `ultralytics-8.0.90/ultralytics/nn/autobackend.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,75 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
-
+# Ultralytics YOLO 🚀, AGPL-3.0 license
+import ast
+import contextlib
 import json
 import platform
+import zipfile
 from collections import OrderedDict, namedtuple
 from pathlib import Path
 from urllib.parse import urlparse
 
 import cv2
 import numpy as np
 import torch
 import torch.nn as nn
 from PIL import Image
 
-from ultralytics.yolo.utils import LOGGER, ROOT, yaml_load
-from ultralytics.yolo.utils.checks import check_requirements, check_suffix, check_version
-from ultralytics.yolo.utils.downloads import attempt_download, is_url
+from ultralytics.yolo.utils import LINUX, LOGGER, ROOT, yaml_load
+from ultralytics.yolo.utils.checks import check_requirements, check_suffix, check_version, check_yaml
+from ultralytics.yolo.utils.downloads import attempt_download_asset, is_url
 from ultralytics.yolo.utils.ops import xywh2xyxy
 
 
+def check_class_names(names):
+    """Check class names. Map imagenet class codes to human-readable names if required. Convert lists to dicts."""
+    if isinstance(names, list):  # names is a list
+        names = dict(enumerate(names))  # convert to dict
+    if isinstance(names, dict):
+        # Convert 1) string keys to int, i.e. '0' to 0, and non-string values to strings, i.e. True to 'True'
+        names = {int(k): str(v) for k, v in names.items()}
+        n = len(names)
+        if max(names.keys()) >= n:
+            raise KeyError(f'{n}-class dataset requires class indices 0-{n - 1}, but you have invalid class indices '
+                           f'{min(names.keys())}-{max(names.keys())} defined in your dataset YAML.')
+        if isinstance(names[0], str) and names[0].startswith('n0'):  # imagenet class codes, i.e. 'n01440764'
+            map = yaml_load(ROOT / 'datasets/ImageNet.yaml')['map']  # human-readable names
+            names = {k: map[v] for k, v in names.items()}
+    return names
+
+
 class AutoBackend(nn.Module):
 
-    def __init__(self, weights='yolov8n.pt', device=torch.device('cpu'), dnn=False, data=None, fp16=False, fuse=True):
+    def __init__(self,
+                 weights='yolov8n.pt',
+                 device=torch.device('cpu'),
+                 dnn=False,
+                 data=None,
+                 fp16=False,
+                 fuse=True,
+                 verbose=True):
         """
         MultiBackend class for python inference on various platforms using Ultralytics YOLO.
 
         Args:
             weights (str): The path to the weights file. Default: 'yolov8n.pt'
             device (torch.device): The device to run the model on.
             dnn (bool): Use OpenCV's DNN module for inference if True, defaults to False.
-            data (dict): Additional data, optional
+            data (str), (Path): Additional data.yaml file for class names, optional
             fp16 (bool): If True, use half precision. Default: False
             fuse (bool): Whether to fuse the model or not. Default: True
+            verbose (bool): Whether to run in verbose mode or not. Default: True
 
         Supported formats and their naming conventions:
             | Format                | Suffix           |
             |-----------------------|------------------|
             | PyTorch               | *.pt             |
             | TorchScript           | *.torchscript    |
             | ONNX Runtime          | *.onnx           |
-            | ONNX OpenCV DNN       | *.onnx --dnn     |
+            | ONNX OpenCV DNN       | *.onnx dnn=True  |
             | OpenVINO              | *.xml            |
             | CoreML                | *.mlmodel        |
             | TensorRT              | *.engine         |
             | TensorFlow SavedModel | *_saved_model    |
             | TensorFlow GraphDef   | *.pb             |
             | TensorFlow Lite       | *.tflite         |
             | TensorFlow Edge TPU   | *_edgetpu.tflite |
@@ -51,87 +78,95 @@
         super().__init__()
         w = str(weights[0] if isinstance(weights, list) else weights)
         nn_module = isinstance(weights, torch.nn.Module)
         pt, jit, onnx, xml, engine, coreml, saved_model, pb, tflite, edgetpu, tfjs, paddle, triton = self._model_type(w)
         fp16 &= pt or jit or onnx or engine or nn_module  # FP16
         nhwc = coreml or saved_model or pb or tflite or edgetpu  # BHWC formats (vs torch BCWH)
         stride = 32  # default stride
-        model = None  # TODO: resolves ONNX inference, verify effect on other backends
+        model, metadata = None, None
         cuda = torch.cuda.is_available() and device.type != 'cpu'  # use CUDA
         if not (pt or triton or nn_module):
-            w = attempt_download(w)  # download if not local
+            w = attempt_download_asset(w)  # download if not local
 
         # NOTE: special case: in-memory pytorch model
         if nn_module:
             model = weights.to(device)
-            model = model.fuse() if fuse else model
-            names = model.module.names if hasattr(model, 'module') else model.names  # get class names
+            model = model.fuse(verbose=verbose) if fuse else model
+            if hasattr(model, 'kpt_shape'):
+                kpt_shape = model.kpt_shape  # pose-only
             stride = max(int(model.stride.max()), 32)  # model stride
+            names = model.module.names if hasattr(model, 'module') else model.names  # get class names
             model.half() if fp16 else model.float()
             self.model = model  # explicitly assign for to(), cpu(), cuda(), half()
             pt = True
         elif pt:  # PyTorch
             from ultralytics.nn.tasks import attempt_load_weights
             model = attempt_load_weights(weights if isinstance(weights, list) else w,
                                          device=device,
                                          inplace=True,
                                          fuse=fuse)
+            if hasattr(model, 'kpt_shape'):
+                kpt_shape = model.kpt_shape  # pose-only
             stride = max(int(model.stride.max()), 32)  # model stride
             names = model.module.names if hasattr(model, 'module') else model.names  # get class names
             model.half() if fp16 else model.float()
             self.model = model  # explicitly assign for to(), cpu(), cuda(), half()
         elif jit:  # TorchScript
             LOGGER.info(f'Loading {w} for TorchScript inference...')
             extra_files = {'config.txt': ''}  # model metadata
             model = torch.jit.load(w, _extra_files=extra_files, map_location=device)
             model.half() if fp16 else model.float()
             if extra_files['config.txt']:  # load metadata dict
-                d = json.loads(extra_files['config.txt'],
-                               object_hook=lambda d: {int(k) if k.isdigit() else k: v
-                                                      for k, v in d.items()})
-                stride, names = int(d['stride']), d['names']
+                metadata = json.loads(extra_files['config.txt'], object_hook=lambda x: dict(x.items()))
         elif dnn:  # ONNX OpenCV DNN
             LOGGER.info(f'Loading {w} for ONNX OpenCV DNN inference...')
             check_requirements('opencv-python>=4.5.4')
             net = cv2.dnn.readNetFromONNX(w)
         elif onnx:  # ONNX Runtime
             LOGGER.info(f'Loading {w} for ONNX Runtime inference...')
             check_requirements(('onnx', 'onnxruntime-gpu' if cuda else 'onnxruntime'))
             import onnxruntime
             providers = ['CUDAExecutionProvider', 'CPUExecutionProvider'] if cuda else ['CPUExecutionProvider']
             session = onnxruntime.InferenceSession(w, providers=providers)
             output_names = [x.name for x in session.get_outputs()]
-            meta = session.get_modelmeta().custom_metadata_map  # metadata
-            if 'stride' in meta:
-                stride, names = int(meta['stride']), eval(meta['names'])
+            metadata = session.get_modelmeta().custom_metadata_map  # metadata
         elif xml:  # OpenVINO
             LOGGER.info(f'Loading {w} for OpenVINO inference...')
             check_requirements('openvino')  # requires openvino-dev: https://pypi.org/project/openvino-dev/
             from openvino.runtime import Core, Layout, get_batch  # noqa
             ie = Core()
-            if not Path(w).is_file():  # if not *.xml
-                w = next(Path(w).glob('*.xml'))  # get *.xml file from *_openvino_model dir
-            network = ie.read_model(model=w, weights=Path(w).with_suffix('.bin'))
+            w = Path(w)
+            if not w.is_file():  # if not *.xml
+                w = next(w.glob('*.xml'))  # get *.xml file from *_openvino_model dir
+            network = ie.read_model(model=str(w), weights=w.with_suffix('.bin'))
             if network.get_parameters()[0].get_layout().empty:
-                network.get_parameters()[0].set_layout(Layout("NCHW"))
+                network.get_parameters()[0].set_layout(Layout('NCHW'))
             batch_dim = get_batch(network)
             if batch_dim.is_static:
                 batch_size = batch_dim.get_length()
-            executable_network = ie.compile_model(network, device_name="CPU")  # device_name="MYRIAD" for Intel NCS2
-            stride, names = self._load_metadata(Path(w).with_suffix('.yaml'))  # load metadata
+            executable_network = ie.compile_model(network, device_name='CPU')  # device_name="MYRIAD" for NCS2
+            metadata = w.parent / 'metadata.yaml'
         elif engine:  # TensorRT
             LOGGER.info(f'Loading {w} for TensorRT inference...')
-            import tensorrt as trt  # https://developer.nvidia.com/nvidia-tensorrt-download
+            try:
+                import tensorrt as trt  # noqa https://developer.nvidia.com/nvidia-tensorrt-download
+            except ImportError:
+                if LINUX:
+                    check_requirements('nvidia-tensorrt', cmds='-U --index-url https://pypi.ngc.nvidia.com')
+                import tensorrt as trt  # noqa
             check_version(trt.__version__, '7.0.0', hard=True)  # require tensorrt>=7.0.0
             if device.type == 'cpu':
                 device = torch.device('cuda:0')
             Binding = namedtuple('Binding', ('name', 'dtype', 'shape', 'data', 'ptr'))
             logger = trt.Logger(trt.Logger.INFO)
+            # Read file
             with open(w, 'rb') as f, trt.Runtime(logger) as runtime:
-                model = runtime.deserialize_cuda_engine(f.read())
+                meta_len = int.from_bytes(f.read(4), byteorder='little')  # read metadata length
+                metadata = json.loads(f.read(meta_len).decode('utf-8'))  # read metadata
+                model = runtime.deserialize_cuda_engine(f.read())  # read engine
             context = model.create_execution_context()
             bindings = OrderedDict()
             output_names = []
             fp16 = False  # default updated below
             dynamic = False
             for i in range(model.num_bindings):
                 name = model.get_binding_name(i)
@@ -149,104 +184,128 @@
                 bindings[name] = Binding(name, dtype, shape, im, int(im.data_ptr()))
             binding_addrs = OrderedDict((n, d.ptr) for n, d in bindings.items())
             batch_size = bindings['images'].shape[0]  # if dynamic, this is instead max batch size
         elif coreml:  # CoreML
             LOGGER.info(f'Loading {w} for CoreML inference...')
             import coremltools as ct
             model = ct.models.MLModel(w)
+            metadata = dict(model.user_defined_metadata)
         elif saved_model:  # TF SavedModel
             LOGGER.info(f'Loading {w} for TensorFlow SavedModel inference...')
             import tensorflow as tf
             keras = False  # assume TF1 saved_model
             model = tf.keras.models.load_model(w) if keras else tf.saved_model.load(w)
+            metadata = Path(w) / 'metadata.yaml'
         elif pb:  # GraphDef https://www.tensorflow.org/guide/migrate#a_graphpb_or_graphpbtxt
             LOGGER.info(f'Loading {w} for TensorFlow GraphDef inference...')
             import tensorflow as tf
 
+            from ultralytics.yolo.engine.exporter import gd_outputs
+
             def wrap_frozen_graph(gd, inputs, outputs):
-                x = tf.compat.v1.wrap_function(lambda: tf.compat.v1.import_graph_def(gd, name=""), [])  # wrapped
+                """Wrap frozen graphs for deployment."""
+                x = tf.compat.v1.wrap_function(lambda: tf.compat.v1.import_graph_def(gd, name=''), [])  # wrapped
                 ge = x.graph.as_graph_element
                 return x.prune(tf.nest.map_structure(ge, inputs), tf.nest.map_structure(ge, outputs))
 
-            def gd_outputs(gd):
-                name_list, input_list = [], []
-                for node in gd.node:  # tensorflow.core.framework.node_def_pb2.NodeDef
-                    name_list.append(node.name)
-                    input_list.extend(node.input)
-                return sorted(f'{x}:0' for x in list(set(name_list) - set(input_list)) if not x.startswith('NoOp'))
-
             gd = tf.Graph().as_graph_def()  # TF GraphDef
             with open(w, 'rb') as f:
                 gd.ParseFromString(f.read())
-            frozen_func = wrap_frozen_graph(gd, inputs="x:0", outputs=gd_outputs(gd))
+            frozen_func = wrap_frozen_graph(gd, inputs='x:0', outputs=gd_outputs(gd))
         elif tflite or edgetpu:  # https://www.tensorflow.org/lite/guide/python#install_tensorflow_lite_for_python
             try:  # https://coral.ai/docs/edgetpu/tflite-python/#update-existing-tf-lite-code-for-the-edge-tpu
                 from tflite_runtime.interpreter import Interpreter, load_delegate
             except ImportError:
                 import tensorflow as tf
-                Interpreter, load_delegate = tf.lite.Interpreter, tf.lite.experimental.load_delegate,
+                Interpreter, load_delegate = tf.lite.Interpreter, tf.lite.experimental.load_delegate
             if edgetpu:  # TF Edge TPU https://coral.ai/software/#edgetpu-runtime
                 LOGGER.info(f'Loading {w} for TensorFlow Lite Edge TPU inference...')
                 delegate = {
                     'Linux': 'libedgetpu.so.1',
                     'Darwin': 'libedgetpu.1.dylib',
                     'Windows': 'edgetpu.dll'}[platform.system()]
                 interpreter = Interpreter(model_path=w, experimental_delegates=[load_delegate(delegate)])
             else:  # TFLite
                 LOGGER.info(f'Loading {w} for TensorFlow Lite inference...')
                 interpreter = Interpreter(model_path=w)  # load TFLite model
             interpreter.allocate_tensors()  # allocate
             input_details = interpreter.get_input_details()  # inputs
             output_details = interpreter.get_output_details()  # outputs
+            # Load metadata
+            with contextlib.suppress(zipfile.BadZipFile):
+                with zipfile.ZipFile(w, 'r') as model:
+                    meta_file = model.namelist()[0]
+                    metadata = ast.literal_eval(model.read(meta_file).decode('utf-8'))
         elif tfjs:  # TF.js
-            raise NotImplementedError('ERROR: YOLOv8 TF.js inference is not supported')
+            raise NotImplementedError('YOLOv8 TF.js inference is not supported')
         elif paddle:  # PaddlePaddle
             LOGGER.info(f'Loading {w} for PaddlePaddle inference...')
             check_requirements('paddlepaddle-gpu' if cuda else 'paddlepaddle')
-            import paddle.inference as pdi
-            if not Path(w).is_file():  # if not *.pdmodel
-                w = next(Path(w).rglob('*.pdmodel'))  # get *.xml file from *_openvino_model dir
-            weights = Path(w).with_suffix('.pdiparams')
-            config = pdi.Config(str(w), str(weights))
+            import paddle.inference as pdi  # noqa
+            w = Path(w)
+            if not w.is_file():  # if not *.pdmodel
+                w = next(w.rglob('*.pdmodel'))  # get *.pdmodel file from *_paddle_model dir
+            config = pdi.Config(str(w), str(w.with_suffix('.pdiparams')))
             if cuda:
                 config.enable_use_gpu(memory_pool_init_size_mb=2048, device_id=0)
             predictor = pdi.create_predictor(config)
             input_handle = predictor.get_input_handle(predictor.get_input_names()[0])
             output_names = predictor.get_output_names()
+            metadata = w.parents[1] / 'metadata.yaml'
         elif triton:  # NVIDIA Triton Inference Server
             LOGGER.info('Triton Inference Server not supported...')
             '''
             TODO:
             check_requirements('tritonclient[all]')
             from utils.triton import TritonRemoteModel
             model = TritonRemoteModel(url=w)
             nhwc = model.runtime.startswith("tensorflow")
             '''
         else:
-            raise NotImplementedError(f'ERROR: {w} is not a supported format')
-
-        # class names
-        if 'names' not in locals():
-            names = yaml_load(data)['names'] if data else {i: f'class{i}' for i in range(999)}
-        if names[0] == 'n01440764' and len(names) == 1000:  # ImageNet
-            names = yaml_load(ROOT / 'yolo/data/datasets/ImageNet.yaml')['names']  # human-readable names
+            from ultralytics.yolo.engine.exporter import export_formats
+            raise TypeError(f"model='{w}' is not a supported model format. "
+                            'See https://docs.ultralytics.com/modes/predict for help.'
+                            f'\n\n{export_formats()}')
+
+        # Load external metadata YAML
+        if isinstance(metadata, (str, Path)) and Path(metadata).exists():
+            metadata = yaml_load(metadata)
+        if metadata:
+            for k, v in metadata.items():
+                if k in ('stride', 'batch'):
+                    metadata[k] = int(v)
+                elif k in ('imgsz', 'names', 'kpt_shape') and isinstance(v, str):
+                    metadata[k] = eval(v)
+            stride = metadata['stride']
+            task = metadata['task']
+            batch = metadata['batch']
+            imgsz = metadata['imgsz']
+            names = metadata['names']
+            kpt_shape = metadata.get('kpt_shape')
+        elif not (pt or triton or nn_module):
+            LOGGER.warning(f"WARNING ⚠️ Metadata not found for 'model={weights}'")
+
+        # Check names
+        if 'names' not in locals():  # names missing
+            names = self._apply_default_class_names(data)
+        names = check_class_names(names)
 
         self.__dict__.update(locals())  # assign all variables to self
 
     def forward(self, im, augment=False, visualize=False):
         """
         Runs inference on the YOLOv8 MultiBackend model.
 
         Args:
             im (torch.Tensor): The image tensor to perform inference on.
             augment (bool): whether to perform data augmentation during inference, defaults to False
             visualize (bool): whether to visualize the output predictions, defaults to False
 
         Returns:
-            (tuple): Tuple containing the raw output tensor, and the processed output for visualization (if visualize=True)
+            (tuple): Tuple containing the raw output tensor, and processed output for visualization (if visualize=True)
         """
         b, ch, h, w = im.shape  # batch, channel, height, width
         if self.fp16 and im.dtype != torch.float16:
             im = im.half()  # to FP16
         if self.nhwc:
             im = im.permute(0, 2, 3, 1)  # torch BCHW to numpy BHWC shape(1,320,192,3)
 
@@ -274,55 +333,70 @@
                     self.bindings[name].data.resize_(tuple(self.context.get_binding_shape(i)))
             s = self.bindings['images'].shape
             assert im.shape == s, f"input size {im.shape} {'>' if self.dynamic else 'not equal to'} max model size {s}"
             self.binding_addrs['images'] = int(im.data_ptr())
             self.context.execute_v2(list(self.binding_addrs.values()))
             y = [self.bindings[x].data for x in sorted(self.output_names)]
         elif self.coreml:  # CoreML
-            im = im.cpu().numpy()
-            im = Image.fromarray((im[0] * 255).astype('uint8'))
+            im = im[0].cpu().numpy()
+            im_pil = Image.fromarray((im * 255).astype('uint8'))
             # im = im.resize((192, 320), Image.ANTIALIAS)
-            y = self.model.predict({'image': im})  # coordinates are xywh normalized
+            y = self.model.predict({'image': im_pil})  # coordinates are xywh normalized
             if 'confidence' in y:
                 box = xywh2xyxy(y['coordinates'] * [[w, h, w, h]])  # xyxy pixels
                 conf, cls = y['confidence'].max(1), y['confidence'].argmax(1).astype(np.float)
                 y = np.concatenate((box, conf.reshape(-1, 1), cls.reshape(-1, 1)), 1)
-            else:
+            elif len(y) == 1:  # classification model
+                y = list(y.values())
+            elif len(y) == 2:  # segmentation model
                 y = list(reversed(y.values()))  # reversed for segmentation models (pred, proto)
         elif self.paddle:  # PaddlePaddle
             im = im.cpu().numpy().astype(np.float32)
             self.input_handle.copy_from_cpu(im)
             self.predictor.run()
             y = [self.predictor.get_output_handle(x).copy_to_cpu() for x in self.output_names]
         elif self.triton:  # NVIDIA Triton Inference Server
             y = self.model(im)
         else:  # TensorFlow (SavedModel, GraphDef, Lite, Edge TPU)
             im = im.cpu().numpy()
             if self.saved_model:  # SavedModel
                 y = self.model(im, training=False) if self.keras else self.model(im)
+                if not isinstance(y, list):
+                    y = [y]
             elif self.pb:  # GraphDef
                 y = self.frozen_func(x=self.tf.constant(im))
+                if len(y) == 2 and len(self.names) == 999:  # segments and names not defined
+                    ip, ib = (0, 1) if len(y[0].shape) == 4 else (1, 0)  # index of protos, boxes
+                    nc = y[ib].shape[1] - y[ip].shape[3] - 4  # y = (1, 160, 160, 32), (1, 116, 8400)
+                    self.names = {i: f'class{i}' for i in range(nc)}
             else:  # Lite or Edge TPU
                 input = self.input_details[0]
-                int8 = input['dtype'] == np.uint8  # is TFLite quantized uint8 model
+                int8 = input['dtype'] == np.int8  # is TFLite quantized int8 model
                 if int8:
                     scale, zero_point = input['quantization']
-                    im = (im / scale + zero_point).astype(np.uint8)  # de-scale
+                    im = (im / scale + zero_point).astype(np.int8)  # de-scale
                 self.interpreter.set_tensor(input['index'], im)
                 self.interpreter.invoke()
                 y = []
                 for output in self.output_details:
                     x = self.interpreter.get_tensor(output['index'])
                     if int8:
                         scale, zero_point = output['quantization']
                         x = (x.astype(np.float32) - zero_point) * scale  # re-scale
                     y.append(x)
+            # TF segment fixes: export is reversed vs ONNX export and protos are transposed
+            if len(y) == 2:  # segment with (det, proto) output order reversed
+                if len(y[1].shape) != 4:
+                    y = list(reversed(y))  # should be y = (1, 116, 8400), (1, 160, 160, 32)
+                y[1] = np.transpose(y[1], (0, 3, 1, 2))  # should be y = (1, 116, 8400), (1, 32, 160, 160)
             y = [x if isinstance(x, np.ndarray) else x.numpy() for x in y]
-            y[0][..., :4] *= [w, h, w, h]  # xywh normalized to pixels
+            # y[0][..., :4] *= [w, h, w, h]  # xywh normalized to pixels
 
+        # for x in y:
+        #     print(type(x), len(x)) if isinstance(x, (list, tuple)) else print(type(x), x.shape)  # debug shapes
         if isinstance(y, (list, tuple)):
             return self.from_numpy(y[0]) if len(y) == 1 else [self.from_numpy(x) for x in y]
         else:
             return self.from_numpy(y)
 
     def from_numpy(self, x):
         """
@@ -330,15 +404,15 @@
 
          Args:
              x (np.ndarray): The array to be converted.
 
          Returns:
              (torch.Tensor): The converted tensor
          """
-        return torch.from_numpy(x).to(self.device) if isinstance(x, np.ndarray) else x
+        return torch.tensor(x).to(self.device) if isinstance(x, np.ndarray) else x
 
     def warmup(self, imgsz=(1, 3, 640, 640)):
         """
         Warm up the model by running one forward pass with a dummy input.
 
         Args:
             imgsz (tuple): The shape of the dummy input tensor in the format (batch_size, channels, height, width)
@@ -349,14 +423,21 @@
         warmup_types = self.pt, self.jit, self.onnx, self.engine, self.saved_model, self.pb, self.triton, self.nn_module
         if any(warmup_types) and (self.device.type != 'cpu' or self.triton):
             im = torch.empty(*imgsz, dtype=torch.half if self.fp16 else torch.float, device=self.device)  # input
             for _ in range(2 if self.jit else 1):  #
                 self.forward(im)  # warmup
 
     @staticmethod
+    def _apply_default_class_names(data):
+        """Applies default class names to an input YAML file or returns numerical class names."""
+        with contextlib.suppress(Exception):
+            return yaml_load(check_yaml(data))['names']
+        return {i: f'class{i}' for i in range(999)}  # return default if above errors
+
+    @staticmethod
     def _model_type(p='path/to/model.pt'):
         """
         This function takes a path to a model file and returns the model type
 
         Args:
             p: path to the model file. Defaults to path/to/model.pt
         """
@@ -365,24 +446,9 @@
         from ultralytics.yolo.engine.exporter import export_formats
         sf = list(export_formats().Suffix)  # export suffixes
         if not is_url(p, check=False) and not isinstance(p, str):
             check_suffix(p, sf)  # checks
         url = urlparse(p)  # if url may be Triton inference server
         types = [s in Path(p).name for s in sf]
         types[8] &= not types[9]  # tflite &= not edgetpu
-        triton = not any(types) and all([any(s in url.scheme for s in ["http", "grpc"]), url.netloc])
+        triton = not any(types) and all([any(s in url.scheme for s in ['http', 'grpc']), url.netloc])
         return types + [triton]
-
-    @staticmethod
-    def _load_metadata(f=Path('path/to/meta.yaml')):
-        """
-        Loads the metadata from a yaml file
-
-        Args:
-            f: The path to the metadata file.
-        """
-
-        # Load metadata from meta.yaml if it exists
-        if f.exists():
-            d = yaml_load(f)
-            return d['stride'], d['names']  # assign stride, names
-        return None, None
```

### Comparing `ultralytics-8.0.9/ultralytics/nn/autoshape.py` & `ultralytics-8.0.90/ultralytics/nn/autoshape.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 """
 Common modules
 """
 
 from copy import copy
 from pathlib import Path
 
 import cv2
 import numpy as np
-import pandas as pd
 import requests
 import torch
 import torch.nn as nn
 from PIL import Image, ImageOps
 from torch.cuda import amp
 
 from ultralytics.nn.autobackend import AutoBackend
@@ -21,50 +20,51 @@
 from ultralytics.yolo.utils.files import increment_path
 from ultralytics.yolo.utils.ops import Profile, make_divisible, non_max_suppression, scale_boxes, xyxy2xywh
 from ultralytics.yolo.utils.plotting import Annotator, colors, save_one_box
 from ultralytics.yolo.utils.torch_utils import copy_attr, smart_inference_mode
 
 
 class AutoShape(nn.Module):
-    # YOLOv8 input-robust model wrapper for passing cv2/np/PIL/torch inputs. Includes preprocessing, inference and NMS
+    """YOLOv8 input-robust model wrapper for passing cv2/np/PIL/torch inputs. Includes preprocessing, inference and NMS."""
     conf = 0.25  # NMS confidence threshold
     iou = 0.45  # NMS IoU threshold
     agnostic = False  # NMS class-agnostic
     multi_label = False  # NMS multiple labels per box
     classes = None  # (optional list) filter by class, i.e. = [0, 15, 16] for COCO persons, cats and dogs
     max_det = 1000  # maximum number of detections per image
     amp = False  # Automatic Mixed Precision (AMP) inference
 
     def __init__(self, model, verbose=True):
+        """Initializes object and copies attributes from model object."""
         super().__init__()
         if verbose:
             LOGGER.info('Adding AutoShape... ')
         copy_attr(self, model, include=('yaml', 'nc', 'hyp', 'names', 'stride', 'abc'), exclude=())  # copy attributes
         self.dmb = isinstance(model, AutoBackend)  # DetectMultiBackend() instance
         self.pt = not self.dmb or model.pt  # PyTorch model
         self.model = model.eval()
         if self.pt:
             m = self.model.model.model[-1] if self.dmb else self.model.model[-1]  # Detect()
             m.inplace = False  # Detect.inplace=False for safe multithread inference
             m.export = True  # do not output loss values
 
     def _apply(self, fn):
-        # Apply to(), cpu(), cuda(), half() to model tensors that are not parameters or registered buffers
+        """Apply to(), cpu(), cuda(), half() to model tensors that are not parameters or registered buffers."""
         self = super()._apply(fn)
         if self.pt:
             m = self.model.model.model[-1] if self.dmb else self.model.model[-1]  # Detect()
             m.stride = fn(m.stride)
             m.grid = list(map(fn, m.grid))
             if isinstance(m.anchor_grid, list):
                 m.anchor_grid = list(map(fn, m.anchor_grid))
         return self
 
     @smart_inference_mode()
     def forward(self, ims, size=640, augment=False, profile=False):
-        # Inference from various sources. For size(height=640, width=1280), RGB images example inputs are:
+        """Inference from various sources. For size(height=640, width=1280), RGB images example inputs are:."""
         #   file:        ims = 'data/images/zidane.jpg'  # str or PosixPath
         #   URI:             = 'https://ultralytics.com/images/zidane.jpg'
         #   OpenCV:          = cv2.imread('image.jpg')[:,:,::-1]  # HWC BGR to RGB x(640,1280,3)
         #   PIL:             = Image.open('image.jpg') or ImageGrab.grab()  # HWC x(640,1280,3)
         #   numpy:           = np.zeros((640,1280,3))  # HWC
         #   torch:           = torch.zeros(16,3,320,640)  # BCHW (scaled to size=640, 0-1 values)
         #   multiple:        = [Image.open('image1.jpg'), Image.open('image2.jpg'), ...]  # list of images
@@ -75,15 +75,15 @@
                 size = (size, size)
             p = next(self.model.parameters()) if self.pt else torch.empty(1, device=self.model.device)  # param
             autocast = self.amp and (p.device.type != 'cpu')  # Automatic Mixed Precision (AMP) inference
             if isinstance(ims, torch.Tensor):  # torch
                 with amp.autocast(autocast):
                     return self.model(ims.to(p.device).type_as(p), augment=augment)  # inference
 
-            # Pre-process
+            # Preprocess
             n, ims = (len(ims), list(ims)) if isinstance(ims, (list, tuple)) else (1, [ims])  # number, list of images
             shape0, shape1, files = [], [], []  # image and inference shapes, filenames
             for i, im in enumerate(ims):
                 f = f'image{i}'  # filename
                 if isinstance(im, (str, Path)):  # filename or uri
                     im, f = Image.open(requests.get(im, stream=True).raw if str(im).startswith('http') else im), im
                     im = np.asarray(ImageOps.exif_transpose(im))
@@ -95,24 +95,24 @@
                 im = im[..., :3] if im.ndim == 3 else cv2.cvtColor(im, cv2.COLOR_GRAY2BGR)  # enforce 3ch input
                 s = im.shape[:2]  # HWC
                 shape0.append(s)  # image shape
                 g = max(size) / max(s)  # gain
                 shape1.append([y * g for y in s])
                 ims[i] = im if im.data.contiguous else np.ascontiguousarray(im)  # update
             shape1 = [make_divisible(x, self.stride) for x in np.array(shape1).max(0)] if self.pt else size  # inf shape
-            x = [LetterBox(shape1, auto=False)(image=im)["img"] for im in ims]  # pad
+            x = [LetterBox(shape1, auto=False)(image=im)['img'] for im in ims]  # pad
             x = np.ascontiguousarray(np.array(x).transpose((0, 3, 1, 2)))  # stack and BHWC to BCHW
             x = torch.from_numpy(x).to(p.device).type_as(p) / 255  # uint8 to fp16/32
 
         with amp.autocast(autocast):
             # Inference
             with dt[1]:
                 y = self.model(x, augment=augment)  # forward
 
-            # Post-process
+            # Postprocess
             with dt[2]:
                 y = non_max_suppression(y if self.dmb else y[0],
                                         self.conf,
                                         self.iou,
                                         self.classes,
                                         self.agnostic,
                                         self.multi_label,
@@ -122,14 +122,15 @@
 
             return Detections(ims, y, files, dt, self.names, x.shape)
 
 
 class Detections:
     # YOLOv8 detections class for inference results
     def __init__(self, ims, pred, files, times=(0, 0, 0), names=None, shape=None):
+        """Initialize object attributes for YOLO detection results."""
         super().__init__()
         d = pred[0].device  # device
         gn = [torch.tensor([*(im.shape[i] for i in [1, 0, 1, 0]), 1, 1], device=d) for im in ims]  # normalizations
         self.ims = ims  # list of images as numpy arrays
         self.pred = pred  # list of tensors pred[0] = (xyxy, conf, cls)
         self.names = names  # class names
         self.files = files  # image filenames
@@ -139,14 +140,15 @@
         self.xyxyn = [x / g for x, g in zip(self.xyxy, gn)]  # xyxy normalized
         self.xywhn = [x / g for x, g in zip(self.xywh, gn)]  # xywh normalized
         self.n = len(self.pred)  # number of images (batch size)
         self.t = tuple(x.t / self.n * 1E3 for x in times)  # timestamps (ms)
         self.s = tuple(shape)  # inference BCHW shape
 
     def _run(self, pprint=False, show=False, save=False, crop=False, render=False, labels=True, save_dir=Path('')):
+        """Return performance metrics and optionally cropped/save images or results."""
         s, crops = '', []
         for i, (im, pred) in enumerate(zip(self.ims, self.pred)):
             s += f'\nimage {i + 1}/{len(self.pred)}: {im.shape[0]}x{im.shape[1]} '  # string
             if pred.shape[0]:
                 for c in pred[:, -1].unique():
                     n = (pred[:, -1] == c).sum()  # detections per class
                     s += f"{n} {self.names[int(c)]}{'s' * (n > 1)}, "  # add to string
@@ -177,61 +179,65 @@
                 im.save(save_dir / f)  # save
                 if i == self.n - 1:
                     LOGGER.info(f"Saved {self.n} image{'s' * (self.n > 1)} to {colorstr('bold', save_dir)}")
             if render:
                 self.ims[i] = np.asarray(im)
         if pprint:
             s = s.lstrip('\n')
-            return f'{s}\nSpeed: %.1fms pre-process, %.1fms inference, %.1fms NMS per image at shape {self.s}' % self.t
+            return f'{s}\nSpeed: %.1fms preprocess, %.1fms inference, %.1fms NMS per image at shape {self.s}' % self.t
         if crop:
             if save:
                 LOGGER.info(f'Saved results to {save_dir}\n')
             return crops
 
     def show(self, labels=True):
+        """Displays YOLO results with detected bounding boxes."""
         self._run(show=True, labels=labels)  # show results
 
     def save(self, labels=True, save_dir='runs/detect/exp', exist_ok=False):
+        """Save detection results with optional labels to specified directory."""
         save_dir = increment_path(save_dir, exist_ok, mkdir=True)  # increment save_dir
         self._run(save=True, labels=labels, save_dir=save_dir)  # save results
 
     def crop(self, save=True, save_dir='runs/detect/exp', exist_ok=False):
+        """Crops images into detections and saves them if 'save' is True."""
         save_dir = increment_path(save_dir, exist_ok, mkdir=True) if save else None
         return self._run(crop=True, save=save, save_dir=save_dir)  # crop results
 
     def render(self, labels=True):
+        """Renders detected objects and returns images."""
         self._run(render=True, labels=labels)  # render results
         return self.ims
 
     def pandas(self):
-        # return detections as pandas DataFrames, i.e. print(results.pandas().xyxy[0])
+        """Return detections as pandas DataFrames, i.e. print(results.pandas().xyxy[0])."""
+        import pandas
         new = copy(self)  # return copy
         ca = 'xmin', 'ymin', 'xmax', 'ymax', 'confidence', 'class', 'name'  # xyxy columns
         cb = 'xcenter', 'ycenter', 'width', 'height', 'confidence', 'class', 'name'  # xywh columns
         for k, c in zip(['xyxy', 'xyxyn', 'xywh', 'xywhn'], [ca, ca, cb, cb]):
             a = [[x[:5] + [int(x[5]), self.names[int(x[5])]] for x in x.tolist()] for x in getattr(self, k)]  # update
-            setattr(new, k, [pd.DataFrame(x, columns=c) for x in a])
+            setattr(new, k, [pandas.DataFrame(x, columns=c) for x in a])
         return new
 
     def tolist(self):
-        # return a list of Detections objects, i.e. 'for result in results.tolist():'
+        """Return a list of Detections objects, i.e. 'for result in results.tolist():'."""
         r = range(self.n)  # iterable
         x = [Detections([self.ims[i]], [self.pred[i]], [self.files[i]], self.times, self.names, self.s) for i in r]
         # for d in x:
         #    for k in ['ims', 'pred', 'xyxy', 'xyxyn', 'xywh', 'xywhn']:
         #        setattr(d, k, getattr(d, k)[0])  # pop out of list
         return x
 
     def print(self):
+        """Print the results of the `self._run()` function."""
         LOGGER.info(self.__str__())
 
     def __len__(self):  # override len(results)
         return self.n
 
     def __str__(self):  # override print(results)
         return self._run(pprint=True)  # print results
 
     def __repr__(self):
+        """Returns a printable representation of the object."""
         return f'YOLOv8 {self.__class__} instance\n' + self.__str__()
-
-
-print('works')
```

### Comparing `ultralytics-8.0.9/ultralytics/nn/modules.py` & `ultralytics-8.0.90/ultralytics/nn/modules.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,461 +1,616 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 """
 Common modules
 """
 
 import math
-import warnings
 
 import torch
 import torch.nn as nn
 
 from ultralytics.yolo.utils.tal import dist2bbox, make_anchors
 
 
 def autopad(k, p=None, d=1):  # kernel, padding, dilation
-    # Pad to 'same' shape outputs
+    """Pad to 'same' shape outputs."""
     if d > 1:
         k = d * (k - 1) + 1 if isinstance(k, int) else [d * (x - 1) + 1 for x in k]  # actual kernel-size
     if p is None:
         p = k // 2 if isinstance(k, int) else [x // 2 for x in k]  # auto-pad
     return p
 
 
 class Conv(nn.Module):
-    # Standard convolution with args(ch_in, ch_out, kernel, stride, padding, groups, dilation, activation)
+    """Standard convolution with args(ch_in, ch_out, kernel, stride, padding, groups, dilation, activation)."""
     default_act = nn.SiLU()  # default activation
 
     def __init__(self, c1, c2, k=1, s=1, p=None, g=1, d=1, act=True):
+        """Initialize Conv layer with given arguments including activation."""
         super().__init__()
         self.conv = nn.Conv2d(c1, c2, k, s, autopad(k, p, d), groups=g, dilation=d, bias=False)
         self.bn = nn.BatchNorm2d(c2)
         self.act = self.default_act if act is True else act if isinstance(act, nn.Module) else nn.Identity()
 
     def forward(self, x):
+        """Apply convolution, batch normalization and activation to input tensor."""
         return self.act(self.bn(self.conv(x)))
 
     def forward_fuse(self, x):
+        """Perform transposed convolution of 2D data."""
         return self.act(self.conv(x))
 
 
 class DWConv(Conv):
-    # Depth-wise convolution
+    """Depth-wise convolution."""
+
     def __init__(self, c1, c2, k=1, s=1, d=1, act=True):  # ch_in, ch_out, kernel, stride, dilation, activation
         super().__init__(c1, c2, k, s, g=math.gcd(c1, c2), d=d, act=act)
 
 
 class DWConvTranspose2d(nn.ConvTranspose2d):
-    # Depth-wise transpose convolution
+    """Depth-wise transpose convolution."""
+
     def __init__(self, c1, c2, k=1, s=1, p1=0, p2=0):  # ch_in, ch_out, kernel, stride, padding, padding_out
         super().__init__(c1, c2, k, s, p1, p2, groups=math.gcd(c1, c2))
 
 
 class ConvTranspose(nn.Module):
-    # Convolution transpose 2d layer
+    """Convolution transpose 2d layer."""
     default_act = nn.SiLU()  # default activation
 
     def __init__(self, c1, c2, k=2, s=2, p=0, bn=True, act=True):
+        """Initialize ConvTranspose2d layer with batch normalization and activation function."""
         super().__init__()
         self.conv_transpose = nn.ConvTranspose2d(c1, c2, k, s, p, bias=not bn)
         self.bn = nn.BatchNorm2d(c2) if bn else nn.Identity()
         self.act = self.default_act if act is True else act if isinstance(act, nn.Module) else nn.Identity()
 
     def forward(self, x):
+        """Applies transposed convolutions, batch normalization and activation to input."""
         return self.act(self.bn(self.conv_transpose(x)))
 
+    def forward_fuse(self, x):
+        """Applies activation and convolution transpose operation to input."""
+        return self.act(self.conv_transpose(x))
+
 
 class DFL(nn.Module):
-    # Integral module of Distribution Focal Loss (DFL) proposed in Generalized Focal Loss https://ieeexplore.ieee.org/document/9792391
+    """
+    Integral module of Distribution Focal Loss (DFL).
+    Proposed in Generalized Focal Loss https://ieeexplore.ieee.org/document/9792391
+    """
+
     def __init__(self, c1=16):
+        """Initialize a convolutional layer with a given number of input channels."""
         super().__init__()
         self.conv = nn.Conv2d(c1, 1, 1, bias=False).requires_grad_(False)
         x = torch.arange(c1, dtype=torch.float)
         self.conv.weight.data[:] = nn.Parameter(x.view(1, c1, 1, 1))
         self.c1 = c1
 
     def forward(self, x):
+        """Applies a transformer layer on input tensor 'x' and returns a tensor."""
         b, c, a = x.shape  # batch, channels, anchors
         return self.conv(x.view(b, 4, self.c1, a).transpose(2, 1).softmax(1)).view(b, 4, a)
         # return self.conv(x.view(b, self.c1, 4, a).softmax(1)).view(b, 4, a)
 
 
 class TransformerLayer(nn.Module):
-    # Transformer layer https://arxiv.org/abs/2010.11929 (LayerNorm layers removed for better performance)
+    """Transformer layer https://arxiv.org/abs/2010.11929 (LayerNorm layers removed for better performance)."""
+
     def __init__(self, c, num_heads):
+        """Initializes a self-attention mechanism using linear transformations and multi-head attention."""
         super().__init__()
         self.q = nn.Linear(c, c, bias=False)
         self.k = nn.Linear(c, c, bias=False)
         self.v = nn.Linear(c, c, bias=False)
         self.ma = nn.MultiheadAttention(embed_dim=c, num_heads=num_heads)
         self.fc1 = nn.Linear(c, c, bias=False)
         self.fc2 = nn.Linear(c, c, bias=False)
 
     def forward(self, x):
+        """Apply a transformer block to the input x and return the output."""
         x = self.ma(self.q(x), self.k(x), self.v(x))[0] + x
         x = self.fc2(self.fc1(x)) + x
         return x
 
 
 class TransformerBlock(nn.Module):
-    # Vision Transformer https://arxiv.org/abs/2010.11929
+    """Vision Transformer https://arxiv.org/abs/2010.11929."""
+
     def __init__(self, c1, c2, num_heads, num_layers):
+        """Initialize a Transformer module with position embedding and specified number of heads and layers."""
         super().__init__()
         self.conv = None
         if c1 != c2:
             self.conv = Conv(c1, c2)
         self.linear = nn.Linear(c2, c2)  # learnable position embedding
         self.tr = nn.Sequential(*(TransformerLayer(c2, num_heads) for _ in range(num_layers)))
         self.c2 = c2
 
     def forward(self, x):
+        """Forward propagates the input through the bottleneck module."""
         if self.conv is not None:
             x = self.conv(x)
         b, _, w, h = x.shape
         p = x.flatten(2).permute(2, 0, 1)
         return self.tr(p + self.linear(p)).permute(1, 2, 0).reshape(b, self.c2, w, h)
 
 
 class Bottleneck(nn.Module):
-    # Standard bottleneck
+    """Standard bottleneck."""
+
     def __init__(self, c1, c2, shortcut=True, g=1, k=(3, 3), e=0.5):  # ch_in, ch_out, shortcut, groups, kernels, expand
         super().__init__()
         c_ = int(c2 * e)  # hidden channels
         self.cv1 = Conv(c1, c_, k[0], 1)
         self.cv2 = Conv(c_, c2, k[1], 1, g=g)
         self.add = shortcut and c1 == c2
 
     def forward(self, x):
+        """'forward()' applies the YOLOv5 FPN to input data."""
         return x + self.cv2(self.cv1(x)) if self.add else self.cv2(self.cv1(x))
 
 
 class BottleneckCSP(nn.Module):
-    # CSP Bottleneck https://github.com/WongKinYiu/CrossStagePartialNetworks
+    """CSP Bottleneck https://github.com/WongKinYiu/CrossStagePartialNetworks."""
+
     def __init__(self, c1, c2, n=1, shortcut=True, g=1, e=0.5):  # ch_in, ch_out, number, shortcut, groups, expansion
         super().__init__()
         c_ = int(c2 * e)  # hidden channels
         self.cv1 = Conv(c1, c_, 1, 1)
         self.cv2 = nn.Conv2d(c1, c_, 1, 1, bias=False)
         self.cv3 = nn.Conv2d(c_, c_, 1, 1, bias=False)
         self.cv4 = Conv(2 * c_, c2, 1, 1)
         self.bn = nn.BatchNorm2d(2 * c_)  # applied to cat(cv2, cv3)
         self.act = nn.SiLU()
         self.m = nn.Sequential(*(Bottleneck(c_, c_, shortcut, g, e=1.0) for _ in range(n)))
 
     def forward(self, x):
+        """Applies a CSP bottleneck with 3 convolutions."""
         y1 = self.cv3(self.m(self.cv1(x)))
         y2 = self.cv2(x)
         return self.cv4(self.act(self.bn(torch.cat((y1, y2), 1))))
 
 
 class C3(nn.Module):
-    # CSP Bottleneck with 3 convolutions
+    """CSP Bottleneck with 3 convolutions."""
+
     def __init__(self, c1, c2, n=1, shortcut=True, g=1, e=0.5):  # ch_in, ch_out, number, shortcut, groups, expansion
         super().__init__()
         c_ = int(c2 * e)  # hidden channels
         self.cv1 = Conv(c1, c_, 1, 1)
         self.cv2 = Conv(c1, c_, 1, 1)
         self.cv3 = Conv(2 * c_, c2, 1)  # optional act=FReLU(c2)
-        self.m = nn.Sequential(*(Bottleneck(c_, c_, shortcut, g, e=1.0) for _ in range(n)))
+        self.m = nn.Sequential(*(Bottleneck(c_, c_, shortcut, g, k=((1, 1), (3, 3)), e=1.0) for _ in range(n)))
 
     def forward(self, x):
+        """Forward pass through the CSP bottleneck with 2 convolutions."""
         return self.cv3(torch.cat((self.m(self.cv1(x)), self.cv2(x)), 1))
 
 
 class C2(nn.Module):
-    # CSP Bottleneck with 2 convolutions
+    """CSP Bottleneck with 2 convolutions."""
+
     def __init__(self, c1, c2, n=1, shortcut=True, g=1, e=0.5):  # ch_in, ch_out, number, shortcut, groups, expansion
         super().__init__()
         self.c = int(c2 * e)  # hidden channels
         self.cv1 = Conv(c1, 2 * self.c, 1, 1)
         self.cv2 = Conv(2 * self.c, c2, 1)  # optional act=FReLU(c2)
         # self.attention = ChannelAttention(2 * self.c)  # or SpatialAttention()
         self.m = nn.Sequential(*(Bottleneck(self.c, self.c, shortcut, g, k=((3, 3), (3, 3)), e=1.0) for _ in range(n)))
 
     def forward(self, x):
-        a, b = self.cv1(x).split((self.c, self.c), 1)
+        """Forward pass through the CSP bottleneck with 2 convolutions."""
+        a, b = self.cv1(x).chunk(2, 1)
         return self.cv2(torch.cat((self.m(a), b), 1))
 
 
 class C2f(nn.Module):
-    # CSP Bottleneck with 2 convolutions
+    """CSP Bottleneck with 2 convolutions."""
+
     def __init__(self, c1, c2, n=1, shortcut=False, g=1, e=0.5):  # ch_in, ch_out, number, shortcut, groups, expansion
         super().__init__()
         self.c = int(c2 * e)  # hidden channels
         self.cv1 = Conv(c1, 2 * self.c, 1, 1)
         self.cv2 = Conv((2 + n) * self.c, c2, 1)  # optional act=FReLU(c2)
         self.m = nn.ModuleList(Bottleneck(self.c, self.c, shortcut, g, k=((3, 3), (3, 3)), e=1.0) for _ in range(n))
 
     def forward(self, x):
+        """Forward pass of a YOLOv5 CSPDarknet backbone layer."""
+        y = list(self.cv1(x).chunk(2, 1))
+        y.extend(m(y[-1]) for m in self.m)
+        return self.cv2(torch.cat(y, 1))
+
+    def forward_split(self, x):
+        """Applies spatial attention to module's input."""
         y = list(self.cv1(x).split((self.c, self.c), 1))
         y.extend(m(y[-1]) for m in self.m)
         return self.cv2(torch.cat(y, 1))
 
 
 class ChannelAttention(nn.Module):
-    # Channel-attention module https://github.com/open-mmlab/mmdetection/tree/v3.0.0rc1/configs/rtmdet
+    """Channel-attention module https://github.com/open-mmlab/mmdetection/tree/v3.0.0rc1/configs/rtmdet."""
+
     def __init__(self, channels: int) -> None:
         super().__init__()
         self.pool = nn.AdaptiveAvgPool2d(1)
         self.fc = nn.Conv2d(channels, channels, 1, 1, 0, bias=True)
         self.act = nn.Sigmoid()
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         return x * self.act(self.fc(self.pool(x)))
 
 
 class SpatialAttention(nn.Module):
-    # Spatial-attention module
+    """Spatial-attention module."""
+
     def __init__(self, kernel_size=7):
+        """Initialize Spatial-attention module with kernel size argument."""
         super().__init__()
         assert kernel_size in (3, 7), 'kernel size must be 3 or 7'
         padding = 3 if kernel_size == 7 else 1
         self.cv1 = nn.Conv2d(2, 1, kernel_size, padding=padding, bias=False)
         self.act = nn.Sigmoid()
 
     def forward(self, x):
+        """Apply channel and spatial attention on input for feature recalibration."""
         return x * self.act(self.cv1(torch.cat([torch.mean(x, 1, keepdim=True), torch.max(x, 1, keepdim=True)[0]], 1)))
 
 
 class CBAM(nn.Module):
-    # Convolutional Block Attention Module
+    """Convolutional Block Attention Module."""
+
     def __init__(self, c1, kernel_size=7):  # ch_in, kernels
         super().__init__()
         self.channel_attention = ChannelAttention(c1)
         self.spatial_attention = SpatialAttention(kernel_size)
 
     def forward(self, x):
+        """Applies the forward pass through C1 module."""
         return self.spatial_attention(self.channel_attention(x))
 
 
 class C1(nn.Module):
-    # CSP Bottleneck with 1 convolution
+    """CSP Bottleneck with 1 convolution."""
+
     def __init__(self, c1, c2, n=1):  # ch_in, ch_out, number
         super().__init__()
         self.cv1 = Conv(c1, c2, 1, 1)
         self.m = nn.Sequential(*(Conv(c2, c2, 3) for _ in range(n)))
 
     def forward(self, x):
+        """Applies cross-convolutions to input in the C3 module."""
         y = self.cv1(x)
         return self.m(y) + y
 
 
 class C3x(C3):
-    # C3 module with cross-convolutions
+    """C3 module with cross-convolutions."""
+
     def __init__(self, c1, c2, n=1, shortcut=True, g=1, e=0.5):
+        """Initialize C3TR instance and set default parameters."""
         super().__init__(c1, c2, n, shortcut, g, e)
         self.c_ = int(c2 * e)
         self.m = nn.Sequential(*(Bottleneck(self.c_, self.c_, shortcut, g, k=((1, 3), (3, 1)), e=1) for _ in range(n)))
 
 
 class C3TR(C3):
-    # C3 module with TransformerBlock()
+    """C3 module with TransformerBlock()."""
+
     def __init__(self, c1, c2, n=1, shortcut=True, g=1, e=0.5):
+        """Initialize C3Ghost module with GhostBottleneck()."""
         super().__init__(c1, c2, n, shortcut, g, e)
         c_ = int(c2 * e)
         self.m = TransformerBlock(c_, c_, 4, n)
 
 
 class C3Ghost(C3):
-    # C3 module with GhostBottleneck()
+    """C3 module with GhostBottleneck()."""
+
     def __init__(self, c1, c2, n=1, shortcut=True, g=1, e=0.5):
+        """Initialize 'SPP' module with various pooling sizes for spatial pyramid pooling."""
         super().__init__(c1, c2, n, shortcut, g, e)
         c_ = int(c2 * e)  # hidden channels
         self.m = nn.Sequential(*(GhostBottleneck(c_, c_) for _ in range(n)))
 
 
 class SPP(nn.Module):
-    # Spatial Pyramid Pooling (SPP) layer https://arxiv.org/abs/1406.4729
+    """Spatial Pyramid Pooling (SPP) layer https://arxiv.org/abs/1406.4729."""
+
     def __init__(self, c1, c2, k=(5, 9, 13)):
+        """Initialize the SPP layer with input/output channels and pooling kernel sizes."""
         super().__init__()
         c_ = c1 // 2  # hidden channels
         self.cv1 = Conv(c1, c_, 1, 1)
         self.cv2 = Conv(c_ * (len(k) + 1), c2, 1, 1)
         self.m = nn.ModuleList([nn.MaxPool2d(kernel_size=x, stride=1, padding=x // 2) for x in k])
 
     def forward(self, x):
+        """Forward pass of the SPP layer, performing spatial pyramid pooling."""
         x = self.cv1(x)
-        with warnings.catch_warnings():
-            warnings.simplefilter('ignore')  # suppress torch 1.9.0 max_pool2d() warning
-            return self.cv2(torch.cat([x] + [m(x) for m in self.m], 1))
+        return self.cv2(torch.cat([x] + [m(x) for m in self.m], 1))
 
 
 class SPPF(nn.Module):
-    # Spatial Pyramid Pooling - Fast (SPPF) layer for YOLOv5 by Glenn Jocher
+    """Spatial Pyramid Pooling - Fast (SPPF) layer for YOLOv5 by Glenn Jocher."""
+
     def __init__(self, c1, c2, k=5):  # equivalent to SPP(k=(5, 9, 13))
         super().__init__()
         c_ = c1 // 2  # hidden channels
         self.cv1 = Conv(c1, c_, 1, 1)
         self.cv2 = Conv(c_ * 4, c2, 1, 1)
         self.m = nn.MaxPool2d(kernel_size=k, stride=1, padding=k // 2)
 
     def forward(self, x):
+        """Forward pass through Ghost Convolution block."""
         x = self.cv1(x)
-        with warnings.catch_warnings():
-            warnings.simplefilter('ignore')  # suppress torch 1.9.0 max_pool2d() warning
-            y1 = self.m(x)
-            y2 = self.m(y1)
-            return self.cv2(torch.cat((x, y1, y2, self.m(y2)), 1))
+        y1 = self.m(x)
+        y2 = self.m(y1)
+        return self.cv2(torch.cat((x, y1, y2, self.m(y2)), 1))
 
 
 class Focus(nn.Module):
-    # Focus wh information into c-space
+    """Focus wh information into c-space."""
+
     def __init__(self, c1, c2, k=1, s=1, p=None, g=1, act=True):  # ch_in, ch_out, kernel, stride, padding, groups
         super().__init__()
         self.conv = Conv(c1 * 4, c2, k, s, p, g, act=act)
         # self.contract = Contract(gain=2)
 
     def forward(self, x):  # x(b,c,w,h) -> y(b,4c,w/2,h/2)
         return self.conv(torch.cat((x[..., ::2, ::2], x[..., 1::2, ::2], x[..., ::2, 1::2], x[..., 1::2, 1::2]), 1))
         # return self.conv(self.contract(x))
 
 
 class GhostConv(nn.Module):
-    # Ghost Convolution https://github.com/huawei-noah/ghostnet
+    """Ghost Convolution https://github.com/huawei-noah/ghostnet."""
+
     def __init__(self, c1, c2, k=1, s=1, g=1, act=True):  # ch_in, ch_out, kernel, stride, groups
         super().__init__()
         c_ = c2 // 2  # hidden channels
         self.cv1 = Conv(c1, c_, k, s, None, g, act=act)
         self.cv2 = Conv(c_, c_, 5, 1, None, c_, act=act)
 
     def forward(self, x):
+        """Forward propagation through a Ghost Bottleneck layer with skip connection."""
         y = self.cv1(x)
         return torch.cat((y, self.cv2(y)), 1)
 
 
 class GhostBottleneck(nn.Module):
-    # Ghost Bottleneck https://github.com/huawei-noah/ghostnet
+    """Ghost Bottleneck https://github.com/huawei-noah/ghostnet."""
+
     def __init__(self, c1, c2, k=3, s=1):  # ch_in, ch_out, kernel, stride
         super().__init__()
         c_ = c2 // 2
         self.conv = nn.Sequential(
             GhostConv(c1, c_, 1, 1),  # pw
             DWConv(c_, c_, k, s, act=False) if s == 2 else nn.Identity(),  # dw
             GhostConv(c_, c2, 1, 1, act=False))  # pw-linear
         self.shortcut = nn.Sequential(DWConv(c1, c1, k, s, act=False), Conv(c1, c2, 1, 1,
                                                                             act=False)) if s == 2 else nn.Identity()
 
     def forward(self, x):
+        """Applies skip connection and concatenation to input tensor."""
         return self.conv(x) + self.shortcut(x)
 
 
 class Concat(nn.Module):
-    # Concatenate a list of tensors along dimension
+    """Concatenate a list of tensors along dimension."""
+
     def __init__(self, dimension=1):
+        """Concatenates a list of tensors along a specified dimension."""
         super().__init__()
         self.d = dimension
 
     def forward(self, x):
+        """Forward pass for the YOLOv8 mask Proto module."""
         return torch.cat(x, self.d)
 
 
 class Proto(nn.Module):
-    # YOLOv8 mask Proto module for segmentation models
+    """YOLOv8 mask Proto module for segmentation models."""
+
     def __init__(self, c1, c_=256, c2=32):  # ch_in, number of protos, number of masks
         super().__init__()
         self.cv1 = Conv(c1, c_, k=3)
         self.upsample = nn.ConvTranspose2d(c_, c_, 2, 2, 0, bias=True)  # nn.Upsample(scale_factor=2, mode='nearest')
         self.cv2 = Conv(c_, c_, k=3)
         self.cv3 = Conv(c_, c2)
 
     def forward(self, x):
+        """Performs a forward pass through layers using an upsampled input image."""
         return self.cv3(self.cv2(self.upsample(self.cv1(x))))
 
 
 class Ensemble(nn.ModuleList):
-    # Ensemble of models
+    """Ensemble of models."""
+
     def __init__(self):
+        """Initialize an ensemble of models."""
         super().__init__()
 
     def forward(self, x, augment=False, profile=False, visualize=False):
+        """Function generates the YOLOv5 network's final layer."""
         y = [module(x, augment, profile, visualize)[0] for module in self]
         # y = torch.stack(y).max(0)[0]  # max ensemble
         # y = torch.stack(y).mean(0)  # mean ensemble
-        y = torch.cat(y, 1)  # nms ensemble
+        y = torch.cat(y, 2)  # nms ensemble, y shape(B, HW, C)
         return y, None  # inference, train output
 
 
-# heads
+# Model heads below ----------------------------------------------------------------------------------------------------
+
+
 class Detect(nn.Module):
-    # YOLOv8 Detect head for detection models
+    """YOLOv8 Detect head for detection models."""
     dynamic = False  # force grid reconstruction
     export = False  # export mode
     shape = None
     anchors = torch.empty(0)  # init
     strides = torch.empty(0)  # init
 
     def __init__(self, nc=80, ch=()):  # detection layer
         super().__init__()
         self.nc = nc  # number of classes
         self.nl = len(ch)  # number of detection layers
         self.reg_max = 16  # DFL channels (ch[0] // 16 to scale 4/8/12/16/20 for n/s/m/l/x)
         self.no = nc + self.reg_max * 4  # number of outputs per anchor
         self.stride = torch.zeros(self.nl)  # strides computed during build
-
         c2, c3 = max((16, ch[0] // 4, self.reg_max * 4)), max(ch[0], self.nc)  # channels
         self.cv2 = nn.ModuleList(
             nn.Sequential(Conv(x, c2, 3), Conv(c2, c2, 3), nn.Conv2d(c2, 4 * self.reg_max, 1)) for x in ch)
         self.cv3 = nn.ModuleList(nn.Sequential(Conv(x, c3, 3), Conv(c3, c3, 3), nn.Conv2d(c3, self.nc, 1)) for x in ch)
         self.dfl = DFL(self.reg_max) if self.reg_max > 1 else nn.Identity()
 
     def forward(self, x):
+        """Concatenates and returns predicted bounding boxes and class probabilities."""
         shape = x[0].shape  # BCHW
         for i in range(self.nl):
             x[i] = torch.cat((self.cv2[i](x[i]), self.cv3[i](x[i])), 1)
         if self.training:
             return x
         elif self.dynamic or self.shape != shape:
             self.anchors, self.strides = (x.transpose(0, 1) for x in make_anchors(x, self.stride, 0.5))
             self.shape = shape
 
-        box, cls = torch.cat([xi.view(shape[0], self.no, -1) for xi in x], 2).split((self.reg_max * 4, self.nc), 1)
+        x_cat = torch.cat([xi.view(shape[0], self.no, -1) for xi in x], 2)
+        if self.export and self.format in ('saved_model', 'pb', 'tflite', 'edgetpu', 'tfjs'):  # avoid TF FlexSplitV ops
+            box = x_cat[:, :self.reg_max * 4]
+            cls = x_cat[:, self.reg_max * 4:]
+        else:
+            box, cls = x_cat.split((self.reg_max * 4, self.nc), 1)
         dbox = dist2bbox(self.dfl(box), self.anchors.unsqueeze(0), xywh=True, dim=1) * self.strides
         y = torch.cat((dbox, cls.sigmoid()), 1)
         return y if self.export else (y, x)
 
     def bias_init(self):
-        # Initialize Detect() biases, WARNING: requires stride availability
+        """Initialize Detect() biases, WARNING: requires stride availability."""
         m = self  # self.model[-1]  # Detect() module
         # cf = torch.bincount(torch.tensor(np.concatenate(dataset.labels, 0)[:, 0]).long(), minlength=nc) + 1
         # ncf = math.log(0.6 / (m.nc - 0.999999)) if cf is None else torch.log(cf / cf.sum())  # nominal class frequency
         for a, b, s in zip(m.cv2, m.cv3, m.stride):  # from
             a[-1].bias.data[:] = 1.0  # box
             b[-1].bias.data[:m.nc] = math.log(5 / m.nc / (640 / s) ** 2)  # cls (.01 objects, 80 classes, 640 img)
 
 
+class MLPBlock(nn.Module):
+
+    def __init__(
+        self,
+        embedding_dim,
+        mlp_dim,
+        act=nn.GELU,
+    ):
+        super().__init__()
+        self.lin1 = nn.Linear(embedding_dim, mlp_dim)
+        self.lin2 = nn.Linear(mlp_dim, embedding_dim)
+        self.act = act()
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        return self.lin2(self.act(self.lin1(x)))
+
+
+# From https://github.com/facebookresearch/detectron2/blob/main/detectron2/layers/batch_norm.py # noqa
+# Itself from https://github.com/facebookresearch/ConvNeXt/blob/d1fa8f6fef0a165b27399986cc2bdacc92777e40/models/convnext.py#L119  # noqa
+class LayerNorm2d(nn.Module):
+
+    def __init__(self, num_channels, eps=1e-6):
+        super().__init__()
+        self.weight = nn.Parameter(torch.ones(num_channels))
+        self.bias = nn.Parameter(torch.zeros(num_channels))
+        self.eps = eps
+
+    def forward(self, x):
+        u = x.mean(1, keepdim=True)
+        s = (x - u).pow(2).mean(1, keepdim=True)
+        x = (x - u) / torch.sqrt(s + self.eps)
+        x = self.weight[:, None, None] * x + self.bias[:, None, None]
+        return x
+
+
 class Segment(Detect):
-    # YOLOv8 Segment head for segmentation models
+    """YOLOv8 Segment head for segmentation models."""
+
     def __init__(self, nc=80, nm=32, npr=256, ch=()):
+        """Initialize the YOLO model attributes such as the number of masks, prototypes, and the convolution layers."""
         super().__init__(nc, ch)
         self.nm = nm  # number of masks
         self.npr = npr  # number of protos
         self.proto = Proto(ch[0], self.npr, self.nm)  # protos
         self.detect = Detect.forward
 
         c4 = max(ch[0] // 4, self.nm)
         self.cv4 = nn.ModuleList(nn.Sequential(Conv(x, c4, 3), Conv(c4, c4, 3), nn.Conv2d(c4, self.nm, 1)) for x in ch)
 
     def forward(self, x):
+        """Return model outputs and mask coefficients if training, otherwise return outputs and mask coefficients."""
         p = self.proto(x[0])  # mask protos
         bs = p.shape[0]  # batch size
 
         mc = torch.cat([self.cv4[i](x[i]).view(bs, self.nm, -1) for i in range(self.nl)], 2)  # mask coefficients
         x = self.detect(self, x)
         if self.training:
             return x, mc, p
         return (torch.cat([x, mc], 1), p) if self.export else (torch.cat([x[0], mc], 1), (x[1], mc, p))
 
 
+class Pose(Detect):
+    """YOLOv8 Pose head for keypoints models."""
+
+    def __init__(self, nc=80, kpt_shape=(17, 3), ch=()):
+        """Initialize YOLO network with default parameters and Convolutional Layers."""
+        super().__init__(nc, ch)
+        self.kpt_shape = kpt_shape  # number of keypoints, number of dims (2 for x,y or 3 for x,y,visible)
+        self.nk = kpt_shape[0] * kpt_shape[1]  # number of keypoints total
+        self.detect = Detect.forward
+
+        c4 = max(ch[0] // 4, self.nk)
+        self.cv4 = nn.ModuleList(nn.Sequential(Conv(x, c4, 3), Conv(c4, c4, 3), nn.Conv2d(c4, self.nk, 1)) for x in ch)
+
+    def forward(self, x):
+        """Perform forward pass through YOLO model and return predictions."""
+        bs = x[0].shape[0]  # batch size
+        kpt = torch.cat([self.cv4[i](x[i]).view(bs, self.nk, -1) for i in range(self.nl)], -1)  # (bs, 17*3, h*w)
+        x = self.detect(self, x)
+        if self.training:
+            return x, kpt
+        pred_kpt = self.kpts_decode(bs, kpt)
+        return torch.cat([x, pred_kpt], 1) if self.export else (torch.cat([x[0], pred_kpt], 1), (x[1], kpt))
+
+    def kpts_decode(self, bs, kpts):
+        """Decodes keypoints."""
+        ndim = self.kpt_shape[1]
+        if self.export:  # required for TFLite export to avoid 'PLACEHOLDER_FOR_GREATER_OP_CODES' bug
+            y = kpts.view(bs, *self.kpt_shape, -1)
+            a = (y[:, :, :2] * 2.0 + (self.anchors - 0.5)) * self.strides
+            if ndim == 3:
+                a = torch.cat((a, y[:, :, 1:2].sigmoid()), 2)
+            return a.view(bs, self.nk, -1)
+        else:
+            y = kpts.clone()
+            if ndim == 3:
+                y[:, 2::3].sigmoid_()  # inplace sigmoid
+            y[:, 0::ndim] = (y[:, 0::ndim] * 2.0 + (self.anchors[0] - 0.5)) * self.strides
+            y[:, 1::ndim] = (y[:, 1::ndim] * 2.0 + (self.anchors[1] - 0.5)) * self.strides
+            return y
+
+
 class Classify(nn.Module):
-    # YOLOv8 classification head, i.e. x(b,c1,20,20) to x(b,c2)
+    """YOLOv8 classification head, i.e. x(b,c1,20,20) to x(b,c2)."""
+
     def __init__(self, c1, c2, k=1, s=1, p=None, g=1):  # ch_in, ch_out, kernel, stride, padding, groups
         super().__init__()
         c_ = 1280  # efficientnet_b0 size
         self.conv = Conv(c1, c_, k, s, autopad(k, p), g)
         self.pool = nn.AdaptiveAvgPool2d(1)  # to x(b,c_,1,1)
         self.drop = nn.Dropout(p=0.0, inplace=True)
         self.linear = nn.Linear(c_, c2)  # to x(b,c2)
 
     def forward(self, x):
+        """Performs a forward pass of the YOLO model on input image data."""
         if isinstance(x, list):
             x = torch.cat(x, 1)
-        return self.linear(self.drop(self.pool(self.conv(x)).flatten(1)))
+        x = self.linear(self.drop(self.pool(self.conv(x)).flatten(1)))
+        return x if self.training else x.softmax(1)
```

### Comparing `ultralytics-8.0.9/ultralytics/nn/tasks.py` & `ultralytics-8.0.90/ultralytics/nn/tasks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import contextlib
 from copy import deepcopy
+from pathlib import Path
 
 import thop
 import torch
 import torch.nn as nn
 
 from ultralytics.nn.modules import (C1, C2, C3, C3TR, SPP, SPPF, Bottleneck, BottleneckCSP, C2f, C3Ghost, C3x, Classify,
                                     Concat, Conv, ConvTranspose, Detect, DWConv, DWConvTranspose2d, Ensemble, Focus,
-                                    GhostBottleneck, GhostConv, Segment)
-from ultralytics.yolo.utils import DEFAULT_CONFIG_DICT, DEFAULT_CONFIG_KEYS, LOGGER, colorstr, yaml_load
-from ultralytics.yolo.utils.checks import check_yaml
-from ultralytics.yolo.utils.torch_utils import (fuse_conv_and_bn, initialize_weights, intersect_dicts, make_divisible,
-                                                model_info, scale_img, time_sync)
+                                    GhostBottleneck, GhostConv, Pose, Segment)
+from ultralytics.yolo.utils import DEFAULT_CFG_DICT, DEFAULT_CFG_KEYS, LOGGER, colorstr, emojis, yaml_load
+from ultralytics.yolo.utils.checks import check_requirements, check_suffix, check_yaml
+from ultralytics.yolo.utils.plotting import feature_visualization
+from ultralytics.yolo.utils.torch_utils import (fuse_conv_and_bn, fuse_deconv_and_bn, initialize_weights,
+                                                intersect_dicts, make_divisible, model_info, scale_img, time_sync)
 
 
 class BaseModel(nn.Module):
     """
     The BaseModel class serves as a base class for all the models in the Ultralytics YOLO family.
     """
 
@@ -53,67 +55,86 @@
             if m.f != -1:  # if not from previous layer
                 x = y[m.f] if isinstance(m.f, int) else [x if j == -1 else y[j] for j in m.f]  # from earlier layers
             if profile:
                 self._profile_one_layer(m, x, dt)
             x = m(x)  # run
             y.append(x if m.i in self.save else None)  # save output
             if visualize:
-                LOGGER.info('visualize feature not yet supported')
-                # TODO: feature_visualization(x, m.type, m.i, save_dir=visualize)
+                feature_visualization(x, m.type, m.i, save_dir=visualize)
         return x
 
     def _profile_one_layer(self, m, x, dt):
         """
-        Profile the computation time and FLOPs of a single layer of the model on a given input. Appends the results to the provided list.
+        Profile the computation time and FLOPs of a single layer of the model on a given input.
+        Appends the results to the provided list.
 
         Args:
             m (nn.Module): The layer to be profiled.
             x (torch.Tensor): The input data to the layer.
             dt (list): A list to store the computation time of the layer.
 
         Returns:
             None
         """
         c = m == self.model[-1]  # is final layer, copy input as inplace fix
-        o = thop.profile(m, inputs=(x.copy() if c else x,), verbose=False)[0] / 1E9 * 2 if thop else 0  # FLOPs
+        o = thop.profile(m, inputs=[x.clone() if c else x], verbose=False)[0] / 1E9 * 2 if thop else 0  # FLOPs
         t = time_sync()
         for _ in range(10):
-            m(x.copy() if c else x)
+            m(x.clone() if c else x)
         dt.append((time_sync() - t) * 100)
         if m == self.model[0]:
             LOGGER.info(f"{'time (ms)':>10s} {'GFLOPs':>10s} {'params':>10s}  module")
         LOGGER.info(f'{dt[-1]:10.2f} {o:10.2f} {m.np:10.0f}  {m.type}')
         if c:
             LOGGER.info(f"{sum(dt):10.2f} {'-':>10s} {'-':>10s}  Total")
 
-    def fuse(self):
+    def fuse(self, verbose=True):
         """
-        Fuse the `Conv2d()` and `BatchNorm2d()` layers of the model into a single layer, in order to improve the computation efficiency.
+        Fuse the `Conv2d()` and `BatchNorm2d()` layers of the model into a single layer, in order to improve the
+        computation efficiency.
 
         Returns:
             (nn.Module): The fused model is returned.
         """
-        LOGGER.info('Fusing layers... ')
-        for m in self.model.modules():
-            if isinstance(m, (Conv, DWConv)) and hasattr(m, 'bn'):
-                m.conv = fuse_conv_and_bn(m.conv, m.bn)  # update conv
-                delattr(m, 'bn')  # remove batchnorm
-                m.forward = m.forward_fuse  # update forward
-        self.info()
+        if not self.is_fused():
+            for m in self.model.modules():
+                if isinstance(m, (Conv, DWConv)) and hasattr(m, 'bn'):
+                    m.conv = fuse_conv_and_bn(m.conv, m.bn)  # update conv
+                    delattr(m, 'bn')  # remove batchnorm
+                    m.forward = m.forward_fuse  # update forward
+                if isinstance(m, ConvTranspose) and hasattr(m, 'bn'):
+                    m.conv_transpose = fuse_deconv_and_bn(m.conv_transpose, m.bn)
+                    delattr(m, 'bn')  # remove batchnorm
+                    m.forward = m.forward_fuse  # update forward
+            self.info(verbose=verbose)
+
         return self
 
-    def info(self, verbose=False, imgsz=640):
+    def is_fused(self, thresh=10):
+        """
+        Check if the model has less than a certain threshold of BatchNorm layers.
+
+        Args:
+            thresh (int, optional): The threshold number of BatchNorm layers. Default is 10.
+
+        Returns:
+            (bool): True if the number of BatchNorm layers in the model is less than the threshold, False otherwise.
+        """
+        bn = tuple(v for k, v in nn.__dict__.items() if 'Norm' in k)  # normalization layers, i.e. BatchNorm2d()
+        return sum(isinstance(v, bn) for v in self.modules()) < thresh  # True if < 'thresh' BatchNorm layers in model
+
+    def info(self, verbose=True, imgsz=640):
         """
         Prints model information
 
         Args:
             verbose (bool): if True, prints out the model information. Defaults to False
             imgsz (int): the size of the image that the model will be trained on. Defaults to 640
         """
-        model_info(self, verbose, imgsz)
+        model_info(self, verbose=verbose, imgsz=imgsz)
 
     def _apply(self, fn):
         """
         `_apply()` is a function that applies a function to all the tensors in the model that are not
         parameters or registered buffers
 
         Args:
@@ -126,62 +147,69 @@
         m = self.model[-1]  # Detect()
         if isinstance(m, (Detect, Segment)):
             m.stride = fn(m.stride)
             m.anchors = fn(m.anchors)
             m.strides = fn(m.strides)
         return self
 
-    def load(self, weights):
-        """
-        This function loads the weights of the model from a file
+    def load(self, weights, verbose=True):
+        """Load the weights into the model.
 
         Args:
-            weights (str): The weights to load into the model.
+            weights (dict) or (torch.nn.Module): The pre-trained weights to be loaded.
+            verbose (bool, optional): Whether to log the transfer progress. Defaults to True.
         """
-        # Force all tasks to implement this function
-        raise NotImplementedError("This function needs to be implemented by derived classes!")
+        model = weights['model'] if isinstance(weights, dict) else weights  # torchvision models are not dicts
+        csd = model.float().state_dict()  # checkpoint state_dict as FP32
+        csd = intersect_dicts(csd, self.state_dict())  # intersect
+        self.load_state_dict(csd, strict=False)  # load
+        if verbose:
+            LOGGER.info(f'Transferred {len(csd)}/{len(self.model.state_dict())} items from pretrained weights')
 
 
 class DetectionModel(BaseModel):
-    # YOLOv8 detection model
+    """YOLOv8 detection model."""
+
     def __init__(self, cfg='yolov8n.yaml', ch=3, nc=None, verbose=True):  # model, input channels, number of classes
         super().__init__()
-        self.yaml = cfg if isinstance(cfg, dict) else yaml_load(check_yaml(cfg), append_filename=True)  # cfg dict
+        self.yaml = cfg if isinstance(cfg, dict) else yaml_model_load(cfg)  # cfg dict
 
         # Define model
         ch = self.yaml['ch'] = self.yaml.get('ch', ch)  # input channels
         if nc and nc != self.yaml['nc']:
             LOGGER.info(f"Overriding model.yaml nc={self.yaml['nc']} with nc={nc}")
             self.yaml['nc'] = nc  # override yaml value
-        self.model, self.save = parse_model(deepcopy(self.yaml), ch=[ch], verbose=verbose)  # model, savelist
+        self.model, self.save = parse_model(deepcopy(self.yaml), ch=ch, verbose=verbose)  # model, savelist
         self.names = {i: f'{i}' for i in range(self.yaml['nc'])}  # default names dict
         self.inplace = self.yaml.get('inplace', True)
 
         # Build strides
         m = self.model[-1]  # Detect()
-        if isinstance(m, (Detect, Segment)):
+        if isinstance(m, (Detect, Segment, Pose)):
             s = 256  # 2x min stride
             m.inplace = self.inplace
-            forward = lambda x: self.forward(x)[0] if isinstance(m, Segment) else self.forward(x)
+            forward = lambda x: self.forward(x)[0] if isinstance(m, (Segment, Pose)) else self.forward(x)
             m.stride = torch.tensor([s / x.shape[-2] for x in forward(torch.zeros(1, ch, s, s))])  # forward
             self.stride = m.stride
             m.bias_init()  # only run once
 
         # Init weights, biases
         initialize_weights(self)
         if verbose:
             self.info()
             LOGGER.info('')
 
     def forward(self, x, augment=False, profile=False, visualize=False):
+        """Run forward pass on input image(s) with optional augmentation and profiling."""
         if augment:
             return self._forward_augment(x)  # augmented inference, None
         return self._forward_once(x, profile, visualize)  # single-scale inference, train
 
     def _forward_augment(self, x):
+        """Perform augmentations on input image x and return augmented inference and train outputs."""
         img_size = x.shape[-2:]  # height, width
         s = [1, 0.83, 0.67]  # scales
         f = [None, 3, None]  # flips (2-ud, 3-lr)
         y = []  # outputs
         for si, fi in zip(s, f):
             xi = scale_img(x.flip(fi) if fi else x, si, gs=int(self.stride.max()))
             yi = self._forward_once(xi)[0]  # forward
@@ -189,62 +217,75 @@
             yi = self._descale_pred(yi, fi, si, img_size)
             y.append(yi)
         y = self._clip_augmented(y)  # clip augmented tails
         return torch.cat(y, -1), None  # augmented inference, train
 
     @staticmethod
     def _descale_pred(p, flips, scale, img_size, dim=1):
-        # de-scale predictions following augmented inference (inverse operation)
+        """De-scale predictions following augmented inference (inverse operation)."""
         p[:, :4] /= scale  # de-scale
         x, y, wh, cls = p.split((1, 1, 2, p.shape[dim] - 4), dim)
         if flips == 2:
             y = img_size[0] - y  # de-flip ud
         elif flips == 3:
             x = img_size[1] - x  # de-flip lr
         return torch.cat((x, y, wh, cls), dim)
 
     def _clip_augmented(self, y):
-        # Clip YOLOv5 augmented inference tails
+        """Clip YOLOv5 augmented inference tails."""
         nl = self.model[-1].nl  # number of detection layers (P3-P5)
         g = sum(4 ** x for x in range(nl))  # grid points
         e = 1  # exclude layer count
         i = (y[0].shape[-1] // g) * sum(4 ** x for x in range(e))  # indices
         y[0] = y[0][..., :-i]  # large
         i = (y[-1].shape[-1] // g) * sum(4 ** (nl - 1 - x) for x in range(e))  # indices
         y[-1] = y[-1][..., i:]  # small
         return y
 
-    def load(self, weights, verbose=True):
-        csd = weights.float().state_dict()  # checkpoint state_dict as FP32
-        csd = intersect_dicts(csd, self.state_dict())  # intersect
-        self.load_state_dict(csd, strict=False)  # load
-        if verbose:
-            LOGGER.info(f'Transferred {len(csd)}/{len(self.model.state_dict())} items from pretrained weights')
-
 
 class SegmentationModel(DetectionModel):
-    # YOLOv8 segmentation model
+    """YOLOv8 segmentation model."""
+
     def __init__(self, cfg='yolov8n-seg.yaml', ch=3, nc=None, verbose=True):
-        super().__init__(cfg, ch, nc, verbose)
+        """Initialize YOLOv8 segmentation model with given config and parameters."""
+        super().__init__(cfg=cfg, ch=ch, nc=nc, verbose=verbose)
+
+    def _forward_augment(self, x):
+        """Undocumented function."""
+        raise NotImplementedError(emojis('WARNING ⚠️ SegmentationModel has not supported augment inference yet!'))
+
+
+class PoseModel(DetectionModel):
+    """YOLOv8 pose model."""
+
+    def __init__(self, cfg='yolov8n-pose.yaml', ch=3, nc=None, data_kpt_shape=(None, None), verbose=True):
+        """Initialize YOLOv8 Pose model."""
+        if not isinstance(cfg, dict):
+            cfg = yaml_model_load(cfg)  # load model YAML
+        if any(data_kpt_shape) and list(data_kpt_shape) != list(cfg['kpt_shape']):
+            LOGGER.info(f"Overriding model.yaml kpt_shape={cfg['kpt_shape']} with kpt_shape={data_kpt_shape}")
+            cfg['kpt_shape'] = data_kpt_shape
+        super().__init__(cfg=cfg, ch=ch, nc=nc, verbose=verbose)
 
 
 class ClassificationModel(BaseModel):
-    # YOLOv8 classification model
+    """YOLOv8 classification model."""
+
     def __init__(self,
                  cfg=None,
                  model=None,
                  ch=3,
-                 nc=1000,
+                 nc=None,
                  cutoff=10,
-                 verbose=True):  # yaml, model, number of classes, cutoff index
+                 verbose=True):  # yaml, model, channels, number of classes, cutoff index, verbose flag
         super().__init__()
         self._from_detection_model(model, nc, cutoff) if model is not None else self._from_yaml(cfg, ch, nc, verbose)
 
     def _from_detection_model(self, model, nc=1000, cutoff=10):
-        # Create a YOLOv5 classification model from a YOLOv5 detection model
+        """Create a YOLOv5 classification model from a YOLOv5 detection model."""
         from ultralytics.nn.autobackend import AutoBackend
         if isinstance(model, AutoBackend):
             model = model.model  # unwrap DetectMultiBackend
         model.model = model.model[:cutoff]  # backbone
         m = model.model[-1]  # last layer
         ch = m.conv.in_channels if hasattr(m, 'conv') else m.cv1.conv.in_channels  # ch into module
         c = Classify(ch, nc)  # Classify()
@@ -252,33 +293,32 @@
         model.model[-1] = c  # replace
         self.model = model.model
         self.stride = model.stride
         self.save = []
         self.nc = nc
 
     def _from_yaml(self, cfg, ch, nc, verbose):
-        self.yaml = cfg if isinstance(cfg, dict) else yaml_load(check_yaml(cfg), append_filename=True)  # cfg dict
+        """Set YOLOv8 model configurations and define the model architecture."""
+        self.yaml = cfg if isinstance(cfg, dict) else yaml_model_load(cfg)  # cfg dict
+
         # Define model
         ch = self.yaml['ch'] = self.yaml.get('ch', ch)  # input channels
         if nc and nc != self.yaml['nc']:
             LOGGER.info(f"Overriding model.yaml nc={self.yaml['nc']} with nc={nc}")
             self.yaml['nc'] = nc  # override yaml value
-        self.model, self.save = parse_model(deepcopy(self.yaml), ch=[ch], verbose=verbose)  # model, savelist
+        elif not nc and not self.yaml.get('nc', None):
+            raise ValueError('nc not specified. Must specify nc in model.yaml or function arguments.')
+        self.model, self.save = parse_model(deepcopy(self.yaml), ch=ch, verbose=verbose)  # model, savelist
+        self.stride = torch.Tensor([1])  # no stride constraints
         self.names = {i: f'{i}' for i in range(self.yaml['nc'])}  # default names dict
         self.info()
 
-    def load(self, weights):
-        model = weights["model"] if isinstance(weights, dict) else weights  # torchvision models are not dicts
-        csd = model.float().state_dict()
-        csd = intersect_dicts(csd, self.state_dict())  # intersect
-        self.load_state_dict(csd, strict=False)  # load
-
     @staticmethod
     def reshape_outputs(model, nc):
-        # Update a TorchVision classification model to class count 'n' if required
+        """Update a TorchVision classification model to class count 'n' if required."""
         name, m = list((model.model if hasattr(model, 'model') else model).named_children())[-1]  # last module
         if isinstance(m, Classify):  # YOLO Classify() head
             if m.linear.out_features != nc:
                 m.linear = nn.Linear(m.linear.in_features, nc)
         elif isinstance(m, nn.Linear):  # ResNet, EfficientNet
             if m.out_features != nc:
                 setattr(model, name, nn.Linear(m.in_features, nc))
@@ -293,65 +333,99 @@
                 if m[i].out_channels != nc:
                     m[i] = nn.Conv2d(m[i].in_channels, nc, m[i].kernel_size, m[i].stride, bias=m[i].bias is not None)
 
 
 # Functions ------------------------------------------------------------------------------------------------------------
 
 
+def torch_safe_load(weight):
+    """
+    This function attempts to load a PyTorch model with the torch.load() function. If a ModuleNotFoundError is raised,
+    it catches the error, logs a warning message, and attempts to install the missing module via the
+    check_requirements() function. After installation, the function again attempts to load the model using torch.load().
+
+    Args:
+        weight (str): The file path of the PyTorch model.
+
+    Returns:
+        (dict): The loaded PyTorch model.
+    """
+    from ultralytics.yolo.utils.downloads import attempt_download_asset
+
+    check_suffix(file=weight, suffix='.pt')
+    file = attempt_download_asset(weight)  # search online if missing locally
+    try:
+        return torch.load(file, map_location='cpu'), file  # load
+    except ModuleNotFoundError as e:  # e.name is missing module name
+        if e.name == 'models':
+            raise TypeError(
+                emojis(f'ERROR ❌️ {weight} appears to be an Ultralytics YOLOv5 model originally trained '
+                       f'with https://github.com/ultralytics/yolov5.\nThis model is NOT forwards compatible with '
+                       f'YOLOv8 at https://github.com/ultralytics/ultralytics.'
+                       f"\nRecommend fixes are to train a new model using the latest 'ultralytics' package or to "
+                       f"run a command with an official YOLOv8 model, i.e. 'yolo predict model=yolov8n.pt'")) from e
+        LOGGER.warning(f"WARNING ⚠️ {weight} appears to require '{e.name}', which is not in ultralytics requirements."
+                       f"\nAutoInstall will run now for '{e.name}' but this feature will be removed in the future."
+                       f"\nRecommend fixes are to train a new model using the latest 'ultralytics' package or to "
+                       f"run a command with an official YOLOv8 model, i.e. 'yolo predict model=yolov8n.pt'")
+        check_requirements(e.name)  # install missing module
+
+        return torch.load(file, map_location='cpu'), file  # load
+
+
 def attempt_load_weights(weights, device=None, inplace=True, fuse=False):
-    # Loads an ensemble of models weights=[a,b,c] or a single model weights=[a] or weights=a
-    from ultralytics.yolo.utils.downloads import attempt_download
+    """Loads an ensemble of models weights=[a,b,c] or a single model weights=[a] or weights=a."""
 
-    model = Ensemble()
+    ensemble = Ensemble()
     for w in weights if isinstance(weights, list) else [weights]:
-        ckpt = torch.load(attempt_download(w), map_location='cpu')  # load
-        args = {**DEFAULT_CONFIG_DICT, **ckpt['train_args']}  # combine model and default args, preferring model args
-        ckpt = (ckpt.get('ema') or ckpt['model']).to(device).float()  # FP32 model
+        ckpt, w = torch_safe_load(w)  # load ckpt
+        args = {**DEFAULT_CFG_DICT, **ckpt['train_args']}  # combine model and default args, preferring model args
+        model = (ckpt.get('ema') or ckpt['model']).to(device).float()  # FP32 model
 
         # Model compatibility updates
-        ckpt.args = {k: v for k, v in args.items() if k in DEFAULT_CONFIG_KEYS}  # attach args to model
-        ckpt.pt_path = weights  # attach *.pt file path to model
-        if not hasattr(ckpt, 'stride'):
-            ckpt.stride = torch.tensor([32.])
+        model.args = args  # attach args to model
+        model.pt_path = w  # attach *.pt file path to model
+        model.task = guess_model_task(model)
+        if not hasattr(model, 'stride'):
+            model.stride = torch.tensor([32.])
 
         # Append
-        model.append(ckpt.fuse().eval() if fuse and hasattr(ckpt, 'fuse') else ckpt.eval())  # model in eval mode
+        ensemble.append(model.fuse().eval() if fuse and hasattr(model, 'fuse') else model.eval())  # model in eval mode
 
     # Module compatibility updates
-    for m in model.modules():
+    for m in ensemble.modules():
         t = type(m)
         if t in (nn.Hardswish, nn.LeakyReLU, nn.ReLU, nn.ReLU6, nn.SiLU, Detect, Segment):
             m.inplace = inplace  # torch 1.7.0 compatibility
         elif t is nn.Upsample and not hasattr(m, 'recompute_scale_factor'):
             m.recompute_scale_factor = None  # torch 1.11.0 compatibility
 
     # Return model
-    if len(model) == 1:
-        return model[-1]
+    if len(ensemble) == 1:
+        return ensemble[-1]
 
     # Return ensemble
-    print(f'Ensemble created with {weights}\n')
+    LOGGER.info(f'Ensemble created with {weights}\n')
     for k in 'names', 'nc', 'yaml':
-        setattr(model, k, getattr(model[0], k))
-    model.stride = model[torch.argmax(torch.tensor([m.stride.max() for m in model])).int()].stride  # max stride
-    assert all(model[0].nc == m.nc for m in model), f'Models have different class counts: {[m.nc for m in model]}'
-    return model
+        setattr(ensemble, k, getattr(ensemble[0], k))
+    ensemble.stride = ensemble[torch.argmax(torch.tensor([m.stride.max() for m in ensemble])).int()].stride
+    assert all(ensemble[0].nc == m.nc for m in ensemble), f'Models differ in class counts {[m.nc for m in ensemble]}'
+    return ensemble
 
 
 def attempt_load_one_weight(weight, device=None, inplace=True, fuse=False):
-    # Loads a single model weights
-    from ultralytics.yolo.utils.downloads import attempt_download
-
-    ckpt = torch.load(attempt_download(weight), map_location='cpu')  # load
-    args = {**DEFAULT_CONFIG_DICT, **ckpt['train_args']}  # combine model and default args, preferring model args
+    """Loads a single model weights."""
+    ckpt, weight = torch_safe_load(weight)  # load ckpt
+    args = {**DEFAULT_CFG_DICT, **ckpt['train_args']}  # combine model and default args, preferring model args
     model = (ckpt.get('ema') or ckpt['model']).to(device).float()  # FP32 model
 
     # Model compatibility updates
-    model.args = {k: v for k, v in args.items() if k in DEFAULT_CONFIG_KEYS}  # attach args to model
+    model.args = {k: v for k, v in args.items() if k in DEFAULT_CFG_KEYS}  # attach args to model
     model.pt_path = weight  # attach *.pt file path to model
+    model.task = guess_model_task(model)
     if not hasattr(model, 'stride'):
         model.stride = torch.tensor([32.])
 
     model = model.fuse().eval() if fuse and hasattr(model, 'fuse') else model.eval()  # model in eval mode
 
     # Module compatibility updates
     for m in model.modules():
@@ -362,50 +436,63 @@
             m.recompute_scale_factor = None  # torch 1.11.0 compatibility
 
     # Return model and ckpt
     return model, ckpt
 
 
 def parse_model(d, ch, verbose=True):  # model_dict, input_channels(3)
-    # Parse a YOLO model.yaml dictionary
-    if verbose:
-        LOGGER.info(f"\n{'':>3}{'from':>20}{'n':>3}{'params':>10}  {'module':<45}{'arguments':<30}")
-    nc, gd, gw, act = d['nc'], d['depth_multiple'], d['width_multiple'], d.get('activation')
+    # Parse a YOLO model.yaml dictionary into a PyTorch model
+    import ast
+
+    # Args
+    max_channels = float('inf')
+    nc, act, scales = (d.get(x) for x in ('nc', 'act', 'scales'))
+    depth, width, kpt_shape = (d.get(x, 1.0) for x in ('depth_multiple', 'width_multiple', 'kpt_shape'))
+    if scales:
+        scale = d.get('scale')
+        if not scale:
+            scale = tuple(scales.keys())[0]
+            LOGGER.warning(f"WARNING ⚠️ no model scale passed. Assuming scale='{scale}'.")
+        depth, width, max_channels = scales[scale]
+
     if act:
         Conv.default_act = eval(act)  # redefine default activation, i.e. Conv.default_act = nn.SiLU()
         if verbose:
             LOGGER.info(f"{colorstr('activation:')} {act}")  # print
 
+    if verbose:
+        LOGGER.info(f"\n{'':>3}{'from':>20}{'n':>3}{'params':>10}  {'module':<45}{'arguments':<30}")
+    ch = [ch]
     layers, save, c2 = [], [], ch[-1]  # layers, savelist, ch out
     for i, (f, n, m, args) in enumerate(d['backbone'] + d['head']):  # from, number, module, args
-        m = eval(m) if isinstance(m, str) else m  # eval strings
+        m = getattr(torch.nn, m[3:]) if 'nn.' in m else globals()[m]  # get module
         for j, a in enumerate(args):
-            with contextlib.suppress(NameError):
-                args[j] = eval(a) if isinstance(a, str) else a  # eval strings
-
-        n = n_ = max(round(n * gd), 1) if n > 1 else n  # depth gain
-        if m in {
-                Classify, Conv, ConvTranspose, GhostConv, Bottleneck, GhostBottleneck, SPP, SPPF, DWConv, Focus,
-                BottleneckCSP, C1, C2, C2f, C3, C3TR, C3Ghost, nn.ConvTranspose2d, DWConvTranspose2d, C3x}:
+            if isinstance(a, str):
+                with contextlib.suppress(ValueError):
+                    args[j] = locals()[a] if a in locals() else ast.literal_eval(a)
+
+        n = n_ = max(round(n * depth), 1) if n > 1 else n  # depth gain
+        if m in (Classify, Conv, ConvTranspose, GhostConv, Bottleneck, GhostBottleneck, SPP, SPPF, DWConv, Focus,
+                 BottleneckCSP, C1, C2, C2f, C3, C3TR, C3Ghost, nn.ConvTranspose2d, DWConvTranspose2d, C3x):
             c1, c2 = ch[f], args[0]
             if c2 != nc:  # if c2 not equal to number of classes (i.e. for Classify() output)
-                c2 = make_divisible(c2 * gw, 8)
+                c2 = make_divisible(min(c2, max_channels) * width, 8)
 
             args = [c1, c2, *args[1:]]
-            if m in {BottleneckCSP, C1, C2, C2f, C3, C3TR, C3Ghost, C3x}:
+            if m in (BottleneckCSP, C1, C2, C2f, C3, C3TR, C3Ghost, C3x):
                 args.insert(2, n)  # number of repeats
                 n = 1
         elif m is nn.BatchNorm2d:
             args = [ch[f]]
         elif m is Concat:
             c2 = sum(ch[x] for x in f)
-        elif m in {Detect, Segment}:
+        elif m in (Detect, Segment, Pose):
             args.append([ch[x] for x in f])
             if m is Segment:
-                args[2] = make_divisible(args[2] * gw, 8)
+                args[2] = make_divisible(min(args[2], max_channels) * width, 8)
         else:
             c2 = ch[f]
 
         m_ = nn.Sequential(*(m(*args) for _ in range(n))) if n > 1 else m(*args)  # module
         t = str(m)[8:-2].replace('__main__.', '')  # module type
         m.np = sum(x.numel() for x in m_.parameters())  # number params
         m_.i, m_.f, m_.type = i, f, t  # attach index, 'from' index, type
@@ -413,7 +500,111 @@
             LOGGER.info(f'{i:>3}{str(f):>20}{n_:>3}{m.np:10.0f}  {t:<45}{str(args):<30}')  # print
         save.extend(x % i for x in ([f] if isinstance(f, int) else f) if x != -1)  # append to savelist
         layers.append(m_)
         if i == 0:
             ch = []
         ch.append(c2)
     return nn.Sequential(*layers), sorted(save)
+
+
+def yaml_model_load(path):
+    """Load a YOLOv8 model from a YAML file."""
+    import re
+
+    path = Path(path)
+    if path.stem in (f'yolov{d}{x}6' for x in 'nsmlx' for d in (5, 8)):
+        new_stem = re.sub(r'(\d+)([nslmx])6(.+)?$', r'\1\2-p6\3', path.stem)
+        LOGGER.warning(f'WARNING ⚠️ Ultralytics YOLO P6 models now use -p6 suffix. Renaming {path.stem} to {new_stem}.')
+        path = path.with_stem(new_stem)
+
+    unified_path = re.sub(r'(\d+)([nslmx])(.+)?$', r'\1\3', str(path))  # i.e. yolov8x.yaml -> yolov8.yaml
+    yaml_file = check_yaml(unified_path, hard=False) or check_yaml(path)
+    d = yaml_load(yaml_file)  # model dict
+    d['scale'] = guess_model_scale(path)
+    d['yaml_file'] = str(path)
+    return d
+
+
+def guess_model_scale(model_path):
+    """
+    Takes a path to a YOLO model's YAML file as input and extracts the size character of the model's scale.
+    The function uses regular expression matching to find the pattern of the model scale in the YAML file name,
+    which is denoted by n, s, m, l, or x. The function returns the size character of the model scale as a string.
+
+    Args:
+        model_path (str) or (Path): The path to the YOLO model's YAML file.
+
+    Returns:
+        (str): The size character of the model's scale, which can be n, s, m, l, or x.
+    """
+    with contextlib.suppress(AttributeError):
+        import re
+        return re.search(r'yolov\d+([nslmx])', Path(model_path).stem).group(1)  # n, s, m, l, or x
+    return ''
+
+
+def guess_model_task(model):
+    """
+    Guess the task of a PyTorch model from its architecture or configuration.
+
+    Args:
+        model (nn.Module) or (dict): PyTorch model or model configuration in YAML format.
+
+    Returns:
+        (str): Task of the model ('detect', 'segment', 'classify', 'pose').
+
+    Raises:
+        SyntaxError: If the task of the model could not be determined.
+    """
+
+    def cfg2task(cfg):
+        """Guess from YAML dictionary."""
+        m = cfg['head'][-1][-2].lower()  # output module name
+        if m in ('classify', 'classifier', 'cls', 'fc'):
+            return 'classify'
+        if m == 'detect':
+            return 'detect'
+        if m == 'segment':
+            return 'segment'
+        if m == 'pose':
+            return 'pose'
+
+    # Guess from model cfg
+    if isinstance(model, dict):
+        with contextlib.suppress(Exception):
+            return cfg2task(model)
+
+    # Guess from PyTorch model
+    if isinstance(model, nn.Module):  # PyTorch model
+        for x in 'model.args', 'model.model.args', 'model.model.model.args':
+            with contextlib.suppress(Exception):
+                return eval(x)['task']
+        for x in 'model.yaml', 'model.model.yaml', 'model.model.model.yaml':
+            with contextlib.suppress(Exception):
+                return cfg2task(eval(x))
+
+        for m in model.modules():
+            if isinstance(m, Detect):
+                return 'detect'
+            elif isinstance(m, Segment):
+                return 'segment'
+            elif isinstance(m, Classify):
+                return 'classify'
+            elif isinstance(m, Pose):
+                return 'pose'
+
+    # Guess from model filename
+    if isinstance(model, (str, Path)):
+        model = Path(model)
+        if '-seg' in model.stem or 'segment' in model.parts:
+            return 'segment'
+        elif '-cls' in model.stem or 'classify' in model.parts:
+            return 'classify'
+        elif '-pose' in model.stem or 'pose' in model.parts:
+            return 'pose'
+        elif 'detect' in model.parts:
+            return 'detect'
+
+    # Unable to determine task from model
+    LOGGER.warning("WARNING ⚠️ Unable to automatically guess model task, assuming 'task=detect'. "
+                   "Explicitly define task for your model, i.e. 'task=detect', 'segment', 'classify', or 'pose'.")
+    return 'detect'  # assume detect
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/data/augment.py` & `ultralytics-8.0.90/ultralytics/yolo/data/augment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import math
 import random
 from copy import deepcopy
 
 import cv2
 import numpy as np
@@ -10,131 +10,148 @@
 import torchvision.transforms as T
 
 from ..utils import LOGGER, colorstr
 from ..utils.checks import check_version
 from ..utils.instance import Instances
 from ..utils.metrics import bbox_ioa
 from ..utils.ops import segment2box
-from .utils import IMAGENET_MEAN, IMAGENET_STD, polygons2masks, polygons2masks_overlap
+from .utils import polygons2masks, polygons2masks_overlap
+
+POSE_FLIPLR_INDEX = [0, 2, 1, 4, 3, 6, 5, 8, 7, 10, 9, 12, 11, 14, 13, 16, 15]
 
 
 # TODO: we might need a BaseTransform to make all these augments be compatible with both classification and semantic
 class BaseTransform:
 
     def __init__(self) -> None:
         pass
 
     def apply_image(self, labels):
+        """Applies image transformation to labels."""
         pass
 
     def apply_instances(self, labels):
+        """Applies transformations to input 'labels' and returns object instances."""
         pass
 
     def apply_semantic(self, labels):
+        """Applies semantic segmentation to an image."""
         pass
 
     def __call__(self, labels):
+        """Applies label transformations to an image, instances and semantic masks."""
         self.apply_image(labels)
         self.apply_instances(labels)
         self.apply_semantic(labels)
 
 
 class Compose:
 
     def __init__(self, transforms):
+        """Initializes the Compose object with a list of transforms."""
         self.transforms = transforms
 
     def __call__(self, data):
+        """Applies a series of transformations to input data."""
         for t in self.transforms:
             data = t(data)
         return data
 
     def append(self, transform):
+        """Appends a new transform to the existing list of transforms."""
         self.transforms.append(transform)
 
     def tolist(self):
+        """Converts list of transforms to a standard Python list."""
         return self.transforms
 
     def __repr__(self):
-        format_string = f"{self.__class__.__name__}("
+        """Return string representation of object."""
+        format_string = f'{self.__class__.__name__}('
         for t in self.transforms:
-            format_string += "\n"
-            format_string += f"    {t}"
-        format_string += "\n)"
+            format_string += '\n'
+            format_string += f'    {t}'
+        format_string += '\n)'
         return format_string
 
 
 class BaseMixTransform:
-    """This implementation is from mmyolo"""
+    """This implementation is from mmyolo."""
 
     def __init__(self, dataset, pre_transform=None, p=0.0) -> None:
         self.dataset = dataset
         self.pre_transform = pre_transform
         self.p = p
 
     def __call__(self, labels):
+        """Applies pre-processing transforms and mixup/mosaic transforms to labels data."""
         if random.uniform(0, 1) > self.p:
             return labels
 
-        # get index of one or three other images
+        # Get index of one or three other images
         indexes = self.get_indexes()
         if isinstance(indexes, int):
             indexes = [indexes]
 
-        # get images information will be used for Mosaic or MixUp
+        # Get images information will be used for Mosaic or MixUp
         mix_labels = [self.dataset.get_label_info(i) for i in indexes]
 
         if self.pre_transform is not None:
             for i, data in enumerate(mix_labels):
                 mix_labels[i] = self.pre_transform(data)
-        labels["mix_labels"] = mix_labels
+        labels['mix_labels'] = mix_labels
 
         # Mosaic or MixUp
         labels = self._mix_transform(labels)
-        labels.pop("mix_labels", None)
+        labels.pop('mix_labels', None)
         return labels
 
     def _mix_transform(self, labels):
+        """Applies MixUp or Mosaic augmentation to the label dictionary."""
         raise NotImplementedError
 
     def get_indexes(self):
+        """Gets a list of shuffled indexes for mosaic augmentation."""
         raise NotImplementedError
 
 
 class Mosaic(BaseMixTransform):
     """Mosaic augmentation.
     Args:
         imgsz (Sequence[int]): Image size after mosaic pipeline of single
             image. The shape order should be (height, width).
             Default to (640, 640).
     """
 
     def __init__(self, dataset, imgsz=640, p=1.0, border=(0, 0)):
-        assert 0 <= p <= 1.0, "The probability should be in range [0, 1]. " f"got {p}."
+        """Initializes the object with a dataset, image size, probability, and border."""
+        assert 0 <= p <= 1.0, 'The probability should be in range [0, 1]. ' f'got {p}.'
         super().__init__(dataset=dataset, p=p)
         self.dataset = dataset
         self.imgsz = imgsz
         self.border = border
 
     def get_indexes(self):
+        """Return a list of 3 random indexes from the dataset."""
         return [random.randint(0, len(self.dataset) - 1) for _ in range(3)]
 
     def _mix_transform(self, labels):
+        """Apply mixup transformation to the input image and labels."""
         mosaic_labels = []
-        assert labels.get("rect_shape", None) is None, "rect and mosaic is exclusive."
-        assert len(labels.get("mix_labels", [])) > 0, "There are no other images for mosaic augment."
+        assert labels.get('rect_shape', None) is None, 'rect and mosaic is exclusive.'
+        assert len(labels.get('mix_labels', [])) > 0, 'There are no other images for mosaic augment.'
         s = self.imgsz
         yc, xc = (int(random.uniform(-x, 2 * s + x)) for x in self.border)  # mosaic center x, y
         for i in range(4):
-            labels_patch = (labels if i == 0 else labels["mix_labels"][i - 1]).copy()
+            labels_patch = labels if i == 0 else labels['mix_labels'][i - 1]
             # Load image
-            img = labels_patch["img"]
-            h, w = labels_patch["resized_shape"]
+            img = labels_patch['img']
+            h, w = labels_patch.pop('resized_shape')
 
-            # place img in img4
+            # Place img in img4
             if i == 0:  # top left
                 img4 = np.full((s * 2, s * 2, img.shape[2]), 114, dtype=np.uint8)  # base image with 4 tiles
                 x1a, y1a, x2a, y2a = max(xc - w, 0), max(yc - h, 0), xc, yc  # xmin, ymin, xmax, ymax (large image)
                 x1b, y1b, x2b, y2b = w - (x2a - x1a), h - (y2a - y1a), w, h  # xmin, ymin, xmax, ymax (small image)
             elif i == 1:  # top right
                 x1a, y1a, x2a, y2a = xc, max(yc - h, 0), min(xc + w, s * 2), yc
                 x1b, y1b, x2b, y2b = 0, h - (y2a - y1a), min(w, x2a - x1a), h
@@ -148,227 +165,244 @@
             img4[y1a:y2a, x1a:x2a] = img[y1b:y2b, x1b:x2b]  # img4[ymin:ymax, xmin:xmax]
             padw = x1a - x1b
             padh = y1a - y1b
 
             labels_patch = self._update_labels(labels_patch, padw, padh)
             mosaic_labels.append(labels_patch)
         final_labels = self._cat_labels(mosaic_labels)
-        final_labels["img"] = img4
+        final_labels['img'] = img4
         return final_labels
 
     def _update_labels(self, labels, padw, padh):
-        """Update labels"""
-        nh, nw = labels["img"].shape[:2]
-        labels["instances"].convert_bbox(format="xyxy")
-        labels["instances"].denormalize(nw, nh)
-        labels["instances"].add_padding(padw, padh)
+        """Update labels."""
+        nh, nw = labels['img'].shape[:2]
+        labels['instances'].convert_bbox(format='xyxy')
+        labels['instances'].denormalize(nw, nh)
+        labels['instances'].add_padding(padw, padh)
         return labels
 
     def _cat_labels(self, mosaic_labels):
+        """Return labels with mosaic border instances clipped."""
         if len(mosaic_labels) == 0:
             return {}
         cls = []
         instances = []
         for labels in mosaic_labels:
-            cls.append(labels["cls"])
-            instances.append(labels["instances"])
+            cls.append(labels['cls'])
+            instances.append(labels['instances'])
         final_labels = {
-            "ori_shape": mosaic_labels[0]["ori_shape"],
-            "resized_shape": (self.imgsz * 2, self.imgsz * 2),
-            "im_file": mosaic_labels[0]["im_file"],
-            "cls": np.concatenate(cls, 0),
-            "instances": Instances.concatenate(instances, axis=0)}
-        final_labels["instances"].clip(self.imgsz * 2, self.imgsz * 2)
+            'im_file': mosaic_labels[0]['im_file'],
+            'ori_shape': mosaic_labels[0]['ori_shape'],
+            'resized_shape': (self.imgsz * 2, self.imgsz * 2),
+            'cls': np.concatenate(cls, 0),
+            'instances': Instances.concatenate(instances, axis=0),
+            'mosaic_border': self.border}
+        final_labels['instances'].clip(self.imgsz * 2, self.imgsz * 2)
         return final_labels
 
 
 class MixUp(BaseMixTransform):
 
     def __init__(self, dataset, pre_transform=None, p=0.0) -> None:
         super().__init__(dataset=dataset, pre_transform=pre_transform, p=p)
 
     def get_indexes(self):
+        """Get a random index from the dataset."""
         return random.randint(0, len(self.dataset) - 1)
 
     def _mix_transform(self, labels):
-        # Applies MixUp augmentation https://arxiv.org/pdf/1710.09412.pdf
+        """Applies MixUp augmentation https://arxiv.org/pdf/1710.09412.pdf."""
         r = np.random.beta(32.0, 32.0)  # mixup ratio, alpha=beta=32.0
-        labels2 = labels["mix_labels"][0]
-        labels["img"] = (labels["img"] * r + labels2["img"] * (1 - r)).astype(np.uint8)
-        labels["instances"] = Instances.concatenate([labels["instances"], labels2["instances"]], axis=0)
-        labels["cls"] = np.concatenate([labels["cls"], labels2["cls"]], 0)
+        labels2 = labels['mix_labels'][0]
+        labels['img'] = (labels['img'] * r + labels2['img'] * (1 - r)).astype(np.uint8)
+        labels['instances'] = Instances.concatenate([labels['instances'], labels2['instances']], axis=0)
+        labels['cls'] = np.concatenate([labels['cls'], labels2['cls']], 0)
         return labels
 
 
 class RandomPerspective:
 
-    def __init__(self, degrees=0.0, translate=0.1, scale=0.5, shear=0.0, perspective=0.0, border=(0, 0)):
+    def __init__(self,
+                 degrees=0.0,
+                 translate=0.1,
+                 scale=0.5,
+                 shear=0.0,
+                 perspective=0.0,
+                 border=(0, 0),
+                 pre_transform=None):
         self.degrees = degrees
         self.translate = translate
         self.scale = scale
         self.shear = shear
         self.perspective = perspective
-        # mosaic border
+        # Mosaic border
         self.border = border
+        self.pre_transform = pre_transform
 
-    def affine_transform(self, img):
-        # Center
-        C = np.eye(3)
+    def affine_transform(self, img, border):
+        """Center."""
+        C = np.eye(3, dtype=np.float32)
 
         C[0, 2] = -img.shape[1] / 2  # x translation (pixels)
         C[1, 2] = -img.shape[0] / 2  # y translation (pixels)
 
         # Perspective
-        P = np.eye(3)
+        P = np.eye(3, dtype=np.float32)
         P[2, 0] = random.uniform(-self.perspective, self.perspective)  # x perspective (about y)
         P[2, 1] = random.uniform(-self.perspective, self.perspective)  # y perspective (about x)
 
         # Rotation and Scale
-        R = np.eye(3)
+        R = np.eye(3, dtype=np.float32)
         a = random.uniform(-self.degrees, self.degrees)
         # a += random.choice([-180, -90, 0, 90])  # add 90deg rotations to small rotations
         s = random.uniform(1 - self.scale, 1 + self.scale)
         # s = 2 ** random.uniform(-scale, scale)
         R[:2] = cv2.getRotationMatrix2D(angle=a, center=(0, 0), scale=s)
 
         # Shear
-        S = np.eye(3)
+        S = np.eye(3, dtype=np.float32)
         S[0, 1] = math.tan(random.uniform(-self.shear, self.shear) * math.pi / 180)  # x shear (deg)
         S[1, 0] = math.tan(random.uniform(-self.shear, self.shear) * math.pi / 180)  # y shear (deg)
 
         # Translation
-        T = np.eye(3)
+        T = np.eye(3, dtype=np.float32)
         T[0, 2] = random.uniform(0.5 - self.translate, 0.5 + self.translate) * self.size[0]  # x translation (pixels)
         T[1, 2] = random.uniform(0.5 - self.translate, 0.5 + self.translate) * self.size[1]  # y translation (pixels)
 
         # Combined rotation matrix
         M = T @ S @ R @ P @ C  # order of operations (right to left) is IMPORTANT
-        # affine image
-        if (self.border[0] != 0) or (self.border[1] != 0) or (M != np.eye(3)).any():  # image changed
+        # Affine image
+        if (border[0] != 0) or (border[1] != 0) or (M != np.eye(3)).any():  # image changed
             if self.perspective:
                 img = cv2.warpPerspective(img, M, dsize=self.size, borderValue=(114, 114, 114))
             else:  # affine
                 img = cv2.warpAffine(img, M[:2], dsize=self.size, borderValue=(114, 114, 114))
         return img, M, s
 
     def apply_bboxes(self, bboxes, M):
-        """apply affine to bboxes only.
+        """
+        Apply affine to bboxes only.
 
         Args:
-            bboxes(ndarray): list of bboxes, xyxy format, with shape (num_bboxes, 4).
-            M(ndarray): affine matrix.
+            bboxes (ndarray): list of bboxes, xyxy format, with shape (num_bboxes, 4).
+            M (ndarray): affine matrix.
+
         Returns:
-            new_bboxes(ndarray): bboxes after affine, [num_bboxes, 4].
+            new_bboxes (ndarray): bboxes after affine, [num_bboxes, 4].
         """
         n = len(bboxes)
         if n == 0:
             return bboxes
 
-        xy = np.ones((n * 4, 3))
+        xy = np.ones((n * 4, 3), dtype=bboxes.dtype)
         xy[:, :2] = bboxes[:, [0, 1, 2, 3, 0, 3, 2, 1]].reshape(n * 4, 2)  # x1y1, x2y2, x1y2, x2y1
         xy = xy @ M.T  # transform
         xy = (xy[:, :2] / xy[:, 2:3] if self.perspective else xy[:, :2]).reshape(n, 8)  # perspective rescale or affine
 
-        # create new boxes
+        # Create new boxes
         x = xy[:, [0, 2, 4, 6]]
         y = xy[:, [1, 3, 5, 7]]
-        return np.concatenate((x.min(1), y.min(1), x.max(1), y.max(1))).reshape(4, n).T
+        return np.concatenate((x.min(1), y.min(1), x.max(1), y.max(1)), dtype=bboxes.dtype).reshape(4, n).T
 
     def apply_segments(self, segments, M):
-        """apply affine to segments and generate new bboxes from segments.
+        """
+        Apply affine to segments and generate new bboxes from segments.
 
         Args:
-            segments(ndarray): list of segments, [num_samples, 500, 2].
-            M(ndarray): affine matrix.
+            segments (ndarray): list of segments, [num_samples, 500, 2].
+            M (ndarray): affine matrix.
+
         Returns:
-            new_segments(ndarray): list of segments after affine, [num_samples, 500, 2].
-            new_bboxes(ndarray): bboxes after affine, [N, 4].
+            new_segments (ndarray): list of segments after affine, [num_samples, 500, 2].
+            new_bboxes (ndarray): bboxes after affine, [N, 4].
         """
         n, num = segments.shape[:2]
         if n == 0:
             return [], segments
 
-        xy = np.ones((n * num, 3))
+        xy = np.ones((n * num, 3), dtype=segments.dtype)
         segments = segments.reshape(-1, 2)
         xy[:, :2] = segments
         xy = xy @ M.T  # transform
         xy = xy[:, :2] / xy[:, 2:3]
         segments = xy.reshape(n, -1, 2)
         bboxes = np.stack([segment2box(xy, self.size[0], self.size[1]) for xy in segments], 0)
         return bboxes, segments
 
     def apply_keypoints(self, keypoints, M):
-        """apply affine to keypoints.
+        """
+        Apply affine to keypoints.
 
         Args:
-            keypoints(ndarray): keypoints, [N, 17, 2].
-            M(ndarray): affine matrix.
+            keypoints (ndarray): keypoints, [N, 17, 3].
+            M (ndarray): affine matrix.
+
         Return:
-            new_keypoints(ndarray): keypoints after affine, [N, 17, 2].
+            new_keypoints (ndarray): keypoints after affine, [N, 17, 3].
         """
-        n = len(keypoints)
+        n, nkpt = keypoints.shape[:2]
         if n == 0:
             return keypoints
-        new_keypoints = np.ones((n * 17, 3))
-        new_keypoints[:, :2] = keypoints.reshape(n * 17, 2)  # num_kpt is hardcoded to 17
-        new_keypoints = new_keypoints @ M.T  # transform
-        new_keypoints = (new_keypoints[:, :2] / new_keypoints[:, 2:3]).reshape(n, 34)  # perspective rescale or affine
-        new_keypoints[keypoints.reshape(-1, 34) == 0] = 0
-        x_kpts = new_keypoints[:, list(range(0, 34, 2))]
-        y_kpts = new_keypoints[:, list(range(1, 34, 2))]
-
-        x_kpts[np.logical_or.reduce((x_kpts < 0, x_kpts > self.size[0], y_kpts < 0, y_kpts > self.size[1]))] = 0
-        y_kpts[np.logical_or.reduce((x_kpts < 0, x_kpts > self.size[0], y_kpts < 0, y_kpts > self.size[1]))] = 0
-        new_keypoints[:, list(range(0, 34, 2))] = x_kpts
-        new_keypoints[:, list(range(1, 34, 2))] = y_kpts
-        return new_keypoints.reshape(n, 17, 2)
+        xy = np.ones((n * nkpt, 3), dtype=keypoints.dtype)
+        visible = keypoints[..., 2].reshape(n * nkpt, 1)
+        xy[:, :2] = keypoints[..., :2].reshape(n * nkpt, 2)
+        xy = xy @ M.T  # transform
+        xy = xy[:, :2] / xy[:, 2:3]  # perspective rescale or affine
+        out_mask = (xy[:, 0] < 0) | (xy[:, 1] < 0) | (xy[:, 0] > self.size[0]) | (xy[:, 1] > self.size[1])
+        visible[out_mask] = 0
+        return np.concatenate([xy, visible], axis=-1).reshape(n, nkpt, 3)
 
     def __call__(self, labels):
         """
         Affine images and targets.
 
         Args:
-            labels(Dict): a dict of `bboxes`, `segments`, `keypoints`.
+            labels (dict): a dict of `bboxes`, `segments`, `keypoints`.
         """
-        img = labels["img"]
-        cls = labels["cls"]
-        instances = labels.pop("instances")
-        # make sure the coord formats are right
-        instances.convert_bbox(format="xyxy")
+        if self.pre_transform and 'mosaic_border' not in labels:
+            labels = self.pre_transform(labels)
+            labels.pop('ratio_pad')  # do not need ratio pad
+
+        img = labels['img']
+        cls = labels['cls']
+        instances = labels.pop('instances')
+        # Make sure the coord formats are right
+        instances.convert_bbox(format='xyxy')
         instances.denormalize(*img.shape[:2][::-1])
 
-        self.size = img.shape[1] + self.border[1] * 2, img.shape[0] + self.border[0] * 2  # w, h
+        border = labels.pop('mosaic_border', self.border)
+        self.size = img.shape[1] + border[1] * 2, img.shape[0] + border[0] * 2  # w, h
         # M is affine matrix
         # scale for func:`box_candidates`
-        img, M, scale = self.affine_transform(img)
+        img, M, scale = self.affine_transform(img, border)
 
         bboxes = self.apply_bboxes(instances.bboxes, M)
 
         segments = instances.segments
         keypoints = instances.keypoints
-        # update bboxes if there are segments.
+        # Update bboxes if there are segments.
         if len(segments):
             bboxes, segments = self.apply_segments(segments, M)
 
         if keypoints is not None:
             keypoints = self.apply_keypoints(keypoints, M)
-        new_instances = Instances(bboxes, segments, keypoints, bbox_format="xyxy", normalized=False)
-        # clip
+        new_instances = Instances(bboxes, segments, keypoints, bbox_format='xyxy', normalized=False)
+        # Clip
         new_instances.clip(*self.size)
 
-        # filter instances
+        # Filter instances
         instances.scale(scale_w=scale, scale_h=scale, bbox_only=True)
-        # make the bboxes have the same scale with new_bboxes
+        # Make the bboxes have the same scale with new_bboxes
         i = self.box_candidates(box1=instances.bboxes.T,
                                 box2=new_instances.bboxes.T,
                                 area_thr=0.01 if len(segments) else 0.10)
-        labels["instances"] = new_instances[i]
-        labels["cls"] = cls[i]
-        labels["img"] = img
-        labels["resized_shape"] = img.shape[:2]
+        labels['instances'] = new_instances[i]
+        labels['cls'] = cls[i]
+        labels['img'] = img
+        labels['resized_shape'] = img.shape[:2]
         return labels
 
     def box_candidates(self, box1, box2, wh_thr=2, ar_thr=100, area_thr=0.1, eps=1e-16):  # box1(4,n), box2(4,n)
         # Compute box candidates: box1 before augment, box2 after augment, wh_thr (pixels), aspect_ratio_thr, area_ratio
         w1, h1 = box1[2] - box1[0], box1[3] - box1[1]
         w2, h2 = box2[2] - box2[0], box2[3] - box2[1]
         ar = np.maximum(w2 / (h2 + eps), h2 / (w2 + eps))  # aspect ratio
@@ -379,15 +413,16 @@
 
     def __init__(self, hgain=0.5, sgain=0.5, vgain=0.5) -> None:
         self.hgain = hgain
         self.sgain = sgain
         self.vgain = vgain
 
     def __call__(self, labels):
-        img = labels["img"]
+        """Applies random horizontal or vertical flip to an image with a given probability."""
+        img = labels['img']
         if self.hgain or self.sgain or self.vgain:
             r = np.random.uniform(-1, 1, 3) * [self.hgain, self.sgain, self.vgain] + 1  # random gains
             hue, sat, val = cv2.split(cv2.cvtColor(img, cv2.COLOR_BGR2HSV))
             dtype = img.dtype  # uint8
 
             x = np.arange(0, 256, dtype=r.dtype)
             lut_hue = ((x * r[0]) % 180).astype(dtype)
@@ -397,57 +432,64 @@
             im_hsv = cv2.merge((cv2.LUT(hue, lut_hue), cv2.LUT(sat, lut_sat), cv2.LUT(val, lut_val)))
             cv2.cvtColor(im_hsv, cv2.COLOR_HSV2BGR, dst=img)  # no return needed
         return labels
 
 
 class RandomFlip:
 
-    def __init__(self, p=0.5, direction="horizontal") -> None:
-        assert direction in ["horizontal", "vertical"], f"Support direction `horizontal` or `vertical`, got {direction}"
+    def __init__(self, p=0.5, direction='horizontal', flip_idx=None) -> None:
+        assert direction in ['horizontal', 'vertical'], f'Support direction `horizontal` or `vertical`, got {direction}'
         assert 0 <= p <= 1.0
 
         self.p = p
         self.direction = direction
+        self.flip_idx = flip_idx
 
     def __call__(self, labels):
-        img = labels["img"]
-        instances = labels.pop("instances")
-        instances.convert_bbox(format="xywh")
+        """Resize image and padding for detection, instance segmentation, pose."""
+        img = labels['img']
+        instances = labels.pop('instances')
+        instances.convert_bbox(format='xywh')
         h, w = img.shape[:2]
         h = 1 if instances.normalized else h
         w = 1 if instances.normalized else w
 
         # Flip up-down
-        if self.direction == "vertical" and random.random() < self.p:
+        if self.direction == 'vertical' and random.random() < self.p:
             img = np.flipud(img)
             instances.flipud(h)
-        if self.direction == "horizontal" and random.random() < self.p:
+        if self.direction == 'horizontal' and random.random() < self.p:
             img = np.fliplr(img)
             instances.fliplr(w)
-        labels["img"] = np.ascontiguousarray(img)
-        labels["instances"] = instances
+            # For keypoints
+            if self.flip_idx is not None and instances.keypoints is not None:
+                instances.keypoints = np.ascontiguousarray(instances.keypoints[:, self.flip_idx, :])
+        labels['img'] = np.ascontiguousarray(img)
+        labels['instances'] = instances
         return labels
 
 
 class LetterBox:
-    """Resize image and padding for detection, instance segmentation, pose"""
+    """Resize image and padding for detection, instance segmentation, pose."""
 
     def __init__(self, new_shape=(640, 640), auto=False, scaleFill=False, scaleup=True, stride=32):
+        """Initialize LetterBox object with specific parameters."""
         self.new_shape = new_shape
         self.auto = auto
         self.scaleFill = scaleFill
         self.scaleup = scaleup
         self.stride = stride
 
     def __call__(self, labels=None, image=None):
+        """Return updated labels and image with added border."""
         if labels is None:
             labels = {}
-        img = labels.get("img") if image is None else image
+        img = labels.get('img') if image is None else image
         shape = img.shape[:2]  # current shape [height, width]
-        new_shape = labels.pop("rect_shape", self.new_shape)
+        new_shape = labels.pop('rect_shape', self.new_shape)
         if isinstance(new_shape, int):
             new_shape = (new_shape, new_shape)
 
         # Scale ratio (new / old)
         r = min(new_shape[0] / shape[0], new_shape[1] / shape[1])
         if not self.scaleup:  # only scale down, do not scale up (for better val mAP)
             r = min(r, 1.0)
@@ -461,58 +503,60 @@
         elif self.scaleFill:  # stretch
             dw, dh = 0.0, 0.0
             new_unpad = (new_shape[1], new_shape[0])
             ratio = new_shape[1] / shape[1], new_shape[0] / shape[0]  # width, height ratios
 
         dw /= 2  # divide padding into 2 sides
         dh /= 2
-        if labels.get("ratio_pad"):
-            labels["ratio_pad"] = (labels["ratio_pad"], (dw, dh))  # for evaluation
+        if labels.get('ratio_pad'):
+            labels['ratio_pad'] = (labels['ratio_pad'], (dw, dh))  # for evaluation
 
         if shape[::-1] != new_unpad:  # resize
             img = cv2.resize(img, new_unpad, interpolation=cv2.INTER_LINEAR)
         top, bottom = int(round(dh - 0.1)), int(round(dh + 0.1))
         left, right = int(round(dw - 0.1)), int(round(dw + 0.1))
         img = cv2.copyMakeBorder(img, top, bottom, left, right, cv2.BORDER_CONSTANT,
                                  value=(114, 114, 114))  # add border
 
         if len(labels):
             labels = self._update_labels(labels, ratio, dw, dh)
-            labels["img"] = img
-            labels["resized_shape"] = new_shape
+            labels['img'] = img
+            labels['resized_shape'] = new_shape
             return labels
         else:
             return img
 
     def _update_labels(self, labels, ratio, padw, padh):
-        """Update labels"""
-        labels["instances"].convert_bbox(format="xyxy")
-        labels["instances"].denormalize(*labels["img"].shape[:2][::-1])
-        labels["instances"].scale(*ratio)
-        labels["instances"].add_padding(padw, padh)
+        """Update labels."""
+        labels['instances'].convert_bbox(format='xyxy')
+        labels['instances'].denormalize(*labels['img'].shape[:2][::-1])
+        labels['instances'].scale(*ratio)
+        labels['instances'].add_padding(padw, padh)
         return labels
 
 
 class CopyPaste:
 
     def __init__(self, p=0.5) -> None:
         self.p = p
 
     def __call__(self, labels):
-        # Implement Copy-Paste augmentation https://arxiv.org/abs/2012.07177, labels as nx5 np.array(cls, xyxy)
-        im = labels["img"]
-        cls = labels["cls"]
-        instances = labels.pop("instances")
-        instances.convert_bbox(format="xyxy")
+        """Implement Copy-Paste augmentation https://arxiv.org/abs/2012.07177, labels as nx5 np.array(cls, xyxy)."""
+        im = labels['img']
+        cls = labels['cls']
+        h, w = im.shape[:2]
+        instances = labels.pop('instances')
+        instances.convert_bbox(format='xyxy')
+        instances.denormalize(w, h)
         if self.p and len(instances.segments):
             n = len(instances)
             _, w, _ = im.shape  # height, width, channels
             im_new = np.zeros(im.shape, np.uint8)
 
-            # calculate ioa first then select indexes randomly
+            # Calculate ioa first then select indexes randomly
             ins_flip = deepcopy(instances)
             ins_flip.fliplr(w)
 
             ioa = bbox_ioa(ins_flip.bboxes, instances.bboxes)  # intersection over area, (N, M)
             indexes = np.nonzero((ioa < 0.30).all(1))[0]  # (N, )
             n = len(indexes)
             for j in random.sample(list(indexes), k=round(self.p * n)):
@@ -520,68 +564,72 @@
                 instances = Instances.concatenate((instances, ins_flip[[j]]), axis=0)
                 cv2.drawContours(im_new, instances.segments[[j]].astype(np.int32), -1, (1, 1, 1), cv2.FILLED)
 
             result = cv2.flip(im, 1)  # augment segments (flip left-right)
             i = cv2.flip(im_new, 1).astype(bool)
             im[i] = result[i]  # cv2.imwrite('debug.jpg', im)  # debug
 
-        labels["img"] = im
-        labels["cls"] = cls
-        labels["instances"] = instances
+        labels['img'] = im
+        labels['cls'] = cls
+        labels['instances'] = instances
         return labels
 
 
 class Albumentations:
     # YOLOv8 Albumentations class (optional, only used if package is installed)
     def __init__(self, p=1.0):
+        """Initialize the transform object for YOLO bbox formatted params."""
         self.p = p
         self.transform = None
-        prefix = colorstr("albumentations: ")
+        prefix = colorstr('albumentations: ')
         try:
             import albumentations as A
 
-            check_version(A.__version__, "1.0.3", hard=True)  # version requirement
+            check_version(A.__version__, '1.0.3', hard=True)  # version requirement
 
             T = [
                 A.Blur(p=0.01),
                 A.MedianBlur(p=0.01),
                 A.ToGray(p=0.01),
                 A.CLAHE(p=0.01),
                 A.RandomBrightnessContrast(p=0.0),
                 A.RandomGamma(p=0.0),
-                A.ImageCompression(quality_lower=75, p=0.0),]  # transforms
-            self.transform = A.Compose(T, bbox_params=A.BboxParams(format="yolo", label_fields=["class_labels"]))
+                A.ImageCompression(quality_lower=75, p=0.0)]  # transforms
+            self.transform = A.Compose(T, bbox_params=A.BboxParams(format='yolo', label_fields=['class_labels']))
 
-            LOGGER.info(prefix + ", ".join(f"{x}".replace("always_apply=False, ", "") for x in T if x.p))
+            LOGGER.info(prefix + ', '.join(f'{x}'.replace('always_apply=False, ', '') for x in T if x.p))
         except ImportError:  # package not installed, skip
             pass
         except Exception as e:
-            LOGGER.info(f"{prefix}{e}")
+            LOGGER.info(f'{prefix}{e}')
 
     def __call__(self, labels):
-        im = labels["img"]
-        cls = labels["cls"]
+        """Generates object detections and returns a dictionary with detection results."""
+        im = labels['img']
+        cls = labels['cls']
         if len(cls):
-            labels["instances"].convert_bbox("xywh")
-            labels["instances"].normalize(*im.shape[:2][::-1])
-            bboxes = labels["instances"].bboxes
+            labels['instances'].convert_bbox('xywh')
+            labels['instances'].normalize(*im.shape[:2][::-1])
+            bboxes = labels['instances'].bboxes
             # TODO: add supports of segments and keypoints
             if self.transform and random.random() < self.p:
                 new = self.transform(image=im, bboxes=bboxes, class_labels=cls)  # transformed
-                labels["img"] = new["image"]
-                labels["cls"] = np.array(new["class_labels"])
-            labels["instances"].update(bboxes=bboxes)
+                if len(new['class_labels']) > 0:  # skip update if no bbox in new im
+                    labels['img'] = new['image']
+                    labels['cls'] = np.array(new['class_labels'])
+                    bboxes = np.array(new['bboxes'])
+            labels['instances'].update(bboxes=bboxes)
         return labels
 
 
 # TODO: technically this is not an augmentation, maybe we should put this to another files
 class Format:
 
     def __init__(self,
-                 bbox_format="xywh",
+                 bbox_format='xywh',
                  normalize=True,
                  return_mask=False,
                  return_keypoint=False,
                  mask_ratio=4,
                  mask_overlap=True,
                  batch_idx=True):
         self.bbox_format = bbox_format
@@ -589,155 +637,149 @@
         self.return_mask = return_mask  # set False when training detection only
         self.return_keypoint = return_keypoint
         self.mask_ratio = mask_ratio
         self.mask_overlap = mask_overlap
         self.batch_idx = batch_idx  # keep the batch indexes
 
     def __call__(self, labels):
-        img = labels["img"]
+        """Return formatted image, classes, bounding boxes & keypoints to be used by 'collate_fn'."""
+        img = labels.pop('img')
         h, w = img.shape[:2]
-        cls = labels.pop("cls")
-        instances = labels.pop("instances")
+        cls = labels.pop('cls')
+        instances = labels.pop('instances')
         instances.convert_bbox(format=self.bbox_format)
         instances.denormalize(w, h)
         nl = len(instances)
 
         if self.return_mask:
             if nl:
                 masks, instances, cls = self._format_segments(instances, cls, w, h)
                 masks = torch.from_numpy(masks)
             else:
                 masks = torch.zeros(1 if self.mask_overlap else nl, img.shape[0] // self.mask_ratio,
                                     img.shape[1] // self.mask_ratio)
-            labels["masks"] = masks
+            labels['masks'] = masks
         if self.normalize:
             instances.normalize(w, h)
-        labels["img"] = self._format_img(img)
-        labels["cls"] = torch.from_numpy(cls) if nl else torch.zeros(nl)
-        labels["bboxes"] = torch.from_numpy(instances.bboxes) if nl else torch.zeros((nl, 4))
+        labels['img'] = self._format_img(img)
+        labels['cls'] = torch.from_numpy(cls) if nl else torch.zeros(nl)
+        labels['bboxes'] = torch.from_numpy(instances.bboxes) if nl else torch.zeros((nl, 4))
         if self.return_keypoint:
-            labels["keypoints"] = torch.from_numpy(instances.keypoints) if nl else torch.zeros((nl, 17, 2))
-        # then we can use collate_fn
+            labels['keypoints'] = torch.from_numpy(instances.keypoints)
+        # Then we can use collate_fn
         if self.batch_idx:
-            labels["batch_idx"] = torch.zeros(nl)
+            labels['batch_idx'] = torch.zeros(nl)
         return labels
 
     def _format_img(self, img):
+        """Format the image for YOLOv5 from Numpy array to PyTorch tensor."""
         if len(img.shape) < 3:
             img = np.expand_dims(img, -1)
         img = np.ascontiguousarray(img.transpose(2, 0, 1)[::-1])
         img = torch.from_numpy(img)
         return img
 
     def _format_segments(self, instances, cls, w, h):
-        """convert polygon points to bitmap"""
+        """convert polygon points to bitmap."""
         segments = instances.segments
         if self.mask_overlap:
             masks, sorted_idx = polygons2masks_overlap((h, w), segments, downsample_ratio=self.mask_ratio)
             masks = masks[None]  # (640, 640) -> (1, 640, 640)
             instances = instances[sorted_idx]
             cls = cls[sorted_idx]
         else:
             masks = polygons2masks((h, w), segments, color=1, downsample_ratio=self.mask_ratio)
 
         return masks, instances, cls
 
 
-def mosaic_transforms(dataset, imgsz, hyp):
+def v8_transforms(dataset, imgsz, hyp):
+    """Convert images to a size suitable for YOLOv8 training."""
     pre_transform = Compose([
         Mosaic(dataset, imgsz=imgsz, p=hyp.mosaic, border=[-imgsz // 2, -imgsz // 2]),
         CopyPaste(p=hyp.copy_paste),
         RandomPerspective(
             degrees=hyp.degrees,
             translate=hyp.translate,
             scale=hyp.scale,
             shear=hyp.shear,
             perspective=hyp.perspective,
-            border=[-imgsz // 2, -imgsz // 2],
-        ),])
+            pre_transform=LetterBox(new_shape=(imgsz, imgsz)),
+        )])
+    flip_idx = dataset.data.get('flip_idx', None)  # for keypoints augmentation
+    if dataset.use_keypoints and flip_idx is None and hyp.fliplr > 0.0:
+        hyp.fliplr = 0.0
+        LOGGER.warning("WARNING ⚠️ No `flip_idx` provided while training keypoints, setting augmentation 'fliplr=0.0'")
     return Compose([
         pre_transform,
         MixUp(dataset, pre_transform=pre_transform, p=hyp.mixup),
         Albumentations(p=1.0),
         RandomHSV(hgain=hyp.hsv_h, sgain=hyp.hsv_s, vgain=hyp.hsv_v),
-        RandomFlip(direction="vertical", p=hyp.flipud),
-        RandomFlip(direction="horizontal", p=hyp.fliplr),])  # transforms
-
-
-def affine_transforms(imgsz, hyp):
-    return Compose([
-        LetterBox(new_shape=(imgsz, imgsz)),
-        RandomPerspective(
-            degrees=hyp.degrees,
-            translate=hyp.translate,
-            scale=hyp.scale,
-            shear=hyp.shear,
-            perspective=hyp.perspective,
-            border=[0, 0],
-        ),
-        Albumentations(p=1.0),
-        RandomHSV(hgain=hyp.hsv_h, sgain=hyp.hsv_s, vgain=hyp.hsv_v),
-        RandomFlip(direction="vertical", p=hyp.flipud),
-        RandomFlip(direction="horizontal", p=hyp.fliplr),])  # transforms
+        RandomFlip(direction='vertical', p=hyp.flipud),
+        RandomFlip(direction='horizontal', p=hyp.fliplr, flip_idx=flip_idx)])  # transforms
 
 
 # Classification augmentations -----------------------------------------------------------------------------------------
-def classify_transforms(size=224):
+def classify_transforms(size=224, mean=(0.0, 0.0, 0.0), std=(1.0, 1.0, 1.0)):  # IMAGENET_MEAN, IMAGENET_STD
     # Transforms to apply if albumentations not installed
-    assert isinstance(size, int), f"ERROR: classify_transforms size {size} must be integer, not (list, tuple)"
-    # T.Compose([T.ToTensor(), T.Resize(size), T.CenterCrop(size), T.Normalize(IMAGENET_MEAN, IMAGENET_STD)])
-    return T.Compose([CenterCrop(size), ToTensor(), T.Normalize(IMAGENET_MEAN, IMAGENET_STD)])
+    if not isinstance(size, int):
+        raise TypeError(f'classify_transforms() size {size} must be integer, not (list, tuple)')
+    if any(mean) or any(std):
+        return T.Compose([CenterCrop(size), ToTensor(), T.Normalize(mean, std, inplace=True)])
+    else:
+        return T.Compose([CenterCrop(size), ToTensor()])
 
 
 def classify_albumentations(
         augment=True,
         size=224,
         scale=(0.08, 1.0),
         hflip=0.5,
         vflip=0.0,
         jitter=0.4,
-        mean=IMAGENET_MEAN,
-        std=IMAGENET_STD,
+        mean=(0.0, 0.0, 0.0),  # IMAGENET_MEAN
+        std=(1.0, 1.0, 1.0),  # IMAGENET_STD
         auto_aug=False,
 ):
     # YOLOv8 classification Albumentations (optional, only used if package is installed)
-    prefix = colorstr("albumentations: ")
+    prefix = colorstr('albumentations: ')
     try:
         import albumentations as A
         from albumentations.pytorch import ToTensorV2
 
-        check_version(A.__version__, "1.0.3", hard=True)  # version requirement
+        check_version(A.__version__, '1.0.3', hard=True)  # version requirement
         if augment:  # Resize and crop
             T = [A.RandomResizedCrop(height=size, width=size, scale=scale)]
             if auto_aug:
                 # TODO: implement AugMix, AutoAug & RandAug in albumentation
-                LOGGER.info(f"{prefix}auto augmentations are currently not supported")
+                LOGGER.info(f'{prefix}auto augmentations are currently not supported')
             else:
                 if hflip > 0:
                     T += [A.HorizontalFlip(p=hflip)]
                 if vflip > 0:
                     T += [A.VerticalFlip(p=vflip)]
                 if jitter > 0:
-                    color_jitter = (float(jitter),) * 3  # repeat value for brightness, contrast, saturation, 0 hue
-                    T += [A.ColorJitter(*color_jitter, 0)]
+                    jitter = float(jitter)
+                    T += [A.ColorJitter(jitter, jitter, jitter, 0)]  # brightness, contrast, saturation, 0 hue
         else:  # Use fixed crop for eval set (reproducibility)
             T = [A.SmallestMaxSize(max_size=size), A.CenterCrop(height=size, width=size)]
         T += [A.Normalize(mean=mean, std=std), ToTensorV2()]  # Normalize and convert to Tensor
-        LOGGER.info(prefix + ", ".join(f"{x}".replace("always_apply=False, ", "") for x in T if x.p))
+        LOGGER.info(prefix + ', '.join(f'{x}'.replace('always_apply=False, ', '') for x in T if x.p))
         return A.Compose(T)
 
     except ImportError:  # package not installed, skip
         pass
     except Exception as e:
-        LOGGER.info(f"{prefix}{e}")
+        LOGGER.info(f'{prefix}{e}')
 
 
 class ClassifyLetterBox:
     # YOLOv8 LetterBox class for image preprocessing, i.e. T.Compose([LetterBox(size), ToTensor()])
     def __init__(self, size=(640, 640), auto=False, stride=32):
+        """Resizes image and crops it to center with max dimensions 'h' and 'w'."""
         super().__init__()
         self.h, self.w = (size, size) if isinstance(size, int) else size
         self.auto = auto  # pass max size integer, automatically solve for short side using stride
         self.stride = stride  # used with auto
 
     def __call__(self, im):  # im = np.array HWC
         imh, imw = im.shape[:2]
@@ -749,27 +791,29 @@
         im_out[top:top + h, left:left + w] = cv2.resize(im, (w, h), interpolation=cv2.INTER_LINEAR)
         return im_out
 
 
 class CenterCrop:
     # YOLOv8 CenterCrop class for image preprocessing, i.e. T.Compose([CenterCrop(size), ToTensor()])
     def __init__(self, size=640):
+        """Converts an image from numpy array to PyTorch tensor."""
         super().__init__()
         self.h, self.w = (size, size) if isinstance(size, int) else size
 
     def __call__(self, im):  # im = np.array HWC
         imh, imw = im.shape[:2]
         m = min(imh, imw)  # min dimension
         top, left = (imh - m) // 2, (imw - m) // 2
         return cv2.resize(im[top:top + m, left:left + m], (self.w, self.h), interpolation=cv2.INTER_LINEAR)
 
 
 class ToTensor:
     # YOLOv8 ToTensor class for image preprocessing, i.e. T.Compose([LetterBox(size), ToTensor()])
     def __init__(self, half=False):
+        """Initialize YOLOv8 ToTensor object with optional half-precision support."""
         super().__init__()
         self.half = half
 
     def __call__(self, im):  # im = np.array HWC in BGR order
         im = np.ascontiguousarray(im.transpose((2, 0, 1))[::-1])  # HWC to CHW -> BGR to RGB -> contiguous
         im = torch.from_numpy(im)  # to torch
         im = im.half() if self.half else im.float()  # uint8 to fp16/32
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/data/base.py` & `ultralytics-8.0.90/ultralytics/yolo/data/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,165 +1,205 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import glob
 import math
 import os
+import random
+from copy import deepcopy
 from multiprocessing.pool import ThreadPool
 from pathlib import Path
 from typing import Optional
 
 import cv2
 import numpy as np
+import psutil
 from torch.utils.data import Dataset
 from tqdm import tqdm
 
-from ..utils import NUM_THREADS, TQDM_BAR_FORMAT
-from .utils import HELP_URL, IMG_FORMATS, LOCAL_RANK
+from ..utils import LOCAL_RANK, LOGGER, NUM_THREADS, TQDM_BAR_FORMAT
+from .utils import HELP_URL, IMG_FORMATS
 
 
 class BaseDataset(Dataset):
-    """Base Dataset.
+    """
+    Base dataset class for loading and processing image data.
+
     Args:
-        img_path (str): image path.
-        pipeline (dict): a dict of image transforms.
-        label_path (str): label path, this can also be an ann_file or other custom label path.
+        img_path (str): Path to the folder containing images.
+        imgsz (int, optional): Image size. Defaults to 640.
+        cache (bool, optional): Cache images to RAM or disk during training. Defaults to False.
+        augment (bool, optional): If True, data augmentation is applied. Defaults to True.
+        hyp (dict, optional): Hyperparameters to apply data augmentation. Defaults to None.
+        prefix (str, optional): Prefix to print in log messages. Defaults to ''.
+        rect (bool, optional): If True, rectangular training is used. Defaults to False.
+        batch_size (int, optional): Size of batches. Defaults to None.
+        stride (int, optional): Stride. Defaults to 32.
+        pad (float, optional): Padding. Defaults to 0.0.
+        single_cls (bool, optional): If True, single class training is used. Defaults to False.
+        classes (list): List of included classes. Default is None.
+
+    Attributes:
+        im_files (list): List of image file paths.
+        labels (list): List of label data dictionaries.
+        ni (int): Number of images in the dataset.
+        ims (list): List of loaded images.
+        npy_files (list): List of numpy file paths.
+        transforms (callable): Image transformation function.
     """
 
-    def __init__(
-        self,
-        img_path,
-        imgsz=640,
-        label_path=None,
-        cache=False,
-        augment=True,
-        hyp=None,
-        prefix="",
-        rect=False,
-        batch_size=None,
-        stride=32,
-        pad=0.5,
-        single_cls=False,
-    ):
+    def __init__(self,
+                 img_path,
+                 imgsz=640,
+                 cache=False,
+                 augment=True,
+                 hyp=None,
+                 prefix='',
+                 rect=False,
+                 batch_size=None,
+                 stride=32,
+                 pad=0.5,
+                 single_cls=False,
+                 classes=None):
         super().__init__()
         self.img_path = img_path
         self.imgsz = imgsz
-        self.label_path = label_path
         self.augment = augment
         self.single_cls = single_cls
         self.prefix = prefix
-
         self.im_files = self.get_img_files(self.img_path)
         self.labels = self.get_labels()
-        if self.single_cls:
-            self.update_labels(include_class=[])
-
-        self.ni = len(self.labels)
-
-        # rect stuff
+        self.update_labels(include_class=classes)  # single_cls and include_class
+        self.ni = len(self.labels)  # number of images
         self.rect = rect
         self.batch_size = batch_size
         self.stride = stride
         self.pad = pad
         if self.rect:
             assert self.batch_size is not None
             self.set_rectangle()
 
-        # cache stuff
+        # Cache stuff
+        if cache == 'ram' and not self.check_cache_ram():
+            cache = False
         self.ims = [None] * self.ni
-        self.npy_files = [Path(f).with_suffix(".npy") for f in self.im_files]
+        self.npy_files = [Path(f).with_suffix('.npy') for f in self.im_files]
         if cache:
             self.cache_images(cache)
 
-        # transforms
+        # Transforms
         self.transforms = self.build_transforms(hyp=hyp)
 
     def get_img_files(self, img_path):
         """Read image files."""
         try:
             f = []  # image files
             for p in img_path if isinstance(img_path, list) else [img_path]:
                 p = Path(p)  # os-agnostic
                 if p.is_dir():  # dir
-                    f += glob.glob(str(p / "**" / "*.*"), recursive=True)
-                    # f = list(p.rglob('*.*'))  # pathlib
+                    f += glob.glob(str(p / '**' / '*.*'), recursive=True)
+                    # F = list(p.rglob('*.*'))  # pathlib
                 elif p.is_file():  # file
                     with open(p) as t:
                         t = t.read().strip().splitlines()
                         parent = str(p.parent) + os.sep
-                        f += [x.replace("./", parent) if x.startswith("./") else x for x in t]  # local to global path
-                        # f += [p.parent / x.lstrip(os.sep) for x in t]  # local to global path (pathlib)
+                        f += [x.replace('./', parent) if x.startswith('./') else x for x in t]  # local to global path
+                        # F += [p.parent / x.lstrip(os.sep) for x in t]  # local to global path (pathlib)
                 else:
-                    raise FileNotFoundError(f"{self.prefix}{p} does not exist")
-            im_files = sorted(x.replace("/", os.sep) for x in f if x.split(".")[-1].lower() in IMG_FORMATS)
+                    raise FileNotFoundError(f'{self.prefix}{p} does not exist')
+            im_files = sorted(x.replace('/', os.sep) for x in f if x.split('.')[-1].lower() in IMG_FORMATS)
             # self.img_files = sorted([x for x in f if x.suffix[1:].lower() in IMG_FORMATS])  # pathlib
-            assert im_files, f"{self.prefix}No images found"
+            assert im_files, f'{self.prefix}No images found'
         except Exception as e:
-            raise FileNotFoundError(f"{self.prefix}Error loading data from {img_path}: {e}\n{HELP_URL}") from e
+            raise FileNotFoundError(f'{self.prefix}Error loading data from {img_path}\n{HELP_URL}') from e
         return im_files
 
     def update_labels(self, include_class: Optional[list]):
-        """include_class, filter labels to include only these classes (optional)"""
+        """include_class, filter labels to include only these classes (optional)."""
         include_class_array = np.array(include_class).reshape(1, -1)
         for i in range(len(self.labels)):
-            if include_class:
-                cls = self.labels[i]["cls"]
-                bboxes = self.labels[i]["bboxes"]
-                segments = self.labels[i]["segments"]
+            if include_class is not None:
+                cls = self.labels[i]['cls']
+                bboxes = self.labels[i]['bboxes']
+                segments = self.labels[i]['segments']
+                keypoints = self.labels[i]['keypoints']
                 j = (cls == include_class_array).any(1)
-                self.labels[i]["cls"] = cls[j]
-                self.labels[i]["bboxes"] = bboxes[j]
+                self.labels[i]['cls'] = cls[j]
+                self.labels[i]['bboxes'] = bboxes[j]
                 if segments:
-                    self.labels[i]["segments"] = segments[j]
+                    self.labels[i]['segments'] = [segments[si] for si, idx in enumerate(j) if idx]
+                if keypoints is not None:
+                    self.labels[i]['keypoints'] = keypoints[j]
             if self.single_cls:
-                self.labels[i]["cls"][:, 0] = 0
+                self.labels[i]['cls'][:, 0] = 0
 
     def load_image(self, i):
-        # Loads 1 image from dataset index 'i', returns (im, resized hw)
+        """Loads 1 image from dataset index 'i', returns (im, resized hw)."""
         im, f, fn = self.ims[i], self.im_files[i], self.npy_files[i]
         if im is None:  # not cached in RAM
             if fn.exists():  # load npy
                 im = np.load(fn)
             else:  # read image
                 im = cv2.imread(f)  # BGR
-                assert im is not None, f"Image Not Found {f}"
+                if im is None:
+                    raise FileNotFoundError(f'Image Not Found {f}')
             h0, w0 = im.shape[:2]  # orig hw
             r = self.imgsz / max(h0, w0)  # ratio
             if r != 1:  # if sizes are not equal
                 interp = cv2.INTER_LINEAR if (self.augment or r > 1) else cv2.INTER_AREA
                 im = cv2.resize(im, (math.ceil(w0 * r), math.ceil(h0 * r)), interpolation=interp)
             return im, (h0, w0), im.shape[:2]  # im, hw_original, hw_resized
         return self.ims[i], self.im_hw0[i], self.im_hw[i]  # im, hw_original, hw_resized
 
     def cache_images(self, cache):
-        # cache images to memory or disk
-        gb = 0  # Gigabytes of cached images
+        """Cache images to memory or disk."""
+        b, gb = 0, 1 << 30  # bytes of cached images, bytes per gigabytes
         self.im_hw0, self.im_hw = [None] * self.ni, [None] * self.ni
-        fcn = self.cache_images_to_disk if cache == "disk" else self.load_image
-        results = ThreadPool(NUM_THREADS).imap(fcn, range(self.ni))
-        pbar = tqdm(enumerate(results), total=self.ni, bar_format=TQDM_BAR_FORMAT, disable=LOCAL_RANK > 0)
-        for i, x in pbar:
-            if cache == "disk":
-                gb += self.npy_files[i].stat().st_size
-            else:  # 'ram'
-                self.ims[i], self.im_hw0[i], self.im_hw[i] = x  # im, hw_orig, hw_resized = load_image(self, i)
-                gb += self.ims[i].nbytes
-            pbar.desc = f"{self.prefix}Caching images ({gb / 1E9:.1f}GB {cache})"
-        pbar.close()
+        fcn = self.cache_images_to_disk if cache == 'disk' else self.load_image
+        with ThreadPool(NUM_THREADS) as pool:
+            results = pool.imap(fcn, range(self.ni))
+            pbar = tqdm(enumerate(results), total=self.ni, bar_format=TQDM_BAR_FORMAT, disable=LOCAL_RANK > 0)
+            for i, x in pbar:
+                if cache == 'disk':
+                    b += self.npy_files[i].stat().st_size
+                else:  # 'ram'
+                    self.ims[i], self.im_hw0[i], self.im_hw[i] = x  # im, hw_orig, hw_resized = load_image(self, i)
+                    b += self.ims[i].nbytes
+                pbar.desc = f'{self.prefix}Caching images ({b / gb:.1f}GB {cache})'
+            pbar.close()
 
     def cache_images_to_disk(self, i):
-        # Saves an image as an *.npy file for faster loading
+        """Saves an image as an *.npy file for faster loading."""
         f = self.npy_files[i]
         if not f.exists():
             np.save(f.as_posix(), cv2.imread(self.im_files[i]))
 
+    def check_cache_ram(self, safety_margin=0.5):
+        """Check image caching requirements vs available memory."""
+        b, gb = 0, 1 << 30  # bytes of cached images, bytes per gigabytes
+        n = min(self.ni, 30)  # extrapolate from 30 random images
+        for _ in range(n):
+            im = cv2.imread(random.choice(self.im_files))  # sample image
+            ratio = self.imgsz / max(im.shape[0], im.shape[1])  # max(h, w)  # ratio
+            b += im.nbytes * ratio ** 2
+        mem_required = b * self.ni / n * (1 + safety_margin)  # GB required to cache dataset into RAM
+        mem = psutil.virtual_memory()
+        cache = mem_required < mem.available  # to cache or not to cache, that is the question
+        if not cache:
+            LOGGER.info(f'{self.prefix}{mem_required / gb:.1f}GB RAM required to cache images '
+                        f'with {int(safety_margin * 100)}% safety margin but only '
+                        f'{mem.available / gb:.1f}/{mem.total / gb:.1f}GB available, '
+                        f"{'caching images ✅' if cache else 'not caching images ⚠️'}")
+        return cache
+
     def set_rectangle(self):
+        """Sets the shape of bounding boxes for YOLO detections as rectangles."""
         bi = np.floor(np.arange(self.ni) / self.batch_size).astype(int)  # batch index
         nb = bi[-1] + 1  # number of batches
 
-        s = np.array([x.pop("shape") for x in self.labels])  # hw
+        s = np.array([x.pop('shape') for x in self.labels])  # hw
         ar = s[:, 0] / s[:, 1]  # aspect ratio
         irect = ar.argsort()
         self.im_files = [self.im_files[i] for i in irect]
         self.labels = [self.labels[i] for i in irect]
         ar = ar[irect]
 
         # Set training image shapes
@@ -172,43 +212,45 @@
             elif mini > 1:
                 shapes[i] = [1, 1 / mini]
 
         self.batch_shapes = np.ceil(np.array(shapes) * self.imgsz / self.stride + self.pad).astype(int) * self.stride
         self.batch = bi  # batch index of image
 
     def __getitem__(self, index):
+        """Returns transformed label information for given index."""
         return self.transforms(self.get_label_info(index))
 
     def get_label_info(self, index):
-        label = self.labels[index].copy()
-        label["img"], label["ori_shape"], label["resized_shape"] = self.load_image(index)
-        label["ratio_pad"] = (
-            label["resized_shape"][0] / label["ori_shape"][0],
-            label["resized_shape"][1] / label["ori_shape"][1],
-        )  # for evaluation
+        """Get and return label information from the dataset."""
+        label = deepcopy(self.labels[index])  # requires deepcopy() https://github.com/ultralytics/ultralytics/pull/1948
+        label.pop('shape', None)  # shape is for rect, remove it
+        label['img'], label['ori_shape'], label['resized_shape'] = self.load_image(index)
+        label['ratio_pad'] = (label['resized_shape'][0] / label['ori_shape'][0],
+                              label['resized_shape'][1] / label['ori_shape'][1])  # for evaluation
         if self.rect:
-            label["rect_shape"] = self.batch_shapes[self.batch[index]]
+            label['rect_shape'] = self.batch_shapes[self.batch[index]]
         label = self.update_labels_info(label)
         return label
 
     def __len__(self):
+        """Returns the length of the labels list for the dataset."""
         return len(self.labels)
 
     def update_labels_info(self, label):
-        """custom your label format here"""
+        """custom your label format here."""
         return label
 
     def build_transforms(self, hyp=None):
         """Users can custom augmentations here
         like:
             if self.augment:
-                # training transforms
+                # Training transforms
                 return Compose([])
             else:
-                # val transforms
+                # Val transforms
                 return Compose([])
         """
         raise NotImplementedError
 
     def get_labels(self):
         """Users can custom their own format here.
         Make sure your output is a list with each element like below:
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/data/dataloaders/stream_loaders.py` & `ultralytics-8.0.90/ultralytics/yolo/data/dataloaders/stream_loaders.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,83 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import glob
 import math
 import os
 import time
+from dataclasses import dataclass
 from pathlib import Path
 from threading import Thread
 from urllib.parse import urlparse
 
 import cv2
 import numpy as np
+import requests
 import torch
 from PIL import Image
 
-from ultralytics.yolo.data.augment import LetterBox
 from ultralytics.yolo.data.utils import IMG_FORMATS, VID_FORMATS
 from ultralytics.yolo.utils import LOGGER, ROOT, is_colab, is_kaggle, ops
 from ultralytics.yolo.utils.checks import check_requirements
 
 
+@dataclass
+class SourceTypes:
+    webcam: bool = False
+    screenshot: bool = False
+    from_img: bool = False
+    tensor: bool = False
+
+
 class LoadStreams:
-    # YOLOv8 streamloader, i.e. `python detect.py --source 'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP streams`
-    def __init__(self, sources='file.streams', imgsz=640, stride=32, auto=True, transforms=None, vid_stride=1):
+    # YOLOv8 streamloader, i.e. `yolo predict source='rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP streams`
+    def __init__(self, sources='file.streams', imgsz=640, vid_stride=1):
+        """Initialize instance variables and check for consistent input stream shapes."""
         torch.backends.cudnn.benchmark = True  # faster for fixed-size inference
         self.mode = 'stream'
         self.imgsz = imgsz
-        self.stride = stride
         self.vid_stride = vid_stride  # video frame-rate stride
         sources = Path(sources).read_text().rsplit() if os.path.isfile(sources) else [sources]
         n = len(sources)
         self.sources = [ops.clean_str(x) for x in sources]  # clean source names for later
         self.imgs, self.fps, self.frames, self.threads = [None] * n, [0] * n, [0] * n, [None] * n
         for i, s in enumerate(sources):  # index, source
             # Start thread to read frames from video stream
             st = f'{i + 1}/{n}: {s}... '
             if urlparse(s).hostname in ('www.youtube.com', 'youtube.com', 'youtu.be'):  # if source is YouTube video
                 # YouTube format i.e. 'https://www.youtube.com/watch?v=Zgi9g1ksQHc' or 'https://youtu.be/Zgi9g1ksQHc'
                 check_requirements(('pafy', 'youtube_dl==2020.12.2'))
                 import pafy  # noqa
-                s = pafy.new(s).getbest(preftype="mp4").url  # YouTube URL
+                s = pafy.new(s).getbest(preftype='mp4').url  # YouTube URL
             s = eval(s) if s.isnumeric() else s  # i.e. s = '0' local webcam
-            if s == 0:
-                assert not is_colab(), '--source 0 webcam unsupported on Colab. Rerun command in a local environment.'
-                assert not is_kaggle(), '--source 0 webcam unsupported on Kaggle. Rerun command in a local environment.'
+            if s == 0 and (is_colab() or is_kaggle()):
+                raise NotImplementedError("'source=0' webcam not supported in Colab and Kaggle notebooks. "
+                                          "Try running 'source=0' in a local environment.")
             cap = cv2.VideoCapture(s)
-            assert cap.isOpened(), f'{st}Failed to open {s}'
+            if not cap.isOpened():
+                raise ConnectionError(f'{st}Failed to open {s}')
             w = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
             h = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
             fps = cap.get(cv2.CAP_PROP_FPS)  # warning: may return 0 or nan
             self.frames[i] = max(int(cap.get(cv2.CAP_PROP_FRAME_COUNT)), 0) or float('inf')  # infinite stream fallback
             self.fps[i] = max((fps if math.isfinite(fps) else 0) % 100, 0) or 30  # 30 FPS fallback
 
-            _, self.imgs[i] = cap.read()  # guarantee first frame
+            success, self.imgs[i] = cap.read()  # guarantee first frame
+            if not success or self.imgs[i] is None:
+                raise ConnectionError(f'{st}Failed to read images from {s}')
             self.threads[i] = Thread(target=self.update, args=([i, cap, s]), daemon=True)
-            LOGGER.info(f"{st} Success ({self.frames[i]} frames {w}x{h} at {self.fps[i]:.2f} FPS)")
+            LOGGER.info(f'{st}Success ✅ ({self.frames[i]} frames of shape {w}x{h} at {self.fps[i]:.2f} FPS)')
             self.threads[i].start()
         LOGGER.info('')  # newline
 
-        # check for common shapes
-        s = np.stack([LetterBox(imgsz, auto, stride=stride)(image=x).shape for x in self.imgs])
-        self.rect = np.unique(s, axis=0).shape[0] == 1  # rect inference if all shapes equal
-        self.auto = auto and self.rect
-        self.transforms = transforms  # optional
-        if not self.rect:
-            LOGGER.warning('WARNING ⚠️ Stream shapes differ. For optimal performance supply similarly-shaped streams.')
+        # Check for common shapes
+        self.bs = self.__len__()
 
     def update(self, i, cap, stream):
-        # Read stream `i` frames in daemon thread
+        """Read stream `i` frames in daemon thread."""
         n, f = 0, self.frames[i]  # frame number, frame array
         while cap.isOpened() and n < f:
             n += 1
             cap.grab()  # .read() = .grab() followed by .retrieve()
             if n % self.vid_stride == 0:
                 success, im = cap.retrieve()
                 if success:
@@ -78,90 +85,80 @@
                 else:
                     LOGGER.warning('WARNING ⚠️ Video stream unresponsive, please check your IP camera connection.')
                     self.imgs[i] = np.zeros_like(self.imgs[i])
                     cap.open(stream)  # re-open stream if signal was lost
             time.sleep(0.0)  # wait time
 
     def __iter__(self):
+        """Iterates through YOLO image feed and re-opens unresponsive streams."""
         self.count = -1
         return self
 
     def __next__(self):
+        """Returns source paths, transformed and original images for processing YOLOv5."""
         self.count += 1
         if not all(x.is_alive() for x in self.threads) or cv2.waitKey(1) == ord('q'):  # q to quit
             cv2.destroyAllWindows()
             raise StopIteration
 
         im0 = self.imgs.copy()
-        if self.transforms:
-            im = np.stack([self.transforms(x) for x in im0])  # transforms
-        else:
-            im = np.stack([LetterBox(self.imgsz, self.auto, stride=self.stride)(image=x) for x in im0])
-            im = im[..., ::-1].transpose((0, 3, 1, 2))  # BGR to RGB, BHWC to BCHW
-            im = np.ascontiguousarray(im)  # contiguous
-
-        return self.sources, im, im0, None, ''
+        return self.sources, im0, None, ''
 
     def __len__(self):
+        """Return the length of the sources object."""
         return len(self.sources)  # 1E12 frames = 32 streams at 30 FPS for 30 years
 
 
 class LoadScreenshots:
-    # YOLOv8 screenshot dataloader, i.e. `python detect.py --source "screen 0 100 100 512 256"`
-    def __init__(self, source, imgsz=640, stride=32, auto=True, transforms=None):
-        # source = [screen_number left top width height] (pixels)
+    # YOLOv8 screenshot dataloader, i.e. `yolo predict source=screen`
+    def __init__(self, source, imgsz=640):
+        """source = [screen_number left top width height] (pixels)."""
         check_requirements('mss')
         import mss  # noqa
 
         source, *params = source.split()
         self.screen, left, top, width, height = 0, None, None, None, None  # default to full screen 0
         if len(params) == 1:
             self.screen = int(params[0])
         elif len(params) == 4:
             left, top, width, height = (int(x) for x in params)
         elif len(params) == 5:
             self.screen, left, top, width, height = (int(x) for x in params)
         self.imgsz = imgsz
-        self.stride = stride
-        self.transforms = transforms
-        self.auto = auto
         self.mode = 'stream'
         self.frame = 0
         self.sct = mss.mss()
+        self.bs = 1
 
         # Parse monitor shape
         monitor = self.sct.monitors[self.screen]
-        self.top = monitor["top"] if top is None else (monitor["top"] + top)
-        self.left = monitor["left"] if left is None else (monitor["left"] + left)
-        self.width = width or monitor["width"]
-        self.height = height or monitor["height"]
-        self.monitor = {"left": self.left, "top": self.top, "width": self.width, "height": self.height}
+        self.top = monitor['top'] if top is None else (monitor['top'] + top)
+        self.left = monitor['left'] if left is None else (monitor['left'] + left)
+        self.width = width or monitor['width']
+        self.height = height or monitor['height']
+        self.monitor = {'left': self.left, 'top': self.top, 'width': self.width, 'height': self.height}
 
     def __iter__(self):
+        """Returns an iterator of the object."""
         return self
 
     def __next__(self):
-        # mss screen capture: get raw pixels from the screen as np array
+        """mss screen capture: get raw pixels from the screen as np array."""
         im0 = np.array(self.sct.grab(self.monitor))[:, :, :3]  # [:, :, :3] BGRA to BGR
-        s = f"screen {self.screen} (LTWH): {self.left},{self.top},{self.width},{self.height}: "
+        s = f'screen {self.screen} (LTWH): {self.left},{self.top},{self.width},{self.height}: '
 
-        if self.transforms:
-            im = self.transforms(im0)  # transforms
-        else:
-            im = LetterBox(self.imgsz, self.auto, stride=self.stride)(image=im0)
-            im = im.transpose((2, 0, 1))[::-1]  # HWC to CHW, BGR to RGB
-            im = np.ascontiguousarray(im)  # contiguous
         self.frame += 1
-        return str(self.screen), im, im0, None, s  # screen, img, original img, im0s, s
+        return str(self.screen), im0, None, s  # screen, img, original img, im0s, s
 
 
 class LoadImages:
-    # YOLOv8 image/video dataloader, i.e. `python detect.py --source image.jpg/vid.mp4`
-    def __init__(self, path, imgsz=640, stride=32, auto=True, transforms=None, vid_stride=1):
-        if isinstance(path, str) and Path(path).suffix == ".txt":  # *.txt file with img/vid/dir on each line
+    # YOLOv8 image/video dataloader, i.e. `yolo predict source=image.jpg/vid.mp4`
+    def __init__(self, path, imgsz=640, vid_stride=1):
+        """Initialize the Dataloader and raise FileNotFoundError if file not found."""
+        if isinstance(path, str) and Path(path).suffix == '.txt':  # *.txt file with img/vid/dir on each line
             path = Path(path).read_text().rsplit()
         files = []
         for p in sorted(path) if isinstance(path, (list, tuple)) else [path]:
             p = str(Path(p).resolve())
             if '*' in p:
                 files.extend(sorted(glob.glob(p, recursive=True)))  # glob
             elif os.path.isdir(p):
@@ -172,141 +169,176 @@
                 raise FileNotFoundError(f'{p} does not exist')
 
         images = [x for x in files if x.split('.')[-1].lower() in IMG_FORMATS]
         videos = [x for x in files if x.split('.')[-1].lower() in VID_FORMATS]
         ni, nv = len(images), len(videos)
 
         self.imgsz = imgsz
-        self.stride = stride
         self.files = images + videos
         self.nf = ni + nv  # number of files
         self.video_flag = [False] * ni + [True] * nv
         self.mode = 'image'
-        self.auto = auto
-        self.transforms = transforms  # optional
         self.vid_stride = vid_stride  # video frame-rate stride
+        self.bs = 1
         if any(videos):
+            self.orientation = None  # rotation degrees
             self._new_video(videos[0])  # new video
         else:
             self.cap = None
-        assert self.nf > 0, f'No images or videos found in {p}. ' \
-                            f'Supported formats are:\nimages: {IMG_FORMATS}\nvideos: {VID_FORMATS}'
+        if self.nf == 0:
+            raise FileNotFoundError(f'No images or videos found in {p}. '
+                                    f'Supported formats are:\nimages: {IMG_FORMATS}\nvideos: {VID_FORMATS}')
 
     def __iter__(self):
+        """Returns an iterator object for VideoStream or ImageFolder."""
         self.count = 0
         return self
 
     def __next__(self):
+        """Return next image, path and metadata from dataset."""
         if self.count == self.nf:
             raise StopIteration
         path = self.files[self.count]
 
         if self.video_flag[self.count]:
             # Read video
             self.mode = 'video'
             for _ in range(self.vid_stride):
                 self.cap.grab()
-            ret_val, im0 = self.cap.retrieve()
-            while not ret_val:
+            success, im0 = self.cap.retrieve()
+            while not success:
                 self.count += 1
                 self.cap.release()
                 if self.count == self.nf:  # last video
                     raise StopIteration
                 path = self.files[self.count]
                 self._new_video(path)
-                ret_val, im0 = self.cap.read()
+                success, im0 = self.cap.read()
 
             self.frame += 1
             # im0 = self._cv2_rotate(im0)  # for use if cv2 autorotation is False
             s = f'video {self.count + 1}/{self.nf} ({self.frame}/{self.frames}) {path}: '
 
         else:
             # Read image
             self.count += 1
             im0 = cv2.imread(path)  # BGR
-            assert im0 is not None, f'Image Not Found {path}'
+            if im0 is None:
+                raise FileNotFoundError(f'Image Not Found {path}')
             s = f'image {self.count}/{self.nf} {path}: '
 
-        if self.transforms:
-            im = self.transforms(im0)  # transforms
-        else:
-            im = LetterBox(self.imgsz, self.auto, stride=self.stride)(image=im0)
-            im = im.transpose((2, 0, 1))[::-1]  # HWC to CHW, BGR to RGB
-            im = np.ascontiguousarray(im)  # contiguous
-
-        return path, im, im0, self.cap, s
+        return [path], [im0], self.cap, s
 
     def _new_video(self, path):
-        # Create a new video capture object
+        """Create a new video capture object."""
         self.frame = 0
         self.cap = cv2.VideoCapture(path)
         self.frames = int(self.cap.get(cv2.CAP_PROP_FRAME_COUNT) / self.vid_stride)
-        self.orientation = int(self.cap.get(cv2.CAP_PROP_ORIENTATION_META))  # rotation degrees
-        # self.cap.set(cv2.CAP_PROP_ORIENTATION_AUTO, 0)  # disable https://github.com/ultralytics/yolov5/issues/8493
+        if hasattr(cv2, 'CAP_PROP_ORIENTATION_META'):  # cv2<4.6.0 compatibility
+            self.orientation = int(self.cap.get(cv2.CAP_PROP_ORIENTATION_META))  # rotation degrees
+            # Disable auto-orientation due to known issues in https://github.com/ultralytics/yolov5/issues/8493
+            # self.cap.set(cv2.CAP_PROP_ORIENTATION_AUTO, 0)
 
     def _cv2_rotate(self, im):
-        # Rotate a cv2 video manually
+        """Rotate a cv2 video manually."""
         if self.orientation == 0:
             return cv2.rotate(im, cv2.ROTATE_90_CLOCKWISE)
         elif self.orientation == 180:
             return cv2.rotate(im, cv2.ROTATE_90_COUNTERCLOCKWISE)
         elif self.orientation == 90:
             return cv2.rotate(im, cv2.ROTATE_180)
         return im
 
     def __len__(self):
+        """Returns the number of files in the object."""
         return self.nf  # number of files
 
 
 class LoadPilAndNumpy:
 
-    def __init__(self, im0, imgsz=640, stride=32, auto=True, transforms=None):
+    def __init__(self, im0, imgsz=640):
+        """Initialize PIL and Numpy Dataloader."""
         if not isinstance(im0, list):
             im0 = [im0]
+        self.paths = [getattr(im, 'filename', f'image{i}.jpg') for i, im in enumerate(im0)]
         self.im0 = [self._single_check(im) for im in im0]
         self.imgsz = imgsz
-        self.stride = stride
-        self.auto = auto
-        self.transforms = transforms
         self.mode = 'image'
-        # generate fake paths
-        self.paths = [f"image{i}.jpg" for i in range(len(self.im0))]
+        # Generate fake paths
+        self.bs = len(self.im0)
 
     @staticmethod
     def _single_check(im):
-        assert isinstance(im, (Image.Image, np.ndarray)), f"Expected PIL/np.ndarray image type, but got {type(im)}"
+        """Validate and format an image to numpy array."""
+        assert isinstance(im, (Image.Image, np.ndarray)), f'Expected PIL/np.ndarray image type, but got {type(im)}'
         if isinstance(im, Image.Image):
+            if im.mode != 'RGB':
+                im = im.convert('RGB')
             im = np.asarray(im)[:, :, ::-1]
             im = np.ascontiguousarray(im)  # contiguous
         return im
 
-    def _single_preprocess(self, im, auto):
-        if self.transforms:
-            im = self.transforms(im)  # transforms
-        else:
-            im = LetterBox(self.imgsz, auto=auto, stride=self.stride)(image=im)
-            im = im.transpose((2, 0, 1))[::-1]  # HWC to CHW, BGR to RGB
-            im = np.ascontiguousarray(im)  # contiguous
-        return im
-
     def __len__(self):
+        """Returns the length of the 'im0' attribute."""
         return len(self.im0)
 
     def __next__(self):
+        """Returns batch paths, images, processed images, None, ''."""
         if self.count == 1:  # loop only once as it's batch inference
             raise StopIteration
-        auto = all(x.shape == self.im0[0].shape for x in self.im0) and self.auto
-        im = [self._single_preprocess(im, auto) for im in self.im0]
-        im = np.stack(im, 0) if len(im) > 1 else im[0][None]
         self.count += 1
-        return self.paths, im, self.im0, None, ''
+        return self.paths, self.im0, None, ''
 
     def __iter__(self):
+        """Enables iteration for class LoadPilAndNumpy."""
         self.count = 0
         return self
 
 
-if __name__ == "__main__":
-    img = cv2.imread(str(ROOT / "assets/bus.jpg"))
+class LoadTensor:
+
+    def __init__(self, imgs) -> None:
+        self.im0 = imgs
+        self.bs = imgs.shape[0]
+        self.mode = 'image'
+
+    def __iter__(self):
+        """Returns an iterator object."""
+        self.count = 0
+        return self
+
+    def __next__(self):
+        """Return next item in the iterator."""
+        if self.count == 1:
+            raise StopIteration
+        self.count += 1
+        return None, self.im0, None, ''  # self.paths, im, self.im0, None, ''
+
+    def __len__(self):
+        """Returns the batch size."""
+        return self.bs
+
+
+def autocast_list(source):
+    """
+    Merges a list of source of different types into a list of numpy arrays or PIL images
+    """
+    files = []
+    for im in source:
+        if isinstance(im, (str, Path)):  # filename or uri
+            files.append(Image.open(requests.get(im, stream=True).raw if str(im).startswith('http') else im))
+        elif isinstance(im, (Image.Image, np.ndarray)):  # PIL or np Image
+            files.append(im)
+        else:
+            raise TypeError(f'type {type(im).__name__} is not a supported Ultralytics prediction source type. \n'
+                            f'See https://docs.ultralytics.com/modes/predict for supported source types.')
+
+    return files
+
+
+LOADERS = [LoadStreams, LoadPilAndNumpy, LoadImages, LoadScreenshots]
+
+if __name__ == '__main__':
+    img = cv2.imread(str(ROOT / 'assets/bus.jpg'))
     dataset = LoadPilAndNumpy(im0=img)
     for d in dataset:
         print(d[0])
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/data/dataloaders/v5augmentations.py` & `ultralytics-8.0.90/ultralytics/yolo/data/dataloaders/v5augmentations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 """
 Image augmentation functions
 """
 
 import math
 import random
 
@@ -20,14 +20,15 @@
 IMAGENET_MEAN = 0.485, 0.456, 0.406  # RGB mean
 IMAGENET_STD = 0.229, 0.224, 0.225  # RGB standard deviation
 
 
 class Albumentations:
     # YOLOv5 Albumentations class (optional, only used if package is installed)
     def __init__(self, size=640):
+        """Instantiate object with image augmentations for YOLOv5."""
         self.transform = None
         prefix = colorstr('albumentations: ')
         try:
             import albumentations as A
             check_version(A.__version__, '1.0.3', hard=True)  # version requirement
 
             T = [
@@ -44,34 +45,35 @@
             LOGGER.info(prefix + ', '.join(f'{x}'.replace('always_apply=False, ', '') for x in T if x.p))
         except ImportError:  # package not installed, skip
             pass
         except Exception as e:
             LOGGER.info(f'{prefix}{e}')
 
     def __call__(self, im, labels, p=1.0):
+        """Transforms input image and labels with probability 'p'."""
         if self.transform and random.random() < p:
             new = self.transform(image=im, bboxes=labels[:, 1:], class_labels=labels[:, 0])  # transformed
             im, labels = new['image'], np.array([[c, *b] for c, b in zip(new['class_labels'], new['bboxes'])])
         return im, labels
 
 
 def normalize(x, mean=IMAGENET_MEAN, std=IMAGENET_STD, inplace=False):
-    # Denormalize RGB images x per ImageNet stats in BCHW format, i.e. = (x - mean) / std
+    """Denormalize RGB images x per ImageNet stats in BCHW format, i.e. = (x - mean) / std."""
     return TF.normalize(x, mean, std, inplace=inplace)
 
 
 def denormalize(x, mean=IMAGENET_MEAN, std=IMAGENET_STD):
-    # Denormalize RGB images x per ImageNet stats in BCHW format, i.e. = x * std + mean
+    """Denormalize RGB images x per ImageNet stats in BCHW format, i.e. = x * std + mean."""
     for i in range(3):
         x[:, i] = x[:, i] * std[i] + mean[i]
     return x
 
 
 def augment_hsv(im, hgain=0.5, sgain=0.5, vgain=0.5):
-    # HSV color-space augmentation
+    """HSV color-space augmentation."""
     if hgain or sgain or vgain:
         r = np.random.uniform(-1, 1, 3) * [hgain, sgain, vgain] + 1  # random gains
         hue, sat, val = cv2.split(cv2.cvtColor(im, cv2.COLOR_BGR2HSV))
         dtype = im.dtype  # uint8
 
         x = np.arange(0, 256, dtype=r.dtype)
         lut_hue = ((x * r[0]) % 180).astype(dtype)
@@ -79,26 +81,26 @@
         lut_val = np.clip(x * r[2], 0, 255).astype(dtype)
 
         im_hsv = cv2.merge((cv2.LUT(hue, lut_hue), cv2.LUT(sat, lut_sat), cv2.LUT(val, lut_val)))
         cv2.cvtColor(im_hsv, cv2.COLOR_HSV2BGR, dst=im)  # no return needed
 
 
 def hist_equalize(im, clahe=True, bgr=False):
-    # Equalize histogram on BGR image 'im' with im.shape(n,m,3) and range 0-255
+    """Equalize histogram on BGR image 'im' with im.shape(n,m,3) and range 0-255."""
     yuv = cv2.cvtColor(im, cv2.COLOR_BGR2YUV if bgr else cv2.COLOR_RGB2YUV)
     if clahe:
         c = cv2.createCLAHE(clipLimit=2.0, tileGridSize=(8, 8))
         yuv[:, :, 0] = c.apply(yuv[:, :, 0])
     else:
         yuv[:, :, 0] = cv2.equalizeHist(yuv[:, :, 0])  # equalize Y channel histogram
     return cv2.cvtColor(yuv, cv2.COLOR_YUV2BGR if bgr else cv2.COLOR_YUV2RGB)  # convert YUV image to RGB
 
 
 def replicate(im, labels):
-    # Replicate labels
+    """Replicate labels."""
     h, w = im.shape[:2]
     boxes = labels[:, 1:].astype(int)
     x1, y1, x2, y2 = boxes.T
     s = ((x2 - x1) + (y2 - y1)) / 2  # side length (pixels)
     for i in s.argsort()[:round(s.size * 0.5)]:  # smallest indices
         x1b, y1b, x2b, y2b = boxes[i]
         bh, bw = y2b - y1b, x2b - x1b
@@ -107,15 +109,15 @@
         im[y1a:y2a, x1a:x2a] = im[y1b:y2b, x1b:x2b]  # im4[ymin:ymax, xmin:xmax]
         labels = np.append(labels, [[labels[i, 0], x1a, y1a, x2a, y2a]], axis=0)
 
     return im, labels
 
 
 def letterbox(im, new_shape=(640, 640), color=(114, 114, 114), auto=True, scaleFill=False, scaleup=True, stride=32):
-    # Resize and pad image while meeting stride-multiple constraints
+    """Resize and pad image while meeting stride-multiple constraints."""
     shape = im.shape[:2]  # current shape [height, width]
     if isinstance(new_shape, int):
         new_shape = (new_shape, new_shape)
 
     # Scale ratio (new / old)
     r = min(new_shape[0] / shape[0], new_shape[1] / shape[1])
     if not scaleup:  # only scale down, do not scale up (for better val mAP)
@@ -209,48 +211,48 @@
             segments = resample_segments(segments)  # upsample
             for i, segment in enumerate(segments):
                 xy = np.ones((len(segment), 3))
                 xy[:, :2] = segment
                 xy = xy @ M.T  # transform
                 xy = xy[:, :2] / xy[:, 2:3] if perspective else xy[:, :2]  # perspective rescale or affine
 
-                # clip
+                # Clip
                 new[i] = segment2box(xy, width, height)
 
         else:  # warp boxes
             xy = np.ones((n * 4, 3))
             xy[:, :2] = targets[:, [1, 2, 3, 4, 1, 4, 3, 2]].reshape(n * 4, 2)  # x1y1, x2y2, x1y2, x2y1
             xy = xy @ M.T  # transform
             xy = (xy[:, :2] / xy[:, 2:3] if perspective else xy[:, :2]).reshape(n, 8)  # perspective rescale or affine
 
-            # create new boxes
+            # Create new boxes
             x = xy[:, [0, 2, 4, 6]]
             y = xy[:, [1, 3, 5, 7]]
             new = np.concatenate((x.min(1), y.min(1), x.max(1), y.max(1))).reshape(4, n).T
 
-            # clip
+            # Clip
             new[:, [0, 2]] = new[:, [0, 2]].clip(0, width)
             new[:, [1, 3]] = new[:, [1, 3]].clip(0, height)
 
-        # filter candidates
+        # Filter candidates
         i = box_candidates(box1=targets[:, 1:5].T * s, box2=new.T, area_thr=0.01 if use_segments else 0.10)
         targets = targets[i]
         targets[:, 1:5] = new[i]
 
     return im, targets
 
 
 def copy_paste(im, labels, segments, p=0.5):
-    # Implement Copy-Paste augmentation https://arxiv.org/abs/2012.07177, labels as nx5 np.array(cls, xyxy)
+    """Implement Copy-Paste augmentation https://arxiv.org/abs/2012.07177, labels as nx5 np.array(cls, xyxy)."""
     n = len(segments)
     if p and n:
         h, w, c = im.shape  # height, width, channels
         im_new = np.zeros(im.shape, np.uint8)
 
-        # calculate ioa first then select indexes randomly
+        # Calculate ioa first then select indexes randomly
         boxes = np.stack([w - labels[:, 3], labels[:, 2], w - labels[:, 1], labels[:, 4]], axis=-1)  # (n, 4)
         ioa = bbox_ioa(boxes, labels[:, 1:5])  # intersection over area
         indexes = np.nonzero((ioa < 0.30).all(1))[0]  # (N, )
         n = len(indexes)
         for j in random.sample(list(indexes), k=round(p * n)):
             l, box, s = labels[j], boxes[j], segments[j]
             labels = np.concatenate((labels, [[l[0], *box]]), 0)
@@ -261,42 +263,42 @@
         i = cv2.flip(im_new, 1).astype(bool)
         im[i] = result[i]  # cv2.imwrite('debug.jpg', im)  # debug
 
     return im, labels, segments
 
 
 def cutout(im, labels, p=0.5):
-    # Applies image cutout augmentation https://arxiv.org/abs/1708.04552
+    """Applies image cutout augmentation https://arxiv.org/abs/1708.04552."""
     if random.random() < p:
         h, w = im.shape[:2]
         scales = [0.5] * 1 + [0.25] * 2 + [0.125] * 4 + [0.0625] * 8 + [0.03125] * 16  # image size fraction
         for s in scales:
             mask_h = random.randint(1, int(h * s))  # create random masks
             mask_w = random.randint(1, int(w * s))
 
-            # box
+            # Box
             xmin = max(0, random.randint(0, w) - mask_w // 2)
             ymin = max(0, random.randint(0, h) - mask_h // 2)
             xmax = min(w, xmin + mask_w)
             ymax = min(h, ymin + mask_h)
 
-            # apply random color mask
+            # Apply random color mask
             im[ymin:ymax, xmin:xmax] = [random.randint(64, 191) for _ in range(3)]
 
-            # return unobscured labels
+            # Return unobscured labels
             if len(labels) and s > 0.03:
                 box = np.array([[xmin, ymin, xmax, ymax]], dtype=np.float32)
                 ioa = bbox_ioa(box, xywhn2xyxy(labels[:, 1:5], w, h))[0]  # intersection over area
                 labels = labels[ioa < 0.60]  # remove >60% obscured labels
 
     return labels
 
 
 def mixup(im, labels, im2, labels2):
-    # Applies MixUp augmentation https://arxiv.org/pdf/1710.09412.pdf
+    """Applies MixUp augmentation https://arxiv.org/pdf/1710.09412.pdf."""
     r = np.random.beta(32.0, 32.0)  # mixup ratio, alpha=beta=32.0
     im = (im * r + im2 * (1 - r)).astype(np.uint8)
     labels = np.concatenate((labels, labels2), 0)
     return im, labels
 
 
 def box_candidates(box1, box2, wh_thr=2, ar_thr=100, area_thr=0.1, eps=1e-16):  # box1(4,n), box2(4,n)
@@ -331,38 +333,39 @@
                 LOGGER.info(f'{prefix}auto augmentations are currently not supported')
             else:
                 if hflip > 0:
                     T += [A.HorizontalFlip(p=hflip)]
                 if vflip > 0:
                     T += [A.VerticalFlip(p=vflip)]
                 if jitter > 0:
-                    color_jitter = (float(jitter),) * 3  # repeat value for brightness, contrast, satuaration, 0 hue
-                    T += [A.ColorJitter(*color_jitter, 0)]
+                    jitter = float(jitter)
+                    T += [A.ColorJitter(jitter, jitter, jitter, 0)]  # brightness, contrast, satuaration, 0 hue
         else:  # Use fixed crop for eval set (reproducibility)
             T = [A.SmallestMaxSize(max_size=size), A.CenterCrop(height=size, width=size)]
         T += [A.Normalize(mean=mean, std=std), ToTensorV2()]  # Normalize and convert to Tensor
         LOGGER.info(prefix + ', '.join(f'{x}'.replace('always_apply=False, ', '') for x in T if x.p))
         return A.Compose(T)
 
     except ImportError:  # package not installed, skip
         LOGGER.warning(f'{prefix}⚠️ not found, install with `pip install albumentations` (recommended)')
     except Exception as e:
         LOGGER.info(f'{prefix}{e}')
 
 
 def classify_transforms(size=224):
-    # Transforms to apply if albumentations not installed
+    """Transforms to apply if albumentations not installed."""
     assert isinstance(size, int), f'ERROR: classify_transforms size {size} must be integer, not (list, tuple)'
     # T.Compose([T.ToTensor(), T.Resize(size), T.CenterCrop(size), T.Normalize(IMAGENET_MEAN, IMAGENET_STD)])
     return T.Compose([CenterCrop(size), ToTensor(), T.Normalize(IMAGENET_MEAN, IMAGENET_STD)])
 
 
 class LetterBox:
     # YOLOv5 LetterBox class for image preprocessing, i.e. T.Compose([LetterBox(size), ToTensor()])
     def __init__(self, size=(640, 640), auto=False, stride=32):
+        """Resizes and crops an image to a specified size for YOLOv5 preprocessing."""
         super().__init__()
         self.h, self.w = (size, size) if isinstance(size, int) else size
         self.auto = auto  # pass max size integer, automatically solve for short side using stride
         self.stride = stride  # used with auto
 
     def __call__(self, im):  # im = np.array HWC
         imh, imw = im.shape[:2]
@@ -374,27 +377,29 @@
         im_out[top:top + h, left:left + w] = cv2.resize(im, (w, h), interpolation=cv2.INTER_LINEAR)
         return im_out
 
 
 class CenterCrop:
     # YOLOv5 CenterCrop class for image preprocessing, i.e. T.Compose([CenterCrop(size), ToTensor()])
     def __init__(self, size=640):
+        """Converts input image into tensor for YOLOv5 processing."""
         super().__init__()
         self.h, self.w = (size, size) if isinstance(size, int) else size
 
     def __call__(self, im):  # im = np.array HWC
         imh, imw = im.shape[:2]
         m = min(imh, imw)  # min dimension
         top, left = (imh - m) // 2, (imw - m) // 2
         return cv2.resize(im[top:top + m, left:left + m], (self.w, self.h), interpolation=cv2.INTER_LINEAR)
 
 
 class ToTensor:
     # YOLOv5 ToTensor class for image preprocessing, i.e. T.Compose([LetterBox(size), ToTensor()])
     def __init__(self, half=False):
+        """Initialize ToTensor class for YOLOv5 image preprocessing."""
         super().__init__()
         self.half = half
 
     def __call__(self, im):  # im = np.array HWC in BGR order
         im = np.ascontiguousarray(im.transpose((2, 0, 1))[::-1])  # HWC to CHW -> BGR to RGB -> contiguous
         im = torch.from_numpy(im)  # to torch
         im = im.half() if self.half else im.float()  # uint8 to fp16/32
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/data/dataloaders/v5loader.py` & `ultralytics-8.0.90/ultralytics/yolo/data/dataloaders/v5loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,68 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 """
 Dataloaders and dataset utils
 """
 
 import contextlib
 import glob
 import hashlib
-import json
 import math
 import os
 import random
 import shutil
 import time
 from itertools import repeat
-from multiprocessing.pool import Pool, ThreadPool
+from multiprocessing.pool import ThreadPool
 from pathlib import Path
 from threading import Thread
 from urllib.parse import urlparse
 
 import cv2
 import numpy as np
 import psutil
 import torch
 import torchvision
-import yaml
 from PIL import ExifTags, Image, ImageOps
 from torch.utils.data import DataLoader, Dataset, dataloader, distributed
 from tqdm import tqdm
 
-from ultralytics.yolo.data.utils import check_dataset, unzip_file
-from ultralytics.yolo.utils import DATASETS_DIR, LOGGER, NUM_THREADS, TQDM_BAR_FORMAT, is_colab, is_kaggle
-from ultralytics.yolo.utils.checks import check_requirements, check_yaml
+from ultralytics.yolo.utils import (DATASETS_DIR, LOGGER, NUM_THREADS, TQDM_BAR_FORMAT, is_colab, is_dir_writeable,
+                                    is_kaggle)
+from ultralytics.yolo.utils.checks import check_requirements
 from ultralytics.yolo.utils.ops import clean_str, segments2boxes, xyn2xy, xywh2xyxy, xywhn2xyxy, xyxy2xywhn
 from ultralytics.yolo.utils.torch_utils import torch_distributed_zero_first
 
 from .v5augmentations import (Albumentations, augment_hsv, classify_albumentations, classify_transforms, copy_paste,
                               letterbox, mixup, random_perspective)
 
 # Parameters
-HELP_URL = 'See https://github.com/ultralytics/yolov5/wiki/Train-Custom-Data'
+HELP_URL = 'See https://docs.ultralytics.com/yolov5/tutorials/train_custom_data'
 IMG_FORMATS = 'bmp', 'dng', 'jpeg', 'jpg', 'mpo', 'png', 'tif', 'tiff', 'webp', 'pfm'  # include image suffixes
 VID_FORMATS = 'asf', 'avi', 'gif', 'm4v', 'mkv', 'mov', 'mp4', 'mpeg', 'mpg', 'ts', 'wmv'  # include video suffixes
 LOCAL_RANK = int(os.getenv('LOCAL_RANK', -1))  # https://pytorch.org/docs/stable/elastic/run.html
 RANK = int(os.getenv('RANK', -1))
 PIN_MEMORY = str(os.getenv('PIN_MEMORY', True)).lower() == 'true'  # global pin_memory for dataloaders
 
 # Get orientation exif tag
 for orientation in ExifTags.TAGS.keys():
     if ExifTags.TAGS[orientation] == 'Orientation':
         break
 
 
 def get_hash(paths):
-    # Returns a single hash value of a list of paths (files or dirs)
+    """Returns a single hash value of a list of paths (files or dirs)."""
     size = sum(os.path.getsize(p) for p in paths if os.path.exists(p))  # sizes
-    h = hashlib.md5(str(size).encode())  # hash sizes
+    h = hashlib.sha256(str(size).encode())  # hash sizes
     h.update(''.join(paths).encode())  # hash paths
     return h.hexdigest()  # return hash
 
 
 def exif_size(img):
-    # Returns exif-corrected PIL size
+    """Returns exif-corrected PIL size."""
     s = img.size  # (width, height)
     with contextlib.suppress(Exception):
         rotation = dict(img._getexif().items())[orientation]
         if rotation in [6, 8]:  # rotation 270 or 90
             s = (s[1], s[0])
     return s
 
@@ -87,20 +85,20 @@
             5: Image.TRANSPOSE,
             6: Image.ROTATE_270,
             7: Image.TRANSVERSE,
             8: Image.ROTATE_90}.get(orientation)
         if method is not None:
             image = image.transpose(method)
             del exif[0x0112]
-            image.info["exif"] = exif.tobytes()
+            image.info['exif'] = exif.tobytes()
     return image
 
 
 def seed_worker(worker_id):
-    # Set dataloader worker seed https://pytorch.org/docs/stable/notes/randomness.html#dataloader
+    """Set dataloader worker seed https://pytorch.org/docs/stable/notes/randomness.html#dataloader."""
     worker_seed = torch.initial_seed() % 2 ** 32
     np.random.seed(worker_seed)
     random.seed(worker_seed)
 
 
 def create_dataloader(path,
                       imgsz,
@@ -154,51 +152,56 @@
                   pin_memory=PIN_MEMORY,
                   collate_fn=LoadImagesAndLabels.collate_fn,
                   worker_init_fn=seed_worker,
                   generator=generator), dataset
 
 
 class InfiniteDataLoader(dataloader.DataLoader):
-    """ Dataloader that reuses workers
+    """Dataloader that reuses workers
 
     Uses same syntax as vanilla DataLoader
     """
 
     def __init__(self, *args, **kwargs):
+        """Dataloader that reuses workers for same syntax as vanilla DataLoader."""
         super().__init__(*args, **kwargs)
         object.__setattr__(self, 'batch_sampler', _RepeatSampler(self.batch_sampler))
         self.iterator = super().__iter__()
 
     def __len__(self):
+        """Returns the length of batch_sampler's sampler."""
         return len(self.batch_sampler.sampler)
 
     def __iter__(self):
+        """Creates a sampler that infinitely repeats."""
         for _ in range(len(self)):
             yield next(self.iterator)
 
 
 class _RepeatSampler:
-    """ Sampler that repeats forever
+    """Sampler that repeats forever
 
     Args:
-        sampler (Sampler)
+        sampler (Dataset.sampler): The sampler to repeat.
     """
 
     def __init__(self, sampler):
+        """Sampler that repeats dataset samples infinitely."""
         self.sampler = sampler
 
     def __iter__(self):
+        """Infinite loop iterating over a given sampler."""
         while True:
             yield from iter(self.sampler)
 
 
 class LoadScreenshots:
     # YOLOv5 screenshot dataloader, i.e. `python detect.py --source "screen 0 100 100 512 256"`
     def __init__(self, source, img_size=640, stride=32, auto=True, transforms=None):
-        # source = [screen_number left top width height] (pixels)
+        """source = [screen_number left top width height] (pixels)."""
         check_requirements('mss')
         import mss
 
         source, *params = source.split()
         self.screen, left, top, width, height = 0, None, None, None, None  # default to full screen 0
         if len(params) == 1:
             self.screen = int(params[0])
@@ -212,42 +215,44 @@
         self.auto = auto
         self.mode = 'stream'
         self.frame = 0
         self.sct = mss.mss()
 
         # Parse monitor shape
         monitor = self.sct.monitors[self.screen]
-        self.top = monitor["top"] if top is None else (monitor["top"] + top)
-        self.left = monitor["left"] if left is None else (monitor["left"] + left)
-        self.width = width or monitor["width"]
-        self.height = height or monitor["height"]
-        self.monitor = {"left": self.left, "top": self.top, "width": self.width, "height": self.height}
+        self.top = monitor['top'] if top is None else (monitor['top'] + top)
+        self.left = monitor['left'] if left is None else (monitor['left'] + left)
+        self.width = width or monitor['width']
+        self.height = height or monitor['height']
+        self.monitor = {'left': self.left, 'top': self.top, 'width': self.width, 'height': self.height}
 
     def __iter__(self):
+        """Iterates over objects with the same structure as the monitor attribute."""
         return self
 
     def __next__(self):
-        # mss screen capture: get raw pixels from the screen as np array
+        """mss screen capture: get raw pixels from the screen as np array."""
         im0 = np.array(self.sct.grab(self.monitor))[:, :, :3]  # [:, :, :3] BGRA to BGR
-        s = f"screen {self.screen} (LTWH): {self.left},{self.top},{self.width},{self.height}: "
+        s = f'screen {self.screen} (LTWH): {self.left},{self.top},{self.width},{self.height}: '
 
         if self.transforms:
             im = self.transforms(im0)  # transforms
         else:
             im = letterbox(im0, self.img_size, stride=self.stride, auto=self.auto)[0]  # padded resize
             im = im.transpose((2, 0, 1))[::-1]  # HWC to CHW, BGR to RGB
             im = np.ascontiguousarray(im)  # contiguous
         self.frame += 1
         return str(self.screen), im, im0, None, s  # screen, img, original img, im0s, s
 
 
 class LoadImages:
     # YOLOv5 image/video dataloader, i.e. `python detect.py --source image.jpg/vid.mp4`
     def __init__(self, path, img_size=640, stride=32, auto=True, transforms=None, vid_stride=1):
-        if isinstance(path, str) and Path(path).suffix == ".txt":  # *.txt file with img/vid/dir on each line
+        """Initialize instance variables and check for valid input."""
+        if isinstance(path, str) and Path(path).suffix == '.txt':  # *.txt file with img/vid/dir on each line
             path = Path(path).read_text().rsplit()
         files = []
         for p in sorted(path) if isinstance(path, (list, tuple)) else [path]:
             p = str(Path(p).resolve())
             if '*' in p:
                 files.extend(sorted(glob.glob(p, recursive=True)))  # glob
             elif os.path.isdir(p):
@@ -274,18 +279,20 @@
             self._new_video(videos[0])  # new video
         else:
             self.cap = None
         assert self.nf > 0, f'No images or videos found in {p}. ' \
                             f'Supported formats are:\nimages: {IMG_FORMATS}\nvideos: {VID_FORMATS}'
 
     def __iter__(self):
+        """Returns an iterator object for iterating over images or videos found in a directory."""
         self.count = 0
         return self
 
     def __next__(self):
+        """Iterator's next item, performs transformation on image and returns path, transformed image, original image, capture and size."""
         if self.count == self.nf:
             raise StopIteration
         path = self.files[self.count]
 
         if self.video_flag[self.count]:
             # Read video
             self.mode = 'video'
@@ -318,38 +325,40 @@
             im = letterbox(im0, self.img_size, stride=self.stride, auto=self.auto)[0]  # padded resize
             im = im.transpose((2, 0, 1))[::-1]  # HWC to CHW, BGR to RGB
             im = np.ascontiguousarray(im)  # contiguous
 
         return path, im, im0, self.cap, s
 
     def _new_video(self, path):
-        # Create a new video capture object
+        """Create a new video capture object."""
         self.frame = 0
         self.cap = cv2.VideoCapture(path)
         self.frames = int(self.cap.get(cv2.CAP_PROP_FRAME_COUNT) / self.vid_stride)
         self.orientation = int(self.cap.get(cv2.CAP_PROP_ORIENTATION_META))  # rotation degrees
         # self.cap.set(cv2.CAP_PROP_ORIENTATION_AUTO, 0)  # disable https://github.com/ultralytics/yolov5/issues/8493
 
     def _cv2_rotate(self, im):
-        # Rotate a cv2 video manually
+        """Rotate a cv2 video manually."""
         if self.orientation == 0:
             return cv2.rotate(im, cv2.ROTATE_90_CLOCKWISE)
         elif self.orientation == 180:
             return cv2.rotate(im, cv2.ROTATE_90_COUNTERCLOCKWISE)
         elif self.orientation == 90:
             return cv2.rotate(im, cv2.ROTATE_180)
         return im
 
     def __len__(self):
+        """Returns the number of files in the class instance."""
         return self.nf  # number of files
 
 
 class LoadStreams:
     # YOLOv5 streamloader, i.e. `python detect.py --source 'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP streams`
     def __init__(self, sources='file.streams', img_size=640, stride=32, auto=True, transforms=None, vid_stride=1):
+        """Initialize YOLO detector with optional transforms and check input shapes."""
         torch.backends.cudnn.benchmark = True  # faster for fixed-size inference
         self.mode = 'stream'
         self.img_size = img_size
         self.stride = stride
         self.vid_stride = vid_stride  # video frame-rate stride
         sources = Path(sources).read_text().rsplit() if os.path.isfile(sources) else [sources]
         n = len(sources)
@@ -358,43 +367,43 @@
         for i, s in enumerate(sources):  # index, source
             # Start thread to read frames from video stream
             st = f'{i + 1}/{n}: {s}... '
             if urlparse(s).hostname in ('www.youtube.com', 'youtube.com', 'youtu.be'):  # if source is YouTube video
                 # YouTube format i.e. 'https://www.youtube.com/watch?v=Zgi9g1ksQHc' or 'https://youtu.be/Zgi9g1ksQHc'
                 check_requirements(('pafy', 'youtube_dl==2020.12.2'))
                 import pafy
-                s = pafy.new(s).getbest(preftype="mp4").url  # YouTube URL
+                s = pafy.new(s).getbest(preftype='mp4').url  # YouTube URL
             s = eval(s) if s.isnumeric() else s  # i.e. s = '0' local webcam
             if s == 0:
                 assert not is_colab(), '--source 0 webcam unsupported on Colab. Rerun command in a local environment.'
                 assert not is_kaggle(), '--source 0 webcam unsupported on Kaggle. Rerun command in a local environment.'
             cap = cv2.VideoCapture(s)
             assert cap.isOpened(), f'{st}Failed to open {s}'
             w = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
             h = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
             fps = cap.get(cv2.CAP_PROP_FPS)  # warning: may return 0 or nan
             self.frames[i] = max(int(cap.get(cv2.CAP_PROP_FRAME_COUNT)), 0) or float('inf')  # infinite stream fallback
             self.fps[i] = max((fps if math.isfinite(fps) else 0) % 100, 0) or 30  # 30 FPS fallback
 
             _, self.imgs[i] = cap.read()  # guarantee first frame
             self.threads[i] = Thread(target=self.update, args=([i, cap, s]), daemon=True)
-            LOGGER.info(f"{st} Success ({self.frames[i]} frames {w}x{h} at {self.fps[i]:.2f} FPS)")
+            LOGGER.info(f'{st} Success ({self.frames[i]} frames {w}x{h} at {self.fps[i]:.2f} FPS)')
             self.threads[i].start()
         LOGGER.info('')  # newline
 
-        # check for common shapes
+        # Check for common shapes
         s = np.stack([letterbox(x, img_size, stride=stride, auto=auto)[0].shape for x in self.imgs])
         self.rect = np.unique(s, axis=0).shape[0] == 1  # rect inference if all shapes equal
         self.auto = auto and self.rect
         self.transforms = transforms  # optional
         if not self.rect:
             LOGGER.warning('WARNING ⚠️ Stream shapes differ. For optimal performance supply similarly-shaped streams.')
 
     def update(self, i, cap, stream):
-        # Read stream `i` frames in daemon thread
+        """Read stream `i` frames in daemon thread."""
         n, f = 0, self.frames[i]  # frame number, frame array
         while cap.isOpened() and n < f:
             n += 1
             cap.grab()  # .read() = .grab() followed by .retrieve()
             if n % self.vid_stride == 0:
                 success, im = cap.retrieve()
                 if success:
@@ -402,18 +411,20 @@
                 else:
                     LOGGER.warning('WARNING ⚠️ Video stream unresponsive, please check your IP camera connection.')
                     self.imgs[i] = np.zeros_like(self.imgs[i])
                     cap.open(stream)  # re-open stream if signal was lost
             time.sleep(0.0)  # wait time
 
     def __iter__(self):
+        """Iterator that returns the class instance."""
         self.count = -1
         return self
 
     def __next__(self):
+        """Return a tuple containing transformed and resized image data."""
         self.count += 1
         if not all(x.is_alive() for x in self.threads) or cv2.waitKey(1) == ord('q'):  # q to quit
             cv2.destroyAllWindows()
             raise StopIteration
 
         im0 = self.imgs.copy()
         if self.transforms:
@@ -422,25 +433,26 @@
             im = np.stack([letterbox(x, self.img_size, stride=self.stride, auto=self.auto)[0] for x in im0])  # resize
             im = im[..., ::-1].transpose((0, 3, 1, 2))  # BGR to RGB, BHWC to BCHW
             im = np.ascontiguousarray(im)  # contiguous
 
         return self.sources, im, im0, None, ''
 
     def __len__(self):
+        """Returns the number of sources as the length of the object."""
         return len(self.sources)  # 1E12 frames = 32 streams at 30 FPS for 30 years
 
 
 def img2label_paths(img_paths):
-    # Define label paths as a function of image paths
+    """Define label paths as a function of image paths."""
     sa, sb = f'{os.sep}images{os.sep}', f'{os.sep}labels{os.sep}'  # /images/, /labels/ substrings
     return [sb.join(x.rsplit(sa, 1)).rsplit('.', 1)[0] + '.txt' for x in img_paths]
 
 
 class LoadImagesAndLabels(Dataset):
-    # YOLOv5 train_loader/val_loader, loads images and labels for training and validation
+    """YOLOv5 train_loader/val_loader, loads images and labels for training and validation."""
     cache_version = 0.6  # dataset labels *.cache version
     rand_interp_methods = [cv2.INTER_NEAREST, cv2.INTER_LINEAR, cv2.INTER_CUBIC, cv2.INTER_AREA, cv2.INTER_LANCZOS4]
 
     def __init__(self,
                  path,
                  img_size=640,
                  batch_size=16,
@@ -489,21 +501,21 @@
         # Check cache
         self.label_files = img2label_paths(self.im_files)  # labels
         cache_path = (p if p.is_file() else Path(self.label_files[0]).parent).with_suffix('.cache')
         try:
             cache, exists = np.load(cache_path, allow_pickle=True).item(), True  # load dict
             assert cache['version'] == self.cache_version  # matches current version
             assert cache['hash'] == get_hash(self.label_files + self.im_files)  # identical hash
-        except Exception:
+        except (FileNotFoundError, AssertionError, AttributeError):
             cache, exists = self.cache_labels(cache_path, prefix), False  # run cache ops
 
         # Display cache
         nf, nm, ne, nc, n = cache.pop('results')  # found, missing, empty, corrupt, total
-        if exists and LOCAL_RANK in {-1, 0}:
-            d = f"Scanning {cache_path}... {nf} images, {nm + ne} backgrounds, {nc} corrupt"
+        if exists and LOCAL_RANK in (-1, 0):
+            d = f'Scanning {cache_path}... {nf} images, {nm + ne} backgrounds, {nc} corrupt'
             tqdm(None, desc=prefix + d, total=n, initial=n, bar_format=TQDM_BAR_FORMAT)  # display cache results
             if cache['msgs']:
                 LOGGER.info('\n'.join(cache['msgs']))  # display warnings
         assert nf > 0 or not augment, f'{prefix}No labels found in {cache_path}, can not start training. {HELP_URL}'
 
         # Read cache
         [cache.pop(k) for k in ('hash', 'version', 'msgs')]  # remove items
@@ -537,15 +549,15 @@
         include_class = []  # filter labels to include only these classes (optional)
         include_class_array = np.array(include_class).reshape(1, -1)
         for i, (label, segment) in enumerate(zip(self.labels, self.segments)):
             if include_class:
                 j = (label[:, 0:1] == include_class_array).any(1)
                 self.labels[i] = label[j]
                 if segment:
-                    self.segments[i] = segment[j]
+                    self.segments[i] = [segment[si] for si, idx in enumerate(j) if idx]
             if single_cls:  # single-class training, merge all classes into 0
                 self.labels[i][:, 0] = 0
 
         # Rectangular Training
         if self.rect:
             # Sort by aspect ratio
             s = self.shapes  # wh
@@ -575,90 +587,89 @@
             cache_images = False
         self.ims = [None] * n
         self.npy_files = [Path(f).with_suffix('.npy') for f in self.im_files]
         if cache_images:
             b, gb = 0, 1 << 30  # bytes of cached images, bytes per gigabytes
             self.im_hw0, self.im_hw = [None] * n, [None] * n
             fcn = self.cache_images_to_disk if cache_images == 'disk' else self.load_image
-            results = ThreadPool(NUM_THREADS).imap(fcn, range(n))
-            pbar = tqdm(enumerate(results), total=n, bar_format=TQDM_BAR_FORMAT, disable=LOCAL_RANK > 0)
-            for i, x in pbar:
-                if cache_images == 'disk':
-                    b += self.npy_files[i].stat().st_size
-                else:  # 'ram'
-                    self.ims[i], self.im_hw0[i], self.im_hw[i] = x  # im, hw_orig, hw_resized = load_image(self, i)
-                    b += self.ims[i].nbytes
-                pbar.desc = f'{prefix}Caching images ({b / gb:.1f}GB {cache_images})'
-            pbar.close()
+            with ThreadPool(NUM_THREADS) as pool:
+                results = pool.imap(fcn, range(n))
+                pbar = tqdm(enumerate(results), total=n, bar_format=TQDM_BAR_FORMAT, disable=LOCAL_RANK > 0)
+                for i, x in pbar:
+                    if cache_images == 'disk':
+                        b += self.npy_files[i].stat().st_size
+                    else:  # 'ram'
+                        self.ims[i], self.im_hw0[i], self.im_hw[i] = x  # im, hw_orig, hw_resized = load_image(self, i)
+                        b += self.ims[i].nbytes
+                    pbar.desc = f'{prefix}Caching images ({b / gb:.1f}GB {cache_images})'
+                pbar.close()
 
     def check_cache_ram(self, safety_margin=0.1, prefix=''):
-        # Check image caching requirements vs available memory
+        """Check image caching requirements vs available memory."""
         b, gb = 0, 1 << 30  # bytes of cached images, bytes per gigabytes
         n = min(self.n, 30)  # extrapolate from 30 random images
         for _ in range(n):
             im = cv2.imread(random.choice(self.im_files))  # sample image
             ratio = self.img_size / max(im.shape[0], im.shape[1])  # max(h, w)  # ratio
             b += im.nbytes * ratio ** 2
         mem_required = b * self.n / n  # GB required to cache dataset into RAM
         mem = psutil.virtual_memory()
         cache = mem_required * (1 + safety_margin) < mem.available  # to cache or not to cache, that is the question
         if not cache:
-            LOGGER.info(f"{prefix}{mem_required / gb:.1f}GB RAM required, "
-                        f"{mem.available / gb:.1f}/{mem.total / gb:.1f}GB available, "
+            LOGGER.info(f'{prefix}{mem_required / gb:.1f}GB RAM required, '
+                        f'{mem.available / gb:.1f}/{mem.total / gb:.1f}GB available, '
                         f"{'caching images ✅' if cache else 'not caching images ⚠️'}")
         return cache
 
     def cache_labels(self, path=Path('./labels.cache'), prefix=''):
+        """Cache labels and save as numpy file for next time."""
         # Cache dataset labels, check images and read shapes
+        if path.exists():
+            path.unlink()  # remove *.cache file if exists
         x = {}  # dict
         nm, nf, ne, nc, msgs = 0, 0, 0, 0, []  # number missing, found, empty, corrupt, messages
-        desc = f"{prefix}Scanning {path.parent / path.stem}..."
-        with Pool(NUM_THREADS) as pool:
-            pbar = tqdm(pool.imap(verify_image_label, zip(self.im_files, self.label_files, repeat(prefix))),
-                        desc=desc,
-                        total=len(self.im_files),
-                        bar_format=TQDM_BAR_FORMAT)
+        desc = f'{prefix}Scanning {path.parent / path.stem}...'
+        total = len(self.im_files)
+        with ThreadPool(NUM_THREADS) as pool:
+            results = pool.imap(verify_image_label, zip(self.im_files, self.label_files, repeat(prefix)))
+            pbar = tqdm(results, desc=desc, total=total, bar_format=TQDM_BAR_FORMAT)
             for im_file, lb, shape, segments, nm_f, nf_f, ne_f, nc_f, msg in pbar:
                 nm += nm_f
                 nf += nf_f
                 ne += ne_f
                 nc += nc_f
                 if im_file:
                     x[im_file] = [lb, shape, segments]
                 if msg:
                     msgs.append(msg)
-                pbar.desc = f"{desc} {nf} images, {nm + ne} backgrounds, {nc} corrupt"
+                pbar.desc = f'{desc} {nf} images, {nm + ne} backgrounds, {nc} corrupt'
+            pbar.close()
 
-        pbar.close()
         if msgs:
             LOGGER.info('\n'.join(msgs))
         if nf == 0:
             LOGGER.warning(f'{prefix}WARNING ⚠️ No labels found in {path}. {HELP_URL}')
         x['hash'] = get_hash(self.label_files + self.im_files)
         x['results'] = nf, nm, ne, nc, len(self.im_files)
         x['msgs'] = msgs  # warnings
         x['version'] = self.cache_version  # cache version
-        try:
-            np.save(path, x)  # save cache for next time
+        if is_dir_writeable(path.parent):
+            np.save(str(path), x)  # save cache for next time
             path.with_suffix('.cache.npy').rename(path)  # remove .npy suffix
             LOGGER.info(f'{prefix}New cache created: {path}')
-        except Exception as e:
-            LOGGER.warning(f'{prefix}WARNING ⚠️ Cache directory {path.parent} is not writeable: {e}')  # not writeable
+        else:
+            LOGGER.warning(f'{prefix}WARNING ⚠️ Cache directory {path.parent} is not writeable')  # not writeable
         return x
 
     def __len__(self):
+        """Returns the length of 'im_files' attribute."""
         return len(self.im_files)
 
-    # def __iter__(self):
-    #     self.count = -1
-    #     print('ran dataset iter')
-    #     #self.shuffled_vector = np.random.permutation(self.nF) if self.augment else np.arange(self.nF)
-    #     return self
-
     def __getitem__(self, index):
+        """Get a sample and its corresponding label, filename and shape from the dataset."""
         index = self.indices[index]  # linear, shuffled, or image_weights
 
         hyp = self.hyp
         mosaic = self.mosaic and random.random() < hyp['mosaic']
         if mosaic:
             # Load mosaic
             img, labels = self.load_mosaic(index)
@@ -725,15 +736,15 @@
         # Convert
         img = img.transpose((2, 0, 1))[::-1]  # HWC to CHW, BGR to RGB
         img = np.ascontiguousarray(img)
 
         return torch.from_numpy(img), labels_out, self.im_files[index], shapes
 
     def load_image(self, i):
-        # Loads 1 image from dataset index 'i', returns (im, original hw, resized hw)
+        """Loads 1 image from dataset index 'i', returns (im, original hw, resized hw)."""
         im, f, fn = self.ims[i], self.im_files[i], self.npy_files[i],
         if im is None:  # not cached in RAM
             if fn.exists():  # load npy
                 im = np.load(fn)
             else:  # read image
                 im = cv2.imread(f)  # BGR
                 assert im is not None, f'Image Not Found {f}'
@@ -742,31 +753,31 @@
             if r != 1:  # if sizes are not equal
                 interp = cv2.INTER_LINEAR if (self.augment or r > 1) else cv2.INTER_AREA
                 im = cv2.resize(im, (math.ceil(w0 * r), math.ceil(h0 * r)), interpolation=interp)
             return im, (h0, w0), im.shape[:2]  # im, hw_original, hw_resized
         return self.ims[i], self.im_hw0[i], self.im_hw[i]  # im, hw_original, hw_resized
 
     def cache_images_to_disk(self, i):
-        # Saves an image as an *.npy file for faster loading
+        """Saves an image as an *.npy file for faster loading."""
         f = self.npy_files[i]
         if not f.exists():
             np.save(f.as_posix(), cv2.imread(self.im_files[i]))
 
     def load_mosaic(self, index):
-        # YOLOv5 4-mosaic loader. Loads 1 image + 3 random images into a 4-image mosaic
+        """YOLOv5 4-mosaic loader. Loads 1 image + 3 random images into a 4-image mosaic."""
         labels4, segments4 = [], []
         s = self.img_size
         yc, xc = (int(random.uniform(-x, 2 * s + x)) for x in self.mosaic_border)  # mosaic center x, y
         indices = [index] + random.choices(self.indices, k=3)  # 3 additional image indices
         random.shuffle(indices)
         for i, index in enumerate(indices):
             # Load image
             img, _, (h, w) = self.load_image(index)
 
-            # place img in img4
+            # Place img in img4
             if i == 0:  # top left
                 img4 = np.full((s * 2, s * 2, img.shape[2]), 114, dtype=np.uint8)  # base image with 4 tiles
                 x1a, y1a, x2a, y2a = max(xc - w, 0), max(yc - h, 0), xc, yc  # xmin, ymin, xmax, ymax (large image)
                 x1b, y1b, x2b, y2b = w - (x2a - x1a), h - (y2a - y1a), w, h  # xmin, ymin, xmax, ymax (small image)
             elif i == 1:  # top right
                 x1a, y1a, x2a, y2a = xc, max(yc - h, 0), min(xc + w, s * 2), yc
                 x1b, y1b, x2b, y2b = 0, h - (y2a - y1a), min(w, x2a - x1a), h
@@ -806,25 +817,25 @@
                                            shear=self.hyp['shear'],
                                            perspective=self.hyp['perspective'],
                                            border=self.mosaic_border)  # border to remove
 
         return img4, labels4
 
     def load_mosaic9(self, index):
-        # YOLOv5 9-mosaic loader. Loads 1 image + 8 random images into a 9-image mosaic
+        """YOLOv5 9-mosaic loader. Loads 1 image + 8 random images into a 9-image mosaic."""
         labels9, segments9 = [], []
         s = self.img_size
         indices = [index] + random.choices(self.indices, k=8)  # 8 additional image indices
         random.shuffle(indices)
         hp, wp = -1, -1  # height, width previous
         for i, index in enumerate(indices):
             # Load image
             img, _, (h, w) = self.load_image(index)
 
-            # place img in img9
+            # Place img in img9
             if i == 0:  # center
                 img9 = np.full((s * 3, s * 3, img.shape[2]), 114, dtype=np.uint8)  # base image with 4 tiles
                 h0, w0 = h, w
                 c = s, s, s + w, s + h  # xmin, ymin, xmax, ymax (base) coordinates
             elif i == 1:  # top
                 c = s, s - h, s + w, s
             elif i == 2:  # top right
@@ -884,15 +895,15 @@
                                            perspective=self.hyp['perspective'],
                                            border=self.mosaic_border)  # border to remove
 
         return img9, labels9
 
     @staticmethod
     def collate_fn(batch):
-        # YOLOv8 collate function, outputs dict
+        """YOLOv8 collate function, outputs dict."""
         im, label, path, shapes = zip(*batch)  # transposed
         for i, lb in enumerate(label):
             lb[:, 0] = i  # add target image index for build_targets()
         batch_idx, cls, bboxes = torch.cat(label, 0).split((1, 1, 4), dim=1)
         return {
             'ori_shape': tuple((x[0] if x else None) for x in shapes),
             'ratio_pad': tuple((x[1] if x else None) for x in shapes),
@@ -900,24 +911,24 @@
             'img': torch.stack(im, 0),
             'cls': cls,
             'bboxes': bboxes,
             'batch_idx': batch_idx.view(-1)}
 
     @staticmethod
     def collate_fn_old(batch):
-        # YOLOv5 original collate function
+        """YOLOv5 original collate function."""
         im, label, path, shapes = zip(*batch)  # transposed
         for i, lb in enumerate(label):
             lb[:, 0] = i  # add target image index for build_targets()
         return torch.stack(im, 0), torch.cat(label, 0), path, shapes
 
 
 # Ancillary functions --------------------------------------------------------------------------------------------------
 def flatten_recursive(path=DATASETS_DIR / 'coco128'):
-    # Flatten a recursive directory by bringing all files to top level
+    """Flatten a recursive directory by bringing all files to top level."""
     new_path = Path(f'{str(path)}_flat')
     if os.path.exists(new_path):
         shutil.rmtree(new_path)  # delete output folder
     os.makedirs(new_path)  # make new output folder
     for file in tqdm(glob.glob(f'{str(Path(path))}/**/*.*', recursive=True)):
         shutil.copyfile(file, new_path / Path(file).name)
 
@@ -926,42 +937,42 @@
     # Convert detection dataset into classification dataset, with one directory per class
     path = Path(path)  # images dir
     shutil.rmtree(path / 'classification') if (path / 'classification').is_dir() else None  # remove existing
     files = list(path.rglob('*.*'))
     n = len(files)  # number of files
     for im_file in tqdm(files, total=n):
         if im_file.suffix[1:] in IMG_FORMATS:
-            # image
+            # Image
             im = cv2.imread(str(im_file))[..., ::-1]  # BGR to RGB
             h, w = im.shape[:2]
 
-            # labels
+            # Labels
             lb_file = Path(img2label_paths([str(im_file)])[0])
             if Path(lb_file).exists():
                 with open(lb_file) as f:
                     lb = np.array([x.split() for x in f.read().strip().splitlines()], dtype=np.float32)  # labels
 
                 for j, x in enumerate(lb):
                     c = int(x[0])  # class
                     f = (path / 'classifier') / f'{c}' / f'{path.stem}_{im_file.stem}_{j}.jpg'  # new filename
                     if not f.parent.is_dir():
                         f.parent.mkdir(parents=True)
 
                     b = x[1:] * [w, h, w, h]  # box
-                    # b[2:] = b[2:].max()  # rectangle to square
+                    # B[2:] = b[2:].max()  # rectangle to square
                     b[2:] = b[2:] * 1.2 + 3  # pad
                     b = xywh2xyxy(b.reshape(-1, 4)).ravel().astype(int)
 
                     b[[0, 2]] = np.clip(b[[0, 2]], 0, w)  # clip boxes outside of image
                     b[[1, 3]] = np.clip(b[[1, 3]], 0, h)
                     assert cv2.imwrite(str(f), im[b[1]:b[3], b[0]:b[2]]), f'box failure in {f}'
 
 
 def autosplit(path=DATASETS_DIR / 'coco128/images', weights=(0.9, 0.1, 0.0), annotated_only=False):
-    """ Autosplit a dataset into train/val/test splits and save path/autosplit_*.txt files
+    """Autosplit a dataset into train/val/test splits and save path/autosplit_*.txt files
     Usage: from utils.dataloaders import *; autosplit()
     Arguments
         path:            Path to images directory
         weights:         Train, val, test weights (list, tuple)
         annotated_only:  Only use images with an annotated txt file
     """
     path = Path(path)  # images dir
@@ -979,32 +990,32 @@
     for i, img in tqdm(zip(indices, files), total=n):
         if not annotated_only or Path(img2label_paths([str(img)])[0]).exists():  # check label
             with open(path.parent / txt[i], 'a') as f:
                 f.write(f'./{img.relative_to(path.parent).as_posix()}' + '\n')  # add image to txt file
 
 
 def verify_image_label(args):
-    # Verify one image-label pair
+    """Verify one image-label pair."""
     im_file, lb_file, prefix = args
     nm, nf, ne, nc, msg, segments = 0, 0, 0, 0, '', []  # number (missing, found, empty, corrupt), message, segments
     try:
-        # verify images
+        # Verify images
         im = Image.open(im_file)
         im.verify()  # PIL verify
         shape = exif_size(im)  # image size
         assert (shape[0] > 9) & (shape[1] > 9), f'image size {shape} <10 pixels'
         assert im.format.lower() in IMG_FORMATS, f'invalid image format {im.format}'
         if im.format.lower() in ('jpg', 'jpeg'):
             with open(im_file, 'rb') as f:
                 f.seek(-2, 2)
                 if f.read() != b'\xff\xd9':  # corrupt JPEG
                     ImageOps.exif_transpose(Image.open(im_file)).save(im_file, 'JPEG', subsampling=0, quality=100)
                     msg = f'{prefix}WARNING ⚠️ {im_file}: corrupt JPEG restored and saved'
 
-        # verify labels
+        # Verify labels
         if os.path.isfile(lb_file):
             nf = 1  # label found
             with open(lb_file) as f:
                 lb = [x.split() for x in f.read().strip().splitlines() if len(x)]
                 if any(len(x) > 6 for x in lb):  # is segment
                     classes = np.array([x[0] for x in lb], dtype=np.float32)
                     segments = [np.array(x[1:], dtype=np.float32).reshape(-1, 2) for x in lb]  # (cls, xy1...)
@@ -1030,178 +1041,60 @@
         return im_file, lb, shape, segments, nm, nf, ne, nc, msg
     except Exception as e:
         nc = 1
         msg = f'{prefix}WARNING ⚠️ {im_file}: ignoring corrupt image/label: {e}'
         return [None, None, None, None, nm, nf, ne, nc, msg]
 
 
-class HUBDatasetStats():
-    """ Class for generating HUB dataset JSON and `-hub` dataset directory
-
-    Arguments
-        path:           Path to data.yaml or data.zip (with data.yaml inside data.zip)
-        autodownload:   Attempt to download dataset if not found locally
-
-    Usage
-        from utils.dataloaders import HUBDatasetStats
-        stats = HUBDatasetStats('coco128.yaml', autodownload=True)  # usage 1
-        stats = HUBDatasetStats('path/to/coco128.zip')  # usage 2
-        stats.get_json(save=False)
-        stats.process_images()
-    """
-
-    def __init__(self, path='coco128.yaml', autodownload=False):
-        # Initialize class
-        zipped, data_dir, yaml_path = self._unzip(Path(path))
-        try:
-            with open(check_yaml(yaml_path), errors='ignore') as f:
-                data = yaml.safe_load(f)  # data dict
-                if zipped:
-                    data['path'] = data_dir
-        except Exception as e:
-            raise Exception("error/HUB/dataset_stats/yaml_load") from e
-
-        check_dataset(data, autodownload)  # download dataset if missing
-        self.hub_dir = Path(data['path'] + '-hub')
-        self.im_dir = self.hub_dir / 'images'
-        self.im_dir.mkdir(parents=True, exist_ok=True)  # makes /images
-        self.stats = {'nc': data['nc'], 'names': list(data['names'].values())}  # statistics dictionary
-        self.data = data
-
-    @staticmethod
-    def _find_yaml(dir):
-        # Return data.yaml file
-        files = list(dir.glob('*.yaml')) or list(dir.rglob('*.yaml'))  # try root level first and then recursive
-        assert files, f'No *.yaml file found in {dir}'
-        if len(files) > 1:
-            files = [f for f in files if f.stem == dir.stem]  # prefer *.yaml files that match dir name
-            assert files, f'Multiple *.yaml files found in {dir}, only 1 *.yaml file allowed'
-        assert len(files) == 1, f'Multiple *.yaml files found: {files}, only 1 *.yaml file allowed in {dir}'
-        return files[0]
-
-    def _unzip(self, path):
-        # Unzip data.zip
-        if not str(path).endswith('.zip'):  # path is data.yaml
-            return False, None, path
-        assert Path(path).is_file(), f'Error unzipping {path}, file not found'
-        unzip_file(path, path=path.parent)
-        dir = path.with_suffix('')  # dataset directory == zip name
-        assert dir.is_dir(), f'Error unzipping {path}, {dir} not found. path/to/abc.zip MUST unzip to path/to/abc/'
-        return True, str(dir), self._find_yaml(dir)  # zipped, data_dir, yaml_path
-
-    def _hub_ops(self, f, max_dim=1920):
-        # HUB ops for 1 image 'f': resize and save at reduced quality in /dataset-hub for web/app viewing
-        f_new = self.im_dir / Path(f).name  # dataset-hub image filename
-        try:  # use PIL
-            im = Image.open(f)
-            r = max_dim / max(im.height, im.width)  # ratio
-            if r < 1.0:  # image too large
-                im = im.resize((int(im.width * r), int(im.height * r)))
-            im.save(f_new, 'JPEG', quality=50, optimize=True)  # save
-        except Exception as e:  # use OpenCV
-            LOGGER.info(f'WARNING ⚠️ HUB ops PIL failure {f}: {e}')
-            im = cv2.imread(f)
-            im_height, im_width = im.shape[:2]
-            r = max_dim / max(im_height, im_width)  # ratio
-            if r < 1.0:  # image too large
-                im = cv2.resize(im, (int(im_width * r), int(im_height * r)), interpolation=cv2.INTER_AREA)
-            cv2.imwrite(str(f_new), im)
-
-    def get_json(self, save=False, verbose=False):
-        # Return dataset JSON for Ultralytics HUB
-        def _round(labels):
-            # Update labels to integer class and 6 decimal place floats
-            return [[int(c), *(round(x, 4) for x in points)] for c, *points in labels]
-
-        for split in 'train', 'val', 'test':
-            if self.data.get(split) is None:
-                self.stats[split] = None  # i.e. no test set
-                continue
-            dataset = LoadImagesAndLabels(self.data[split])  # load dataset
-            x = np.array([
-                np.bincount(label[:, 0].astype(int), minlength=self.data['nc'])
-                for label in tqdm(dataset.labels, total=dataset.n, desc='Statistics')])  # shape(128x80)
-            self.stats[split] = {
-                'instance_stats': {
-                    'total': int(x.sum()),
-                    'per_class': x.sum(0).tolist()},
-                'image_stats': {
-                    'total': dataset.n,
-                    'unlabelled': int(np.all(x == 0, 1).sum()),
-                    'per_class': (x > 0).sum(0).tolist()},
-                'labels': [{
-                    str(Path(k).name): _round(v.tolist())} for k, v in zip(dataset.im_files, dataset.labels)]}
-
-        # Save, print and return
-        if save:
-            stats_path = self.hub_dir / 'stats.json'
-            print(f'Saving {stats_path.resolve()}...')
-            with open(stats_path, 'w') as f:
-                json.dump(self.stats, f)  # save stats.json
-        if verbose:
-            print(json.dumps(self.stats, indent=2, sort_keys=False))
-        return self.stats
-
-    def process_images(self):
-        # Compress images for Ultralytics HUB
-        for split in 'train', 'val', 'test':
-            if self.data.get(split) is None:
-                continue
-            dataset = LoadImagesAndLabels(self.data[split])  # load dataset
-            desc = f'{split} images'
-            for _ in tqdm(ThreadPool(NUM_THREADS).imap(self._hub_ops, dataset.im_files), total=dataset.n, desc=desc):
-                pass
-        print(f'Done. All images saved to {self.im_dir}')
-        return self.im_dir
-
-
 # Classification dataloaders -------------------------------------------------------------------------------------------
 class ClassificationDataset(torchvision.datasets.ImageFolder):
     """
     YOLOv5 Classification Dataset.
     Arguments
         root:  Dataset path
         transform:  torchvision transforms, used by default
         album_transform: Albumentations transforms, used if installed
     """
 
     def __init__(self, root, augment, imgsz, cache=False):
+        """Initialize YOLO dataset with root, augmentation, image size, and cache parameters."""
         super().__init__(root=root)
         self.torch_transforms = classify_transforms(imgsz)
         self.album_transforms = classify_albumentations(augment, imgsz) if augment else None
         self.cache_ram = cache is True or cache == 'ram'
         self.cache_disk = cache == 'disk'
         self.samples = [list(x) + [Path(x[0]).with_suffix('.npy'), None] for x in self.samples]  # file, index, npy, im
 
     def __getitem__(self, i):
+        """Retrieves data items of 'dataset' via indices & creates InfiniteDataLoader."""
         f, j, fn, im = self.samples[i]  # filename, index, filename.with_suffix('.npy'), image
         if self.cache_ram and im is None:
             im = self.samples[i][3] = cv2.imread(f)
         elif self.cache_disk:
             if not fn.exists():  # load npy
                 np.save(fn.as_posix(), cv2.imread(f))
             im = np.load(fn)
         else:  # read image
             im = cv2.imread(f)  # BGR
         if self.album_transforms:
-            sample = self.album_transforms(image=cv2.cvtColor(im, cv2.COLOR_BGR2RGB))["image"]
+            sample = self.album_transforms(image=cv2.cvtColor(im, cv2.COLOR_BGR2RGB))['image']
         else:
             sample = self.torch_transforms(im)
         return sample, j
 
 
 def create_classification_dataloader(path,
                                      imgsz=224,
                                      batch_size=16,
                                      augment=True,
                                      cache=False,
                                      rank=-1,
                                      workers=8,
                                      shuffle=True):
-    # Returns Dataloader object to be used with YOLOv5 Classifier
+    """Returns Dataloader object to be used with YOLOv5 Classifier."""
     with torch_distributed_zero_first(rank):  # init dataset *.cache only once if DDP
         dataset = ClassificationDataset(root=path, imgsz=imgsz, augment=augment, cache=cache)
     batch_size = min(batch_size, len(dataset))
     nd = torch.cuda.device_count()
     nw = min([os.cpu_count() // max(nd, 1), batch_size if batch_size > 1 else 0, workers])
     sampler = None if rank == -1 else distributed.DistributedSampler(dataset, shuffle=shuffle)
     generator = torch.Generator()
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/data/dataset_wrappers.py` & `ultralytics-8.0.90/ultralytics/yolo/data/dataset_wrappers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,54 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import collections
 from copy import deepcopy
 
 from .augment import LetterBox
 
 
 class MixAndRectDataset:
-    """A wrapper of multiple images mixed dataset.
+    """
+    A dataset class that applies mosaic and mixup transformations as well as rectangular training.
 
-    Args:
-        dataset (:obj:`BaseDataset`): The dataset to be mixed.
-        transforms (Sequence[dict]): config dict to be composed.
+    Attributes:
+        dataset: The base dataset.
+        imgsz: The size of the images in the dataset.
     """
 
     def __init__(self, dataset):
+        """
+        Args:
+            dataset (BaseDataset): The base dataset to apply transformations to.
+        """
         self.dataset = dataset
         self.imgsz = dataset.imgsz
 
     def __len__(self):
+        """Returns the number of items in the dataset."""
         return len(self.dataset)
 
     def __getitem__(self, index):
+        """
+        Applies mosaic, mixup and rectangular training transformations to an item in the dataset.
+
+        Args:
+            index (int): Index of the item in the dataset.
+
+        Returns:
+            (dict): A dictionary containing the transformed item data.
+        """
         labels = deepcopy(self.dataset[index])
         for transform in self.dataset.transforms.tolist():
-            # mosaic and mixup
-            if hasattr(transform, "get_indexes"):
+            # Mosaic and mixup
+            if hasattr(transform, 'get_indexes'):
                 indexes = transform.get_indexes(self.dataset)
                 if not isinstance(indexes, collections.abc.Sequence):
                     indexes = [indexes]
                 mix_labels = [deepcopy(self.dataset[index]) for index in indexes]
-                labels["mix_labels"] = mix_labels
+                labels['mix_labels'] = mix_labels
             if self.dataset.rect and isinstance(transform, LetterBox):
                 transform.new_shape = self.dataset.batch_shapes[self.dataset.batch[index]]
             labels = transform(labels)
-            if "mix_labels" in labels:
-                labels.pop("mix_labels")
+            if 'mix_labels' in labels:
+                labels.pop('mix_labels')
         return labels
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/data/datasets/Argoverse.yaml` & `ultralytics-8.0.90/ultralytics/datasets/Argoverse.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 # Argoverse-HD dataset (ring-front-center camera) http://www.cs.cmu.edu/~mengtial/proj/streaming/ by Argo AI
-# Example usage: python train.py --data Argoverse.yaml
+# Example usage: yolo train data=Argoverse.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── Argoverse  ← downloads here (31.3 GB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/Argoverse  # dataset root dir
 train: Argoverse-1.1/images/train/  # train images (relative to 'path') 39384 images
@@ -24,18 +24,17 @@
   6: traffic_light
   7: stop_sign
 
 
 # Download script/URL (optional) ---------------------------------------------------------------------------------------
 download: |
   import json
-
   from tqdm import tqdm
-  from utils.general import download, Path
-
+  from ultralytics.yolo.utils.downloads import download
+  from pathlib import Path
 
   def argoverse2yolo(set):
       labels = {}
       a = json.load(open(set, "rb"))
       for annot in tqdm(a['annotations'], desc=f"Converting {set} to YOLOv5 format..."):
           img_id = annot['image_id']
           img_name = a['images'][img_id]['name']
@@ -61,14 +60,14 @@
           with open(k, "w") as f:
               f.writelines(labels[k])
 
 
   # Download
   dir = Path(yaml['path'])  # dataset root dir
   urls = ['https://argoverse-hd.s3.us-east-2.amazonaws.com/Argoverse-HD-Full.zip']
-  download(urls, dir=dir, delete=False)
+  download(urls, dir=dir)
 
   # Convert
   annotations_dir = 'Argoverse-HD/annotations/'
   (dir / 'Argoverse-1.1' / 'tracking').rename(dir / 'Argoverse-1.1' / 'images')  # rename 'tracking' to 'images'
   for d in "train.json", "val.json":
       argoverse2yolo(dir / annotations_dir / d)  # convert VisDrone annotations to YOLO labels
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/data/datasets/GlobalWheat2020.yaml` & `ultralytics-8.0.90/ultralytics/datasets/GlobalWheat2020.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 # Global Wheat 2020 dataset http://www.global-wheat.com/ by University of Saskatchewan
-# Example usage: python train.py --data GlobalWheat2020.yaml
+# Example usage: yolo train data=GlobalWheat2020.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── GlobalWheat2020  ← downloads here (7.0 GB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/GlobalWheat2020  # dataset root dir
 train: # train images (relative to 'path') 3422 images
@@ -28,16 +28,16 @@
 # Classes
 names:
   0: wheat_head
 
 
 # Download script/URL (optional) ---------------------------------------------------------------------------------------
 download: |
-  from utils.general import download, Path
-
+  from ultralytics.yolo.utils.downloads import download
+  from pathlib import Path
 
   # Download
   dir = Path(yaml['path'])  # dataset root dir
   urls = ['https://zenodo.org/record/4298502/files/global-wheat-codalab-official.zip',
           'https://github.com/ultralytics/yolov5/releases/download/v1.0/GlobalWheat2020_labels.zip']
   download(urls, dir=dir)
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/data/datasets/Objects365.yaml` & `ultralytics-8.0.90/ultralytics/datasets/Objects365.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 # Objects365 dataset https://www.objects365.org/ by Megvii
-# Example usage: python train.py --data Objects365.yaml
+# Example usage: yolo train data=Objects365.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── Objects365  ← downloads here (712 GB = 367G data + 345G zips)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/Objects365  # dataset root dir
 train: images/train  # train images (relative to 'path') 1742289 images
@@ -382,15 +382,20 @@
   364: Table Tennis
 
 
 # Download script/URL (optional) ---------------------------------------------------------------------------------------
 download: |
   from tqdm import tqdm
 
-  from utils.general import Path, check_requirements, download, np, xyxy2xywhn
+  from ultralytics.yolo.utils.checks import check_requirements
+  from ultralytics.yolo.utils.downloads import download
+  from ultralytics.yolo.utils.ops import xyxy2xywhn
+
+  import numpy as np
+  from pathlib import Path
 
   check_requirements(('pycocotools>=2.0',))
   from pycocotools.coco import COCO
 
   # Make Directories
   dir = Path(yaml['path'])  # dataset root dir
   for p in 'images', 'labels':
@@ -402,20 +407,20 @@
   for split, patches in [('train', 50 + 1), ('val', 43 + 1)]:
       print(f"Processing {split} in {patches} patches ...")
       images, labels = dir / 'images' / split, dir / 'labels' / split
 
       # Download
       url = f"https://dorc.ks3-cn-beijing.ksyun.com/data-set/2020Objects365%E6%95%B0%E6%8D%AE%E9%9B%86/{split}/"
       if split == 'train':
-          download([f'{url}zhiyuan_objv2_{split}.tar.gz'], dir=dir, delete=False)  # annotations json
-          download([f'{url}patch{i}.tar.gz' for i in range(patches)], dir=images, curl=True, delete=False, threads=8)
+          download([f'{url}zhiyuan_objv2_{split}.tar.gz'], dir=dir)  # annotations json
+          download([f'{url}patch{i}.tar.gz' for i in range(patches)], dir=images, curl=True, threads=8)
       elif split == 'val':
-          download([f'{url}zhiyuan_objv2_{split}.json'], dir=dir, delete=False)  # annotations json
-          download([f'{url}images/v1/patch{i}.tar.gz' for i in range(15 + 1)], dir=images, curl=True, delete=False, threads=8)
-          download([f'{url}images/v2/patch{i}.tar.gz' for i in range(16, patches)], dir=images, curl=True, delete=False, threads=8)
+          download([f'{url}zhiyuan_objv2_{split}.json'], dir=dir)  # annotations json
+          download([f'{url}images/v1/patch{i}.tar.gz' for i in range(15 + 1)], dir=images, curl=True, threads=8)
+          download([f'{url}images/v2/patch{i}.tar.gz' for i in range(16, patches)], dir=images, curl=True, threads=8)
 
       # Move
       for f in tqdm(images.rglob('*.jpg'), desc=f'Moving {split} images'):
           f.rename(images / f.name)  # move to /images/{split}
 
       # Labels
       coco = COCO(dir / f'zhiyuan_objv2_{split}.json')
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/data/datasets/SKU-110K.yaml` & `ultralytics-8.0.90/ultralytics/datasets/SKU-110K.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 # SKU-110K retail items dataset https://github.com/eg4000/SKU110K_CVPR19 by Trax Retail
-# Example usage: python train.py --data SKU-110K.yaml
+# Example usage: yolo train data=SKU-110K.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── SKU-110K  ← downloads here (13.6 GB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/SKU-110K  # dataset root dir
 train: train.txt  # train images (relative to 'path')  8219 images
@@ -17,23 +17,28 @@
 names:
   0: object
 
 
 # Download script/URL (optional) ---------------------------------------------------------------------------------------
 download: |
   import shutil
+  from pathlib import Path
+
+  import numpy as np
+  import pandas as pd
   from tqdm import tqdm
-  from utils.general import np, pd, Path, download, xyxy2xywh
 
+  from ultralytics.yolo.utils.downloads import download
+  from ultralytics.yolo.utils.ops import xyxy2xywh
 
   # Download
   dir = Path(yaml['path'])  # dataset root dir
   parent = Path(dir.parent)  # download dir
   urls = ['http://trax-geometry.s3.amazonaws.com/cvpr_challenge/SKU110K_fixed.tar.gz']
-  download(urls, dir=parent, delete=False)
+  download(urls, dir=parent)
 
   # Rename directories
   if dir.exists():
       shutil.rmtree(dir)
   (parent / 'SKU110K_fixed').rename(dir)  # rename dir
   (dir / 'labels').mkdir(parents=True, exist_ok=True)  # create labels dir
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/data/datasets/VOC.yaml` & `ultralytics-8.0.90/ultralytics/datasets/VOC.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 # PASCAL VOC dataset http://host.robots.ox.ac.uk/pascal/VOC by University of Oxford
-# Example usage: python train.py --data VOC.yaml
+# Example usage: yolo train data=VOC.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── VOC  ← downloads here (2.8 GB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/VOC
 train: # train images (relative to 'path')  16551 images
@@ -44,16 +44,16 @@
 
 
 # Download script/URL (optional) ---------------------------------------------------------------------------------------
 download: |
   import xml.etree.ElementTree as ET
 
   from tqdm import tqdm
-  from utils.general import download, Path
-
+  from ultralytics.yolo.utils.downloads import download
+  from pathlib import Path
 
   def convert_label(path, lb_path, year, image_id):
       def convert_box(size, box):
           dw, dh = 1. / size[0], 1. / size[1]
           x, y, w, h = (box[0] + box[1]) / 2.0 - 1, (box[2] + box[3]) / 2.0 - 1, box[1] - box[0], box[3] - box[2]
           return x * dw, y * dh, w * dw, h * dh
 
@@ -77,15 +77,15 @@
 
   # Download
   dir = Path(yaml['path'])  # dataset root dir
   url = 'https://github.com/ultralytics/yolov5/releases/download/v1.0/'
   urls = [f'{url}VOCtrainval_06-Nov-2007.zip',  # 446MB, 5012 images
           f'{url}VOCtest_06-Nov-2007.zip',  # 438MB, 4953 images
           f'{url}VOCtrainval_11-May-2012.zip']  # 1.95GB, 17126 images
-  download(urls, dir=dir / 'images', delete=False, curl=True, threads=3)
+  download(urls, dir=dir / 'images', curl=True, threads=3)
 
   # Convert
   path = dir / 'images/VOCdevkit'
   for year, image_set in ('2012', 'train'), ('2012', 'val'), ('2007', 'train'), ('2007', 'val'), ('2007', 'test'):
       imgs_path = dir / 'images' / f'{image_set}{year}'
       lbs_path = dir / 'labels' / f'{image_set}{year}'
       imgs_path.mkdir(exist_ok=True, parents=True)
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/data/datasets/VisDrone.yaml` & `ultralytics-8.0.90/ultralytics/datasets/VisDrone.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 # VisDrone2019-DET dataset https://github.com/VisDrone/VisDrone-Dataset by Tianjin University
-# Example usage: python train.py --data VisDrone.yaml
+# Example usage: yolo train data=VisDrone.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── VisDrone  ← downloads here (2.3 GB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/VisDrone  # dataset root dir
 train: VisDrone2019-DET-train/images  # train images (relative to 'path')  6471 images
@@ -25,15 +25,18 @@
   7: awning-tricycle
   8: bus
   9: motor
 
 
 # Download script/URL (optional) ---------------------------------------------------------------------------------------
 download: |
-  from utils.general import download, os, Path
+  import os
+  from pathlib import Path
+
+  from ultralytics.yolo.utils.downloads import download
 
   def visdrone2yolo(dir):
       from PIL import Image
       from tqdm import tqdm
 
       def convert_box(size, box):
           # Convert VisDrone box to YOLO xywh box
@@ -49,15 +52,15 @@
           with open(f, 'r') as file:  # read annotation.txt
               for row in [x.split(',') for x in file.read().strip().splitlines()]:
                   if row[4] == '0':  # VisDrone 'ignored regions' class 0
                       continue
                   cls = int(row[5]) - 1
                   box = convert_box(img_size, tuple(map(int, row[:4])))
                   lines.append(f"{cls} {' '.join(f'{x:.6f}' for x in box)}\n")
-                  with open(str(f).replace(os.sep + 'annotations' + os.sep, os.sep + 'labels' + os.sep), 'w') as fl:
+                  with open(str(f).replace(f'{os.sep}annotations{os.sep}', f'{os.sep}labels{os.sep}'), 'w') as fl:
                       fl.writelines(lines)  # write label.txt
 
 
   # Download
   dir = Path(yaml['path'])  # dataset root dir
   urls = ['https://github.com/ultralytics/yolov5/releases/download/v1.0/VisDrone2019-DET-train.zip',
           'https://github.com/ultralytics/yolov5/releases/download/v1.0/VisDrone2019-DET-val.zip',
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/data/datasets/coco.yaml` & `ultralytics-8.0.90/ultralytics/datasets/coco.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 # COCO 2017 dataset http://cocodataset.org by Microsoft
-# Example usage: python train.py --data coco.yaml
+# Example usage: yolo train data=coco.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── coco  ← downloads here (20.1 GB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/coco  # dataset root dir
 train: train2017.txt  # train images (relative to 'path') 118287 images
@@ -95,19 +95,21 @@
   77: teddy bear
   78: hair drier
   79: toothbrush
 
 
 # Download script/URL (optional)
 download: |
-  from utils.general import download, Path
+  from ultralytics.yolo.utils.downloads import download
+  from pathlib import Path
+
   # Download labels
   segments = True  # segment or box labels
   dir = Path(yaml['path'])  # dataset root dir
   url = 'https://github.com/ultralytics/yolov5/releases/download/v1.0/'
   urls = [url + ('coco2017labels-segments.zip' if segments else 'coco2017labels.zip')]  # labels
   download(urls, dir=dir.parent)
   # Download data
   urls = ['http://images.cocodataset.org/zips/train2017.zip',  # 19G, 118k images
           'http://images.cocodataset.org/zips/val2017.zip',  # 1G, 5k images
           'http://images.cocodataset.org/zips/test2017.zip']  # 7G, 41k images (optional)
-  download(urls, dir=dir / 'images', threads=3)
+  download(urls, dir=dir / 'images', threads=3)
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/data/datasets/coco128-seg.yaml` & `ultralytics-8.0.90/ultralytics/datasets/coco8.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
-# COCO128-seg dataset https://www.kaggle.com/ultralytics/coco128 (first 128 images from COCO train2017) by Ultralytics
-# Example usage: python train.py --data coco128.yaml
+# Ultralytics YOLO 🚀, AGPL-3.0 license
+# COCO8 dataset (first 8 images from COCO train2017) by Ultralytics
+# Example usage: yolo train data=coco8.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
-#     └── coco128-seg  ← downloads here (7 MB)
+#     └── coco8  ← downloads here (1 MB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
-path: ../datasets/coco128-seg  # dataset root dir
-train: images/train2017  # train images (relative to 'path') 128 images
-val: images/train2017  # val images (relative to 'path') 128 images
+path: ../datasets/coco8  # dataset root dir
+train: images/train  # train images (relative to 'path') 4 images
+val: images/val  # val images (relative to 'path') 4 images
 test:  # test images (optional)
 
 # Classes
 names:
   0: person
   1: bicycle
   2: car
@@ -94,8 +94,8 @@
   76: scissors
   77: teddy bear
   78: hair drier
   79: toothbrush
 
 
 # Download script/URL (optional)
-download: https://ultralytics.com/assets/coco128-seg.zip
+download: https://ultralytics.com/assets/coco8.zip
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/data/datasets/coco128.yaml` & `ultralytics-8.0.90/ultralytics/datasets/coco128.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 # COCO128 dataset https://www.kaggle.com/ultralytics/coco128 (first 128 images from COCO train2017) by Ultralytics
-# Example usage: python train.py --data coco128.yaml
+# Example usage: yolo train data=coco128.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── coco128  ← downloads here (7 MB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/coco128  # dataset root dir
 train: images/train2017  # train images (relative to 'path') 128 images
@@ -94,8 +94,8 @@
   76: scissors
   77: teddy bear
   78: hair drier
   79: toothbrush
 
 
 # Download script/URL (optional)
-download: https://ultralytics.com/assets/coco128.zip
+download: https://ultralytics.com/assets/coco128.zip
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/data/datasets/coco8-seg.yaml` & `ultralytics-8.0.90/ultralytics/datasets/coco8-seg.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 # COCO8-seg dataset (first 8 images from COCO train2017) by Ultralytics
-# Example usage: python train.py --data coco8-seg.yaml
+# Example usage: yolo train data=coco8-seg.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── coco8-seg  ← downloads here (1 MB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/coco8-seg  # dataset root dir
 train: images/train  # train images (relative to 'path') 4 images
@@ -94,8 +94,8 @@
   76: scissors
   77: teddy bear
   78: hair drier
   79: toothbrush
 
 
 # Download script/URL (optional)
-download: https://ultralytics.com/assets/coco8-seg.zip
+download: https://ultralytics.com/assets/coco8-seg.zip
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/data/datasets/xView.yaml` & `ultralytics-8.0.90/ultralytics/datasets/xView.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 # DIUx xView 2018 Challenge https://challenge.xviewdataset.org by U.S. National Geospatial-Intelligence Agency (NGA)
 # --------  DOWNLOAD DATA MANUALLY and jar xf val_images.zip to 'datasets/xView' before running train command!  --------
-# Example usage: python train.py --data xView.yaml
+# Example usage: yolo train data=xView.yaml
 # parent
-# ├── yolov5
+# ├── ultralytics
 # └── datasets
 #     └── xView  ← downloads here (20.7 GB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/xView  # dataset root dir
 train: images/autosplit_train.txt  # train images (relative to 'path') 90% of 847 train images
@@ -83,16 +83,16 @@
   import os
   from pathlib import Path
 
   import numpy as np
   from PIL import Image
   from tqdm import tqdm
 
-  from utils.dataloaders import autosplit
-  from utils.general import download, xyxy2xywhn
+  from ultralytics.yolo.data.dataloaders.v5loader import autosplit
+  from ultralytics.yolo.utils.ops import xyxy2xywhn
 
 
   def convert_labels(fname=Path('xView/xView_train.geojson')):
       # Convert xView geoJSON labels to YOLO format
       path = fname.parent
       with open(fname) as f:
           print(f'Loading {fname}...')
@@ -134,15 +134,15 @@
 
 
   # Download manually from https://challenge.xviewdataset.org
   dir = Path(yaml['path'])  # dataset root dir
   # urls = ['https://d307kc0mrhucc3.cloudfront.net/train_labels.zip',  # train labels
   #         'https://d307kc0mrhucc3.cloudfront.net/train_images.zip',  # 15G, 847 train images
   #         'https://d307kc0mrhucc3.cloudfront.net/val_images.zip']  # 5G, 282 val images (no labels)
-  # download(urls, dir=dir, delete=False)
+  # download(urls, dir=dir)
 
   # Convert labels
   convert_labels(dir / 'xView_train.geojson')
 
   # Move images
   images = Path(dir / 'images')
   images.mkdir(parents=True, exist_ok=True)
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/engine/exporter.py` & `ultralytics-8.0.90/ultralytics/yolo/engine/exporter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 """
 Export a YOLOv8 PyTorch model to other formats. TensorFlow exports authored by https://github.com/zldrobit
 
 Format                  | `format=argument`         | Model
 ---                     | ---                       | ---
 PyTorch                 | -                         | yolov8n.pt
 TorchScript             | `torchscript`             | yolov8n.torchscript
@@ -14,99 +14,102 @@
 TensorFlow GraphDef     | `pb`                      | yolov8n.pb
 TensorFlow Lite         | `tflite`                  | yolov8n.tflite
 TensorFlow Edge TPU     | `edgetpu`                 | yolov8n_edgetpu.tflite
 TensorFlow.js           | `tfjs`                    | yolov8n_web_model/
 PaddlePaddle            | `paddle`                  | yolov8n_paddle_model/
 
 Requirements:
-    $ pip install -r requirements.txt coremltools onnx onnx-simplifier onnxruntime openvino-dev tensorflow-cpu  # CPU
-    $ pip install -r requirements.txt coremltools onnx onnx-simplifier onnxruntime-gpu openvino-dev tensorflow  # GPU
+    $ pip install ultralytics[export]
 
 Python:
     from ultralytics import YOLO
-    model = YOLO('yolov8n.yaml')
+    model = YOLO('yolov8n.pt')
     results = model.export(format='onnx')
 
 CLI:
     $ yolo mode=export model=yolov8n.pt format=onnx
 
 Inference:
-    $ python detect.py --weights yolov8n.pt                 # PyTorch
-                                 yolov8n.torchscript        # TorchScript
-                                 yolov8n.onnx               # ONNX Runtime or OpenCV DNN with --dnn
-                                 yolov8n_openvino_model     # OpenVINO
-                                 yolov8n.engine             # TensorRT
-                                 yolov8n.mlmodel            # CoreML (macOS-only)
-                                 yolov8n_saved_model        # TensorFlow SavedModel
-                                 yolov8n.pb                 # TensorFlow GraphDef
-                                 yolov8n.tflite             # TensorFlow Lite
-                                 yolov8n_edgetpu.tflite     # TensorFlow Edge TPU
-                                 yolov8n_paddle_model       # PaddlePaddle
+    $ yolo predict model=yolov8n.pt                 # PyTorch
+                         yolov8n.torchscript        # TorchScript
+                         yolov8n.onnx               # ONNX Runtime or OpenCV DNN with --dnn
+                         yolov8n_openvino_model     # OpenVINO
+                         yolov8n.engine             # TensorRT
+                         yolov8n.mlmodel            # CoreML (macOS-only)
+                         yolov8n_saved_model        # TensorFlow SavedModel
+                         yolov8n.pb                 # TensorFlow GraphDef
+                         yolov8n.tflite             # TensorFlow Lite
+                         yolov8n_edgetpu.tflite     # TensorFlow Edge TPU
+                         yolov8n_paddle_model       # PaddlePaddle
 
 TensorFlow.js:
     $ cd .. && git clone https://github.com/zldrobit/tfjs-yolov5-example.git && cd tfjs-yolov5-example
     $ npm install
     $ ln -s ../../yolov5/yolov8n_web_model public/yolov8n_web_model
     $ npm start
 """
-import contextlib
 import json
 import os
 import platform
-import re
 import subprocess
 import time
 import warnings
-from collections import defaultdict
 from copy import deepcopy
 from pathlib import Path
 
-import hydra
-import numpy as np
-import pandas as pd
 import torch
 
-import ultralytics
-from ultralytics.nn.modules import Detect, Segment
-from ultralytics.nn.tasks import ClassificationModel, DetectionModel, SegmentationModel
-from ultralytics.yolo.configs import get_config
-from ultralytics.yolo.data.dataloaders.stream_loaders import LoadImages
-from ultralytics.yolo.data.utils import check_dataset
-from ultralytics.yolo.utils import DEFAULT_CONFIG, LOGGER, callbacks, colorstr, get_default_args, yaml_save
-from ultralytics.yolo.utils.checks import check_imgsz, check_requirements, check_version, check_yaml
+from ultralytics.nn.autobackend import check_class_names
+from ultralytics.nn.modules import C2f, Detect, Segment
+from ultralytics.nn.tasks import DetectionModel, SegmentationModel
+from ultralytics.yolo.cfg import get_cfg
+from ultralytics.yolo.utils import (DEFAULT_CFG, LINUX, LOGGER, MACOS, __version__, callbacks, colorstr,
+                                    get_default_args, yaml_save)
+from ultralytics.yolo.utils.checks import check_imgsz, check_requirements, check_version
 from ultralytics.yolo.utils.files import file_size
 from ultralytics.yolo.utils.ops import Profile
-from ultralytics.yolo.utils.torch_utils import guess_task_from_head, select_device, smart_inference_mode
+from ultralytics.yolo.utils.torch_utils import get_latest_opset, select_device, smart_inference_mode
 
-MACOS = platform.system() == 'Darwin'  # macOS environment
+ARM64 = platform.machine() in ('arm64', 'aarch64')
 
 
 def export_formats():
-    # YOLOv8 export formats
+    """YOLOv8 export formats."""
+    import pandas
     x = [
         ['PyTorch', '-', '.pt', True, True],
         ['TorchScript', 'torchscript', '.torchscript', True, True],
         ['ONNX', 'onnx', '.onnx', True, True],
         ['OpenVINO', 'openvino', '_openvino_model', True, False],
         ['TensorRT', 'engine', '.engine', False, True],
         ['CoreML', 'coreml', '.mlmodel', True, False],
         ['TensorFlow SavedModel', 'saved_model', '_saved_model', True, True],
         ['TensorFlow GraphDef', 'pb', '.pb', True, True],
         ['TensorFlow Lite', 'tflite', '.tflite', True, False],
-        ['TensorFlow Edge TPU', 'edgetpu', '_edgetpu.tflite', False, False],
-        ['TensorFlow.js', 'tfjs', '_web_model', False, False],
-        ['PaddlePaddle', 'paddle', '_paddle_model', True, True],]
-    return pd.DataFrame(x, columns=['Format', 'Argument', 'Suffix', 'CPU', 'GPU'])
+        ['TensorFlow Edge TPU', 'edgetpu', '_edgetpu.tflite', True, False],
+        ['TensorFlow.js', 'tfjs', '_web_model', True, False],
+        ['PaddlePaddle', 'paddle', '_paddle_model', True, True], ]
+    return pandas.DataFrame(x, columns=['Format', 'Argument', 'Suffix', 'CPU', 'GPU'])
+
+
+def gd_outputs(gd):
+    """TensorFlow GraphDef model output node names."""
+    name_list, input_list = [], []
+    for node in gd.node:  # tensorflow.core.framework.node_def_pb2.NodeDef
+        name_list.append(node.name)
+        input_list.extend(node.input)
+    return sorted(f'{x}:0' for x in list(set(name_list) - set(input_list)) if not x.startswith('NoOp'))
 
 
 def try_export(inner_func):
-    # YOLOv8 export decorator, i..e @try_export
+    """YOLOv8 export decorator, i..e @try_export."""
     inner_args = get_default_args(inner_func)
 
     def outer_func(*args, **kwargs):
+        """Export a model."""
         prefix = inner_args['prefix']
         try:
             with Profile() as dt:
                 f, model = inner_func(*args, **kwargs)
             LOGGER.info(f'{prefix} export success ✅ {dt.t:.1f}s, saved as {f} ({file_size(f):.1f} MB)')
             return f, model
         except Exception as e:
@@ -114,61 +117,62 @@
             return None, None
 
     return outer_func
 
 
 class Exporter:
     """
-    Exporter
-
     A class for exporting a model.
 
     Attributes:
-        args (OmegaConf): Configuration for the exporter.
+        args (SimpleNamespace): Configuration for the exporter.
         save_dir (Path): Directory to save results.
     """
 
-    def __init__(self, config=DEFAULT_CONFIG, overrides=None):
+    def __init__(self, cfg=DEFAULT_CFG, overrides=None, _callbacks=None):
         """
         Initializes the Exporter class.
 
         Args:
-            config (str, optional): Path to a configuration file. Defaults to DEFAULT_CONFIG.
+            cfg (str, optional): Path to a configuration file. Defaults to DEFAULT_CFG.
             overrides (dict, optional): Configuration overrides. Defaults to None.
+            _callbacks (list, optional): List of callback functions. Defaults to None.
         """
-        if overrides is None:
-            overrides = {}
-        self.args = get_config(config, overrides)
-        self.callbacks = defaultdict(list, {k: [v] for k, v in callbacks.default_callbacks.items()})  # add callbacks
+        self.args = get_cfg(cfg, overrides)
+        self.callbacks = _callbacks or callbacks.get_default_callbacks()
         callbacks.add_integration_callbacks(self)
 
     @smart_inference_mode()
     def __call__(self, model=None):
-        self.run_callbacks("on_export_start")
+        """Returns list of exported files/dirs after running callbacks."""
+        self.run_callbacks('on_export_start')
         t = time.time()
         format = self.args.format.lower()  # to lowercase
+        if format in ('tensorrt', 'trt'):  # engine aliases
+            format = 'engine'
         fmts = tuple(export_formats()['Argument'][1:])  # available export formats
         flags = [x == format for x in fmts]
-        assert sum(flags), f'ERROR: Invalid format={format}, valid formats are {fmts}'
+        if sum(flags) != 1:
+            raise ValueError(f"Invalid export format='{format}'. Valid formats are {fmts}")
         jit, onnx, xml, engine, coreml, saved_model, pb, tflite, edgetpu, tfjs, paddle = flags  # export booleans
 
         # Load PyTorch model
         self.device = select_device('cpu' if self.args.device is None else self.args.device)
-        if self.args.half:
-            if self.device.type == 'cpu' and not coreml:
-                LOGGER.info('half=True only compatible with GPU or CoreML export, i.e. use device=0 or format=coreml')
-                self.args.half = False
-            assert not self.args.dynamic, '--half not compatible with --dynamic, i.e. use either --half or --dynamic'
+        if self.args.half and onnx and self.device.type == 'cpu':
+            LOGGER.warning('WARNING ⚠️ half=True only compatible with GPU export, i.e. use device=0')
+            self.args.half = False
+            assert not self.args.dynamic, 'half=True not compatible with dynamic=True, i.e. use only one.'
 
         # Checks
-        # if self.args.batch == model.args['batch_size']:  # user has not modified training batch_size
-        self.args.batch = 1
+        model.names = check_class_names(model.names)
         self.imgsz = check_imgsz(self.args.imgsz, stride=model.stride, min_dim=2)  # check image size
         if self.args.optimize:
             assert self.device.type == 'cpu', '--optimize not compatible with cuda devices, i.e. use --device cpu'
+        if edgetpu and not LINUX:
+            raise SystemError('Edge TPU export only supported on Linux. See https://coral.ai/docs/edgetpu/compiler/')
 
         # Input
         im = torch.zeros(self.args.batch, 3, *self.imgsz).to(self.device)
         file = Path(getattr(model, 'pt_path', None) or getattr(model, 'yaml_file', None) or model.yaml['yaml_file'])
         if file.suffix == '.yaml':
             file = Path(file.name)
 
@@ -179,110 +183,126 @@
         model.eval()
         model.float()
         model = model.fuse()
         for k, m in model.named_modules():
             if isinstance(m, (Detect, Segment)):
                 m.dynamic = self.args.dynamic
                 m.export = True
+                m.format = self.args.format
+            elif isinstance(m, C2f) and not any((saved_model, pb, tflite, edgetpu, tfjs)):
+                # EdgeTPU does not support FlexSplitV while split provides cleaner ONNX graph
+                m.forward = m.forward_split
 
         y = None
         for _ in range(2):
             y = model(im)  # dry runs
-        if self.args.half and not coreml:
+        if self.args.half and (engine or onnx) and self.device.type != 'cpu':
             im, model = im.half(), model.half()  # to FP16
-        shape = tuple((y[0] if isinstance(y, tuple) else y).shape)  # model output shape
-        LOGGER.info(
-            f"\n{colorstr('PyTorch:')} starting from {file} with output shape {shape} ({file_size(file):.1f} MB)")
 
         # Warnings
         warnings.filterwarnings('ignore', category=torch.jit.TracerWarning)  # suppress TracerWarning
         warnings.filterwarnings('ignore', category=UserWarning)  # suppress shape prim::Constant missing ONNX warning
         warnings.filterwarnings('ignore', category=DeprecationWarning)  # suppress CoreML np.bool deprecation warning
 
         # Assign
         self.im = im
         self.model = model
         self.file = file
-        self.output_shape = tuple(y.shape) if isinstance(y, torch.Tensor) else (x.shape for x in y)
-        self.metadata = {'stride': int(max(model.stride)), 'names': model.names}  # model metadata
-        self.pretty_name = self.file.stem.replace('yolo', 'YOLO')
+        self.output_shape = tuple(y.shape) if isinstance(y, torch.Tensor) else tuple(tuple(x.shape) for x in y)
+        self.pretty_name = Path(self.model.yaml.get('yaml_file', self.file)).stem.replace('yolo', 'YOLO')
+        trained_on = f'trained on {Path(self.args.data).name}' if self.args.data else '(untrained)'
+        description = f'Ultralytics {self.pretty_name} model {trained_on}'
+        self.metadata = {
+            'description': description,
+            'author': 'Ultralytics',
+            'license': 'AGPL-3.0 https://ultralytics.com/license',
+            'version': __version__,
+            'stride': int(max(model.stride)),
+            'task': model.task,
+            'batch': self.args.batch,
+            'imgsz': self.imgsz,
+            'names': model.names}  # model metadata
+        if model.task == 'pose':
+            self.metadata['kpt_shape'] = model.kpt_shape
+
+        LOGGER.info(f"\n{colorstr('PyTorch:')} starting from {file} with input shape {tuple(im.shape)} BCHW and "
+                    f'output shape(s) {self.output_shape} ({file_size(file):.1f} MB)')
 
         # Exports
         f = [''] * len(fmts)  # exported filenames
         if jit:  # TorchScript
-            f[0], _ = self._export_torchscript()
+            f[0], _ = self.export_torchscript()
         if engine:  # TensorRT required before ONNX
-            f[1], _ = self._export_engine()
+            f[1], _ = self.export_engine()
         if onnx or xml:  # OpenVINO requires ONNX
-            f[2], _ = self._export_onnx()
+            f[2], _ = self.export_onnx()
         if xml:  # OpenVINO
-            f[3], _ = self._export_openvino()
+            f[3], _ = self.export_openvino()
         if coreml:  # CoreML
-            f[4], _ = self._export_coreml()
+            f[4], _ = self.export_coreml()
         if any((saved_model, pb, tflite, edgetpu, tfjs)):  # TensorFlow formats
-            raise NotImplementedError('YOLOv8 TensorFlow export support is still under development. '
-                                      'Please consider contributing to the effort if you have TF expertise. Thank you!')
-            assert not isinstance(model, ClassificationModel), 'ClassificationModel TF exports not yet supported.'
-            nms = False
-            f[5], s_model = self._export_saved_model(nms=nms or self.args.agnostic_nms or tfjs,
-                                                     agnostic_nms=self.args.agnostic_nms or tfjs)
+            self.args.int8 |= edgetpu
+            f[5], s_model = self.export_saved_model()
             if pb or tfjs:  # pb prerequisite to tfjs
-                f[6], _ = self._export_pb(s_model)
-            if tflite or edgetpu:
-                f[7], _ = self._export_tflite(s_model,
-                                              int8=self.args.int8 or edgetpu,
-                                              data=self.args.data,
-                                              nms=nms,
-                                              agnostic_nms=self.args.agnostic_nms)
-                if edgetpu:
-                    f[8], _ = self._export_edgetpu()
-                self._add_tflite_metadata(f[8] or f[7], num_outputs=len(s_model.outputs))
+                f[6], _ = self.export_pb(s_model)
+            if tflite:
+                f[7], _ = self.export_tflite(s_model, nms=False, agnostic_nms=self.args.agnostic_nms)
+            if edgetpu:
+                f[8], _ = self.export_edgetpu(tflite_model=Path(f[5]) / f'{self.file.stem}_full_integer_quant.tflite')
             if tfjs:
-                f[9], _ = self._export_tfjs()
+                f[9], _ = self.export_tfjs()
         if paddle:  # PaddlePaddle
-            f[10], _ = self._export_paddle()
+            f[10], _ = self.export_paddle()
 
         # Finish
         f = [str(x) for x in f if x]  # filter out '' and None
         if any(f):
-            task = guess_task_from_head(model.yaml["head"][-1][-2])
-            s = "-WARNING ⚠️ not yet supported for YOLOv8 exported models"
-            LOGGER.info(f'\nExport complete ({time.time() - t:.1f}s)'
-                        f"\nResults saved to {colorstr('bold', file.parent.resolve())}"
-                        f"\nPredict:         yolo task={task} mode=predict model={f[-1]} {s}"
-                        f"\nValidate:        yolo task={task} mode=val model={f[-1]} {s}"
-                        f"\nVisualize:       https://netron.app")
+            f = str(Path(f[-1]))
+            square = self.imgsz[0] == self.imgsz[1]
+            s = '' if square else f"WARNING ⚠️ non-PyTorch val requires square images, 'imgsz={self.imgsz}' will not " \
+                                  f"work. Use export 'imgsz={max(self.imgsz)}' if val is required."
+            imgsz = self.imgsz[0] if square else str(self.imgsz)[1:-1].replace(' ', '')
+            data = f'data={self.args.data}' if model.task == 'segment' and format == 'pb' else ''
+            LOGGER.info(
+                f'\nExport complete ({time.time() - t:.1f}s)'
+                f"\nResults saved to {colorstr('bold', file.parent.resolve())}"
+                f'\nPredict:         yolo predict task={model.task} model={f} imgsz={imgsz} {data}'
+                f'\nValidate:        yolo val task={model.task} model={f} imgsz={imgsz} data={self.args.data} {s}'
+                f'\nVisualize:       https://netron.app')
 
-        self.run_callbacks("on_export_end")
+        self.run_callbacks('on_export_end')
         return f  # return list of exported files/dirs
 
     @try_export
-    def _export_torchscript(self, prefix=colorstr('TorchScript:')):
-        # YOLOv8 TorchScript model export
+    def export_torchscript(self, prefix=colorstr('TorchScript:')):
+        """YOLOv8 TorchScript model export."""
         LOGGER.info(f'\n{prefix} starting export with torch {torch.__version__}...')
         f = self.file.with_suffix('.torchscript')
 
         ts = torch.jit.trace(self.model, self.im, strict=False)
-        d = {"shape": self.im.shape, "stride": int(max(self.model.stride)), "names": self.model.names}
-        extra_files = {'config.txt': json.dumps(d)}  # torch._C.ExtraFilesMap()
+        extra_files = {'config.txt': json.dumps(self.metadata)}  # torch._C.ExtraFilesMap()
         if self.args.optimize:  # https://pytorch.org/tutorials/recipes/mobile_interpreter.html
             LOGGER.info(f'{prefix} optimizing for mobile...')
             from torch.utils.mobile_optimizer import optimize_for_mobile
             optimize_for_mobile(ts)._save_for_lite_interpreter(str(f), _extra_files=extra_files)
         else:
             ts.save(str(f), _extra_files=extra_files)
         return f, None
 
     @try_export
-    def _export_onnx(self, prefix=colorstr('ONNX:')):
-        # YOLOv8 ONNX export
-        check_requirements('onnx>=1.12.0')
+    def export_onnx(self, prefix=colorstr('ONNX:')):
+        """YOLOv8 ONNX export."""
+        requirements = ['onnx>=1.12.0']
+        if self.args.simplify:
+            requirements += ['onnxsim>=0.4.17', 'onnxruntime-gpu' if torch.cuda.is_available() else 'onnxruntime']
+        check_requirements(requirements)
         import onnx  # noqa
 
-        LOGGER.info(f'\n{prefix} starting export with onnx {onnx.__version__}...')
+        opset_version = self.args.opset or get_latest_opset()
+        LOGGER.info(f'\n{prefix} starting export with onnx {onnx.__version__} opset {opset_version}...')
         f = str(self.file.with_suffix('.onnx'))
 
         output_names = ['output0', 'output1'] if isinstance(self.model, SegmentationModel) else ['output0']
         dynamic = self.args.dynamic
         if dynamic:
             dynamic = {'images': {0: 'batch', 2: 'height', 3: 'width'}}  # shape(1,3,640,640)
             if isinstance(self.model, SegmentationModel):
@@ -292,393 +312,386 @@
                 dynamic['output0'] = {0: 'batch', 1: 'anchors'}  # shape(1,25200,85)
 
         torch.onnx.export(
             self.model.cpu() if dynamic else self.model,  # --dynamic only compatible with cpu
             self.im.cpu() if dynamic else self.im,
             f,
             verbose=False,
-            opset_version=self.args.opset,
+            opset_version=opset_version,
             do_constant_folding=True,  # WARNING: DNN inference with torch>=1.12 may require do_constant_folding=False
             input_names=['images'],
             output_names=output_names,
             dynamic_axes=dynamic or None)
 
         # Checks
         model_onnx = onnx.load(f)  # load onnx model
-        onnx.checker.check_model(model_onnx)  # check onnx model
-
-        # Metadata
-        d = {'stride': int(max(self.model.stride)), 'names': self.model.names}
-        for k, v in d.items():
-            meta = model_onnx.metadata_props.add()
-            meta.key, meta.value = k, str(v)
-        onnx.save(model_onnx, f)
+        # onnx.checker.check_model(model_onnx)  # check onnx model
 
         # Simplify
         if self.args.simplify:
             try:
-                check_requirements('onnxsim')
                 import onnxsim
 
-                LOGGER.info(f'{prefix} simplifying with onnx-simplifier {onnxsim.__version__}...')
-                subprocess.run(f'onnxsim {f} {f}', shell=True)
+                LOGGER.info(f'{prefix} simplifying with onnxsim {onnxsim.__version__}...')
+                # subprocess.run(f'onnxsim {f} {f}', shell=True)
+                model_onnx, check = onnxsim.simplify(model_onnx)
+                assert check, 'Simplified ONNX model could not be validated'
             except Exception as e:
                 LOGGER.info(f'{prefix} simplifier failure: {e}')
+
+        # Metadata
+        for k, v in self.metadata.items():
+            meta = model_onnx.metadata_props.add()
+            meta.key, meta.value = k, str(v)
+
+        onnx.save(model_onnx, f)
         return f, model_onnx
 
     @try_export
-    def _export_openvino(self, prefix=colorstr('OpenVINO:')):
-        # YOLOv8 OpenVINO export
-        check_requirements('openvino-dev')  # requires openvino-dev: https://pypi.org/project/openvino-dev/
-        import openvino.inference_engine as ie  # noqa
+    def export_openvino(self, prefix=colorstr('OpenVINO:')):
+        """YOLOv8 OpenVINO export."""
+        check_requirements('openvino-dev>=2022.3')  # requires openvino-dev: https://pypi.org/project/openvino-dev/
+        import openvino.runtime as ov  # noqa
+        from openvino.tools import mo  # noqa
 
-        LOGGER.info(f'\n{prefix} starting export with openvino {ie.__version__}...')
+        LOGGER.info(f'\n{prefix} starting export with openvino {ov.__version__}...')
         f = str(self.file).replace(self.file.suffix, f'_openvino_model{os.sep}')
         f_onnx = self.file.with_suffix('.onnx')
+        f_ov = str(Path(f) / self.file.with_suffix('.xml').name)
 
-        cmd = f"mo --input_model {f_onnx} --output_dir {f} --data_type {'FP16' if self.args.half else 'FP32'}"
-        subprocess.run(cmd.split(), check=True, env=os.environ)  # export
-        yaml_save(Path(f) / self.file.with_suffix('.yaml').name, self.metadata)  # add metadata.yaml
+        ov_model = mo.convert_model(f_onnx,
+                                    model_name=self.pretty_name,
+                                    framework='onnx',
+                                    compress_to_fp16=self.args.half)  # export
+        ov.serialize(ov_model, f_ov)  # save
+        yaml_save(Path(f) / 'metadata.yaml', self.metadata)  # add metadata.yaml
         return f, None
 
     @try_export
-    def _export_paddle(self, prefix=colorstr('PaddlePaddle:')):
-        # YOLOv8 Paddle export
+    def export_paddle(self, prefix=colorstr('PaddlePaddle:')):
+        """YOLOv8 Paddle export."""
         check_requirements(('paddlepaddle', 'x2paddle'))
         import x2paddle  # noqa
         from x2paddle.convert import pytorch2paddle  # noqa
 
         LOGGER.info(f'\n{prefix} starting export with X2Paddle {x2paddle.__version__}...')
         f = str(self.file).replace(self.file.suffix, f'_paddle_model{os.sep}')
 
         pytorch2paddle(module=self.model, save_dir=f, jit_type='trace', input_examples=[self.im])  # export
-        yaml_save(Path(f) / self.file.with_suffix('.yaml').name, self.metadata)  # add metadata.yaml
+        yaml_save(Path(f) / 'metadata.yaml', self.metadata)  # add metadata.yaml
         return f, None
 
     @try_export
-    def _export_coreml(self, prefix=colorstr('CoreML:')):
-        # YOLOv8 CoreML export
+    def export_coreml(self, prefix=colorstr('CoreML:')):
+        """YOLOv8 CoreML export."""
         check_requirements('coremltools>=6.0')
         import coremltools as ct  # noqa
 
-        class iOSModel(torch.nn.Module):
-            # Wrap an Ultralytics YOLO model for iOS export
-            def __init__(self, model, im):
-                super().__init__()
-                b, c, h, w = im.shape  # batch, channel, height, width
-                self.model = model
-                self.nc = len(model.names)  # number of classes
-                if w == h:
-                    self.normalize = 1.0 / w  # scalar
-                else:
-                    self.normalize = torch.tensor([1.0 / w, 1.0 / h, 1.0 / w, 1.0 / h])  # broadcast (slower, smaller)
-
-            def forward(self, x):
-                xywh, cls = self.model(x)[0].transpose(0, 1).split((4, self.nc), 1)
-                return cls, xywh * self.normalize  # confidence (3780, 80), coordinates (3780, 4)
-
         LOGGER.info(f'\n{prefix} starting export with coremltools {ct.__version__}...')
         f = self.file.with_suffix('.mlmodel')
 
-        model = iOSModel(self.model, self.im).eval() if self.args.nms else self.model
-        ts = torch.jit.trace(model, self.im, strict=False)  # TorchScript model
-        ct_model = ct.convert(ts, inputs=[ct.ImageType('image', shape=self.im.shape, scale=1 / 255, bias=[0, 0, 0])])
+        bias = [0.0, 0.0, 0.0]
+        scale = 1 / 255
+        classifier_config = None
+        if self.model.task == 'classify':
+            classifier_config = ct.ClassifierConfig(list(self.model.names.values())) if self.args.nms else None
+            model = self.model
+        elif self.model.task == 'detect':
+            model = iOSDetectModel(self.model, self.im) if self.args.nms else self.model
+        else:
+            # TODO CoreML Segment and Pose model pipelining
+            model = self.model
+
+        ts = torch.jit.trace(model.eval(), self.im, strict=False)  # TorchScript model
+        ct_model = ct.convert(ts,
+                              inputs=[ct.ImageType('image', shape=self.im.shape, scale=scale, bias=bias)],
+                              classifier_config=classifier_config)
         bits, mode = (8, 'kmeans_lut') if self.args.int8 else (16, 'linear') if self.args.half else (32, None)
         if bits < 32:
-            if MACOS:  # quantization only supported on macOS
-                ct_model = ct.models.neural_network.quantization_utils.quantize_weights(ct_model, bits, mode)
-            else:
-                LOGGER.info(f'{prefix} quantization only supported on macOS, skipping...')
-        if self.args.nms:
+            if 'kmeans' in mode:
+                check_requirements('scikit-learn')  # scikit-learn package required for k-means quantization
+            ct_model = ct.models.neural_network.quantization_utils.quantize_weights(ct_model, bits, mode)
+        if self.args.nms and self.model.task == 'detect':
             ct_model = self._pipeline_coreml(ct_model)
 
+        m = self.metadata  # metadata dict
+        ct_model.short_description = m.pop('description')
+        ct_model.author = m.pop('author')
+        ct_model.license = m.pop('license')
+        ct_model.version = m.pop('version')
+        ct_model.user_defined_metadata.update({k: str(v) for k, v in m.items()})
         ct_model.save(str(f))
         return f, ct_model
 
     @try_export
-    def _export_engine(self, workspace=4, verbose=False, prefix=colorstr('TensorRT:')):
-        # YOLOv8 TensorRT export https://developer.nvidia.com/tensorrt
-        assert self.im.device.type != 'cpu', 'export running on CPU but must be on GPU, i.e. `device==0`'
+    def export_engine(self, workspace=4, verbose=False, prefix=colorstr('TensorRT:')):
+        """YOLOv8 TensorRT export https://developer.nvidia.com/tensorrt."""
+        assert self.im.device.type != 'cpu', "export running on CPU but must be on GPU, i.e. use 'device=0'"
         try:
             import tensorrt as trt  # noqa
         except ImportError:
-            if platform.system() == 'Linux':
+            if LINUX:
                 check_requirements('nvidia-tensorrt', cmds='-U --index-url https://pypi.ngc.nvidia.com')
             import tensorrt as trt  # noqa
 
         check_version(trt.__version__, '7.0.0', hard=True)  # require tensorrt>=8.0.0
-        self._export_onnx()
-        onnx = self.file.with_suffix('.onnx')
+        self.args.simplify = True
+        f_onnx, _ = self.export_onnx()
 
         LOGGER.info(f'\n{prefix} starting export with TensorRT {trt.__version__}...')
-        assert onnx.exists(), f'failed to export ONNX file: {onnx}'
+        assert Path(f_onnx).exists(), f'failed to export ONNX file: {f_onnx}'
         f = self.file.with_suffix('.engine')  # TensorRT engine file
         logger = trt.Logger(trt.Logger.INFO)
         if verbose:
             logger.min_severity = trt.Logger.Severity.VERBOSE
 
         builder = trt.Builder(logger)
         config = builder.create_builder_config()
         config.max_workspace_size = workspace * 1 << 30
         # config.set_memory_pool_limit(trt.MemoryPoolType.WORKSPACE, workspace << 30)  # fix TRT 8.4 deprecation notice
 
         flag = (1 << int(trt.NetworkDefinitionCreationFlag.EXPLICIT_BATCH))
         network = builder.create_network(flag)
         parser = trt.OnnxParser(network, logger)
-        if not parser.parse_from_file(str(onnx)):
-            raise RuntimeError(f'failed to load ONNX file: {onnx}')
+        if not parser.parse_from_file(f_onnx):
+            raise RuntimeError(f'failed to load ONNX file: {f_onnx}')
 
         inputs = [network.get_input(i) for i in range(network.num_inputs)]
         outputs = [network.get_output(i) for i in range(network.num_outputs)]
         for inp in inputs:
             LOGGER.info(f'{prefix} input "{inp.name}" with shape{inp.shape} {inp.dtype}')
         for out in outputs:
             LOGGER.info(f'{prefix} output "{out.name}" with shape{out.shape} {out.dtype}')
 
         if self.args.dynamic:
             shape = self.im.shape
             if shape[0] <= 1:
-                LOGGER.warning(f"{prefix} WARNING ⚠️ --dynamic model requires maximum --batch-size argument")
+                LOGGER.warning(f'{prefix} WARNING ⚠️ --dynamic model requires maximum --batch-size argument')
             profile = builder.create_optimization_profile()
             for inp in inputs:
                 profile.set_shape(inp.name, (1, *shape[1:]), (max(1, shape[0] // 2), *shape[1:]), shape)
             config.add_optimization_profile(profile)
 
         LOGGER.info(
             f'{prefix} building FP{16 if builder.platform_has_fast_fp16 and self.args.half else 32} engine as {f}')
         if builder.platform_has_fast_fp16 and self.args.half:
             config.set_flag(trt.BuilderFlag.FP16)
+
+        # Write file
         with builder.build_engine(network, config) as engine, open(f, 'wb') as t:
+            # Metadata
+            meta = json.dumps(self.metadata)
+            t.write(len(meta).to_bytes(4, byteorder='little', signed=True))
+            t.write(meta.encode())
+            # Model
             t.write(engine.serialize())
+
         return f, None
 
     @try_export
-    def _export_saved_model(self,
-                            nms=False,
-                            agnostic_nms=False,
-                            topk_per_class=100,
-                            topk_all=100,
-                            iou_thres=0.45,
-                            conf_thres=0.25,
-                            prefix=colorstr('TensorFlow SavedModel:')):
-
-        # YOLOv8 TensorFlow SavedModel export
+    def export_saved_model(self, prefix=colorstr('TensorFlow SavedModel:')):
+        """YOLOv8 TensorFlow SavedModel export."""
         try:
             import tensorflow as tf  # noqa
         except ImportError:
-            check_requirements(f"tensorflow{'' if torch.cuda.is_available() else '-macos' if MACOS else '-cpu'}")
+            cuda = torch.cuda.is_available()
+            check_requirements(f"tensorflow{'-macos' if MACOS else '-aarch64' if ARM64 else '' if cuda else '-cpu'}")
             import tensorflow as tf  # noqa
-        check_requirements(("onnx", "onnx2tf", "sng4onnx", "onnxsim", "onnx_graphsurgeon"),
-                           cmds="--extra-index-url https://pypi.ngc.nvidia.com ")
+        check_requirements(('onnx', 'onnx2tf>=1.7.7', 'sng4onnx>=1.0.1', 'onnxsim>=0.4.17', 'onnx_graphsurgeon>=0.3.26',
+                            'tflite_support', 'onnxruntime-gpu' if torch.cuda.is_available() else 'onnxruntime'),
+                           cmds='--extra-index-url https://pypi.ngc.nvidia.com')
 
         LOGGER.info(f'\n{prefix} starting export with tensorflow {tf.__version__}...')
-        f = str(self.file).replace(self.file.suffix, '_saved_model')
+        f = Path(str(self.file).replace(self.file.suffix, '_saved_model'))
+        if f.is_dir():
+            import shutil
+            shutil.rmtree(f)  # delete output folder
 
         # Export to ONNX
-        self._export_onnx()
-        onnx = self.file.with_suffix('.onnx')
+        self.args.simplify = True
+        f_onnx, _ = self.export_onnx()
 
-        # Export to TF SavedModel
-        subprocess.run(f'onnx2tf -i {onnx} --output_signaturedefs -o {f}', shell=True)
+        # Export to TF
+        int8 = '-oiqt -qt per-tensor' if self.args.int8 else ''
+        cmd = f'onnx2tf -i {f_onnx} -o {f} -nuo --non_verbose {int8}'
+        LOGGER.info(f"\n{prefix} running '{cmd.strip()}'")
+        subprocess.run(cmd, shell=True)
+        yaml_save(f / 'metadata.yaml', self.metadata)  # add metadata.yaml
+
+        # Remove/rename TFLite models
+        if self.args.int8:
+            for file in f.rglob('*_dynamic_range_quant.tflite'):
+                file.rename(file.with_stem(file.stem.replace('_dynamic_range_quant', '_int8')))
+            for file in f.rglob('*_integer_quant_with_int16_act.tflite'):
+                file.unlink()  # delete extra fp16 activation TFLite files
+
+        # Add TFLite metadata
+        for file in f.rglob('*.tflite'):
+            f.unlink() if 'quant_with_int16_act.tflite' in str(f) else self._add_tflite_metadata(file)
 
         # Load saved_model
         keras_model = tf.saved_model.load(f, tags=None, options=None)
 
-        return f, keras_model
+        return str(f), keras_model
 
     @try_export
-    def _export_saved_model_OLD(self,
-                                nms=False,
-                                agnostic_nms=False,
-                                topk_per_class=100,
-                                topk_all=100,
-                                iou_thres=0.45,
-                                conf_thres=0.25,
-                                prefix=colorstr('TensorFlow SavedModel:')):
-        # YOLOv8 TensorFlow SavedModel export
-        try:
-            import tensorflow as tf  # noqa
-        except ImportError:
-            check_requirements(f"tensorflow{'' if torch.cuda.is_available() else '-macos' if MACOS else '-cpu'}")
-            import tensorflow as tf  # noqa
-        # from models.tf import TFModel
-        from tensorflow.python.framework.convert_to_constants import convert_variables_to_constants_v2  # noqa
-
-        LOGGER.info(f'\n{prefix} starting export with tensorflow {tf.__version__}...')
-        f = str(self.file).replace(self.file.suffix, '_saved_model')
-        batch_size, ch, *imgsz = list(self.im.shape)  # BCHW
-
-        tf_models = None  # TODO: no TF modules available
-        tf_model = tf_models.TFModel(cfg=self.model.yaml, model=self.model.cpu(), nc=self.model.nc, imgsz=imgsz)
-        im = tf.zeros((batch_size, *imgsz, ch))  # BHWC order for TensorFlow
-        _ = tf_model.predict(im, nms, agnostic_nms, topk_per_class, topk_all, iou_thres, conf_thres)
-        inputs = tf.keras.Input(shape=(*imgsz, ch), batch_size=None if self.args.dynamic else batch_size)
-        outputs = tf_model.predict(inputs, nms, agnostic_nms, topk_per_class, topk_all, iou_thres, conf_thres)
-        keras_model = tf.keras.Model(inputs=inputs, outputs=outputs)
-        keras_model.trainable = False
-        keras_model.summary()
-        if self.args.keras:
-            keras_model.save(f, save_format='tf')
-        else:
-            spec = tf.TensorSpec(keras_model.inputs[0].shape, keras_model.inputs[0].dtype)
-            m = tf.function(lambda x: keras_model(x))  # full model
-            m = m.get_concrete_function(spec)
-            frozen_func = convert_variables_to_constants_v2(m)
-            tfm = tf.Module()
-            tfm.__call__ = tf.function(lambda x: frozen_func(x)[:4] if nms else frozen_func(x), [spec])
-            tfm.__call__(im)
-            tf.saved_model.save(tfm,
-                                f,
-                                options=tf.saved_model.SaveOptions(experimental_custom_gradients=False)
-                                if check_version(tf.__version__, '2.6') else tf.saved_model.SaveOptions())
-        return f, keras_model
-
-    @try_export
-    def _export_pb(self, keras_model, file, prefix=colorstr('TensorFlow GraphDef:')):
-        # YOLOv8 TensorFlow GraphDef *.pb export https://github.com/leimao/Frozen_Graph_TensorFlow
+    def export_pb(self, keras_model, prefix=colorstr('TensorFlow GraphDef:')):
+        """YOLOv8 TensorFlow GraphDef *.pb export https://github.com/leimao/Frozen_Graph_TensorFlow."""
         import tensorflow as tf  # noqa
         from tensorflow.python.framework.convert_to_constants import convert_variables_to_constants_v2  # noqa
 
         LOGGER.info(f'\n{prefix} starting export with tensorflow {tf.__version__}...')
-        f = file.with_suffix('.pb')
+        f = self.file.with_suffix('.pb')
 
         m = tf.function(lambda x: keras_model(x))  # full model
         m = m.get_concrete_function(tf.TensorSpec(keras_model.inputs[0].shape, keras_model.inputs[0].dtype))
         frozen_func = convert_variables_to_constants_v2(m)
         frozen_func.graph.as_graph_def()
         tf.io.write_graph(graph_or_graph_def=frozen_func.graph, logdir=str(f.parent), name=f.name, as_text=False)
         return f, None
 
     @try_export
-    def _export_tflite(self, keras_model, int8, data, nms, agnostic_nms, prefix=colorstr('TensorFlow Lite:')):
-        # YOLOv8 TensorFlow Lite export
+    def export_tflite(self, keras_model, nms, agnostic_nms, prefix=colorstr('TensorFlow Lite:')):
+        """YOLOv8 TensorFlow Lite export."""
         import tensorflow as tf  # noqa
 
         LOGGER.info(f'\n{prefix} starting export with tensorflow {tf.__version__}...')
-        batch_size, ch, *imgsz = list(self.im.shape)  # BCHW
-        f = str(self.file).replace(self.file.suffix, '-fp16.tflite')
-
-        converter = tf.lite.TFLiteConverter.from_keras_model(keras_model)
-        converter.target_spec.supported_ops = [tf.lite.OpsSet.TFLITE_BUILTINS]
-        converter.target_spec.supported_types = [tf.float16]
-        converter.optimizations = [tf.lite.Optimize.DEFAULT]
-        if int8:
-
-            def representative_dataset_gen(dataset, n_images=100):
-                # Dataset generator for use with converter.representative_dataset, returns a generator of np arrays
-                for n, (path, img, im0s, vid_cap, string) in enumerate(dataset):
-                    im = np.transpose(img, [1, 2, 0])
-                    im = np.expand_dims(im, axis=0).astype(np.float32)
-                    im /= 255
-                    yield [im]
-                    if n >= n_images:
-                        break
-
-            dataset = LoadImages(check_dataset(check_yaml(data))['train'], imgsz=imgsz, auto=False)
-            converter.representative_dataset = lambda: representative_dataset_gen(dataset, n_images=100)
-            converter.target_spec.supported_ops = [tf.lite.OpsSet.TFLITE_BUILTINS_INT8]
-            converter.target_spec.supported_types = []
-            converter.inference_input_type = tf.uint8  # or tf.int8
-            converter.inference_output_type = tf.uint8  # or tf.int8
-            converter.experimental_new_quantizer = True
-            f = str(self.file).replace(self.file.suffix, '-int8.tflite')
-        if nms or agnostic_nms:
-            converter.target_spec.supported_ops.append(tf.lite.OpsSet.SELECT_TF_OPS)
-
-        tflite_model = converter.convert()
-        open(f, "wb").write(tflite_model)
-        return f, None
+        saved_model = Path(str(self.file).replace(self.file.suffix, '_saved_model'))
+        if self.args.int8:
+            f = saved_model / f'{self.file.stem}_int8.tflite'  # fp32 in/out
+        elif self.args.half:
+            f = saved_model / f'{self.file.stem}_float16.tflite'  # fp32 in/out
+        else:
+            f = saved_model / f'{self.file.stem}_float32.tflite'
+        return str(f), None
 
     @try_export
-    def _export_edgetpu(self, prefix=colorstr('Edge TPU:')):
-        # YOLOv8 Edge TPU export https://coral.ai/docs/edgetpu/models-intro/
+    def export_edgetpu(self, tflite_model='', prefix=colorstr('Edge TPU:')):
+        """YOLOv8 Edge TPU export https://coral.ai/docs/edgetpu/models-intro/."""
+        LOGGER.warning(f'{prefix} WARNING ⚠️ Edge TPU known bug https://github.com/ultralytics/ultralytics/issues/1185')
+
         cmd = 'edgetpu_compiler --version'
         help_url = 'https://coral.ai/docs/edgetpu/compiler/'
-        assert platform.system() == 'Linux', f'export only supported on Linux. See {help_url}'
-        if subprocess.run(f'{cmd} >/dev/null', shell=True).returncode != 0:
+        assert LINUX, f'export only supported on Linux. See {help_url}'
+        if subprocess.run(cmd, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL, shell=True).returncode != 0:
             LOGGER.info(f'\n{prefix} export requires Edge TPU compiler. Attempting install from {help_url}')
             sudo = subprocess.run('sudo --version >/dev/null', shell=True).returncode == 0  # sudo installed on system
             for c in (
                     'curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -',
-                    'echo "deb https://packages.cloud.google.com/apt coral-edgetpu-stable main" | '  # no comma
-                    'sudo tee /etc/apt/sources.list.d/coral-edgetpu.list',
-                    'sudo apt-get update',
-                    'sudo apt-get install edgetpu-compiler'):
+                    'echo "deb https://packages.cloud.google.com/apt coral-edgetpu-stable main" | sudo tee /etc/apt/sources.list.d/coral-edgetpu.list',
+                    'sudo apt-get update', 'sudo apt-get install edgetpu-compiler'):
                 subprocess.run(c if sudo else c.replace('sudo ', ''), shell=True, check=True)
         ver = subprocess.run(cmd, shell=True, capture_output=True, check=True).stdout.decode().split()[-1]
 
         LOGGER.info(f'\n{prefix} starting export with Edge TPU compiler {ver}...')
-        f = str(self.file).replace(self.file.suffix, '-int8_edgetpu.tflite')  # Edge TPU model
-        f_tfl = str(self.file).replace(self.file.suffix, '-int8.tflite')  # TFLite model
+        f = str(tflite_model).replace('.tflite', '_edgetpu.tflite')  # Edge TPU model
 
-        cmd = f"edgetpu_compiler -s -d -k 10 --out_dir {self.file.parent} {f_tfl}"
+        cmd = f'edgetpu_compiler -s -d -k 10 --out_dir {Path(f).parent} {tflite_model}'
+        LOGGER.info(f"{prefix} running '{cmd}'")
         subprocess.run(cmd.split(), check=True)
+        self._add_tflite_metadata(f)
         return f, None
 
     @try_export
-    def _export_tfjs(self, prefix=colorstr('TensorFlow.js:')):
-        # YOLOv8 TensorFlow.js export
+    def export_tfjs(self, prefix=colorstr('TensorFlow.js:')):
+        """YOLOv8 TensorFlow.js export."""
         check_requirements('tensorflowjs')
+        import tensorflow as tf
         import tensorflowjs as tfjs  # noqa
 
         LOGGER.info(f'\n{prefix} starting export with tensorflowjs {tfjs.__version__}...')
         f = str(self.file).replace(self.file.suffix, '_web_model')  # js dir
         f_pb = self.file.with_suffix('.pb')  # *.pb path
-        f_json = Path(f) / 'model.json'  # *.json path
 
-        cmd = f'tensorflowjs_converter --input_format=tf_frozen_model ' \
-              f'--output_node_names=Identity,Identity_1,Identity_2,Identity_3 {f_pb} {f}'
-        subprocess.run(cmd.split())
-
-        with open(f_json, 'w') as j:  # sort JSON Identity_* in ascending order
-            subst = re.sub(
-                r'{"outputs": {"Identity.?.?": {"name": "Identity.?.?"}, '
-                r'"Identity.?.?": {"name": "Identity.?.?"}, '
-                r'"Identity.?.?": {"name": "Identity.?.?"}, '
-                r'"Identity.?.?": {"name": "Identity.?.?"}}}', r'{"outputs": {"Identity": {"name": "Identity"}, '
-                r'"Identity_1": {"name": "Identity_1"}, '
-                r'"Identity_2": {"name": "Identity_2"}, '
-                r'"Identity_3": {"name": "Identity_3"}}}', f_json.read_text())
-            j.write(subst)
+        gd = tf.Graph().as_graph_def()  # TF GraphDef
+        with open(f_pb, 'rb') as file:
+            gd.ParseFromString(file.read())
+        outputs = ','.join(gd_outputs(gd))
+        LOGGER.info(f'\n{prefix} output node names: {outputs}')
+
+        cmd = f'tensorflowjs_converter --input_format=tf_frozen_model --output_node_names={outputs} {f_pb} {f}'
+        subprocess.run(cmd.split(), check=True)
+
+        # f_json = Path(f) / 'model.json'  # *.json path
+        # with open(f_json, 'w') as j:  # sort JSON Identity_* in ascending order
+        #     subst = re.sub(
+        #         r'{"outputs": {"Identity.?.?": {"name": "Identity.?.?"}, '
+        #         r'"Identity.?.?": {"name": "Identity.?.?"}, '
+        #         r'"Identity.?.?": {"name": "Identity.?.?"}, '
+        #         r'"Identity.?.?": {"name": "Identity.?.?"}}}',
+        #         r'{"outputs": {"Identity": {"name": "Identity"}, '
+        #         r'"Identity_1": {"name": "Identity_1"}, '
+        #         r'"Identity_2": {"name": "Identity_2"}, '
+        #         r'"Identity_3": {"name": "Identity_3"}}}',
+        #         f_json.read_text(),
+        #     )
+        #     j.write(subst)
+        yaml_save(Path(f) / 'metadata.yaml', self.metadata)  # add metadata.yaml
         return f, None
 
-    def _add_tflite_metadata(self, file, num_outputs):
-        # Add metadata to *.tflite models per https://www.tensorflow.org/lite/models/convert/metadata
-        with contextlib.suppress(ImportError):
-            # check_requirements('tflite_support')
-            from tflite_support import flatbuffers  # noqa
-            from tflite_support import metadata as _metadata  # noqa
-            from tflite_support import metadata_schema_py_generated as _metadata_fb  # noqa
-
-            tmp_file = Path('/tmp/meta.txt')
-            with open(tmp_file, 'w') as meta_f:
-                meta_f.write(str(self.metadata))
-
-            model_meta = _metadata_fb.ModelMetadataT()
-            label_file = _metadata_fb.AssociatedFileT()
-            label_file.name = tmp_file.name
-            model_meta.associatedFiles = [label_file]
-
-            subgraph = _metadata_fb.SubGraphMetadataT()
-            subgraph.inputTensorMetadata = [_metadata_fb.TensorMetadataT()]
-            subgraph.outputTensorMetadata = [_metadata_fb.TensorMetadataT()] * num_outputs
-            model_meta.subgraphMetadata = [subgraph]
-
-            b = flatbuffers.Builder(0)
-            b.Finish(model_meta.Pack(b), _metadata.MetadataPopulator.METADATA_FILE_IDENTIFIER)
-            metadata_buf = b.Output()
-
-            populator = _metadata.MetadataPopulator.with_model_file(file)
-            populator.load_metadata_buffer(metadata_buf)
-            populator.load_associated_files([str(tmp_file)])
-            populator.populate()
-            tmp_file.unlink()
+    def _add_tflite_metadata(self, file):
+        """Add metadata to *.tflite models per https://www.tensorflow.org/lite/models/convert/metadata."""
+        from tflite_support import flatbuffers  # noqa
+        from tflite_support import metadata as _metadata  # noqa
+        from tflite_support import metadata_schema_py_generated as _metadata_fb  # noqa
+
+        # Create model info
+        model_meta = _metadata_fb.ModelMetadataT()
+        model_meta.name = self.metadata['description']
+        model_meta.version = self.metadata['version']
+        model_meta.author = self.metadata['author']
+        model_meta.license = self.metadata['license']
+
+        # Label file
+        tmp_file = Path(file).parent / 'temp_meta.txt'
+        with open(tmp_file, 'w') as f:
+            f.write(str(self.metadata))
+
+        label_file = _metadata_fb.AssociatedFileT()
+        label_file.name = tmp_file.name
+        label_file.type = _metadata_fb.AssociatedFileType.TENSOR_AXIS_LABELS
+
+        # Create input info
+        input_meta = _metadata_fb.TensorMetadataT()
+        input_meta.name = 'image'
+        input_meta.description = 'Input image to be detected.'
+        input_meta.content = _metadata_fb.ContentT()
+        input_meta.content.contentProperties = _metadata_fb.ImagePropertiesT()
+        input_meta.content.contentProperties.colorSpace = _metadata_fb.ColorSpaceType.RGB
+        input_meta.content.contentPropertiesType = _metadata_fb.ContentProperties.ImageProperties
+
+        # Create output info
+        output1 = _metadata_fb.TensorMetadataT()
+        output1.name = 'output'
+        output1.description = 'Coordinates of detected objects, class labels, and confidence score'
+        output1.associatedFiles = [label_file]
+        if self.model.task == 'segment':
+            output2 = _metadata_fb.TensorMetadataT()
+            output2.name = 'output'
+            output2.description = 'Mask protos'
+            output2.associatedFiles = [label_file]
+
+        # Create subgraph info
+        subgraph = _metadata_fb.SubGraphMetadataT()
+        subgraph.inputTensorMetadata = [input_meta]
+        subgraph.outputTensorMetadata = [output1, output2] if self.model.task == 'segment' else [output1]
+        model_meta.subgraphMetadata = [subgraph]
+
+        b = flatbuffers.Builder(0)
+        b.Finish(model_meta.Pack(b), _metadata.MetadataPopulator.METADATA_FILE_IDENTIFIER)
+        metadata_buf = b.Output()
+
+        populator = _metadata.MetadataPopulator.with_model_file(str(file))
+        populator.load_metadata_buffer(metadata_buf)
+        populator.load_associated_files([str(tmp_file)])
+        populator.populate()
+        tmp_file.unlink()
 
     def _pipeline_coreml(self, model, prefix=colorstr('CoreML Pipeline:')):
-        # YOLOv8 CoreML pipeline
+        """YOLOv8 CoreML pipeline."""
         import coremltools as ct  # noqa
 
         LOGGER.info(f'{prefix} starting pipeline with coremltools {ct.__version__}...')
         batch_size, ch, h, w = list(self.im.shape)  # BCHW
 
         # Output shapes
         spec = model.get_spec()
@@ -687,16 +700,16 @@
             from PIL import Image
             img = Image.new('RGB', (w, h))  # img(192 width, 320 height)
             # img = torch.zeros((*opt.img_size, 3)).numpy()  # img size(320,192,3) iDetection
             out = model.predict({'image': img})
             out0_shape = out[out0.name].shape
             out1_shape = out[out1.name].shape
         else:  # linux and windows can not run model.predict(), get sizes from pytorch output y
-            out0_shape = self.output_shape[1], self.output_shape[2] - 5  # (3780, 80)
-            out1_shape = self.output_shape[1], 4  # (3780, 4)
+            out0_shape = self.output_shape[2], self.output_shape[1] - 4  # (3780, 80)
+            out1_shape = self.output_shape[2], 4  # (3780, 4)
 
         # Checks
         names = self.metadata['names']
         nx, ny = spec.description.input[0].type.imageType.width, spec.description.input[0].type.imageType.height
         na, nc = out0_shape
         # na, nc = out0.type.multiArrayType.shape  # number anchors, classes
         assert len(names) == nc, f'{len(names)} names found for nc={nc}'  # check
@@ -714,15 +727,15 @@
         # flexible_shape_utils.add_enumerated_image_sizes(spec, feature_name='image', sizes=s)
         # r = flexible_shape_utils.NeuralNetworkImageSizeRange()  # shape ranges
         # r.add_height_range((192, 640))
         # r.add_width_range((192, 640))
         # flexible_shape_utils.update_image_size_range(spec, feature_name='image', size_range=r)
 
         # Print
-        print(spec.description)
+        # print(spec.description)
 
         # Model from spec
         model = ct.models.MLModel(spec)
 
         # 3. Create NMS protobuf
         nms_spec = ct.proto.Model_pb2.Model()
         nms_spec.specificationVersion = 5
@@ -771,18 +784,14 @@
         # Correct datatypes
         pipeline.spec.description.input[0].ParseFromString(model._spec.description.input[0].SerializeToString())
         pipeline.spec.description.output[0].ParseFromString(nms_model._spec.description.output[0].SerializeToString())
         pipeline.spec.description.output[1].ParseFromString(nms_model._spec.description.output[1].SerializeToString())
 
         # Update metadata
         pipeline.spec.specificationVersion = 5
-        pipeline.spec.description.metadata.versionString = f'Ultralytics YOLOv{ultralytics.__version__}'
-        pipeline.spec.description.metadata.shortDescription = f'Ultralytics {self.pretty_name} CoreML model'
-        pipeline.spec.description.metadata.author = 'Ultralytics (https://ultralytics.com)'
-        pipeline.spec.description.metadata.license = 'GPL-3.0 license (https://ultralytics.com/license)'
         pipeline.spec.description.metadata.userDefined.update({
             'IoU threshold': str(nms.iouThreshold),
             'Confidence threshold': str(nms.confidenceThreshold)})
 
         # Save the model
         model = ct.models.MLModel(pipeline.spec)
         model.input_description['image'] = 'Input image'
@@ -790,40 +799,55 @@
         model.input_description['confidenceThreshold'] = \
             f'(optional) Confidence threshold override (default: {nms.confidenceThreshold})'
         model.output_description['confidence'] = 'Boxes × Class confidence (see user-defined metadata "classes")'
         model.output_description['coordinates'] = 'Boxes × [x, y, width, height] (relative to image size)'
         LOGGER.info(f'{prefix} pipeline success')
         return model
 
+    def add_callback(self, event: str, callback):
+        """
+        Appends the given callback.
+        """
+        self.callbacks[event].append(callback)
+
     def run_callbacks(self, event: str):
+        """Execute all callbacks for a given event."""
         for callback in self.callbacks.get(event, []):
             callback(self)
 
 
-@hydra.main(version_base=None, config_path=str(DEFAULT_CONFIG.parent), config_name=DEFAULT_CONFIG.name)
-def export(cfg):
-    cfg.model = cfg.model or "yolov8n.yaml"
-    cfg.format = cfg.format or "torchscript"
-
-    # exporter = Exporter(cfg)
-    #
-    # model = None
-    # if isinstance(cfg.model, (str, Path)):
-    #     if Path(cfg.model).suffix == '.yaml':
-    #         model = DetectionModel(cfg.model)
-    #     elif Path(cfg.model).suffix == '.pt':
-    #         model = attempt_load_weights(cfg.model, fuse=True)
-    #     else:
-    #         TypeError(f'Unsupported model type {cfg.model}')
-    # exporter(model=model)
+class iOSDetectModel(torch.nn.Module):
+    """Wrap an Ultralytics YOLO model for iOS export."""
+
+    def __init__(self, model, im):
+        """Initialize the iOSDetectModel class with a YOLO model and example image."""
+        super().__init__()
+        b, c, h, w = im.shape  # batch, channel, height, width
+        self.model = model
+        self.nc = len(model.names)  # number of classes
+        if w == h:
+            self.normalize = 1.0 / w  # scalar
+        else:
+            self.normalize = torch.tensor([1.0 / w, 1.0 / h, 1.0 / w, 1.0 / h])  # broadcast (slower, smaller)
+
+    def forward(self, x):
+        """Normalize predictions of object detection model with input size-dependent factors."""
+        xywh, cls = self.model(x)[0].transpose(0, 1).split((4, self.nc), 1)
+        return cls, xywh * self.normalize  # confidence (3780, 80), coordinates (3780, 4)
+
+
+def export(cfg=DEFAULT_CFG):
+    """Export a YOLOv model to a specific format."""
+    cfg.model = cfg.model or 'yolov8n.yaml'
+    cfg.format = cfg.format or 'torchscript'
 
     from ultralytics import YOLO
     model = YOLO(cfg.model)
-    model.export(**cfg)
+    model.export(**vars(cfg))
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     """
     CLI:
     yolo mode=export model=yolov8n.yaml format=onnx
     """
     export()
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/engine/trainer.py` & `ultralytics-8.0.90/ultralytics/yolo/engine/trainer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,60 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
-"""
-Simple training loop; Boilerplate that could apply to any arbitrary neural network,
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 """
+Train a model on a dataset
 
+Usage:
+    $ yolo mode=train model=yolov8n.pt data=coco128.yaml imgsz=640 epochs=100 batch=16
+"""
 import os
 import subprocess
 import time
-from collections import defaultdict
 from copy import deepcopy
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 import torch
 import torch.distributed as dist
 import torch.nn as nn
-from omegaconf import OmegaConf  # noqa
-from omegaconf import open_dict
 from torch.cuda import amp
 from torch.nn.parallel import DistributedDataParallel as DDP
 from torch.optim import lr_scheduler
 from tqdm import tqdm
 
-import ultralytics.yolo.utils as utils
-from ultralytics import __version__
-from ultralytics.nn.tasks import attempt_load_one_weight
-from ultralytics.yolo.configs import get_config
-from ultralytics.yolo.data.utils import check_dataset, check_dataset_yaml
-from ultralytics.yolo.utils import (DEFAULT_CONFIG, LOGGER, RANK, SETTINGS, TQDM_BAR_FORMAT, callbacks, colorstr,
-                                    yaml_save)
+from ultralytics.nn.tasks import attempt_load_one_weight, attempt_load_weights
+from ultralytics.yolo.cfg import get_cfg
+from ultralytics.yolo.data.utils import check_cls_dataset, check_det_dataset
+from ultralytics.yolo.utils import (DEFAULT_CFG, LOGGER, ONLINE, RANK, ROOT, SETTINGS, TQDM_BAR_FORMAT, __version__,
+                                    callbacks, clean_url, colorstr, emojis, yaml_save)
 from ultralytics.yolo.utils.autobatch import check_train_batch_size
 from ultralytics.yolo.utils.checks import check_file, check_imgsz, print_args
 from ultralytics.yolo.utils.dist import ddp_cleanup, generate_ddp_command
 from ultralytics.yolo.utils.files import get_latest_run, increment_path
-from ultralytics.yolo.utils.torch_utils import ModelEMA, de_parallel, init_seeds, one_cycle, strip_optimizer
+from ultralytics.yolo.utils.torch_utils import (EarlyStopping, ModelEMA, de_parallel, init_seeds, one_cycle,
+                                                select_device, strip_optimizer)
 
 
 class BaseTrainer:
     """
     BaseTrainer
 
     A base class for creating trainers.
 
     Attributes:
-        args (OmegaConf): Configuration for the trainer.
+        args (SimpleNamespace): Configuration for the trainer.
         check_resume (method): Method to check if training should be resumed from a saved checkpoint.
-        console (logging.Logger): Logger instance.
         validator (BaseValidator): Validator instance.
         model (nn.Module): Model instance.
         callbacks (defaultdict): Dictionary of callbacks.
         save_dir (Path): Directory to save results.
         wdir (Path): Directory to save weights.
         last (Path): Path to last checkpoint.
         best (Path): Path to best checkpoint.
+        save_period (int): Save checkpoint every x epochs (disabled if < 1).
         batch_size (int): Batch size for training.
         epochs (int): Number of epochs to train for.
         start_epoch (int): Starting epoch for training.
         device (torch.device): Device to use for training.
         amp (bool): Flag to enable AMP (Automatic Mixed Precision).
         scaler (amp.GradScaler): Gradient scaler for AMP.
         data (str): Path to data.
@@ -69,67 +67,68 @@
         fitness (float): Current fitness value.
         loss (float): Current loss value.
         tloss (float): Total loss value.
         loss_names (list): List of loss names.
         csv (Path): Path to results CSV file.
     """
 
-    def __init__(self, config=DEFAULT_CONFIG, overrides=None):
+    def __init__(self, cfg=DEFAULT_CFG, overrides=None, _callbacks=None):
         """
         Initializes the BaseTrainer class.
 
         Args:
-            config (str, optional): Path to a configuration file. Defaults to DEFAULT_CONFIG.
+            cfg (str, optional): Path to a configuration file. Defaults to DEFAULT_CFG.
             overrides (dict, optional): Configuration overrides. Defaults to None.
         """
-        if overrides is None:
-            overrides = {}
-        self.args = get_config(config, overrides)
-        self.device = utils.torch_utils.select_device(self.args.device, self.args.batch)
+        self.args = get_cfg(cfg, overrides)
+        self.device = select_device(self.args.device, self.args.batch)
         self.check_resume()
-        self.console = LOGGER
         self.validator = None
         self.model = None
-        self.callbacks = defaultdict(list)
+        self.metrics = None
         init_seeds(self.args.seed + 1 + RANK, deterministic=self.args.deterministic)
 
         # Dirs
         project = self.args.project or Path(SETTINGS['runs_dir']) / self.args.task
-        name = self.args.name or f"{self.args.mode}"
-        self.save_dir = Path(
-            self.args.get(
-                "save_dir",
-                increment_path(Path(project) / name, exist_ok=self.args.exist_ok if RANK in {-1, 0} else True)))
+        name = self.args.name or f'{self.args.mode}'
+        if hasattr(self.args, 'save_dir'):
+            self.save_dir = Path(self.args.save_dir)
+        else:
+            self.save_dir = Path(
+                increment_path(Path(project) / name, exist_ok=self.args.exist_ok if RANK in (-1, 0) else True))
         self.wdir = self.save_dir / 'weights'  # weights dir
-        if RANK in {-1, 0}:
+        if RANK in (-1, 0):
             self.wdir.mkdir(parents=True, exist_ok=True)  # make dir
-            with open_dict(self.args):
-                self.args.save_dir = str(self.save_dir)
-            yaml_save(self.save_dir / 'args.yaml', OmegaConf.to_container(self.args, resolve=True))  # save run args
+            self.args.save_dir = str(self.save_dir)
+            yaml_save(self.save_dir / 'args.yaml', vars(self.args))  # save run args
         self.last, self.best = self.wdir / 'last.pt', self.wdir / 'best.pt'  # checkpoint paths
+        self.save_period = self.args.save_period
 
         self.batch_size = self.args.batch
         self.epochs = self.args.epochs
         self.start_epoch = 0
         if RANK == -1:
-            print_args(dict(self.args))
+            print_args(vars(self.args))
 
         # Device
-        self.amp = self.device.type != 'cpu'
-        self.scaler = amp.GradScaler(enabled=self.amp)
         if self.device.type == 'cpu':
             self.args.workers = 0  # faster CPU training as time dominated by inference, not dataloading
 
-        # Model and Dataloaders.
+        # Model and Dataset
         self.model = self.args.model
-        self.data = self.args.data
-        if self.data.endswith(".yaml"):
-            self.data = check_dataset_yaml(self.data)
-        else:
-            self.data = check_dataset(self.data)
+        try:
+            if self.args.task == 'classify':
+                self.data = check_cls_dataset(self.args.data)
+            elif self.args.data.endswith('.yaml') or self.args.task in ('detect', 'segment'):
+                self.data = check_det_dataset(self.args.data)
+                if 'yaml_file' in self.data:
+                    self.args.data = self.data['yaml_file']  # for validating 'yolo train data=url.zip' usage
+        except Exception as e:
+            raise RuntimeError(emojis(f"Dataset '{clean_url(self.args.data)}' error ❌ {e}")) from e
+
         self.trainset, self.testset = self.get_dataset(self.data)
         self.ema = None
 
         # Optimization utils init
         self.lf = None
         self.scheduler = None
 
@@ -139,16 +138,16 @@
         self.loss = None
         self.tloss = None
         self.loss_names = ['Loss']
         self.csv = self.save_dir / 'results.csv'
         self.plot_idx = [0, 1, 2]
 
         # Callbacks
-        self.callbacks = defaultdict(list, {k: [v] for k, v in callbacks.default_callbacks.items()})  # add callbacks
-        if RANK in {0, -1}:
+        self.callbacks = _callbacks or callbacks.get_default_callbacks()
+        if RANK in (-1, 0):
             callbacks.add_integration_callbacks(self)
 
     def add_callback(self, event: str, callback):
         """
         Appends the given callback.
         """
         self.callbacks[event].append(callback)
@@ -156,156 +155,178 @@
     def set_callback(self, event: str, callback):
         """
         Overrides the existing callbacks with the given callback.
         """
         self.callbacks[event] = [callback]
 
     def run_callbacks(self, event: str):
+        """Run all existing callbacks associated with a particular event."""
         for callback in self.callbacks.get(event, []):
             callback(self)
 
     def train(self):
-        # Allow device='', device=None on Multi-GPU systems to default to device=0
+        """Allow device='', device=None on Multi-GPU systems to default to device=0."""
         if isinstance(self.args.device, int) or self.args.device:  # i.e. device=0 or device=[0,1,2,3]
             world_size = torch.cuda.device_count()
         elif torch.cuda.is_available():  # i.e. device=None or device=''
             world_size = 1  # default to device 0
         else:  # i.e. device='cpu' or 'mps'
             world_size = 0
 
         # Run subprocess if DDP training, else train normally
-        if world_size > 1 and "LOCAL_RANK" not in os.environ:
-            command = generate_ddp_command(world_size, self)
+        if world_size > 1 and 'LOCAL_RANK' not in os.environ:
+            # Argument checks
+            if self.args.rect:
+                LOGGER.warning("WARNING ⚠️ 'rect=True' is incompatible with Multi-GPU training, setting rect=False")
+                self.args.rect = False
+            # Command
+            cmd, file = generate_ddp_command(world_size, self)
             try:
-                subprocess.run(command)
+                LOGGER.info(f'Running DDP command {cmd}')
+                subprocess.run(cmd, check=True)
             except Exception as e:
-                self.console(e)
+                raise e
             finally:
-                ddp_cleanup(command, self)
+                ddp_cleanup(self, str(file))
         else:
-            self._do_train(int(os.getenv("RANK", -1)), world_size)
+            self._do_train(world_size)
 
-    def _setup_ddp(self, rank, world_size):
-        # os.environ['MASTER_ADDR'] = 'localhost'
-        # os.environ['MASTER_PORT'] = '9020'
-        torch.cuda.set_device(rank)
-        self.device = torch.device('cuda', rank)
-        self.console.info(f"DDP settings: RANK {rank}, WORLD_SIZE {world_size}, DEVICE {self.device}")
-        dist.init_process_group("nccl" if dist.is_nccl_available() else "gloo", rank=rank, world_size=world_size)
+    def _setup_ddp(self, world_size):
+        """Initializes and sets the DistributedDataParallel parameters for training."""
+        torch.cuda.set_device(RANK)
+        self.device = torch.device('cuda', RANK)
+        LOGGER.info(f'DDP settings: RANK {RANK}, WORLD_SIZE {world_size}, DEVICE {self.device}')
+        dist.init_process_group('nccl' if dist.is_nccl_available() else 'gloo', rank=RANK, world_size=world_size)
 
-    def _setup_train(self, rank, world_size):
+    def _setup_train(self, world_size):
         """
         Builds dataloaders and optimizer on correct rank process.
         """
-        # model
-        self.run_callbacks("on_pretrain_routine_start")
+        # Model
+        self.run_callbacks('on_pretrain_routine_start')
         ckpt = self.setup_model()
         self.model = self.model.to(self.device)
         self.set_model_attributes()
+        # Check AMP
+        self.amp = torch.tensor(self.args.amp).to(self.device)  # True or False
+        if self.amp and RANK in (-1, 0):  # Single-GPU and DDP
+            callbacks_backup = callbacks.default_callbacks.copy()  # backup callbacks as check_amp() resets them
+            self.amp = torch.tensor(check_amp(self.model), device=self.device)
+            callbacks.default_callbacks = callbacks_backup  # restore callbacks
+        if RANK > -1:  # DDP
+            dist.broadcast(self.amp, src=0)  # broadcast the tensor from rank 0 to all other ranks (returns None)
+        self.amp = bool(self.amp)  # as boolean
+        self.scaler = amp.GradScaler(enabled=self.amp)
         if world_size > 1:
-            self.model = DDP(self.model, device_ids=[rank])
+            self.model = DDP(self.model, device_ids=[RANK])
         # Check imgsz
         gs = max(int(self.model.stride.max() if hasattr(self.model, 'stride') else 32), 32)  # grid size (max stride)
-        self.args.imgsz = check_imgsz(self.args.imgsz, stride=gs, floor=gs * 2)
+        self.args.imgsz = check_imgsz(self.args.imgsz, stride=gs, floor=gs, max_dim=1)
         # Batch size
         if self.batch_size == -1:
             if RANK == -1:  # single-GPU only, estimate best batch size
                 self.batch_size = check_train_batch_size(self.model, self.args.imgsz, self.amp)
             else:
                 SyntaxError('batch=-1 to use AutoBatch is only available in Single-GPU training. '
                             'Please pass a valid batch size value for Multi-GPU DDP training, i.e. batch=16')
 
         # Optimizer
         self.accumulate = max(round(self.args.nbs / self.batch_size), 1)  # accumulate loss before optimizing
-        self.args.weight_decay *= self.batch_size * self.accumulate / self.args.nbs  # scale weight_decay
+        weight_decay = self.args.weight_decay * self.batch_size * self.accumulate / self.args.nbs  # scale weight_decay
         self.optimizer = self.build_optimizer(model=self.model,
                                               name=self.args.optimizer,
                                               lr=self.args.lr0,
                                               momentum=self.args.momentum,
-                                              decay=self.args.weight_decay)
+                                              decay=weight_decay)
         # Scheduler
         if self.args.cos_lr:
             self.lf = one_cycle(1, self.args.lrf, self.epochs)  # cosine 1->hyp['lrf']
         else:
             self.lf = lambda x: (1 - x / self.epochs) * (1.0 - self.args.lrf) + self.args.lrf  # linear
         self.scheduler = lr_scheduler.LambdaLR(self.optimizer, lr_lambda=self.lf)
-        self.scheduler.last_epoch = self.start_epoch - 1  # do not move
+        self.stopper, self.stop = EarlyStopping(patience=self.args.patience), False
 
-        # dataloaders
+        # Dataloaders
         batch_size = self.batch_size // world_size if world_size > 1 else self.batch_size
-        self.train_loader = self.get_dataloader(self.trainset, batch_size=batch_size, rank=rank, mode="train")
-        if rank in {0, -1}:
-            self.test_loader = self.get_dataloader(self.testset, batch_size=batch_size * 2, rank=-1, mode="val")
+        self.train_loader = self.get_dataloader(self.trainset, batch_size=batch_size, rank=RANK, mode='train')
+        if RANK in (-1, 0):
+            self.test_loader = self.get_dataloader(self.testset, batch_size=batch_size * 2, rank=-1, mode='val')
             self.validator = self.get_validator()
-            metric_keys = self.validator.metrics.keys + self.label_loss_items(prefix="val")
+            metric_keys = self.validator.metrics.keys + self.label_loss_items(prefix='val')
             self.metrics = dict(zip(metric_keys, [0] * len(metric_keys)))  # TODO: init metrics for plot_results()?
             self.ema = ModelEMA(self.model)
+            if self.args.plots and not self.args.v5loader:
+                self.plot_training_labels()
         self.resume_training(ckpt)
-        self.run_callbacks("on_pretrain_routine_end")
+        self.scheduler.last_epoch = self.start_epoch - 1  # do not move
+        self.run_callbacks('on_pretrain_routine_end')
 
-    def _do_train(self, rank=-1, world_size=1):
+    def _do_train(self, world_size=1):
+        """Train completed, evaluate and plot if specified by arguments."""
         if world_size > 1:
-            self._setup_ddp(rank, world_size)
+            self._setup_ddp(world_size)
 
-        self._setup_train(rank, world_size)
+        self._setup_train(world_size)
 
         self.epoch_time = None
         self.epoch_time_start = time.time()
         self.train_time_start = time.time()
         nb = len(self.train_loader)  # number of batches
         nw = max(round(self.args.warmup_epochs * nb), 100)  # number of warmup iterations
         last_opt_step = -1
-        self.run_callbacks("on_train_start")
-        self.log(f"Image sizes {self.args.imgsz} train, {self.args.imgsz} val\n"
-                 f'Using {self.train_loader.num_workers * (world_size or 1)} dataloader workers\n'
-                 f"Logging results to {colorstr('bold', self.save_dir)}\n"
-                 f"Starting training for {self.epochs} epochs...")
+        self.run_callbacks('on_train_start')
+        LOGGER.info(f'Image sizes {self.args.imgsz} train, {self.args.imgsz} val\n'
+                    f'Using {self.train_loader.num_workers * (world_size or 1)} dataloader workers\n'
+                    f"Logging results to {colorstr('bold', self.save_dir)}\n"
+                    f'Starting training for {self.epochs} epochs...')
         if self.args.close_mosaic:
             base_idx = (self.epochs - self.args.close_mosaic) * nb
             self.plot_idx.extend([base_idx, base_idx + 1, base_idx + 2])
+        epoch = self.epochs  # predefine for resume fully trained model edge cases
         for epoch in range(self.start_epoch, self.epochs):
             self.epoch = epoch
-            self.run_callbacks("on_train_epoch_start")
+            self.run_callbacks('on_train_epoch_start')
             self.model.train()
-            if rank != -1:
+            if RANK != -1:
                 self.train_loader.sampler.set_epoch(epoch)
             pbar = enumerate(self.train_loader)
             # Update dataloader attributes (optional)
             if epoch == (self.epochs - self.args.close_mosaic):
-                self.console.info("Closing dataloader mosaic")
+                LOGGER.info('Closing dataloader mosaic')
                 if hasattr(self.train_loader.dataset, 'mosaic'):
                     self.train_loader.dataset.mosaic = False
                 if hasattr(self.train_loader.dataset, 'close_mosaic'):
                     self.train_loader.dataset.close_mosaic(hyp=self.args)
+                self.train_loader.reset()
 
-            if rank in {-1, 0}:
-                self.console.info(self.progress_string())
+            if RANK in (-1, 0):
+                LOGGER.info(self.progress_string())
                 pbar = tqdm(enumerate(self.train_loader), total=nb, bar_format=TQDM_BAR_FORMAT)
             self.tloss = None
             self.optimizer.zero_grad()
             for i, batch in pbar:
-                self.run_callbacks("on_train_batch_start")
+                self.run_callbacks('on_train_batch_start')
                 # Warmup
                 ni = i + nb * epoch
                 if ni <= nw:
                     xi = [0, nw]  # x interp
                     self.accumulate = max(1, np.interp(ni, xi, [1, self.args.nbs / self.batch_size]).round())
                     for j, x in enumerate(self.optimizer.param_groups):
-                        # bias lr falls from 0.1 to lr0, all other lrs rise from 0.0 to lr0
+                        # Bias lr falls from 0.1 to lr0, all other lrs rise from 0.0 to lr0
                         x['lr'] = np.interp(
                             ni, xi, [self.args.warmup_bias_lr if j == 0 else 0.0, x['initial_lr'] * self.lf(epoch)])
                         if 'momentum' in x:
                             x['momentum'] = np.interp(ni, xi, [self.args.warmup_momentum, self.args.momentum])
 
                 # Forward
                 with torch.cuda.amp.autocast(self.amp):
                     batch = self.preprocess_batch(batch)
-                    preds = self.model(batch["img"])
+                    preds = self.model(batch['img'])
                     self.loss, self.loss_items = self.criterion(preds, batch)
-                    if rank != -1:
+                    if RANK != -1:
                         self.loss *= world_size
                     self.tloss = (self.tloss * i + self.loss_items) / (i + 1) if self.tloss is not None \
                         else self.loss_items
 
                 # Backward
                 self.scaler.scale(self.loss).backward()
 
@@ -314,103 +335,118 @@
                     self.optimizer_step()
                     last_opt_step = ni
 
                 # Log
                 mem = f'{torch.cuda.memory_reserved() / 1E9 if torch.cuda.is_available() else 0:.3g}G'  # (GB)
                 loss_len = self.tloss.shape[0] if len(self.tloss.size()) else 1
                 losses = self.tloss if loss_len > 1 else torch.unsqueeze(self.tloss, 0)
-                if rank in {-1, 0}:
+                if RANK in (-1, 0):
                     pbar.set_description(
                         ('%11s' * 2 + '%11.4g' * (2 + loss_len)) %
-                        (f'{epoch + 1}/{self.epochs}', mem, *losses, batch["cls"].shape[0], batch["img"].shape[-1]))
+                        (f'{epoch + 1}/{self.epochs}', mem, *losses, batch['cls'].shape[0], batch['img'].shape[-1]))
                     self.run_callbacks('on_batch_end')
                     if self.args.plots and ni in self.plot_idx:
                         self.plot_training_samples(batch, ni)
 
-                self.run_callbacks("on_train_batch_end")
+                self.run_callbacks('on_train_batch_end')
 
-            self.lr = {f"lr/pg{ir}": x['lr'] for ir, x in enumerate(self.optimizer.param_groups)}  # for loggers
+            self.lr = {f'lr/pg{ir}': x['lr'] for ir, x in enumerate(self.optimizer.param_groups)}  # for loggers
 
             self.scheduler.step()
-            self.run_callbacks("on_train_epoch_end")
+            self.run_callbacks('on_train_epoch_end')
 
-            if rank in {-1, 0}:
+            if RANK in (-1, 0):
 
                 # Validation
                 self.ema.update_attr(self.model, include=['yaml', 'nc', 'args', 'names', 'stride', 'class_weights'])
-                final_epoch = (epoch + 1 == self.epochs)
+                final_epoch = (epoch + 1 == self.epochs) or self.stopper.possible_stop
+
                 if self.args.val or final_epoch:
                     self.metrics, self.fitness = self.validate()
                 self.save_metrics(metrics={**self.label_loss_items(self.tloss), **self.metrics, **self.lr})
+                self.stop = self.stopper(epoch + 1, self.fitness)
 
                 # Save model
                 if self.args.save or (epoch + 1 == self.epochs):
                     self.save_model()
                     self.run_callbacks('on_model_save')
 
             tnow = time.time()
             self.epoch_time = tnow - self.epoch_time_start
             self.epoch_time_start = tnow
-            self.run_callbacks("on_fit_epoch_end")
-            # TODO: termination condition
+            self.run_callbacks('on_fit_epoch_end')
+            torch.cuda.empty_cache()  # clears GPU vRAM at end of epoch, can help with out of memory errors
 
-        if rank in {-1, 0}:
+            # Early Stopping
+            if RANK != -1:  # if DDP training
+                broadcast_list = [self.stop if RANK == 0 else None]
+                dist.broadcast_object_list(broadcast_list, 0)  # broadcast 'stop' to all ranks
+                if RANK != 0:
+                    self.stop = broadcast_list[0]
+            if self.stop:
+                break  # must break all DDP ranks
+
+        if RANK in (-1, 0):
             # Do final val with best.pt
-            self.log(f'\n{epoch - self.start_epoch + 1} epochs completed in '
-                     f'{(time.time() - self.train_time_start) / 3600:.3f} hours.')
+            LOGGER.info(f'\n{epoch - self.start_epoch + 1} epochs completed in '
+                        f'{(time.time() - self.train_time_start) / 3600:.3f} hours.')
             self.final_eval()
             if self.args.plots:
                 self.plot_metrics()
-            self.log(f"Results saved to {colorstr('bold', self.save_dir)}")
             self.run_callbacks('on_train_end')
         torch.cuda.empty_cache()
         self.run_callbacks('teardown')
 
     def save_model(self):
+        """Save model checkpoints based on various conditions."""
         ckpt = {
             'epoch': self.epoch,
             'best_fitness': self.best_fitness,
             'model': deepcopy(de_parallel(self.model)).half(),
             'ema': deepcopy(self.ema.ema).half(),
             'updates': self.ema.updates,
             'optimizer': self.optimizer.state_dict(),
-            'train_args': self.args,
+            'train_args': vars(self.args),  # save as dict
             'date': datetime.now().isoformat(),
             'version': __version__}
 
         # Save last, best and delete
         torch.save(ckpt, self.last)
         if self.best_fitness == self.fitness:
             torch.save(ckpt, self.best)
+        if (self.epoch > 0) and (self.save_period > 0) and (self.epoch % self.save_period == 0):
+            torch.save(ckpt, self.wdir / f'epoch{self.epoch}.pt')
         del ckpt
 
-    def get_dataset(self, data):
+    @staticmethod
+    def get_dataset(data):
         """
         Get train, val path from data dict if it exists. Returns None if data format is not recognized.
         """
-        return data["train"], data.get("val") or data.get("test")
+        return data['train'], data.get('val') or data.get('test')
 
     def setup_model(self):
         """
         load/create/download model for any task.
         """
         if isinstance(self.model, torch.nn.Module):  # if model is loaded beforehand. No setup needed
             return
 
         model, weights = self.model, None
         ckpt = None
-        if str(model).endswith(".pt"):
+        if str(model).endswith('.pt'):
             weights, ckpt = attempt_load_one_weight(model)
-            cfg = ckpt["model"].yaml
+            cfg = ckpt['model'].yaml
         else:
             cfg = model
-        self.model = self.get_model(cfg=cfg, weights=weights)  # calls Model(cfg, weights)
+        self.model = self.get_model(cfg=cfg, weights=weights, verbose=RANK == -1)  # calls Model(cfg, weights)
         return ckpt
 
     def optimizer_step(self):
+        """Perform a single step of the training optimizer with gradient clipping and EMA update."""
         self.scaler.unscale_(self.optimizer)  # unscale gradients
         torch.nn.utils.clip_grad_norm_(self.model.parameters(), max_norm=10.0)  # clip gradients
         self.scaler.step(self.optimizer)
         self.scaler.update()
         self.optimizer.zero_grad()
         if self.ema:
             self.ema.update(self.model)
@@ -422,129 +458,141 @@
         return batch
 
     def validate(self):
         """
         Runs validation on test set using self.validator. The returned dict is expected to contain "fitness" key.
         """
         metrics = self.validator(self)
-        fitness = metrics.pop("fitness", -self.loss.detach().cpu().numpy())  # use loss as fitness measure if not found
+        fitness = metrics.pop('fitness', -self.loss.detach().cpu().numpy())  # use loss as fitness measure if not found
         if not self.best_fitness or self.best_fitness < fitness:
             self.best_fitness = fitness
         return metrics, fitness
 
-    def log(self, text, rank=-1):
-        """
-        Logs the given text to given ranks process if provided, otherwise logs to all ranks.
-
-        Args"
-            text (str): text to log
-            rank (List[Int]): process rank
-
-        """
-        if rank in {-1, 0}:
-            self.console.info(text)
-
     def get_model(self, cfg=None, weights=None, verbose=True):
+        """Get model and raise NotImplementedError for loading cfg files."""
         raise NotImplementedError("This task trainer doesn't support loading cfg files")
 
     def get_validator(self):
-        raise NotImplementedError("get_validator function not implemented in trainer")
+        """Returns a NotImplementedError when the get_validator function is called."""
+        raise NotImplementedError('get_validator function not implemented in trainer')
 
-    def get_dataloader(self, dataset_path, batch_size=16, rank=0):
+    def get_dataloader(self, dataset_path, batch_size=16, rank=0, mode='train'):
         """
         Returns dataloader derived from torch.data.Dataloader.
         """
-        raise NotImplementedError("get_dataloader function not implemented in trainer")
+        raise NotImplementedError('get_dataloader function not implemented in trainer')
+
+    def build_dataset(self, img_path, mode='train', batch=None):
+        """Build dataset"""
+        raise NotImplementedError('build_dataset function not implemented in trainer')
 
     def criterion(self, preds, batch):
         """
         Returns loss and individual loss items as Tensor.
         """
-        raise NotImplementedError("criterion function not implemented in trainer")
+        raise NotImplementedError('criterion function not implemented in trainer')
 
-    def label_loss_items(self, loss_items=None, prefix="train"):
+    def label_loss_items(self, loss_items=None, prefix='train'):
         """
         Returns a loss dict with labelled training loss items tensor
         """
         # Not needed for classification but necessary for segmentation & detection
-        return {"loss": loss_items} if loss_items is not None else ["loss"]
+        return {'loss': loss_items} if loss_items is not None else ['loss']
 
     def set_model_attributes(self):
         """
         To set or update model parameters before training.
         """
-        self.model.names = self.data["names"]
+        self.model.names = self.data['names']
 
     def build_targets(self, preds, targets):
+        """Builds target tensors for training YOLO model."""
         pass
 
     def progress_string(self):
-        return ""
+        """Returns a string describing training progress."""
+        return ''
 
     # TODO: may need to put these following functions into callback
     def plot_training_samples(self, batch, ni):
+        """Plots training samples during YOLOv5 training."""
+        pass
+
+    def plot_training_labels(self):
+        """Plots training labels for YOLO model."""
         pass
 
     def save_metrics(self, metrics):
+        """Saves training metrics to a CSV file."""
         keys, vals = list(metrics.keys()), list(metrics.values())
         n = len(metrics) + 1  # number of cols
         s = '' if self.csv.exists() else (('%23s,' * n % tuple(['epoch'] + keys)).rstrip(',') + '\n')  # header
         with open(self.csv, 'a') as f:
             f.write(s + ('%23.5g,' * n % tuple([self.epoch] + vals)).rstrip(',') + '\n')
 
     def plot_metrics(self):
+        """Plot and display metrics visually."""
         pass
 
     def final_eval(self):
+        """Performs final evaluation and validation for object detection YOLO model."""
         for f in self.last, self.best:
             if f.exists():
                 strip_optimizer(f)  # strip optimizers
                 if f is self.best:
-                    self.console.info(f'\nValidating {f}...')
-                    self.validator.args.save_json = True
+                    LOGGER.info(f'\nValidating {f}...')
                     self.metrics = self.validator(model=f)
                     self.metrics.pop('fitness', None)
                     self.run_callbacks('on_fit_epoch_end')
 
     def check_resume(self):
+        """Check if resume checkpoint exists and update arguments accordingly."""
         resume = self.args.resume
         if resume:
-            last = Path(check_file(resume) if isinstance(resume, (str, Path)) else get_latest_run())
-            args_yaml = last.parent.parent / 'args.yaml'  # train options yaml
-            assert args_yaml.is_file(), \
-                FileNotFoundError('Resume checkpoint f{last} not found. '
-                                  'Please pass a valid checkpoint to resume from, i.e. yolo resume=path/to/last.pt')
-            args = get_config(args_yaml)  # replace
-            args.model, resume = str(last), True  # reinstate
-            self.args = args
+            try:
+                last = Path(
+                    check_file(resume) if isinstance(resume, (str,
+                                                              Path)) and Path(resume).exists() else get_latest_run())
+                self.args = get_cfg(attempt_load_weights(last).args)
+                self.args.model, resume = str(last), True  # reinstate
+            except Exception as e:
+                raise FileNotFoundError('Resume checkpoint not found. Please pass a valid checkpoint to resume from, '
+                                        "i.e. 'yolo train resume model=path/to/last.pt'") from e
         self.resume = resume
 
     def resume_training(self, ckpt):
+        """Resume YOLO training from given epoch and best fitness."""
         if ckpt is None:
             return
         best_fitness = 0.0
         start_epoch = ckpt['epoch'] + 1
         if ckpt['optimizer'] is not None:
             self.optimizer.load_state_dict(ckpt['optimizer'])  # optimizer
             best_fitness = ckpt['best_fitness']
         if self.ema and ckpt.get('ema'):
             self.ema.ema.load_state_dict(ckpt['ema'].float().state_dict())  # EMA
             self.ema.updates = ckpt['updates']
         if self.resume:
             assert start_epoch > 0, \
                 f'{self.args.model} training to {self.epochs} epochs is finished, nothing to resume.\n' \
-                f"Start a new training without --resume, i.e. 'yolo task=... mode=train model={self.args.model}'"
+                f"Start a new training without resuming, i.e. 'yolo train model={self.args.model}'"
             LOGGER.info(
-                f'Resuming training from {self.args.model} from epoch {start_epoch} to {self.epochs} total epochs')
+                f'Resuming training from {self.args.model} from epoch {start_epoch + 1} to {self.epochs} total epochs')
         if self.epochs < start_epoch:
             LOGGER.info(
                 f"{self.model} has been trained for {ckpt['epoch']} epochs. Fine-tuning for {self.epochs} more epochs.")
             self.epochs += ckpt['epoch']  # finetune additional epochs
         self.best_fitness = best_fitness
         self.start_epoch = start_epoch
+        if start_epoch > (self.epochs - self.args.close_mosaic):
+            LOGGER.info('Closing dataloader mosaic')
+            if hasattr(self.train_loader.dataset, 'mosaic'):
+                self.train_loader.dataset.mosaic = False
+            if hasattr(self.train_loader.dataset, 'close_mosaic'):
+                self.train_loader.dataset.close_mosaic(hyp=self.args)
 
     @staticmethod
     def build_optimizer(model, name='Adam', lr=0.001, momentum=0.9, decay=1e-5):
         """
         Builds an optimizer with the specified parameters and parameter groups.
 
         Args:
@@ -577,9 +625,53 @@
             optimizer = torch.optim.SGD(g[2], lr=lr, momentum=momentum, nesterov=True)
         else:
             raise NotImplementedError(f'Optimizer {name} not implemented.')
 
         optimizer.add_param_group({'params': g[0], 'weight_decay': decay})  # add g0 with weight_decay
         optimizer.add_param_group({'params': g[1], 'weight_decay': 0.0})  # add g1 (BatchNorm2d weights)
         LOGGER.info(f"{colorstr('optimizer:')} {type(optimizer).__name__}(lr={lr}) with parameter groups "
-                    f"{len(g[1])} weight(decay=0.0), {len(g[0])} weight(decay={decay}), {len(g[2])} bias")
+                    f'{len(g[1])} weight(decay=0.0), {len(g[0])} weight(decay={decay}), {len(g[2])} bias')
         return optimizer
+
+
+def check_amp(model):
+    """
+    This function checks the PyTorch Automatic Mixed Precision (AMP) functionality of a YOLOv8 model.
+    If the checks fail, it means there are anomalies with AMP on the system that may cause NaN losses or zero-mAP
+    results, so AMP will be disabled during training.
+
+    Args:
+        model (nn.Module): A YOLOv8 model instance.
+
+    Returns:
+        (bool): Returns True if the AMP functionality works correctly with YOLOv8 model, else False.
+
+    Raises:
+        AssertionError: If the AMP checks fail, indicating anomalies with the AMP functionality on the system.
+    """
+    device = next(model.parameters()).device  # get model device
+    if device.type in ('cpu', 'mps'):
+        return False  # AMP only used on CUDA devices
+
+    def amp_allclose(m, im):
+        """All close FP32 vs AMP results."""
+        a = m(im, device=device, verbose=False)[0].boxes.data  # FP32 inference
+        with torch.cuda.amp.autocast(True):
+            b = m(im, device=device, verbose=False)[0].boxes.data  # AMP inference
+        del m
+        return a.shape == b.shape and torch.allclose(a, b.float(), atol=0.5)  # close to 0.5 absolute tolerance
+
+    f = ROOT / 'assets/bus.jpg'  # image to check
+    im = f if f.exists() else 'https://ultralytics.com/images/bus.jpg' if ONLINE else np.ones((640, 640, 3))
+    prefix = colorstr('AMP: ')
+    LOGGER.info(f'{prefix}running Automatic Mixed Precision (AMP) checks with YOLOv8n...')
+    try:
+        from ultralytics import YOLO
+        assert amp_allclose(YOLO('yolov8n.pt'), im)
+        LOGGER.info(f'{prefix}checks passed ✅')
+    except ConnectionError:
+        LOGGER.warning(f"{prefix}checks skipped ⚠️, offline and unable to download YOLOv8n. Setting 'amp=True'.")
+    except AssertionError:
+        LOGGER.warning(f'{prefix}checks failed ❌. Anomalies were detected with AMP on your system that may lead to '
+                       f'NaN losses or zero-mAP results, so AMP will be disabled during training.')
+        return False
+    return True
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/utils/autobatch.py` & `ultralytics-8.0.90/ultralytics/yolo/utils/autobatch.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,55 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 """
-Auto-batch utils
+Functions for estimating the best YOLO batch size to use a fraction of the available CUDA memory in PyTorch.
 """
 
 from copy import deepcopy
 
 import numpy as np
 import torch
 
 from ultralytics.yolo.utils import LOGGER, colorstr
 from ultralytics.yolo.utils.torch_utils import profile
 
 
 def check_train_batch_size(model, imgsz=640, amp=True):
-    # Check YOLOv5 training batch size
+    """
+    Check YOLO training batch size using the autobatch() function.
+
+    Args:
+        model (torch.nn.Module): YOLO model to check batch size for.
+        imgsz (int): Image size used for training.
+        amp (bool): If True, use automatic mixed precision (AMP) for training.
+
+    Returns:
+        (int): Optimal batch size computed using the autobatch() function.
+    """
+
     with torch.cuda.amp.autocast(amp):
         return autobatch(deepcopy(model).train(), imgsz)  # compute optimal batch size
 
 
-def autobatch(model, imgsz=640, fraction=0.7, batch_size=16):
-    # Automatically estimate best YOLOv5 batch size to use `fraction` of available CUDA memory
-    # Usage:
-    #     import torch
-    #     from utils.autobatch import autobatch
-    #     model = torch.hub.load('ultralytics/yolov5', 'yolov5s', autoshape=False)
-    #     print(autobatch(model))
+def autobatch(model, imgsz=640, fraction=0.67, batch_size=16):
+    """
+    Automatically estimate the best YOLO batch size to use a fraction of the available CUDA memory.
+
+    Args:
+        model (torch.nn.module): YOLO model to compute batch size for.
+        imgsz (int, optional): The image size used as input for the YOLO model. Defaults to 640.
+        fraction (float, optional): The fraction of available CUDA memory to use. Defaults to 0.67.
+        batch_size (int, optional): The default batch size to use if an error is detected. Defaults to 16.
+
+    Returns:
+        (int): The optimal batch size.
+    """
 
     # Check device
     prefix = colorstr('AutoBatch: ')
-    LOGGER.info(f'{prefix}Computing optimal batch size for --imgsz {imgsz}')
+    LOGGER.info(f'{prefix}Computing optimal batch size for imgsz={imgsz}')
     device = next(model.parameters()).device  # get model device
     if device.type == 'cpu':
         LOGGER.info(f'{prefix}CUDA not detected, using default CPU batch-size {batch_size}')
         return batch_size
     if torch.backends.cudnn.benchmark:
         LOGGER.info(f'{prefix} ⚠️ Requires torch.backends.cudnn.benchmark=False, using default batch-size {batch_size}')
         return batch_size
@@ -48,25 +65,26 @@
     LOGGER.info(f'{prefix}{d} ({properties.name}) {t:.2f}G total, {r:.2f}G reserved, {a:.2f}G allocated, {f:.2f}G free')
 
     # Profile batch sizes
     batch_sizes = [1, 2, 4, 8, 16]
     try:
         img = [torch.empty(b, 3, imgsz, imgsz) for b in batch_sizes]
         results = profile(img, model, n=3, device=device)
-    except Exception as e:
-        LOGGER.warning(f'{prefix}{e}')
 
-    # Fit a solution
-    y = [x[2] for x in results if x]  # memory [2]
-    p = np.polyfit(batch_sizes[:len(y)], y, deg=1)  # first degree polynomial fit
-    b = int((f * fraction - p[1]) / p[0])  # y intercept (optimal batch size)
-    if None in results:  # some sizes failed
-        i = results.index(None)  # first fail index
-        if b >= batch_sizes[i]:  # y intercept above failure point
-            b = batch_sizes[max(i - 1, 0)]  # select prior safe point
-    if b < 1 or b > 1024:  # b outside of safe range
-        b = batch_size
-        LOGGER.warning(f'{prefix}WARNING ⚠️ CUDA anomaly detected, recommend restart environment and retry command.')
-
-    fraction = (np.polyval(p, b) + r + a) / t  # actual fraction predicted
-    LOGGER.info(f'{prefix}Using batch-size {b} for {d} {t * fraction:.2f}G/{t:.2f}G ({fraction * 100:.0f}%) ✅')
-    return b
+        # Fit a solution
+        y = [x[2] for x in results if x]  # memory [2]
+        p = np.polyfit(batch_sizes[:len(y)], y, deg=1)  # first degree polynomial fit
+        b = int((f * fraction - p[1]) / p[0])  # y intercept (optimal batch size)
+        if None in results:  # some sizes failed
+            i = results.index(None)  # first fail index
+            if b >= batch_sizes[i]:  # y intercept above failure point
+                b = batch_sizes[max(i - 1, 0)]  # select prior safe point
+        if b < 1 or b > 1024:  # b outside of safe range
+            b = batch_size
+            LOGGER.info(f'{prefix}WARNING ⚠️ CUDA anomaly detected, using default batch-size {batch_size}.')
+
+        fraction = (np.polyval(p, b) + r + a) / t  # actual fraction predicted
+        LOGGER.info(f'{prefix}Using batch-size {b} for {d} {t * fraction:.2f}G/{t:.2f}G ({fraction * 100:.0f}%) ✅')
+        return b
+    except Exception as e:
+        LOGGER.warning(f'{prefix}WARNING ⚠️ error detected: {e},  using default batch-size {batch_size}.')
+        return batch_size
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/utils/checks.py` & `ultralytics-8.0.90/ultralytics/yolo/data/dataset.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,293 +1,247 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
-import glob
-import inspect
-import math
-import os
-import platform
-import shutil
-import urllib
+from itertools import repeat
+from multiprocessing.pool import ThreadPool
 from pathlib import Path
-from subprocess import check_output
-from typing import Optional
 
 import cv2
 import numpy as np
-import pkg_resources as pkg
-import psutil
 import torch
-from IPython import display
+import torchvision
+from tqdm import tqdm
 
-from ultralytics.yolo.utils import (AUTOINSTALL, FONT, LOGGER, ROOT, USER_CONFIG_DIR, TryExcept, colorstr, emojis,
-                                    is_colab, is_docker, is_jupyter_notebook)
+from ..utils import LOCAL_RANK, NUM_THREADS, TQDM_BAR_FORMAT, is_dir_writeable
+from .augment import Compose, Format, Instances, LetterBox, classify_albumentations, classify_transforms, v8_transforms
+from .base import BaseDataset
+from .utils import HELP_URL, LOGGER, get_hash, img2label_paths, verify_image_label
 
 
-def is_ascii(s) -> bool:
+class YOLODataset(BaseDataset):
     """
-    Check if a string is composed of only ASCII characters.
+    Dataset class for loading object detection and/or segmentation labels in YOLO format.
 
     Args:
-        s (str): String to be checked.
-
-    Returns:
-        bool: True if the string is composed only of ASCII characters, False otherwise.
-    """
-    # Convert list, tuple, None, etc. to string
-    s = str(s)
-
-    # Check if the string is composed of only ASCII characters
-    return all(ord(c) < 128 for c in s)
-
-
-def check_imgsz(imgsz, stride=32, min_dim=1, floor=0):
-    """
-    Verify image size is a multiple of the given stride in each dimension. If the image size is not a multiple of the
-    stride, update it to the nearest multiple of the stride that is greater than or equal to the given floor value.
-
-    Args:
-        imgsz (int or List[int]): Image size.
-        stride (int): Stride value.
-        min_dim (int): Minimum number of dimensions.
-        floor (int): Minimum allowed value for image size.
-
-    Returns:
-        List[int]: Updated image size.
-    """
-    # Convert stride to integer if it is a tensor
-    stride = int(stride.max() if isinstance(stride, torch.Tensor) else stride)
-
-    # Convert image size to list if it is an integer
-    if isinstance(imgsz, int):
-        imgsz = [imgsz]
-
-    # Make image size a multiple of the stride
-    sz = [max(math.ceil(x / stride) * stride, floor) for x in imgsz]
-
-    # Print warning message if image size was updated
-    if sz != imgsz:
-        LOGGER.warning(f'WARNING ⚠️ --img-size {imgsz} must be multiple of max stride {stride}, updating to {sz}')
-
-    # Add missing dimensions if necessary
-    sz = [sz[0], sz[0]] if min_dim == 2 and len(sz) == 1 else sz[0] if min_dim == 1 and len(sz) == 1 else sz
-
-    return sz
-
-
-def check_version(current: str = "0.0.0",
-                  minimum: str = "0.0.0",
-                  name: str = "version ",
-                  pinned: bool = False,
-                  hard: bool = False,
-                  verbose: bool = False) -> bool:
-    """
-    Check current version against the required minimum version.
-
-    Args:
-        current (str): Current version.
-        minimum (str): Required minimum version.
-        name (str): Name to be used in warning message.
-        pinned (bool): If True, versions must match exactly. If False, minimum version must be satisfied.
-        hard (bool): If True, raise an AssertionError if the minimum version is not met.
-        verbose (bool): If True, print warning message if minimum version is not met.
-
-    Returns:
-        bool: True if minimum version is met, False otherwise.
-    """
-    from pkg_resources import parse_version
-    current, minimum = (parse_version(x) for x in (current, minimum))
-    result = (current == minimum) if pinned else (current >= minimum)  # bool
-    warning_message = f"WARNING ⚠️ {name}{minimum} is required by YOLOv8, but {name}{current} is currently installed"
-    if hard:
-        assert result, emojis(warning_message)  # assert min requirements met
-    if verbose and not result:
-        LOGGER.warning(warning_message)
-    return result
-
-
-def check_font(font: str = FONT, progress: bool = False) -> None:
-    """
-    Download font file to the user's configuration directory if it does not already exist.
-
-    Args:
-        font (str): Path to font file.
-        progress (bool): If True, display a progress bar during the download.
-
-    Returns:
-        None
-    """
-    font = Path(font)
-
-    # Destination path for the font file
-    file = USER_CONFIG_DIR / font.name
-
-    # Check if font file exists at the source or destination path
-    if not font.exists() and not file.exists():
-        # Download font file
-        url = f'https://ultralytics.com/assets/{font.name}'
-        LOGGER.info(f'Downloading {url} to {file}...')
-        torch.hub.download_url_to_file(url, str(file), progress=progress)
-
-
-def check_online() -> bool:
-    """
-    Check internet connectivity by attempting to connect to a known online host.
-
-    Returns:
-        bool: True if connection is successful, False otherwise.
-    """
-    import socket
-    try:
-        # Check host accessibility by attempting to establish a connection
-        socket.create_connection(("1.1.1.1", 443), timeout=5)
-        return True
-    except OSError:
-        return False
-
-
-def check_python(minimum: str = '3.7.0') -> bool:
-    """
-    Check current python version against the required minimum version.
+        data (dict, optional): A dataset YAML dictionary. Defaults to None.
+        use_segments (bool, optional): If True, segmentation masks are used as labels. Defaults to False.
+        use_keypoints (bool, optional): If True, keypoints are used as labels. Defaults to False.
+
+    Returns:
+        (torch.utils.data.Dataset): A PyTorch dataset object that can be used for training an object detection model.
+    """
+    cache_version = '1.0.2'  # dataset labels *.cache version, >= 1.0.0 for YOLOv8
+    rand_interp_methods = [cv2.INTER_NEAREST, cv2.INTER_LINEAR, cv2.INTER_CUBIC, cv2.INTER_AREA, cv2.INTER_LANCZOS4]
+
+    def __init__(self, *args, data=None, use_segments=False, use_keypoints=False, **kwargs):
+        self.use_segments = use_segments
+        self.use_keypoints = use_keypoints
+        self.data = data
+        assert not (self.use_segments and self.use_keypoints), 'Can not use both segments and keypoints.'
+        super().__init__(*args, **kwargs)
+
+    def cache_labels(self, path=Path('./labels.cache')):
+        """Cache dataset labels, check images and read shapes.
+        Args:
+            path (Path): path where to save the cache file (default: Path('./labels.cache')).
+        Returns:
+            (dict): labels.
+        """
+        x = {'labels': []}
+        nm, nf, ne, nc, msgs = 0, 0, 0, 0, []  # number missing, found, empty, corrupt, messages
+        desc = f'{self.prefix}Scanning {path.parent / path.stem}...'
+        total = len(self.im_files)
+        nkpt, ndim = self.data.get('kpt_shape', (0, 0))
+        if self.use_keypoints and (nkpt <= 0 or ndim not in (2, 3)):
+            raise ValueError("'kpt_shape' in data.yaml missing or incorrect. Should be a list with [number of "
+                             "keypoints, number of dims (2 for x,y or 3 for x,y,visible)], i.e. 'kpt_shape: [17, 3]'")
+        with ThreadPool(NUM_THREADS) as pool:
+            results = pool.imap(func=verify_image_label,
+                                iterable=zip(self.im_files, self.label_files, repeat(self.prefix),
+                                             repeat(self.use_keypoints), repeat(len(self.data['names'])), repeat(nkpt),
+                                             repeat(ndim)))
+            pbar = tqdm(results, desc=desc, total=total, bar_format=TQDM_BAR_FORMAT)
+            for im_file, lb, shape, segments, keypoint, nm_f, nf_f, ne_f, nc_f, msg in pbar:
+                nm += nm_f
+                nf += nf_f
+                ne += ne_f
+                nc += nc_f
+                if im_file:
+                    x['labels'].append(
+                        dict(
+                            im_file=im_file,
+                            shape=shape,
+                            cls=lb[:, 0:1],  # n, 1
+                            bboxes=lb[:, 1:],  # n, 4
+                            segments=segments,
+                            keypoints=keypoint,
+                            normalized=True,
+                            bbox_format='xywh'))
+                if msg:
+                    msgs.append(msg)
+                pbar.desc = f'{desc} {nf} images, {nm + ne} backgrounds, {nc} corrupt'
+            pbar.close()
+
+        if msgs:
+            LOGGER.info('\n'.join(msgs))
+        if nf == 0:
+            LOGGER.warning(f'{self.prefix}WARNING ⚠️ No labels found in {path}. {HELP_URL}')
+        x['hash'] = get_hash(self.label_files + self.im_files)
+        x['results'] = nf, nm, ne, nc, len(self.im_files)
+        x['msgs'] = msgs  # warnings
+        x['version'] = self.cache_version  # cache version
+        if is_dir_writeable(path.parent):
+            if path.exists():
+                path.unlink()  # remove *.cache file if exists
+            np.save(str(path), x)  # save cache for next time
+            path.with_suffix('.cache.npy').rename(path)  # remove .npy suffix
+            LOGGER.info(f'{self.prefix}New cache created: {path}')
+        else:
+            LOGGER.warning(f'{self.prefix}WARNING ⚠️ Cache directory {path.parent} is not writeable, cache not saved.')
+        return x
 
-    Args:
-        minimum (str): Required minimum version of python.
+    def get_labels(self):
+        """Returns dictionary of labels for YOLO training."""
+        self.label_files = img2label_paths(self.im_files)
+        cache_path = Path(self.label_files[0]).parent.with_suffix('.cache')
+        try:
+            import gc
+            gc.disable()  # reduce pickle load time https://github.com/ultralytics/ultralytics/pull/1585
+            cache, exists = np.load(str(cache_path), allow_pickle=True).item(), True  # load dict
+            gc.enable()
+            assert cache['version'] == self.cache_version  # matches current version
+            assert cache['hash'] == get_hash(self.label_files + self.im_files)  # identical hash
+        except (FileNotFoundError, AssertionError, AttributeError):
+            cache, exists = self.cache_labels(cache_path), False  # run cache ops
+
+        # Display cache
+        nf, nm, ne, nc, n = cache.pop('results')  # found, missing, empty, corrupt, total
+        if exists and LOCAL_RANK in (-1, 0):
+            d = f'Scanning {cache_path}... {nf} images, {nm + ne} backgrounds, {nc} corrupt'
+            tqdm(None, desc=self.prefix + d, total=n, initial=n, bar_format=TQDM_BAR_FORMAT)  # display cache results
+            if cache['msgs']:
+                LOGGER.info('\n'.join(cache['msgs']))  # display warnings
+        if nf == 0:  # number of labels found
+            raise FileNotFoundError(f'{self.prefix}No labels found in {cache_path}, can not start training. {HELP_URL}')
+
+        # Read cache
+        [cache.pop(k) for k in ('hash', 'version', 'msgs')]  # remove items
+        labels = cache['labels']
+        self.im_files = [lb['im_file'] for lb in labels]  # update im_files
+
+        # Check if the dataset is all boxes or all segments
+        lengths = ((len(lb['cls']), len(lb['bboxes']), len(lb['segments'])) for lb in labels)
+        len_cls, len_boxes, len_segments = (sum(x) for x in zip(*lengths))
+        if len_segments and len_boxes != len_segments:
+            LOGGER.warning(
+                f'WARNING ⚠️ Box and segment counts should be equal, but got len(segments) = {len_segments}, '
+                f'len(boxes) = {len_boxes}. To resolve this only boxes will be used and all segments will be removed. '
+                'To avoid this please supply either a detect or segment dataset, not a detect-segment mixed dataset.')
+            for lb in labels:
+                lb['segments'] = []
+        if len_cls == 0:
+            raise ValueError(f'All labels empty in {cache_path}, can not start training without labels. {HELP_URL}')
+        return labels
+
+    # TODO: use hyp config to set all these augmentations
+    def build_transforms(self, hyp=None):
+        """Builds and appends transforms to the list."""
+        if self.augment:
+            hyp.mosaic = hyp.mosaic if self.augment and not self.rect else 0.0
+            hyp.mixup = hyp.mixup if self.augment and not self.rect else 0.0
+            transforms = v8_transforms(self, self.imgsz, hyp)
+        else:
+            transforms = Compose([LetterBox(new_shape=(self.imgsz, self.imgsz), scaleup=False)])
+        transforms.append(
+            Format(bbox_format='xywh',
+                   normalize=True,
+                   return_mask=self.use_segments,
+                   return_keypoint=self.use_keypoints,
+                   batch_idx=True,
+                   mask_ratio=hyp.mask_ratio,
+                   mask_overlap=hyp.overlap_mask))
+        return transforms
+
+    def close_mosaic(self, hyp):
+        """Sets mosaic, copy_paste and mixup options to 0.0 and builds transformations."""
+        hyp.mosaic = 0.0  # set mosaic ratio=0.0
+        hyp.copy_paste = 0.0  # keep the same behavior as previous v8 close-mosaic
+        hyp.mixup = 0.0  # keep the same behavior as previous v8 close-mosaic
+        self.transforms = self.build_transforms(hyp)
+
+    def update_labels_info(self, label):
+        """custom your label format here."""
+        # NOTE: cls is not with bboxes now, classification and semantic segmentation need an independent cls label
+        # we can make it also support classification and semantic segmentation by add or remove some dict keys there.
+        bboxes = label.pop('bboxes')
+        segments = label.pop('segments')
+        keypoints = label.pop('keypoints', None)
+        bbox_format = label.pop('bbox_format')
+        normalized = label.pop('normalized')
+        label['instances'] = Instances(bboxes, segments, keypoints, bbox_format=bbox_format, normalized=normalized)
+        return label
+
+    @staticmethod
+    def collate_fn(batch):
+        """Collates data samples into batches."""
+        new_batch = {}
+        keys = batch[0].keys()
+        values = list(zip(*[list(b.values()) for b in batch]))
+        for i, k in enumerate(keys):
+            value = values[i]
+            if k == 'img':
+                value = torch.stack(value, 0)
+            if k in ['masks', 'keypoints', 'bboxes', 'cls']:
+                value = torch.cat(value, 0)
+            new_batch[k] = value
+        new_batch['batch_idx'] = list(new_batch['batch_idx'])
+        for i in range(len(new_batch['batch_idx'])):
+            new_batch['batch_idx'][i] += i  # add target image index for build_targets()
+        new_batch['batch_idx'] = torch.cat(new_batch['batch_idx'], 0)
+        return new_batch
+
+
+# Classification dataloaders -------------------------------------------------------------------------------------------
+class ClassificationDataset(torchvision.datasets.ImageFolder):
+    """
+    YOLOv5 Classification Dataset.
+    Arguments
+        root:  Dataset path
+        transform:  torchvision transforms, used by default
+        album_transform: Albumentations transforms, used if installed
+    """
+
+    def __init__(self, root, augment, imgsz, cache=False):
+        """Initialize YOLO object with root, image size, augmentations, and cache settings"""
+        super().__init__(root=root)
+        self.torch_transforms = classify_transforms(imgsz)
+        self.album_transforms = classify_albumentations(augment, imgsz) if augment else None
+        self.cache_ram = cache is True or cache == 'ram'
+        self.cache_disk = cache == 'disk'
+        self.samples = [list(x) + [Path(x[0]).with_suffix('.npy'), None] for x in self.samples]  # file, index, npy, im
+
+    def __getitem__(self, i):
+        """Returns subset of data and targets corresponding to given indices."""
+        f, j, fn, im = self.samples[i]  # filename, index, filename.with_suffix('.npy'), image
+        if self.cache_ram and im is None:
+            im = self.samples[i][3] = cv2.imread(f)
+        elif self.cache_disk:
+            if not fn.exists():  # load npy
+                np.save(fn.as_posix(), cv2.imread(f))
+            im = np.load(fn)
+        else:  # read image
+            im = cv2.imread(f)  # BGR
+        if self.album_transforms:
+            sample = self.album_transforms(image=cv2.cvtColor(im, cv2.COLOR_BGR2RGB))['image']
+        else:
+            sample = self.torch_transforms(im)
+        return {'img': sample, 'cls': j}
 
-    Returns:
-        None
-    """
-    check_version(platform.python_version(), minimum, name='Python ', hard=True)
+    def __len__(self) -> int:
+        return len(self.samples)
 
 
-@TryExcept()
-def check_requirements(requirements=ROOT.parent / 'requirements.txt', exclude=(), install=True, cmds=''):
-    # Check installed dependencies meet YOLOv5 requirements (pass *.txt file or list of packages or single package str)
-    prefix = colorstr('red', 'bold', 'requirements:')
-    check_python()  # check python version
-    if isinstance(requirements, Path):  # requirements.txt file
-        file = requirements.resolve()
-        assert file.exists(), f"{prefix} {file} not found, check failed."
-        with file.open() as f:
-            requirements = [f'{x.name}{x.specifier}' for x in pkg.parse_requirements(f) if x.name not in exclude]
-    elif isinstance(requirements, str):
-        requirements = [requirements]
-
-    s = ''
-    n = 0
-    for r in requirements:
-        try:
-            pkg.require(r)
-        except (pkg.VersionConflict, pkg.DistributionNotFound):  # exception if requirements not met
-            s += f'"{r}" '
-            n += 1
+# TODO: support semantic segmentation
+class SemanticDataset(BaseDataset):
 
-    if s and install and AUTOINSTALL:  # check environment variable
-        LOGGER.info(f"{prefix} YOLOv8 requirement{'s' * (n > 1)} {s}not found, attempting AutoUpdate...")
-        try:
-            assert check_online(), "AutoUpdate skipped (offline)"
-            LOGGER.info(check_output(f'pip install {s} {cmds}', shell=True).decode())
-            source = file if 'file' in locals() else requirements
-            s = f"{prefix} {n} package{'s' * (n > 1)} updated per {source}\n" \
-                f"{prefix} ⚠️ {colorstr('bold', 'Restart runtime or rerun command for updates to take effect')}\n"
-            LOGGER.info(s)
-        except Exception as e:
-            LOGGER.warning(f'{prefix} ❌ {e}')
-
-
-def check_suffix(file='yolov8n.pt', suffix=('.pt',), msg=''):
-    # Check file(s) for acceptable suffix
-    if file and suffix:
-        if isinstance(suffix, str):
-            suffix = [suffix]
-        for f in file if isinstance(file, (list, tuple)) else [file]:
-            s = Path(f).suffix.lower()  # file suffix
-            if len(s):
-                assert s in suffix, f"{msg}{f} acceptable suffix is {suffix}"
-
-
-def check_file(file, suffix=''):
-    # Search/download file (if necessary) and return path
-    check_suffix(file, suffix)  # optional
-    file = str(file)  # convert to str()
-    if Path(file).is_file() or not file:  # exists
-        return file
-    elif file.startswith(('http:/', 'https:/')):  # download
-        url = file  # warning: Pathlib turns :// -> :/
-        file = Path(urllib.parse.unquote(file).split('?')[0]).name  # '%2F' to '/', split https://url.com/file.txt?auth
-        if Path(file).is_file():
-            LOGGER.info(f'Found {url} locally at {file}')  # file already exists
-        else:
-            LOGGER.info(f'Downloading {url} to {file}...')
-            torch.hub.download_url_to_file(url, file)
-            assert Path(file).exists() and Path(file).stat().st_size > 0, f'File download failed: {url}'  # check
-        return file
-    else:  # search
-        files = []
-        for d in 'models', 'yolo/data':  # search directories
-            files.extend(glob.glob(str(ROOT / d / '**' / file), recursive=True))  # find file
-        assert len(files), f'File not found: {file}'  # assert file was found
-        assert len(files) == 1, f"Multiple files match '{file}', specify exact path: {files}"  # assert unique
-        return files[0]  # return file
-
-
-def check_yaml(file, suffix=('.yaml', '.yml')):
-    # Search/download YAML file (if necessary) and return path, checking suffix
-    return check_file(file, suffix)
-
-
-def check_imshow(warn=False):
-    # Check if environment supports image displays
-    try:
-        assert not is_jupyter_notebook()
-        assert not is_docker()
-        cv2.imshow('test', np.zeros((1, 1, 3)))
-        cv2.waitKey(1)
-        cv2.destroyAllWindows()
-        cv2.waitKey(1)
-        return True
-    except Exception as e:
-        if warn:
-            LOGGER.warning(f'WARNING ⚠️ Environment does not support cv2.imshow() or PIL Image.show()\n{e}')
-        return False
-
-
-def check_yolo(verbose=True):
-    from ultralytics.yolo.utils.torch_utils import select_device
-
-    if is_colab():
-        shutil.rmtree('sample_data', ignore_errors=True)  # remove colab /sample_data directory
-
-    if verbose:
-        # System info
-        gib = 1 << 30  # bytes per GiB
-        ram = psutil.virtual_memory().total
-        total, used, free = shutil.disk_usage("/")
-        display.clear_output()
-        s = f'({os.cpu_count()} CPUs, {ram / gib:.1f} GB RAM, {(total - free) / gib:.1f}/{total / gib:.1f} GB disk)'
-    else:
-        s = ''
-
-    select_device(newline=False)
-    LOGGER.info(f'Setup complete ✅ {s}')
-
-
-def git_describe(path=ROOT):  # path must be a directory
-    # Return human-readable git description, i.e. v5.0-5-g3e25f1e https://git-scm.com/docs/git-describe
-    try:
-        assert (Path(path) / '.git').is_dir()
-        return check_output(f'git -C {path} describe --tags --long --always', shell=True).decode()[:-1]
-    except Exception:
-        return ''
-
-
-def print_args(args: Optional[dict] = None, show_file=True, show_func=False):
-    # Print function arguments (optional args dict)
-    x = inspect.currentframe().f_back  # previous frame
-    file, _, func, _, _ = inspect.getframeinfo(x)
-    if args is None:  # get args automatically
-        args, _, _, frm = inspect.getargvalues(x)
-        args = {k: v for k, v in frm.items() if k in args}
-    try:
-        file = Path(file).resolve().relative_to(ROOT).with_suffix('')
-    except ValueError:
-        file = Path(file).stem
-    s = (f'{file}: ' if show_file else '') + (f'{func}: ' if show_func else '')
-    LOGGER.info(colorstr(s) + ', '.join(f'{k}={v}' for k, v in args.items()))
+    def __init__(self):
+        """Initialize a SemanticDataset object."""
+        pass
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/utils/files.py` & `ultralytics-8.0.90/ultralytics/yolo/utils/files.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import contextlib
 import glob
 import os
-import urllib
 from datetime import datetime
 from pathlib import Path
-from zipfile import ZipFile
 
 
 class WorkingDirectory(contextlib.ContextDecorator):
-    # Usage: @WorkingDirectory(dir) decorator or 'with WorkingDirectory(dir):' context manager
+    """Usage: @WorkingDirectory(dir) decorator or 'with WorkingDirectory(dir):' context manager."""
+
     def __init__(self, new_dir):
+        """Sets the working directory to 'new_dir' upon instantiation."""
         self.dir = new_dir  # new dir
         self.cwd = Path.cwd().resolve()  # current dir
 
     def __enter__(self):
+        """Changes the current directory to the specified directory."""
         os.chdir(self.dir)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
+        """Restore the current working directory on context exit."""
         os.chdir(self.cwd)
 
 
 def increment_path(path, exist_ok=False, sep='', mkdir=False):
     """
     Increments a file or directory path, i.e. runs/exp --> runs/exp{sep}2, runs/exp{sep}3, ... etc.
 
     If the path exists and exist_ok is not set to True, the path will be incremented by appending a number and sep to
     the end of the path. If the path is a file, the file extension will be preserved. If the path is a directory, the
     number will be appended directly to the end of the path. If mkdir is set to True, the path will be created as a
     directory if it does not already exist.
 
     Args:
-    path (str or pathlib.Path): Path to increment.
-    exist_ok (bool, optional): If True, the path will not be incremented and will be returned as-is. Defaults to False.
-    sep (str, optional): Separator to use between the path and the incrementation number. Defaults to an empty string.
-    mkdir (bool, optional): If True, the path will be created as a directory if it does not exist. Defaults to False.
+        path (str, pathlib.Path): Path to increment.
+        exist_ok (bool, optional): If True, the path will not be incremented and returned as-is. Defaults to False.
+        sep (str, optional): Separator to use between the path and the incrementation number. Defaults to ''.
+        mkdir (bool, optional): Create a directory if it does not exist. Defaults to False.
 
     Returns:
-    pathlib.Path: Incremented path.
+        (pathlib.Path): Incremented path.
     """
     path = Path(path)  # os-agnostic
     if path.exists() and not exist_ok:
         path, suffix = (path.with_suffix(''), path.suffix) if path.is_file() else (path, '')
 
         # Method 1
         for n in range(2, 9999):
@@ -53,51 +55,35 @@
 
     if mkdir:
         path.mkdir(parents=True, exist_ok=True)  # make directory
 
     return path
 
 
-def unzip_file(file, path=None, exclude=('.DS_Store', '__MACOSX')):
-    # Unzip a *.zip file to path/, excluding files containing strings in exclude list
-    if path is None:
-        path = Path(file).parent  # default path
-    with ZipFile(file) as zipObj:
-        for f in zipObj.namelist():  # list all archived filenames in the zip
-            if all(x not in f for x in exclude):
-                zipObj.extract(f, path=path)
-
-
 def file_age(path=__file__):
-    # Return days since last file update
+    """Return days since last file update."""
     dt = (datetime.now() - datetime.fromtimestamp(Path(path).stat().st_mtime))  # delta
     return dt.days  # + dt.seconds / 86400  # fractional days
 
 
 def file_date(path=__file__):
-    # Return human-readable file modification date, i.e. '2021-3-26'
+    """Return human-readable file modification date, i.e. '2021-3-26'."""
     t = datetime.fromtimestamp(Path(path).stat().st_mtime)
     return f'{t.year}-{t.month}-{t.day}'
 
 
 def file_size(path):
-    # Return file/dir size (MB)
-    mb = 1 << 20  # bytes to MiB (1024 ** 2)
-    path = Path(path)
-    if path.is_file():
-        return path.stat().st_size / mb
-    elif path.is_dir():
-        return sum(f.stat().st_size for f in path.glob('**/*') if f.is_file()) / mb
-    else:
-        return 0.0
-
-
-def url2file(url):
-    # Convert URL to filename, i.e. https://url.com/file.txt?auth -> file.txt
-    url = str(Path(url)).replace(':/', '://')  # Pathlib turns :// -> :/
-    return Path(urllib.parse.unquote(url)).name.split('?')[0]  # '%2F' to '/', split https://url.com/file.txt?auth
+    """Return file/dir size (MB)."""
+    if isinstance(path, (str, Path)):
+        mb = 1 << 20  # bytes to MiB (1024 ** 2)
+        path = Path(path)
+        if path.is_file():
+            return path.stat().st_size / mb
+        elif path.is_dir():
+            return sum(f.stat().st_size for f in path.glob('**/*') if f.is_file()) / mb
+    return 0.0
 
 
 def get_latest_run(search_dir='.'):
-    # Return path to most recent 'last.pt' in /runs (i.e. to --resume from)
+    """Return path to most recent 'last.pt' in /runs (i.e. to --resume from)."""
     last_list = glob.glob(f'{search_dir}/**/last*.pt', recursive=True)
     return max(last_list, key=os.path.getctime) if last_list else ''
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/utils/instance.py` & `ultralytics-8.0.90/ultralytics/yolo/utils/instance.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
 from collections import abc
 from itertools import repeat
 from numbers import Number
 from typing import List
 
 import numpy as np
 
 from .ops import ltwh2xywh, ltwh2xyxy, resample_segments, xywh2ltwh, xywh2xyxy, xyxy2ltwh, xyxy2xywh
 
 
-# From PyTorch internals
 def _ntuple(n):
+    """From PyTorch internals."""
 
     def parse(x):
+        """Parse bounding boxes format between XYWH and LTWH."""
         return x if isinstance(x, abc.Iterable) else tuple(repeat(x, n))
 
     return parse
 
 
 to_4tuple = _ntuple(4)
 
 # `xyxy` means left top and right bottom
 # `xywh` means center x, center y and width, height(yolo format)
 # `ltwh` means left top and width, height(coco format)
-_formats = ["xyxy", "xywh", "ltwh"]
+_formats = ['xyxy', 'xywh', 'ltwh']
 
-__all__ = ["Bboxes"]
+__all__ = 'Bboxes',  # tuple or list
 
 
 class Bboxes:
-    """Now only numpy is supported"""
+    """Now only numpy is supported."""
 
-    def __init__(self, bboxes, format="xyxy") -> None:
-        assert format in _formats
+    def __init__(self, bboxes, format='xyxy') -> None:
+        assert format in _formats, f'Invalid bounding box format: {format}, format must be one of {_formats}'
         bboxes = bboxes[None, :] if bboxes.ndim == 1 else bboxes
         assert bboxes.ndim == 2
         assert bboxes.shape[1] == 4
         self.bboxes = bboxes
         self.format = format
         # self.normalized = normalized
 
@@ -60,32 +61,34 @@
     #             bboxes = ltwh2xyxy(self.bboxes)
     #         else:
     #             bboxes = ltwh2xywh(self.bboxes)
     #
     #     return Bboxes(bboxes, format)
 
     def convert(self, format):
-        assert format in _formats
+        """Converts bounding box format from one type to another."""
+        assert format in _formats, f'Invalid bounding box format: {format}, format must be one of {_formats}'
         if self.format == format:
             return
-        elif self.format == "xyxy":
-            bboxes = xyxy2xywh(self.bboxes) if format == "xywh" else xyxy2ltwh(self.bboxes)
-        elif self.format == "xywh":
-            bboxes = xywh2xyxy(self.bboxes) if format == "xyxy" else xywh2ltwh(self.bboxes)
+        elif self.format == 'xyxy':
+            bboxes = xyxy2xywh(self.bboxes) if format == 'xywh' else xyxy2ltwh(self.bboxes)
+        elif self.format == 'xywh':
+            bboxes = xywh2xyxy(self.bboxes) if format == 'xyxy' else xywh2ltwh(self.bboxes)
         else:
-            bboxes = ltwh2xyxy(self.bboxes) if format == "xyxy" else ltwh2xywh(self.bboxes)
+            bboxes = ltwh2xyxy(self.bboxes) if format == 'xyxy' else ltwh2xywh(self.bboxes)
         self.bboxes = bboxes
         self.format = format
 
     def areas(self):
-        self.convert("xyxy")
+        """Return box areas."""
+        self.convert('xyxy')
         return (self.bboxes[:, 2] - self.bboxes[:, 0]) * (self.bboxes[:, 3] - self.bboxes[:, 1])
 
     # def denormalize(self, w, h):
-    #     if not self.normalized:
+    #    if not self.normalized:
     #         return
     #     assert (self.bboxes <= 1.0).all()
     #     self.bboxes[:, 0::2] *= w
     #     self.bboxes[:, 1::2] *= h
     #     self.normalized = False
     #
     # def normalize(self, w, h):
@@ -95,85 +98,101 @@
     #     self.bboxes[:, 0::2] /= w
     #     self.bboxes[:, 1::2] /= h
     #     self.normalized = True
 
     def mul(self, scale):
         """
         Args:
-            scale (tuple | List | int): the scale for four coords.
+            scale (tuple) or (list) or (int): the scale for four coords.
         """
         if isinstance(scale, Number):
             scale = to_4tuple(scale)
         assert isinstance(scale, (tuple, list))
         assert len(scale) == 4
         self.bboxes[:, 0] *= scale[0]
         self.bboxes[:, 1] *= scale[1]
         self.bboxes[:, 2] *= scale[2]
         self.bboxes[:, 3] *= scale[3]
 
     def add(self, offset):
         """
         Args:
-            offset (tuple | List | int): the offset for four coords.
+            offset (tuple) or (list) or (int): the offset for four coords.
         """
         if isinstance(offset, Number):
             offset = to_4tuple(offset)
         assert isinstance(offset, (tuple, list))
         assert len(offset) == 4
         self.bboxes[:, 0] += offset[0]
         self.bboxes[:, 1] += offset[1]
         self.bboxes[:, 2] += offset[2]
         self.bboxes[:, 3] += offset[3]
 
     def __len__(self):
+        """Return the number of boxes."""
         return len(self.bboxes)
 
     @classmethod
-    def concatenate(cls, boxes_list: List["Bboxes"], axis=0) -> "Bboxes":
+    def concatenate(cls, boxes_list: List['Bboxes'], axis=0) -> 'Bboxes':
         """
-        Concatenates a list of Boxes into a single Bboxes
+        Concatenate a list of Bboxes objects into a single Bboxes object.
 
-        Arguments:
-            boxes_list (list[Bboxes])
+        Args:
+            boxes_list (List[Bboxes]): A list of Bboxes objects to concatenate.
+            axis (int, optional): The axis along which to concatenate the bounding boxes.
+                                   Defaults to 0.
 
         Returns:
-            Bboxes: the concatenated Boxes
+            Bboxes: A new Bboxes object containing the concatenated bounding boxes.
+
+        Note:
+            The input should be a list or tuple of Bboxes objects.
         """
         assert isinstance(boxes_list, (list, tuple))
         if not boxes_list:
             return cls(np.empty(0))
         assert all(isinstance(box, Bboxes) for box in boxes_list)
 
         if len(boxes_list) == 1:
             return boxes_list[0]
         return cls(np.concatenate([b.bboxes for b in boxes_list], axis=axis))
 
-    def __getitem__(self, index) -> "Bboxes":
+    def __getitem__(self, index) -> 'Bboxes':
         """
+        Retrieve a specific bounding box or a set of bounding boxes using indexing.
+
         Args:
-            index: int, slice, or a BoolArray
+            index (int, slice, or np.ndarray): The index, slice, or boolean array to select
+                                               the desired bounding boxes.
 
         Returns:
-            Bboxes: Create a new :class:`Bboxes` by indexing.
+            Bboxes: A new Bboxes object containing the selected bounding boxes.
+
+        Raises:
+            AssertionError: If the indexed bounding boxes do not form a 2-dimensional matrix.
+
+        Note:
+            When using boolean indexing, make sure to provide a boolean array with the same
+            length as the number of bounding boxes.
         """
         if isinstance(index, int):
             return Bboxes(self.bboxes[index].view(1, -1))
         b = self.bboxes[index]
-        assert b.ndim == 2, f"Indexing on Bboxes with {index} failed to return a matrix!"
+        assert b.ndim == 2, f'Indexing on Bboxes with {index} failed to return a matrix!'
         return Bboxes(b)
 
 
 class Instances:
 
-    def __init__(self, bboxes, segments=None, keypoints=None, bbox_format="xywh", normalized=True) -> None:
+    def __init__(self, bboxes, segments=None, keypoints=None, bbox_format='xywh', normalized=True) -> None:
         """
         Args:
             bboxes (ndarray): bboxes with shape [N, 4].
             segments (list | ndarray): segments.
-            keypoints (ndarray): keypoints with shape [N, 17, 2].
+            keypoints (ndarray): keypoints(x, y, visible) with shape [N, 17, 3].
         """
         if segments is None:
             segments = []
         self._bboxes = Bboxes(bboxes=bboxes, format=bbox_format)
         self.keypoints = keypoints
         self.normalized = normalized
 
@@ -183,141 +202,164 @@
             # (N, 1000, 2)
             segments = np.stack(segments, axis=0)
         else:
             segments = np.zeros((0, 1000, 2), dtype=np.float32)
         self.segments = segments
 
     def convert_bbox(self, format):
+        """Convert bounding box format."""
         self._bboxes.convert(format=format)
 
     def bbox_areas(self):
+        """Calculate the area of bounding boxes."""
         self._bboxes.areas()
 
     def scale(self, scale_w, scale_h, bbox_only=False):
-        """this might be similar with denormalize func but without normalized sign"""
+        """this might be similar with denormalize func but without normalized sign."""
         self._bboxes.mul(scale=(scale_w, scale_h, scale_w, scale_h))
         if bbox_only:
             return
         self.segments[..., 0] *= scale_w
         self.segments[..., 1] *= scale_h
         if self.keypoints is not None:
             self.keypoints[..., 0] *= scale_w
             self.keypoints[..., 1] *= scale_h
 
     def denormalize(self, w, h):
+        """Denormalizes boxes, segments, and keypoints from normalized coordinates."""
         if not self.normalized:
             return
         self._bboxes.mul(scale=(w, h, w, h))
         self.segments[..., 0] *= w
         self.segments[..., 1] *= h
         if self.keypoints is not None:
             self.keypoints[..., 0] *= w
             self.keypoints[..., 1] *= h
         self.normalized = False
 
     def normalize(self, w, h):
+        """Normalize bounding boxes, segments, and keypoints to image dimensions."""
         if self.normalized:
             return
         self._bboxes.mul(scale=(1 / w, 1 / h, 1 / w, 1 / h))
         self.segments[..., 0] /= w
         self.segments[..., 1] /= h
         if self.keypoints is not None:
             self.keypoints[..., 0] /= w
             self.keypoints[..., 1] /= h
         self.normalized = True
 
     def add_padding(self, padw, padh):
-        # handle rect and mosaic situation
-        assert not self.normalized, "you should add padding with absolute coordinates."
+        """Handle rect and mosaic situation."""
+        assert not self.normalized, 'you should add padding with absolute coordinates.'
         self._bboxes.add(offset=(padw, padh, padw, padh))
         self.segments[..., 0] += padw
         self.segments[..., 1] += padh
         if self.keypoints is not None:
             self.keypoints[..., 0] += padw
             self.keypoints[..., 1] += padh
 
-    def __getitem__(self, index) -> "Instances":
+    def __getitem__(self, index) -> 'Instances':
         """
+        Retrieve a specific instance or a set of instances using indexing.
+
         Args:
-            index: int, slice, or a BoolArray
+            index (int, slice, or np.ndarray): The index, slice, or boolean array to select
+                                               the desired instances.
 
         Returns:
-            Instances: Create a new :class:`Instances` by indexing.
+            Instances: A new Instances object containing the selected bounding boxes,
+                       segments, and keypoints if present.
+
+        Note:
+            When using boolean indexing, make sure to provide a boolean array with the same
+            length as the number of instances.
         """
         segments = self.segments[index] if len(self.segments) else self.segments
         keypoints = self.keypoints[index] if self.keypoints is not None else None
         bboxes = self.bboxes[index]
         bbox_format = self._bboxes.format
         return Instances(
             bboxes=bboxes,
             segments=segments,
             keypoints=keypoints,
             bbox_format=bbox_format,
             normalized=self.normalized,
         )
 
     def flipud(self, h):
-        if self._bboxes.format == "xyxy":
+        """Flips the coordinates of bounding boxes, segments, and keypoints vertically."""
+        if self._bboxes.format == 'xyxy':
             y1 = self.bboxes[:, 1].copy()
             y2 = self.bboxes[:, 3].copy()
             self.bboxes[:, 1] = h - y2
             self.bboxes[:, 3] = h - y1
         else:
             self.bboxes[:, 1] = h - self.bboxes[:, 1]
         self.segments[..., 1] = h - self.segments[..., 1]
         if self.keypoints is not None:
             self.keypoints[..., 1] = h - self.keypoints[..., 1]
 
     def fliplr(self, w):
-        if self._bboxes.format == "xyxy":
+        """Reverses the order of the bounding boxes and segments horizontally."""
+        if self._bboxes.format == 'xyxy':
             x1 = self.bboxes[:, 0].copy()
             x2 = self.bboxes[:, 2].copy()
             self.bboxes[:, 0] = w - x2
             self.bboxes[:, 2] = w - x1
         else:
             self.bboxes[:, 0] = w - self.bboxes[:, 0]
         self.segments[..., 0] = w - self.segments[..., 0]
         if self.keypoints is not None:
             self.keypoints[..., 0] = w - self.keypoints[..., 0]
 
     def clip(self, w, h):
+        """Clips bounding boxes, segments, and keypoints values to stay within image boundaries."""
         ori_format = self._bboxes.format
-        self.convert_bbox(format="xyxy")
+        self.convert_bbox(format='xyxy')
         self.bboxes[:, [0, 2]] = self.bboxes[:, [0, 2]].clip(0, w)
         self.bboxes[:, [1, 3]] = self.bboxes[:, [1, 3]].clip(0, h)
-        if ori_format != "xyxy":
+        if ori_format != 'xyxy':
             self.convert_bbox(format=ori_format)
         self.segments[..., 0] = self.segments[..., 0].clip(0, w)
         self.segments[..., 1] = self.segments[..., 1].clip(0, h)
         if self.keypoints is not None:
             self.keypoints[..., 0] = self.keypoints[..., 0].clip(0, w)
             self.keypoints[..., 1] = self.keypoints[..., 1].clip(0, h)
 
     def update(self, bboxes, segments=None, keypoints=None):
+        """Updates instance variables."""
         new_bboxes = Bboxes(bboxes, format=self._bboxes.format)
         self._bboxes = new_bboxes
         if segments is not None:
             self.segments = segments
         if keypoints is not None:
             self.keypoints = keypoints
 
     def __len__(self):
+        """Return the length of the instance list."""
         return len(self.bboxes)
 
     @classmethod
-    def concatenate(cls, instances_list: List["Instances"], axis=0) -> "Instances":
+    def concatenate(cls, instances_list: List['Instances'], axis=0) -> 'Instances':
         """
-        Concatenates a list of Boxes into a single Bboxes
+        Concatenates a list of Instances objects into a single Instances object.
 
-        Arguments:
-            instances_list (list[Bboxes])
-            axis
+        Args:
+            instances_list (List[Instances]): A list of Instances objects to concatenate.
+            axis (int, optional): The axis along which the arrays will be concatenated. Defaults to 0.
 
         Returns:
-            Boxes: the concatenated Boxes
+            Instances: A new Instances object containing the concatenated bounding boxes,
+                       segments, and keypoints if present.
+
+        Note:
+            The `Instances` objects in the list should have the same properties, such as
+            the format of the bounding boxes, whether keypoints are present, and if the
+            coordinates are normalized.
         """
         assert isinstance(instances_list, (list, tuple))
         if not instances_list:
             return cls(np.empty(0))
         assert all(isinstance(instance, Instances) for instance in instances_list)
 
         if len(instances_list) == 1:
@@ -330,8 +372,9 @@
         cat_boxes = np.concatenate([ins.bboxes for ins in instances_list], axis=axis)
         cat_segments = np.concatenate([b.segments for b in instances_list], axis=axis)
         cat_keypoints = np.concatenate([b.keypoints for b in instances_list], axis=axis) if use_keypoint else None
         return cls(cat_boxes, cat_segments, cat_keypoints, bbox_format, normalized)
 
     @property
     def bboxes(self):
+        """Return bounding boxes."""
         return self._bboxes.bboxes
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/utils/metrics.py` & `ultralytics-8.0.90/ultralytics/yolo/utils/plotting.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,617 +1,507 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
-"""
-Model validation metrics
-"""
+# Ultralytics YOLO 🚀, AGPL-3.0 license
+
+import contextlib
 import math
-import warnings
 from pathlib import Path
 
+import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
-import torch.nn as nn
-
-from ultralytics.yolo.utils import TryExcept
-
-
-# boxes
-def box_area(box):
-    # box = xyxy(4,n)
-    return (box[2] - box[0]) * (box[3] - box[1])
-
-
-def bbox_ioa(box1, box2, eps=1e-7):
-    """Returns the intersection over box2 area given box1, box2. Boxes are x1y1x2y2
-    box1:       np.array of shape(nx4)
-    box2:       np.array of shape(mx4)
-    returns:    np.array of shape(nxm)
-    """
+from PIL import Image, ImageDraw, ImageFont
+from PIL import __version__ as pil_version
 
-    # Get the coordinates of bounding boxes
-    b1_x1, b1_y1, b1_x2, b1_y2 = box1.T
-    b2_x1, b2_y1, b2_x2, b2_y2 = box2.T
+from ultralytics.yolo.utils import LOGGER, TryExcept, plt_settings, threaded
 
-    # Intersection area
-    inter_area = (np.minimum(b1_x2[:, None], b2_x2) - np.maximum(b1_x1[:, None], b2_x1)).clip(0) * \
-                 (np.minimum(b1_y2[:, None], b2_y2) - np.maximum(b1_y1[:, None], b2_y1)).clip(0)
+from .checks import check_font, check_version, is_ascii
+from .files import increment_path
+from .ops import clip_boxes, scale_image, xywh2xyxy, xyxy2xywh
+
+
+class Colors:
+    # Ultralytics color palette https://ultralytics.com/
+    def __init__(self):
+        """Initialize colors as hex = matplotlib.colors.TABLEAU_COLORS.values()."""
+        hexs = ('FF3838', 'FF9D97', 'FF701F', 'FFB21D', 'CFD231', '48F90A', '92CC17', '3DDB86', '1A9334', '00D4BB',
+                '2C99A8', '00C2FF', '344593', '6473FF', '0018EC', '8438FF', '520085', 'CB38FF', 'FF95C8', 'FF37C7')
+        self.palette = [self.hex2rgb(f'#{c}') for c in hexs]
+        self.n = len(self.palette)
+        self.pose_palette = np.array([[255, 128, 0], [255, 153, 51], [255, 178, 102], [230, 230, 0], [255, 153, 255],
+                                      [153, 204, 255], [255, 102, 255], [255, 51, 255], [102, 178, 255], [51, 153, 255],
+                                      [255, 153, 153], [255, 102, 102], [255, 51, 51], [153, 255, 153], [102, 255, 102],
+                                      [51, 255, 51], [0, 255, 0], [0, 0, 255], [255, 0, 0], [255, 255, 255]],
+                                     dtype=np.uint8)
+
+    def __call__(self, i, bgr=False):
+        """Converts hex color codes to rgb values."""
+        c = self.palette[int(i) % self.n]
+        return (c[2], c[1], c[0]) if bgr else c
+
+    @staticmethod
+    def hex2rgb(h):  # rgb order (PIL)
+        return tuple(int(h[1 + i:1 + i + 2], 16) for i in (0, 2, 4))
+
+
+colors = Colors()  # create instance for 'from utils.plots import colors'
+
+
+class Annotator:
+    # YOLOv8 Annotator for train/val mosaics and jpgs and detect/hub inference annotations
+    def __init__(self, im, line_width=None, font_size=None, font='Arial.ttf', pil=False, example='abc'):
+        """Initialize the Annotator class with image and line width along with color palette for keypoints and limbs."""
+        assert im.data.contiguous, 'Image not contiguous. Apply np.ascontiguousarray(im) to Annotator() input images.'
+        non_ascii = not is_ascii(example)  # non-latin labels, i.e. asian, arabic, cyrillic
+        self.pil = pil or non_ascii
+        if self.pil:  # use PIL
+            self.pil_9_2_0_check = check_version(pil_version, '9.2.0')  # deprecation check
+            self.im = im if isinstance(im, Image.Image) else Image.fromarray(im)
+            self.draw = ImageDraw.Draw(self.im)
+            try:
+                font = check_font('Arial.Unicode.ttf' if non_ascii else font)
+                size = font_size or max(round(sum(self.im.size) / 2 * 0.035), 12)
+                self.font = ImageFont.truetype(str(font), size)
+            except Exception:
+                self.font = ImageFont.load_default()
+        else:  # use cv2
+            self.im = im
+        self.lw = line_width or max(round(sum(im.shape) / 2 * 0.003), 2)  # line width
+        # Pose
+        self.skeleton = [[16, 14], [14, 12], [17, 15], [15, 13], [12, 13], [6, 12], [7, 13], [6, 7], [6, 8], [7, 9],
+                         [8, 10], [9, 11], [2, 3], [1, 2], [1, 3], [2, 4], [3, 5], [4, 6], [5, 7]]
+
+        self.limb_color = colors.pose_palette[[9, 9, 9, 9, 7, 7, 7, 0, 0, 0, 0, 0, 16, 16, 16, 16, 16, 16, 16]]
+        self.kpt_color = colors.pose_palette[[16, 16, 16, 16, 16, 0, 0, 0, 0, 0, 0, 9, 9, 9, 9, 9, 9]]
+
+    def box_label(self, box, label='', color=(128, 128, 128), txt_color=(255, 255, 255)):
+        """Add one xyxy box to image with label."""
+        if isinstance(box, torch.Tensor):
+            box = box.tolist()
+        if self.pil or not is_ascii(label):
+            self.draw.rectangle(box, width=self.lw, outline=color)  # box
+            if label:
+                if self.pil_9_2_0_check:
+                    _, _, w, h = self.font.getbbox(label)  # text width, height (New)
+                else:
+                    w, h = self.font.getsize(label)  # text width, height (Old, deprecated in 9.2.0)
+                outside = box[1] - h >= 0  # label fits outside box
+                self.draw.rectangle(
+                    (box[0], box[1] - h if outside else box[1], box[0] + w + 1,
+                     box[1] + 1 if outside else box[1] + h + 1),
+                    fill=color,
+                )
+                # self.draw.text((box[0], box[1]), label, fill=txt_color, font=self.font, anchor='ls')  # for PIL>8.0
+                self.draw.text((box[0], box[1] - h if outside else box[1]), label, fill=txt_color, font=self.font)
+        else:  # cv2
+            p1, p2 = (int(box[0]), int(box[1])), (int(box[2]), int(box[3]))
+            cv2.rectangle(self.im, p1, p2, color, thickness=self.lw, lineType=cv2.LINE_AA)
+            if label:
+                tf = max(self.lw - 1, 1)  # font thickness
+                w, h = cv2.getTextSize(label, 0, fontScale=self.lw / 3, thickness=tf)[0]  # text width, height
+                outside = p1[1] - h >= 3
+                p2 = p1[0] + w, p1[1] - h - 3 if outside else p1[1] + h + 3
+                cv2.rectangle(self.im, p1, p2, color, -1, cv2.LINE_AA)  # filled
+                cv2.putText(self.im,
+                            label, (p1[0], p1[1] - 2 if outside else p1[1] + h + 2),
+                            0,
+                            self.lw / 3,
+                            txt_color,
+                            thickness=tf,
+                            lineType=cv2.LINE_AA)
 
-    # box2 area
-    box2_area = (b2_x2 - b2_x1) * (b2_y2 - b2_y1) + eps
-
-    # Intersection over box2 area
-    return inter_area / box2_area
-
-
-def box_iou(box1, box2, eps=1e-7):
-    # https://github.com/pytorch/vision/blob/master/torchvision/ops/boxes.py
-    """
-    Return intersection-over-union (Jaccard index) of boxes.
-    Both sets of boxes are expected to be in (x1, y1, x2, y2) format.
-    Arguments:
-        box1 (Tensor[N, 4])
-        box2 (Tensor[M, 4])
-    Returns:
-        iou (Tensor[N, M]): the NxM matrix containing the pairwise
-            IoU values for every element in boxes1 and boxes2
-    """
-
-    # inter(N,M) = (rb(N,M,2) - lt(N,M,2)).clamp(0).prod(2)
-    (a1, a2), (b1, b2) = box1.unsqueeze(1).chunk(2, 2), box2.unsqueeze(0).chunk(2, 2)
-    inter = (torch.min(a2, b2) - torch.max(a1, b1)).clamp(0).prod(2)
-
-    # IoU = inter / (area1 + area2 - inter)
-    return inter / ((a2 - a1).prod(2) + (b2 - b1).prod(2) - inter + eps)
-
-
-def bbox_iou(box1, box2, xywh=True, GIoU=False, DIoU=False, CIoU=False, eps=1e-7):
-    # Returns Intersection over Union (IoU) of box1(1,4) to box2(n,4)
-
-    # Get the coordinates of bounding boxes
-    if xywh:  # transform from xywh to xyxy
-        (x1, y1, w1, h1), (x2, y2, w2, h2) = box1.chunk(4, -1), box2.chunk(4, -1)
-        w1_, h1_, w2_, h2_ = w1 / 2, h1 / 2, w2 / 2, h2 / 2
-        b1_x1, b1_x2, b1_y1, b1_y2 = x1 - w1_, x1 + w1_, y1 - h1_, y1 + h1_
-        b2_x1, b2_x2, b2_y1, b2_y2 = x2 - w2_, x2 + w2_, y2 - h2_, y2 + h2_
-    else:  # x1, y1, x2, y2 = box1
-        b1_x1, b1_y1, b1_x2, b1_y2 = box1.chunk(4, -1)
-        b2_x1, b2_y1, b2_x2, b2_y2 = box2.chunk(4, -1)
-        w1, h1 = b1_x2 - b1_x1, b1_y2 - b1_y1 + eps
-        w2, h2 = b2_x2 - b2_x1, b2_y2 - b2_y1 + eps
-
-    # Intersection area
-    inter = (b1_x2.minimum(b2_x2) - b1_x1.maximum(b2_x1)).clamp(0) * \
-            (b1_y2.minimum(b2_y2) - b1_y1.maximum(b2_y1)).clamp(0)
-
-    # Union Area
-    union = w1 * h1 + w2 * h2 - inter + eps
-
-    # IoU
-    iou = inter / union
-    if CIoU or DIoU or GIoU:
-        cw = b1_x2.maximum(b2_x2) - b1_x1.minimum(b2_x1)  # convex (smallest enclosing box) width
-        ch = b1_y2.maximum(b2_y2) - b1_y1.minimum(b2_y1)  # convex height
-        if CIoU or DIoU:  # Distance or Complete IoU https://arxiv.org/abs/1911.08287v1
-            c2 = cw ** 2 + ch ** 2 + eps  # convex diagonal squared
-            rho2 = ((b2_x1 + b2_x2 - b1_x1 - b1_x2) ** 2 + (b2_y1 + b2_y2 - b1_y1 - b1_y2) ** 2) / 4  # center dist ** 2
-            if CIoU:  # https://github.com/Zzh-tju/DIoU-SSD-pytorch/blob/master/utils/box/box_utils.py#L47
-                v = (4 / math.pi ** 2) * (torch.atan(w2 / h2) - torch.atan(w1 / h1)).pow(2)
-                with torch.no_grad():
-                    alpha = v / (v - iou + (1 + eps))
-                return iou - (rho2 / c2 + v * alpha)  # CIoU
-            return iou - rho2 / c2  # DIoU
-        c_area = cw * ch + eps  # convex area
-        return iou - (c_area - union) / c_area  # GIoU https://arxiv.org/pdf/1902.09630.pdf
-    return iou  # IoU
-
-
-def mask_iou(mask1, mask2, eps=1e-7):
-    """
-    mask1: [N, n] m1 means number of predicted objects
-    mask2: [M, n] m2 means number of gt objects
-    Note: n means image_w x image_h
-    return: masks iou, [N, M]
-    """
-    intersection = torch.matmul(mask1, mask2.t()).clamp(0)
-    union = (mask1.sum(1)[:, None] + mask2.sum(1)[None]) - intersection  # (area1 + area2) - intersection
-    return intersection / (union + eps)
+    def masks(self, masks, colors, im_gpu, alpha=0.5, retina_masks=False):
+        """Plot masks at once.
+        Args:
+            masks (tensor): predicted masks on cuda, shape: [n, h, w]
+            colors (List[List[Int]]): colors for predicted masks, [[r, g, b] * n]
+            im_gpu (tensor): img is in cuda, shape: [3, h, w], range: [0, 1]
+            alpha (float): mask transparency: 0.0 fully transparent, 1.0 opaque
+        """
+        if self.pil:
+            # Convert to numpy first
+            self.im = np.asarray(self.im).copy()
+        if len(masks) == 0:
+            self.im[:] = im_gpu.permute(1, 2, 0).contiguous().cpu().numpy() * 255
+        if im_gpu.device != masks.device:
+            im_gpu = im_gpu.to(masks.device)
+        colors = torch.tensor(colors, device=masks.device, dtype=torch.float32) / 255.0  # shape(n,3)
+        colors = colors[:, None, None]  # shape(n,1,1,3)
+        masks = masks.unsqueeze(3)  # shape(n,h,w,1)
+        masks_color = masks * (colors * alpha)  # shape(n,h,w,3)
+
+        inv_alph_masks = (1 - masks * alpha).cumprod(0)  # shape(n,h,w,1)
+        mcs = masks_color.max(dim=0).values  # shape(n,h,w,3)
+
+        im_gpu = im_gpu.flip(dims=[0])  # flip channel
+        im_gpu = im_gpu.permute(1, 2, 0).contiguous()  # shape(h,w,3)
+        im_gpu = im_gpu * inv_alph_masks[-1] + mcs
+        im_mask = (im_gpu * 255)
+        im_mask_np = im_mask.byte().cpu().numpy()
+        self.im[:] = im_mask_np if retina_masks else scale_image(im_mask_np, self.im.shape)
+        if self.pil:
+            # Convert im back to PIL and update draw
+            self.fromarray(self.im)
 
+    def kpts(self, kpts, shape=(640, 640), radius=5, kpt_line=True):
+        """Plot keypoints on the image.
 
-def masks_iou(mask1, mask2, eps=1e-7):
-    """
-    mask1: [N, n] m1 means number of predicted objects
-    mask2: [N, n] m2 means number of gt objects
-    Note: n means image_w x image_h
-    return: masks iou, (N, )
-    """
-    intersection = (mask1 * mask2).sum(1).clamp(0)  # (N, )
-    union = (mask1.sum(1) + mask2.sum(1))[None] - intersection  # (area1 + area2) - intersection
-    return intersection / (union + eps)
-
-
-def smooth_BCE(eps=0.1):  # https://github.com/ultralytics/yolov3/issues/238#issuecomment-598028441
-    # return positive, negative label smoothing BCE targets
-    return 1.0 - 0.5 * eps, 0.5 * eps
-
-
-# losses
-class FocalLoss(nn.Module):
-    # Wraps focal loss around existing loss_fcn(), i.e. criteria = FocalLoss(nn.BCEWithLogitsLoss(), gamma=1.5)
-    def __init__(self, loss_fcn, gamma=1.5, alpha=0.25):
-        super().__init__()
-        self.loss_fcn = loss_fcn  # must be nn.BCEWithLogitsLoss()
-        self.gamma = gamma
-        self.alpha = alpha
-        self.reduction = loss_fcn.reduction
-        self.loss_fcn.reduction = 'none'  # required to apply FL to each element
-
-    def forward(self, pred, true):
-        loss = self.loss_fcn(pred, true)
-        # p_t = torch.exp(-loss)
-        # loss *= self.alpha * (1.000001 - p_t) ** self.gamma  # non-zero power for gradient stability
-
-        # TF implementation https://github.com/tensorflow/addons/blob/v0.7.1/tensorflow_addons/losses/focal_loss.py
-        pred_prob = torch.sigmoid(pred)  # prob from logits
-        p_t = true * pred_prob + (1 - true) * (1 - pred_prob)
-        alpha_factor = true * self.alpha + (1 - true) * (1 - self.alpha)
-        modulating_factor = (1.0 - p_t) ** self.gamma
-        loss *= alpha_factor * modulating_factor
-
-        if self.reduction == 'mean':
-            return loss.mean()
-        elif self.reduction == 'sum':
-            return loss.sum()
-        else:  # 'none'
-            return loss
-
-
-class ConfusionMatrix:
-    # Updated version of https://github.com/kaanakan/object_detection_confusion_matrix
-    def __init__(self, nc, conf=0.25, iou_thres=0.45):
-        self.matrix = np.zeros((nc + 1, nc + 1))
-        self.nc = nc  # number of classes
-        self.conf = conf
-        self.iou_thres = iou_thres
+        Args:
+            kpts (tensor): Predicted keypoints with shape [17, 3]. Each keypoint has (x, y, confidence).
+            shape (tuple): Image shape as a tuple (h, w), where h is the height and w is the width.
+            radius (int, optional): Radius of the drawn keypoints. Default is 5.
+            kpt_line (bool, optional): If True, the function will draw lines connecting keypoints
+                                       for human pose. Default is True.
 
-    def process_batch(self, detections, labels):
-        """
-        Return intersection-over-union (Jaccard index) of boxes.
-        Both sets of boxes are expected to be in (x1, y1, x2, y2) format.
-        Arguments:
-            detections (Array[N, 6]), x1, y1, x2, y2, conf, class
-            labels (Array[M, 5]), class, x1, y1, x2, y2
-        Returns:
-            None, updates confusion matrix accordingly
+        Note: `kpt_line=True` currently only supports human pose plotting.
         """
-        if detections is None:
-            gt_classes = labels.int()
-            for gc in gt_classes:
-                self.matrix[self.nc, gc] += 1  # background FN
-            return
-
-        detections = detections[detections[:, 4] > self.conf]
-        gt_classes = labels[:, 0].int()
-        detection_classes = detections[:, 5].int()
-        iou = box_iou(labels[:, 1:], detections[:, :4])
-
-        x = torch.where(iou > self.iou_thres)
-        if x[0].shape[0]:
-            matches = torch.cat((torch.stack(x, 1), iou[x[0], x[1]][:, None]), 1).cpu().numpy()
-            if x[0].shape[0] > 1:
-                matches = matches[matches[:, 2].argsort()[::-1]]
-                matches = matches[np.unique(matches[:, 1], return_index=True)[1]]
-                matches = matches[matches[:, 2].argsort()[::-1]]
-                matches = matches[np.unique(matches[:, 0], return_index=True)[1]]
+        if self.pil:
+            # Convert to numpy first
+            self.im = np.asarray(self.im).copy()
+        nkpt, ndim = kpts.shape
+        is_pose = nkpt == 17 and ndim == 3
+        kpt_line &= is_pose  # `kpt_line=True` for now only supports human pose plotting
+        for i, k in enumerate(kpts):
+            color_k = [int(x) for x in self.kpt_color[i]] if is_pose else colors(i)
+            x_coord, y_coord = k[0], k[1]
+            if x_coord % shape[1] != 0 and y_coord % shape[0] != 0:
+                if len(k) == 3:
+                    conf = k[2]
+                    if conf < 0.5:
+                        continue
+                cv2.circle(self.im, (int(x_coord), int(y_coord)), radius, color_k, -1, lineType=cv2.LINE_AA)
+
+        if kpt_line:
+            ndim = kpts.shape[-1]
+            for i, sk in enumerate(self.skeleton):
+                pos1 = (int(kpts[(sk[0] - 1), 0]), int(kpts[(sk[0] - 1), 1]))
+                pos2 = (int(kpts[(sk[1] - 1), 0]), int(kpts[(sk[1] - 1), 1]))
+                if ndim == 3:
+                    conf1 = kpts[(sk[0] - 1), 2]
+                    conf2 = kpts[(sk[1] - 1), 2]
+                    if conf1 < 0.5 or conf2 < 0.5:
+                        continue
+                if pos1[0] % shape[1] == 0 or pos1[1] % shape[0] == 0 or pos1[0] < 0 or pos1[1] < 0:
+                    continue
+                if pos2[0] % shape[1] == 0 or pos2[1] % shape[0] == 0 or pos2[0] < 0 or pos2[1] < 0:
+                    continue
+                cv2.line(self.im, pos1, pos2, [int(x) for x in self.limb_color[i]], thickness=2, lineType=cv2.LINE_AA)
+        if self.pil:
+            # Convert im back to PIL and update draw
+            self.fromarray(self.im)
+
+    def rectangle(self, xy, fill=None, outline=None, width=1):
+        """Add rectangle to image (PIL-only)."""
+        self.draw.rectangle(xy, fill, outline, width)
+
+    def text(self, xy, text, txt_color=(255, 255, 255), anchor='top', box_style=False):
+        """Adds text to an image using PIL or cv2."""
+        if anchor == 'bottom':  # start y from font bottom
+            w, h = self.font.getsize(text)  # text width, height
+            xy[1] += 1 - h
+        if self.pil:
+            if box_style:
+                w, h = self.font.getsize(text)
+                self.draw.rectangle((xy[0], xy[1], xy[0] + w + 1, xy[1] + h + 1), fill=txt_color)
+                # Using `txt_color` for background and draw fg with white color
+                txt_color = (255, 255, 255)
+            self.draw.text(xy, text, fill=txt_color, font=self.font)
         else:
-            matches = np.zeros((0, 3))
-
-        n = matches.shape[0] > 0
-        m0, m1, _ = matches.transpose().astype(int)
-        for i, gc in enumerate(gt_classes):
-            j = m0 == i
-            if n and sum(j) == 1:
-                self.matrix[detection_classes[m1[j]], gc] += 1  # correct
-            else:
-                self.matrix[self.nc, gc] += 1  # true background
-
-        if n:
-            for i, dc in enumerate(detection_classes):
-                if not any(m1 == i):
-                    self.matrix[dc, self.nc] += 1  # predicted background
-
-    def matrix(self):
-        return self.matrix
-
-    def tp_fp(self):
-        tp = self.matrix.diagonal()  # true positives
-        fp = self.matrix.sum(1) - tp  # false positives
-        # fn = self.matrix.sum(0) - tp  # false negatives (missed detections)
-        return tp[:-1], fp[:-1]  # remove background class
-
-    @TryExcept('WARNING ⚠️ ConfusionMatrix plot failure')
-    def plot(self, normalize=True, save_dir='', names=()):
-        import seaborn as sn
-
-        array = self.matrix / ((self.matrix.sum(0).reshape(1, -1) + 1E-9) if normalize else 1)  # normalize columns
-        array[array < 0.005] = np.nan  # don't annotate (would appear as 0.00)
-
-        fig, ax = plt.subplots(1, 1, figsize=(12, 9), tight_layout=True)
-        nc, nn = self.nc, len(names)  # number of classes, names
-        sn.set(font_scale=1.0 if nc < 50 else 0.8)  # for label size
-        labels = (0 < nn < 99) and (nn == nc)  # apply names to ticklabels
-        ticklabels = (names + ['background']) if labels else "auto"
-        with warnings.catch_warnings():
-            warnings.simplefilter('ignore')  # suppress empty matrix RuntimeWarning: All-NaN slice encountered
-            sn.heatmap(array,
-                       ax=ax,
-                       annot=nc < 30,
-                       annot_kws={
-                           "size": 8},
-                       cmap='Blues',
-                       fmt='.2f',
-                       square=True,
-                       vmin=0.0,
-                       xticklabels=ticklabels,
-                       yticklabels=ticklabels).set_facecolor((1, 1, 1))
-        ax.set_xlabel('True')
-        ax.set_ylabel('Predicted')
-        ax.set_title('Confusion Matrix')
-        fig.savefig(Path(save_dir) / 'confusion_matrix.png', dpi=250)
-        plt.close(fig)
-
-    def print(self):
-        for i in range(self.nc + 1):
-            print(' '.join(map(str, self.matrix[i])))
-
-
-def smooth(y, f=0.05):
-    # Box filter of fraction f
-    nf = round(len(y) * f * 2) // 2 + 1  # number of filter elements (must be odd)
-    p = np.ones(nf // 2)  # ones padding
-    yp = np.concatenate((p * y[0], y, p * y[-1]), 0)  # y padded
-    return np.convolve(yp, np.ones(nf) / nf, mode='valid')  # y-smoothed
-
-
-def plot_pr_curve(px, py, ap, save_dir=Path('pr_curve.png'), names=()):
-    # Precision-recall curve
-    fig, ax = plt.subplots(1, 1, figsize=(9, 6), tight_layout=True)
-    py = np.stack(py, axis=1)
-
-    if 0 < len(names) < 21:  # display per-class legend if < 21 classes
-        for i, y in enumerate(py.T):
-            ax.plot(px, y, linewidth=1, label=f'{names[i]} {ap[i, 0]:.3f}')  # plot(recall, precision)
+            if box_style:
+                tf = max(self.lw - 1, 1)  # font thickness
+                w, h = cv2.getTextSize(text, 0, fontScale=self.lw / 3, thickness=tf)[0]  # text width, height
+                outside = xy[1] - h >= 3
+                p2 = xy[0] + w, xy[1] - h - 3 if outside else xy[1] + h + 3
+                cv2.rectangle(self.im, xy, p2, txt_color, -1, cv2.LINE_AA)  # filled
+                # Using `txt_color` for background and draw fg with white color
+                txt_color = (255, 255, 255)
+            tf = max(self.lw - 1, 1)  # font thickness
+            cv2.putText(self.im, text, xy, 0, self.lw / 3, txt_color, thickness=tf, lineType=cv2.LINE_AA)
+
+    def fromarray(self, im):
+        """Update self.im from a numpy array."""
+        self.im = im if isinstance(im, Image.Image) else Image.fromarray(im)
+        self.draw = ImageDraw.Draw(self.im)
+
+    def result(self):
+        """Return annotated image as array."""
+        return np.asarray(self.im)
+
+
+@TryExcept()  # known issue https://github.com/ultralytics/yolov5/issues/5395
+@plt_settings()
+def plot_labels(boxes, cls, names=(), save_dir=Path('')):
+    """Save and plot image with no axis or spines."""
+    import pandas as pd
+    import seaborn as sn
+
+    # Plot dataset labels
+    LOGGER.info(f"Plotting labels to {save_dir / 'labels.jpg'}... ")
+    b = boxes.transpose()  # classes, boxes
+    nc = int(cls.max() + 1)  # number of classes
+    x = pd.DataFrame(b.transpose(), columns=['x', 'y', 'width', 'height'])
+
+    # Seaborn correlogram
+    sn.pairplot(x, corner=True, diag_kind='auto', kind='hist', diag_kws=dict(bins=50), plot_kws=dict(pmax=0.9))
+    plt.savefig(save_dir / 'labels_correlogram.jpg', dpi=200)
+    plt.close()
+
+    # Matplotlib labels
+    ax = plt.subplots(2, 2, figsize=(8, 8), tight_layout=True)[1].ravel()
+    y = ax[0].hist(cls, bins=np.linspace(0, nc, nc + 1) - 0.5, rwidth=0.8)
+    with contextlib.suppress(Exception):  # color histogram bars by class
+        [y[2].patches[i].set_color([x / 255 for x in colors(i)]) for i in range(nc)]  # known issue #3195
+    ax[0].set_ylabel('instances')
+    if 0 < len(names) < 30:
+        ax[0].set_xticks(range(len(names)))
+        ax[0].set_xticklabels(list(names.values()), rotation=90, fontsize=10)
     else:
-        ax.plot(px, py, linewidth=1, color='grey')  # plot(recall, precision)
-
-    ax.plot(px, py.mean(1), linewidth=3, color='blue', label='all classes %.3f mAP@0.5' % ap[:, 0].mean())
-    ax.set_xlabel('Recall')
-    ax.set_ylabel('Precision')
-    ax.set_xlim(0, 1)
-    ax.set_ylim(0, 1)
-    ax.legend(bbox_to_anchor=(1.04, 1), loc="upper left")
-    ax.set_title('Precision-Recall Curve')
-    fig.savefig(save_dir, dpi=250)
-    plt.close(fig)
-
-
-def plot_mc_curve(px, py, save_dir=Path('mc_curve.png'), names=(), xlabel='Confidence', ylabel='Metric'):
-    # Metric-confidence curve
-    fig, ax = plt.subplots(1, 1, figsize=(9, 6), tight_layout=True)
-
-    if 0 < len(names) < 21:  # display per-class legend if < 21 classes
-        for i, y in enumerate(py):
-            ax.plot(px, y, linewidth=1, label=f'{names[i]}')  # plot(confidence, metric)
+        ax[0].set_xlabel('classes')
+    sn.histplot(x, x='x', y='y', ax=ax[2], bins=50, pmax=0.9)
+    sn.histplot(x, x='width', y='height', ax=ax[3], bins=50, pmax=0.9)
+
+    # Rectangles
+    boxes[:, 0:2] = 0.5  # center
+    boxes = xywh2xyxy(boxes) * 1000
+    img = Image.fromarray(np.ones((1000, 1000, 3), dtype=np.uint8) * 255)
+    for cls, box in zip(cls[:500], boxes[:500]):
+        ImageDraw.Draw(img).rectangle(box, width=1, outline=colors(cls))  # plot
+    ax[1].imshow(img)
+    ax[1].axis('off')
+
+    for a in [0, 1, 2, 3]:
+        for s in ['top', 'right', 'left', 'bottom']:
+            ax[a].spines[s].set_visible(False)
+
+    plt.savefig(save_dir / 'labels.jpg', dpi=200)
+    plt.close()
+
+
+def save_one_box(xyxy, im, file=Path('im.jpg'), gain=1.02, pad=10, square=False, BGR=False, save=True):
+    """Save image crop as {file} with crop size multiple {gain} and {pad} pixels. Save and/or return crop."""
+    b = xyxy2xywh(xyxy.view(-1, 4))  # boxes
+    if square:
+        b[:, 2:] = b[:, 2:].max(1)[0].unsqueeze(1)  # attempt rectangle to square
+    b[:, 2:] = b[:, 2:] * gain + pad  # box wh * gain + pad
+    xyxy = xywh2xyxy(b).long()
+    clip_boxes(xyxy, im.shape)
+    crop = im[int(xyxy[0, 1]):int(xyxy[0, 3]), int(xyxy[0, 0]):int(xyxy[0, 2]), ::(1 if BGR else -1)]
+    if save:
+        file.parent.mkdir(parents=True, exist_ok=True)  # make directory
+        f = str(increment_path(file).with_suffix('.jpg'))
+        # cv2.imwrite(f, crop)  # save BGR, https://github.com/ultralytics/yolov5/issues/7007 chroma subsampling issue
+        Image.fromarray(crop[..., ::-1]).save(f, quality=95, subsampling=0)  # save RGB
+    return crop
+
+
+@threaded
+def plot_images(images,
+                batch_idx,
+                cls,
+                bboxes=np.zeros(0, dtype=np.float32),
+                masks=np.zeros(0, dtype=np.uint8),
+                kpts=np.zeros((0, 51), dtype=np.float32),
+                paths=None,
+                fname='images.jpg',
+                names=None):
+    # Plot image grid with labels
+    if isinstance(images, torch.Tensor):
+        images = images.cpu().float().numpy()
+    if isinstance(cls, torch.Tensor):
+        cls = cls.cpu().numpy()
+    if isinstance(bboxes, torch.Tensor):
+        bboxes = bboxes.cpu().numpy()
+    if isinstance(masks, torch.Tensor):
+        masks = masks.cpu().numpy().astype(int)
+    if isinstance(kpts, torch.Tensor):
+        kpts = kpts.cpu().numpy()
+    if isinstance(batch_idx, torch.Tensor):
+        batch_idx = batch_idx.cpu().numpy()
+
+    max_size = 1920  # max image size
+    max_subplots = 16  # max image subplots, i.e. 4x4
+    bs, _, h, w = images.shape  # batch size, _, height, width
+    bs = min(bs, max_subplots)  # limit plot images
+    ns = np.ceil(bs ** 0.5)  # number of subplots (square)
+    if np.max(images[0]) <= 1:
+        images *= 255  # de-normalise (optional)
+
+    # Build Image
+    mosaic = np.full((int(ns * h), int(ns * w), 3), 255, dtype=np.uint8)  # init
+    for i, im in enumerate(images):
+        if i == max_subplots:  # if last batch has fewer images than we expect
+            break
+        x, y = int(w * (i // ns)), int(h * (i % ns))  # block origin
+        im = im.transpose(1, 2, 0)
+        mosaic[y:y + h, x:x + w, :] = im
+
+    # Resize (optional)
+    scale = max_size / ns / max(h, w)
+    if scale < 1:
+        h = math.ceil(scale * h)
+        w = math.ceil(scale * w)
+        mosaic = cv2.resize(mosaic, tuple(int(x * ns) for x in (w, h)))
+
+    # Annotate
+    fs = int((h + w) * ns * 0.01)  # font size
+    annotator = Annotator(mosaic, line_width=round(fs / 10), font_size=fs, pil=True, example=names)
+    for i in range(i + 1):
+        x, y = int(w * (i // ns)), int(h * (i % ns))  # block origin
+        annotator.rectangle([x, y, x + w, y + h], None, (255, 255, 255), width=2)  # borders
+        if paths:
+            annotator.text((x + 5, y + 5), text=Path(paths[i]).name[:40], txt_color=(220, 220, 220))  # filenames
+        if len(cls) > 0:
+            idx = batch_idx == i
+            classes = cls[idx].astype('int')
+
+            if len(bboxes):
+                boxes = xywh2xyxy(bboxes[idx, :4]).T
+                labels = bboxes.shape[1] == 4  # labels if no conf column
+                conf = None if labels else bboxes[idx, 4]  # check for confidence presence (label vs pred)
+
+                if boxes.shape[1]:
+                    if boxes.max() <= 1.01:  # if normalized with tolerance 0.01
+                        boxes[[0, 2]] *= w  # scale to pixels
+                        boxes[[1, 3]] *= h
+                    elif scale < 1:  # absolute coords need scale if image scales
+                        boxes *= scale
+                boxes[[0, 2]] += x
+                boxes[[1, 3]] += y
+                for j, box in enumerate(boxes.T.tolist()):
+                    c = classes[j]
+                    color = colors(c)
+                    c = names.get(c, c) if names else c
+                    if labels or conf[j] > 0.25:  # 0.25 conf thresh
+                        label = f'{c}' if labels else f'{c} {conf[j]:.1f}'
+                        annotator.box_label(box, label, color=color)
+            elif len(classes):
+                for c in classes:
+                    color = colors(c)
+                    c = names.get(c, c) if names else c
+                    annotator.text((x, y), f'{c}', txt_color=color, box_style=True)
+
+            # Plot keypoints
+            if len(kpts):
+                kpts_ = kpts[idx].copy()
+                if len(kpts_):
+                    if kpts_[..., 0].max() <= 1.01 or kpts_[..., 1].max() <= 1.01:  # if normalized with tolerance .01
+                        kpts_[..., 0] *= w  # scale to pixels
+                        kpts_[..., 1] *= h
+                    elif scale < 1:  # absolute coords need scale if image scales
+                        kpts_ *= scale
+                kpts_[..., 0] += x
+                kpts_[..., 1] += y
+                for j in range(len(kpts_)):
+                    if labels or conf[j] > 0.25:  # 0.25 conf thresh
+                        annotator.kpts(kpts_[j])
+
+            # Plot masks
+            if len(masks):
+                if idx.shape[0] == masks.shape[0]:  # overlap_masks=False
+                    image_masks = masks[idx]
+                else:  # overlap_masks=True
+                    image_masks = masks[[i]]  # (1, 640, 640)
+                    nl = idx.sum()
+                    index = np.arange(nl).reshape((nl, 1, 1)) + 1
+                    image_masks = np.repeat(image_masks, nl, axis=0)
+                    image_masks = np.where(image_masks == index, 1.0, 0.0)
+
+                im = np.asarray(annotator.im).copy()
+                for j, box in enumerate(boxes.T.tolist()):
+                    if labels or conf[j] > 0.25:  # 0.25 conf thresh
+                        color = colors(classes[j])
+                        mh, mw = image_masks[j].shape
+                        if mh != h or mw != w:
+                            mask = image_masks[j].astype(np.uint8)
+                            mask = cv2.resize(mask, (w, h))
+                            mask = mask.astype(bool)
+                        else:
+                            mask = image_masks[j].astype(bool)
+                        with contextlib.suppress(Exception):
+                            im[y:y + h, x:x + w, :][mask] = im[y:y + h, x:x + w, :][mask] * 0.4 + np.array(color) * 0.6
+                annotator.fromarray(im)
+    annotator.im.save(fname)  # save
+
+
+@plt_settings()
+def plot_results(file='path/to/results.csv', dir='', segment=False, pose=False, classify=False):
+    """Plot training results.csv. Usage: from utils.plots import *; plot_results('path/to/results.csv')."""
+    import pandas as pd
+    save_dir = Path(file).parent if file else Path(dir)
+    if classify:
+        fig, ax = plt.subplots(2, 2, figsize=(6, 6), tight_layout=True)
+        index = [1, 4, 2, 3]
+    elif segment:
+        fig, ax = plt.subplots(2, 8, figsize=(18, 6), tight_layout=True)
+        index = [1, 2, 3, 4, 5, 6, 9, 10, 13, 14, 15, 16, 7, 8, 11, 12]
+    elif pose:
+        fig, ax = plt.subplots(2, 9, figsize=(21, 6), tight_layout=True)
+        index = [1, 2, 3, 4, 5, 6, 7, 10, 11, 14, 15, 16, 17, 18, 8, 9, 12, 13]
     else:
-        ax.plot(px, py.T, linewidth=1, color='grey')  # plot(confidence, metric)
+        fig, ax = plt.subplots(2, 5, figsize=(12, 6), tight_layout=True)
+        index = [1, 2, 3, 4, 5, 8, 9, 10, 6, 7]
+    ax = ax.ravel()
+    files = list(save_dir.glob('results*.csv'))
+    assert len(files), f'No results.csv files found in {save_dir.resolve()}, nothing to plot.'
+    for f in files:
+        try:
+            data = pd.read_csv(f)
+            s = [x.strip() for x in data.columns]
+            x = data.values[:, 0]
+            for i, j in enumerate(index):
+                y = data.values[:, j].astype('float')
+                # y[y == 0] = np.nan  # don't show zero values
+                ax[i].plot(x, y, marker='.', label=f.stem, linewidth=2, markersize=8)
+                ax[i].set_title(s[j], fontsize=12)
+                # if j in [8, 9, 10]:  # share train and val loss y axes
+                #     ax[i].get_shared_y_axes().join(ax[i], ax[i - 5])
+        except Exception as e:
+            LOGGER.warning(f'WARNING: Plotting error for {f}: {e}')
+    ax[1].legend()
+    fig.savefig(save_dir / 'results.png', dpi=200)
+    plt.close()
+
+
+def output_to_target(output, max_det=300):
+    """Convert model output to target format [batch_id, class_id, x, y, w, h, conf] for plotting."""
+    targets = []
+    for i, o in enumerate(output):
+        box, conf, cls = o[:max_det, :6].cpu().split((4, 1, 1), 1)
+        j = torch.full((conf.shape[0], 1), i)
+        targets.append(torch.cat((j, cls, xyxy2xywh(box), conf), 1))
+    targets = torch.cat(targets, 0).numpy()
+    return targets[:, 0], targets[:, 1], targets[:, 2:]
 
-    y = smooth(py.mean(0), 0.05)
-    ax.plot(px, y, linewidth=3, color='blue', label=f'all classes {y.max():.2f} at {px[y.argmax()]:.3f}')
-    ax.set_xlabel(xlabel)
-    ax.set_ylabel(ylabel)
-    ax.set_xlim(0, 1)
-    ax.set_ylim(0, 1)
-    ax.legend(bbox_to_anchor=(1.04, 1), loc="upper left")
-    ax.set_title(f'{ylabel}-Confidence Curve')
-    fig.savefig(save_dir, dpi=250)
-    plt.close(fig)
-
-
-def compute_ap(recall, precision):
-    """ Compute the average precision, given the recall and precision curves
-    # Arguments
-        recall:    The recall curve (list)
-        precision: The precision curve (list)
-    # Returns
-        Average precision, precision curve, recall curve
-    """
 
-    # Append sentinel values to beginning and end
-    mrec = np.concatenate(([0.0], recall, [1.0]))
-    mpre = np.concatenate(([1.0], precision, [0.0]))
-
-    # Compute the precision envelope
-    mpre = np.flip(np.maximum.accumulate(np.flip(mpre)))
-
-    # Integrate area under curve
-    method = 'interp'  # methods: 'continuous', 'interp'
-    if method == 'interp':
-        x = np.linspace(0, 1, 101)  # 101-point interp (COCO)
-        ap = np.trapz(np.interp(x, mrec, mpre), x)  # integrate
-    else:  # 'continuous'
-        i = np.where(mrec[1:] != mrec[:-1])[0]  # points where x-axis (recall) changes
-        ap = np.sum((mrec[i + 1] - mrec[i]) * mpre[i + 1])  # area under curve
-
-    return ap, mpre, mrec
-
-
-def ap_per_class(tp, conf, pred_cls, target_cls, plot=False, save_dir=Path(), names=(), eps=1e-16, prefix=""):
-    """ Compute the average precision, given the recall and precision curves.
-    Source: https://github.com/rafaelpadilla/Object-Detection-Metrics.
-    # Arguments
-        tp:  True positives (nparray, nx1 or nx10).
-        conf:  Objectness value from 0-1 (nparray).
-        pred_cls:  Predicted object classes (nparray).
-        target_cls:  True object classes (nparray).
-        plot:  Plot precision-recall curve at mAP@0.5
-        save_dir:  Plot save directory
-    # Returns
-        The average precision as computed in py-faster-rcnn.
+def feature_visualization(x, module_type, stage, n=32, save_dir=Path('runs/detect/exp')):
     """
+    Visualize feature maps of a given model module during inference.
 
-    # Sort by objectness
-    i = np.argsort(-conf)
-    tp, conf, pred_cls = tp[i], conf[i], pred_cls[i]
-
-    # Find unique classes
-    unique_classes, nt = np.unique(target_cls, return_counts=True)
-    nc = unique_classes.shape[0]  # number of classes, number of detections
-
-    # Create Precision-Recall curve and compute AP for each class
-    px, py = np.linspace(0, 1, 1000), []  # for plotting
-    ap, p, r = np.zeros((nc, tp.shape[1])), np.zeros((nc, 1000)), np.zeros((nc, 1000))
-    for ci, c in enumerate(unique_classes):
-        i = pred_cls == c
-        n_l = nt[ci]  # number of labels
-        n_p = i.sum()  # number of predictions
-        if n_p == 0 or n_l == 0:
-            continue
-
-        # Accumulate FPs and TPs
-        fpc = (1 - tp[i]).cumsum(0)
-        tpc = tp[i].cumsum(0)
-
-        # Recall
-        recall = tpc / (n_l + eps)  # recall curve
-        r[ci] = np.interp(-px, -conf[i], recall[:, 0], left=0)  # negative x, xp because xp decreases
-
-        # Precision
-        precision = tpc / (tpc + fpc)  # precision curve
-        p[ci] = np.interp(-px, -conf[i], precision[:, 0], left=1)  # p at pr_score
-
-        # AP from recall-precision curve
-        for j in range(tp.shape[1]):
-            ap[ci, j], mpre, mrec = compute_ap(recall[:, j], precision[:, j])
-            if plot and j == 0:
-                py.append(np.interp(px, mrec, mpre))  # precision at mAP@0.5
-
-    # Compute F1 (harmonic mean of precision and recall)
-    f1 = 2 * p * r / (p + r + eps)
-    names = [v for k, v in names.items() if k in unique_classes]  # list: only classes that have data
-    names = dict(enumerate(names))  # to dict
-    if plot:
-        plot_pr_curve(px, py, ap, save_dir / f'{prefix}PR_curve.png', names)
-        plot_mc_curve(px, f1, save_dir / f'{prefix}F1_curve.png', names, ylabel='F1')
-        plot_mc_curve(px, p, save_dir / f'{prefix}P_curve.png', names, ylabel='Precision')
-        plot_mc_curve(px, r, save_dir / f'{prefix}R_curve.png', names, ylabel='Recall')
-
-    i = smooth(f1.mean(0), 0.1).argmax()  # max F1 index
-    p, r, f1 = p[:, i], r[:, i], f1[:, i]
-    tp = (r * nt).round()  # true positives
-    fp = (tp / (p + eps) - tp).round()  # false positives
-    return tp, fp, p, r, f1, ap, unique_classes.astype(int)
-
-
-class Metric:
-
-    def __init__(self) -> None:
-        self.p = []  # (nc, )
-        self.r = []  # (nc, )
-        self.f1 = []  # (nc, )
-        self.all_ap = []  # (nc, 10)
-        self.ap_class_index = []  # (nc, )
-
-    @property
-    def ap50(self):
-        """AP@0.5 of all classes.
-        Return:
-            (nc, ) or [].
-        """
-        return self.all_ap[:, 0] if len(self.all_ap) else []
-
-    @property
-    def ap(self):
-        """AP@0.5:0.95
-        Return:
-            (nc, ) or [].
-        """
-        return self.all_ap.mean(1) if len(self.all_ap) else []
-
-    @property
-    def mp(self):
-        """mean precision of all classes.
-        Return:
-            float.
-        """
-        return self.p.mean() if len(self.p) else 0.0
-
-    @property
-    def mr(self):
-        """mean recall of all classes.
-        Return:
-            float.
-        """
-        return self.r.mean() if len(self.r) else 0.0
-
-    @property
-    def map50(self):
-        """Mean AP@0.5 of all classes.
-        Return:
-            float.
-        """
-        return self.all_ap[:, 0].mean() if len(self.all_ap) else 0.0
+    Args:
+        x (torch.Tensor): Features to be visualized.
+        module_type (str): Module type.
+        stage (int): Module stage within the model.
+        n (int, optional): Maximum number of feature maps to plot. Defaults to 32.
+        save_dir (Path, optional): Directory to save results. Defaults to Path('runs/detect/exp').
 
-    @property
-    def map(self):
-        """Mean AP@0.5:0.95 of all classes.
-        Return:
-            float.
-        """
-        return self.all_ap.mean() if len(self.all_ap) else 0.0
-
-    def mean_results(self):
-        """Mean of results, return mp, mr, map50, map"""
-        return [self.mp, self.mr, self.map50, self.map]
-
-    def class_result(self, i):
-        """class-aware result, return p[i], r[i], ap50[i], ap[i]"""
-        return self.p[i], self.r[i], self.ap50[i], self.ap[i]
-
-    def get_maps(self, nc):
-        maps = np.zeros(nc) + self.map
-        for i, c in enumerate(self.ap_class_index):
-            maps[c] = self.ap[i]
-        return maps
-
-    def fitness(self):
-        # Model fitness as a weighted combination of metrics
-        w = [0.0, 0.0, 0.1, 0.9]  # weights for [P, R, mAP@0.5, mAP@0.5:0.95]
-        return (np.array(self.mean_results()) * w).sum()
-
-    def update(self, results):
-        """
-        Args:
-            results: tuple(p, r, ap, f1, ap_class)
-        """
-        self.p, self.r, self.f1, self.all_ap, self.ap_class_index = results
-
-
-class DetMetrics:
-
-    def __init__(self, save_dir=Path("."), plot=False, names=()) -> None:
-        self.save_dir = save_dir
-        self.plot = plot
-        self.names = names
-        self.metric = Metric()
-
-    def process(self, tp, conf, pred_cls, target_cls):
-        results = ap_per_class(tp, conf, pred_cls, target_cls, plot=self.plot, save_dir=self.save_dir,
-                               names=self.names)[2:]
-        self.metric.update(results)
-
-    @property
-    def keys(self):
-        return ["metrics/precision(B)", "metrics/recall(B)", "metrics/mAP50(B)", "metrics/mAP50-95(B)"]
-
-    def mean_results(self):
-        return self.metric.mean_results()
-
-    def class_result(self, i):
-        return self.metric.class_result(i)
-
-    def get_maps(self, nc):
-        return self.metric.get_maps(nc)
-
-    @property
-    def fitness(self):
-        return self.metric.fitness()
-
-    @property
-    def ap_class_index(self):
-        return self.metric.ap_class_index
-
-    @property
-    def results_dict(self):
-        return dict(zip(self.keys + ["fitness"], self.mean_results() + [self.fitness]))
-
-
-class SegmentMetrics:
-
-    def __init__(self, save_dir=Path("."), plot=False, names=()) -> None:
-        self.save_dir = save_dir
-        self.plot = plot
-        self.names = names
-        self.metric_box = Metric()
-        self.metric_mask = Metric()
-
-    def process(self, tp_m, tp_b, conf, pred_cls, target_cls):
-        results_mask = ap_per_class(tp_m,
-                                    conf,
-                                    pred_cls,
-                                    target_cls,
-                                    plot=self.plot,
-                                    save_dir=self.save_dir,
-                                    names=self.names,
-                                    prefix="Mask")[2:]
-        self.metric_mask.update(results_mask)
-        results_box = ap_per_class(tp_b,
-                                   conf,
-                                   pred_cls,
-                                   target_cls,
-                                   plot=self.plot,
-                                   save_dir=self.save_dir,
-                                   names=self.names,
-                                   prefix="Box")[2:]
-        self.metric_box.update(results_box)
-
-    @property
-    def keys(self):
-        return [
-            "metrics/precision(B)", "metrics/recall(B)", "metrics/mAP50(B)", "metrics/mAP50-95(B)",
-            "metrics/precision(M)", "metrics/recall(M)", "metrics/mAP50(M)", "metrics/mAP50-95(M)"]
-
-    def mean_results(self):
-        return self.metric_box.mean_results() + self.metric_mask.mean_results()
-
-    def class_result(self, i):
-        return self.metric_box.class_result(i) + self.metric_mask.class_result(i)
-
-    def get_maps(self, nc):
-        return self.metric_box.get_maps(nc) + self.metric_mask.get_maps(nc)
-
-    @property
-    def fitness(self):
-        return self.metric_mask.fitness() + self.metric_box.fitness()
-
-    @property
-    def ap_class_index(self):
-        # boxes and masks have the same ap_class_index
-        return self.metric_box.ap_class_index
-
-    @property
-    def results_dict(self):
-        return dict(zip(self.keys + ["fitness"], self.mean_results() + [self.fitness]))
-
-
-class ClassifyMetrics:
-
-    def __init__(self) -> None:
-        self.top1 = 0
-        self.top5 = 0
-
-    def process(self, targets, pred):
-        # target classes and predicted classes
-        pred, targets = torch.cat(pred), torch.cat(targets)
-        correct = (targets[:, None] == pred).float()
-        acc = torch.stack((correct[:, 0], correct.max(1).values), dim=1)  # (top1, top5) accuracy
-        self.top1, self.top5 = acc.mean(0).tolist()
-
-    @property
-    def fitness(self):
-        return self.top5
-
-    @property
-    def results_dict(self):
-        return dict(zip(self.keys + ["fitness"], [self.top1, self.top5, self.fitness]))
-
-    @property
-    def keys(self):
-        return ["metrics/accuracy_top1", "metrics/accuracy_top5"]
+    Returns:
+        None: This function does not return any value; it saves the visualization to the specified directory.
+    """
+    for m in ['Detect', 'Pose', 'Segment']:
+        if m in module_type:
+            return
+    batch, channels, height, width = x.shape  # batch, channels, height, width
+    if height > 1 and width > 1:
+        f = save_dir / f"stage{stage}_{module_type.split('.')[-1]}_features.png"  # filename
+
+        blocks = torch.chunk(x[0].cpu(), channels, dim=0)  # select batch index 0, block by channels
+        n = min(n, channels)  # number of plots
+        fig, ax = plt.subplots(math.ceil(n / 8), 8, tight_layout=True)  # 8 rows x n/8 cols
+        ax = ax.ravel()
+        plt.subplots_adjust(wspace=0.05, hspace=0.05)
+        for i in range(n):
+            ax[i].imshow(blocks[i].squeeze())  # cmap='gray'
+            ax[i].axis('off')
+
+        LOGGER.info(f'Saving {f}... ({n}/{channels})')
+        plt.savefig(f, dpi=300, bbox_inches='tight')
+        plt.close()
+        np.save(str(f.with_suffix('.npy')), x[0].cpu().numpy())  # npy save
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/utils/ops.py` & `ultralytics-8.0.90/ultralytics/yolo/utils/ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,16 @@
     Returns:
       (np.ndarray): the minimum and maximum x and y values of the segment.
     """
     # Convert 1 segment label to 1 box label, applying inside-image constraint, i.e. (xy1, xy2, ...) to (xyxy)
     x, y = segment.T  # segment xy
     inside = (x >= 0) & (y >= 0) & (x <= width) & (y <= height)
     x, y, = x[inside], y[inside]
-    return np.array([x.min(), y.min(), x.max(), y.max()]) if any(x) else np.zeros(4)  # xyxy
+    return np.array([x.min(), y.min(), x.max(), y.max()], dtype=segment.dtype) if any(x) else np.zeros(
+        4, dtype=segment.dtype)  # xyxy
 
 
 def scale_boxes(img1_shape, boxes, img0_shape, ratio_pad=None):
     """
     Rescales bounding boxes (in the format of xyxy) from the shape of the image they were originally specified in
     (img1_shape) to the shape of a different image (img0_shape).
 
@@ -115,18 +116,18 @@
 
 def make_divisible(x, divisor):
     """
     Returns the nearest number that is divisible by the given divisor.
 
     Args:
         x (int): The number to make divisible.
-        divisor (int or torch.Tensor): The divisor.
+        divisor (int) or (torch.Tensor): The divisor.
 
     Returns:
-        int: The nearest number divisible by the divisor.
+        (int): The nearest number divisible by the divisor.
     """
     if isinstance(divisor, torch.Tensor):
         divisor = int(divisor.max())  # to int
     return math.ceil(x / divisor) * divisor
 
 
 def non_max_suppression(
@@ -134,36 +135,42 @@
         conf_thres=0.25,
         iou_thres=0.45,
         classes=None,
         agnostic=False,
         multi_label=False,
         labels=(),
         max_det=300,
-        nm=0,  # number of masks
+        nc=0,  # number of classes (optional)
+        max_time_img=0.05,
+        max_nms=30000,
+        max_wh=7680,
 ):
     """
     Perform non-maximum suppression (NMS) on a set of boxes, with support for masks and multiple labels per box.
 
     Arguments:
-        prediction (torch.Tensor): A tensor of shape (batch_size, num_boxes, num_classes + 4 + num_masks)
+        prediction (torch.Tensor): A tensor of shape (batch_size, num_classes + 4 + num_masks, num_boxes)
             containing the predicted boxes, classes, and masks. The tensor should be in the format
             output by a model, such as YOLO.
         conf_thres (float): The confidence threshold below which boxes will be filtered out.
             Valid values are between 0.0 and 1.0.
         iou_thres (float): The IoU threshold below which boxes will be filtered out during NMS.
             Valid values are between 0.0 and 1.0.
         classes (List[int]): A list of class indices to consider. If None, all classes will be considered.
         agnostic (bool): If True, the model is agnostic to the number of classes, and all
             classes will be considered as one.
         multi_label (bool): If True, each box may have multiple labels.
         labels (List[List[Union[int, float, torch.Tensor]]]): A list of lists, where each inner
             list contains the apriori labels for a given image. The list should be in the format
             output by a dataloader, with each label being a tuple of (class_index, x1, y1, x2, y2).
         max_det (int): The maximum number of boxes to keep after NMS.
-        nm (int): The number of masks output by the model.
+        nc (int): (optional) The number of classes output by the model. Any indices after this will be considered masks.
+        max_time_img (float): The maximum time (seconds) for processing one image.
+        max_nms (int): The maximum number of boxes into torchvision.ops.nms().
+        max_wh (int): The maximum box width and height in pixels
 
     Returns:
         (List[torch.Tensor]): A list of length batch_size, where each element is a tensor of
             shape (num_boxes, 6 + num_masks) containing the kept boxes, with columns
             (x1, y1, x2, y2, confidence, class, mask1, mask2, ...).
     """
 
@@ -174,23 +181,22 @@
         prediction = prediction[0]  # select only inference output
 
     device = prediction.device
     mps = 'mps' in device.type  # Apple MPS
     if mps:  # MPS not fully supported yet, convert tensors to CPU before NMS
         prediction = prediction.cpu()
     bs = prediction.shape[0]  # batch size
-    nc = prediction.shape[1] - nm - 4  # number of classes
+    nc = nc or (prediction.shape[1] - 4)  # number of classes
+    nm = prediction.shape[1] - nc - 4
     mi = 4 + nc  # mask start index
     xc = prediction[:, 4:mi].amax(1) > conf_thres  # candidates
 
     # Settings
     # min_wh = 2  # (pixels) minimum box width and height
-    max_wh = 7680  # (pixels) maximum box width and height
-    max_nms = 30000  # maximum number of boxes into torchvision.ops.nms()
-    time_limit = 0.5 + 0.05 * bs  # seconds to quit after
+    time_limit = 0.5 + max_time_img * bs  # seconds to quit after
     redundant = True  # require redundant detections
     multi_label &= nc > 1  # multiple labels per box (adds 0.5ms/img)
     merge = False  # use merge-NMS
 
     t = time.time()
     output = [torch.zeros((0, 6 + nm), device=prediction.device)] * bs
     for xi, x in enumerate(prediction):  # image index, image inference
@@ -236,15 +242,15 @@
 
         # Batched NMS
         c = x[:, 5:6] * (0 if agnostic else max_wh)  # classes
         boxes, scores = x[:, :4] + c, x[:, 4]  # boxes (offset by class), scores
         i = torchvision.ops.nms(boxes, scores, iou_thres)  # NMS
         i = i[:max_det]  # limit detections
         if merge and (1 < n < 3E3):  # Merge NMS (boxes merged using weighted mean)
-            # update boxes as boxes(i,4) = weights(i,n) * boxes(n,4)
+            # Update boxes as boxes(i,4) = weights(i,n) * boxes(n,4)
             iou = box_iou(boxes[i], boxes) > iou_thres  # iou matrix
             weights = iou * scores[None]  # box weights
             x[i, :4] = torch.mm(weights, x[:, :4]).float() / weights.sum(1, keepdim=True)  # merged boxes
             if redundant:
                 i = i[iou.sum(1) > 1]  # require redundancy
 
         output[xi] = x[i]
@@ -272,70 +278,68 @@
         boxes[..., 2].clamp_(0, shape[1])  # x2
         boxes[..., 3].clamp_(0, shape[0])  # y2
     else:  # np.array (faster grouped)
         boxes[..., [0, 2]] = boxes[..., [0, 2]].clip(0, shape[1])  # x1, x2
         boxes[..., [1, 3]] = boxes[..., [1, 3]].clip(0, shape[0])  # y1, y2
 
 
-def clip_coords(boxes, shape):
+def clip_coords(coords, shape):
     """
-    Clip bounding xyxy bounding boxes to image shape (height, width).
+    Clip line coordinates to the image boundaries.
 
     Args:
-        boxes (torch.Tensor or numpy.ndarray): Bounding boxes to be clipped.
-        shape (tuple): The shape of the image. (height, width)
+        coords (torch.Tensor) or (numpy.ndarray): A list of line coordinates.
+        shape (tuple): A tuple of integers representing the size of the image in the format (height, width).
 
     Returns:
-        None
-
-    Note:
-        The input `boxes` is modified in-place, there is no return value.
+        (None): The function modifies the input `coordinates` in place, by clipping each coordinate to the image boundaries.
     """
-    if isinstance(boxes, torch.Tensor):  # faster individually
-        boxes[:, 0].clamp_(0, shape[1])  # x1
-        boxes[:, 1].clamp_(0, shape[0])  # y1
-        boxes[:, 2].clamp_(0, shape[1])  # x2
-        boxes[:, 3].clamp_(0, shape[0])  # y2
+    if isinstance(coords, torch.Tensor):  # faster individually
+        coords[..., 0].clamp_(0, shape[1])  # x
+        coords[..., 1].clamp_(0, shape[0])  # y
     else:  # np.array (faster grouped)
-        boxes[:, [0, 2]] = boxes[:, [0, 2]].clip(0, shape[1])  # x1, x2
-        boxes[:, [1, 3]] = boxes[:, [1, 3]].clip(0, shape[0])  # y1, y2
+        coords[..., 0] = coords[..., 0].clip(0, shape[1])  # x
+        coords[..., 1] = coords[..., 1].clip(0, shape[0])  # y
 
 
-def scale_image(im1_shape, masks, im0_shape, ratio_pad=None):
+def scale_image(masks, im0_shape, ratio_pad=None):
     """
     Takes a mask, and resizes it to the original image size
 
     Args:
-      im1_shape (tuple): model input shape, [h, w]
-      masks (torch.Tensor): [h, w, num]
+      masks (torch.Tensor): resized and padded masks/images, [h, w, num]/[h, w, 3].
       im0_shape (tuple): the original image shape
       ratio_pad (tuple): the ratio of the padding to the original image.
 
     Returns:
       masks (torch.Tensor): The masks that are being returned.
     """
     # Rescale coordinates (xyxy) from im1_shape to im0_shape
+    im1_shape = masks.shape
+    if im1_shape[:2] == im0_shape[:2]:
+        return masks
     if ratio_pad is None:  # calculate from im0_shape
         gain = min(im1_shape[0] / im0_shape[0], im1_shape[1] / im0_shape[1])  # gain  = old / new
         pad = (im1_shape[1] - im0_shape[1] * gain) / 2, (im1_shape[0] - im0_shape[0] * gain) / 2  # wh padding
     else:
+        gain = ratio_pad[0][0]
         pad = ratio_pad[1]
     top, left = int(pad[1]), int(pad[0])  # y, x
     bottom, right = int(im1_shape[0] - pad[1]), int(im1_shape[1] - pad[0])
 
     if len(masks.shape) < 2:
         raise ValueError(f'"len of masks shape" should be 2 or 3, but got {len(masks.shape)}')
     masks = masks[top:bottom, left:right]
     # masks = masks.permute(2, 0, 1).contiguous()
     # masks = F.interpolate(masks[None], im0_shape[:2], mode='bilinear', align_corners=False)[0]
     # masks = masks.permute(1, 2, 0).contiguous()
     masks = cv2.resize(masks, (im0_shape[1], im0_shape[0]))
-
     if len(masks.shape) == 2:
         masks = masks[:, :, None]
+
     return masks
 
 
 def xyxy2xywh(x):
     """
     Convert bounding box coordinates from (x1, y1, x2, y2) format to (x, y, width, height) format.
 
@@ -522,15 +526,16 @@
     Returns:
       segments (list): the resampled segments.
     """
     for i, s in enumerate(segments):
         s = np.concatenate((s, s[0:1, :]), axis=0)
         x = np.linspace(0, len(s) - 1, n)
         xp = np.arange(len(s))
-        segments[i] = np.concatenate([np.interp(x, xp, s[:, i]) for i in range(2)]).reshape(2, -1).T  # segment xy
+        segments[i] = np.concatenate([np.interp(x, xp, s[:, i]) for i in range(2)],
+                                     dtype=np.float32).reshape(2, -1).T  # segment xy
     return segments
 
 
 def crop_mask(masks, boxes):
     """
     It takes a mask and a bounding box, and returns a mask that is cropped to the bounding box
 
@@ -538,17 +543,17 @@
       masks (torch.Tensor): [h, w, n] tensor of masks
       boxes (torch.Tensor): [n, 4] tensor of bbox coordinates in relative point form
 
     Returns:
       (torch.Tensor): The masks are being cropped to the bounding box.
     """
     n, h, w = masks.shape
-    x1, y1, x2, y2 = torch.chunk(boxes[:, :, None], 4, 1)  # x1 shape(1,1,n)
-    r = torch.arange(w, device=masks.device, dtype=x1.dtype)[None, None, :]  # rows shape(1,w,1)
-    c = torch.arange(h, device=masks.device, dtype=x1.dtype)[None, :, None]  # cols shape(h,1,1)
+    x1, y1, x2, y2 = torch.chunk(boxes[:, :, None], 4, 1)  # x1 shape(n,1,1)
+    r = torch.arange(w, device=masks.device, dtype=x1.dtype)[None, None, :]  # rows shape(1,1,w)
+    c = torch.arange(h, device=masks.device, dtype=x1.dtype)[None, :, None]  # cols shape(1,h,1)
 
     return masks * ((r >= x1) * (r < x2) * (c >= y1) * (c < y2))
 
 
 def process_mask_upsample(protos, masks_in, bboxes, shape):
     """
     It takes the output of the mask head, and applies the mask to the bounding boxes. This produces masks of higher
@@ -568,25 +573,26 @@
     masks = F.interpolate(masks[None], shape, mode='bilinear', align_corners=False)[0]  # CHW
     masks = crop_mask(masks, bboxes)  # CHW
     return masks.gt_(0.5)
 
 
 def process_mask(protos, masks_in, bboxes, shape, upsample=False):
     """
-    It takes the output of the mask head, and applies the mask to the bounding boxes. This is faster but produces
-    downsampled quality of mask
+    Apply masks to bounding boxes using the output of the mask head.
 
     Args:
-      protos (torch.Tensor): [mask_dim, mask_h, mask_w]
-      masks_in (torch.Tensor): [n, mask_dim], n is number of masks after nms
-      bboxes (torch.Tensor): [n, 4], n is number of masks after nms
-      shape (tuple): the size of the input image (h,w)
+        protos (torch.Tensor): A tensor of shape [mask_dim, mask_h, mask_w].
+        masks_in (torch.Tensor): A tensor of shape [n, mask_dim], where n is the number of masks after NMS.
+        bboxes (torch.Tensor): A tensor of shape [n, 4], where n is the number of masks after NMS.
+        shape (tuple): A tuple of integers representing the size of the input image in the format (h, w).
+        upsample (bool): A flag to indicate whether to upsample the mask to the original image size. Default is False.
 
     Returns:
-      (torch.Tensor): The processed masks.
+        (torch.Tensor): A binary mask tensor of shape [n, h, w], where n is the number of masks after NMS, and h and w
+            are the height and width of the input image. The mask is applied to the bounding boxes.
     """
 
     c, mh, mw = protos.shape  # CHW
     ih, iw = shape
     masks = (masks_in @ protos.float().view(c, -1)).sigmoid().view(-1, mh, mw)  # CHW
 
     downsampled_bboxes = bboxes.clone()
@@ -623,43 +629,44 @@
     masks = masks[:, top:bottom, left:right]
 
     masks = F.interpolate(masks[None], shape, mode='bilinear', align_corners=False)[0]  # CHW
     masks = crop_mask(masks, bboxes)  # CHW
     return masks.gt_(0.5)
 
 
-def scale_segments(img1_shape, segments, img0_shape, ratio_pad=None, normalize=False):
+def scale_coords(img1_shape, coords, img0_shape, ratio_pad=None, normalize=False):
     """
     Rescale segment coordinates (xyxy) from img1_shape to img0_shape
 
     Args:
-      img1_shape (tuple): The shape of the image that the segments are from.
-      segments (torch.Tensor): the segments to be scaled
+      img1_shape (tuple): The shape of the image that the coords are from.
+      coords (torch.Tensor): the coords to be scaled
       img0_shape (tuple): the shape of the image that the segmentation is being applied to
       ratio_pad (tuple): the ratio of the image size to the padded image size.
       normalize (bool): If True, the coordinates will be normalized to the range [0, 1]. Defaults to False
 
     Returns:
-      segments (torch.Tensor): the segmented image.
+      coords (torch.Tensor): the segmented image.
     """
     if ratio_pad is None:  # calculate from img0_shape
         gain = min(img1_shape[0] / img0_shape[0], img1_shape[1] / img0_shape[1])  # gain  = old / new
         pad = (img1_shape[1] - img0_shape[1] * gain) / 2, (img1_shape[0] - img0_shape[0] * gain) / 2  # wh padding
     else:
         gain = ratio_pad[0][0]
         pad = ratio_pad[1]
 
-    segments[:, 0] -= pad[0]  # x padding
-    segments[:, 1] -= pad[1]  # y padding
-    segments /= gain
-    clip_segments(segments, img0_shape)
+    coords[..., 0] -= pad[0]  # x padding
+    coords[..., 1] -= pad[1]  # y padding
+    coords[..., 0] /= gain
+    coords[..., 1] /= gain
+    clip_coords(coords, img0_shape)
     if normalize:
-        segments[:, 0] /= img0_shape[1]  # width
-        segments[:, 1] /= img0_shape[0]  # height
-    return segments
+        coords[..., 0] /= img0_shape[1]  # width
+        coords[..., 1] /= img0_shape[0]  # height
+    return coords
 
 
 def masks2segments(masks, strategy='largest'):
     """
     It takes a list of masks(n,h,w) and returns a list of segments(n,xy)
 
     Args:
@@ -679,35 +686,18 @@
                 c = np.array(c[np.array([len(x) for x in c]).argmax()]).reshape(-1, 2)
         else:
             c = np.zeros((0, 2))  # no segments found
         segments.append(c.astype('float32'))
     return segments
 
 
-def clip_segments(segments, shape):
-    """
-    It takes a list of line segments (x1,y1,x2,y2) and clips them to the image shape (height, width)
-
-    Args:
-      segments (list): a list of segments, each segment is a list of points, each point is a list of x,y
-    coordinates
-      shape (tuple): the shape of the image
-    """
-    if isinstance(segments, torch.Tensor):  # faster individually
-        segments[:, 0].clamp_(0, shape[1])  # x
-        segments[:, 1].clamp_(0, shape[0])  # y
-    else:  # np.array (faster grouped)
-        segments[:, 0] = segments[:, 0].clip(0, shape[1])  # x
-        segments[:, 1] = segments[:, 1].clip(0, shape[0])  # y
-
-
 def clean_str(s):
     """
     Cleans a string by replacing special characters with underscore _
 
     Args:
       s (str): a string needing special characters replaced
 
     Returns:
       (str): a string with special characters replaced by an underscore _
     """
-    return re.sub(pattern="[|@#!¡·$€%&()=?¿^*;:,¨´><+]", repl="_", string=s)
+    return re.sub(pattern='[|@#!¡·$€%&()=?¿^*;:,¨´><+]', repl='_', string=s)
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/utils/tal.py` & `ultralytics-8.0.90/ultralytics/yolo/utils/tal.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from .checks import check_version
 from .metrics import bbox_iou
@@ -44,47 +44,64 @@
     if fg_mask.max() > 1:  # one anchor is assigned to multiple gt_bboxes
         mask_multi_gts = (fg_mask.unsqueeze(1) > 1).repeat([1, n_max_boxes, 1])  # (b, n_max_boxes, h*w)
         max_overlaps_idx = overlaps.argmax(1)  # (b, h*w)
         is_max_overlaps = F.one_hot(max_overlaps_idx, n_max_boxes)  # (b, h*w, n_max_boxes)
         is_max_overlaps = is_max_overlaps.permute(0, 2, 1).to(overlaps.dtype)  # (b, n_max_boxes, h*w)
         mask_pos = torch.where(mask_multi_gts, is_max_overlaps, mask_pos)  # (b, n_max_boxes, h*w)
         fg_mask = mask_pos.sum(-2)
-    # find each grid serve which gt(index)
+    # Find each grid serve which gt(index)
     target_gt_idx = mask_pos.argmax(-2)  # (b, h*w)
     return target_gt_idx, fg_mask, mask_pos
 
 
 class TaskAlignedAssigner(nn.Module):
+    """
+    A task-aligned assigner for object detection.
+
+    This class assigns ground-truth (gt) objects to anchors based on the task-aligned metric,
+    which combines both classification and localization information.
+
+    Attributes:
+        topk (int): The number of top candidates to consider.
+        num_classes (int): The number of object classes.
+        alpha (float): The alpha parameter for the classification component of the task-aligned metric.
+        beta (float): The beta parameter for the localization component of the task-aligned metric.
+        eps (float): A small value to prevent division by zero.
+    """
 
     def __init__(self, topk=13, num_classes=80, alpha=1.0, beta=6.0, eps=1e-9):
+        """Initialize a TaskAlignedAssigner object with customizable hyperparameters."""
         super().__init__()
         self.topk = topk
         self.num_classes = num_classes
         self.bg_idx = num_classes
         self.alpha = alpha
         self.beta = beta
         self.eps = eps
 
     @torch.no_grad()
     def forward(self, pd_scores, pd_bboxes, anc_points, gt_labels, gt_bboxes, mask_gt):
-        """This code referenced to
-           https://github.com/Nioolek/PPYOLOE_pytorch/blob/master/ppyoloe/assigner/tal_assigner.py
+        """
+        Compute the task-aligned assignment.
+        Reference https://github.com/Nioolek/PPYOLOE_pytorch/blob/master/ppyoloe/assigner/tal_assigner.py
 
         Args:
             pd_scores (Tensor): shape(bs, num_total_anchors, num_classes)
             pd_bboxes (Tensor): shape(bs, num_total_anchors, 4)
             anc_points (Tensor): shape(num_total_anchors, 2)
             gt_labels (Tensor): shape(bs, n_max_boxes, 1)
             gt_bboxes (Tensor): shape(bs, n_max_boxes, 4)
             mask_gt (Tensor): shape(bs, n_max_boxes, 1)
+
         Returns:
             target_labels (Tensor): shape(bs, num_total_anchors)
             target_bboxes (Tensor): shape(bs, num_total_anchors, 4)
             target_scores (Tensor): shape(bs, num_total_anchors, num_classes)
             fg_mask (Tensor): shape(bs, num_total_anchors)
+            target_gt_idx (Tensor): shape(bs, num_total_anchors)
         """
         self.bs = pd_scores.size(0)
         self.n_max_boxes = gt_bboxes.size(1)
 
         if self.n_max_boxes == 0:
             device = gt_bboxes.device
             return (torch.full_like(pd_scores[..., 0], self.bg_idx).to(device), torch.zeros_like(pd_bboxes).to(device),
@@ -92,89 +109,127 @@
                     torch.zeros_like(pd_scores[..., 0]).to(device))
 
         mask_pos, align_metric, overlaps = self.get_pos_mask(pd_scores, pd_bboxes, gt_labels, gt_bboxes, anc_points,
                                                              mask_gt)
 
         target_gt_idx, fg_mask, mask_pos = select_highest_overlaps(mask_pos, overlaps, self.n_max_boxes)
 
-        # assigned target
+        # Assigned target
         target_labels, target_bboxes, target_scores = self.get_targets(gt_labels, gt_bboxes, target_gt_idx, fg_mask)
 
-        # normalize
+        # Normalize
         align_metric *= mask_pos
         pos_align_metrics = align_metric.amax(axis=-1, keepdim=True)  # b, max_num_obj
         pos_overlaps = (overlaps * mask_pos).amax(axis=-1, keepdim=True)  # b, max_num_obj
         norm_align_metric = (align_metric * pos_overlaps / (pos_align_metrics + self.eps)).amax(-2).unsqueeze(-1)
         target_scores = target_scores * norm_align_metric
 
         return target_labels, target_bboxes, target_scores, fg_mask.bool(), target_gt_idx
 
     def get_pos_mask(self, pd_scores, pd_bboxes, gt_labels, gt_bboxes, anc_points, mask_gt):
-        # get anchor_align metric, (b, max_num_obj, h*w)
-        align_metric, overlaps = self.get_box_metrics(pd_scores, pd_bboxes, gt_labels, gt_bboxes)
-        # get in_gts mask, (b, max_num_obj, h*w)
+        """Get in_gts mask, (b, max_num_obj, h*w)."""
         mask_in_gts = select_candidates_in_gts(anc_points, gt_bboxes)
-        # get topk_metric mask, (b, max_num_obj, h*w)
-        mask_topk = self.select_topk_candidates(align_metric * mask_in_gts,
-                                                topk_mask=mask_gt.repeat([1, 1, self.topk]).bool())
-        # merge all mask to a final mask, (b, max_num_obj, h*w)
+        # Get anchor_align metric, (b, max_num_obj, h*w)
+        align_metric, overlaps = self.get_box_metrics(pd_scores, pd_bboxes, gt_labels, gt_bboxes, mask_in_gts * mask_gt)
+        # Get topk_metric mask, (b, max_num_obj, h*w)
+        mask_topk = self.select_topk_candidates(align_metric, topk_mask=mask_gt.repeat([1, 1, self.topk]).bool())
+        # Merge all mask to a final mask, (b, max_num_obj, h*w)
         mask_pos = mask_topk * mask_in_gts * mask_gt
 
         return mask_pos, align_metric, overlaps
 
-    def get_box_metrics(self, pd_scores, pd_bboxes, gt_labels, gt_bboxes):
+    def get_box_metrics(self, pd_scores, pd_bboxes, gt_labels, gt_bboxes, mask_gt):
+        """Compute alignment metric given predicted and ground truth bounding boxes."""
+        na = pd_bboxes.shape[-2]
+        mask_gt = mask_gt.bool()  # b, max_num_obj, h*w
+        overlaps = torch.zeros([self.bs, self.n_max_boxes, na], dtype=pd_bboxes.dtype, device=pd_bboxes.device)
+        bbox_scores = torch.zeros([self.bs, self.n_max_boxes, na], dtype=pd_scores.dtype, device=pd_scores.device)
+
         ind = torch.zeros([2, self.bs, self.n_max_boxes], dtype=torch.long)  # 2, b, max_num_obj
         ind[0] = torch.arange(end=self.bs).view(-1, 1).repeat(1, self.n_max_boxes)  # b, max_num_obj
         ind[1] = gt_labels.long().squeeze(-1)  # b, max_num_obj
-        # get the scores of each grid for each gt cls
-        bbox_scores = pd_scores[ind[0], :, ind[1]]  # b, max_num_obj, h*w
+        # Get the scores of each grid for each gt cls
+        bbox_scores[mask_gt] = pd_scores[ind[0], :, ind[1]][mask_gt]  # b, max_num_obj, h*w
+
+        # (b, max_num_obj, 1, 4), (b, 1, h*w, 4)
+        pd_boxes = pd_bboxes.unsqueeze(1).repeat(1, self.n_max_boxes, 1, 1)[mask_gt]
+        gt_boxes = gt_bboxes.unsqueeze(2).repeat(1, 1, na, 1)[mask_gt]
+        overlaps[mask_gt] = bbox_iou(gt_boxes, pd_boxes, xywh=False, CIoU=True).squeeze(-1).clamp(0)
 
-        overlaps = bbox_iou(gt_bboxes.unsqueeze(2), pd_bboxes.unsqueeze(1), xywh=False, CIoU=True).squeeze(3).clamp(0)
         align_metric = bbox_scores.pow(self.alpha) * overlaps.pow(self.beta)
         return align_metric, overlaps
 
     def select_topk_candidates(self, metrics, largest=True, topk_mask=None):
         """
+        Select the top-k candidates based on the given metrics.
+
         Args:
-            metrics: (b, max_num_obj, h*w).
-            topk_mask: (b, max_num_obj, topk) or None
+            metrics (Tensor): A tensor of shape (b, max_num_obj, h*w), where b is the batch size,
+                              max_num_obj is the maximum number of objects, and h*w represents the
+                              total number of anchor points.
+            largest (bool): If True, select the largest values; otherwise, select the smallest values.
+            topk_mask (Tensor): An optional boolean tensor of shape (b, max_num_obj, topk), where
+                                topk is the number of top candidates to consider. If not provided,
+                                the top-k values are automatically computed based on the given metrics.
+
+        Returns:
+            (Tensor): A tensor of shape (b, max_num_obj, h*w) containing the selected top-k candidates.
         """
 
         num_anchors = metrics.shape[-1]  # h*w
         # (b, max_num_obj, topk)
         topk_metrics, topk_idxs = torch.topk(metrics, self.topk, dim=-1, largest=largest)
         if topk_mask is None:
             topk_mask = (topk_metrics.max(-1, keepdim=True) > self.eps).tile([1, 1, self.topk])
         # (b, max_num_obj, topk)
-        topk_idxs = torch.where(topk_mask, topk_idxs, 0)
+        topk_idxs[~topk_mask] = 0
         # (b, max_num_obj, topk, h*w) -> (b, max_num_obj, h*w)
-        is_in_topk = F.one_hot(topk_idxs, num_anchors).sum(-2)
+        is_in_topk = torch.zeros(metrics.shape, dtype=torch.long, device=metrics.device)
+        for it in range(self.topk):
+            is_in_topk += F.one_hot(topk_idxs[:, :, it], num_anchors)
+        # is_in_topk = F.one_hot(topk_idxs, num_anchors).sum(-2)
         # filter invalid bboxes
         is_in_topk = torch.where(is_in_topk > 1, 0, is_in_topk)
         return is_in_topk.to(metrics.dtype)
 
     def get_targets(self, gt_labels, gt_bboxes, target_gt_idx, fg_mask):
         """
+        Compute target labels, target bounding boxes, and target scores for the positive anchor points.
+
         Args:
-            gt_labels: (b, max_num_obj, 1)
-            gt_bboxes: (b, max_num_obj, 4)
-            target_gt_idx: (b, h*w)
-            fg_mask: (b, h*w)
+            gt_labels (Tensor): Ground truth labels of shape (b, max_num_obj, 1), where b is the
+                                batch size and max_num_obj is the maximum number of objects.
+            gt_bboxes (Tensor): Ground truth bounding boxes of shape (b, max_num_obj, 4).
+            target_gt_idx (Tensor): Indices of the assigned ground truth objects for positive
+                                    anchor points, with shape (b, h*w), where h*w is the total
+                                    number of anchor points.
+            fg_mask (Tensor): A boolean tensor of shape (b, h*w) indicating the positive
+                              (foreground) anchor points.
+
+        Returns:
+            (Tuple[Tensor, Tensor, Tensor]): A tuple containing the following tensors:
+                - target_labels (Tensor): Shape (b, h*w), containing the target labels for
+                                          positive anchor points.
+                - target_bboxes (Tensor): Shape (b, h*w, 4), containing the target bounding boxes
+                                          for positive anchor points.
+                - target_scores (Tensor): Shape (b, h*w, num_classes), containing the target scores
+                                          for positive anchor points, where num_classes is the number
+                                          of object classes.
         """
 
-        # assigned target labels, (b, 1)
+        # Assigned target labels, (b, 1)
         batch_ind = torch.arange(end=self.bs, dtype=torch.int64, device=gt_labels.device)[..., None]
         target_gt_idx = target_gt_idx + batch_ind * self.n_max_boxes  # (b, h*w)
         target_labels = gt_labels.long().flatten()[target_gt_idx]  # (b, h*w)
 
-        # assigned target boxes, (b, max_num_obj, 4) -> (b, h*w)
+        # Assigned target boxes, (b, max_num_obj, 4) -> (b, h*w)
         target_bboxes = gt_bboxes.view(-1, 4)[target_gt_idx]
 
-        # assigned target scores
-        target_labels.clamp(0)
+        # Assigned target scores
+        target_labels.clamp_(0)
         target_scores = F.one_hot(target_labels, self.num_classes)  # (b, h*w, 80)
         fg_scores_mask = fg_mask[:, :, None].repeat(1, 1, self.num_classes)  # (b, h*w, 80)
         target_scores = torch.where(fg_scores_mask > 0, target_scores, 0)
 
         return target_labels, target_bboxes, target_scores
 
 
@@ -191,21 +246,21 @@
         anchor_points.append(torch.stack((sx, sy), -1).view(-1, 2))
         stride_tensor.append(torch.full((h * w, 1), stride, dtype=dtype, device=device))
     return torch.cat(anchor_points), torch.cat(stride_tensor)
 
 
 def dist2bbox(distance, anchor_points, xywh=True, dim=-1):
     """Transform distance(ltrb) to box(xywh or xyxy)."""
-    lt, rb = torch.split(distance, 2, dim)
+    lt, rb = distance.chunk(2, dim)
     x1y1 = anchor_points - lt
     x2y2 = anchor_points + rb
     if xywh:
         c_xy = (x1y1 + x2y2) / 2
         wh = x2y2 - x1y1
         return torch.cat((c_xy, wh), dim)  # xywh bbox
     return torch.cat((x1y1, x2y2), dim)  # xyxy bbox
 
 
 def bbox2dist(anchor_points, bbox, reg_max):
     """Transform bbox(xyxy) to dist(ltrb)."""
-    x1y1, x2y2 = torch.split(bbox, 2, -1)
+    x1y1, x2y2 = bbox.chunk(2, -1)
     return torch.cat((anchor_points - x1y1, x2y2 - anchor_points), -1).clamp(0, reg_max - 0.01)  # dist (lt, rb)
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/utils/torch_utils.py` & `ultralytics-8.0.90/ultralytics/yolo/utils/torch_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,112 +1,116 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import math
 import os
 import platform
 import random
 import time
 from contextlib import contextmanager
 from copy import deepcopy
 from pathlib import Path
+from typing import Union
 
 import numpy as np
 import thop
 import torch
 import torch.distributed as dist
 import torch.nn as nn
 import torch.nn.functional as F
-from torch.nn.parallel import DistributedDataParallel as DDP
+import torchvision
 
-import ultralytics
-from ultralytics.yolo.utils import DEFAULT_CONFIG_DICT, DEFAULT_CONFIG_KEYS, LOGGER
-from ultralytics.yolo.utils.checks import git_describe
+from ultralytics.yolo.utils import DEFAULT_CFG_DICT, DEFAULT_CFG_KEYS, LOGGER, RANK, __version__
+from ultralytics.yolo.utils.checks import check_version
 
-from .checks import check_version
-
-LOCAL_RANK = int(os.getenv('LOCAL_RANK', -1))  # https://pytorch.org/docs/stable/elastic/run.html
-RANK = int(os.getenv('RANK', -1))
-WORLD_SIZE = int(os.getenv('WORLD_SIZE', 1))
+TORCHVISION_0_10 = check_version(torchvision.__version__, '0.10.0')
+TORCH_1_9 = check_version(torch.__version__, '1.9.0')
+TORCH_1_11 = check_version(torch.__version__, '1.11.0')
+TORCH_1_12 = check_version(torch.__version__, '1.12.0')
+TORCH_2_X = check_version(torch.__version__, minimum='2.0')
 
 
 @contextmanager
 def torch_distributed_zero_first(local_rank: int):
-    # Decorator to make all processes in distributed training wait for each local_master to do something
-    initialized = torch.distributed.is_initialized()  # prevent 'Default process group has not been initialized' errors
-    if initialized and local_rank not in {-1, 0}:
+    """Decorator to make all processes in distributed training wait for each local_master to do something."""
+    initialized = torch.distributed.is_available() and torch.distributed.is_initialized()
+    if initialized and local_rank not in (-1, 0):
         dist.barrier(device_ids=[local_rank])
     yield
     if initialized and local_rank == 0:
         dist.barrier(device_ids=[0])
 
 
-def smart_inference_mode(torch_1_9=check_version(torch.__version__, '1.9.0')):
-    # Applies torch.inference_mode() decorator if torch>=1.9.0 else torch.no_grad() decorator
+def smart_inference_mode():
+    """Applies torch.inference_mode() decorator if torch>=1.9.0 else torch.no_grad() decorator."""
+
     def decorate(fn):
-        return (torch.inference_mode if torch_1_9 else torch.no_grad)()(fn)
+        """Applies appropriate torch decorator for inference mode based on torch version."""
+        return (torch.inference_mode if TORCH_1_9 else torch.no_grad)()(fn)
 
     return decorate
 
 
-def DDP_model(model):
-    # Model DDP creation with checks
-    assert not check_version(torch.__version__, '1.12.0', pinned=True), \
-        'torch==1.12.0 torchvision==0.13.0 DDP training is not supported due to a known issue. ' \
-        'Please upgrade or downgrade torch to use DDP. See https://github.com/ultralytics/yolov5/issues/8395'
-    if check_version(torch.__version__, '1.11.0'):
-        return DDP(model, device_ids=[LOCAL_RANK], output_device=LOCAL_RANK, static_graph=True)
-    else:
-        return DDP(model, device_ids=[LOCAL_RANK], output_device=LOCAL_RANK)
-
-
-def select_device(device='', batch_size=0, newline=False):
-    # device = None or 'cpu' or 0 or '0' or '0,1,2,3'
-    ver = git_describe() or ultralytics.__version__  # git commit or pip package version
-    s = f'Ultralytics YOLOv{ver} 🚀 Python-{platform.python_version()} torch-{torch.__version__} '
-    device = str(device).strip().lower().replace('cuda:', '').replace('none', '')  # to string, 'cuda:0' to '0'
+def select_device(device='', batch=0, newline=False, verbose=True):
+    """Selects PyTorch Device. Options are device = None or 'cpu' or 0 or '0' or '0,1,2,3'."""
+    s = f'Ultralytics YOLOv{__version__} 🚀 Python-{platform.python_version()} torch-{torch.__version__} '
+    device = str(device).lower()
+    for remove in 'cuda:', 'none', '(', ')', '[', ']', "'", ' ':
+        device = device.replace(remove, '')  # to string, 'cuda:0' -> '0' and '(0, 1)' -> '0,1'
     cpu = device == 'cpu'
     mps = device == 'mps'  # Apple Metal Performance Shaders (MPS)
     if cpu or mps:
         os.environ['CUDA_VISIBLE_DEVICES'] = '-1'  # force torch.cuda.is_available() = False
     elif device:  # non-cpu device requested
+        visible = os.environ.get('CUDA_VISIBLE_DEVICES', None)
         os.environ['CUDA_VISIBLE_DEVICES'] = device  # set environment variable - must be before assert is_available()
-        assert torch.cuda.is_available() and torch.cuda.device_count() >= len(device.replace(',', '')), \
-            f"Invalid CUDA 'device={device}' requested, use 'device=cpu' or pass valid CUDA device(s)"
+        if not (torch.cuda.is_available() and torch.cuda.device_count() >= len(device.replace(',', ''))):
+            LOGGER.info(s)
+            install = 'See https://pytorch.org/get-started/locally/ for up-to-date torch install instructions if no ' \
+                      'CUDA devices are seen by torch.\n' if torch.cuda.device_count() == 0 else ''
+            raise ValueError(f"Invalid CUDA 'device={device}' requested."
+                             f" Use 'device=cpu' or pass valid CUDA device(s) if available,"
+                             f" i.e. 'device=0' or 'device=0,1,2,3' for Multi-GPU.\n"
+                             f'\ntorch.cuda.is_available(): {torch.cuda.is_available()}'
+                             f'\ntorch.cuda.device_count(): {torch.cuda.device_count()}'
+                             f"\nos.environ['CUDA_VISIBLE_DEVICES']: {visible}\n"
+                             f'{install}')
 
     if not cpu and not mps and torch.cuda.is_available():  # prefer GPU if available
         devices = device.split(',') if device else '0'  # range(torch.cuda.device_count())  # i.e. 0,1,6,7
         n = len(devices)  # device count
-        if n > 1 and batch_size > 0:  # check batch_size is divisible by device_count
-            assert batch_size % n == 0, f'batch-size {batch_size} not multiple of GPU count {n}'
+        if n > 1 and batch > 0 and batch % n != 0:  # check batch_size is divisible by device_count
+            raise ValueError(f"'batch={batch}' must be a multiple of GPU count {n}. Try 'batch={batch // n * n}' or "
+                             f"'batch={batch // n * n + n}', the nearest batch sizes evenly divisible by {n}.")
         space = ' ' * (len(s) + 1)
         for i, d in enumerate(devices):
             p = torch.cuda.get_device_properties(i)
             s += f"{'' if i == 0 else space}CUDA:{d} ({p.name}, {p.total_memory / (1 << 20):.0f}MiB)\n"  # bytes to MB
         arg = 'cuda:0'
-    elif mps and getattr(torch, 'has_mps', False) and torch.backends.mps.is_available():  # prefer MPS if available
+    elif mps and getattr(torch, 'has_mps', False) and torch.backends.mps.is_available() and TORCH_2_X:
+        # Prefer MPS if available
         s += 'MPS\n'
         arg = 'mps'
     else:  # revert to CPU
         s += 'CPU\n'
         arg = 'cpu'
 
-    if RANK == -1:
+    if verbose and RANK == -1:
         LOGGER.info(s if newline else s.rstrip())
     return torch.device(arg)
 
 
 def time_sync():
-    # PyTorch-accurate time
+    """PyTorch-accurate time."""
     if torch.cuda.is_available():
         torch.cuda.synchronize()
     return time.time()
 
 
 def fuse_conv_and_bn(conv, bn):
-    # Fuse Conv2d() and BatchNorm2d() layers https://tehnokv.com/posts/fusing-batchnorm-and-conv/
+    """Fuse Conv2d() and BatchNorm2d() layers https://tehnokv.com/posts/fusing-batchnorm-and-conv/."""
     fusedconv = nn.Conv2d(conv.in_channels,
                           conv.out_channels,
                           kernel_size=conv.kernel_size,
                           stride=conv.stride,
                           padding=conv.padding,
                           dilation=conv.dilation,
                           groups=conv.groups,
@@ -121,54 +125,87 @@
     b_conv = torch.zeros(conv.weight.size(0), device=conv.weight.device) if conv.bias is None else conv.bias
     b_bn = bn.bias - bn.weight.mul(bn.running_mean).div(torch.sqrt(bn.running_var + bn.eps))
     fusedconv.bias.copy_(torch.mm(w_bn, b_conv.reshape(-1, 1)).reshape(-1) + b_bn)
 
     return fusedconv
 
 
-def model_info(model, verbose=False, imgsz=640):
-    # Model information. imgsz may be int or list, i.e. imgsz=640 or imgsz=[640, 320]
+def fuse_deconv_and_bn(deconv, bn):
+    """Fuse ConvTranspose2d() and BatchNorm2d() layers."""
+    fuseddconv = nn.ConvTranspose2d(deconv.in_channels,
+                                    deconv.out_channels,
+                                    kernel_size=deconv.kernel_size,
+                                    stride=deconv.stride,
+                                    padding=deconv.padding,
+                                    output_padding=deconv.output_padding,
+                                    dilation=deconv.dilation,
+                                    groups=deconv.groups,
+                                    bias=True).requires_grad_(False).to(deconv.weight.device)
+
+    # Prepare filters
+    w_deconv = deconv.weight.clone().view(deconv.out_channels, -1)
+    w_bn = torch.diag(bn.weight.div(torch.sqrt(bn.eps + bn.running_var)))
+    fuseddconv.weight.copy_(torch.mm(w_bn, w_deconv).view(fuseddconv.weight.shape))
+
+    # Prepare spatial bias
+    b_conv = torch.zeros(deconv.weight.size(1), device=deconv.weight.device) if deconv.bias is None else deconv.bias
+    b_bn = bn.bias - bn.weight.mul(bn.running_mean).div(torch.sqrt(bn.running_var + bn.eps))
+    fuseddconv.bias.copy_(torch.mm(w_bn, b_conv.reshape(-1, 1)).reshape(-1) + b_bn)
+
+    return fuseddconv
+
+
+def model_info(model, detailed=False, verbose=True, imgsz=640):
+    """Model information. imgsz may be int or list, i.e. imgsz=640 or imgsz=[640, 320]."""
+    if not verbose:
+        return
     n_p = get_num_params(model)
     n_g = get_num_gradients(model)  # number gradients
-    if verbose:
-        print(f"{'layer':>5} {'name':>40} {'gradient':>9} {'parameters':>12} {'shape':>20} {'mu':>10} {'sigma':>10}")
+    if detailed:
+        LOGGER.info(
+            f"{'layer':>5} {'name':>40} {'gradient':>9} {'parameters':>12} {'shape':>20} {'mu':>10} {'sigma':>10}")
         for i, (name, p) in enumerate(model.named_parameters()):
             name = name.replace('module_list.', '')
-            print('%5g %40s %9s %12g %20s %10.3g %10.3g' %
-                  (i, name, p.requires_grad, p.numel(), list(p.shape), p.mean(), p.std()))
+            LOGGER.info('%5g %40s %9s %12g %20s %10.3g %10.3g' %
+                        (i, name, p.requires_grad, p.numel(), list(p.shape), p.mean(), p.std()))
 
     flops = get_flops(model, imgsz)
+    fused = ' (fused)' if model.is_fused() else ''
     fs = f', {flops:.1f} GFLOPs' if flops else ''
     m = Path(getattr(model, 'yaml_file', '') or model.yaml.get('yaml_file', '')).stem.replace('yolo', 'YOLO') or 'Model'
-    LOGGER.info(f"{m} summary: {len(list(model.modules()))} layers, {n_p} parameters, {n_g} gradients{fs}")
+    LOGGER.info(f'{m} summary{fused}: {len(list(model.modules()))} layers, {n_p} parameters, {n_g} gradients{fs}')
 
 
 def get_num_params(model):
+    """Return the total number of parameters in a YOLO model."""
     return sum(x.numel() for x in model.parameters())
 
 
 def get_num_gradients(model):
+    """Return the total number of parameters with gradients in a YOLO model."""
     return sum(x.numel() for x in model.parameters() if x.requires_grad)
 
 
 def get_flops(model, imgsz=640):
+    """Return a YOLO model's FLOPs."""
     try:
         model = de_parallel(model)
         p = next(model.parameters())
         stride = max(int(model.stride.max()), 32) if hasattr(model, 'stride') else 32  # max stride
         im = torch.empty((1, p.shape[1], stride, stride), device=p.device)  # input image in BCHW format
-        flops = thop.profile(deepcopy(model), inputs=(im,), verbose=False)[0] / 1E9 * 2  # stride GFLOPs
+        flops = thop.profile(deepcopy(model), inputs=[im], verbose=False)[0] / 1E9 * 2  # stride GFLOPs
         imgsz = imgsz if isinstance(imgsz, list) else [imgsz, imgsz]  # expand if int/float
         flops = flops * imgsz[0] / stride * imgsz[1] / stride  # 640x640 GFLOPs
         return flops
     except Exception:
         return 0
 
 
 def initialize_weights(model):
+    """Initialize model weights to random values."""
     for m in model.modules():
         t = type(m)
         if t is nn.Conv2d:
             pass  # nn.init.kaiming_normal_(m.weight, mode='fan_out', nonlinearity='relu')
         elif t is nn.BatchNorm2d:
             m.eps = 1e-3
             m.momentum = 0.03
@@ -185,166 +222,163 @@
     img = F.interpolate(img, size=s, mode='bilinear', align_corners=False)  # resize
     if not same_shape:  # pad/crop img
         h, w = (math.ceil(x * ratio / gs) * gs for x in (h, w))
     return F.pad(img, [0, w - s[1], 0, h - s[0]], value=0.447)  # value = imagenet mean
 
 
 def make_divisible(x, divisor):
-    # Returns nearest x divisible by divisor
+    """Returns nearest x divisible by divisor."""
     if isinstance(divisor, torch.Tensor):
         divisor = int(divisor.max())  # to int
     return math.ceil(x / divisor) * divisor
 
 
 def copy_attr(a, b, include=(), exclude=()):
-    # Copy attributes from b to a, options to only include [...] and to exclude [...]
+    """Copies attributes from object 'b' to object 'a', with options to include/exclude certain attributes."""
     for k, v in b.__dict__.items():
         if (len(include) and k not in include) or k.startswith('_') or k in exclude:
             continue
         else:
             setattr(a, k, v)
 
 
+def get_latest_opset():
+    """Return second-most (for maturity) recently supported ONNX opset by this version of torch."""
+    return max(int(k[14:]) for k in vars(torch.onnx) if 'symbolic_opset' in k) - 1  # opset
+
+
 def intersect_dicts(da, db, exclude=()):
-    # Dictionary intersection of matching keys and shapes, omitting 'exclude' keys, using da values
+    """Returns a dictionary of intersecting keys with matching shapes, excluding 'exclude' keys, using da values."""
     return {k: v for k, v in da.items() if k in db and all(x not in k for x in exclude) and v.shape == db[k].shape}
 
 
 def is_parallel(model):
-    # Returns True if model is of type DP or DDP
-    return type(model) in (nn.parallel.DataParallel, nn.parallel.DistributedDataParallel)
+    """Returns True if model is of type DP or DDP."""
+    return isinstance(model, (nn.parallel.DataParallel, nn.parallel.DistributedDataParallel))
 
 
 def de_parallel(model):
-    # De-parallelize a model: returns single-GPU model if model is of type DP or DDP
+    """De-parallelize a model: returns single-GPU model if model is of type DP or DDP."""
     return model.module if is_parallel(model) else model
 
 
 def one_cycle(y1=0.0, y2=1.0, steps=100):
-    # lambda function for sinusoidal ramp from y1 to y2 https://arxiv.org/pdf/1812.01187.pdf
+    """Returns a lambda function for sinusoidal ramp from y1 to y2 https://arxiv.org/pdf/1812.01187.pdf."""
     return lambda x: ((1 - math.cos(x * math.pi / steps)) / 2) * (y2 - y1) + y1
 
 
 def init_seeds(seed=0, deterministic=False):
-    # Initialize random number generator (RNG) seeds https://pytorch.org/docs/stable/notes/randomness.html
+    """Initialize random number generator (RNG) seeds https://pytorch.org/docs/stable/notes/randomness.html."""
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
     torch.cuda.manual_seed(seed)
     torch.cuda.manual_seed_all(seed)  # for Multi-GPU, exception safe
     # torch.backends.cudnn.benchmark = True  # AutoBatch problem https://github.com/ultralytics/yolov5/issues/9287
-    if deterministic and check_version(torch.__version__, '1.12.0'):  # https://github.com/ultralytics/yolov5/pull/8213
+    if deterministic and TORCH_1_12:  # https://github.com/ultralytics/yolov5/pull/8213
         torch.use_deterministic_algorithms(True)
         torch.backends.cudnn.deterministic = True
         os.environ['CUBLAS_WORKSPACE_CONFIG'] = ':4096:8'
         os.environ['PYTHONHASHSEED'] = str(seed)
 
 
 class ModelEMA:
-    """ Updated Exponential Moving Average (EMA) from https://github.com/rwightman/pytorch-image-models
+    """Updated Exponential Moving Average (EMA) from https://github.com/rwightman/pytorch-image-models
     Keeps a moving average of everything in the model state_dict (parameters and buffers)
     For EMA details see https://www.tensorflow.org/api_docs/python/tf/train/ExponentialMovingAverage
+    To disable EMA set the `enabled` attribute to `False`.
     """
 
     def __init__(self, model, decay=0.9999, tau=2000, updates=0):
-        # Create EMA
+        """Create EMA."""
         self.ema = deepcopy(de_parallel(model)).eval()  # FP32 EMA
         self.updates = updates  # number of EMA updates
         self.decay = lambda x: decay * (1 - math.exp(-x / tau))  # decay exponential ramp (to help early epochs)
         for p in self.ema.parameters():
             p.requires_grad_(False)
+        self.enabled = True
 
     def update(self, model):
-        # Update EMA parameters
-        self.updates += 1
-        d = self.decay(self.updates)
-
-        msd = de_parallel(model).state_dict()  # model state_dict
-        for k, v in self.ema.state_dict().items():
-            if v.dtype.is_floating_point:  # true for FP16 and FP32
-                v *= d
-                v += (1 - d) * msd[k].detach()
-        # assert v.dtype == msd[k].dtype == torch.float32, f'{k}: EMA {v.dtype} and model {msd[k].dtype} must be FP32'
+        """Update EMA parameters."""
+        if self.enabled:
+            self.updates += 1
+            d = self.decay(self.updates)
+
+            msd = de_parallel(model).state_dict()  # model state_dict
+            for k, v in self.ema.state_dict().items():
+                if v.dtype.is_floating_point:  # true for FP16 and FP32
+                    v *= d
+                    v += (1 - d) * msd[k].detach()
+                    # assert v.dtype == msd[k].dtype == torch.float32, f'{k}: EMA {v.dtype},  model {msd[k].dtype}'
 
     def update_attr(self, model, include=(), exclude=('process_group', 'reducer')):
-        # Update EMA attributes
-        copy_attr(self.ema, model, include, exclude)
+        """Updates attributes and saves stripped model with optimizer removed."""
+        if self.enabled:
+            copy_attr(self.ema, model, include, exclude)
 
 
-def strip_optimizer(f='best.pt', s=''):
+def strip_optimizer(f: Union[str, Path] = 'best.pt', s: str = '') -> None:
     """
     Strip optimizer from 'f' to finalize training, optionally save as 's'.
 
-    Usage:
-        from ultralytics.yolo.utils.torch_utils import strip_optimizer
-        from pathlib import Path
-        for f in Path('/Users/glennjocher/Downloads/weights').glob('*.pt'):
-            strip_optimizer(f)
-
     Args:
-        f (str): file path to model state to strip the optimizer from. Default is 'best.pt'.
-        s (str): file path to save the model with stripped optimizer to. Default is ''. If not provided, the original file will be overwritten.
+        f (str): file path to model to strip the optimizer from. Default is 'best.pt'.
+        s (str): file path to save the model with stripped optimizer to. If not provided, 'f' will be overwritten.
 
     Returns:
         None
+
+    Usage:
+        from pathlib import Path
+        from ultralytics.yolo.utils.torch_utils import strip_optimizer
+        for f in Path('/Users/glennjocher/Downloads/weights').rglob('*.pt'):
+            strip_optimizer(f)
     """
     x = torch.load(f, map_location=torch.device('cpu'))
-    args = {**DEFAULT_CONFIG_DICT, **x['train_args']}  # combine model args with default args, preferring model args
+    args = {**DEFAULT_CFG_DICT, **x['train_args']}  # combine model args with default args, preferring model args
     if x.get('ema'):
         x['model'] = x['ema']  # replace model with ema
     for k in 'optimizer', 'best_fitness', 'ema', 'updates':  # keys
         x[k] = None
     x['epoch'] = -1
     x['model'].half()  # to FP16
     for p in x['model'].parameters():
         p.requires_grad = False
-    x['train_args'] = {k: v for k, v in args.items() if k in DEFAULT_CONFIG_KEYS}  # strip non-default keys
+    x['train_args'] = {k: v for k, v in args.items() if k in DEFAULT_CFG_KEYS}  # strip non-default keys
+    # x['model'].args = x['train_args']
     torch.save(x, s or f)
     mb = os.path.getsize(s or f) / 1E6  # filesize
     LOGGER.info(f"Optimizer stripped from {f},{f' saved as {s},' if s else ''} {mb:.1f}MB")
 
 
-def guess_task_from_head(head):
-    task = None
-    if head.lower() in ["classify", "classifier", "cls", "fc"]:
-        task = "classify"
-    if head.lower() in ["detect"]:
-        task = "detect"
-    if head.lower() in ["segment"]:
-        task = "segment"
-
-    if not task:
-        raise SyntaxError("task or model not recognized! Please refer the docs at : ")  # TODO: add docs links
-
-    return task
-
-
 def profile(input, ops, n=10, device=None):
-    """ YOLOv8 speed/memory/FLOPs profiler
+    """
+    YOLOv8 speed/memory/FLOPs profiler
+
     Usage:
         input = torch.randn(16, 3, 640, 640)
         m1 = lambda x: x * torch.sigmoid(x)
         m2 = nn.SiLU()
         profile(input, [m1, m2], n=100)  # profile over 100 iterations
     """
     results = []
     if not isinstance(device, torch.device):
         device = select_device(device)
-    print(f"{'Params':>12s}{'GFLOPs':>12s}{'GPU_mem (GB)':>14s}{'forward (ms)':>14s}{'backward (ms)':>14s}"
-          f"{'input':>24s}{'output':>24s}")
+    LOGGER.info(f"{'Params':>12s}{'GFLOPs':>12s}{'GPU_mem (GB)':>14s}{'forward (ms)':>14s}{'backward (ms)':>14s}"
+                f"{'input':>24s}{'output':>24s}")
 
     for x in input if isinstance(input, list) else [input]:
         x = x.to(device)
         x.requires_grad = True
         for m in ops if isinstance(ops, list) else [ops]:
             m = m.to(device) if hasattr(m, 'to') else m  # device
             m = m.half() if hasattr(m, 'half') and isinstance(x, torch.Tensor) and x.dtype is torch.float16 else m
             tf, tb, t = 0, 0, [0, 0, 0]  # dt forward, backward
             try:
-                flops = thop.profile(m, inputs=(x,), verbose=False)[0] / 1E9 * 2  # GFLOPs
+                flops = thop.profile(m, inputs=[x], verbose=False)[0] / 1E9 * 2  # GFLOPs
             except Exception:
                 flops = 0
 
             try:
                 for _ in range(n):
                     t[0] = time_sync()
                     y = m(x)
@@ -356,14 +390,59 @@
                         # print(e)  # for debug
                         t[2] = float('nan')
                     tf += (t[1] - t[0]) * 1000 / n  # ms per op forward
                     tb += (t[2] - t[1]) * 1000 / n  # ms per op backward
                 mem = torch.cuda.memory_reserved() / 1E9 if torch.cuda.is_available() else 0  # (GB)
                 s_in, s_out = (tuple(x.shape) if isinstance(x, torch.Tensor) else 'list' for x in (x, y))  # shapes
                 p = sum(x.numel() for x in m.parameters()) if isinstance(m, nn.Module) else 0  # parameters
-                print(f'{p:12}{flops:12.4g}{mem:>14.3f}{tf:14.4g}{tb:14.4g}{str(s_in):>24s}{str(s_out):>24s}')
+                LOGGER.info(f'{p:12}{flops:12.4g}{mem:>14.3f}{tf:14.4g}{tb:14.4g}{str(s_in):>24s}{str(s_out):>24s}')
                 results.append([p, flops, mem, tf, tb, s_in, s_out])
             except Exception as e:
-                print(e)
+                LOGGER.info(e)
                 results.append(None)
             torch.cuda.empty_cache()
     return results
+
+
+class EarlyStopping:
+    """
+    Early stopping class that stops training when a specified number of epochs have passed without improvement.
+    """
+
+    def __init__(self, patience=50):
+        """
+        Initialize early stopping object
+
+        Args:
+            patience (int, optional): Number of epochs to wait after fitness stops improving before stopping.
+        """
+        self.best_fitness = 0.0  # i.e. mAP
+        self.best_epoch = 0
+        self.patience = patience or float('inf')  # epochs to wait after fitness stops improving to stop
+        self.possible_stop = False  # possible stop may occur next epoch
+
+    def __call__(self, epoch, fitness):
+        """
+        Check whether to stop training
+
+        Args:
+            epoch (int): Current epoch of training
+            fitness (float): Fitness value of current epoch
+
+        Returns:
+            (bool): True if training should stop, False otherwise
+        """
+        if fitness is None:  # check if fitness=None (happens when val=False)
+            return False
+
+        if fitness >= self.best_fitness:  # >= 0 to allow for early zero-fitness stage of training
+            self.best_epoch = epoch
+            self.best_fitness = fitness
+        delta = epoch - self.best_epoch  # epochs without improvement
+        self.possible_stop = delta >= (self.patience - 1)  # possible stop may occur next epoch
+        stop = delta >= self.patience  # stop training if patience exceeded
+        if stop:
+            LOGGER.info(f'Stopping training early as no improvement observed in last {self.patience} epochs. '
+                        f'Best results observed at epoch {self.best_epoch}, best model saved as best.pt.\n'
+                        f'To update EarlyStopping(patience={self.patience}) pass a new patience value, '
+                        f'i.e. `patience=300` or use `patience=0` to disable EarlyStopping.')
+        return stop
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/v8/classify/train.py` & `ultralytics-8.0.90/ultralytics/yolo/v8/classify/train.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
-import hydra
 import torch
 import torchvision
 
 from ultralytics.nn.tasks import ClassificationModel, attempt_load_one_weight
 from ultralytics.yolo import v8
-from ultralytics.yolo.data import build_classification_dataloader
+from ultralytics.yolo.data import ClassificationDataset, build_dataloader
 from ultralytics.yolo.engine.trainer import BaseTrainer
-from ultralytics.yolo.utils import DEFAULT_CONFIG
-from ultralytics.yolo.utils.torch_utils import strip_optimizer
+from ultralytics.yolo.utils import DEFAULT_CFG, LOGGER, RANK, colorstr
+from ultralytics.yolo.utils.plotting import plot_images, plot_results
+from ultralytics.yolo.utils.torch_utils import is_parallel, strip_optimizer, torch_distributed_zero_first
 
 
 class ClassificationTrainer(BaseTrainer):
 
-    def __init__(self, config=DEFAULT_CONFIG, overrides=None):
+    def __init__(self, cfg=DEFAULT_CFG, overrides=None, _callbacks=None):
+        """Initialize a ClassificationTrainer object with optional configuration overrides and callbacks."""
         if overrides is None:
             overrides = {}
-        overrides["task"] = "classify"
-        super().__init__(config, overrides)
+        overrides['task'] = 'classify'
+        super().__init__(cfg, overrides, _callbacks)
 
     def set_model_attributes(self):
-        self.model.names = self.data["names"]
+        """Set the YOLO model's class names from the loaded dataset."""
+        self.model.names = self.data['names']
 
     def get_model(self, cfg=None, weights=None, verbose=True):
-        model = ClassificationModel(cfg, nc=self.data["nc"])
+        """Returns a modified PyTorch model configured for training YOLO."""
+        model = ClassificationModel(cfg, nc=self.data['nc'], verbose=verbose and RANK == -1)
         if weights:
             model.load(weights)
 
-        pretrained = False
+        pretrained = self.args.pretrained
         for m in model.modules():
             if not pretrained and hasattr(m, 'reset_parameters'):
                 m.reset_parameters()
             if isinstance(m, torch.nn.Dropout) and self.args.dropout:
                 m.p = self.args.dropout  # set dropout
         for p in model.parameters():
             p.requires_grad = True  # for training
@@ -43,114 +46,127 @@
 
         return model
 
     def setup_model(self):
         """
         load/create/download model for any task
         """
-        # classification models require special handling
+        # Classification models require special handling
 
         if isinstance(self.model, torch.nn.Module):  # if model is loaded beforehand. No setup needed
             return
 
         model = str(self.model)
         # Load a YOLO model locally, from torchvision, or from Ultralytics assets
-        if model.endswith(".pt"):
+        if model.endswith('.pt'):
             self.model, _ = attempt_load_one_weight(model, device='cpu')
-            for p in model.parameters():
+            for p in self.model.parameters():
                 p.requires_grad = True  # for training
-        elif model.endswith(".yaml"):
+        elif model.endswith('.yaml'):
             self.model = self.get_model(cfg=model)
         elif model in torchvision.models.__dict__:
             pretrained = True
             self.model = torchvision.models.__dict__[model](weights='IMAGENET1K_V1' if pretrained else None)
         else:
             FileNotFoundError(f'ERROR: model={model} not found locally or online. Please check model name.')
+        ClassificationModel.reshape_outputs(self.model, self.data['nc'])
 
         return  # dont return ckpt. Classification doesn't support resume
 
-    def get_dataloader(self, dataset_path, batch_size=16, rank=0, mode="train"):
-        loader = build_classification_dataloader(path=dataset_path,
-                                                 imgsz=self.args.imgsz,
-                                                 batch_size=batch_size if mode == "train" else (batch_size * 2),
-                                                 augment=mode == "train",
-                                                 rank=rank,
-                                                 workers=self.args.workers)
-        if mode != "train":
-            self.model.transforms = loader.dataset.torch_transforms  # attach inference transforms
+    def build_dataset(self, img_path, mode='train'):
+        dataset = ClassificationDataset(root=img_path, imgsz=self.args.imgsz, augment=mode == 'train')
+        return dataset
+
+    def get_dataloader(self, dataset_path, batch_size=16, rank=0, mode='train'):
+        """Returns PyTorch DataLoader with transforms to preprocess images for inference."""
+        with torch_distributed_zero_first(rank):  # init dataset *.cache only once if DDP
+            dataset = self.build_dataset(dataset_path, mode)
+
+        loader = build_dataloader(dataset, batch_size, self.args.workers, rank=rank)
+        # Attach inference transforms
+        if mode != 'train':
+            if is_parallel(self.model):
+                self.model.module.transforms = loader.dataset.torch_transforms
+            else:
+                self.model.transforms = loader.dataset.torch_transforms
         return loader
 
     def preprocess_batch(self, batch):
-        batch["img"] = batch["img"].to(self.device)
-        batch["cls"] = batch["cls"].to(self.device)
+        """Preprocesses a batch of images and classes."""
+        batch['img'] = batch['img'].to(self.device)
+        batch['cls'] = batch['cls'].to(self.device)
         return batch
 
     def progress_string(self):
+        """Returns a formatted string showing training progress."""
         return ('\n' + '%11s' * (4 + len(self.loss_names))) % \
             ('Epoch', 'GPU_mem', *self.loss_names, 'Instances', 'Size')
 
     def get_validator(self):
+        """Returns an instance of ClassificationValidator for validation."""
         self.loss_names = ['loss']
-        return v8.classify.ClassificationValidator(self.test_loader, self.save_dir, logger=self.console)
+        return v8.classify.ClassificationValidator(self.test_loader, self.save_dir)
 
     def criterion(self, preds, batch):
-        loss = torch.nn.functional.cross_entropy(preds, batch["cls"], reduction='sum') / self.args.nbs
+        """Compute the classification loss between predictions and true labels."""
+        loss = torch.nn.functional.cross_entropy(preds, batch['cls'], reduction='sum') / self.args.nbs
         loss_items = loss.detach()
         return loss, loss_items
 
-    # def label_loss_items(self, loss_items=None, prefix="train"):
-    #     """
-    #     Returns a loss dict with labelled training loss items tensor
-    #     """
-    #     # Not needed for classification but necessary for segmentation & detection
-    #     keys = [f"{prefix}/{x}" for x in self.loss_names]
-    #     if loss_items is not None:
-    #         loss_items = [round(float(x), 5) for x in loss_items]  # convert tensors to 5 decimal place floats
-    #         return dict(zip(keys, loss_items))
-    #     else:
-    #         return keys
-
-    def label_loss_items(self, loss_items=None, prefix="train"):
+    def label_loss_items(self, loss_items=None, prefix='train'):
         """
         Returns a loss dict with labelled training loss items tensor
         """
         # Not needed for classification but necessary for segmentation & detection
-        keys = [f"{prefix}/{x}" for x in self.loss_names]
+        keys = [f'{prefix}/{x}' for x in self.loss_names]
         if loss_items is None:
             return keys
         loss_items = [round(float(loss_items), 5)]
         return dict(zip(keys, loss_items))
 
     def resume_training(self, ckpt):
+        """Resumes training from a given checkpoint."""
         pass
 
+    def plot_metrics(self):
+        """Plots metrics from a CSV file."""
+        plot_results(file=self.csv, classify=True)  # save results.png
+
     def final_eval(self):
+        """Evaluate trained model and save validation results."""
         for f in self.last, self.best:
             if f.exists():
                 strip_optimizer(f)  # strip optimizers
                 # TODO: validate best.pt after training completes
                 # if f is self.best:
-                #     self.console.info(f'\nValidating {f}...')
+                #     LOGGER.info(f'\nValidating {f}...')
                 #     self.validator.args.save_json = True
                 #     self.metrics = self.validator(model=f)
                 #     self.metrics.pop('fitness', None)
                 #     self.run_callbacks('on_fit_epoch_end')
+        LOGGER.info(f"Results saved to {colorstr('bold', self.save_dir)}")
 
-
-@hydra.main(version_base=None, config_path=str(DEFAULT_CONFIG.parent), config_name=DEFAULT_CONFIG.name)
-def train(cfg):
-    cfg.model = cfg.model or "yolov8n-cls.pt"  # or "resnet18"
-    cfg.data = cfg.data or "mnist160"  # or yolo.ClassificationDataset("mnist")
-    cfg.lr0 = 0.1
-    cfg.weight_decay = 5e-5
-    cfg.label_smoothing = 0.1
-    cfg.warmup_epochs = 0.0
-    cfg.device = cfg.device if cfg.device is not None else ''
-    # trainer = ClassificationTrainer(cfg)
-    # trainer.train()
-    from ultralytics import YOLO
-    model = YOLO(cfg.model)
-    model.train(**cfg)
+    def plot_training_samples(self, batch, ni):
+        """Plots training samples with their annotations."""
+        plot_images(images=batch['img'],
+                    batch_idx=torch.arange(len(batch['img'])),
+                    cls=batch['cls'].squeeze(-1),
+                    fname=self.save_dir / f'train_batch{ni}.jpg')
+
+
+def train(cfg=DEFAULT_CFG, use_python=False):
+    """Train the YOLO classification model."""
+    model = cfg.model or 'yolov8n-cls.pt'  # or "resnet18"
+    data = cfg.data or 'mnist160'  # or yolo.ClassificationDataset("mnist")
+    device = cfg.device if cfg.device is not None else ''
+
+    args = dict(model=model, data=data, device=device)
+    if use_python:
+        from ultralytics import YOLO
+        YOLO(model).train(**args)
+    else:
+        trainer = ClassificationTrainer(overrides=args)
+        trainer.train()
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     train()
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/v8/detect/train.py` & `ultralytics-8.0.90/ultralytics/yolo/v8/detect/train.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,112 +1,143 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
-
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 from copy import copy
 
-import hydra
+import numpy as np
 import torch
 import torch.nn as nn
 
 from ultralytics.nn.tasks import DetectionModel
 from ultralytics.yolo import v8
-from ultralytics.yolo.data import build_dataloader
+from ultralytics.yolo.data import build_dataloader, build_yolo_dataset
 from ultralytics.yolo.data.dataloaders.v5loader import create_dataloader
 from ultralytics.yolo.engine.trainer import BaseTrainer
-from ultralytics.yolo.utils import DEFAULT_CONFIG, colorstr
+from ultralytics.yolo.utils import DEFAULT_CFG, LOGGER, RANK, colorstr
 from ultralytics.yolo.utils.loss import BboxLoss
 from ultralytics.yolo.utils.ops import xywh2xyxy
-from ultralytics.yolo.utils.plotting import plot_images, plot_results
+from ultralytics.yolo.utils.plotting import plot_images, plot_labels, plot_results
 from ultralytics.yolo.utils.tal import TaskAlignedAssigner, dist2bbox, make_anchors
-from ultralytics.yolo.utils.torch_utils import de_parallel
+from ultralytics.yolo.utils.torch_utils import de_parallel, torch_distributed_zero_first
 
 
 # BaseTrainer python usage
 class DetectionTrainer(BaseTrainer):
 
-    def get_dataloader(self, dataset_path, batch_size, mode="train", rank=0):
-        # TODO: manage splits differently
-        # calculate stride - check if model is initialized
+    def build_dataset(self, img_path, mode='train', batch=None):
+        """Build YOLO Dataset
+
+        Args:
+            img_path (str): Path to the folder containing images.
+            mode (str): `train` mode or `val` mode, users are able to customize different augmentations for each mode.
+            batch (int, optional): Size of batches, this is for `rect`. Defaults to None.
+        """
         gs = max(int(de_parallel(self.model).stride.max() if self.model else 0), 32)
-        return create_dataloader(path=dataset_path,
-                                 imgsz=self.args.imgsz,
-                                 batch_size=batch_size,
-                                 stride=gs,
-                                 hyp=dict(self.args),
-                                 augment=mode == "train",
-                                 cache=self.args.cache,
-                                 pad=0 if mode == "train" else 0.5,
-                                 rect=self.args.rect,
-                                 rank=rank,
-                                 workers=self.args.workers,
-                                 close_mosaic=self.args.close_mosaic != 0,
-                                 prefix=colorstr(f'{mode}: '),
-                                 shuffle=mode == "train",
-                                 seed=self.args.seed)[0] if self.args.v5loader else \
-            build_dataloader(self.args, batch_size, img_path=dataset_path, stride=gs, rank=rank, mode=mode)[0]
+        return build_yolo_dataset(self.args, img_path, batch, self.data, mode=mode, rect=mode == 'val', stride=gs)
+
+    def get_dataloader(self, dataset_path, batch_size, rank=0, mode='train'):
+        """TODO: manage splits differently."""
+        # Calculate stride - check if model is initialized
+        if self.args.v5loader:
+            LOGGER.warning("WARNING ⚠️ 'v5loader' feature is deprecated and will be removed soon. You can train using "
+                           'the default YOLOv8 dataloader instead, no argument is needed.')
+            gs = max(int(de_parallel(self.model).stride.max() if self.model else 0), 32)
+            return create_dataloader(path=dataset_path,
+                                     imgsz=self.args.imgsz,
+                                     batch_size=batch_size,
+                                     stride=gs,
+                                     hyp=vars(self.args),
+                                     augment=mode == 'train',
+                                     cache=self.args.cache,
+                                     pad=0 if mode == 'train' else 0.5,
+                                     rect=self.args.rect or mode == 'val',
+                                     rank=rank,
+                                     workers=self.args.workers,
+                                     close_mosaic=self.args.close_mosaic != 0,
+                                     prefix=colorstr(f'{mode}: '),
+                                     shuffle=mode == 'train',
+                                     seed=self.args.seed)[0]
+        assert mode in ['train', 'val']
+        with torch_distributed_zero_first(rank):  # init dataset *.cache only once if DDP
+            dataset = self.build_dataset(dataset_path, mode, batch_size)
+        shuffle = mode == 'train'
+        if getattr(dataset, 'rect', False) and shuffle:
+            LOGGER.warning("WARNING ⚠️ 'rect=True' is incompatible with DataLoader shuffle, setting shuffle=False")
+            shuffle = False
+        workers = self.args.workers if mode == 'train' else self.args.workers * 2
+        dataloader = build_dataloader(dataset, batch_size, workers, shuffle, rank)
+        return dataloader
 
     def preprocess_batch(self, batch):
-        batch["img"] = batch["img"].to(self.device, non_blocking=True).float() / 255
+        """Preprocesses a batch of images by scaling and converting to float."""
+        batch['img'] = batch['img'].to(self.device, non_blocking=True).float() / 255
         return batch
 
     def set_model_attributes(self):
-        # nl = de_parallel(self.model).model[-1].nl  # number of detection layers (to scale hyps)
+        """nl = de_parallel(self.model).model[-1].nl  # number of detection layers (to scale hyps)."""
         # self.args.box *= 3 / nl  # scale to layers
         # self.args.cls *= self.data["nc"] / 80 * 3 / nl  # scale to classes and layers
         # self.args.cls *= (self.args.imgsz / 640) ** 2 * 3 / nl  # scale to image size and layers
-        self.model.nc = self.data["nc"]  # attach number of classes to model
-        self.model.names = self.data["names"]  # attach class names to model
+        self.model.nc = self.data['nc']  # attach number of classes to model
+        self.model.names = self.data['names']  # attach class names to model
         self.model.args = self.args  # attach hyperparameters to model
         # TODO: self.model.class_weights = labels_to_class_weights(dataset.labels, nc).to(device) * nc
 
     def get_model(self, cfg=None, weights=None, verbose=True):
-        model = DetectionModel(cfg, ch=3, nc=self.data["nc"], verbose=verbose)
+        """Return a YOLO detection model."""
+        model = DetectionModel(cfg, nc=self.data['nc'], verbose=verbose and RANK == -1)
         if weights:
             model.load(weights)
-
         return model
 
     def get_validator(self):
+        """Returns a DetectionValidator for YOLO model validation."""
         self.loss_names = 'box_loss', 'cls_loss', 'dfl_loss'
-        return v8.detect.DetectionValidator(self.test_loader,
-                                            save_dir=self.save_dir,
-                                            logger=self.console,
-                                            args=copy(self.args))
+        return v8.detect.DetectionValidator(self.test_loader, save_dir=self.save_dir, args=copy(self.args))
 
     def criterion(self, preds, batch):
+        """Compute loss for YOLO prediction and ground-truth."""
         if not hasattr(self, 'compute_loss'):
             self.compute_loss = Loss(de_parallel(self.model))
         return self.compute_loss(preds, batch)
 
-    def label_loss_items(self, loss_items=None, prefix="train"):
+    def label_loss_items(self, loss_items=None, prefix='train'):
         """
         Returns a loss dict with labelled training loss items tensor
         """
         # Not needed for classification but necessary for segmentation & detection
-        keys = [f"{prefix}/{x}" for x in self.loss_names]
+        keys = [f'{prefix}/{x}' for x in self.loss_names]
         if loss_items is not None:
             loss_items = [round(float(x), 5) for x in loss_items]  # convert tensors to 5 decimal place floats
             return dict(zip(keys, loss_items))
         else:
             return keys
 
     def progress_string(self):
+        """Returns a formatted string of training progress with epoch, GPU memory, loss, instances and size."""
         return ('\n' + '%11s' *
                 (4 + len(self.loss_names))) % ('Epoch', 'GPU_mem', *self.loss_names, 'Instances', 'Size')
 
     def plot_training_samples(self, batch, ni):
-        plot_images(images=batch["img"],
-                    batch_idx=batch["batch_idx"],
-                    cls=batch["cls"].squeeze(-1),
-                    bboxes=batch["bboxes"],
-                    paths=batch["im_file"],
-                    fname=self.save_dir / f"train_batch{ni}.jpg")
+        """Plots training samples with their annotations."""
+        plot_images(images=batch['img'],
+                    batch_idx=batch['batch_idx'],
+                    cls=batch['cls'].squeeze(-1),
+                    bboxes=batch['bboxes'],
+                    paths=batch['im_file'],
+                    fname=self.save_dir / f'train_batch{ni}.jpg')
 
     def plot_metrics(self):
+        """Plots metrics from a CSV file."""
         plot_results(file=self.csv)  # save results.png
 
+    def plot_training_labels(self):
+        """Create a labeled training plot of the YOLO model."""
+        boxes = np.concatenate([lb['bboxes'] for lb in self.train_loader.dataset.labels], 0)
+        cls = np.concatenate([lb['cls'] for lb in self.train_loader.dataset.labels], 0)
+        plot_labels(boxes, cls.squeeze(), names=self.data['names'], save_dir=self.save_dir)
+
 
 # Criterion class for computing training losses
 class Loss:
 
     def __init__(self, model):  # model must be de-paralleled
 
         device = next(model.parameters()).device  # get model device
@@ -118,70 +149,75 @@
         self.stride = m.stride  # model strides
         self.nc = m.nc  # number of classes
         self.no = m.no
         self.reg_max = m.reg_max
         self.device = device
 
         self.use_dfl = m.reg_max > 1
+
         self.assigner = TaskAlignedAssigner(topk=10, num_classes=self.nc, alpha=0.5, beta=6.0)
         self.bbox_loss = BboxLoss(m.reg_max - 1, use_dfl=self.use_dfl).to(device)
         self.proj = torch.arange(m.reg_max, dtype=torch.float, device=device)
 
     def preprocess(self, targets, batch_size, scale_tensor):
+        """Preprocesses the target counts and matches with the input batch size to output a tensor."""
         if targets.shape[0] == 0:
             out = torch.zeros(batch_size, 0, 5, device=self.device)
         else:
             i = targets[:, 0]  # image index
             _, counts = i.unique(return_counts=True)
+            counts = counts.to(dtype=torch.int32)
             out = torch.zeros(batch_size, counts.max(), 5, device=self.device)
             for j in range(batch_size):
                 matches = i == j
                 n = matches.sum()
                 if n:
                     out[j, :n] = targets[matches, 1:]
             out[..., 1:5] = xywh2xyxy(out[..., 1:5].mul_(scale_tensor))
         return out
 
     def bbox_decode(self, anchor_points, pred_dist):
+        """Decode predicted object bounding box coordinates from anchor points and distribution."""
         if self.use_dfl:
             b, a, c = pred_dist.shape  # batch, anchors, channels
             pred_dist = pred_dist.view(b, a, 4, c // 4).softmax(3).matmul(self.proj.type(pred_dist.dtype))
             # pred_dist = pred_dist.view(b, a, c // 4, 4).transpose(2,3).softmax(3).matmul(self.proj.type(pred_dist.dtype))
             # pred_dist = (pred_dist.view(b, a, c // 4, 4).softmax(2) * self.proj.type(pred_dist.dtype).view(1, 1, -1, 1)).sum(2)
         return dist2bbox(pred_dist, anchor_points, xywh=False)
 
     def __call__(self, preds, batch):
+        """Calculate the sum of the loss for box, cls and dfl multiplied by batch size."""
         loss = torch.zeros(3, device=self.device)  # box, cls, dfl
         feats = preds[1] if isinstance(preds, tuple) else preds
         pred_distri, pred_scores = torch.cat([xi.view(feats[0].shape[0], self.no, -1) for xi in feats], 2).split(
             (self.reg_max * 4, self.nc), 1)
 
         pred_scores = pred_scores.permute(0, 2, 1).contiguous()
         pred_distri = pred_distri.permute(0, 2, 1).contiguous()
 
         dtype = pred_scores.dtype
         batch_size = pred_scores.shape[0]
         imgsz = torch.tensor(feats[0].shape[2:], device=self.device, dtype=dtype) * self.stride[0]  # image size (h,w)
         anchor_points, stride_tensor = make_anchors(feats, self.stride, 0.5)
 
         # targets
-        targets = torch.cat((batch["batch_idx"].view(-1, 1), batch["cls"].view(-1, 1), batch["bboxes"]), 1)
+        targets = torch.cat((batch['batch_idx'].view(-1, 1), batch['cls'].view(-1, 1), batch['bboxes']), 1)
         targets = self.preprocess(targets.to(self.device), batch_size, scale_tensor=imgsz[[1, 0, 1, 0]])
         gt_labels, gt_bboxes = targets.split((1, 4), 2)  # cls, xyxy
         mask_gt = gt_bboxes.sum(2, keepdim=True).gt_(0)
 
         # pboxes
         pred_bboxes = self.bbox_decode(anchor_points, pred_distri)  # xyxy, (b, h*w, 4)
 
         _, target_bboxes, target_scores, fg_mask, _ = self.assigner(
             pred_scores.detach().sigmoid(), (pred_bboxes.detach() * stride_tensor).type(gt_bboxes.dtype),
             anchor_points * stride_tensor, gt_labels, gt_bboxes, mask_gt)
 
         target_bboxes /= stride_tensor
-        target_scores_sum = target_scores.sum()
+        target_scores_sum = max(target_scores.sum(), 1)
 
         # cls loss
         # loss[1] = self.varifocal_loss(pred_scores, target_scores, target_labels) / target_scores_sum  # VFL way
         loss[1] = self.bce(pred_scores, target_scores.to(dtype)).sum() / target_scores_sum  # BCE
 
         # bbox loss
         if fg_mask.sum():
@@ -191,21 +227,24 @@
         loss[0] *= self.hyp.box  # box gain
         loss[1] *= self.hyp.cls  # cls gain
         loss[2] *= self.hyp.dfl  # dfl gain
 
         return loss.sum() * batch_size, loss.detach()  # loss(box, cls, dfl)
 
 
-@hydra.main(version_base=None, config_path=str(DEFAULT_CONFIG.parent), config_name=DEFAULT_CONFIG.name)
-def train(cfg):
-    cfg.model = cfg.model or "yolov8n.pt"
-    cfg.data = cfg.data or "coco128.yaml"  # or yolo.ClassificationDataset("mnist")
-    cfg.device = cfg.device if cfg.device is not None else ''
-    # trainer = DetectionTrainer(cfg)
-    # trainer.train()
-    from ultralytics import YOLO
-    model = YOLO(cfg.model)
-    model.train(**cfg)
+def train(cfg=DEFAULT_CFG, use_python=False):
+    """Train and optimize YOLO model given training data and device."""
+    model = cfg.model or 'yolov8n.pt'
+    data = cfg.data or 'coco128.yaml'  # or yolo.ClassificationDataset("mnist")
+    device = cfg.device if cfg.device is not None else ''
+
+    args = dict(model=model, data=data, device=device)
+    if use_python:
+        from ultralytics import YOLO
+        YOLO(model).train(**args)
+    else:
+        trainer = DetectionTrainer(overrides=args)
+        trainer.train()
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     train()
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/v8/detect/val.py` & `ultralytics-8.0.90/ultralytics/yolo/v8/pose/val.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,154 +1,135 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
-import os
 from pathlib import Path
 
-import hydra
 import numpy as np
 import torch
 
-from ultralytics.yolo.data import build_dataloader
-from ultralytics.yolo.data.dataloaders.v5loader import create_dataloader
-from ultralytics.yolo.engine.validator import BaseValidator
-from ultralytics.yolo.utils import DEFAULT_CONFIG, colorstr, ops, yaml_load
-from ultralytics.yolo.utils.checks import check_file, check_requirements
-from ultralytics.yolo.utils.metrics import ConfusionMatrix, DetMetrics, box_iou
+from ultralytics.yolo.utils import DEFAULT_CFG, LOGGER, ops
+from ultralytics.yolo.utils.checks import check_requirements
+from ultralytics.yolo.utils.metrics import OKS_SIGMA, PoseMetrics, box_iou, kpt_iou
 from ultralytics.yolo.utils.plotting import output_to_target, plot_images
-from ultralytics.yolo.utils.torch_utils import de_parallel
+from ultralytics.yolo.v8.detect import DetectionValidator
 
 
-class DetectionValidator(BaseValidator):
+class PoseValidator(DetectionValidator):
 
-    def __init__(self, dataloader=None, save_dir=None, pbar=None, logger=None, args=None):
-        super().__init__(dataloader, save_dir, pbar, logger, args)
-        self.data_dict = yaml_load(check_file(self.args.data), append_filename=True) if self.args.data else None
-        self.is_coco = False
-        self.class_map = None
-        self.metrics = DetMetrics(save_dir=self.save_dir)
-        self.iouv = torch.linspace(0.5, 0.95, 10)  # iou vector for mAP@0.5:0.95
-        self.niou = self.iouv.numel()
+    def __init__(self, dataloader=None, save_dir=None, pbar=None, args=None, _callbacks=None):
+        """Initialize a 'PoseValidator' object with custom parameters and assigned attributes."""
+        super().__init__(dataloader, save_dir, pbar, args, _callbacks)
+        self.args.task = 'pose'
+        self.metrics = PoseMetrics(save_dir=self.save_dir)
 
     def preprocess(self, batch):
-        batch["img"] = batch["img"].to(self.device, non_blocking=True)
-        batch["img"] = (batch["img"].half() if self.args.half else batch["img"].float()) / 255
-        for k in ["batch_idx", "cls", "bboxes"]:
-            batch[k] = batch[k].to(self.device)
-
-        nb = len(batch["img"])
-        self.lb = [torch.cat([batch["cls"], batch["bboxes"]], dim=-1)[batch["batch_idx"] == i]
-                   for i in range(nb)] if self.args.save_hybrid else []  # for autolabelling
-
+        """Preprocesses the batch by converting the 'keypoints' data into a float and moving it to the device."""
+        batch = super().preprocess(batch)
+        batch['keypoints'] = batch['keypoints'].to(self.device).float()
         return batch
 
-    def init_metrics(self, model):
-        head = model.model[-1] if self.training else model.model.model[-1]
-        val = self.data.get('val', '')  # validation path
-        self.is_coco = isinstance(val, str) and val.endswith(f'coco{os.sep}val2017.txt')  # is COCO dataset
-        self.class_map = ops.coco80_to_coco91_class() if self.is_coco else list(range(1000))
-        self.args.save_json |= self.is_coco and not self.training  # run on final val if training COCO
-        self.nc = head.nc
-        self.names = model.names
-        self.metrics.names = self.names
-        self.metrics.plot = self.args.plots
-        self.confusion_matrix = ConfusionMatrix(nc=self.nc)
-        self.seen = 0
-        self.jdict = []
-        self.stats = []
-
     def get_desc(self):
-        return ('%22s' + '%11s' * 6) % ('Class', 'Images', 'Instances', 'Box(P', "R", "mAP50", "mAP50-95)")
+        """Returns description of evaluation metrics in string format."""
+        return ('%22s' + '%11s' * 10) % ('Class', 'Images', 'Instances', 'Box(P', 'R', 'mAP50', 'mAP50-95)', 'Pose(P',
+                                         'R', 'mAP50', 'mAP50-95)')
 
     def postprocess(self, preds):
+        """Apply non-maximum suppression and return detections with high confidence scores."""
         preds = ops.non_max_suppression(preds,
                                         self.args.conf,
                                         self.args.iou,
                                         labels=self.lb,
                                         multi_label=True,
                                         agnostic=self.args.single_cls,
-                                        max_det=self.args.max_det)
+                                        max_det=self.args.max_det,
+                                        nc=self.nc)
         return preds
 
+    def init_metrics(self, model):
+        """Initiate pose estimation metrics for YOLO model."""
+        super().init_metrics(model)
+        self.kpt_shape = self.data['kpt_shape']
+        is_pose = self.kpt_shape == [17, 3]
+        nkpt = self.kpt_shape[0]
+        self.sigma = OKS_SIGMA if is_pose else np.ones(nkpt) / nkpt
+
     def update_metrics(self, preds, batch):
-        # Metrics
+        """Metrics."""
         for si, pred in enumerate(preds):
-            idx = batch["batch_idx"] == si
-            cls = batch["cls"][idx]
-            bbox = batch["bboxes"][idx]
+            idx = batch['batch_idx'] == si
+            cls = batch['cls'][idx]
+            bbox = batch['bboxes'][idx]
+            kpts = batch['keypoints'][idx]
             nl, npr = cls.shape[0], pred.shape[0]  # number of labels, predictions
-            shape = batch["ori_shape"][si]
+            nk = kpts.shape[1]  # number of keypoints
+            shape = batch['ori_shape'][si]
+            correct_kpts = torch.zeros(npr, self.niou, dtype=torch.bool, device=self.device)  # init
             correct_bboxes = torch.zeros(npr, self.niou, dtype=torch.bool, device=self.device)  # init
             self.seen += 1
 
             if npr == 0:
                 if nl:
-                    self.stats.append((correct_bboxes, *torch.zeros((2, 0), device=self.device), cls.squeeze(-1)))
+                    self.stats.append((correct_bboxes, correct_kpts, *torch.zeros(
+                        (2, 0), device=self.device), cls.squeeze(-1)))
                     if self.args.plots:
                         self.confusion_matrix.process_batch(detections=None, labels=cls.squeeze(-1))
                 continue
 
             # Predictions
             if self.args.single_cls:
                 pred[:, 5] = 0
             predn = pred.clone()
-            ops.scale_boxes(batch["img"][si].shape[1:], predn[:, :4], shape,
-                            ratio_pad=batch["ratio_pad"][si])  # native-space pred
+            ops.scale_boxes(batch['img'][si].shape[1:], predn[:, :4], shape,
+                            ratio_pad=batch['ratio_pad'][si])  # native-space pred
+            pred_kpts = predn[:, 6:].view(npr, nk, -1)
+            ops.scale_coords(batch['img'][si].shape[1:], pred_kpts, shape, ratio_pad=batch['ratio_pad'][si])
 
             # Evaluate
             if nl:
-                height, width = batch["img"].shape[2:]
+                height, width = batch['img'].shape[2:]
                 tbox = ops.xywh2xyxy(bbox) * torch.tensor(
                     (width, height, width, height), device=self.device)  # target boxes
-                ops.scale_boxes(batch["img"][si].shape[1:], tbox, shape,
-                                ratio_pad=batch["ratio_pad"][si])  # native-space labels
+                ops.scale_boxes(batch['img'][si].shape[1:], tbox, shape,
+                                ratio_pad=batch['ratio_pad'][si])  # native-space labels
+                tkpts = kpts.clone()
+                tkpts[..., 0] *= width
+                tkpts[..., 1] *= height
+                tkpts = ops.scale_coords(batch['img'][si].shape[1:], tkpts, shape, ratio_pad=batch['ratio_pad'][si])
                 labelsn = torch.cat((cls, tbox), 1)  # native-space labels
-                correct_bboxes = self._process_batch(predn, labelsn)
-                # TODO: maybe remove these `self.` arguments as they already are member variable
+                correct_bboxes = self._process_batch(predn[:, :6], labelsn)
+                correct_kpts = self._process_batch(predn[:, :6], labelsn, pred_kpts, tkpts)
                 if self.args.plots:
                     self.confusion_matrix.process_batch(predn, labelsn)
-            self.stats.append((correct_bboxes, pred[:, 4], pred[:, 5], cls.squeeze(-1)))  # (conf, pcls, tcls)
+
+            # Append correct_masks, correct_boxes, pconf, pcls, tcls
+            self.stats.append((correct_bboxes, correct_kpts, pred[:, 4], pred[:, 5], cls.squeeze(-1)))
 
             # Save
             if self.args.save_json:
-                self.pred_to_json(predn, batch["im_file"][si])
+                self.pred_to_json(predn, batch['im_file'][si])
             # if self.args.save_txt:
             #    save_one_txt(predn, save_conf, shape, file=save_dir / 'labels' / f'{path.stem}.txt')
 
-    def get_stats(self):
-        stats = [torch.cat(x, 0).cpu().numpy() for x in zip(*self.stats)]  # to numpy
-        if len(stats) and stats[0].any():
-            self.metrics.process(*stats)
-        self.nt_per_class = np.bincount(stats[-1].astype(int), minlength=self.nc)  # number of targets per class
-        return self.metrics.results_dict
-
-    def print_results(self):
-        pf = '%22s' + '%11i' * 2 + '%11.3g' * len(self.metrics.keys)  # print format
-        self.logger.info(pf % ("all", self.seen, self.nt_per_class.sum(), *self.metrics.mean_results()))
-        if self.nt_per_class.sum() == 0:
-            self.logger.warning(
-                f'WARNING ⚠️ no labels found in {self.args.task} set, can not compute metrics without labels')
-
-        # Print results per class
-        if (self.args.verbose or not self.training) and self.nc > 1 and len(self.stats):
-            for i, c in enumerate(self.metrics.ap_class_index):
-                self.logger.info(pf % (self.names[c], self.seen, self.nt_per_class[c], *self.metrics.class_result(i)))
-
-        if self.args.plots:
-            self.confusion_matrix.plot(save_dir=self.save_dir, names=list(self.names.values()))
-
-    def _process_batch(self, detections, labels):
+    def _process_batch(self, detections, labels, pred_kpts=None, gt_kpts=None):
         """
         Return correct prediction matrix
         Arguments:
             detections (array[N, 6]), x1, y1, x2, y2, conf, class
             labels (array[M, 5]), class, x1, y1, x2, y2
+            pred_kpts (array[N, 51]), 51 = 17 * 3
+            gt_kpts (array[N, 51])
         Returns:
             correct (array[N, 10]), for 10 IoU levels
         """
-        iou = box_iou(labels[:, 1:], detections[:, :4])
+        if pred_kpts is not None and gt_kpts is not None:
+            # `0.53` is from https://github.com/jin-s13/xtcocoapi/blob/master/xtcocotools/cocoeval.py#L384
+            area = ops.xyxy2xywh(labels[:, 1:])[:, 2:].prod(1) * 0.53
+            iou = kpt_iou(gt_kpts, pred_kpts, sigma=self.sigma, area=area)
+        else:  # boxes
+            iou = box_iou(labels[:, 1:], detections[:, :4])
+
         correct = np.zeros((detections.shape[0], self.iouv.shape[0])).astype(bool)
         correct_class = labels[:, 0:1] == detections[:, 5]
         for i in range(len(self.iouv)):
             x = torch.where((iou >= self.iouv[i]) & correct_class)  # IoU > threshold and classes match
             if x[0].shape[0]:
                 matches = torch.cat((torch.stack(x, 1), iou[x[0], x[1]][:, None]),
                                     1).cpu().numpy()  # [label, detect, iou]
@@ -156,89 +137,87 @@
                     matches = matches[matches[:, 2].argsort()[::-1]]
                     matches = matches[np.unique(matches[:, 1], return_index=True)[1]]
                     # matches = matches[matches[:, 2].argsort()[::-1]]
                     matches = matches[np.unique(matches[:, 0], return_index=True)[1]]
                 correct[matches[:, 1].astype(int), i] = True
         return torch.tensor(correct, dtype=torch.bool, device=detections.device)
 
-    def get_dataloader(self, dataset_path, batch_size):
-        # TODO: manage splits differently
-        # calculate stride - check if model is initialized
-        gs = max(int(de_parallel(self.model).stride if self.model else 0), 32)
-        return create_dataloader(path=dataset_path,
-                                 imgsz=self.args.imgsz,
-                                 batch_size=batch_size,
-                                 stride=gs,
-                                 hyp=dict(self.args),
-                                 cache=False,
-                                 pad=0.5,
-                                 rect=True,
-                                 workers=self.args.workers,
-                                 prefix=colorstr(f'{self.args.mode}: '),
-                                 shuffle=False,
-                                 seed=self.args.seed)[0] if self.args.v5loader else \
-            build_dataloader(self.args, batch_size, img_path=dataset_path, stride=gs, mode="val")[0]
-
     def plot_val_samples(self, batch, ni):
-        plot_images(batch["img"],
-                    batch["batch_idx"],
-                    batch["cls"].squeeze(-1),
-                    batch["bboxes"],
-                    paths=batch["im_file"],
-                    fname=self.save_dir / f"val_batch{ni}_labels.jpg",
+        """Plots and saves validation set samples with predicted bounding boxes and keypoints."""
+        plot_images(batch['img'],
+                    batch['batch_idx'],
+                    batch['cls'].squeeze(-1),
+                    batch['bboxes'],
+                    kpts=batch['keypoints'],
+                    paths=batch['im_file'],
+                    fname=self.save_dir / f'val_batch{ni}_labels.jpg',
                     names=self.names)
 
     def plot_predictions(self, batch, preds, ni):
-        plot_images(batch["img"],
+        """Plots predictions for YOLO model."""
+        pred_kpts = torch.cat([p[:, 6:].view(-1, *self.kpt_shape)[:15] for p in preds], 0)
+        plot_images(batch['img'],
                     *output_to_target(preds, max_det=15),
-                    paths=batch["im_file"],
+                    kpts=pred_kpts,
+                    paths=batch['im_file'],
                     fname=self.save_dir / f'val_batch{ni}_pred.jpg',
                     names=self.names)  # pred
 
     def pred_to_json(self, predn, filename):
+        """Converts YOLO predictions to COCO JSON format."""
         stem = Path(filename).stem
         image_id = int(stem) if stem.isnumeric() else stem
         box = ops.xyxy2xywh(predn[:, :4])  # xywh
         box[:, :2] -= box[:, 2:] / 2  # xy center to top-left corner
         for p, b in zip(predn.tolist(), box.tolist()):
             self.jdict.append({
                 'image_id': image_id,
                 'category_id': self.class_map[int(p[5])],
                 'bbox': [round(x, 3) for x in b],
+                'keypoints': p[6:],
                 'score': round(p[4], 5)})
 
     def eval_json(self, stats):
+        """Evaluates object detection model using COCO JSON format."""
         if self.args.save_json and self.is_coco and len(self.jdict):
-            anno_json = self.data['path'] / "annotations/instances_val2017.json"  # annotations
-            pred_json = self.save_dir / "predictions.json"  # predictions
-            self.logger.info(f'\nEvaluating pycocotools mAP using {pred_json} and {anno_json}...')
+            anno_json = self.data['path'] / 'annotations/person_keypoints_val2017.json'  # annotations
+            pred_json = self.save_dir / 'predictions.json'  # predictions
+            LOGGER.info(f'\nEvaluating pycocotools mAP using {pred_json} and {anno_json}...')
             try:  # https://github.com/cocodataset/cocoapi/blob/master/PythonAPI/pycocoEvalDemo.ipynb
                 check_requirements('pycocotools>=2.0.6')
                 from pycocotools.coco import COCO  # noqa
                 from pycocotools.cocoeval import COCOeval  # noqa
 
                 for x in anno_json, pred_json:
-                    assert x.is_file(), f"{x} file not found"
+                    assert x.is_file(), f'{x} file not found'
                 anno = COCO(str(anno_json))  # init annotations api
                 pred = anno.loadRes(str(pred_json))  # init predictions api (must pass string, not Path)
-                eval = COCOeval(anno, pred, 'bbox')
-                if self.is_coco:
-                    eval.params.imgIds = [int(Path(x).stem) for x in self.dataloader.dataset.im_files]  # images to eval
-                eval.evaluate()
-                eval.accumulate()
-                eval.summarize()
-                stats[self.metrics.keys[-1]], stats[self.metrics.keys[-2]] = eval.stats[:2]  # update mAP50-95 and mAP50
+                for i, eval in enumerate([COCOeval(anno, pred, 'bbox'), COCOeval(anno, pred, 'keypoints')]):
+                    if self.is_coco:
+                        eval.params.imgIds = [int(Path(x).stem) for x in self.dataloader.dataset.im_files]  # im to eval
+                    eval.evaluate()
+                    eval.accumulate()
+                    eval.summarize()
+                    idx = i * 4 + 2
+                    stats[self.metrics.keys[idx + 1]], stats[
+                        self.metrics.keys[idx]] = eval.stats[:2]  # update mAP50-95 and mAP50
             except Exception as e:
-                self.logger.warning(f'pycocotools unable to run: {e}')
+                LOGGER.warning(f'pycocotools unable to run: {e}')
         return stats
 
 
-@hydra.main(version_base=None, config_path=str(DEFAULT_CONFIG.parent), config_name=DEFAULT_CONFIG.name)
-def val(cfg):
-    cfg.model = cfg.model or "yolov8n.pt"
-    cfg.data = cfg.data or "coco128.yaml"
-    validator = DetectionValidator(args=cfg)
-    validator(model=cfg.model)
+def val(cfg=DEFAULT_CFG, use_python=False):
+    """Performs validation on YOLO model using given data."""
+    model = cfg.model or 'yolov8n-pose.pt'
+    data = cfg.data or 'coco8-pose.yaml'
+
+    args = dict(model=model, data=data)
+    if use_python:
+        from ultralytics import YOLO
+        YOLO(model).val(**args)
+    else:
+        validator = PoseValidator(args=args)
+        validator(model=args['model'])
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     val()
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/v8/segment/train.py` & `ultralytics-8.0.90/ultralytics/yolo/v8/pose/train.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,157 +1,180 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
 from copy import copy
 
-import hydra
 import torch
-import torch.nn.functional as F
+import torch.nn as nn
 
-from ultralytics.nn.tasks import SegmentationModel
+from ultralytics.nn.tasks import PoseModel
 from ultralytics.yolo import v8
-from ultralytics.yolo.utils import DEFAULT_CONFIG
-from ultralytics.yolo.utils.ops import crop_mask, xyxy2xywh
+from ultralytics.yolo.utils import DEFAULT_CFG
+from ultralytics.yolo.utils.loss import KeypointLoss
+from ultralytics.yolo.utils.metrics import OKS_SIGMA
+from ultralytics.yolo.utils.ops import xyxy2xywh
 from ultralytics.yolo.utils.plotting import plot_images, plot_results
 from ultralytics.yolo.utils.tal import make_anchors
 from ultralytics.yolo.utils.torch_utils import de_parallel
 from ultralytics.yolo.v8.detect.train import Loss
 
 
 # BaseTrainer python usage
-class SegmentationTrainer(v8.detect.DetectionTrainer):
+class PoseTrainer(v8.detect.DetectionTrainer):
 
-    def __init__(self, config=DEFAULT_CONFIG, overrides=None):
+    def __init__(self, cfg=DEFAULT_CFG, overrides=None, _callbacks=None):
+        """Initialize a PoseTrainer object with specified configurations and overrides."""
         if overrides is None:
             overrides = {}
-        overrides["task"] = "segment"
-        super().__init__(config, overrides)
+        overrides['task'] = 'pose'
+        super().__init__(cfg, overrides, _callbacks)
 
     def get_model(self, cfg=None, weights=None, verbose=True):
-        model = SegmentationModel(cfg, ch=3, nc=self.data["nc"], verbose=verbose)
+        """Get pose estimation model with specified configuration and weights."""
+        model = PoseModel(cfg, ch=3, nc=self.data['nc'], data_kpt_shape=self.data['kpt_shape'], verbose=verbose)
         if weights:
             model.load(weights)
 
         return model
 
+    def set_model_attributes(self):
+        """Sets keypoints shape attribute of PoseModel."""
+        super().set_model_attributes()
+        self.model.kpt_shape = self.data['kpt_shape']
+
     def get_validator(self):
-        self.loss_names = 'box_loss', 'seg_loss', 'cls_loss', 'dfl_loss'
-        return v8.segment.SegmentationValidator(self.test_loader,
-                                                save_dir=self.save_dir,
-                                                logger=self.console,
-                                                args=copy(self.args))
+        """Returns an instance of the PoseValidator class for validation."""
+        self.loss_names = 'box_loss', 'pose_loss', 'kobj_loss', 'cls_loss', 'dfl_loss'
+        return v8.pose.PoseValidator(self.test_loader, save_dir=self.save_dir, args=copy(self.args))
 
     def criterion(self, preds, batch):
+        """Computes pose loss for the YOLO model."""
         if not hasattr(self, 'compute_loss'):
-            self.compute_loss = SegLoss(de_parallel(self.model), overlap=self.args.overlap_mask)
+            self.compute_loss = PoseLoss(de_parallel(self.model))
         return self.compute_loss(preds, batch)
 
     def plot_training_samples(self, batch, ni):
-        images = batch["img"]
-        masks = batch["masks"]
-        cls = batch["cls"].squeeze(-1)
-        bboxes = batch["bboxes"]
-        paths = batch["im_file"]
-        batch_idx = batch["batch_idx"]
-        plot_images(images, batch_idx, cls, bboxes, masks, paths=paths, fname=self.save_dir / f"train_batch{ni}.jpg")
+        """Plot a batch of training samples with annotated class labels, bounding boxes, and keypoints."""
+        images = batch['img']
+        kpts = batch['keypoints']
+        cls = batch['cls'].squeeze(-1)
+        bboxes = batch['bboxes']
+        paths = batch['im_file']
+        batch_idx = batch['batch_idx']
+        plot_images(images,
+                    batch_idx,
+                    cls,
+                    bboxes,
+                    kpts=kpts,
+                    paths=paths,
+                    fname=self.save_dir / f'train_batch{ni}.jpg')
 
     def plot_metrics(self):
-        plot_results(file=self.csv, segment=True)  # save results.png
+        """Plots training/val metrics."""
+        plot_results(file=self.csv, pose=True)  # save results.png
 
 
 # Criterion class for computing training losses
-class SegLoss(Loss):
+class PoseLoss(Loss):
 
-    def __init__(self, model, overlap=True):  # model must be de-paralleled
+    def __init__(self, model):  # model must be de-paralleled
         super().__init__(model)
-        self.nm = model.model[-1].nm  # number of masks
-        self.overlap = overlap
+        self.kpt_shape = model.model[-1].kpt_shape
+        self.bce_pose = nn.BCEWithLogitsLoss()
+        is_pose = self.kpt_shape == [17, 3]
+        nkpt = self.kpt_shape[0]  # number of keypoints
+        sigmas = torch.from_numpy(OKS_SIGMA).to(self.device) if is_pose else torch.ones(nkpt, device=self.device) / nkpt
+        self.keypoint_loss = KeypointLoss(sigmas=sigmas)
 
     def __call__(self, preds, batch):
-        loss = torch.zeros(4, device=self.device)  # box, cls, dfl
-        feats, pred_masks, proto = preds if len(preds) == 3 else preds[1]
-        batch_size, _, mask_h, mask_w = proto.shape  # batch size, number of masks, mask height, mask width
+        """Calculate the total loss and detach it."""
+        loss = torch.zeros(5, device=self.device)  # box, cls, dfl, kpt_location, kpt_visibility
+        feats, pred_kpts = preds if isinstance(preds[0], list) else preds[1]
         pred_distri, pred_scores = torch.cat([xi.view(feats[0].shape[0], self.no, -1) for xi in feats], 2).split(
             (self.reg_max * 4, self.nc), 1)
 
         # b, grids, ..
         pred_scores = pred_scores.permute(0, 2, 1).contiguous()
         pred_distri = pred_distri.permute(0, 2, 1).contiguous()
-        pred_masks = pred_masks.permute(0, 2, 1).contiguous()
+        pred_kpts = pred_kpts.permute(0, 2, 1).contiguous()
 
         dtype = pred_scores.dtype
         imgsz = torch.tensor(feats[0].shape[2:], device=self.device, dtype=dtype) * self.stride[0]  # image size (h,w)
         anchor_points, stride_tensor = make_anchors(feats, self.stride, 0.5)
 
         # targets
-        batch_idx = batch["batch_idx"].view(-1, 1)
-        targets = torch.cat((batch_idx, batch["cls"].view(-1, 1), batch["bboxes"]), 1)
+        batch_size = pred_scores.shape[0]
+        batch_idx = batch['batch_idx'].view(-1, 1)
+        targets = torch.cat((batch_idx, batch['cls'].view(-1, 1), batch['bboxes']), 1)
         targets = self.preprocess(targets.to(self.device), batch_size, scale_tensor=imgsz[[1, 0, 1, 0]])
         gt_labels, gt_bboxes = targets.split((1, 4), 2)  # cls, xyxy
         mask_gt = gt_bboxes.sum(2, keepdim=True).gt_(0)
 
-        masks = batch["masks"].to(self.device).float()
-        if tuple(masks.shape[-2:]) != (mask_h, mask_w):  # downsample
-            masks = F.interpolate(masks[None], (mask_h, mask_w), mode="nearest")[0]
-
         # pboxes
         pred_bboxes = self.bbox_decode(anchor_points, pred_distri)  # xyxy, (b, h*w, 4)
+        pred_kpts = self.kpts_decode(anchor_points, pred_kpts.view(batch_size, -1, *self.kpt_shape))  # (b, h*w, 17, 3)
 
         _, target_bboxes, target_scores, fg_mask, target_gt_idx = self.assigner(
             pred_scores.detach().sigmoid(), (pred_bboxes.detach() * stride_tensor).type(gt_bboxes.dtype),
             anchor_points * stride_tensor, gt_labels, gt_bboxes, mask_gt)
 
-        target_scores_sum = target_scores.sum()
+        target_scores_sum = max(target_scores.sum(), 1)
 
         # cls loss
         # loss[1] = self.varifocal_loss(pred_scores, target_scores, target_labels) / target_scores_sum  # VFL way
-        loss[2] = self.bce(pred_scores, target_scores.to(dtype)).sum() / target_scores_sum  # BCE
+        loss[3] = self.bce(pred_scores, target_scores.to(dtype)).sum() / target_scores_sum  # BCE
 
         # bbox loss
         if fg_mask.sum():
-            loss[0], loss[3] = self.bbox_loss(pred_distri, pred_bboxes, anchor_points, target_bboxes / stride_tensor,
-                                              target_scores, target_scores_sum, fg_mask)
+            target_bboxes /= stride_tensor
+            loss[0], loss[4] = self.bbox_loss(pred_distri, pred_bboxes, anchor_points, target_bboxes, target_scores,
+                                              target_scores_sum, fg_mask)
+            keypoints = batch['keypoints'].to(self.device).float().clone()
+            keypoints[..., 0] *= imgsz[1]
+            keypoints[..., 1] *= imgsz[0]
             for i in range(batch_size):
                 if fg_mask[i].sum():
-                    mask_idx = target_gt_idx[i][fg_mask[i]] + 1
-                    if self.overlap:
-                        gt_mask = torch.where(masks[[i]] == mask_idx.view(-1, 1, 1), 1.0, 0.0)
-                    else:
-                        gt_mask = masks[batch_idx == i][mask_idx]
-                    xyxyn = target_bboxes[i][fg_mask[i]] / imgsz[[1, 0, 1, 0]]
-                    marea = xyxy2xywh(xyxyn)[:, 2:].prod(1)
-                    mxyxy = xyxyn * torch.tensor([mask_w, mask_h, mask_w, mask_h], device=self.device)
-                    loss[1] += self.single_mask_loss(gt_mask, pred_masks[i][fg_mask[i]], proto[i], mxyxy,
-                                                     marea)  # seg loss
-        # WARNING: Uncomment lines below in case of Multi-GPU DDP unused gradient errors
-        #         else:
-        #             loss[1] += proto.sum() * 0
-        # else:
-        #     loss[1] += proto.sum() * 0
+                    idx = target_gt_idx[i][fg_mask[i]]
+                    gt_kpt = keypoints[batch_idx.view(-1) == i][idx]  # (n, 51)
+                    gt_kpt[..., 0] /= stride_tensor[fg_mask[i]]
+                    gt_kpt[..., 1] /= stride_tensor[fg_mask[i]]
+                    area = xyxy2xywh(target_bboxes[i][fg_mask[i]])[:, 2:].prod(1, keepdim=True)
+                    pred_kpt = pred_kpts[i][fg_mask[i]]
+                    kpt_mask = gt_kpt[..., 2] != 0
+                    loss[1] += self.keypoint_loss(pred_kpt, gt_kpt, kpt_mask, area)  # pose loss
+                    # kpt_score loss
+                    if pred_kpt.shape[-1] == 3:
+                        loss[2] += self.bce_pose(pred_kpt[..., 2], kpt_mask.float())  # keypoint obj loss
 
         loss[0] *= self.hyp.box  # box gain
-        loss[1] *= self.hyp.box / batch_size  # seg gain
-        loss[2] *= self.hyp.cls  # cls gain
-        loss[3] *= self.hyp.dfl  # dfl gain
+        loss[1] *= self.hyp.pose / batch_size  # pose gain
+        loss[2] *= self.hyp.kobj / batch_size  # kobj gain
+        loss[3] *= self.hyp.cls  # cls gain
+        loss[4] *= self.hyp.dfl  # dfl gain
 
         return loss.sum() * batch_size, loss.detach()  # loss(box, cls, dfl)
 
-    def single_mask_loss(self, gt_mask, pred, proto, xyxy, area):
-        # Mask loss for one image
-        pred_mask = (pred @ proto.view(self.nm, -1)).view(-1, *proto.shape[1:])  # (n, 32) @ (32,80,80) -> (n,80,80)
-        loss = F.binary_cross_entropy_with_logits(pred_mask, gt_mask, reduction="none")
-        return (crop_mask(loss, xyxy).mean(dim=(1, 2)) / area).mean()
-
-
-@hydra.main(version_base=None, config_path=str(DEFAULT_CONFIG.parent), config_name=DEFAULT_CONFIG.name)
-def train(cfg):
-    cfg.model = cfg.model or "yolov8n-seg.pt"
-    cfg.data = cfg.data or "coco128-seg.yaml"  # or yolo.ClassificationDataset("mnist")
-    cfg.device = cfg.device if cfg.device is not None else ''
-    # trainer = SegmentationTrainer(cfg)
-    # trainer.train()
-    from ultralytics import YOLO
-    model = YOLO(cfg.model)
-    model.train(**cfg)
+    def kpts_decode(self, anchor_points, pred_kpts):
+        """Decodes predicted keypoints to image coordinates."""
+        y = pred_kpts.clone()
+        y[..., :2] *= 2.0
+        y[..., 0] += anchor_points[:, [0]] - 0.5
+        y[..., 1] += anchor_points[:, [1]] - 0.5
+        return y
+
+
+def train(cfg=DEFAULT_CFG, use_python=False):
+    """Train the YOLO model on the given data and device."""
+    model = cfg.model or 'yolov8n-pose.yaml'
+    data = cfg.data or 'coco8-pose.yaml'
+    device = cfg.device if cfg.device is not None else ''
+
+    args = dict(model=model, data=data, device=device)
+    if use_python:
+        from ultralytics import YOLO
+        YOLO(model).train(**args)
+    else:
+        trainer = PoseTrainer(overrides=args)
+        trainer.train()
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     train()
```

### Comparing `ultralytics-8.0.9/ultralytics/yolo/v8/segment/val.py` & `ultralytics-8.0.90/ultralytics/yolo/v8/segment/val.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,141 +1,137 @@
-# Ultralytics YOLO 🚀, GPL-3.0 license
+# Ultralytics YOLO 🚀, AGPL-3.0 license
 
-import os
 from multiprocessing.pool import ThreadPool
 from pathlib import Path
 
-import hydra
 import numpy as np
 import torch
 import torch.nn.functional as F
 
-from ultralytics.yolo.utils import DEFAULT_CONFIG, NUM_THREADS, ops
+from ultralytics.yolo.utils import DEFAULT_CFG, LOGGER, NUM_THREADS, ops
 from ultralytics.yolo.utils.checks import check_requirements
-from ultralytics.yolo.utils.metrics import ConfusionMatrix, SegmentMetrics, box_iou, mask_iou
+from ultralytics.yolo.utils.metrics import SegmentMetrics, box_iou, mask_iou
 from ultralytics.yolo.utils.plotting import output_to_target, plot_images
 from ultralytics.yolo.v8.detect import DetectionValidator
 
 
 class SegmentationValidator(DetectionValidator):
 
-    def __init__(self, dataloader=None, save_dir=None, pbar=None, logger=None, args=None):
-        super().__init__(dataloader, save_dir, pbar, logger, args)
-        self.args.task = "segment"
+    def __init__(self, dataloader=None, save_dir=None, pbar=None, args=None, _callbacks=None):
+        """Initialize SegmentationValidator and set task to 'segment', metrics to SegmentMetrics."""
+        super().__init__(dataloader, save_dir, pbar, args, _callbacks)
+        self.args.task = 'segment'
         self.metrics = SegmentMetrics(save_dir=self.save_dir)
 
     def preprocess(self, batch):
+        """Preprocesses batch by converting masks to float and sending to device."""
         batch = super().preprocess(batch)
-        batch["masks"] = batch["masks"].to(self.device).float()
+        batch['masks'] = batch['masks'].to(self.device).float()
         return batch
 
     def init_metrics(self, model):
-        head = model.model[-1] if self.training else model.model.model[-1]
-        val = self.data.get('val', '')  # validation path
-        self.is_coco = isinstance(val, str) and val.endswith(f'coco{os.sep}val2017.txt')  # is COCO dataset
-        self.class_map = ops.coco80_to_coco91_class() if self.is_coco else list(range(1000))
-        self.args.save_json |= self.is_coco and not self.training  # run on final val if training COCO
-        self.nc = head.nc
-        self.nm = head.nm if hasattr(head, "nm") else 32
-        self.names = model.names
-        self.metrics.names = self.names
-        self.metrics.plot = self.args.plots
-        self.confusion_matrix = ConfusionMatrix(nc=self.nc)
+        """Initialize metrics and select mask processing function based on save_json flag."""
+        super().init_metrics(model)
         self.plot_masks = []
-        self.seen = 0
-        self.jdict = []
-        self.stats = []
         if self.args.save_json:
+            check_requirements('pycocotools>=2.0.6')
             self.process = ops.process_mask_upsample  # more accurate
         else:
             self.process = ops.process_mask  # faster
 
     def get_desc(self):
-        return ('%22s' + '%11s' * 10) % ('Class', 'Images', 'Instances', 'Box(P', "R", "mAP50", "mAP50-95)", "Mask(P",
-                                         "R", "mAP50", "mAP50-95)")
+        """Return a formatted description of evaluation metrics."""
+        return ('%22s' + '%11s' * 10) % ('Class', 'Images', 'Instances', 'Box(P', 'R', 'mAP50', 'mAP50-95)', 'Mask(P',
+                                         'R', 'mAP50', 'mAP50-95)')
 
     def postprocess(self, preds):
+        """Postprocesses YOLO predictions and returns output detections with proto."""
         p = ops.non_max_suppression(preds[0],
                                     self.args.conf,
                                     self.args.iou,
                                     labels=self.lb,
                                     multi_label=True,
                                     agnostic=self.args.single_cls,
                                     max_det=self.args.max_det,
-                                    nm=self.nm)
-        return p, preds[1][-1]
+                                    nc=self.nc)
+        proto = preds[1][-1] if len(preds[1]) == 3 else preds[1]  # second output is len 3 if pt, but only 1 if exported
+        return p, proto
 
     def update_metrics(self, preds, batch):
-        # Metrics
+        """Metrics."""
         for si, (pred, proto) in enumerate(zip(preds[0], preds[1])):
-            idx = batch["batch_idx"] == si
-            cls = batch["cls"][idx]
-            bbox = batch["bboxes"][idx]
+            idx = batch['batch_idx'] == si
+            cls = batch['cls'][idx]
+            bbox = batch['bboxes'][idx]
             nl, npr = cls.shape[0], pred.shape[0]  # number of labels, predictions
-            shape = batch["ori_shape"][si]
+            shape = batch['ori_shape'][si]
             correct_masks = torch.zeros(npr, self.niou, dtype=torch.bool, device=self.device)  # init
             correct_bboxes = torch.zeros(npr, self.niou, dtype=torch.bool, device=self.device)  # init
             self.seen += 1
 
             if npr == 0:
                 if nl:
-                    self.stats.append((correct_masks, correct_bboxes, *torch.zeros(
+                    self.stats.append((correct_bboxes, correct_masks, *torch.zeros(
                         (2, 0), device=self.device), cls.squeeze(-1)))
                     if self.args.plots:
                         self.confusion_matrix.process_batch(detections=None, labels=cls.squeeze(-1))
                 continue
 
             # Masks
             midx = [si] if self.args.overlap_mask else idx
-            gt_masks = batch["masks"][midx]
-            pred_masks = self.process(proto, pred[:, 6:], pred[:, :4], shape=batch["img"][si].shape[1:])
+            gt_masks = batch['masks'][midx]
+            pred_masks = self.process(proto, pred[:, 6:], pred[:, :4], shape=batch['img'][si].shape[1:])
 
             # Predictions
             if self.args.single_cls:
                 pred[:, 5] = 0
             predn = pred.clone()
-            ops.scale_boxes(batch["img"][si].shape[1:], predn[:, :4], shape,
-                            ratio_pad=batch["ratio_pad"][si])  # native-space pred
+            ops.scale_boxes(batch['img'][si].shape[1:], predn[:, :4], shape,
+                            ratio_pad=batch['ratio_pad'][si])  # native-space pred
 
             # Evaluate
             if nl:
-                height, width = batch["img"].shape[2:]
+                height, width = batch['img'].shape[2:]
                 tbox = ops.xywh2xyxy(bbox) * torch.tensor(
                     (width, height, width, height), device=self.device)  # target boxes
-                ops.scale_boxes(batch["img"][si].shape[1:], tbox, shape,
-                                ratio_pad=batch["ratio_pad"][si])  # native-space labels
+                ops.scale_boxes(batch['img'][si].shape[1:], tbox, shape,
+                                ratio_pad=batch['ratio_pad'][si])  # native-space labels
                 labelsn = torch.cat((cls, tbox), 1)  # native-space labels
                 correct_bboxes = self._process_batch(predn, labelsn)
                 # TODO: maybe remove these `self.` arguments as they already are member variable
                 correct_masks = self._process_batch(predn,
                                                     labelsn,
                                                     pred_masks,
                                                     gt_masks,
                                                     overlap=self.args.overlap_mask,
                                                     masks=True)
                 if self.args.plots:
                     self.confusion_matrix.process_batch(predn, labelsn)
 
             # Append correct_masks, correct_boxes, pconf, pcls, tcls
-            self.stats.append((correct_masks, correct_bboxes, pred[:, 4], pred[:, 5], cls.squeeze(-1)))
+            self.stats.append((correct_bboxes, correct_masks, pred[:, 4], pred[:, 5], cls.squeeze(-1)))
 
             pred_masks = torch.as_tensor(pred_masks, dtype=torch.uint8)
             if self.args.plots and self.batch_i < 3:
                 self.plot_masks.append(pred_masks[:15].cpu())  # filter top 15 to plot
 
             # Save
             if self.args.save_json:
-                pred_masks = ops.scale_image(batch["img"][si].shape[1:],
-                                             pred_masks.permute(1, 2, 0).contiguous().cpu().numpy(),
+                pred_masks = ops.scale_image(pred_masks.permute(1, 2, 0).contiguous().cpu().numpy(),
                                              shape,
-                                             ratio_pad=batch["ratio_pad"][si])
-                self.pred_to_json(predn, batch["im_file"][si], pred_masks)
+                                             ratio_pad=batch['ratio_pad'][si])
+                self.pred_to_json(predn, batch['im_file'][si], pred_masks)
             # if self.args.save_txt:
             #    save_one_txt(predn, save_conf, shape, file=save_dir / 'labels' / f'{path.stem}.txt')
 
+    def finalize_metrics(self, *args, **kwargs):
+        """Sets speed and confusion matrix for evaluation metrics."""
+        self.metrics.speed = self.speed
+        self.metrics.confusion_matrix = self.confusion_matrix
+
     def _process_batch(self, detections, labels, pred_masks=None, gt_masks=None, overlap=False, masks=False):
         """
         Return correct prediction matrix
         Arguments:
             detections (array[N, 6]), x1, y1, x2, y2, conf, class
             labels (array[M, 5]), class, x1, y1, x2, y2
         Returns:
@@ -144,15 +140,15 @@
         if masks:
             if overlap:
                 nl = len(labels)
                 index = torch.arange(nl, device=gt_masks.device).view(nl, 1, 1) + 1
                 gt_masks = gt_masks.repeat(nl, 1, 1)  # shape(1,640,640) -> (n,640,640)
                 gt_masks = torch.where(gt_masks == index, 1.0, 0.0)
             if gt_masks.shape[1:] != pred_masks.shape[1:]:
-                gt_masks = F.interpolate(gt_masks[None], pred_masks.shape[1:], mode="bilinear", align_corners=False)[0]
+                gt_masks = F.interpolate(gt_masks[None], pred_masks.shape[1:], mode='bilinear', align_corners=False)[0]
                 gt_masks = gt_masks.gt_(0.5)
             iou = mask_iou(gt_masks.view(gt_masks.shape[0], -1), pred_masks.view(pred_masks.shape[0], -1))
         else:  # boxes
             iou = box_iou(labels[:, 1:], detections[:, :4])
 
         correct = np.zeros((detections.shape[0], self.iouv.shape[0])).astype(bool)
         correct_class = labels[:, 0:1] == detections[:, 5]
@@ -166,39 +162,43 @@
                     matches = matches[np.unique(matches[:, 1], return_index=True)[1]]
                     # matches = matches[matches[:, 2].argsort()[::-1]]
                     matches = matches[np.unique(matches[:, 0], return_index=True)[1]]
                 correct[matches[:, 1].astype(int), i] = True
         return torch.tensor(correct, dtype=torch.bool, device=detections.device)
 
     def plot_val_samples(self, batch, ni):
-        plot_images(batch["img"],
-                    batch["batch_idx"],
-                    batch["cls"].squeeze(-1),
-                    batch["bboxes"],
-                    batch["masks"],
-                    paths=batch["im_file"],
-                    fname=self.save_dir / f"val_batch{ni}_labels.jpg",
+        """Plots validation samples with bounding box labels."""
+        plot_images(batch['img'],
+                    batch['batch_idx'],
+                    batch['cls'].squeeze(-1),
+                    batch['bboxes'],
+                    batch['masks'],
+                    paths=batch['im_file'],
+                    fname=self.save_dir / f'val_batch{ni}_labels.jpg',
                     names=self.names)
 
     def plot_predictions(self, batch, preds, ni):
-        plot_images(batch["img"],
+        """Plots batch predictions with masks and bounding boxes."""
+        plot_images(batch['img'],
                     *output_to_target(preds[0], max_det=15),
                     torch.cat(self.plot_masks, dim=0) if len(self.plot_masks) else self.plot_masks,
-                    paths=batch["im_file"],
+                    paths=batch['im_file'],
                     fname=self.save_dir / f'val_batch{ni}_pred.jpg',
                     names=self.names)  # pred
         self.plot_masks.clear()
 
     def pred_to_json(self, predn, filename, pred_masks):
-        # Save one JSON result {"image_id": 42, "category_id": 18, "bbox": [258.15, 41.29, 348.26, 243.78], "score": 0.236}
-        from pycocotools.mask import encode
+        """Save one JSON result."""
+        # Example result = {"image_id": 42, "category_id": 18, "bbox": [258.15, 41.29, 348.26, 243.78], "score": 0.236}
+        from pycocotools.mask import encode  # noqa
 
         def single_encode(x):
-            rle = encode(np.asarray(x[:, :, None], order="F", dtype="uint8"))[0]
-            rle["counts"] = rle["counts"].decode("utf-8")
+            """Encode predicted masks as RLE and append results to jdict."""
+            rle = encode(np.asarray(x[:, :, None], order='F', dtype='uint8'))[0]
+            rle['counts'] = rle['counts'].decode('utf-8')
             return rle
 
         stem = Path(filename).stem
         image_id = int(stem) if stem.isnumeric() else stem
         box = ops.xyxy2xywh(predn[:, :4])  # xywh
         box[:, :2] -= box[:, 2:] / 2  # xy center to top-left corner
         pred_masks = np.transpose(pred_masks, (2, 0, 1))
@@ -209,44 +209,51 @@
                 'image_id': image_id,
                 'category_id': self.class_map[int(p[5])],
                 'bbox': [round(x, 3) for x in b],
                 'score': round(p[4], 5),
                 'segmentation': rles[i]})
 
     def eval_json(self, stats):
+        """Return COCO-style object detection evaluation metrics."""
         if self.args.save_json and self.is_coco and len(self.jdict):
-            anno_json = self.data['path'] / "annotations/instances_val2017.json"  # annotations
-            pred_json = self.save_dir / "predictions.json"  # predictions
-            self.logger.info(f'\nEvaluating pycocotools mAP using {pred_json} and {anno_json}...')
+            anno_json = self.data['path'] / 'annotations/instances_val2017.json'  # annotations
+            pred_json = self.save_dir / 'predictions.json'  # predictions
+            LOGGER.info(f'\nEvaluating pycocotools mAP using {pred_json} and {anno_json}...')
             try:  # https://github.com/cocodataset/cocoapi/blob/master/PythonAPI/pycocoEvalDemo.ipynb
                 check_requirements('pycocotools>=2.0.6')
                 from pycocotools.coco import COCO  # noqa
                 from pycocotools.cocoeval import COCOeval  # noqa
 
                 for x in anno_json, pred_json:
-                    assert x.is_file(), f"{x} file not found"
+                    assert x.is_file(), f'{x} file not found'
                 anno = COCO(str(anno_json))  # init annotations api
                 pred = anno.loadRes(str(pred_json))  # init predictions api (must pass string, not Path)
                 for i, eval in enumerate([COCOeval(anno, pred, 'bbox'), COCOeval(anno, pred, 'segm')]):
                     if self.is_coco:
-                        eval.params.imgIds = [int(Path(x).stem)
-                                              for x in self.dataloader.dataset.im_files]  # images to eval
+                        eval.params.imgIds = [int(Path(x).stem) for x in self.dataloader.dataset.im_files]  # im to eval
                     eval.evaluate()
                     eval.accumulate()
                     eval.summarize()
                     idx = i * 4 + 2
                     stats[self.metrics.keys[idx + 1]], stats[
                         self.metrics.keys[idx]] = eval.stats[:2]  # update mAP50-95 and mAP50
             except Exception as e:
-                self.logger.warning(f'pycocotools unable to run: {e}')
+                LOGGER.warning(f'pycocotools unable to run: {e}')
         return stats
 
 
-@hydra.main(version_base=None, config_path=str(DEFAULT_CONFIG.parent), config_name=DEFAULT_CONFIG.name)
-def val(cfg):
-    cfg.data = cfg.data or "coco128-seg.yaml"
-    validator = SegmentationValidator(args=cfg)
-    validator(model=cfg.model)
+def val(cfg=DEFAULT_CFG, use_python=False):
+    """Validate trained YOLO model on validation data."""
+    model = cfg.model or 'yolov8n-seg.pt'
+    data = cfg.data or 'coco128-seg.yaml'
+
+    args = dict(model=model, data=data)
+    if use_python:
+        from ultralytics import YOLO
+        YOLO(model).val(**args)
+    else:
+        validator = SegmentationValidator(args=args)
+        validator(model=args['model'])
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     val()
```

### Comparing `ultralytics-8.0.9/ultralytics.egg-info/PKG-INFO` & `ultralytics-8.0.90/ultralytics.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.0.9
+Version: 8.0.90
 Summary: Ultralytics YOLOv8
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
-License: GPL-3.0
+License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/ultralytics
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7,<=3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: export
 License-File: LICENSE
 
 <div align="center">
   <p>
-    <a align="center" href="https://ultralytics.com/yolov8" target="_blank">
+    <a href="https://ultralytics.com/yolov8" target="_blank">
       <img width="100%" src="https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/banner-yolov8.png"></a>
   </p>
 
 [English](README.md) | [简体中文](README.zh-CN.md)
 <br>
 
 <div>
@@ -46,80 +50,54 @@
     <br>
     <a href="https://console.paperspace.com/github/ultralytics/ultralytics"><img src="https://assets.paperspace.io/img/gradient-badge.svg" alt="Run on Gradient"/></a>
     <a href="https://colab.research.google.com/github/ultralytics/ultralytics/blob/main/examples/tutorial.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>
     <a href="https://www.kaggle.com/ultralytics/yolov8"><img src="https://kaggle.com/static/images/open-in-kaggle.svg" alt="Open In Kaggle"></a>
   </div>
   <br>
 
-[Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics), developed by [Ultralytics](https://ultralytics.com),
-is a cutting-edge, state-of-the-art (SOTA) model that builds upon the success of previous YOLO versions and introduces
-new features and improvements to further boost performance and flexibility. YOLOv8 is designed to be fast, accurate, and
-easy to use, making it an excellent choice for a wide range of object detection, image segmentation and image
-classification tasks.
+[Ultralytics](https://ultralytics.com) [YOLOv8](https://github.com/ultralytics/ultralytics) is a cutting-edge, state-of-the-art (SOTA) model that builds upon the success of previous YOLO versions and introduces new features and improvements to further boost performance and flexibility. YOLOv8 is designed to be fast, accurate, and easy to use, making it an excellent choice for a wide range of object detection and tracking, instance segmentation, image classification and pose estimation tasks.
+
+We hope that the resources here will help you get the most out of YOLOv8. Please browse the YOLOv8 <a href="https://docs.ultralytics.com/">Docs</a> for details, raise an issue on <a href="https://github.com/ultralytics/ultralytics/issues/new/choose">GitHub</a> for support, and join our <a href="https://discord.gg/n6cFeSPZdD">Discord</a> community for questions and discussions!
 
 To request an Enterprise License please complete the form at [Ultralytics Licensing](https://ultralytics.com/license).
 
 <img width="100%" src="https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/yolo-comparison-plots.png"></a>
 
 <div align="center">
-    <a href="https://github.com/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://www.linkedin.com/company/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://twitter.com/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://www.producthunt.com/@glenn_jocher" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-producthunt.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://youtube.com/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://www.facebook.com/ultralytics" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-facebook.png" width="2%" alt="" /></a>
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
-    <a href="https://www.instagram.com/ultralytics/" style="text-decoration:none;">
-      <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="2%" alt="" /></a>
-  </div>
+  <a href="https://github.com/ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://www.linkedin.com/company/ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://twitter.com/ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://youtube.com/ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://www.tiktok.com/@ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-tiktok.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://www.instagram.com/ultralytics/" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="2%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="2%" alt="" />
+  <a href="https://discord.gg/n6cFeSPZdD" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/blob/main/social/logo-social-discord.png" width="2%" alt="" /></a>
 </div>
-
-## <div align="center">Ultralytics Live Session</div>
-
-<div align="center">
-
-[Ultralytics Live Session 3](https://youtu.be/IPcpYO5ITa8) ✨ is here! Join us on January 24th at 18 CET as we dive into
-the latest advancements in YOLOv8, and demonstrate how to use this cutting-edge, SOTA model to improve your object
-detection, instance segmentation, and image classification projects. See firsthand how YOLOv8's speed, accuracy, and
-ease of use make it a top choice for professionals and researchers alike.
-
-In addition to learning about the exciting new features and improvements of Ultralytics YOLOv8, you will also have the
-opportunity to ask questions and interact with our team during the live Q&A session. We encourage you to come prepared
-with any questions you may have.
-
-To join the webinar, visit our YouTube [Channel](https://www.youtube.com/@Ultralytics/streams) and turn on your
-notifications!
-
-<a align="center" href="https://youtu.be/IPcpYO5ITa8" target="_blank">
-<img width="80%" src="https://user-images.githubusercontent.com/107626595/212887899-e94b006c-5192-40fa-8b24-7b5428e065e8.png"></a>
 </div>
 
 ## <div align="center">Documentation</div>
 
-See below for a quickstart installation and usage example, and see the [YOLOv8 Docs](https://docs.ultralytics.com) for
-full documentation on training, validation, prediction and deployment.
+See below for a quickstart installation and usage example, and see the [YOLOv8 Docs](https://docs.ultralytics.com) for full documentation on training, validation, prediction and deployment.
 
 <details open>
 <summary>Install</summary>
 
-Pip install the ultralytics package including
-all [requirements.txt](https://github.com/ultralytics/ultralytics/blob/main/requirements.txt) in a
-[**3.10>=Python>=3.7**](https://www.python.org/) environment, including
-[**PyTorch>=1.7**](https://pytorch.org/get-started/locally/).
+Pip install the ultralytics package including all [requirements](https://github.com/ultralytics/ultralytics/blob/main/requirements.txt) in a [**Python>=3.7**](https://www.python.org/) environment with [**PyTorch>=1.7**](https://pytorch.org/get-started/locally/).
 
 ```bash
 pip install ultralytics
 ```
 
 </details>
 
@@ -127,199 +105,194 @@
 <summary>Usage</summary>
 
 #### CLI
 
 YOLOv8 may be used directly in the Command Line Interface (CLI) with a `yolo` command:
 
 ```bash
-yolo predict model=yolov8n.pt source="https://ultralytics.com/images/bus.jpg"
+yolo predict model=yolov8n.pt source='https://ultralytics.com/images/bus.jpg'
 ```
 
-`yolo` can be used for a variety of tasks and modes and accepts additional arguments, i.e. `imgsz=640`. See the YOLOv8
-[CLI Docs](https://docs.ultralytics.com/cli) for examples.
+`yolo` can be used for a variety of tasks and modes and accepts additional arguments, i.e. `imgsz=640`. See the YOLOv8 [CLI Docs](https://docs.ultralytics.com/usage/cli) for examples.
 
 #### Python
 
-YOLOv8 may also be used directly in a Python environment, and accepts the
-same [arguments](https://docs.ultralytics.com/config/) as in the CLI example above:
+YOLOv8 may also be used directly in a Python environment, and accepts the same [arguments](https://docs.ultralytics.com/usage/cfg/) as in the CLI example above:
 
 ```python
 from ultralytics import YOLO
 
 # Load a model
 model = YOLO("yolov8n.yaml")  # build a new model from scratch
 model = YOLO("yolov8n.pt")  # load a pretrained model (recommended for training)
 
 # Use the model
-results = model.train(data="coco128.yaml", epochs=3)  # train the model
-results = model.val()  # evaluate model performance on the validation set
+model.train(data="coco128.yaml", epochs=3)  # train the model
+metrics = model.val()  # evaluate model performance on the validation set
 results = model("https://ultralytics.com/images/bus.jpg")  # predict on an image
 success = model.export(format="onnx")  # export the model to ONNX format
 ```
 
-[Models](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) download automatically from the latest
-Ultralytics [release](https://github.com/ultralytics/assets/releases). See
-YOLOv8 [Python Docs](https://docs.ultralytics.com/python) for more examples.
-
-#### Known Issues / TODOs
-
-We are still working on several parts of YOLOv8! We aim to have these completed soon to bring the YOLOv8 feature set up
-to par with YOLOv5, including export and inference to all the same formats. We are also writing a YOLOv8 paper which we
-will submit to [arxiv.org](https://arxiv.org) once complete.
-
-- [ ] TensorFlow exports
-- [ ] DDP resume
-- [ ] [arxiv.org](https://arxiv.org) paper
+[Models](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) download automatically from the latest Ultralytics [release](https://github.com/ultralytics/assets/releases). See YOLOv8 [Python Docs](https://docs.ultralytics.com/usage/python) for more examples.
 
 </details>
 
 ## <div align="center">Models</div>
 
-All YOLOv8 pretrained models are available here. Detection and Segmentation models are pretrained on the COCO dataset,
-while Classification models are pretrained on the ImageNet dataset.
+All YOLOv8 pretrained models are available here. Detect, Segment and Pose models are pretrained on the [COCO](https://github.com/ultralytics/ultralytics/blob/main/ultralytics/datasets/coco.yaml) dataset, while Classify models are pretrained on the [ImageNet](https://github.com/ultralytics/ultralytics/blob/main/ultralytics/datasets/ImageNet.yaml) dataset.
 
-[Models](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) download automatically from the latest
-Ultralytics [release](https://github.com/ultralytics/assets/releases) on first use.
+[Models](https://github.com/ultralytics/ultralytics/tree/main/ultralytics/models) download automatically from the latest Ultralytics [release](https://github.com/ultralytics/assets/releases) on first use.
 
 <details open><summary>Detection</summary>
 
-See [Detection Docs](https://docs.ultralytics.com/tasks/detection/) for usage examples with these models.
+See [Detection Docs](https://docs.ultralytics.com/tasks/detect/) for usage examples with these models.
 
 | Model                                                                                | size<br><sup>(pixels) | mAP<sup>val<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |
 | ------------------------------------------------------------------------------------ | --------------------- | -------------------- | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
 | [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n.pt) | 640                   | 37.3                 | 80.4                           | 0.99                                | 3.2                | 8.7               |
 | [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s.pt) | 640                   | 44.9                 | 128.4                          | 1.20                                | 11.2               | 28.6              |
 | [YOLOv8m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m.pt) | 640                   | 50.2                 | 234.7                          | 1.83                                | 25.9               | 78.9              |
 | [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l.pt) | 640                   | 52.9                 | 375.2                          | 2.39                                | 43.7               | 165.2             |
 | [YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x.pt) | 640                   | 53.9                 | 479.1                          | 3.53                                | 68.2               | 257.8             |
 
 - **mAP<sup>val</sup>** values are for single-model single-scale on [COCO val2017](http://cocodataset.org) dataset.
   <br>Reproduce by `yolo val detect data=coco.yaml device=0`
-- **Speed** averaged over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/)
-  instance.
-  <br>Reproduce by `yolo val detect data=coco128.yaml batch=1 device=0/cpu`
+- **Speed** averaged over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) instance.
+  <br>Reproduce by `yolo val detect data=coco128.yaml batch=1 device=0|cpu`
 
 </details>
 
 <details><summary>Segmentation</summary>
 
-See [Segmentation Docs](https://docs.ultralytics.com/tasks/segmentation/) for usage examples with these models.
+See [Segmentation Docs](https://docs.ultralytics.com/tasks/segment/) for usage examples with these models.
 
-| Model                                                                                    | size<br><sup>(pixels) | mAP<sup>box<br>50-95 | mAP<sup>mask<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |
-| ---------------------------------------------------------------------------------------- | --------------------- | -------------------- | --------------------- | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
-| [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640                   | 36.7                 | 30.5                  | 96.1                           | 1.21                                | 3.4                | 12.6              |
-| [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-seg.pt) | 640                   | 44.6                 | 36.8                  | 155.7                          | 1.47                                | 11.8               | 42.6              |
-| [YOLOv8m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-seg.pt) | 640                   | 49.9                 | 40.8                  | 317.0                          | 2.18                                | 27.3               | 110.2             |
-| [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-seg.pt) | 640                   | 52.3                 | 42.6                  | 572.4                          | 2.79                                | 46.0               | 220.5             |
-| [YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-seg.pt) | 640                   | 53.4                 | 43.4                  | 712.1                          | 4.02                                | 71.8               | 344.1             |
+| Model                                                                                        | size<br><sup>(pixels) | mAP<sup>box<br>50-95 | mAP<sup>mask<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |
+| -------------------------------------------------------------------------------------------- | --------------------- | -------------------- | --------------------- | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
+| [YOLOv8n-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640                   | 36.7                 | 30.5                  | 96.1                           | 1.21                                | 3.4                | 12.6              |
+| [YOLOv8s-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-seg.pt) | 640                   | 44.6                 | 36.8                  | 155.7                          | 1.47                                | 11.8               | 42.6              |
+| [YOLOv8m-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-seg.pt) | 640                   | 49.9                 | 40.8                  | 317.0                          | 2.18                                | 27.3               | 110.2             |
+| [YOLOv8l-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-seg.pt) | 640                   | 52.3                 | 42.6                  | 572.4                          | 2.79                                | 46.0               | 220.5             |
+| [YOLOv8x-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-seg.pt) | 640                   | 53.4                 | 43.4                  | 712.1                          | 4.02                                | 71.8               | 344.1             |
 
 - **mAP<sup>val</sup>** values are for single-model single-scale on [COCO val2017](http://cocodataset.org) dataset.
   <br>Reproduce by `yolo val segment data=coco.yaml device=0`
-- **Speed** averaged over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/)
-  instance.
-  <br>Reproduce by `yolo val segment data=coco128-seg.yaml batch=1 device=0/cpu`
+- **Speed** averaged over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) instance.
+  <br>Reproduce by `yolo val segment data=coco128-seg.yaml batch=1 device=0|cpu`
 
 </details>
 
 <details><summary>Classification</summary>
 
-See [Classification Docs](https://docs.ultralytics.com/tasks/classification/) for usage examples with these models.
+See [Classification Docs](https://docs.ultralytics.com/tasks/classify/) for usage examples with these models.
 
-| Model                                                                                    | size<br><sup>(pixels) | acc<br><sup>top1 | acc<br><sup>top5 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) at 640 |
-| ---------------------------------------------------------------------------------------- | --------------------- | ---------------- | ---------------- | ------------------------------ | ----------------------------------- | ------------------ | ------------------------ |
-| [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-cls.pt) | 224                   | 66.6             | 87.0             | 12.9                           | 0.31                                | 2.7                | 4.3                      |
-| [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-cls.pt) | 224                   | 72.3             | 91.1             | 23.4                           | 0.35                                | 6.4                | 13.5                     |
-| [YOLOv8m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-cls.pt) | 224                   | 76.4             | 93.2             | 85.4                           | 0.62                                | 17.0               | 42.7                     |
-| [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-cls.pt) | 224                   | 78.0             | 94.1             | 163.0                          | 0.87                                | 37.5               | 99.7                     |
-| [YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-cls.pt) | 224                   | 78.4             | 94.3             | 232.0                          | 1.01                                | 57.4               | 154.8                    |
+| Model                                                                                        | size<br><sup>(pixels) | acc<br><sup>top1 | acc<br><sup>top5 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) at 640 |
+| -------------------------------------------------------------------------------------------- | --------------------- | ---------------- | ---------------- | ------------------------------ | ----------------------------------- | ------------------ | ------------------------ |
+| [YOLOv8n-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-cls.pt) | 224                   | 66.6             | 87.0             | 12.9                           | 0.31                                | 2.7                | 4.3                      |
+| [YOLOv8s-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-cls.pt) | 224                   | 72.3             | 91.1             | 23.4                           | 0.35                                | 6.4                | 13.5                     |
+| [YOLOv8m-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-cls.pt) | 224                   | 76.4             | 93.2             | 85.4                           | 0.62                                | 17.0               | 42.7                     |
+| [YOLOv8l-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-cls.pt) | 224                   | 78.0             | 94.1             | 163.0                          | 0.87                                | 37.5               | 99.7                     |
+| [YOLOv8x-cls](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-cls.pt) | 224                   | 78.4             | 94.3             | 232.0                          | 1.01                                | 57.4               | 154.8                    |
 
 - **acc** values are model accuracies on the [ImageNet](https://www.image-net.org/) dataset validation set.
   <br>Reproduce by `yolo val classify data=path/to/ImageNet device=0`
-- **Speed** averaged over ImageNet val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/)
-  instance.
-  <br>Reproduce by `yolo val classify data=path/to/ImageNet batch=1 device=0/cpu`
+- **Speed** averaged over ImageNet val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) instance.
+  <br>Reproduce by `yolo val classify data=path/to/ImageNet batch=1 device=0|cpu`
+
+</details>
+
+<details><summary>Pose</summary>
+
+See [Pose Docs](https://docs.ultralytics.com/tasks/pose) for usage examples with these models.
+
+| Model                                                                                                | size<br><sup>(pixels) | mAP<sup>pose<br>50-95 | mAP<sup>pose<br>50 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |
+| ---------------------------------------------------------------------------------------------------- | --------------------- | --------------------- | ------------------ | ------------------------------ | ----------------------------------- | ------------------ | ----------------- |
+| [YOLOv8n-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-pose.pt)       | 640                   | 50.4                  | 80.1               | 131.8                          | 1.18                                | 3.3                | 9.2               |
+| [YOLOv8s-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-pose.pt)       | 640                   | 60.0                  | 86.2               | 233.2                          | 1.42                                | 11.6               | 30.2              |
+| [YOLOv8m-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-pose.pt)       | 640                   | 65.0                  | 88.8               | 456.3                          | 2.00                                | 26.4               | 81.0              |
+| [YOLOv8l-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l-pose.pt)       | 640                   | 67.6                  | 90.0               | 784.5                          | 2.59                                | 44.4               | 168.6             |
+| [YOLOv8x-pose](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-pose.pt)       | 640                   | 69.2                  | 90.2               | 1607.1                         | 3.73                                | 69.4               | 263.2             |
+| [YOLOv8x-pose-p6](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x-pose-p6.pt) | 1280                  | 71.6                  | 91.2               | 4088.7                         | 10.04                               | 99.1               | 1066.4            |
+
+- **mAP<sup>val</sup>** values are for single-model single-scale on [COCO Keypoints val2017](http://cocodataset.org)
+  dataset.
+  <br>Reproduce by `yolo val pose data=coco-pose.yaml device=0`
+- **Speed** averaged over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/instance-types/p4/) instance.
+  <br>Reproduce by `yolo val pose data=coco8-pose.yaml batch=1 device=0|cpu`
 
 </details>
 
 ## <div align="center">Integrations</div>
 
 <br>
-<a align="center" href="https://bit.ly/ultralytics_hub" target="_blank">
+<a href="https://bit.ly/ultralytics_hub" target="_blank">
 <img width="100%" src="https://github.com/ultralytics/assets/raw/main/yolov8/banner-integrations.png"></a>
 <br>
 <br>
 
 <div align="center">
   <a href="https://roboflow.com/?ref=ultralytics">
-    <img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-roboflow.png" width="10%" /></a>
+    <img src="https://github.com/ultralytics/assets/raw/main/partners/logo-roboflow.png" width="10%" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="15%" height="0" alt="" />
   <a href="https://cutt.ly/yolov5-readme-clearml">
-    <img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-clearml.png" width="10%" /></a>
+    <img src="https://github.com/ultralytics/assets/raw/main/partners/logo-clearml.png" width="10%" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="15%" height="0" alt="" />
-  <a href="https://bit.ly/yolov5-readme-comet">
-    <img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-comet.png" width="10%" /></a>
+  <a href="https://bit.ly/yolov8-readme-comet">
+    <img src="https://github.com/ultralytics/assets/raw/main/partners/logo-comet.png" width="10%" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="15%" height="0" alt="" />
   <a href="https://bit.ly/yolov5-neuralmagic">
-    <img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-neuralmagic.png" width="10%" /></a>
+    <img src="https://github.com/ultralytics/assets/raw/main/partners/logo-neuralmagic.png" width="10%" /></a>
 </div>
 
-|                                                           Roboflow                                                           |                                                            ClearML ⭐ NEW                                                            |                                                                        Comet ⭐ NEW                                                                         |                                           Neural Magic ⭐ NEW                                           |
-| :--------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------: |
-| Label and export your custom datasets directly to YOLOv8 for training with [Roboflow](https://roboflow.com/?ref=ultralytics) | Automatically track, visualize and even remotely train YOLOv8 using [ClearML](https://cutt.ly/yolov5-readme-clearml) (open-source!) | Free forever, [Comet](https://bit.ly/yolov5-readme-comet2) lets you save YOLOv8 models, resume training, and interactively visualize and debug predictions | Run YOLOv8 inference up to 6x faster with [Neural Magic DeepSparse](https://bit.ly/yolov5-neuralmagic) |
+|                                                           Roboflow                                                           |                                                            ClearML ⭐ NEW                                                            |                                                                        Comet ⭐ NEW                                                                        |                                           Neural Magic ⭐ NEW                                           |
+| :--------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------: |
+| Label and export your custom datasets directly to YOLOv8 for training with [Roboflow](https://roboflow.com/?ref=ultralytics) | Automatically track, visualize and even remotely train YOLOv8 using [ClearML](https://cutt.ly/yolov5-readme-clearml) (open-source!) | Free forever, [Comet](https://bit.ly/yolov8-readme-comet) lets you save YOLOv8 models, resume training, and interactively visualize and debug predictions | Run YOLOv8 inference up to 6x faster with [Neural Magic DeepSparse](https://bit.ly/yolov5-neuralmagic) |
 
 ## <div align="center">Ultralytics HUB</div>
 
-[Ultralytics HUB](https://bit.ly/ultralytics_hub) is our ⭐ **NEW** no-code solution to visualize datasets, train YOLOv8
-🚀 models, and deploy to the real world in a seamless experience. Get started for **Free** now! Also run YOLOv8 models on
-your iOS or Android device by downloading the [Ultralytics App](https://ultralytics.com/app_install)!
+Experience seamless AI with [Ultralytics HUB](https://bit.ly/ultralytics_hub) ⭐, the all-in-one solution for data visualization, YOLOv5 and YOLOv8 🚀 model training and deployment, without any coding. Transform images into actionable insights and bring your AI visions to life with ease using our cutting-edge platform and user-friendly [Ultralytics App](https://ultralytics.com/app_install). Start your journey for **Free** now!
 
-<a align="center" href="https://bit.ly/ultralytics_hub" target="_blank">
+<a href="https://bit.ly/ultralytics_hub" target="_blank">
 <img width="100%" src="https://github.com/ultralytics/assets/raw/main/im/ultralytics-hub.png"></a>
 
 ## <div align="center">Contribute</div>
 
-We love your input! YOLOv5 and YOLOv8 would not be possible without help from our community. Please see
-our [Contributing Guide](CONTRIBUTING.md) to get started, and fill out
-our [Survey](https://ultralytics.com/survey?utm_source=github&utm_medium=social&utm_campaign=Survey) to send us feedback
-on your experience. Thank you 🙏 to all our contributors!
+We love your input! YOLOv5 and YOLOv8 would not be possible without help from our community. Please see our [Contributing Guide](https://docs.ultralytics.com/help/contributing) to get started, and fill out our [Survey](https://ultralytics.com/survey?utm_source=github&utm_medium=social&utm_campaign=Survey) to send us feedback on your experience. Thank you 🙏 to all our contributors!
 
 <!-- SVG image from https://opencollective.com/ultralytics/contributors.svg?width=990 -->
 
-<a href="https://github.com/ultralytics/ultralytics/graphs/contributors"><img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/image-contributors-1280.png"/></a>
+<a href="https://github.com/ultralytics/yolov5/graphs/contributors">
+<img width="100%" src="https://github.com/ultralytics/assets/raw/main/im/image-contributors.png"></a>
 
 ## <div align="center">License</div>
 
 YOLOv8 is available under two different licenses:
 
-- **GPL-3.0 License**: See [LICENSE](https://github.com/ultralytics/ultralytics/blob/main/LICENSE) file for details.
-- **Enterprise License**: Provides greater flexibility for commercial product development without the open-source
-  requirements of GPL-3.0. Typical use cases are embedding Ultralytics software and AI models in commercial products and
-  applications. Request an Enterprise License at [Ultralytics Licensing](https://ultralytics.com/license).
+- **AGPL-3.0 License**: See [LICENSE](https://github.com/ultralytics/ultralytics/blob/main/LICENSE) file for details.
+- **Enterprise License**: Provides greater flexibility for commercial product development without the open-source requirements of AGPL-3.0. Typical use cases are embedding Ultralytics software and AI models in commercial products and applications. Request an Enterprise License at [Ultralytics Licensing](https://ultralytics.com/license).
 
 ## <div align="center">Contact</div>
 
-For YOLOv8 bugs and feature requests please visit [GitHub Issues](https://github.com/ultralytics/ultralytics/issues).
-For professional support please [Contact Us](https://ultralytics.com/contact).
+For YOLOv8 bug reports and feature requests please visit [GitHub Issues](https://github.com/ultralytics/ultralytics/issues), and join our [Discord](https://discord.gg/n6cFeSPZdD) community for questions and discussions!
 
 <br>
 <div align="center">
   <a href="https://github.com/ultralytics" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
   <a href="https://www.linkedin.com/company/ultralytics" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
   <a href="https://twitter.com/ultralytics" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
-  <a href="https://www.producthunt.com/@glenn_jocher" style="text-decoration:none;">
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-producthunt.png" width="3%" alt="" /></a>
-  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
   <a href="https://youtube.com/ultralytics" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
-  <a href="https://www.facebook.com/ultralytics" style="text-decoration:none;">
-    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-facebook.png" width="3%" alt="" /></a>
+  <a href="https://www.tiktok.com/@ultralytics" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-tiktok.png" width="3%" alt="" /></a>
   <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
   <a href="https://www.instagram.com/ultralytics/" style="text-decoration:none;">
     <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="3%" alt="" /></a>
+  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
+  <a href="https://discord.gg/n6cFeSPZdD" style="text-decoration:none;">
+    <img src="https://github.com/ultralytics/assets/blob/main/social/logo-social-discord.png" width="3%" alt="" /></a>
 </div>
```

#### html2text {}

```diff
@@ -1,99 +1,85 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.0.9 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.0.90 Summary: Ultralytics
 YOLOv8 Home-page: https://github.com/ultralytics/ultralytics Author:
-Ultralytics Author-email: hello@ultralytics.com License: GPL-3.0 Project-URL:
+Ultralytics Author-email: hello@ultralytics.com License: AGPL-3.0 Project-URL:
 Bug Reports, https://github.com/ultralytics/ultralytics/issues Project-URL:
 Funding, https://ultralytics.com Project-URL: Source, https://github.com/
 ultralytics/ultralytics Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Science/
-Research Classifier: License :: OSI Approved :: GNU General Public License v3
-(GPLv3) Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Topic :: Software Development
+Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: GNU Affero General
+Public License v3 or later (AGPLv3+) Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Scientific/
 Engineering :: Image Recognition Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS Classifier: Operating System :: Microsoft
-:: Windows Requires-Python: >=3.7,<=3.11 Description-Content-Type: text/
-markdown Provides-Extra: dev License-File: LICENSE
+:: Windows Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: export License-File: LICENSE
    [https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/banner-
                                   yolov8.png]
             [English](README.md) | [ç®ä½ä¸­æ](README.zh-CN.md)
               [Ultralytics_CI] [YOLOv8_Citation] [Docker_Pulls]
               [Run_on_Gradient] [Open_In_Colab] [Open_In_Kaggle]
 
-[Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics), developed by
- [Ultralytics](https://ultralytics.com), is a cutting-edge, state-of-the-art
-    (SOTA) model that builds upon the success of previous YOLO versions and
-   introduces new features and improvements to further boost performance and
- flexibility. YOLOv8 is designed to be fast, accurate, and easy to use, making
-it an excellent choice for a wide range of object detection, image segmentation
-    and image classification tasks. To request an Enterprise License please
-complete the form at [Ultralytics Licensing](https://ultralytics.com/license).
-    [https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/yolo-
-                             comparison-plots.png]
+[Ultralytics](https://ultralytics.com) [YOLOv8](https://github.com/ultralytics/
+ultralytics) is a cutting-edge, state-of-the-art (SOTA) model that builds upon
+     the success of previous YOLO versions and introduces new features and
+ improvements to further boost performance and flexibility. YOLOv8 is designed
+to be fast, accurate, and easy to use, making it an excellent choice for a wide
+     range of object detection and tracking, instance segmentation, image
+classification and pose estimation tasks. We hope that the resources here will
+help you get the most out of YOLOv8. Please browse the YOLOv8 Docs for details,
+   raise an issue on GitHub for support, and join our Discord community for
+questions and discussions! To request an Enterprise License please complete the
+  form at [Ultralytics Licensing](https://ultralytics.com/license). [https://
+   raw.githubusercontent.com/ultralytics/assets/main/yolov8/yolo-comparison-
+                                  plots.png]
 
 ##
-                           Ultralytics Live Session
-[Ultralytics Live Session 3](https://youtu.be/IPcpYO5ITa8) â¨ is here! Join us
- on January 24th at 18 CET as we dive into the latest advancements in YOLOv8,
-and demonstrate how to use this cutting-edge, SOTA model to improve your object
-   detection, instance segmentation, and image classification projects. See
- firsthand how YOLOv8's speed, accuracy, and ease of use make it a top choice
-  for professionals and researchers alike. In addition to learning about the
-  exciting new features and improvements of Ultralytics YOLOv8, you will also
-  have the opportunity to ask questions and interact with our team during the
-live Q&A session. We encourage you to come prepared with any questions you may
-have. To join the webinar, visit our YouTube [Channel](https://www.youtube.com/
-     @Ultralytics/streams) and turn on your notifications! [https://user-
-   images.githubusercontent.com/107626595/212887899-e94b006c-5192-40fa-8b24-
-                               7b5428e065e8.png]
-##
                                  Documentation
 See below for a quickstart installation and usage example, and see the [YOLOv8
 Docs](https://docs.ultralytics.com) for full documentation on training,
 validation, prediction and deployment.  Install Pip install the ultralytics
-package including all [requirements.txt](https://github.com/ultralytics/
-ultralytics/blob/main/requirements.txt) in a [**3.10>=Python>=3.7**](https://
-www.python.org/) environment, including [**PyTorch>=1.7**](https://pytorch.org/
-get-started/locally/). ```bash pip install ultralytics ```   Usage #### CLI
-YOLOv8 may be used directly in the Command Line Interface (CLI) with a `yolo`
-command: ```bash yolo predict model=yolov8n.pt source="https://ultralytics.com/
-images/bus.jpg" ``` `yolo` can be used for a variety of tasks and modes and
-accepts additional arguments, i.e. `imgsz=640`. See the YOLOv8 [CLI Docs]
-(https://docs.ultralytics.com/cli) for examples. #### Python YOLOv8 may also be
+package including all [requirements](https://github.com/ultralytics/
+ultralytics/blob/main/requirements.txt) in a [**Python>=3.7**](https://
+www.python.org/) environment with [**PyTorch>=1.7**](https://pytorch.org/get-
+started/locally/). ```bash pip install ultralytics ```   Usage #### CLI YOLOv8
+may be used directly in the Command Line Interface (CLI) with a `yolo` command:
+```bash yolo predict model=yolov8n.pt source='https://ultralytics.com/images/
+bus.jpg' ``` `yolo` can be used for a variety of tasks and modes and accepts
+additional arguments, i.e. `imgsz=640`. See the YOLOv8 [CLI Docs](https://
+docs.ultralytics.com/usage/cli) for examples. #### Python YOLOv8 may also be
 used directly in a Python environment, and accepts the same [arguments](https:/
-/docs.ultralytics.com/config/) as in the CLI example above: ```python from
+/docs.ultralytics.com/usage/cfg/) as in the CLI example above: ```python from
 ultralytics import YOLO # Load a model model = YOLO("yolov8n.yaml") # build a
 new model from scratch model = YOLO("yolov8n.pt") # load a pretrained model
-(recommended for training) # Use the model results = model.train
-(data="coco128.yaml", epochs=3) # train the model results = model.val() #
-evaluate model performance on the validation set results = model("https://
-ultralytics.com/images/bus.jpg") # predict on an image success = model.export
-(format="onnx") # export the model to ONNX format ``` [Models](https://
-github.com/ultralytics/ultralytics/tree/main/ultralytics/models) download
-automatically from the latest Ultralytics [release](https://github.com/
-ultralytics/assets/releases). See YOLOv8 [Python Docs](https://
-docs.ultralytics.com/python) for more examples. #### Known Issues / TODOs We
-are still working on several parts of YOLOv8! We aim to have these completed
-soon to bring the YOLOv8 feature set up to par with YOLOv5, including export
-and inference to all the same formats. We are also writing a YOLOv8 paper which
-we will submit to [arxiv.org](https://arxiv.org) once complete. - [ ]
-TensorFlow exports - [ ] DDP resume - [ ] [arxiv.org](https://arxiv.org) paper
-##
+(recommended for training) # Use the model model.train(data="coco128.yaml",
+epochs=3) # train the model metrics = model.val() # evaluate model performance
+on the validation set results = model("https://ultralytics.com/images/bus.jpg")
+# predict on an image success = model.export(format="onnx") # export the model
+to ONNX format ``` [Models](https://github.com/ultralytics/ultralytics/tree/
+main/ultralytics/models) download automatically from the latest Ultralytics
+[release](https://github.com/ultralytics/assets/releases). See YOLOv8 [Python
+Docs](https://docs.ultralytics.com/usage/python) for more examples.  ##
                                     Models
-All YOLOv8 pretrained models are available here. Detection and Segmentation
-models are pretrained on the COCO dataset, while Classification models are
-pretrained on the ImageNet dataset. [Models](https://github.com/ultralytics/
-ultralytics/tree/main/ultralytics/models) download automatically from the
-latest Ultralytics [release](https://github.com/ultralytics/assets/releases) on
-first use. Detection See [Detection Docs](https://docs.ultralytics.com/tasks/
-detection/) for usage examples with these models. | Model | size
+All YOLOv8 pretrained models are available here. Detect, Segment and Pose
+models are pretrained on the [COCO](https://github.com/ultralytics/ultralytics/
+blob/main/ultralytics/datasets/coco.yaml) dataset, while Classify models are
+pretrained on the [ImageNet](https://github.com/ultralytics/ultralytics/blob/
+main/ultralytics/datasets/ImageNet.yaml) dataset. [Models](https://github.com/
+ultralytics/ultralytics/tree/main/ultralytics/models) download automatically
+from the latest Ultralytics [release](https://github.com/ultralytics/assets/
+releases) on first use. Detection See [Detection Docs](https://
+docs.ultralytics.com/tasks/detect/) for usage examples with these models. |
+Model | size
 (pixels) | mAPval
 50-95 | Speed
 CPU ONNX
 (ms) | Speed
 A100 TensorRT
 (ms) | params
 (M) | FLOPs
@@ -110,119 +96,151 @@
 | 165.2 | | [YOLOv8x](https://github.com/ultralytics/assets/releases/download/
 v0.0.0/yolov8x.pt) | 640 | 53.9 | 479.1 | 3.53 | 68.2 | 257.8 | - **mAPval**
 values are for single-model single-scale on [COCO val2017](http://
 cocodataset.org) dataset.
 Reproduce by `yolo val detect data=coco.yaml device=0` - **Speed** averaged
 over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/
 instance-types/p4/) instance.
-Reproduce by `yolo val detect data=coco128.yaml batch=1 device=0/cpu`
+Reproduce by `yolo val detect data=coco128.yaml batch=1 device=0|cpu`
 Segmentation See [Segmentation Docs](https://docs.ultralytics.com/tasks/
-segmentation/) for usage examples with these models. | Model | size
+segment/) for usage examples with these models. | Model | size
 (pixels) | mAPbox
 50-95 | mAPmask
 50-95 | Speed
 CPU ONNX
 (ms) | Speed
 A100 TensorRT
 (ms) | params
 (M) | FLOPs
 (B) | | -----------------------------------------------------------------------
------------------ | --------------------- | -------------------- | ------------
---------- | ------------------------------ | ----------------------------------
-- | ------------------ | ----------------- | | [YOLOv8n](https://github.com/
-ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640 | 36.7 | 30.5
-| 96.1 | 1.21 | 3.4 | 12.6 | | [YOLOv8s](https://github.com/ultralytics/assets/
-releases/download/v0.0.0/yolov8s-seg.pt) | 640 | 44.6 | 36.8 | 155.7 | 1.47 |
-11.8 | 42.6 | | [YOLOv8m](https://github.com/ultralytics/assets/releases/
-download/v0.0.0/yolov8m-seg.pt) | 640 | 49.9 | 40.8 | 317.0 | 2.18 | 27.3 |
-110.2 | | [YOLOv8l](https://github.com/ultralytics/assets/releases/download/
-v0.0.0/yolov8l-seg.pt) | 640 | 52.3 | 42.6 | 572.4 | 2.79 | 46.0 | 220.5 | |
-[YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/
-yolov8x-seg.pt) | 640 | 53.4 | 43.4 | 712.1 | 4.02 | 71.8 | 344.1 | -
-**mAPval** values are for single-model single-scale on [COCO val2017](http://
-cocodataset.org) dataset.
+--------------------- | --------------------- | -------------------- | --------
+------------- | ------------------------------ | ------------------------------
+----- | ------------------ | ----------------- | | [YOLOv8n-seg](https://
+github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-seg.pt) | 640 |
+36.7 | 30.5 | 96.1 | 1.21 | 3.4 | 12.6 | | [YOLOv8s-seg](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8s-seg.pt) | 640 | 44.6 | 36.8
+| 155.7 | 1.47 | 11.8 | 42.6 | | [YOLOv8m-seg](https://github.com/ultralytics/
+assets/releases/download/v0.0.0/yolov8m-seg.pt) | 640 | 49.9 | 40.8 | 317.0 |
+2.18 | 27.3 | 110.2 | | [YOLOv8l-seg](https://github.com/ultralytics/assets/
+releases/download/v0.0.0/yolov8l-seg.pt) | 640 | 52.3 | 42.6 | 572.4 | 2.79 |
+46.0 | 220.5 | | [YOLOv8x-seg](https://github.com/ultralytics/assets/releases/
+download/v0.0.0/yolov8x-seg.pt) | 640 | 53.4 | 43.4 | 712.1 | 4.02 | 71.8 |
+344.1 | - **mAPval** values are for single-model single-scale on [COCO val2017]
+(http://cocodataset.org) dataset.
 Reproduce by `yolo val segment data=coco.yaml device=0` - **Speed** averaged
 over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/
 instance-types/p4/) instance.
-Reproduce by `yolo val segment data=coco128-seg.yaml batch=1 device=0/cpu`
+Reproduce by `yolo val segment data=coco128-seg.yaml batch=1 device=0|cpu`
 Classification See [Classification Docs](https://docs.ultralytics.com/tasks/
-classification/) for usage examples with these models. | Model | size
+classify/) for usage examples with these models. | Model | size
 (pixels) | acc
 top1 | acc
 top5 | Speed
 CPU ONNX
 (ms) | Speed
 A100 TensorRT
 (ms) | params
 (M) | FLOPs
 (B) at 640 | | ----------------------------------------------------------------
------------------------- | --------------------- | ---------------- | ---------
-------- | ------------------------------ | ----------------------------------
-- | ------------------ | ------------------------ | | [YOLOv8n](https://
+---------------------------- | --------------------- | ---------------- | -----
+----------- | ------------------------------ | --------------------------------
+--- | ------------------ | ------------------------ | | [YOLOv8n-cls](https://
 github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-cls.pt) | 224 |
-66.6 | 87.0 | 12.9 | 0.31 | 2.7 | 4.3 | | [YOLOv8s](https://github.com/
+66.6 | 87.0 | 12.9 | 0.31 | 2.7 | 4.3 | | [YOLOv8s-cls](https://github.com/
 ultralytics/assets/releases/download/v0.0.0/yolov8s-cls.pt) | 224 | 72.3 | 91.1
-| 23.4 | 0.35 | 6.4 | 13.5 | | [YOLOv8m](https://github.com/ultralytics/assets/
-releases/download/v0.0.0/yolov8m-cls.pt) | 224 | 76.4 | 93.2 | 85.4 | 0.62 |
-17.0 | 42.7 | | [YOLOv8l](https://github.com/ultralytics/assets/releases/
-download/v0.0.0/yolov8l-cls.pt) | 224 | 78.0 | 94.1 | 163.0 | 0.87 | 37.5 |
-99.7 | | [YOLOv8x](https://github.com/ultralytics/assets/releases/download/
-v0.0.0/yolov8x-cls.pt) | 224 | 78.4 | 94.3 | 232.0 | 1.01 | 57.4 | 154.8 | -
-**acc** values are model accuracies on the [ImageNet](https://www.image-
-net.org/) dataset validation set.
+| 23.4 | 0.35 | 6.4 | 13.5 | | [YOLOv8m-cls](https://github.com/ultralytics/
+assets/releases/download/v0.0.0/yolov8m-cls.pt) | 224 | 76.4 | 93.2 | 85.4 |
+0.62 | 17.0 | 42.7 | | [YOLOv8l-cls](https://github.com/ultralytics/assets/
+releases/download/v0.0.0/yolov8l-cls.pt) | 224 | 78.0 | 94.1 | 163.0 | 0.87 |
+37.5 | 99.7 | | [YOLOv8x-cls](https://github.com/ultralytics/assets/releases/
+download/v0.0.0/yolov8x-cls.pt) | 224 | 78.4 | 94.3 | 232.0 | 1.01 | 57.4 |
+154.8 | - **acc** values are model accuracies on the [ImageNet](https://
+www.image-net.org/) dataset validation set.
 Reproduce by `yolo val classify data=path/to/ImageNet device=0` - **Speed**
 averaged over ImageNet val images using an [Amazon EC2 P4d](https://
 aws.amazon.com/ec2/instance-types/p4/) instance.
-Reproduce by `yolo val classify data=path/to/ImageNet batch=1 device=0/cpu`  ##
+Reproduce by `yolo val classify data=path/to/ImageNet batch=1 device=0|cpu`
+Pose See [Pose Docs](https://docs.ultralytics.com/tasks/pose) for usage
+examples with these models. | Model | size
+(pixels) | mAPpose
+50-95 | mAPpose
+50 | Speed
+CPU ONNX
+(ms) | Speed
+A100 TensorRT
+(ms) | params
+(M) | FLOPs
+(B) | | -----------------------------------------------------------------------
+----------------------------- | --------------------- | --------------------- |
+------------------ | ------------------------------ | -------------------------
+---------- | ------------------ | ----------------- | | [YOLOv8n-pose](https://
+github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n-pose.pt) | 640 |
+50.4 | 80.1 | 131.8 | 1.18 | 3.3 | 9.2 | | [YOLOv8s-pose](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8s-pose.pt) | 640 | 60.0 |
+86.2 | 233.2 | 1.42 | 11.6 | 30.2 | | [YOLOv8m-pose](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8m-pose.pt) | 640 | 65.0 |
+88.8 | 456.3 | 2.00 | 26.4 | 81.0 | | [YOLOv8l-pose](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8l-pose.pt) | 640 | 67.6 |
+90.0 | 784.5 | 2.59 | 44.4 | 168.6 | | [YOLOv8x-pose](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8x-pose.pt) | 640 | 69.2 |
+90.2 | 1607.1 | 3.73 | 69.4 | 263.2 | | [YOLOv8x-pose-p6](https://github.com/
+ultralytics/assets/releases/download/v0.0.0/yolov8x-pose-p6.pt) | 1280 | 71.6 |
+91.2 | 4088.7 | 10.04 | 99.1 | 1066.4 | - **mAPval** values are for single-
+model single-scale on [COCO Keypoints val2017](http://cocodataset.org) dataset.
+
+Reproduce by `yolo val pose data=coco-pose.yaml device=0` - **Speed** averaged
+over COCO val images using an [Amazon EC2 P4d](https://aws.amazon.com/ec2/
+instance-types/p4/) instance.
+Reproduce by `yolo val pose data=coco8-pose.yaml batch=1 device=0|cpu`  ##
                                  Integrations
 
 [https://github.com/ultralytics/assets/raw/main/yolov8/banner-integrations.png]
 
 
-      [https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-
- roboflow.png]  [https://github.com/ultralytics/yolov5/releases/download/v1.0/
- logo-clearml.png]  [https://github.com/ultralytics/yolov5/releases/download/
-v1.0/logo-comet.png]  [https://github.com/ultralytics/yolov5/releases/download/
-                          v1.0/logo-neuralmagic.png]
+ [https://github.com/ultralytics/assets/raw/main/partners/logo-roboflow.png]
+ [https://github.com/ultralytics/assets/raw/main/partners/logo-clearml.png]
+  [https://github.com/ultralytics/assets/raw/main/partners/logo-comet.png]
+[https://github.com/ultralytics/assets/raw/main/partners/logo-neuralmagic.png]
 | Roboflow | ClearML â­ NEW | Comet â­ NEW | Neural Magic â­ NEW | | :------
 -------------------------------------------------------------------------------
 -------------------------------------: | :-------------------------------------
 -------------------------------------------------------------------------------
 -------------: | :-------------------------------------------------------------
 -------------------------------------------------------------------------------
-------------: | :--------------------------------------------------------------
---------------------------------------: | | Label and export your custom
+-----------: | :---------------------------------------------------------------
+-------------------------------------: | | Label and export your custom
 datasets directly to YOLOv8 for training with [Roboflow](https://roboflow.com/
 ?ref=ultralytics) | Automatically track, visualize and even remotely train
 YOLOv8 using [ClearML](https://cutt.ly/yolov5-readme-clearml) (open-source!) |
-Free forever, [Comet](https://bit.ly/yolov5-readme-comet2) lets you save YOLOv8
+Free forever, [Comet](https://bit.ly/yolov8-readme-comet) lets you save YOLOv8
 models, resume training, and interactively visualize and debug predictions |
 Run YOLOv8 inference up to 6x faster with [Neural Magic DeepSparse](https://
 bit.ly/yolov5-neuralmagic) | ##
                                 Ultralytics HUB
-[Ultralytics HUB](https://bit.ly/ultralytics_hub) is our â­ **NEW** no-code
-solution to visualize datasets, train YOLOv8 ð models, and deploy to the
-real world in a seamless experience. Get started for **Free** now! Also run
-YOLOv8 models on your iOS or Android device by downloading the [Ultralytics
-App](https://ultralytics.com/app_install)! [https://github.com/ultralytics/
-assets/raw/main/im/ultralytics-hub.png] ##
+Experience seamless AI with [Ultralytics HUB](https://bit.ly/ultralytics_hub)
+â­, the all-in-one solution for data visualization, YOLOv5 and YOLOv8 ð
+model training and deployment, without any coding. Transform images into
+actionable insights and bring your AI visions to life with ease using our
+cutting-edge platform and user-friendly [Ultralytics App](https://
+ultralytics.com/app_install). Start your journey for **Free** now! [https://
+github.com/ultralytics/assets/raw/main/im/ultralytics-hub.png] ##
                                   Contribute
 We love your input! YOLOv5 and YOLOv8 would not be possible without help from
-our community. Please see our [Contributing Guide](CONTRIBUTING.md) to get
-started, and fill out our [Survey](https://ultralytics.com/
+our community. Please see our [Contributing Guide](https://
+docs.ultralytics.com/help/contributing) to get started, and fill out our
+[Survey](https://ultralytics.com/
 survey?utm_source=github&utm_medium=social&utm_campaign=Survey) to send us
 feedback on your experience. Thank you ð to all our contributors!  [https://
-github.com/ultralytics/yolov5/releases/download/v1.0/image-contributors-
-1280.png] ##
+github.com/ultralytics/assets/raw/main/im/image-contributors.png] ##
                                     License
-YOLOv8 is available under two different licenses: - **GPL-3.0 License**: See
+YOLOv8 is available under two different licenses: - **AGPL-3.0 License**: See
 [LICENSE](https://github.com/ultralytics/ultralytics/blob/main/LICENSE) file
 for details. - **Enterprise License**: Provides greater flexibility for
-commercial product development without the open-source requirements of GPL-3.0.
-Typical use cases are embedding Ultralytics software and AI models in
+commercial product development without the open-source requirements of AGPL-
+3.0. Typical use cases are embedding Ultralytics software and AI models in
 commercial products and applications. Request an Enterprise License at
 [Ultralytics Licensing](https://ultralytics.com/license). ##
                                     Contact
-For YOLOv8 bugs and feature requests please visit [GitHub Issues](https://
-github.com/ultralytics/ultralytics/issues). For professional support please
-[Contact Us](https://ultralytics.com/contact).
+For YOLOv8 bug reports and feature requests please visit [GitHub Issues](https:
+//github.com/ultralytics/ultralytics/issues), and join our [Discord](https://
+discord.gg/n6cFeSPZdD) community for questions and discussions!
```

### Comparing `ultralytics-8.0.9/ultralytics.egg-info/SOURCES.txt` & `ultralytics-8.0.90/ultralytics.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -2,115 +2,146 @@
 LICENSE
 MANIFEST.in
 README.md
 README.zh-CN.md
 requirements.txt
 setup.cfg
 setup.py
+tests/test_cli.py
+tests/test_engine.py
+tests/test_python.py
 ultralytics/__init__.py
 ultralytics.egg-info/PKG-INFO
 ultralytics.egg-info/SOURCES.txt
 ultralytics.egg-info/dependency_links.txt
 ultralytics.egg-info/entry_points.txt
 ultralytics.egg-info/requires.txt
 ultralytics.egg-info/top_level.txt
+ultralytics/assets/bus.jpg
+ultralytics/assets/zidane.jpg
+ultralytics/datasets/Argoverse.yaml
+ultralytics/datasets/GlobalWheat2020.yaml
+ultralytics/datasets/ImageNet.yaml
+ultralytics/datasets/Objects365.yaml
+ultralytics/datasets/SKU-110K.yaml
+ultralytics/datasets/VOC.yaml
+ultralytics/datasets/VisDrone.yaml
+ultralytics/datasets/coco-pose.yaml
+ultralytics/datasets/coco.yaml
+ultralytics/datasets/coco128-seg.yaml
+ultralytics/datasets/coco128.yaml
+ultralytics/datasets/coco8-pose.yaml
+ultralytics/datasets/coco8-seg.yaml
+ultralytics/datasets/coco8.yaml
+ultralytics/datasets/xView.yaml
 ultralytics/hub/__init__.py
 ultralytics/hub/auth.py
 ultralytics/hub/session.py
 ultralytics/hub/utils.py
 ultralytics/models/v3/yolov3-spp.yaml
 ultralytics/models/v3/yolov3-tiny.yaml
 ultralytics/models/v3/yolov3.yaml
-ultralytics/models/v5/yolov5l.yaml
-ultralytics/models/v5/yolov5m.yaml
-ultralytics/models/v5/yolov5n.yaml
-ultralytics/models/v5/yolov5s.yaml
-ultralytics/models/v5/yolov5x.yaml
-ultralytics/models/v8/yolov8l.yaml
-ultralytics/models/v8/yolov8m.yaml
-ultralytics/models/v8/yolov8n.yaml
-ultralytics/models/v8/yolov8s.yaml
-ultralytics/models/v8/yolov8x.yaml
-ultralytics/models/v8/yolov8x6.yaml
-ultralytics/models/v8/cls/yolov8l-cls.yaml
-ultralytics/models/v8/cls/yolov8m-cls.yaml
-ultralytics/models/v8/cls/yolov8n-cls.yaml
-ultralytics/models/v8/cls/yolov8s-cls.yaml
-ultralytics/models/v8/cls/yolov8x-cls.yaml
-ultralytics/models/v8/seg/yolov8l-seg.yaml
-ultralytics/models/v8/seg/yolov8m-seg.yaml
-ultralytics/models/v8/seg/yolov8n-seg.yaml
-ultralytics/models/v8/seg/yolov8s-seg.yaml
-ultralytics/models/v8/seg/yolov8x-seg.yaml
+ultralytics/models/v5/yolov5-p6.yaml
+ultralytics/models/v5/yolov5.yaml
+ultralytics/models/v8/yolov8-cls.yaml
+ultralytics/models/v8/yolov8-p2.yaml
+ultralytics/models/v8/yolov8-p6.yaml
+ultralytics/models/v8/yolov8-pose-p6.yaml
+ultralytics/models/v8/yolov8-pose.yaml
+ultralytics/models/v8/yolov8-seg.yaml
+ultralytics/models/v8/yolov8.yaml
 ultralytics/nn/__init__.py
 ultralytics/nn/autobackend.py
 ultralytics/nn/autoshape.py
 ultralytics/nn/modules.py
 ultralytics/nn/tasks.py
+ultralytics/tracker/__init__.py
+ultralytics/tracker/track.py
+ultralytics/tracker/cfg/botsort.yaml
+ultralytics/tracker/cfg/bytetrack.yaml
+ultralytics/tracker/trackers/__init__.py
+ultralytics/tracker/trackers/basetrack.py
+ultralytics/tracker/trackers/bot_sort.py
+ultralytics/tracker/trackers/byte_tracker.py
+ultralytics/tracker/utils/__init__.py
+ultralytics/tracker/utils/gmc.py
+ultralytics/tracker/utils/kalman_filter.py
+ultralytics/tracker/utils/matching.py
+ultralytics/vit/__init__.py
+ultralytics/vit/sam/__init__.py
+ultralytics/vit/sam/amg.py
+ultralytics/vit/sam/autosize.py
+ultralytics/vit/sam/build.py
+ultralytics/vit/sam/model.py
+ultralytics/vit/sam/predict.py
+ultralytics/vit/sam/modules/__init__.py
+ultralytics/vit/sam/modules/decoders.py
+ultralytics/vit/sam/modules/encoders.py
+ultralytics/vit/sam/modules/mask_generator.py
+ultralytics/vit/sam/modules/prompt_predictor.py
+ultralytics/vit/sam/modules/sam.py
+ultralytics/vit/sam/modules/transformer.py
 ultralytics/yolo/__init__.py
-ultralytics/yolo/cli.py
-ultralytics/yolo/configs/__init__.py
-ultralytics/yolo/configs/default.yaml
-ultralytics/yolo/configs/hydra_patch.py
+ultralytics/yolo/cfg/__init__.py
+ultralytics/yolo/cfg/default.yaml
 ultralytics/yolo/data/__init__.py
+ultralytics/yolo/data/annotator.py
 ultralytics/yolo/data/augment.py
 ultralytics/yolo/data/base.py
 ultralytics/yolo/data/build.py
 ultralytics/yolo/data/dataset.py
 ultralytics/yolo/data/dataset_wrappers.py
 ultralytics/yolo/data/utils.py
 ultralytics/yolo/data/dataloaders/__init__.py
 ultralytics/yolo/data/dataloaders/stream_loaders.py
 ultralytics/yolo/data/dataloaders/v5augmentations.py
 ultralytics/yolo/data/dataloaders/v5loader.py
-ultralytics/yolo/data/datasets/Argoverse.yaml
-ultralytics/yolo/data/datasets/GlobalWheat2020.yaml
-ultralytics/yolo/data/datasets/ImageNet.yaml
-ultralytics/yolo/data/datasets/Objects365.yaml
-ultralytics/yolo/data/datasets/SKU-110K.yaml
-ultralytics/yolo/data/datasets/VOC.yaml
-ultralytics/yolo/data/datasets/VisDrone.yaml
-ultralytics/yolo/data/datasets/coco.yaml
-ultralytics/yolo/data/datasets/coco128-seg.yaml
-ultralytics/yolo/data/datasets/coco128.yaml
-ultralytics/yolo/data/datasets/coco8-seg.yaml
-ultralytics/yolo/data/datasets/coco8.yaml
-ultralytics/yolo/data/datasets/xView.yaml
 ultralytics/yolo/engine/__init__.py
 ultralytics/yolo/engine/exporter.py
 ultralytics/yolo/engine/model.py
 ultralytics/yolo/engine/predictor.py
 ultralytics/yolo/engine/results.py
 ultralytics/yolo/engine/trainer.py
 ultralytics/yolo/engine/validator.py
 ultralytics/yolo/utils/__init__.py
 ultralytics/yolo/utils/autobatch.py
+ultralytics/yolo/utils/benchmarks.py
 ultralytics/yolo/utils/checks.py
 ultralytics/yolo/utils/dist.py
 ultralytics/yolo/utils/downloads.py
+ultralytics/yolo/utils/errors.py
 ultralytics/yolo/utils/files.py
 ultralytics/yolo/utils/instance.py
 ultralytics/yolo/utils/loss.py
 ultralytics/yolo/utils/metrics.py
 ultralytics/yolo/utils/ops.py
 ultralytics/yolo/utils/plotting.py
 ultralytics/yolo/utils/tal.py
 ultralytics/yolo/utils/torch_utils.py
+ultralytics/yolo/utils/tuner.py
 ultralytics/yolo/utils/callbacks/__init__.py
 ultralytics/yolo/utils/callbacks/base.py
 ultralytics/yolo/utils/callbacks/clearml.py
 ultralytics/yolo/utils/callbacks/comet.py
 ultralytics/yolo/utils/callbacks/hub.py
+ultralytics/yolo/utils/callbacks/mlflow.py
+ultralytics/yolo/utils/callbacks/neptune.py
+ultralytics/yolo/utils/callbacks/raytune.py
 ultralytics/yolo/utils/callbacks/tensorboard.py
+ultralytics/yolo/utils/callbacks/wb.py
 ultralytics/yolo/v8/__init__.py
 ultralytics/yolo/v8/classify/__init__.py
 ultralytics/yolo/v8/classify/predict.py
 ultralytics/yolo/v8/classify/train.py
 ultralytics/yolo/v8/classify/val.py
 ultralytics/yolo/v8/detect/__init__.py
 ultralytics/yolo/v8/detect/predict.py
 ultralytics/yolo/v8/detect/train.py
 ultralytics/yolo/v8/detect/val.py
+ultralytics/yolo/v8/pose/__init__.py
+ultralytics/yolo/v8/pose/predict.py
+ultralytics/yolo/v8/pose/train.py
+ultralytics/yolo/v8/pose/val.py
 ultralytics/yolo/v8/segment/__init__.py
 ultralytics/yolo/v8/segment/predict.py
 ultralytics/yolo/v8/segment/train.py
 ultralytics/yolo/v8/segment/val.py
```


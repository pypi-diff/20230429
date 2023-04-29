# Comparing `tmp/nataili-0.3.3.tar.gz` & `tmp/nataili-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nataili-0.3.3.tar", last modified: Sun Apr  2 17:55:20 2023, max compression
+gzip compressed data, was "nataili-0.3.4.tar", last modified: Sat Apr 29 10:01:22 2023, max compression
```

## Comparing `nataili-0.3.3.tar` & `nataili-0.3.4.tar`

### file list

```diff
@@ -1,769 +1,769 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.599988 nataili-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-02 17:54:57.000000 nataili-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-02 17:54:57.000000 nataili-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    42173 2023-04-02 17:55:20.599988 nataili-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-02 17:54:57.000000 nataili-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.459982 nataili-0.3.3/annotator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.459982 nataili-0.3.3/annotator/canny/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/canny/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.459982 nataili-0.3.3/annotator/hed/
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/hed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.459982 nataili-0.3.3/annotator/midas/
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/midas/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.459982 nataili-0.3.3/annotator/midas/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/midas/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/midas/midas/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/midas/midas/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/midas/midas/dpt_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/midas/midas/midas_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/midas/midas/midas_net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/midas/midas/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/midas/midas/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/midas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.463982 nataili-0.3.3/annotator/mlsd/
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/mlsd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.463982 nataili-0.3.3/annotator/mlsd/models/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/mlsd/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/mlsd/models/mbv2_mlsd_large.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/mlsd/models/mbv2_mlsd_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)    24049 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/mlsd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.463982 nataili-0.3.3/annotator/openpose/
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/openpose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/openpose/body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/openpose/hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/openpose/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/openpose/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.463982 nataili-0.3.3/annotator/uniformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.443982 nataili-0.3.3/annotator/uniformer/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.463982 nataili-0.3.3/annotator/uniformer/configs/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.467982 nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/cityscapes_769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/pascal_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/pascal_context_59.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/pascal_voc12.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.471983 nataili-0.3.3/annotator/uniformer/configs/_base_/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/ann_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/apcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/ccnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/danet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/dmnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/dnl_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/emanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/encnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/fcn_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/fcn_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/fpn_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/fpn_uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/gcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/nonlocal_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/ocrnet_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/ocrnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/pointrend_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/psanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/pspnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/upernet_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/models/upernet_uniformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.471983 nataili-0.3.3/annotator/uniformer/configs/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/schedules/schedule_160k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/schedules/schedule_20k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/schedules/schedule_40k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/configs/_base_/schedules/schedule_80k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.443982 nataili-0.3.3/annotator/uniformer/exp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.475983 nataili-0.3.3/annotator/uniformer/exp/upernet_global_small/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/exp/upernet_global_small/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/exp/upernet_global_small/test_config_g.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/exp/upernet_global_small/test_config_h32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/exp/upernet_global_small/test_config_w32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.475983 nataili-0.3.3/annotator/uniformer/mmcv/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.475983 nataili-0.3.3/annotator/uniformer/mmcv/arraymisc/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/arraymisc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/arraymisc/quantization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.475983 nataili-0.3.3/annotator/uniformer/mmcv/cnn/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/alexnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.479983 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/context_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/conv_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/generalized_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/hsigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/hswish.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/non_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/swish.py
--rw-r--r--   0 runner    (1001) docker     (123)    24639 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.479983 nataili-0.3.3/annotator/uniformer/mmcv/cnn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22104 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/utils/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)    26006 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/utils/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/cnn/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.483983 nataili-0.3.3/annotator/uniformer/mmcv/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/engine/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.483983 nataili-0.3.3/annotator/uniformer/mmcv/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41933 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.483983 nataili-0.3.3/annotator/uniformer/mmcv/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.483983 nataili-0.3.3/annotator/uniformer/mmcv/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/image/colorspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/image/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/image/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/image/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/image/photometric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.495983 nataili-0.3.3/annotator/uniformer/mmcv/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/assign_score_withk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/ball_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/border_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/box_iou_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/carafe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/cc_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/contour_expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/corner_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15603 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/deform_roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/deprecated_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/furthest_point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/fused_bias_leakyrelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/gather_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/group_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/iou3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/knn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/masked_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/merge_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/modulated_deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15175 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/multi_scale_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16237 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/pixel_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/points_in_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/points_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/psa_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/roi_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/roi_align_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/roiaware_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/roipoint_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/saconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/scatter_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/three_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/three_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/tin_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/upfirdn2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/ops/voxelize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.495983 nataili-0.3.3/annotator/uniformer/mmcv/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/parallel/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/parallel/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/parallel/data_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/parallel/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/parallel/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/parallel/distributed_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/parallel/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/parallel/scatter_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/parallel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.499984 nataili-0.3.3/annotator/uniformer/mmcv/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    20846 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    25136 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/epoch_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/fp16_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.503984 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/closure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)    22448 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/iter_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.503984 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/dvclive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/pavi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/wandb.py
--rw-r--r--   0 runner    (1001) docker     (123)    26034 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/lr_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    21296 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/momentum_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    21654 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/sampler_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/sync_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/iter_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/log_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.503984 nataili-0.3.3/annotator/uniformer/mmcv/runner/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11803 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.507984 nataili-0.3.3/annotator/uniformer/mmcv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26263 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/utils/ext_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/utils/parrots_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.507984 nataili-0.3.3/annotator/uniformer/mmcv/video/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/video/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/video/optflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/video/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.511984 nataili-0.3.3/annotator/uniformer/mmcv/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/visualization/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/visualization/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv/visualization/optflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.511984 nataili-0.3.3/annotator/uniformer/mmcv_custom/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv_custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19091 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmcv_custom/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.511984 nataili-0.3.3/annotator/uniformer/mmseg/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.511984 nataili-0.3.3/annotator/uniformer/mmseg/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/apis/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/apis/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/apis/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.511984 nataili-0.3.3/annotator/uniformer/mmseg/core/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.511984 nataili-0.3.3/annotator/uniformer/mmseg/core/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/core/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/core/evaluation/class_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/core/evaluation/eval_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/core/evaluation/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.515984 nataili-0.3.3/annotator/uniformer/mmseg/core/seg/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/core/seg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/core/seg/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.515984 nataili-0.3.3/annotator/uniformer/mmseg/core/seg/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/core/seg/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.515984 nataili-0.3.3/annotator/uniformer/mmseg/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.519985 nataili-0.3.3/annotator/uniformer/mmseg/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/datasets/ade.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/datasets/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/datasets/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/datasets/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/datasets/pascal_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.519985 nataili-0.3.3/annotator/uniformer/mmseg/datasets/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/datasets/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/datasets/pipelines/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/datasets/pipelines/formating.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/datasets/pipelines/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/datasets/pipelines/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)    30993 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/datasets/pipelines/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/datasets/voc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.519985 nataili-0.3.3/annotator/uniformer/mmseg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.523985 nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14436 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    21226 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/resnest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24310 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/resnext.py
--rw-r--r--   0 runner    (1001) docker     (123)    18269 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18476 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18085 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.527985 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/ann_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/apc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/cc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/da_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/dm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/dnl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/ema_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/enc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/fpn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/gc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/lraspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/nl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/ocr_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/point_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/psa_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/psp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/uper_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.527985 nataili-0.3.3/annotator/uniformer/mmseg/models/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/losses/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/losses/lovasz_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.527985 nataili-0.3.3/annotator/uniformer/mmseg/models/necks/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/necks/fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/necks/multilevel_neck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.531985 nataili-0.3.3/annotator/uniformer/mmseg/models/segmentors/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/segmentors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/segmentors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/segmentors/encoder_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.531985 nataili-0.3.3/annotator/uniformer/mmseg/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/utils/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/utils/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/utils/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/utils/res_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/utils/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/utils/self_attention_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/utils/up_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/models/utils/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.531985 nataili-0.3.3/annotator/uniformer/mmseg/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/ops/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/ops/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.531985 nataili-0.3.3/annotator/uniformer/mmseg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/uniformer/mmseg/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-02 17:54:57.000000 nataili-0.3.3/annotator/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.531985 nataili-0.3.3/cldm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/cldm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18762 2023-04-02 17:54:57.000000 nataili-0.3.3/cldm/cldm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-02 17:54:57.000000 nataili-0.3.3/cldm/hack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-02 17:54:57.000000 nataili-0.3.3/cldm/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.535985 nataili-0.3.3/ldm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.535985 nataili-0.3.3/ldm/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/data/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/data/lsun.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/lr_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.535985 nataili-0.3.3/ldm/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17618 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/models/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10948 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/models/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/models/blip_itm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/models/blip_nlvr.py
--rw-r--r--   0 runner    (1001) docker     (123)    16070 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/models/blip_pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/models/blip_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/models/blip_vqa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.539985 nataili-0.3.3/ldm/models/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/models/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/models/diffusion/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/models/diffusion/ddim.py
--rw-r--r--   0 runner    (1001) docker     (123)    71801 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/models/diffusion/ddpm.py
--rw-r--r--   0 runner    (1001) docker     (123)    68674 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/models/diffusion/ddpm_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/models/diffusion/kdiffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/models/diffusion/plms.py
--rw-r--r--   0 runner    (1001) docker     (123)    41754 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/models/med.py
--rw-r--r--   0 runner    (1001) docker     (123)    36706 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/models/nlvr_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/models/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.539985 nataili-0.3.3/ldm/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16123 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.543985 nataili-0.3.3/ldm/modules/diffusionmodules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/diffusionmodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35017 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/diffusionmodules/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    37882 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/diffusionmodules/openaimodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/diffusionmodules/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.543985 nataili-0.3.3/ldm/modules/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/distributions/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/ema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.543985 nataili-0.3.3/ldm/modules/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/encoders/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.543985 nataili-0.3.3/ldm/modules/image_degradation/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/image_degradation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/image_degradation/bsrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    22238 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/image_degradation/bsrgan_light.py
--rw-r--r--   0 runner    (1001) docker     (123)    29026 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/image_degradation/utils_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.543985 nataili-0.3.3/ldm/modules/losses/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/losses/contperceptual.py
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/losses/vqperceptual.py
--rw-r--r--   0 runner    (1001) docker     (123)    20169 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/modules/x_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.543985 nataili-0.3.3/ldm2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.543985 nataili-0.3.3/ldm2/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/data/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.543985 nataili-0.3.3/ldm2/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/models/autoencoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.547986 nataili-0.3.3/ldm2/models/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/models/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17501 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/models/diffusion/ddim.py
--rw-r--r--   0 runner    (1001) docker     (123)    85040 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/models/diffusion/ddpm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.547986 nataili-0.3.3/ldm2/models/diffusion/dpm_solver/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/models/diffusion/dpm_solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66122 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/models/diffusion/dpm_solver/dpm_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/models/diffusion/dpm_solver/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/models/diffusion/plms.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/models/diffusion/sampling_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.547986 nataili-0.3.3/ldm2/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.547986 nataili-0.3.3/ldm2/modules/diffusionmodules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/diffusionmodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34477 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/diffusionmodules/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    30367 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/diffusionmodules/openaimodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/diffusionmodules/upscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/diffusionmodules/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.551986 nataili-0.3.3/ldm2/modules/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/distributions/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/ema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.551986 nataili-0.3.3/ldm2/modules/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/encoders/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.551986 nataili-0.3.3/ldm2/modules/image_degradation/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/image_degradation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25199 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/image_degradation/bsrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    22342 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/image_degradation/bsrgan_light.py
--rw-r--r--   0 runner    (1001) docker     (123)    29024 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/image_degradation/utils_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.551986 nataili-0.3.3/ldm2/modules/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/midas/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.555986 nataili-0.3.3/ldm2/modules/midas/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/midas/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/midas/midas/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/midas/midas/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/midas/midas/dpt_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/midas/midas/midas_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/midas/midas/midas_net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/midas/midas/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/midas/midas/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/modules/midas/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-04-02 17:54:57.000000 nataili-0.3.3/ldm2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.559986 nataili-0.3.3/nataili/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.563986 nataili-0.3.3/nataili/aitemplate/
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/aitemplate/AITemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/aitemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16960 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/aitemplate/ait_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/aitemplate/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)    29299 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/aitemplate/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/aitemplate/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/aitemplate.json
--rw-r--r--   0 runner    (1001) docker     (123)    80572 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/artists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.563986 nataili-0.3.3/nataili/blip/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/blip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/blip/caption.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/blip.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.563986 nataili-0.3.3/nataili/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/cache/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/cldm_v15.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/cldm_v21.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.563986 nataili-0.3.3/nataili/clip/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/clip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/clip/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/clip/coca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/clip/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    11849 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/clip/interrogate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.567986 nataili-0.3.3/nataili/clip/predictor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/clip/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/clip/predictor/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/clip/predictor/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/clip/predictor/prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/clip/predictor/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/clip/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/clip.json
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/codeformer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.567986 nataili-0.3.3/nataili/codeformers/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/codeformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/codeformers/codeformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/diffusers.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.567986 nataili-0.3.3/nataili/esrgan/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/esrgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/esrgan/esrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/esrgan.json
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/flavors.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.567986 nataili-0.3.3/nataili/gfpgan/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/gfpgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/gfpgan/gfpgan.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/gfpgan.json
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/med_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/mediums.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.571987 nataili-0.3.3/nataili/model_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/model_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/model_manager/aitemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)    20516 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/model_manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/model_manager/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/model_manager/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/model_manager/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/model_manager/compvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/model_manager/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/model_manager/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/model_manager/esrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/model_manager/gfpgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/model_manager/new.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/model_manager/safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/model_manager/sdu.py
--rw-r--r--   0 runner    (1001) docker     (123)    18333 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/model_manager/super.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/models.json
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/movements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/pix2pix.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/safety_checker.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.571987 nataili-0.3.3/nataili/sdu/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/sdu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/sdu/sdu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/sdu.json
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/sites.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.571987 nataili-0.3.3/nataili/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/stable_diffusion/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    54183 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/stable_diffusion/compvis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.571987 nataili-0.3.3/nataili/stable_diffusion/diffusers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/stable_diffusion/diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/stable_diffusion/diffusers/depth2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     9968 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/stable_diffusion/diffusers/inpainting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/stable_diffusion/prompt_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)   132857 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)    22260 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/tags.txt
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/techniques.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.571987 nataili-0.3.3/nataili/train/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/train/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.571987 nataili-0.3.3/nataili/train/dataset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.575987 nataili-0.3.3/nataili/train/dataset/EveryDream/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/train/dataset/EveryDream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/train/dataset/EveryDream/aspects.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/train/dataset/EveryDream/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/train/dataset/EveryDream/dl_singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/train/dataset/EveryDream/ed_dl_wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/train/dataset/EveryDream/ed_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/train/dataset/EveryDream/every_dream.py
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/train/dataset/EveryDream/image_train_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/train/dataset/EveryDream/latent_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/train/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.575987 nataili-0.3.3/nataili/train/dreambooth/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/train/dreambooth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/train/dreambooth/dreambooth_lora.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.575987 nataili-0.3.3/nataili/train/lora/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/train/lora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35676 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/train/lora/lora.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.575987 nataili-0.3.3/nataili/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.579987 nataili-0.3.3/nataili/ui/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/ui/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/ui/gradio/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/ui/gradio/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/ui/gradio/coca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/ui/gradio/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/ui/gradio/lora.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.583987 nataili-0.3.3/nataili/util/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.583987 nataili-0.3.3/nataili/util/blip/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/blip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/blip/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    41146 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/blip/med.py
--rw-r--r--   0 runner    (1001) docker     (123)    14469 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/blip/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/check_prompt_length.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.583987 nataili-0.3.3/nataili/util/codeformer/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/codeformer_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    23072 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/face_restoration_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.583987 nataili-0.3.3/nataili/util/codeformer/facelib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.587987 nataili-0.3.3/nataili/util/codeformer/facelib/detection/
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/detection/align_trans.py
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/detection/matlab_cp2tform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.587987 nataili-0.3.3/nataili/util/codeformer/facelib/detection/retinaface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/detection/retinaface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/detection/retinaface/retinaface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/detection/retinaface/retinaface_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/detection/retinaface/retinaface_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.587987 nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/face_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.587987 nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/models/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/models/yolo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.587987 nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.591987 nataili-0.3.3/nataili/util/codeformer/facelib/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/parsing/bisenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/parsing/parsenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/parsing/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.591987 nataili-0.3.3/nataili/util/codeformer/facelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22702 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/utils/face_restoration_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/utils/face_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/facelib/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/init_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/init_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    15214 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/codeformer/vqgan_arch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.591987 nataili-0.3.3/nataili/util/controlnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/controlnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/create_random_tensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/get_next_sequence_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.591987 nataili-0.3.3/nataili/util/gfpgan/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/gfpgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/gfpgan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/image_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/load_learned_embed_in_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/load_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/normalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/process_prompt_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/save_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/seed_to_int.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/util/voodoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/v1-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/v1-inpainting-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/v2-inference-v.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/v2-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/v2-inpainting-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/v2-midas-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-02 17:54:57.000000 nataili-0.3.3/nataili/x4-upscaling.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.559986 nataili-0.3.3/nataili.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42173 2023-04-02 17:55:20.000000 nataili-0.3.3/nataili.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27216 2023-04-02 17:55:20.000000 nataili-0.3.3/nataili.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 17:55:20.000000 nataili-0.3.3/nataili.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-02 17:55:20.000000 nataili-0.3.3/nataili.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-02 17:55:20.000000 nataili-0.3.3/nataili.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-02 17:55:20.000000 nataili-0.3.3/nataili.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-02 17:55:07.000000 nataili-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-02 17:54:57.000000 nataili-0.3.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.599988 nataili-0.3.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/bulk_image_embeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/bulk_image_embeds_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/download_all_stable_diffusion_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/sdu.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_ait.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_all_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_blip.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_clip_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_clip_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_coca.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_codeformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_compvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_compvis_inpainting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_control_voodoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_controlnet_canny.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_controlnet_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_controlnet_hed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_controlnet_hough.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_controlnet_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_controlnet_openpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_controlnet_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_depth2img.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_dreambooth_lora.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_esrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_file_hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_gfpgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_img2img_voodoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_inpainting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_pix2pix.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_pix2pix_voodoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_sd2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_txt2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_txt2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_txt2img_hires_voodoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-02 17:54:57.000000 nataili-0.3.3/scripts/test_txt2img_voodoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-02 17:55:20.599988 nataili-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-02 17:55:07.000000 nataili-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 17:55:20.599988 nataili-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-04-02 17:54:57.000000 nataili-0.3.3/tests/prompt_weights.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.213161 nataili-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-29 10:00:59.000000 nataili-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-29 10:00:59.000000 nataili-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    41929 2023-04-29 10:01:22.213161 nataili-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-29 10:00:59.000000 nataili-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.133162 nataili-0.3.4/annotator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.133162 nataili-0.3.4/annotator/canny/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/canny/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.133162 nataili-0.3.4/annotator/hed/
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/hed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.133162 nataili-0.3.4/annotator/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/midas/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.133162 nataili-0.3.4/annotator/midas/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/midas/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/midas/midas/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/midas/midas/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/midas/midas/dpt_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/midas/midas/midas_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/midas/midas/midas_net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/midas/midas/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/midas/midas/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/midas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.133162 nataili-0.3.4/annotator/mlsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/mlsd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.137162 nataili-0.3.4/annotator/mlsd/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/mlsd/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/mlsd/models/mbv2_mlsd_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/mlsd/models/mbv2_mlsd_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24049 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/mlsd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.137162 nataili-0.3.4/annotator/openpose/
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/openpose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/openpose/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/openpose/hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/openpose/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/openpose/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.137162 nataili-0.3.4/annotator/uniformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.125162 nataili-0.3.4/annotator/uniformer/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.137162 nataili-0.3.4/annotator/uniformer/configs/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.137162 nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/cityscapes_769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/pascal_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/pascal_context_59.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/pascal_voc12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.141162 nataili-0.3.4/annotator/uniformer/configs/_base_/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/ann_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/apcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/ccnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/danet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/dmnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/dnl_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/emanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/encnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/fcn_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/fcn_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/fpn_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/fpn_uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/gcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/nonlocal_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/ocrnet_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/ocrnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/pointrend_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/psanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/pspnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/upernet_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/models/upernet_uniformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.141162 nataili-0.3.4/annotator/uniformer/configs/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/schedules/schedule_160k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/schedules/schedule_20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/schedules/schedule_40k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/configs/_base_/schedules/schedule_80k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.125162 nataili-0.3.4/annotator/uniformer/exp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.141162 nataili-0.3.4/annotator/uniformer/exp/upernet_global_small/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/exp/upernet_global_small/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/exp/upernet_global_small/test_config_g.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/exp/upernet_global_small/test_config_h32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/exp/upernet_global_small/test_config_w32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.141162 nataili-0.3.4/annotator/uniformer/mmcv/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.141162 nataili-0.3.4/annotator/uniformer/mmcv/arraymisc/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/arraymisc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/arraymisc/quantization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.141162 nataili-0.3.4/annotator/uniformer/mmcv/cnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/alexnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.145162 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/context_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/conv_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/generalized_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/hsigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/hswish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/non_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/swish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24639 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.145162 nataili-0.3.4/annotator/uniformer/mmcv/cnn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22104 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/utils/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26006 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/utils/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/cnn/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.145162 nataili-0.3.4/annotator/uniformer/mmcv/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/engine/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.145162 nataili-0.3.4/annotator/uniformer/mmcv/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41933 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.149162 nataili-0.3.4/annotator/uniformer/mmcv/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.149162 nataili-0.3.4/annotator/uniformer/mmcv/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/image/colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/image/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/image/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/image/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/image/photometric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.153162 nataili-0.3.4/annotator/uniformer/mmcv/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/assign_score_withk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/ball_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/border_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/box_iou_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/carafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/cc_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/contour_expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/corner_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15603 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/deform_roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/deprecated_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/furthest_point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/fused_bias_leakyrelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/gather_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/group_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/iou3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/masked_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/merge_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/modulated_deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15175 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/multi_scale_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16237 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/pixel_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/points_in_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/points_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/psa_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/roi_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/roi_align_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/roiaware_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/roipoint_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/saconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/scatter_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/three_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/three_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/tin_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/upfirdn2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/ops/voxelize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.157162 nataili-0.3.4/annotator/uniformer/mmcv/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/parallel/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/parallel/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/parallel/data_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/parallel/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/parallel/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/parallel/distributed_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/parallel/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/parallel/scatter_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/parallel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.157162 nataili-0.3.4/annotator/uniformer/mmcv/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20846 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25136 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/epoch_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/fp16_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.157162 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/closure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22448 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/iter_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.161162 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/dvclive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/pavi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/wandb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26034 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/lr_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21296 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/momentum_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21654 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/sampler_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/sync_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/iter_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/log_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.161162 nataili-0.3.4/annotator/uniformer/mmcv/runner/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11803 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.161162 nataili-0.3.4/annotator/uniformer/mmcv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26263 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/utils/ext_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/utils/parrots_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.161162 nataili-0.3.4/annotator/uniformer/mmcv/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/video/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/video/optflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/video/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.161162 nataili-0.3.4/annotator/uniformer/mmcv/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/visualization/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/visualization/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv/visualization/optflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.165162 nataili-0.3.4/annotator/uniformer/mmcv_custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv_custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19091 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmcv_custom/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.165162 nataili-0.3.4/annotator/uniformer/mmseg/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.165162 nataili-0.3.4/annotator/uniformer/mmseg/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/apis/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/apis/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/apis/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.165162 nataili-0.3.4/annotator/uniformer/mmseg/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.165162 nataili-0.3.4/annotator/uniformer/mmseg/core/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/core/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/core/evaluation/class_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/core/evaluation/eval_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/core/evaluation/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.165162 nataili-0.3.4/annotator/uniformer/mmseg/core/seg/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/core/seg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/core/seg/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.165162 nataili-0.3.4/annotator/uniformer/mmseg/core/seg/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/core/seg/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.165162 nataili-0.3.4/annotator/uniformer/mmseg/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.165162 nataili-0.3.4/annotator/uniformer/mmseg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/datasets/ade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/datasets/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/datasets/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/datasets/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/datasets/pascal_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.169162 nataili-0.3.4/annotator/uniformer/mmseg/datasets/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/datasets/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/datasets/pipelines/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/datasets/pipelines/formating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/datasets/pipelines/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/datasets/pipelines/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30993 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/datasets/pipelines/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/datasets/voc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.169162 nataili-0.3.4/annotator/uniformer/mmseg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.169162 nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14436 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21226 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/resnest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24310 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/resnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18269 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18476 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18085 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.173162 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/ann_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/apc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/cc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/da_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/dm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/dnl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/ema_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/enc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/fpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/gc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/lraspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/nl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/ocr_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/point_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/psa_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/psp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/uper_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.173162 nataili-0.3.4/annotator/uniformer/mmseg/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/losses/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/losses/lovasz_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.173162 nataili-0.3.4/annotator/uniformer/mmseg/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/necks/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/necks/multilevel_neck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.173162 nataili-0.3.4/annotator/uniformer/mmseg/models/segmentors/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/segmentors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/segmentors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/segmentors/encoder_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.173162 nataili-0.3.4/annotator/uniformer/mmseg/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/utils/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/utils/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/utils/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/utils/res_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/utils/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/utils/self_attention_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/utils/up_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/models/utils/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.177162 nataili-0.3.4/annotator/uniformer/mmseg/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/ops/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/ops/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.177162 nataili-0.3.4/annotator/uniformer/mmseg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/uniformer/mmseg/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-29 10:00:59.000000 nataili-0.3.4/annotator/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.177162 nataili-0.3.4/cldm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/cldm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18762 2023-04-29 10:00:59.000000 nataili-0.3.4/cldm/cldm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-29 10:00:59.000000 nataili-0.3.4/cldm/hack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-29 10:00:59.000000 nataili-0.3.4/cldm/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.177162 nataili-0.3.4/ldm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.177162 nataili-0.3.4/ldm/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/data/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/data/lsun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/lr_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.177162 nataili-0.3.4/ldm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17618 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/models/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10948 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/models/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/models/blip_itm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/models/blip_nlvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16070 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/models/blip_pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/models/blip_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/models/blip_vqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.181161 nataili-0.3.4/ldm/models/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/models/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/models/diffusion/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/models/diffusion/ddim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71801 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/models/diffusion/ddpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68674 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/models/diffusion/ddpm_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/models/diffusion/kdiffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/models/diffusion/plms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41754 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/models/med.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36706 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/models/nlvr_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/models/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.181161 nataili-0.3.4/ldm/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16123 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.181161 nataili-0.3.4/ldm/modules/diffusionmodules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/diffusionmodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35017 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/diffusionmodules/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37882 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/diffusionmodules/openaimodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/diffusionmodules/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.181161 nataili-0.3.4/ldm/modules/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/distributions/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/ema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.181161 nataili-0.3.4/ldm/modules/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/encoders/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.181161 nataili-0.3.4/ldm/modules/image_degradation/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/image_degradation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/image_degradation/bsrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22238 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/image_degradation/bsrgan_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29026 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/image_degradation/utils_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.181161 nataili-0.3.4/ldm/modules/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/losses/contperceptual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/losses/vqperceptual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20169 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/modules/x_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.181161 nataili-0.3.4/ldm2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.181161 nataili-0.3.4/ldm2/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/data/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.181161 nataili-0.3.4/ldm2/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/models/autoencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.185161 nataili-0.3.4/ldm2/models/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/models/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17501 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/models/diffusion/ddim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85040 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/models/diffusion/ddpm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.185161 nataili-0.3.4/ldm2/models/diffusion/dpm_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/models/diffusion/dpm_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66122 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/models/diffusion/dpm_solver/dpm_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/models/diffusion/dpm_solver/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/models/diffusion/plms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/models/diffusion/sampling_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.185161 nataili-0.3.4/ldm2/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.185161 nataili-0.3.4/ldm2/modules/diffusionmodules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/diffusionmodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34477 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/diffusionmodules/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30367 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/diffusionmodules/openaimodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/diffusionmodules/upscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/diffusionmodules/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.185161 nataili-0.3.4/ldm2/modules/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/distributions/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/ema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.185161 nataili-0.3.4/ldm2/modules/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/encoders/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.185161 nataili-0.3.4/ldm2/modules/image_degradation/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/image_degradation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25199 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/image_degradation/bsrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22342 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/image_degradation/bsrgan_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29024 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/image_degradation/utils_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.185161 nataili-0.3.4/ldm2/modules/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/midas/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.189161 nataili-0.3.4/ldm2/modules/midas/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/midas/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/midas/midas/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/midas/midas/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/midas/midas/dpt_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/midas/midas/midas_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/midas/midas/midas_net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/midas/midas/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/midas/midas/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/modules/midas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-04-29 10:00:59.000000 nataili-0.3.4/ldm2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.189161 nataili-0.3.4/nataili/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.193161 nataili-0.3.4/nataili/aitemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/aitemplate/AITemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/aitemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16960 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/aitemplate/ait_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/aitemplate/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29299 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/aitemplate/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/aitemplate/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/aitemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)    80572 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/artists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.193161 nataili-0.3.4/nataili/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/blip/caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/blip.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.193161 nataili-0.3.4/nataili/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/cache/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/cldm_v15.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/cldm_v21.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.193161 nataili-0.3.4/nataili/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/clip/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/clip/coca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/clip/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11849 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/clip/interrogate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.193161 nataili-0.3.4/nataili/clip/predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/clip/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/clip/predictor/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/clip/predictor/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/clip/predictor/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/clip/predictor/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/clip/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/clip.json
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/codeformer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.193161 nataili-0.3.4/nataili/codeformers/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/codeformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/codeformers/codeformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/diffusers.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.193161 nataili-0.3.4/nataili/esrgan/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/esrgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/esrgan/esrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/esrgan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/flavors.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.197162 nataili-0.3.4/nataili/gfpgan/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/gfpgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/gfpgan/gfpgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/gfpgan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/med_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/mediums.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.197162 nataili-0.3.4/nataili/model_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/model_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/model_manager/aitemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/model_manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/model_manager/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/model_manager/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/model_manager/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/model_manager/compvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/model_manager/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/model_manager/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/model_manager/esrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/model_manager/gfpgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/model_manager/new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/model_manager/safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/model_manager/sdu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18333 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/model_manager/super.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/models.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/movements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/pix2pix.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/safety_checker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.197162 nataili-0.3.4/nataili/sdu/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/sdu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/sdu/sdu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/sdu.json
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/sites.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.197162 nataili-0.3.4/nataili/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/stable_diffusion/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54183 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/stable_diffusion/compvis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.197162 nataili-0.3.4/nataili/stable_diffusion/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/stable_diffusion/diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/stable_diffusion/diffusers/depth2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9968 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/stable_diffusion/diffusers/inpainting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/stable_diffusion/prompt_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132857 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22260 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/tags.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/techniques.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.197162 nataili-0.3.4/nataili/train/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/train/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.197162 nataili-0.3.4/nataili/train/dataset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.201161 nataili-0.3.4/nataili/train/dataset/EveryDream/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/train/dataset/EveryDream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/train/dataset/EveryDream/aspects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/train/dataset/EveryDream/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/train/dataset/EveryDream/dl_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/train/dataset/EveryDream/ed_dl_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/train/dataset/EveryDream/ed_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/train/dataset/EveryDream/every_dream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/train/dataset/EveryDream/image_train_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/train/dataset/EveryDream/latent_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/train/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.201161 nataili-0.3.4/nataili/train/dreambooth/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/train/dreambooth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/train/dreambooth/dreambooth_lora.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.201161 nataili-0.3.4/nataili/train/lora/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/train/lora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35676 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/train/lora/lora.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.201161 nataili-0.3.4/nataili/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.201161 nataili-0.3.4/nataili/ui/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/ui/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/ui/gradio/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/ui/gradio/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/ui/gradio/coca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/ui/gradio/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/ui/gradio/lora.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.201161 nataili-0.3.4/nataili/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.205161 nataili-0.3.4/nataili/util/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/blip/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41146 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/blip/med.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14469 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/blip/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/check_prompt_length.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.205161 nataili-0.3.4/nataili/util/codeformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/codeformer_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23072 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/face_restoration_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.205161 nataili-0.3.4/nataili/util/codeformer/facelib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.205161 nataili-0.3.4/nataili/util/codeformer/facelib/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/detection/align_trans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/detection/matlab_cp2tform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.205161 nataili-0.3.4/nataili/util/codeformer/facelib/detection/retinaface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/detection/retinaface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/detection/retinaface/retinaface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/detection/retinaface/retinaface_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/detection/retinaface/retinaface_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.205161 nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/face_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.205161 nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/models/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/models/yolo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.209161 nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.209161 nataili-0.3.4/nataili/util/codeformer/facelib/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/parsing/bisenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/parsing/parsenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/parsing/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.209161 nataili-0.3.4/nataili/util/codeformer/facelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22702 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/utils/face_restoration_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/utils/face_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/facelib/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/init_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/init_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15214 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/codeformer/vqgan_arch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.209161 nataili-0.3.4/nataili/util/controlnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/controlnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/create_random_tensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/get_next_sequence_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.209161 nataili-0.3.4/nataili/util/gfpgan/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/gfpgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/gfpgan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/image_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/load_learned_embed_in_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/load_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/normalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/process_prompt_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/save_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/seed_to_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/util/voodoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/v1-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/v1-inpainting-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/v2-inference-v.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/v2-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/v2-inpainting-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/v2-midas-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-29 10:00:59.000000 nataili-0.3.4/nataili/x4-upscaling.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.193161 nataili-0.3.4/nataili.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41929 2023-04-29 10:01:22.000000 nataili-0.3.4/nataili.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27216 2023-04-29 10:01:22.000000 nataili-0.3.4/nataili.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:01:22.000000 nataili-0.3.4/nataili.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-29 10:01:22.000000 nataili-0.3.4/nataili.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-29 10:01:22.000000 nataili-0.3.4/nataili.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-29 10:01:22.000000 nataili-0.3.4/nataili.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-29 10:01:07.000000 nataili-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-29 10:00:59.000000 nataili-0.3.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.213161 nataili-0.3.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/bulk_image_embeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/bulk_image_embeds_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/download_all_stable_diffusion_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/sdu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_ait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_all_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_clip_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_clip_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_coca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_codeformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_compvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_compvis_inpainting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_control_voodoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_controlnet_canny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_controlnet_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_controlnet_hed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_controlnet_hough.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_controlnet_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_controlnet_openpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_controlnet_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_depth2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_dreambooth_lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_esrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_file_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_gfpgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_img2img_voodoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_inpainting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_pix2pix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_pix2pix_voodoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_sd2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_txt2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_txt2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_txt2img_hires_voodoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-29 10:00:59.000000 nataili-0.3.4/scripts/test_txt2img_voodoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-29 10:01:22.213161 nataili-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-29 10:01:07.000000 nataili-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:01:22.213161 nataili-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-04-29 10:00:59.000000 nataili-0.3.4/tests/prompt_weights.py
```

### Comparing `nataili-0.3.3/LICENSE` & `nataili-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/PKG-INFO` & `nataili-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nataili
-Version: 0.3.3
+Version: 0.3.4
 Summary: Nataili: Multimodal AI Python Library
 Author-email: hlky <goto@github.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -677,17 +677,19 @@
 # Nataili: Multimodal AI Python Library
 
 [![PyPI version](https://badge.fury.io/py/nataili.svg)](https://badge.fury.io/py/nataili)
 [![Downloads](https://pepy.tech/badge/nataili)](https://pepy.tech/project/nataili)
 
 ![GitHub license](https://img.shields.io/github/license/db0/nataili)
 
-**!! NOTICE: Currently this package is looking for a lead developer !!**
+**!! NOTICE: This package is obsolete !!**
 
-Our only ML Develeloper has dropped out and the reamining team does not have the required skills to add new features. **If you see the value in this package, we urge you to contact us if you're interested in picking it up**. You can reach us [in discord](https://discord.gg/3DxrhksKzn) or in this repository issues.
+Please switch to using [hordelib](https://pypi.org/project/hordelib/) which is based on ComfyUI.
+
+---
 
 Nataili is a Python library that provides tools for building multimodal AI applications. With its modular design, Nataili makes it easy to use only the tools you need to build custom AI solutions.
 
 Some of the technologies included in Nataili are:
 
 * AITemplate: Fast diffusion
 * BLIP: Image captioning
```

### Comparing `nataili-0.3.3/README.md` & `nataili-0.3.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # Nataili: Multimodal AI Python Library
 
 [![PyPI version](https://badge.fury.io/py/nataili.svg)](https://badge.fury.io/py/nataili)
 [![Downloads](https://pepy.tech/badge/nataili)](https://pepy.tech/project/nataili)
 
 ![GitHub license](https://img.shields.io/github/license/db0/nataili)
 
-**!! NOTICE: Currently this package is looking for a lead developer !!**
+**!! NOTICE: This package is obsolete !!**
 
-Our only ML Develeloper has dropped out and the reamining team does not have the required skills to add new features. **If you see the value in this package, we urge you to contact us if you're interested in picking it up**. You can reach us [in discord](https://discord.gg/3DxrhksKzn) or in this repository issues.
+Please switch to using [hordelib](https://pypi.org/project/hordelib/) which is based on ComfyUI.
+
+---
 
 Nataili is a Python library that provides tools for building multimodal AI applications. With its modular design, Nataili makes it easy to use only the tools you need to build custom AI solutions.
 
 Some of the technologies included in Nataili are:
 
 * AITemplate: Fast diffusion
 * BLIP: Image captioning
```

### Comparing `nataili-0.3.3/annotator/hed/__init__.py` & `nataili-0.3.4/annotator/hed/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/midas/__init__.py` & `nataili-0.3.4/annotator/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/midas/api.py` & `nataili-0.3.4/annotator/midas/api.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/midas/midas/blocks.py` & `nataili-0.3.4/annotator/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/midas/midas/dpt_depth.py` & `nataili-0.3.4/annotator/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/midas/midas/midas_net.py` & `nataili-0.3.4/annotator/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/midas/midas/midas_net_custom.py` & `nataili-0.3.4/annotator/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/midas/midas/transforms.py` & `nataili-0.3.4/annotator/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/midas/midas/vit.py` & `nataili-0.3.4/annotator/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/midas/utils.py` & `nataili-0.3.4/annotator/midas/utils.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/mlsd/__init__.py` & `nataili-0.3.4/annotator/mlsd/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/mlsd/models/mbv2_mlsd_large.py` & `nataili-0.3.4/annotator/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/mlsd/models/mbv2_mlsd_tiny.py` & `nataili-0.3.4/annotator/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/mlsd/utils.py` & `nataili-0.3.4/annotator/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/openpose/__init__.py` & `nataili-0.3.4/annotator/openpose/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/openpose/body.py` & `nataili-0.3.4/annotator/openpose/body.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/openpose/hand.py` & `nataili-0.3.4/annotator/openpose/hand.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/openpose/model.py` & `nataili-0.3.4/annotator/openpose/model.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/openpose/util.py` & `nataili-0.3.4/annotator/openpose/util.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/__init__.py` & `nataili-0.3.4/annotator/uniformer/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/ade20k.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/chase_db1.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/cityscapes.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/cityscapes_769x769.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/cityscapes_769x769.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/drive.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/hrf.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/pascal_context.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/pascal_context_59.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/pascal_context_59.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/pascal_voc12.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/pascal_voc12.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/datasets/stare.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/ann_r50-d8.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/ann_r50-d8.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/apcnet_r50-d8.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/apcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/ccnet_r50-d8.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/ccnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/cgnet.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/cgnet.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/danet_r50-d8.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/danet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/deeplabv3_r50-d8.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/deeplabv3_r50-d8.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/dmnet_r50-d8.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/dmnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/dnl_r50-d8.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/dnl_r50-d8.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/emanet_r50-d8.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/emanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/encnet_r50-d8.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/encnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/fast_scnn.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/fcn_hr18.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/fcn_hr18.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/fcn_r50-d8.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/fcn_r50-d8.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/fcn_unet_s5-d16.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/fcn_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/fpn_r50.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/fpn_r50.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/fpn_uniformer.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/fpn_uniformer.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/gcnet_r50-d8.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/gcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/lraspp_m-v3-d8.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/lraspp_m-v3-d8.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/nonlocal_r50-d8.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/nonlocal_r50-d8.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/ocrnet_hr18.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/ocrnet_hr18.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/ocrnet_r50-d8.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/ocrnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/pointrend_r50.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/pointrend_r50.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/psanet_r50-d8.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/psanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/pspnet_r50-d8.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/pspnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/upernet_r50.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/upernet_r50.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/configs/_base_/models/upernet_uniformer.py` & `nataili-0.3.4/annotator/uniformer/configs/_base_/models/upernet_uniformer.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/exp/upernet_global_small/config.py` & `nataili-0.3.4/annotator/uniformer/exp/upernet_global_small/config.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/exp/upernet_global_small/test_config_g.py` & `nataili-0.3.4/annotator/uniformer/exp/upernet_global_small/test_config_g.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/exp/upernet_global_small/test_config_h32.py` & `nataili-0.3.4/annotator/uniformer/exp/upernet_global_small/test_config_h32.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/exp/upernet_global_small/test_config_w32.py` & `nataili-0.3.4/annotator/uniformer/exp/upernet_global_small/test_config_w32.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/arraymisc/quantization.py` & `nataili-0.3.4/annotator/uniformer/mmcv/arraymisc/quantization.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/__init__.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/alexnet.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/alexnet.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/__init__.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/activation.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/activation.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/context_block.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/context_block.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/conv.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/conv.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/conv_module.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/conv_module.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/conv_ws.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/conv_ws.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/drop.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/generalized_attention.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/generalized_attention.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/hsigmoid.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/hsigmoid.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/hswish.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/hswish.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/non_local.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/non_local.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/norm.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/norm.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/padding.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/padding.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/plugin.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/plugin.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/registry.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/registry.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/scale.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/scale.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/transformer.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/transformer.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/upsample.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/upsample.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/bricks/wrappers.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/bricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/builder.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/builder.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/resnet.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/utils/__init__.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/utils/flops_counter.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/utils/fuse_conv_bn.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/utils/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/utils/sync_bn.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/utils/sync_bn.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/utils/weight_init.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/cnn/vgg.py` & `nataili-0.3.4/annotator/uniformer/mmcv/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/engine/test.py` & `nataili-0.3.4/annotator/uniformer/mmcv/engine/test.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/fileio/file_client.py` & `nataili-0.3.4/annotator/uniformer/mmcv/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/fileio/handlers/base.py` & `nataili-0.3.4/annotator/uniformer/mmcv/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/fileio/handlers/json_handler.py` & `nataili-0.3.4/annotator/uniformer/mmcv/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/fileio/handlers/pickle_handler.py` & `nataili-0.3.4/annotator/uniformer/mmcv/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/fileio/handlers/yaml_handler.py` & `nataili-0.3.4/annotator/uniformer/mmcv/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/fileio/io.py` & `nataili-0.3.4/annotator/uniformer/mmcv/fileio/io.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/fileio/parse.py` & `nataili-0.3.4/annotator/uniformer/mmcv/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/image/__init__.py` & `nataili-0.3.4/annotator/uniformer/mmcv/image/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/image/colorspace.py` & `nataili-0.3.4/annotator/uniformer/mmcv/image/colorspace.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/image/geometric.py` & `nataili-0.3.4/annotator/uniformer/mmcv/image/geometric.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/image/io.py` & `nataili-0.3.4/annotator/uniformer/mmcv/image/io.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/image/misc.py` & `nataili-0.3.4/annotator/uniformer/mmcv/image/misc.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/image/photometric.py` & `nataili-0.3.4/annotator/uniformer/mmcv/image/photometric.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/__init__.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/assign_score_withk.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/assign_score_withk.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/ball_query.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/ball_query.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/bbox.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/border_align.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/border_align.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/box_iou_rotated.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/box_iou_rotated.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/carafe.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/carafe.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/cc_attention.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/cc_attention.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/contour_expand.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/contour_expand.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/corner_pool.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/corner_pool.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/correlation.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/correlation.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/deform_conv.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/deform_conv.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/deform_roi_pool.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/deform_roi_pool.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/deprecated_wrappers.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/deprecated_wrappers.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/focal_loss.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/focal_loss.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/furthest_point_sample.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/furthest_point_sample.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/fused_bias_leakyrelu.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/fused_bias_leakyrelu.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/gather_points.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/gather_points.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/group_points.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/group_points.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/info.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/info.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/iou3d.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/iou3d.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/knn.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/knn.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/masked_conv.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/masked_conv.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/merge_cells.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/merge_cells.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/modulated_deform_conv.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/modulated_deform_conv.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/multi_scale_deform_attn.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/multi_scale_deform_attn.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/nms.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/nms.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/pixel_group.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/pixel_group.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/point_sample.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/point_sample.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/points_in_boxes.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/points_in_boxes.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/points_sampler.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/points_sampler.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/psa_mask.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/psa_mask.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/roi_align.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/roi_align.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/roi_align_rotated.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/roi_pool.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/roi_pool.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/roiaware_pool3d.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/roiaware_pool3d.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/roipoint_pool3d.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/roipoint_pool3d.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/saconv.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/saconv.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/scatter_points.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/scatter_points.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/sync_bn.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/sync_bn.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/three_interpolate.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/three_interpolate.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/three_nn.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/three_nn.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/tin_shift.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/tin_shift.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/upfirdn2d.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/ops/voxelize.py` & `nataili-0.3.4/annotator/uniformer/mmcv/ops/voxelize.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/parallel/_functions.py` & `nataili-0.3.4/annotator/uniformer/mmcv/parallel/_functions.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/parallel/collate.py` & `nataili-0.3.4/annotator/uniformer/mmcv/parallel/collate.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/parallel/data_container.py` & `nataili-0.3.4/annotator/uniformer/mmcv/parallel/data_container.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/parallel/data_parallel.py` & `nataili-0.3.4/annotator/uniformer/mmcv/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/parallel/distributed.py` & `nataili-0.3.4/annotator/uniformer/mmcv/parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/parallel/distributed_deprecated.py` & `nataili-0.3.4/annotator/uniformer/mmcv/parallel/distributed_deprecated.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/parallel/scatter_gather.py` & `nataili-0.3.4/annotator/uniformer/mmcv/parallel/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/parallel/utils.py` & `nataili-0.3.4/annotator/uniformer/mmcv/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/__init__.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/base_module.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/base_module.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/base_runner.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/builder.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/builder.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/checkpoint.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/default_constructor.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/default_constructor.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/dist_utils.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/dist_utils.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/epoch_based_runner.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/epoch_based_runner.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/fp16_utils.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/fp16_utils.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/__init__.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/checkpoint.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/ema.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/ema.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/evaluation.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/evaluation.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/hook.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/__init__.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/base.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/base.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/dvclive.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/dvclive.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/mlflow.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/mlflow.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/neptune.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/neptune.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/pavi.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/pavi.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/tensorboard.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/text.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/text.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/logger/wandb.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/logger/wandb.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/lr_updater.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/lr_updater.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/memory.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/memory.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/momentum_updater.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/momentum_updater.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/optimizer.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/optimizer.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/profiler.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/profiler.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/sampler_seed.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/sampler_seed.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/hooks/sync_buffer.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/hooks/sync_buffer.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/iter_based_runner.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/iter_based_runner.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/log_buffer.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/log_buffer.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/optimizer/builder.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/optimizer/default_constructor.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/priority.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/priority.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/runner/utils.py` & `nataili-0.3.4/annotator/uniformer/mmcv/runner/utils.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/utils/__init__.py` & `nataili-0.3.4/annotator/uniformer/mmcv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/utils/config.py` & `nataili-0.3.4/annotator/uniformer/mmcv/utils/config.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/utils/env.py` & `nataili-0.3.4/annotator/uniformer/mmcv/utils/env.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/utils/ext_loader.py` & `nataili-0.3.4/annotator/uniformer/mmcv/utils/ext_loader.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/utils/logging.py` & `nataili-0.3.4/annotator/uniformer/mmcv/utils/logging.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/utils/misc.py` & `nataili-0.3.4/annotator/uniformer/mmcv/utils/misc.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/utils/parrots_jit.py` & `nataili-0.3.4/annotator/uniformer/mmcv/utils/parrots_jit.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/utils/parrots_wrapper.py` & `nataili-0.3.4/annotator/uniformer/mmcv/utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/utils/path.py` & `nataili-0.3.4/annotator/uniformer/mmcv/utils/path.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/utils/progressbar.py` & `nataili-0.3.4/annotator/uniformer/mmcv/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/utils/registry.py` & `nataili-0.3.4/annotator/uniformer/mmcv/utils/registry.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/utils/testing.py` & `nataili-0.3.4/annotator/uniformer/mmcv/utils/testing.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/utils/timer.py` & `nataili-0.3.4/annotator/uniformer/mmcv/utils/timer.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/utils/trace.py` & `nataili-0.3.4/annotator/uniformer/mmcv/utils/trace.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/utils/version_utils.py` & `nataili-0.3.4/annotator/uniformer/mmcv/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/version.py` & `nataili-0.3.4/annotator/uniformer/mmcv/version.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/video/__init__.py` & `nataili-0.3.4/annotator/uniformer/mmcv/video/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/video/io.py` & `nataili-0.3.4/annotator/uniformer/mmcv/video/io.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/video/optflow.py` & `nataili-0.3.4/annotator/uniformer/mmcv/video/optflow.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/video/processing.py` & `nataili-0.3.4/annotator/uniformer/mmcv/video/processing.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/visualization/color.py` & `nataili-0.3.4/annotator/uniformer/mmcv/visualization/color.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/visualization/image.py` & `nataili-0.3.4/annotator/uniformer/mmcv/visualization/image.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv/visualization/optflow.py` & `nataili-0.3.4/annotator/uniformer/mmcv/visualization/optflow.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmcv_custom/checkpoint.py` & `nataili-0.3.4/annotator/uniformer/mmcv_custom/checkpoint.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/apis/inference.py` & `nataili-0.3.4/annotator/uniformer/mmseg/apis/inference.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/apis/test.py` & `nataili-0.3.4/annotator/uniformer/mmseg/apis/test.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/apis/train.py` & `nataili-0.3.4/annotator/uniformer/mmseg/apis/train.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/core/evaluation/class_names.py` & `nataili-0.3.4/annotator/uniformer/mmseg/core/evaluation/class_names.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/core/evaluation/eval_hooks.py` & `nataili-0.3.4/annotator/uniformer/mmseg/core/evaluation/eval_hooks.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/core/evaluation/metrics.py` & `nataili-0.3.4/annotator/uniformer/mmseg/core/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py` & `nataili-0.3.4/annotator/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/datasets/__init__.py` & `nataili-0.3.4/annotator/uniformer/mmseg/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/datasets/ade.py` & `nataili-0.3.4/annotator/uniformer/mmseg/datasets/ade.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/datasets/builder.py` & `nataili-0.3.4/annotator/uniformer/mmseg/datasets/builder.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/datasets/chase_db1.py` & `nataili-0.3.4/annotator/uniformer/mmseg/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/datasets/cityscapes.py` & `nataili-0.3.4/annotator/uniformer/mmseg/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/datasets/custom.py` & `nataili-0.3.4/annotator/uniformer/mmseg/datasets/custom.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/datasets/dataset_wrappers.py` & `nataili-0.3.4/annotator/uniformer/mmseg/datasets/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/datasets/drive.py` & `nataili-0.3.4/annotator/uniformer/mmseg/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/datasets/hrf.py` & `nataili-0.3.4/annotator/uniformer/mmseg/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/datasets/pascal_context.py` & `nataili-0.3.4/annotator/uniformer/mmseg/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/datasets/pipelines/__init__.py` & `nataili-0.3.4/annotator/uniformer/mmseg/datasets/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/datasets/pipelines/compose.py` & `nataili-0.3.4/annotator/uniformer/mmseg/datasets/pipelines/compose.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/datasets/pipelines/formating.py` & `nataili-0.3.4/annotator/uniformer/mmseg/datasets/pipelines/formating.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/datasets/pipelines/loading.py` & `nataili-0.3.4/annotator/uniformer/mmseg/datasets/pipelines/loading.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/datasets/pipelines/test_time_aug.py` & `nataili-0.3.4/annotator/uniformer/mmseg/datasets/pipelines/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/datasets/pipelines/transforms.py` & `nataili-0.3.4/annotator/uniformer/mmseg/datasets/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/datasets/stare.py` & `nataili-0.3.4/annotator/uniformer/mmseg/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/datasets/voc.py` & `nataili-0.3.4/annotator/uniformer/mmseg/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/__init__.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/cgnet.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/cgnet.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/fast_scnn.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/hrnet.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/hrnet.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/mobilenet_v2.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/mobilenet_v3.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/resnest.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/resnest.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/resnet.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/resnext.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/unet.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/unet.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/uniformer.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/uniformer.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/backbones/vit.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/builder.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/builder.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/__init__.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/ann_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/ann_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/apc_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/apc_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/aspp_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/aspp_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/cascade_decode_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/cascade_decode_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/cc_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/cc_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/da_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/da_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/decode_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/decode_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/dm_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/dm_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/dnl_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/dnl_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/ema_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/ema_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/enc_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/enc_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/fcn_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/fcn_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/fpn_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/fpn_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/gc_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/gc_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/lraspp_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/lraspp_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/nl_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/nl_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/ocr_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/ocr_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/point_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/point_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/psa_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/psa_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/psp_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/psp_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/sep_aspp_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/sep_aspp_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/sep_fcn_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/sep_fcn_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/decode_heads/uper_head.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/decode_heads/uper_head.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/losses/__init__.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/losses/accuracy.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/losses/cross_entropy_loss.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/losses/dice_loss.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/losses/dice_loss.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/losses/lovasz_loss.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/losses/lovasz_loss.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/losses/utils.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/losses/utils.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/necks/fpn.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/necks/fpn.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/necks/multilevel_neck.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/necks/multilevel_neck.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/segmentors/base.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/segmentors/base.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/segmentors/encoder_decoder.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/segmentors/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/utils/drop.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/utils/drop.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/utils/inverted_residual.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/utils/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/utils/make_divisible.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/utils/make_divisible.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/utils/res_layer.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/utils/res_layer.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/utils/se_layer.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/utils/se_layer.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/utils/self_attention_block.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/utils/self_attention_block.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/utils/up_conv_block.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/utils/up_conv_block.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/models/utils/weight_init.py` & `nataili-0.3.4/annotator/uniformer/mmseg/models/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/ops/encoding.py` & `nataili-0.3.4/annotator/uniformer/mmseg/ops/encoding.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/ops/wrappers.py` & `nataili-0.3.4/annotator/uniformer/mmseg/ops/wrappers.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/uniformer/mmseg/utils/logger.py` & `nataili-0.3.4/annotator/uniformer/mmseg/utils/logger.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/annotator/util.py` & `nataili-0.3.4/annotator/util.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/cldm/cldm.py` & `nataili-0.3.4/cldm/cldm.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/cldm/hack.py` & `nataili-0.3.4/cldm/hack.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/cldm/logger.py` & `nataili-0.3.4/cldm/logger.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/data/base.py` & `nataili-0.3.4/ldm/data/base.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/data/imagenet.py` & `nataili-0.3.4/ldm/data/imagenet.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/data/lsun.py` & `nataili-0.3.4/ldm/data/lsun.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/lr_scheduler.py` & `nataili-0.3.4/ldm/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/models/autoencoder.py` & `nataili-0.3.4/ldm/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/models/blip.py` & `nataili-0.3.4/ldm/models/blip.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/models/blip_itm.py` & `nataili-0.3.4/ldm/models/blip_itm.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/models/blip_nlvr.py` & `nataili-0.3.4/ldm/models/blip_nlvr.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/models/blip_pretrain.py` & `nataili-0.3.4/ldm/models/blip_pretrain.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/models/blip_retrieval.py` & `nataili-0.3.4/ldm/models/blip_retrieval.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/models/blip_vqa.py` & `nataili-0.3.4/ldm/models/blip_vqa.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/models/diffusion/classifier.py` & `nataili-0.3.4/ldm/models/diffusion/classifier.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/models/diffusion/ddim.py` & `nataili-0.3.4/ldm/models/diffusion/ddim.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/models/diffusion/ddpm.py` & `nataili-0.3.4/ldm/models/diffusion/ddpm.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/models/diffusion/ddpm_edit.py` & `nataili-0.3.4/ldm/models/diffusion/ddpm_edit.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/models/diffusion/kdiffusion.py` & `nataili-0.3.4/ldm/models/diffusion/kdiffusion.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/models/diffusion/plms.py` & `nataili-0.3.4/ldm/models/diffusion/plms.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/models/med.py` & `nataili-0.3.4/ldm/models/med.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/models/nlvr_encoder.py` & `nataili-0.3.4/ldm/models/nlvr_encoder.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/models/vit.py` & `nataili-0.3.4/ldm/models/vit.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/modules/attention.py` & `nataili-0.3.4/ldm/modules/attention.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/modules/diffusionmodules/model.py` & `nataili-0.3.4/ldm/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/modules/diffusionmodules/openaimodel.py` & `nataili-0.3.4/ldm/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/modules/diffusionmodules/util.py` & `nataili-0.3.4/ldm/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/modules/distributions/distributions.py` & `nataili-0.3.4/ldm/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/modules/ema.py` & `nataili-0.3.4/ldm/modules/ema.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/modules/encoders/modules.py` & `nataili-0.3.4/ldm/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/modules/image_degradation/bsrgan.py` & `nataili-0.3.4/ldm/modules/image_degradation/bsrgan.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/modules/image_degradation/bsrgan_light.py` & `nataili-0.3.4/ldm/modules/image_degradation/bsrgan_light.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/modules/image_degradation/utils_image.py` & `nataili-0.3.4/ldm/modules/image_degradation/utils_image.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/modules/losses/contperceptual.py` & `nataili-0.3.4/ldm/modules/losses/contperceptual.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/modules/losses/vqperceptual.py` & `nataili-0.3.4/ldm/modules/losses/vqperceptual.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/modules/x_transformer.py` & `nataili-0.3.4/ldm/modules/x_transformer.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm/util.py` & `nataili-0.3.4/ldm/util.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/data/util.py` & `nataili-0.3.4/ldm2/data/util.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/models/autoencoder.py` & `nataili-0.3.4/ldm2/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/models/diffusion/ddim.py` & `nataili-0.3.4/ldm2/models/diffusion/ddim.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/models/diffusion/ddpm.py` & `nataili-0.3.4/ldm2/models/diffusion/ddpm.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/models/diffusion/dpm_solver/dpm_solver.py` & `nataili-0.3.4/ldm2/models/diffusion/dpm_solver/dpm_solver.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/models/diffusion/dpm_solver/sampler.py` & `nataili-0.3.4/ldm2/models/diffusion/dpm_solver/sampler.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/models/diffusion/plms.py` & `nataili-0.3.4/ldm2/models/diffusion/plms.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/models/diffusion/sampling_util.py` & `nataili-0.3.4/ldm2/models/diffusion/sampling_util.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/attention.py` & `nataili-0.3.4/ldm2/modules/attention.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/diffusionmodules/model.py` & `nataili-0.3.4/ldm2/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/diffusionmodules/openaimodel.py` & `nataili-0.3.4/ldm2/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/diffusionmodules/upscaling.py` & `nataili-0.3.4/ldm2/modules/diffusionmodules/upscaling.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/diffusionmodules/util.py` & `nataili-0.3.4/ldm2/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/distributions/distributions.py` & `nataili-0.3.4/ldm2/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/ema.py` & `nataili-0.3.4/ldm2/modules/ema.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/encoders/modules.py` & `nataili-0.3.4/ldm2/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/image_degradation/bsrgan.py` & `nataili-0.3.4/ldm2/modules/image_degradation/bsrgan.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/image_degradation/bsrgan_light.py` & `nataili-0.3.4/ldm2/modules/image_degradation/bsrgan_light.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/image_degradation/utils_image.py` & `nataili-0.3.4/ldm2/modules/image_degradation/utils_image.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/midas/api.py` & `nataili-0.3.4/ldm2/modules/midas/api.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/midas/midas/blocks.py` & `nataili-0.3.4/ldm2/modules/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/midas/midas/dpt_depth.py` & `nataili-0.3.4/ldm2/modules/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/midas/midas/midas_net.py` & `nataili-0.3.4/ldm2/modules/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/midas/midas/midas_net_custom.py` & `nataili-0.3.4/ldm2/modules/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/midas/midas/transforms.py` & `nataili-0.3.4/ldm2/modules/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/midas/midas/vit.py` & `nataili-0.3.4/ldm2/modules/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/modules/midas/utils.py` & `nataili-0.3.4/ldm2/modules/midas/utils.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/ldm2/util.py` & `nataili-0.3.4/ldm2/util.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/aitemplate/AITemplate.py` & `nataili-0.3.4/nataili/aitemplate/AITemplate.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/aitemplate/ait_pipeline.py` & `nataili-0.3.4/nataili/aitemplate/ait_pipeline.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/aitemplate/dtype.py` & `nataili-0.3.4/nataili/aitemplate/dtype.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/aitemplate/model.py` & `nataili-0.3.4/nataili/aitemplate/model.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/aitemplate/torch_utils.py` & `nataili-0.3.4/nataili/aitemplate/torch_utils.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/aitemplate.json` & `nataili-0.3.4/nataili/aitemplate.json`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/artists.txt` & `nataili-0.3.4/nataili/artists.txt`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/blip/caption.py` & `nataili-0.3.4/nataili/blip/caption.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/blip.json` & `nataili-0.3.4/nataili/blip.json`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/cache/cache.py` & `nataili-0.3.4/nataili/cache/cache.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/cldm_v15.yaml` & `nataili-0.3.4/nataili/cldm_v15.yaml`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/cldm_v21.yaml` & `nataili-0.3.4/nataili/cldm_v21.yaml`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/clip/bulk.py` & `nataili-0.3.4/nataili/clip/bulk.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/clip/coca.py` & `nataili-0.3.4/nataili/clip/coca.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/clip/image.py` & `nataili-0.3.4/nataili/clip/image.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/clip/interrogate.py` & `nataili-0.3.4/nataili/clip/interrogate.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/clip/predictor/inference.py` & `nataili-0.3.4/nataili/clip/predictor/inference.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/clip/predictor/mlp.py` & `nataili-0.3.4/nataili/clip/predictor/mlp.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/clip/predictor/prepare.py` & `nataili-0.3.4/nataili/clip/predictor/prepare.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/clip/predictor/train.py` & `nataili-0.3.4/nataili/clip/predictor/train.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/clip/text.py` & `nataili-0.3.4/nataili/clip/text.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/clip.json` & `nataili-0.3.4/nataili/clip.json`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/codeformers/codeformers.py` & `nataili-0.3.4/nataili/codeformers/codeformers.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/controlnet.json` & `nataili-0.3.4/nataili/controlnet.json`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/diffusers.json` & `nataili-0.3.4/nataili/diffusers.json`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/esrgan/esrgan.py` & `nataili-0.3.4/nataili/esrgan/esrgan.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/esrgan.json` & `nataili-0.3.4/nataili/esrgan.json`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/flavors.txt` & `nataili-0.3.4/nataili/flavors.txt`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/gfpgan/gfpgan.py` & `nataili-0.3.4/nataili/gfpgan/gfpgan.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/gfpgan.json` & `nataili-0.3.4/nataili/gfpgan.json`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/mediums.txt` & `nataili-0.3.4/nataili/mediums.txt`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/model_manager/aitemplate.py` & `nataili-0.3.4/nataili/model_manager/aitemplate.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/model_manager/base.py` & `nataili-0.3.4/nataili/model_manager/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,26 @@
                 logger.info(model)
 
     def download_model_reference(self):
         try:
             logger.init("Model Reference", status="Downloading")
             response = requests.get(self.remote_db)
             logger.init_ok("Model Reference", status="OK")
-            models = response.json()
+            temp_models = response.json()
+            models = {}
+            # XXX filter out safetensors models for compvis
+            for model_name, model_data in temp_models.items():
+                skip = False
+                if model_data.get("type") == "ckpt" and "stable diffusion" in model_data.get("baseline", ""):
+                    downloads = model_data.get("config", {}).get("download", [])
+                    for download in downloads:
+                        if download.get("file_name").lower().endswith(".safetensors"):
+                            skip = True
+                if not skip:
+                    models[model_name] = model_data
             return models
         except Exception as e:
             logger.init_err("Model Reference", status=f"Download failed: {e}")
             logger.init_warn("Model Reference", status="Local")
             return json.loads((self.models_path).read_text())
 
     def get_model(self, model_name):
```

### Comparing `nataili-0.3.3/nataili/model_manager/blip.py` & `nataili-0.3.4/nataili/model_manager/blip.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/model_manager/clip.py` & `nataili-0.3.4/nataili/model_manager/clip.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/model_manager/codeformer.py` & `nataili-0.3.4/nataili/model_manager/codeformer.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/model_manager/compvis.py` & `nataili-0.3.4/nataili/model_manager/compvis.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/model_manager/controlnet.py` & `nataili-0.3.4/nataili/model_manager/controlnet.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/model_manager/diffusers.py` & `nataili-0.3.4/nataili/model_manager/diffusers.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/model_manager/esrgan.py` & `nataili-0.3.4/nataili/model_manager/esrgan.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/model_manager/gfpgan.py` & `nataili-0.3.4/nataili/model_manager/gfpgan.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/model_manager/new.py` & `nataili-0.3.4/nataili/model_manager/new.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/model_manager/safety_checker.py` & `nataili-0.3.4/nataili/model_manager/safety_checker.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/model_manager/sdu.py` & `nataili-0.3.4/nataili/model_manager/sdu.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/model_manager/super.py` & `nataili-0.3.4/nataili/model_manager/super.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/movements.txt` & `nataili-0.3.4/nataili/movements.txt`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/pix2pix.yaml` & `nataili-0.3.4/nataili/pix2pix.yaml`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/safety_checker.json` & `nataili-0.3.4/nataili/safety_checker.json`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/sdu/sdu.py` & `nataili-0.3.4/nataili/sdu/sdu.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/sdu.json` & `nataili-0.3.4/nataili/sdu.json`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/stable_diffusion/annotation.py` & `nataili-0.3.4/nataili/stable_diffusion/annotation.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/stable_diffusion/compvis.py` & `nataili-0.3.4/nataili/stable_diffusion/compvis.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/stable_diffusion/diffusers/depth2img.py` & `nataili-0.3.4/nataili/stable_diffusion/diffusers/depth2img.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/stable_diffusion/diffusers/inpainting.py` & `nataili-0.3.4/nataili/stable_diffusion/diffusers/inpainting.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/stable_diffusion/prompt_weights.py` & `nataili-0.3.4/nataili/stable_diffusion/prompt_weights.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/stable_diffusion.json` & `nataili-0.3.4/nataili/stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/tags.txt` & `nataili-0.3.4/nataili/tags.txt`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/techniques.txt` & `nataili-0.3.4/nataili/techniques.txt`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/train/dataset/EveryDream/aspects.py` & `nataili-0.3.4/nataili/train/dataset/EveryDream/aspects.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/train/dataset/EveryDream/data_loader.py` & `nataili-0.3.4/nataili/train/dataset/EveryDream/data_loader.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/train/dataset/EveryDream/ed_dl_wrap.py` & `nataili-0.3.4/nataili/train/dataset/EveryDream/ed_dl_wrap.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/train/dataset/EveryDream/ed_validate.py` & `nataili-0.3.4/nataili/train/dataset/EveryDream/ed_validate.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/train/dataset/EveryDream/every_dream.py` & `nataili-0.3.4/nataili/train/dataset/EveryDream/every_dream.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/train/dataset/EveryDream/image_train_item.py` & `nataili-0.3.4/nataili/train/dataset/EveryDream/image_train_item.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/train/dataset/EveryDream/latent_cache.py` & `nataili-0.3.4/nataili/train/dataset/EveryDream/latent_cache.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/train/dreambooth/dreambooth_lora.py` & `nataili-0.3.4/nataili/train/dreambooth/dreambooth_lora.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/train/lora/lora.py` & `nataili-0.3.4/nataili/train/lora/lora.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/ui/gradio/base.py` & `nataili-0.3.4/nataili/ui/gradio/base.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/ui/gradio/blip.py` & `nataili-0.3.4/nataili/ui/gradio/blip.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/ui/gradio/coca.py` & `nataili-0.3.4/nataili/ui/gradio/coca.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/ui/gradio/codeformer.py` & `nataili-0.3.4/nataili/ui/gradio/codeformer.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/ui/gradio/lora.py` & `nataili-0.3.4/nataili/ui/gradio/lora.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/__init__.py` & `nataili-0.3.4/nataili/util/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/blip/blip.py` & `nataili-0.3.4/nataili/util/blip/blip.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/blip/med.py` & `nataili-0.3.4/nataili/util/blip/med.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/blip/vit.py` & `nataili-0.3.4/nataili/util/blip/vit.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/cache.py` & `nataili-0.3.4/nataili/util/cache.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/cast.py` & `nataili-0.3.4/nataili/util/cast.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/check_prompt_length.py` & `nataili-0.3.4/nataili/util/check_prompt_length.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/codeformer.py` & `nataili-0.3.4/nataili/util/codeformer/codeformer.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/codeformer_arch.py` & `nataili-0.3.4/nataili/util/codeformer/codeformer_arch.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/face_restoration_helper.py` & `nataili-0.3.4/nataili/util/codeformer/face_restoration_helper.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/detection/__init__.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/detection/align_trans.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/detection/align_trans.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/detection/matlab_cp2tform.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/detection/matlab_cp2tform.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/detection/retinaface/retinaface.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/detection/retinaface/retinaface.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/detection/retinaface/retinaface_net.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/detection/retinaface/retinaface_net.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/detection/retinaface/retinaface_utils.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/detection/retinaface/retinaface_utils.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/face_detector.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/face_detector.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/models/common.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/models/common.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/models/experimental.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/models/experimental.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/models/yolo.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/models/yolo.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/utils/datasets.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/utils/general.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/utils/general.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/detection/yolov5face/utils/torch_utils.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/detection/yolov5face/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/parsing/__init__.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/parsing/bisenet.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/parsing/bisenet.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/parsing/parsenet.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/parsing/parsenet.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/parsing/resnet.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/parsing/resnet.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/utils/face_restoration_helper.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/utils/face_restoration_helper.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/utils/face_utils.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/utils/face_utils.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/facelib/utils/misc.py` & `nataili-0.3.4/nataili/util/codeformer/facelib/utils/misc.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/init_detection.py` & `nataili-0.3.4/nataili/util/codeformer/init_detection.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/init_parsing.py` & `nataili-0.3.4/nataili/util/codeformer/init_parsing.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/misc.py` & `nataili-0.3.4/nataili/util/codeformer/misc.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/realesrgan.py` & `nataili-0.3.4/nataili/util/codeformer/realesrgan.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/codeformer/vqgan_arch.py` & `nataili-0.3.4/nataili/util/codeformer/vqgan_arch.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/create_random_tensors.py` & `nataili-0.3.4/nataili/util/create_random_tensors.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/get_next_sequence_number.py` & `nataili-0.3.4/nataili/util/get_next_sequence_number.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/gfpgan/utils.py` & `nataili-0.3.4/nataili/util/gfpgan/utils.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/image_grid.py` & `nataili-0.3.4/nataili/util/image_grid.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/img2img.py` & `nataili-0.3.4/nataili/util/img2img.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/load_learned_embed_in_clip.py` & `nataili-0.3.4/nataili/util/load_learned_embed_in_clip.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/load_list.py` & `nataili-0.3.4/nataili/util/load_list.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/logger.py` & `nataili-0.3.4/nataili/util/logger.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/monitor.py` & `nataili-0.3.4/nataili/util/monitor.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/postprocessor.py` & `nataili-0.3.4/nataili/util/postprocessor.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/process_prompt_tokens.py` & `nataili-0.3.4/nataili/util/process_prompt_tokens.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/save_sample.py` & `nataili-0.3.4/nataili/util/save_sample.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/seed_to_int.py` & `nataili-0.3.4/nataili/util/seed_to_int.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/switch.py` & `nataili-0.3.4/nataili/util/switch.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/util/voodoo.py` & `nataili-0.3.4/nataili/util/voodoo.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/v1-inference.yaml` & `nataili-0.3.4/nataili/v1-inference.yaml`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/v1-inpainting-inference.yaml` & `nataili-0.3.4/nataili/v1-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/v2-inference-v.yaml` & `nataili-0.3.4/nataili/v2-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/v2-inference.yaml` & `nataili-0.3.4/nataili/v2-inference.yaml`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/v2-inpainting-inference.yaml` & `nataili-0.3.4/nataili/v2-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/v2-midas-inference.yaml` & `nataili-0.3.4/nataili/v2-midas-inference.yaml`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili/x4-upscaling.yaml` & `nataili-0.3.4/nataili/x4-upscaling.yaml`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/nataili.egg-info/PKG-INFO` & `nataili-0.3.4/nataili.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nataili
-Version: 0.3.3
+Version: 0.3.4
 Summary: Nataili: Multimodal AI Python Library
 Author-email: hlky <goto@github.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -677,17 +677,19 @@
 # Nataili: Multimodal AI Python Library
 
 [![PyPI version](https://badge.fury.io/py/nataili.svg)](https://badge.fury.io/py/nataili)
 [![Downloads](https://pepy.tech/badge/nataili)](https://pepy.tech/project/nataili)
 
 ![GitHub license](https://img.shields.io/github/license/db0/nataili)
 
-**!! NOTICE: Currently this package is looking for a lead developer !!**
+**!! NOTICE: This package is obsolete !!**
 
-Our only ML Develeloper has dropped out and the reamining team does not have the required skills to add new features. **If you see the value in this package, we urge you to contact us if you're interested in picking it up**. You can reach us [in discord](https://discord.gg/3DxrhksKzn) or in this repository issues.
+Please switch to using [hordelib](https://pypi.org/project/hordelib/) which is based on ComfyUI.
+
+---
 
 Nataili is a Python library that provides tools for building multimodal AI applications. With its modular design, Nataili makes it easy to use only the tools you need to build custom AI solutions.
 
 Some of the technologies included in Nataili are:
 
 * AITemplate: Fast diffusion
 * BLIP: Image captioning
```

### Comparing `nataili-0.3.3/nataili.egg-info/SOURCES.txt` & `nataili-0.3.4/nataili.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/pyproject.toml` & `nataili-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [build-system]
 requires = ["setuptools>=64.0", "pip>=20.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nataili"
-version = "v0.3.3"
+version = "v0.3.4"
 authors = [
     { name="hlky", email="goto@github.com" },
 ]
 description = "Nataili: Multimodal AI Python Library"
 readme = "README.md"
 license = { file="LICENSE" }
 dynamic = ["dependencies"]
```

### Comparing `nataili-0.3.3/scripts/bulk_image_embeds.py` & `nataili-0.3.4/scripts/bulk_image_embeds.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/bulk_image_embeds_webdataset.py` & `nataili-0.3.4/scripts/bulk_image_embeds_webdataset.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/sdu.py` & `nataili-0.3.4/scripts/sdu.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_all_models.py` & `nataili-0.3.4/scripts/test_all_models.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_clip_rank.py` & `nataili-0.3.4/scripts/test_clip_rank.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_clip_similarity.py` & `nataili-0.3.4/scripts/test_clip_similarity.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_coca.py` & `nataili-0.3.4/scripts/test_coca.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_codeformers.py` & `nataili-0.3.4/scripts/test_codeformers.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_compvis.py` & `nataili-0.3.4/scripts/test_compvis.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_compvis_inpainting.py` & `nataili-0.3.4/scripts/test_compvis_inpainting.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_control.py` & `nataili-0.3.4/scripts/test_control.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_control_voodoo.py` & `nataili-0.3.4/scripts/test_control_voodoo.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_controlnet_canny.py` & `nataili-0.3.4/scripts/test_controlnet_canny.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_controlnet_depth.py` & `nataili-0.3.4/scripts/test_controlnet_depth.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_controlnet_hed.py` & `nataili-0.3.4/scripts/test_controlnet_hed.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_controlnet_hough.py` & `nataili-0.3.4/scripts/test_controlnet_hough.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_controlnet_normal.py` & `nataili-0.3.4/scripts/test_controlnet_normal.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_controlnet_openpose.py` & `nataili-0.3.4/scripts/test_controlnet_openpose.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_controlnet_seg.py` & `nataili-0.3.4/scripts/test_controlnet_seg.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_depth2img.py` & `nataili-0.3.4/scripts/test_depth2img.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_file_hashes.py` & `nataili-0.3.4/scripts/test_file_hashes.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_img2img.py` & `nataili-0.3.4/scripts/test_img2img.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_img2img_voodoo.py` & `nataili-0.3.4/scripts/test_img2img_voodoo.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_inpainting.py` & `nataili-0.3.4/scripts/test_inpainting.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_pix2pix.py` & `nataili-0.3.4/scripts/test_pix2pix.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_pix2pix_voodoo.py` & `nataili-0.3.4/scripts/test_pix2pix_voodoo.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_safety_checker.py` & `nataili-0.3.4/scripts/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_sd2.py` & `nataili-0.3.4/scripts/test_sd2.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_txt2img.py` & `nataili-0.3.4/scripts/test_txt2img.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_txt2img_hires.py` & `nataili-0.3.4/scripts/test_txt2img_hires.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_txt2img_hires_voodoo.py` & `nataili-0.3.4/scripts/test_txt2img_hires_voodoo.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/scripts/test_txt2img_voodoo.py` & `nataili-0.3.4/scripts/test_txt2img_voodoo.py`

 * *Files identical despite different names*

### Comparing `nataili-0.3.3/setup.py` & `nataili-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 requirements = []
 with open("requirements.txt") as reqstxt:
     requirements = reqstxt.readlines()
 
 setup(
     name="nataili",
-    version="v0.3.3",
+    version="v0.3.4",
     description="",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "nataili_ui_coca = nataili.ui.gradio.coca:main",
             "nataili_ui_blip = nataili.ui.gradio.blip:main",
```

### Comparing `nataili-0.3.3/tests/prompt_weights.py` & `nataili-0.3.4/tests/prompt_weights.py`

 * *Files identical despite different names*


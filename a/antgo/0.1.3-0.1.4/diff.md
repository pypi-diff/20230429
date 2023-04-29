# Comparing `tmp/antgo-0.1.3.tar.gz` & `tmp/antgo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antgo-0.1.3.tar", last modified: Tue Apr 25 02:44:25 2023, max compression
+gzip compressed data, was "antgo-0.1.4.tar", last modified: Sat Apr 29 06:56:00 2023, max compression
```

## Comparing `antgo-0.1.3.tar` & `antgo-0.1.4.tar`

### file list

```diff
@@ -1,944 +1,944 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.578096 antgo-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/LICENSE.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-04-25 02:41:44.000000 antgo-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-25 02:44:25.578096 antgo-0.1.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     4480 2023-04-25 02:41:44.000000 antgo-0.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.282095 antgo-0.1.3/antgo/
--rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.290095 antgo-0.1.3/antgo/ant/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25864 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/activelearning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/activelearning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/activelearning_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9805 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/batch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14101 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/browser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28324 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)    34652 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    22044 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/environment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4162 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/flags.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44521 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/train.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/ant/watch.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1711 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      228 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/config.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)     8645 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.294095 antgo-0.1.3/antgo/crowdsource/
--rwxr-xr-x   0 runner    (1001) docker     (123)      206 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/crowdsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/crowdsource/activelearning_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/crowdsource/base_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    12973 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/crowdsource/batch_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43022 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/crowdsource/browser_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6412 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/crowdsource/crowdsource_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    27245 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/crowdsource/demo_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    15578 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/crowdsource/ensemble_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    33823 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/crowdsource/label_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/crowdsource/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8055 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/crowdsource/watch_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.298095 antgo-0.1.3/antgo/cutils/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8249 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/cutils/maskApi.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2176 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/cutils/maskApi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.298095 antgo-0.1.3/antgo/dataflow/
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5412 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/basic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22875 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14235 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.310095 antgo-0.1.3/antgo/dataflow/dataset/
--rwxr-xr-x   0 runner    (1001) docker     (123)      783 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/ade20k.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14996 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/celeba.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5425 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/cityscape.py
--rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/clsdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    25177 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/coco2017.py
--rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/cusdomcls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29220 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/empty_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/fashionai_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/fashionai_landmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/flic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3139 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/horse2zebra.py
--rw-r--r--   0 runner    (1001) docker     (123)    35327 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16512 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/interhand26M.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3083 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/iphone2dslr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8328 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/lfw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/lip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/lsp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/mpii.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3725 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/omniglot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/parallel_read.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13131 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/pascal_voc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/proxy_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/queue_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/random_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14554 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4465 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/simpleimages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/simplevideos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/spider_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3559 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/vggface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/dataset/visalso.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/datasetio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.310095 antgo-0.1.3/antgo/dataflow/datasynth/
--rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/datasynth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.314095 antgo-0.1.3/antgo/dataflow/imgaug/
--rwxr-xr-x   0 runner    (1001) docker     (123)      943 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/imgaug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65619 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/imgaug/autoaugment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    46247 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/imgaug/batch_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/imgaug/colorspace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3274 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/imgaug/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    25279 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/imgaug/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/imgaug/gridmask_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16268 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/imgaug/op_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)   104820 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/imgaug/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/imgaug/operators_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    17718 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/imgaug/photometric.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10813 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/imgaug/regular.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/imgaug/util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21369 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/dataflow/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.314095 antgo-0.1.3/antgo/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.318095 antgo-0.1.3/antgo/framework/helper/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/activelearning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.322095 antgo-0.1.3/antgo/framework/helper/apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/apis/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/base_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.322095 antgo-0.1.3/antgo/framework/helper/cnn/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/alexnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.322095 antgo-0.1.3/antgo/framework/helper/cnn/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/backbone/ddr_lcnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/backbone/ddr_mobilenet_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.330095 antgo-0.1.3/antgo/framework/helper/cnn/bricks/
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/context_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/conv2d_adaptive_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/conv_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/depthwise_separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/generalized_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/hsigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/hswish.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/non_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/swish.py
--rw-r--r--   0 runner    (1001) docker     (123)    37224 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/waterfall.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/bricks/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.334095 antgo-0.1.3/antgo/framework/helper/cnn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/utils/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/utils/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)    26005 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/utils/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/cnn/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.334095 antgo-0.1.3/antgo/framework/helper/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.334095 antgo-0.1.3/antgo/framework/helper/configs/activelearning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/configs/activelearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/configs/activelearning/ac_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.334095 antgo-0.1.3/antgo/framework/helper/configs/adda/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/configs/adda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/configs/adda/adda_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.334095 antgo-0.1.3/antgo/framework/helper/configs/distillation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/configs/distillation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/configs/distillation/reviewkd_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.334095 antgo-0.1.3/antgo/framework/helper/configs/semi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/configs/semi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/configs/semi/dense_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/configs/semi/detmpl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/configs/semi/mpl_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.338095 antgo-0.1.3/antgo/framework/helper/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/dataset/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/dataset/dataset_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/dataset/dataset_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/dataset/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/dataset/kvdataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.338095 antgo-0.1.3/antgo/framework/helper/dataset/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/dataset/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37456 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/dataset/pipelines/auto_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/dataset/pipelines/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/dataset/pipelines/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    29127 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/dataset/pipelines/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.342095 antgo-0.1.3/antgo/framework/helper/dataset/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/dataset/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/dataset/samplers/class_aware_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/dataset/samplers/distributed_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/dataset/samplers/group_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/dataset/samplers/infinite_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/dataset/samplers/kv_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    22421 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/dataset/tfdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.342095 antgo-0.1.3/antgo/framework/helper/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.342095 antgo-0.1.3/antgo/framework/helper/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.346095 antgo-0.1.3/antgo/framework/helper/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/metrics/kp2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/metrics/seg2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.346095 antgo-0.1.3/antgo/framework/helper/models/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.346095 antgo-0.1.3/antgo/framework/helper/models/activelearning/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/activelearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/activelearning/acnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.346095 antgo-0.1.3/antgo/framework/helper/models/adda/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/adda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/adda/adda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.350095 antgo-0.1.3/antgo/framework/helper/models/classification/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.350095 antgo-0.1.3/antgo/framework/helper/models/classification/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/classification/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23127 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/classification/backbones/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/classification/backbones/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    23751 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/classification/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/classification/backbones/resnext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.350095 antgo-0.1.3/antgo/framework/helper/models/classification/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/classification/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/classification/heads/cls_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/classification/heads/stacked_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.350095 antgo-0.1.3/antgo/framework/helper/models/classification/losses/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/classification/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/classification/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/classification/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/classification/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.354095 antgo-0.1.3/antgo/framework/helper/models/classification/model/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/classification/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/classification/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/classification/model/classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.354095 antgo-0.1.3/antgo/framework/helper/models/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.354095 antgo-0.1.3/antgo/framework/helper/models/detectors/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.354095 antgo-0.1.3/antgo/framework/helper/models/detectors/core/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.358095 antgo-0.1.3/antgo/framework/helper/models/detectors/core/anchor/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/anchor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/anchor/anchor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/anchor/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/anchor/point_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/anchor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.358095 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.362095 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/approx_max_iou_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/assign_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/atss_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/base_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/center_region_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/grid_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/hungarian_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/max_iou_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/point_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/region_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/sim_ota_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/uniform_assigner.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.366095 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/coder/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/coder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/coder/base_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/coder/bucketing_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/coder/delta_xywh_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/coder/distance_point_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/coder/legacy_delta_xywh_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/coder/pseudo_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/coder/tblr_bbox_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/coder/yolo_bbox_coder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.366095 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/iou2d_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.366095 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/match_costs/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/match_costs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/match_costs/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/match_costs/match_cost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.370095 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/combined_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/instance_balanced_pos_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/iou_balanced_neg_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/ohem_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/pseudo_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/sampling_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/score_hlr_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.374095 antgo-0.1.3/antgo/framework/helper/models/detectors/core/mask/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/mask/mask_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    40231 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/mask/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/mask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.374095 antgo-0.1.3/antgo/framework/helper/models/detectors/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/utils/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.374095 antgo-0.1.3/antgo/framework/helper/models/detectors/head/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/head/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/head/base_dense_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    20169 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/head/fcos_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    22430 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/head/focs_head_ml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.382095 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/ae_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/balanced_l1_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/gaussian_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/gfocal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/ghm_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/iou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/kd_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/mse_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/pisa_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/seesaw_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/smooth_l1_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/losses/varifocal_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.382095 antgo-0.1.3/antgo/framework/helper/models/detectors/model/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/model/ttfnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.382095 antgo-0.1.3/antgo/framework/helper/models/detectors/neck/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/neck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/neck/fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/single_stage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.382095 antgo-0.1.3/antgo/framework/helper/models/detectors/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/utils/gaussian_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/utils/util_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/detectors/utils/util_random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.382095 antgo-0.1.3/antgo/framework/helper/models/distillation/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/distillation_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.390096 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/ab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/afd.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/at.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/bss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/cc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/crd.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/dml.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/fitnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/fsp.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/ft.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/hcl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/irg.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/logits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/lwm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/mgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/nst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/ofd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/pkt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/rkd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/sobolev.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/sp.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/st.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/distillation/loss/vid.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/dummy_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/ema_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.390096 antgo-0.1.3/antgo/framework/helper/models/nas/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.390096 antgo-0.1.3/antgo/framework/helper/models/nas/elastic_nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/elastic_nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.394096 antgo-0.1.3/antgo/framework/helper/models/nas/elastic_nn/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/elastic_nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29450 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/elastic_nn/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/model_zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.394096 antgo-0.1.3/antgo/framework/helper/models/nas/ofa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/ofa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.394096 antgo-0.1.3/antgo/framework/helper/models/nas/ofa/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/ofa/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/ofa/baseline/fastdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/ofa/baseline/mobilenet_v3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.394096 antgo-0.1.3/antgo/framework/helper/models/nas/ofa/networks/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/ofa/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/ofa/networks/ofa_fastdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16116 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/ofa/networks/ofa_mbv3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.394096 antgo-0.1.3/antgo/framework/helper/models/nas/ofa/training/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/ofa/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/ofa/training/epoch_based_sampling_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/ofa/training/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/ofa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.398095 antgo-0.1.3/antgo/framework/helper/models/nas/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/search/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.398095 antgo-0.1.3/antgo/framework/helper/models/nas/search/accuracy_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/search/accuracy_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/search/accuracy_predictor/arch_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.398095 antgo-0.1.3/antgo/framework/helper/models/nas/search/efficiency_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/search/efficiency_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/search/efficiency_predictor/latency_lookup_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.398095 antgo-0.1.3/antgo/framework/helper/models/nas/search/search_algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/search/search_algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/search/search_algorithm/evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.402095 antgo-0.1.3/antgo/framework/helper/models/nas/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/tutorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/tutorial/accuracy_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/tutorial/evolution_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15018 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/tutorial/flops_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/tutorial/imagenet_eval_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/tutorial/latency_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.406096 antgo-0.1.3/antgo/framework/helper/models/nas/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/utils/common_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    24233 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/utils/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/utils/my_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/utils/pytorch_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/nas/utils/pytorch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.406096 antgo-0.1.3/antgo/framework/helper/models/pose3d/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/pose3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.406096 antgo-0.1.3/antgo/framework/helper/models/pose3d/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/pose3d/backbone/QNetLite0_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/pose3d/backbone/QNetLite0_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/pose3d/backbone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.410096 antgo-0.1.3/antgo/framework/helper/models/pose3d/head/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/pose3d/head/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/pose3d/head/handpose_qnet_lite0_pose_heatmap2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/pose3d/head/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/pose3d/head/twohand_3dpose_latent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.410096 antgo-0.1.3/antgo/framework/helper/models/pose3d/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/pose3d/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/pose3d/losses/gaussian_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/pose3d/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/pose3d/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.410096 antgo-0.1.3/antgo/framework/helper/models/pose3d/model/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/pose3d/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/pose3d/model/ddr_twohand_pose3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/pose3d/model/keynet_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.410096 antgo-0.1.3/antgo/framework/helper/models/pose3d/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/pose3d/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/proxy_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.410096 antgo-0.1.3/antgo/framework/helper/models/segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.414095 antgo-0.1.3/antgo/framework/helper/models/segmentation/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/segmentation/backbone/DDRQNetLite0.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/segmentation/backbone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.414095 antgo-0.1.3/antgo/framework/helper/models/segmentation/head/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/segmentation/head/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/segmentation/head/aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/segmentation/head/simple_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.414095 antgo-0.1.3/antgo/framework/helper/models/segmentation/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/segmentation/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.414095 antgo-0.1.3/antgo/framework/helper/models/segmentation/model/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/segmentation/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/segmentation/model/encoder_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.418095 antgo-0.1.3/antgo/framework/helper/models/semi/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/semi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/semi/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/semi/detmpl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.418095 antgo-0.1.3/antgo/framework/helper/models/semi/hook/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/semi/hook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/semi/hook/mean_teacher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.418095 antgo-0.1.3/antgo/framework/helper/models/semi/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/semi/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/semi/losses/quality_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/semi/mpl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.426096 antgo-0.1.3/antgo/framework/helper/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10458 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/utils/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/utils/brick_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/utils/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/utils/ckpt_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/utils/conv_upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/utils/csp_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/utils/gaussian_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/utils/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/utils/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/utils/normed_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/utils/panoptic_gt_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/utils/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/utils/res_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/utils/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/utils/structure_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    40231 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/models/utils/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/multi_stream_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.430096 antgo-0.1.3/antgo/framework/helper/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/parallel/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/parallel/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/parallel/data_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/parallel/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/parallel/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/parallel/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/parallel/scatter_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/parallel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.434096 antgo-0.1.3/antgo/framework/helper/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19868 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    27545 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/epoch_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/fp16_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.438096 antgo-0.1.3/antgo/framework/helper/runner/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/closure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)    23377 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/iter_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.442096 antgo-0.1.3/antgo/framework/helper/runner/hooks/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/logger/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/logger/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/logger/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    28500 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/lr_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    24618 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/momentum_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/sampler_seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.442096 antgo-0.1.3/antgo/framework/helper/runner/hooks/samplingmethods/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/samplingmethods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/samplingmethods/kcenter_greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/samplingmethods/sampling_def.py
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/submodules_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/sync_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/hooks/weight_adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/iter_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/log_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.442096 antgo-0.1.3/antgo/framework/helper/runner/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/runner/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/task_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.446096 antgo-0.1.3/antgo/framework/helper/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/tools/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/tools/exp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/tools/export_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/tools/schedule_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/tools/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    27342 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.450096 antgo-0.1.3/antgo/framework/helper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/compat_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    27018 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/device_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/ext_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    19158 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/math_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/parrots_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/util_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/helper/utils/version_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.454096 antgo-0.1.3/antgo/framework/paddle2torch/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/paddle2torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.454096 antgo-0.1.3/antgo/framework/paddle2torch/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/paddle2torch/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/paddle2torch/mapper/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/paddle2torch/mapper/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/paddle2torch/mapper/nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/paddle2torch/mapper/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/paddle2torch/mapper/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.454096 antgo-0.1.3/antgo/framework/paddle2torch/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/paddle2torch/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/paddle2torch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.454096 antgo-0.1.3/antgo/framework/paddle2torch/vision/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/paddle2torch/vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.454096 antgo-0.1.3/antgo/framework/torch2paddle/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.462096 antgo-0.1.3/antgo/framework/torch2paddle/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.462096 antgo-0.1.3/antgo/framework/torch2paddle/mapper/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/cuda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/cuda/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/nn_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/nn_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/nn_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/parambase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.462096 antgo-0.1.3/antgo/framework/torch2paddle/mapper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/mapper/varbase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.466096 antgo-0.1.3/antgo/framework/torch2paddle/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28762 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/tools/ast_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/tools/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/tools/dependency_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.466096 antgo-0.1.3/antgo/framework/torch2paddle/vision/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/vision/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/vision/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/framework/torch2paddle/vision/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24880 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    15294 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/interactcontext.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29822 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20912 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/main_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.478096 antgo-0.1.3/antgo/measures/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2528 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/ali_fashion_attribute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/ali_fashion_landmark_ne.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5903 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/average_precision.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4744 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/binary_c.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1554 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/binomial_deviance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2060 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/confusion_matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21500 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/crowdsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9002 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/deep_analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6339 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/face_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1985 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/kdd_average_precision.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3456 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/matting_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/moving_statistic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4826 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/multi_c.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4348 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/multic_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/multil_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/normalized_error.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    45355 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/objdect_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2826 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/pck.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/person_search_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6784 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/precision_recall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8696 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/quadratic_weighted_kappa.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2438 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/regression_metric.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2765 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/regression_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13252 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/repeat_statistic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      192 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/retrieval_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5448 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/segmentation_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3467 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/significance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7540 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/statistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/topk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/track_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4010 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/measures/yesno_crowdsource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.478096 antgo-0.1.3/antgo/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.482096 antgo-0.1.3/antgo/pipeline/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.482096 antgo-0.1.3/antgo/pipeline/engine/execution/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/engine/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/engine/execution/base_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/engine/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/engine/operator_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/engine/operator_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/engine/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.486096 antgo-0.1.3/antgo/pipeline/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.486096 antgo-0.1.3/antgo/pipeline/functional/common/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/common/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17173 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/data_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/entity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.486096 antgo-0.1.3/antgo/pipeline/functional/image/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/image/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/image/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/image/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.490096 antgo-0.1.3/antgo/pipeline/functional/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/mixins/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/mixins/computer_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/mixins/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/mixins/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/mixins/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/mixins/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/mixins/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/mixins/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/mixins/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/mixins/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/mixins/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/mixins/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/mixins/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/option.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/functional/storages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.490096 antgo-0.1.3/antgo/pipeline/hparam/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/hparam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/hparam/hyperparameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.490096 antgo-0.1.3/antgo/pipeline/hub/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.490096 antgo-0.1.3/antgo/pipeline/hub/builtin/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/hub/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.494096 antgo-0.1.3/antgo/pipeline/hub/builtin/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/hub/builtin/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/hub/builtin/operators/inference_model_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/hub/builtin/operators/inference_onnx_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/hub/builtin/operators/runas_op.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.494096 antgo-0.1.3/antgo/pipeline/hub/external/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/hub/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.494096 antgo-0.1.3/antgo/pipeline/hub/external/mm/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/hub/external/mm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/hub/external/mm/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/hub/external/mm/inpainting.py
--rw-r--r--   0 runner    (1001) docker     (123)    18069 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/hub/external/mm/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/hub/external/mm/pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/hub/external/mm/restoration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/hub/external/mm/segmentor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.494096 antgo-0.1.3/antgo/pipeline/models/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.278095 antgo-0.1.3/antgo/pipeline/models/cfg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.498096 antgo-0.1.3/antgo/pipeline/models/cfg/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/models/cfg/dataset/coco.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.498096 antgo-0.1.3/antgo/pipeline/models/cfg/detector/
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/models/cfg/detector/yolov7-e6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/models/cfg/detector/yolov7-w6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/models/cfg/detector/yolov7.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/models/cfg/detector/yolov7x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.498096 antgo-0.1.3/antgo/pipeline/models/detector/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/models/detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/models/detector/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.498096 antgo-0.1.3/antgo/pipeline/models/detector/yolov7/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/models/detector/yolov7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/models/detector/yolov7/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/models/detector/yolov7/yolov7.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.498096 antgo-0.1.3/antgo/pipeline/models/pose/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/models/pose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.498096 antgo-0.1.3/antgo/pipeline/models/segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/models/segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.502096 antgo-0.1.3/antgo/pipeline/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86819 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/models/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/models/utils/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/models/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.502096 antgo-0.1.3/antgo/pipeline/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/operators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/operators/nop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.502096 antgo-0.1.3/antgo/pipeline/serve/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.502096 antgo-0.1.3/antgo/pipeline/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/pipeline/utils/repo_normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.506096 antgo-0.1.3/antgo/resource/
--rwxr-xr-x   0 runner    (1001) docker     (123)      200 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.506096 antgo-0.1.3/antgo/resource/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.506096 antgo-0.1.3/antgo/resource/app/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/css/359.32c5c11e.css
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/css/385.1759eef9.css
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/css/854.9e012a59.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/css/app.48eb9280.css
--rw-r--r--   0 runner    (1001) docker     (123)   219463 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/css/chunk-vendors.1944359c.css
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.522096 antgo-0.1.3/antgo/resource/app/js/
--rw-r--r--   0 runner    (1001) docker     (123)   182502 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/js/359.afb86915.js
--rw-r--r--   0 runner    (1001) docker     (123)   828443 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/js/359.afb86915.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/js/385.90ba0f66.js
--rw-r--r--   0 runner    (1001) docker     (123)    31358 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/js/385.90ba0f66.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/js/532.f949def3.js
--rw-r--r--   0 runner    (1001) docker     (123)    24678 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/js/532.f949def3.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/js/651.c5601578.js
--rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/js/651.c5601578.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/js/769.b7247054.js
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/js/769.b7247054.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/js/854.d3c0e54f.js
--rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/js/854.d3c0e54f.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/js/880.cba02e88.js
--rw-r--r--   0 runner    (1001) docker     (123)    19810 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/js/880.cba02e88.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/js/app.f01f9b7a.js
--rw-r--r--   0 runner    (1001) docker     (123)    33636 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/js/app.f01f9b7a.js.map
--rw-r--r--   0 runner    (1001) docker     (123)  1289477 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/js/chunk-vendors.18913786.js
--rw-r--r--   0 runner    (1001) docker     (123)  3750898 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/app/js/chunk-vendors.18913786.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.534096 antgo-0.1.3/antgo/resource/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/dataset/3dpw.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/dataset/ade20k.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/dataset/cityscapes.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/dataset/coco.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/dataset/flic.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/dataset/h36m.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/dataset/lfw.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15596 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/dataset/lip.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/dataset/lsp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/dataset/mpii.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/dataset/vgg-face2-data.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/dataset/vgg-face2-meta.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/dataset/voc.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    23363 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/html.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.542096 antgo-0.1.3/antgo/resource/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/static/antgo.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     9662 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/static/antgo.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/static/antgo.js
--rw-r--r--   0 runner    (1001) docker     (123)   236514 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/static/apply.png
--rw-r--r--   0 runner    (1001) docker     (123)   292973 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/static/banner.png
--rw-r--r--   0 runner    (1001) docker     (123)    32806 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/static/card.png
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/static/crowdsource.js
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/static/error.json
--rw-r--r--   0 runner    (1001) docker     (123)    85624 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/static/filetree.png
--rw-r--r--   0 runner    (1001) docker     (123)    32294 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/static/holder.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   106186 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/static/register.png
--rw-r--r--   0 runner    (1001) docker     (123)   244247 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/static/start-experiment.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.550096 antgo-0.1.3/antgo/resource/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/activelearning.html
--rwxr-xr-x   0 runner    (1001) docker     (123)    16328 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/crowdsource.html
--rw-r--r--   0 runner    (1001) docker     (123)    22287 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/demo.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.550096 antgo-0.1.3/antgo/resource/templates/mvp/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.554096 antgo-0.1.3/antgo/resource/templates/mvp/cifar10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.554096 antgo-0.1.3/antgo/resource/templates/mvp/cifar10/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/cifar10/configs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/cifar10/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/cifar10/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    19161 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/cifar10/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/cifar10/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.554096 antgo-0.1.3/antgo/resource/templates/mvp/cifar10/models/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/cifar10/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/cifar10/models/wideres.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/coco_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/install.sh
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/launch.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/lsp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/pascal_voc_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/mvp/visalso_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/project.json
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/sample_gt.json
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/sample_meta.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    61982 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/statistic-report.html
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/task.template
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/task_main_file.template
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/task_main_param.template
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/task_shell.template
--rw-r--r--   0 runner    (1001) docker     (123)    30333 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/trainmaster.html
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/trainworker.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     1867 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/resource/templates/yesno_crowdsource.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.554096 antgo-0.1.3/antgo/sandbox/
--rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/sandbox/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2542 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/sandbox/sandbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.558096 antgo-0.1.3/antgo/script/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/script/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/script/create_dataset_share.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/script/custom_submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/script/data_convert_cifar10_tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/script/data_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/script/local_submit.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/script/ssh-launch.sh
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/script/ssh-submit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/script/ssh-submit.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/script/ssh_submit.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/script/submit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/script/test.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.562096 antgo-0.1.3/antgo/task/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/task/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12291 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/task/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.562096 antgo-0.1.3/antgo/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/tools/browser_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/tools/download_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/tools/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/tools/filter_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25713 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/tools/label_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/tools/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/tools/share_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.574096 antgo-0.1.3/antgo/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      402 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1756 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/_bbox.pyx
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/_encode_png.pyx
--rwxr-xr-x   0 runner    (1001) docker     (123)    11418 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/_mask.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/args.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1150 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/argscope.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/colormap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8104 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/concurrency.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1887 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/cpu.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1242 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/encode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3819 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/fs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2915 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/gpu.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4076 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4553 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/mask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9588 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/netvis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10128 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/parallel_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/pickledb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/processbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/sample_gt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1372 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.574096 antgo-0.1.3/antgo/utils/shared_queue/
--rwxr-xr-x   0 runner    (1001) docker     (123)      992 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/shared_queue/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3163 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/shared_queue/queue.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17513 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/shared_queue/sharedmemory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/timer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3959 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-04-25 02:41:44.000000 antgo-0.1.3/antgo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.286095 antgo-0.1.3/antgo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-25 02:44:25.000000 antgo-0.1.3/antgo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36262 2023-04-25 02:44:25.000000 antgo-0.1.3/antgo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 02:44:25.000000 antgo-0.1.3/antgo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 02:44:25.000000 antgo-0.1.3/antgo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 02:44:25.000000 antgo-0.1.3/antgo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 02:44:25.000000 antgo-0.1.3/antgo.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-04-25 02:41:44.000000 antgo-0.1.3/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-04-25 02:41:44.000000 antgo-0.1.3/roadmap.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 02:44:25.578096 antgo-0.1.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2183 2023-04-25 02:41:44.000000 antgo-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:44:25.578096 antgo-0.1.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-25 02:41:44.000000 antgo-0.1.3/test/test_antgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-25 02:41:44.000000 antgo-0.1.3/test/test_paddle_c.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-25 02:41:44.000000 antgo-0.1.3/test/test_torch_c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.982218 antgo-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/LICENSE.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-04-29 06:53:15.000000 antgo-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-29 06:56:00.978217 antgo-0.1.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4480 2023-04-29 06:53:15.000000 antgo-0.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.638213 antgo-0.1.4/antgo/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.646213 antgo-0.1.4/antgo/ant/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25864 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/activelearning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/activelearning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/activelearning_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9805 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/batch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14101 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/browser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28324 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34652 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22044 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/environment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4162 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/flags.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44521 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/ant/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1711 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/config.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8645 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.654213 antgo-0.1.4/antgo/crowdsource/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      206 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/activelearning_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/base_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12973 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/batch_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43022 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/browser_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6412 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/crowdsource_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27245 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/demo_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15578 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/ensemble_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33823 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/label_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8055 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/crowdsource/watch_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.654213 antgo-0.1.4/antgo/cutils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8249 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/cutils/maskApi.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2176 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/cutils/maskApi.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.654213 antgo-0.1.4/antgo/dataflow/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5412 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/basic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22875 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14235 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.670213 antgo-0.1.4/antgo/dataflow/dataset/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      783 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/ade20k.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14996 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/celeba.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5425 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/cityscape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/clsdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25177 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/coco2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/cusdomcls.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29220 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/empty_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/fashionai_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/fashionai_landmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/flic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3139 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/horse2zebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35327 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16512 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/interhand26M.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3083 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/iphone2dslr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8328 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/lfw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/lip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/lsp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/mpii.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3725 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/omniglot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/parallel_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13131 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/pascal_voc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/proxy_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/queue_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/random_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14554 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4465 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/simpleimages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/simplevideos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/spider_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3559 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/vggface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/dataset/visalso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/datasetio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.670213 antgo-0.1.4/antgo/dataflow/datasynth/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/datasynth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.674214 antgo-0.1.4/antgo/dataflow/imgaug/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1037 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65619 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/autoaugment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46247 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/batch_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/colorspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3274 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25279 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/gridmask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16268 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/op_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/operators_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17718 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/photometric.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10813 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/regular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/imgaug/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21369 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/dataflow/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.678213 antgo-0.1.4/antgo/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.682214 antgo-0.1.4/antgo/framework/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/activelearning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.682214 antgo-0.1.4/antgo/framework/helper/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/apis/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/base_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.682214 antgo-0.1.4/antgo/framework/helper/cnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/alexnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.686214 antgo-0.1.4/antgo/framework/helper/cnn/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/backbone/ddr_lcnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/backbone/ddr_mobilenet_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.694214 antgo-0.1.4/antgo/framework/helper/cnn/bricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/context_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/conv2d_adaptive_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/conv_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/depthwise_separable_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/generalized_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/hsigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/hswish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/non_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/swish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37224 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/bricks/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.698214 antgo-0.1.4/antgo/framework/helper/cnn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/utils/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/utils/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26005 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/utils/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/cnn/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.698214 antgo-0.1.4/antgo/framework/helper/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.698214 antgo-0.1.4/antgo/framework/helper/configs/activelearning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/activelearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/activelearning/ac_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.698214 antgo-0.1.4/antgo/framework/helper/configs/adda/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/adda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/adda/adda_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.698214 antgo-0.1.4/antgo/framework/helper/configs/distillation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/distillation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/distillation/reviewkd_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.702214 antgo-0.1.4/antgo/framework/helper/configs/semi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/semi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/semi/dense_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/semi/detmpl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/configs/semi/mpl_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.702214 antgo-0.1.4/antgo/framework/helper/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/dataset_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/dataset_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/kvdataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.706214 antgo-0.1.4/antgo/framework/helper/dataset/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37456 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/pipelines/auto_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/pipelines/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/pipelines/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29127 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/pipelines/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.710214 antgo-0.1.4/antgo/framework/helper/dataset/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/samplers/class_aware_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/samplers/distributed_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/samplers/group_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/samplers/infinite_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/samplers/kv_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/dataset/tfdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.710214 antgo-0.1.4/antgo/framework/helper/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36707 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.714214 antgo-0.1.4/antgo/framework/helper/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.714214 antgo-0.1.4/antgo/framework/helper/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/metrics/kp2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/metrics/seg2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.718214 antgo-0.1.4/antgo/framework/helper/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.718214 antgo-0.1.4/antgo/framework/helper/models/activelearning/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/activelearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/activelearning/acnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.718214 antgo-0.1.4/antgo/framework/helper/models/adda/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/adda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/adda/adda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.718214 antgo-0.1.4/antgo/framework/helper/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.718214 antgo-0.1.4/antgo/framework/helper/models/classification/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23127 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/backbones/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/backbones/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23751 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/backbones/resnext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.722214 antgo-0.1.4/antgo/framework/helper/models/classification/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/heads/cls_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/heads/stacked_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.722214 antgo-0.1.4/antgo/framework/helper/models/classification/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.722214 antgo-0.1.4/antgo/framework/helper/models/classification/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/classification/model/classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.722214 antgo-0.1.4/antgo/framework/helper/models/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.726214 antgo-0.1.4/antgo/framework/helper/models/detectors/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.726214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.726214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/anchor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/point_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.726214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.734214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/approx_max_iou_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/assign_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/atss_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/base_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/center_region_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/grid_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/hungarian_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/max_iou_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/point_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/region_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/sim_ota_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/uniform_assigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.734214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/base_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/bucketing_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/delta_xywh_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/distance_point_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/legacy_delta_xywh_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/pseudo_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/tblr_bbox_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/yolo_bbox_coder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.738214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/iou2d_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.738214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/match_costs/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/match_costs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/match_costs/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/match_costs/match_cost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.742214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/combined_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/instance_balanced_pos_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/iou_balanced_neg_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/ohem_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/pseudo_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/sampling_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/score_hlr_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.742214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/mask/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/mask/mask_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40231 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/mask/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/mask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.742214 antgo-0.1.4/antgo/framework/helper/models/detectors/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/utils/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.746214 antgo-0.1.4/antgo/framework/helper/models/detectors/head/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/head/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/head/base_dense_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19071 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/head/fcos_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24258 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/head/fcos_head_ml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.750214 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/ae_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/balanced_l1_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/gaussian_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/gfocal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/ghm_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15521 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/iou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/kd_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/mse_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/pisa_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10116 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/seesaw_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/smooth_l1_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/losses/varifocal_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.750214 antgo-0.1.4/antgo/framework/helper/models/detectors/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/model/ttfnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.750214 antgo-0.1.4/antgo/framework/helper/models/detectors/neck/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/neck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/neck/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/single_stage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.754214 antgo-0.1.4/antgo/framework/helper/models/detectors/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/utils/gaussian_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/utils/util_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/detectors/utils/util_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.754214 antgo-0.1.4/antgo/framework/helper/models/distillation/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/distillation_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.762215 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/ab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/afd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/bss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/cc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/crd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/dml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/fitnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/fsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/ft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/hcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/irg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/logits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/lwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/mgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/nst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/ofd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/pkt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/rkd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/sobolev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/sp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/st.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/distillation/loss/vid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/dummy_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/ema_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.762215 antgo-0.1.4/antgo/framework/helper/models/nas/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.762215 antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.762215 antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29450 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/model_zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.766215 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.766215 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/baseline/fastdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/baseline/mobilenet_v3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.766215 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/networks/ofa_fastdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16116 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/networks/ofa_mbv3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.766215 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/training/epoch_based_sampling_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/training/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/ofa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.766215 antgo-0.1.4/antgo/framework/helper/models/nas/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/search/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.770215 antgo-0.1.4/antgo/framework/helper/models/nas/search/accuracy_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/search/accuracy_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/search/accuracy_predictor/arch_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.770215 antgo-0.1.4/antgo/framework/helper/models/nas/search/efficiency_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/search/efficiency_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/search/efficiency_predictor/latency_lookup_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.770215 antgo-0.1.4/antgo/framework/helper/models/nas/search/search_algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/search/search_algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/search/search_algorithm/evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.770215 antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/accuracy_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/evolution_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15018 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/flops_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/imagenet_eval_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/latency_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.774215 antgo-0.1.4/antgo/framework/helper/models/nas/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/utils/common_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24233 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/utils/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/utils/my_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/utils/pytorch_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/nas/utils/pytorch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.774215 antgo-0.1.4/antgo/framework/helper/models/pose3d/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.774215 antgo-0.1.4/antgo/framework/helper/models/pose3d/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/backbone/QNetLite0_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/backbone/QNetLite0_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/backbone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.778215 antgo-0.1.4/antgo/framework/helper/models/pose3d/head/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/head/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/head/handpose_qnet_lite0_pose_heatmap2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/head/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/head/twohand_3dpose_latent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.778215 antgo-0.1.4/antgo/framework/helper/models/pose3d/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/losses/gaussian_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.778215 antgo-0.1.4/antgo/framework/helper/models/pose3d/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/model/ddr_twohand_pose3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/model/keynet_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.778215 antgo-0.1.4/antgo/framework/helper/models/pose3d/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/pose3d/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/proxy_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.778215 antgo-0.1.4/antgo/framework/helper/models/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.782215 antgo-0.1.4/antgo/framework/helper/models/segmentation/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/segmentation/backbone/DDRQNetLite0.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/segmentation/backbone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.782215 antgo-0.1.4/antgo/framework/helper/models/segmentation/head/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/segmentation/head/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/segmentation/head/aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/segmentation/head/simple_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.782215 antgo-0.1.4/antgo/framework/helper/models/segmentation/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/segmentation/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.782215 antgo-0.1.4/antgo/framework/helper/models/segmentation/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/segmentation/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/segmentation/model/encoder_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.782215 antgo-0.1.4/antgo/framework/helper/models/semi/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/semi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/semi/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/semi/detmpl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.782215 antgo-0.1.4/antgo/framework/helper/models/semi/hook/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/semi/hook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/semi/hook/mean_teacher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.786215 antgo-0.1.4/antgo/framework/helper/models/semi/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/semi/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/semi/losses/quality_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/semi/mpl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.790215 antgo-0.1.4/antgo/framework/helper/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10458 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/brick_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/ckpt_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/conv_upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/csp_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/gaussian_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/normed_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/panoptic_gt_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/res_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/structure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40231 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/models/utils/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/multi_stream_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.794215 antgo-0.1.4/antgo/framework/helper/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/parallel/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/parallel/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/parallel/data_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/parallel/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/parallel/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/parallel/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/parallel/scatter_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/parallel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.798215 antgo-0.1.4/antgo/framework/helper/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19868 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27545 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/epoch_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/fp16_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.806215 antgo-0.1.4/antgo/framework/helper/runner/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/closure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23377 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/iter_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.806215 antgo-0.1.4/antgo/framework/helper/runner/hooks/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/logger/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/logger/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/logger/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28452 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/lr_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24618 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/momentum_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/sampler_seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.806215 antgo-0.1.4/antgo/framework/helper/runner/hooks/samplingmethods/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/samplingmethods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/samplingmethods/kcenter_greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/samplingmethods/sampling_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/submodules_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/sync_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/hooks/weight_adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/iter_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/log_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.810215 antgo-0.1.4/antgo/framework/helper/runner/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/runner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/task_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.810215 antgo-0.1.4/antgo/framework/helper/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/tools/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/tools/exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/tools/export_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/tools/schedule_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/tools/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27342 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.818215 antgo-0.1.4/antgo/framework/helper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/compat_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27018 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/device_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/ext_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19158 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/math_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/parrots_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/util_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/helper/utils/version_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.818215 antgo-0.1.4/antgo/framework/paddle2torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.822215 antgo-0.1.4/antgo/framework/paddle2torch/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/mapper/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/mapper/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/mapper/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/mapper/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/mapper/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.822215 antgo-0.1.4/antgo/framework/paddle2torch/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.822215 antgo-0.1.4/antgo/framework/paddle2torch/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/paddle2torch/vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.822215 antgo-0.1.4/antgo/framework/torch2paddle/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.830216 antgo-0.1.4/antgo/framework/torch2paddle/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.830216 antgo-0.1.4/antgo/framework/torch2paddle/mapper/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/cuda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/cuda/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/nn_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/nn_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/nn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/parambase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.830216 antgo-0.1.4/antgo/framework/torch2paddle/mapper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/mapper/varbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.830216 antgo-0.1.4/antgo/framework/torch2paddle/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28762 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/tools/ast_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/tools/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/tools/dependency_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.834215 antgo-0.1.4/antgo/framework/torch2paddle/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/vision/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/vision/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/framework/torch2paddle/vision/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24880 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15294 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/interactcontext.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29822 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20912 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/main_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.846216 antgo-0.1.4/antgo/measures/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2528 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/ali_fashion_attribute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/ali_fashion_landmark_ne.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5903 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/average_precision.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4744 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/binary_c.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1554 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/binomial_deviance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2060 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/confusion_matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21500 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/crowdsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9002 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/deep_analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6339 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/face_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1985 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/kdd_average_precision.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3456 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/matting_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/moving_statistic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4826 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/multi_c.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4348 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/multic_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/multil_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/normalized_error.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45355 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/objdect_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2826 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/pck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/person_search_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6784 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/precision_recall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8696 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/quadratic_weighted_kappa.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2438 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/regression_metric.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2765 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/regression_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13252 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/repeat_statistic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      192 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/retrieval_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5448 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/segmentation_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3467 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/significance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7540 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/track_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4010 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/measures/yesno_crowdsource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.846216 antgo-0.1.4/antgo/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.850216 antgo-0.1.4/antgo/pipeline/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.850216 antgo-0.1.4/antgo/pipeline/engine/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/engine/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/engine/execution/base_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/engine/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/engine/operator_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/engine/operator_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/engine/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.850216 antgo-0.1.4/antgo/pipeline/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.850216 antgo-0.1.4/antgo/pipeline/functional/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/common/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17173 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/data_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/entity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.854216 antgo-0.1.4/antgo/pipeline/functional/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/image/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/image/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/image/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.862216 antgo-0.1.4/antgo/pipeline/functional/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/computer_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/mixins/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/functional/storages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.862216 antgo-0.1.4/antgo/pipeline/hparam/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hparam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hparam/hyperparameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.862216 antgo-0.1.4/antgo/pipeline/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.862216 antgo-0.1.4/antgo/pipeline/hub/builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.862216 antgo-0.1.4/antgo/pipeline/hub/builtin/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/builtin/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/builtin/operators/inference_model_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/builtin/operators/inference_onnx_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/builtin/operators/runas_op.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.866216 antgo-0.1.4/antgo/pipeline/hub/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.870216 antgo-0.1.4/antgo/pipeline/hub/external/mm/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/external/mm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/external/mm/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/external/mm/inpainting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18069 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/external/mm/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/external/mm/pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/external/mm/restoration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/hub/external/mm/segmentor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.870216 antgo-0.1.4/antgo/pipeline/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.630213 antgo-0.1.4/antgo/pipeline/models/cfg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.870216 antgo-0.1.4/antgo/pipeline/models/cfg/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/cfg/dataset/coco.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.870216 antgo-0.1.4/antgo/pipeline/models/cfg/detector/
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/cfg/detector/yolov7-e6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/cfg/detector/yolov7-w6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/cfg/detector/yolov7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/cfg/detector/yolov7x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.870216 antgo-0.1.4/antgo/pipeline/models/detector/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/detector/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.874216 antgo-0.1.4/antgo/pipeline/models/detector/yolov7/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/detector/yolov7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/detector/yolov7/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/detector/yolov7/yolov7.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.874216 antgo-0.1.4/antgo/pipeline/models/pose/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/pose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.874216 antgo-0.1.4/antgo/pipeline/models/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.878216 antgo-0.1.4/antgo/pipeline/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86819 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/utils/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/models/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.878216 antgo-0.1.4/antgo/pipeline/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/operators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/operators/nop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.878216 antgo-0.1.4/antgo/pipeline/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.878216 antgo-0.1.4/antgo/pipeline/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/pipeline/utils/repo_normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.878216 antgo-0.1.4/antgo/resource/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      200 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.882216 antgo-0.1.4/antgo/resource/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.882216 antgo-0.1.4/antgo/resource/app/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/css/359.32c5c11e.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/css/385.1759eef9.css
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/css/854.9e012a59.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/css/app.48eb9280.css
+-rw-r--r--   0 runner    (1001) docker     (123)   219463 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/css/chunk-vendors.1944359c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.898216 antgo-0.1.4/antgo/resource/app/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   182502 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/359.afb86915.js
+-rw-r--r--   0 runner    (1001) docker     (123)   828443 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/359.afb86915.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/385.90ba0f66.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31358 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/385.90ba0f66.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/532.f949def3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24678 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/532.f949def3.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/651.c5601578.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/651.c5601578.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/769.b7247054.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/769.b7247054.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/854.d3c0e54f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/854.d3c0e54f.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/880.cba02e88.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19810 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/880.cba02e88.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/app.f01f9b7a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33636 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/app.f01f9b7a.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)  1289477 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/chunk-vendors.18913786.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3750898 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/app/js/chunk-vendors.18913786.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.918217 antgo-0.1.4/antgo/resource/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/3dpw.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/ade20k.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/cityscapes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/coco.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/flic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/h36m.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/lfw.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15596 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/lip.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/lsp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/mpii.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/vgg-face2-data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/vgg-face2-meta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/dataset/voc.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23363 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.926217 antgo-0.1.4/antgo/resource/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/antgo.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9662 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/antgo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/antgo.js
+-rw-r--r--   0 runner    (1001) docker     (123)   236514 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/apply.png
+-rw-r--r--   0 runner    (1001) docker     (123)   292973 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/banner.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32806 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/card.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/crowdsource.js
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/error.json
+-rw-r--r--   0 runner    (1001) docker     (123)    85624 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/filetree.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32294 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/holder.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   106186 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/register.png
+-rw-r--r--   0 runner    (1001) docker     (123)   244247 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/static/start-experiment.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.938217 antgo-0.1.4/antgo/resource/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/activelearning.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16328 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/crowdsource.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22287 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/demo.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.942217 antgo-0.1.4/antgo/resource/templates/mvp/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.946217 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.946217 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19161 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.950217 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/cifar10/models/wideres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/coco_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/install.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/launch.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/lsp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/pascal_voc_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/mvp/visalso_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/project.json
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/sample_gt.json
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/sample_meta.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    61982 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/statistic-report.html
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/task.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/task_main_file.template
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/task_main_param.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/task_shell.template
+-rw-r--r--   0 runner    (1001) docker     (123)    30333 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/trainmaster.html
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/trainworker.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1867 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/resource/templates/yesno_crowdsource.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.950217 antgo-0.1.4/antgo/sandbox/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/sandbox/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2542 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/sandbox/sandbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.958217 antgo-0.1.4/antgo/script/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/create_dataset_share.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/custom_submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/data_convert_cifar10_tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/data_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/local_submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/ssh-launch.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/ssh-submit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/ssh-submit.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/ssh_submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/submit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/script/test.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.958217 antgo-0.1.4/antgo/task/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/task/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12291 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/task/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.962217 antgo-0.1.4/antgo/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/tools/browser_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/tools/download_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/tools/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/tools/filter_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25713 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/tools/label_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/tools/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/tools/share_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.974218 antgo-0.1.4/antgo/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      402 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1756 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/_bbox.pyx
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/_encode_png.pyx
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11418 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/_mask.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/args.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1150 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/argscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/colormap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8104 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/concurrency.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1887 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/cpu.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1242 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/encode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3819 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/fs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2915 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/gpu.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4076 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4553 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/mask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9588 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/netvis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10128 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/parallel_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/pickledb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/processbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/sample_gt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1372 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.978217 antgo-0.1.4/antgo/utils/shared_queue/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      992 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/shared_queue/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3163 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/shared_queue/queue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17513 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/shared_queue/sharedmemory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3959 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-04-29 06:53:15.000000 antgo-0.1.4/antgo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.638213 antgo-0.1.4/antgo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-29 06:56:00.000000 antgo-0.1.4/antgo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36262 2023-04-29 06:56:00.000000 antgo-0.1.4/antgo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 06:56:00.000000 antgo-0.1.4/antgo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-29 06:56:00.000000 antgo-0.1.4/antgo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 06:56:00.000000 antgo-0.1.4/antgo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 06:56:00.000000 antgo-0.1.4/antgo.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-04-29 06:53:15.000000 antgo-0.1.4/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-04-29 06:53:15.000000 antgo-0.1.4/roadmap.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 06:56:00.982218 antgo-0.1.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2183 2023-04-29 06:53:15.000000 antgo-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:56:00.978217 antgo-0.1.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-29 06:53:15.000000 antgo-0.1.4/test/test_antgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-29 06:53:15.000000 antgo-0.1.4/test/test_paddle_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-29 06:53:15.000000 antgo-0.1.4/test/test_torch_c.py
```

### Comparing `antgo-0.1.3/PKG-INFO` & `antgo-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antgo
-Version: 0.1.3
+Version: 0.1.4
 Summary: machine learning experiment platform
 Home-page: https://github.com/jianzfb/antgo
 Author: jian
 Author-email: jian@mltalker.com
 License-File: LICENSE.md
 
 ======================
```

### Comparing `antgo-0.1.3/README.rst` & `antgo-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/ant/activelearning.py` & `antgo-0.1.4/antgo/ant/activelearning.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/ant/activelearning_api.py` & `antgo-0.1.4/antgo/ant/activelearning_api.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/ant/activelearning_v2.py` & `antgo-0.1.4/antgo/ant/activelearning_v2.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/ant/base.py` & `antgo-0.1.4/antgo/ant/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/ant/batch.py` & `antgo-0.1.4/antgo/ant/batch.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/ant/browser.py` & `antgo-0.1.4/antgo/ant/browser.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/ant/challenge.py` & `antgo-0.1.4/antgo/ant/challenge.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/ant/client.py` & `antgo-0.1.4/antgo/ant/client.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/ant/debug.py` & `antgo-0.1.4/antgo/ant/debug.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/ant/demo.py` & `antgo-0.1.4/antgo/ant/demo.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/ant/download.py` & `antgo-0.1.4/antgo/ant/download.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/ant/ensemble.py` & `antgo-0.1.4/antgo/ant/ensemble.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/ant/environment.py` & `antgo-0.1.4/antgo/ant/environment.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/ant/flags.py` & `antgo-0.1.4/antgo/ant/flags.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/ant/train.py` & `antgo-0.1.4/antgo/ant/train.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/ant/utils.py` & `antgo-0.1.4/antgo/ant/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/ant/watch.py` & `antgo-0.1.4/antgo/ant/watch.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/config.py` & `antgo-0.1.4/antgo/config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/context.py` & `antgo-0.1.4/antgo/context.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/crowdsource/activelearning_server.py` & `antgo-0.1.4/antgo/crowdsource/activelearning_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/crowdsource/base_server.py` & `antgo-0.1.4/antgo/crowdsource/base_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/crowdsource/batch_server.py` & `antgo-0.1.4/antgo/crowdsource/batch_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/crowdsource/browser_server.py` & `antgo-0.1.4/antgo/crowdsource/browser_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/crowdsource/crowdsource_server.py` & `antgo-0.1.4/antgo/crowdsource/crowdsource_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/crowdsource/demo_server.py` & `antgo-0.1.4/antgo/crowdsource/demo_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/crowdsource/ensemble_server.py` & `antgo-0.1.4/antgo/crowdsource/ensemble_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/crowdsource/label_server.py` & `antgo-0.1.4/antgo/crowdsource/label_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/crowdsource/utils.py` & `antgo-0.1.4/antgo/crowdsource/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/crowdsource/watch_server.py` & `antgo-0.1.4/antgo/crowdsource/watch_server.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/cutils/maskApi.c` & `antgo-0.1.4/antgo/cutils/maskApi.c`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/cutils/maskApi.h` & `antgo-0.1.4/antgo/cutils/maskApi.h`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/basic.py` & `antgo-0.1.4/antgo/dataflow/basic.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/common.py` & `antgo-0.1.4/antgo/dataflow/common.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/core.py` & `antgo-0.1.4/antgo/dataflow/core.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/__init__.py` & `antgo-0.1.4/antgo/dataflow/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/ade20k.py` & `antgo-0.1.4/antgo/dataflow/dataset/ade20k.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/celeba.py` & `antgo-0.1.4/antgo/dataflow/dataset/celeba.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/cifar.py` & `antgo-0.1.4/antgo/dataflow/dataset/cifar.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/cityscape.py` & `antgo-0.1.4/antgo/dataflow/dataset/cityscape.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/clsdataset.py` & `antgo-0.1.4/antgo/dataflow/dataset/clsdataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/coco2017.py` & `antgo-0.1.4/antgo/dataflow/dataset/coco2017.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/cusdomcls.py` & `antgo-0.1.4/antgo/dataflow/dataset/cusdomcls.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/dataset.py` & `antgo-0.1.4/antgo/dataflow/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/empty_dataset.py` & `antgo-0.1.4/antgo/dataflow/dataset/empty_dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/fashionai_attribute.py` & `antgo-0.1.4/antgo/dataflow/dataset/fashionai_attribute.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/fashionai_landmark.py` & `antgo-0.1.4/antgo/dataflow/dataset/fashionai_landmark.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/flic.py` & `antgo-0.1.4/antgo/dataflow/dataset/flic.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/horse2zebra.py` & `antgo-0.1.4/antgo/dataflow/dataset/horse2zebra.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/imagenet.py` & `antgo-0.1.4/antgo/dataflow/dataset/imagenet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/interhand26M.py` & `antgo-0.1.4/antgo/dataflow/dataset/interhand26M.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/iphone2dslr.py` & `antgo-0.1.4/antgo/dataflow/dataset/iphone2dslr.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/lfw.py` & `antgo-0.1.4/antgo/dataflow/dataset/lfw.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/lip.py` & `antgo-0.1.4/antgo/dataflow/dataset/lip.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/lsp.py` & `antgo-0.1.4/antgo/dataflow/dataset/lsp.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/mnist.py` & `antgo-0.1.4/antgo/dataflow/dataset/mnist.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/mpii.py` & `antgo-0.1.4/antgo/dataflow/dataset/mpii.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/omniglot.py` & `antgo-0.1.4/antgo/dataflow/dataset/omniglot.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/parallel_read.py` & `antgo-0.1.4/antgo/dataflow/dataset/parallel_read.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/pascal_voc.py` & `antgo-0.1.4/antgo/dataflow/dataset/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/proxy_dataset.py` & `antgo-0.1.4/antgo/dataflow/dataset/proxy_dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/queue_dataset.py` & `antgo-0.1.4/antgo/dataflow/dataset/queue_dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/random_dataset.py` & `antgo-0.1.4/antgo/dataflow/dataset/random_dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/reader.py` & `antgo-0.1.4/antgo/dataflow/dataset/reader.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/simpleimages.py` & `antgo-0.1.4/antgo/dataflow/dataset/simpleimages.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/simplevideos.py` & `antgo-0.1.4/antgo/dataflow/dataset/simplevideos.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/spider_dataset.py` & `antgo-0.1.4/antgo/dataflow/dataset/spider_dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/vggface.py` & `antgo-0.1.4/antgo/dataflow/dataset/vggface.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/dataset/visalso.py` & `antgo-0.1.4/antgo/dataflow/dataset/visalso.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/datasetio.py` & `antgo-0.1.4/antgo/dataflow/datasetio.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/imgaug/autoaugment_utils.py` & `antgo-0.1.4/antgo/dataflow/imgaug/autoaugment_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/imgaug/batch_operators.py` & `antgo-0.1.4/antgo/dataflow/imgaug/batch_operators.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/imgaug/colorspace.py` & `antgo-0.1.4/antgo/dataflow/imgaug/colorspace.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/imgaug/functional.py` & `antgo-0.1.4/antgo/dataflow/imgaug/functional.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/imgaug/geometric.py` & `antgo-0.1.4/antgo/dataflow/imgaug/geometric.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/imgaug/gridmask_utils.py` & `antgo-0.1.4/antgo/dataflow/imgaug/gridmask_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/imgaug/op_helper.py` & `antgo-0.1.4/antgo/dataflow/imgaug/op_helper.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/imgaug/operators.py` & `antgo-0.1.4/antgo/dataflow/imgaug/operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import absolute_import
 from __future__ import print_function
 from __future__ import division
-
 try:
     from collections.abc import Sequence
 except Exception:
     from collections import Sequence
 
 from numbers import Number
 
@@ -69,15 +68,15 @@
         image = sample['image']
         sample.pop('image')
         return image, sample
 
 
 # FINISH FIX
 class DecodeImage(BaseOperator):
-    def __init__(self, to_rgb=True, with_mixup=False, with_cutmix=False, backend="cv", inputs=None):
+    def __init__(self, to_rgb=False, with_mixup=False, with_cutmix=False, backend="cv", inputs=None):
         """ Transform the image data to numpy format.
         Args:
             to_rgb (bool): whether to convert BGR to RGB
             with_mixup (bool): whether or not to mixup image and gt_bbbox/gt_score
             with_cutmix (bool): whether or not to cutmix image and gt_bbbox/gt_score
         """
 
@@ -634,21 +633,25 @@
 
 
 # FINISH FIX
 class Rotation(BaseOperator):
     """
     Rotate the image with bounding box
     """
-    def __init__(self, degree=30, border_value=[0, 0, 0], label_border_value=255,inputs=None):
+    def __init__(self, degree=30, border_value=[0, 0, 0], label_border_value=255, prob=0.5, inputs=None):
         super(Rotation, self).__init__(inputs=inputs)
         self._degree = degree
         self._border_value = border_value
         self._label_border_value = label_border_value
+        self.prob = prob
 
     def __call__(self, sample, context=None):
+        if np.random.random() > self.prob:
+            return sample
+
         im = sample['image']
         height, width = im.shape[:2]
         cx, cy = width // 2, height // 2
         angle = np.random.randint(0, self._degree * 2) - self._degree
         rot_mat = cv2.getRotationMatrix2D((cx, cy), angle, 1.0)
         image_rotated = cv2.warpAffine(
                 src=im,
@@ -882,14 +885,42 @@
 
         sample['bboxes'] = gt_bbox
         sample['image'] = im
         return sample
 
 
 # FINISH FIX
+class CorrectBoxes(BaseOperator):
+    """
+        修正bboxes错误(bboxes的标注有时存在问题)
+    """
+    def __init__(self, is_normalized=False, inputs=None):
+        super().__init__(inputs=inputs)
+        self.is_normalized = is_normalized
+    
+    def __call__(self, sample, context=None):
+        if 'bboxes' not in sample:
+            return sample
+
+        h, w = sample['image'].shape[:2]
+        min_x = np.minimum(sample['bboxes'][:,0:1], sample['bboxes'][:,2:3])
+        min_y = np.minimum(sample['bboxes'][:,1:2], sample['bboxes'][:,3:4])
+        max_x = np.maximum(sample['bboxes'][:,0:1], sample['bboxes'][:,2:3])
+        max_y = np.maximum(sample['bboxes'][:,1:2], sample['bboxes'][:,3:4])
+        sample['bboxes'] = np.concatenate([min_x, min_y, max_x, max_y], -1)
+        
+        if self.is_normalized:
+            sample['bboxes'] = np.clip(sample['bboxes'], 0, 1)
+        else:
+            sample['bboxes'][:,0::2] = np.clip(sample['bboxes'][:,0::2], 0, w)
+            sample['bboxes'][:,1::2] = np.clip(sample['bboxes'][:,1::2], 0, h)
+        return sample
+
+
+# FINISH FIX
 class RandomFlipImage(BaseOperator):
     def __init__(self, 
                 prob=0.5, 
                 is_normalized=False,
                 swap_ids=[[1,3,19,5,7,9,11,13,15],[2,4,20,6,8,10,12,14,16]], 
                 swap_labels=[[0,1],[1,0]],
                 inputs=None):
@@ -1226,17 +1257,17 @@
         for id in range(count):
             im = ops[id](im)
         sample['image'] = im
         return sample
 
 
 # FINISH FIX(?)
-class CropImage(BaseOperator):
+class RandomCropImageV2(BaseOperator):
     # 已经完成验证
-    def __init__(self, prob=0.5, batch_sampler=[[1, 50, 0.3, 1.0, 0.5, 2.0, 0.3, 1.0]], satisfy_all=False, avoid_no_bbox=True, inputs=None):
+    def __init__(self, batch_sampler=[[1, 50, 0.3, 1.0, 0.5, 2.0, 0.3, 1.0]], satisfy_all=False, avoid_no_bbox=True, prob=0.5, inputs=None):
         """
         Args:
             batch_sampler (list): Multiple sets of different
                                   parameters for cropping.
             satisfy_all (bool): whether all boxes must satisfy.
             e.g.[[1, 1, 1.0, 1.0, 1.0, 1.0, 0.0, 1.0],
                  [1, 50, 0.3, 1.0, 0.5, 2.0, 0.1, 1.0],
@@ -1247,15 +1278,15 @@
                  [1, 50, 0.3, 1.0, 0.5, 2.0, 0.0, 1.0]]
            [max sample, max trial, min scale, max scale,
             min aspect ratio, max aspect ratio,
             min overlap, max overlap]
             avoid_no_bbox (bool): whether to to avoid the
                                   situation where the box does not appear.
         """
-        super(CropImage, self).__init__(inputs=inputs)
+        super(RandomCropImageV2, self).__init__(inputs=inputs)
         self.batch_sampler = batch_sampler
         self.satisfy_all = satisfy_all
         self.avoid_no_bbox = avoid_no_bbox
         self.prob = prob
 
     def rotate_2d(self, pt_2d, rot_rad):
         x = pt_2d[0]
@@ -1315,17 +1346,14 @@
             return sample
 
         assert 'image' in sample, "image data not found"
         im = sample['image']
         gt_bbox = sample['bboxes']
         gt_class = sample['labels']
         im_height, im_width = im.shape[:2]
-        # gt_score = None
-        # if 'gt_score' in sample:
-        #     gt_score = sample['gt_score']
 
         sampled_bbox = []
         for sampler in self.batch_sampler:
             found = 0
             for i in range(sampler[1]):
                 if found >= sampler[0]:
                     break
@@ -1385,14 +1413,108 @@
                 crop_trans = np.matmul(crop_trans, base_trans)
                 sample['image_meta']['transform_matrix'] = crop_trans
 
             return sample
         return sample
 
 
+class RandomCropImageV1(BaseOperator):
+    def __init__(self, size, padding, fill, prob=0.5, inputs=None):
+        super(RandomCropImageV1, self).__init__(inputs=inputs)
+        self.size = size    # width, height
+        self.padding = padding if isinstance(padding, tuple) else (padding, padding, padding, padding)
+        self.fill = fill
+        self.prob = prob
+
+    def __call__(self, sample, context=None):
+        if np.random.random() > self.prob:
+            return sample
+        image = sample['image']
+
+        # 添加padding
+        padding_top = self.padding[0]
+        padding_left = self.padding[2]
+        image = cv2.copyMakeBorder(
+            image, self.padding[0], self.padding[1], self.padding[2], self.padding[2], cv2.BORDER_CONSTANT, value=self.fill)
+        if 'segments' in sample and sample['segments'].size != 0:
+            # 无效位置填充255
+            sample['segments'] = cv2.copyMakeBorder(
+                sample['segments'], self.padding[0], self.padding[1], self.padding[2], self.padding[2], cv2.BORDER_CONSTANT, value=255)
+
+        height, width = image.shape[:2]
+        if width < self.size[0]:
+            image = cv2.copyMakeBorder(
+                image, 0, 0, self.size[0]-width, 0, cv2.BORDER_CONSTANT, value=self.fill)
+            padding_left += (self.size[0]-width)
+            if 'segments' in sample and sample['segments'].size != 0:
+                # 无效位置填充255
+                sample['segments'] = cv2.copyMakeBorder(
+                    sample['segments'], 0, 0, self.size[0]-width, 0, cv2.BORDER_CONSTANT, value=255)
+
+        if height < self.size[1]:
+            image = cv2.copyMakeBorder(
+                image, self.size[1]-height, 0, 0, 0, cv2.BORDER_CONSTANT, value=self.fill)
+            padding_top += (self.size[1]-height)
+            if 'segments' in sample and sample['segments'].size != 0:
+                # 无效位置填充255
+                sample['segments'] = cv2.copyMakeBorder(
+                    sample['segments'], self.size[1]-height, 0, 0, 0, cv2.BORDER_CONSTANT, value=255)
+
+        height, width = image.shape[:2]
+
+        xmin = np.random.randint(0, width-self.size[0] if width > self.size[0] else 1)
+        ymin = np.random.randint(0, height-self.size[1] if height > self.size[1] else 1)
+        crop_image = image[ymin:ymin+self.size[1], xmin:xmin+self.size[0]].copy()
+        sample['image'] = crop_image
+        if 'segments' in sample and sample['segments'].size != 0:
+            crop_segments = sample['segments'][ymin:ymin+self.size[1], xmin:xmin+self.size[0]].copy()
+            sample['segments'] = crop_segments
+
+        x_offset = padding_top - xmin
+        y_offset = padding_left - ymin
+        valid = None
+        if 'bboxes' in sample:
+            # Nx4
+            boxes = sample['bboxes'] + np.array([[x_offset, y_offset, x_offset, y_offset]])
+
+            boxes[:,0::2] = np.clip(boxes[:,0::2], 0, self.size[0])
+            boxes[:,1::2] = np.clip(boxes[:,1::2], 0, self.size[1])
+    
+            # filter boxes with no area
+            area = np.prod(boxes[..., 2:] - boxes[..., :2], axis=1)
+            valid = (area > 1.).nonzero()[0]
+            sample['bboxes'] = boxes[valid]
+            sample['labels'] = sample['labels'][valid]            
+
+        if 'joints2d' in sample:
+            # NxJOINT_NUMx2
+            joints2d = sample['joints2d'] + np.array([[[x_offset, y_offset]]])
+
+            if valid is not None:
+                # 挑选出有效joints2d (与bboxes对齐)
+                joints2d = joints2d[valid]
+
+            joints_vis = sample['joints_vis']
+            invalid_p =  joints2d[:,0] < 0 or joints2d[:,0] > self.size[0] or joints2d[:,1] < 0 or joints2d[:,1] > self.size[1]
+            joints_vis[invalid_p] = 0
+            if valid is not None:
+                # 挑选出有效joints_vis (与bboxes对齐)
+                joints_vis = joints_vis[valid]
+            sample['joints_vis'] = joints_vis
+
+            joints2d[:,:,0] = np.clip(joints2d[:,:,0], 0, self.size[0])
+            joints2d[:,:,1] = np.clip(joints2d[:,:,1], 0, self.size[1])
+            sample['joints2d'] = joints2d
+
+        if 'image_meta' in sample:
+            sample['image_meta']['image_shape'] = (crop_image.shape[0], crop_image.shape[1])
+
+        return sample
+
+
 # FINISH FIX
 class NormalizeBox(BaseOperator):
     # FINISH CORRET (JIAN)
     # only for det task
     """Transform the bounding box's coornidates to [0,1]."""
 
     def __init__(self, inputs=None):
@@ -1750,14 +1872,16 @@
                 self.interp_dict.keys()))
 
         self.interp = interp  # 'RANDOM' for yolov3
 
     def __call__(self, sample, context=None):
         w = sample['image'].shape[1]
         h = sample['image'].shape[0]
+        if w == self.target_dim[0] and h == self.target_dim[1]:
+            return sample
 
         if self.interp == "RANDOM":
             interp = random.choice(list(self.interp_dict.keys()))
         else:
             interp = self.interp
 
         resize_w, resize_h = self.target_dim
@@ -1799,16 +1923,14 @@
         sample['width'] = resize_w
         sample['image'] = cv2.resize(
             sample['image'], (resize_w, resize_h), interpolation=self.interp_dict[interp])
         
         if 'image_2' in sample:
             sample['image_2'] = cv2.resize(
                 sample['image_2'], (resize_w, resize_h), interpolation=self.interp_dict[interp])
-
-        # vis_2d_boxes_in_image(sample['image'], sample['bboxes'],sample['labels'], './b.png')
         return sample
 
     
 # FINSH FIX
 class ColorDistort(BaseOperator):
     """Random color distortion.
     Args:
```

### Comparing `antgo-0.1.3/antgo/dataflow/imgaug/operators_3d.py` & `antgo-0.1.4/antgo/dataflow/imgaug/operators_3d.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/imgaug/photometric.py` & `antgo-0.1.4/antgo/dataflow/imgaug/photometric.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/imgaug/regular.py` & `antgo-0.1.4/antgo/dataflow/imgaug/regular.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/imgaug/util.py` & `antgo-0.1.4/antgo/dataflow/imgaug/util.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/recorder.py` & `antgo-0.1.4/antgo/dataflow/recorder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/dataflow/vis.py` & `antgo-0.1.4/antgo/dataflow/vis.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/activelearning.py` & `antgo-0.1.4/antgo/framework/helper/activelearning.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/apis/train.py` & `antgo-0.1.4/antgo/framework/helper/apis/train.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/base_module.py` & `antgo-0.1.4/antgo/framework/helper/base_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/base_trainer.py` & `antgo-0.1.4/antgo/framework/helper/base_trainer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/__init__.py` & `antgo-0.1.4/antgo/framework/helper/cnn/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/alexnet.py` & `antgo-0.1.4/antgo/framework/helper/cnn/alexnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/backbone/ddr_lcnet.py` & `antgo-0.1.4/antgo/framework/helper/cnn/backbone/ddr_lcnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/backbone/ddr_mobilenet_v2.py` & `antgo-0.1.4/antgo/framework/helper/cnn/backbone/ddr_mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/__init__.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/activation.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/activation.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/context_block.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/context_block.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/conv.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/conv.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/conv2d_adaptive_padding.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/conv2d_adaptive_padding.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/conv_module.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/conv_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/conv_ws.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/conv_ws.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/depthwise_separable_conv_module.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/drop.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/generalized_attention.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/generalized_attention.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/hsigmoid.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/hsigmoid.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/hswish.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/hswish.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/inverted_residual.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/make_divisible.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/make_divisible.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/non_local.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/non_local.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/norm.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/norm.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/padding.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/padding.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/plugin.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/plugin.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/registry.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/registry.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/scale.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/scale.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/se_layer.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/se_layer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/transformer.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/transformer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/upsample.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/upsample.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/waterfall.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/waterfall.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/bricks/wrappers.py` & `antgo-0.1.4/antgo/framework/helper/cnn/bricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/resnet.py` & `antgo-0.1.4/antgo/framework/helper/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/utils/__init__.py` & `antgo-0.1.4/antgo/framework/helper/cnn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/utils/flops_counter.py` & `antgo-0.1.4/antgo/framework/helper/cnn/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/utils/fuse_conv_bn.py` & `antgo-0.1.4/antgo/framework/helper/cnn/utils/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/utils/sync_bn.py` & `antgo-0.1.4/antgo/framework/helper/cnn/utils/sync_bn.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/utils/weight_init.py` & `antgo-0.1.4/antgo/framework/helper/cnn/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/cnn/vgg.py` & `antgo-0.1.4/antgo/framework/helper/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/configs/activelearning/ac_config.py` & `antgo-0.1.4/antgo/framework/helper/configs/activelearning/ac_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/configs/adda/adda_config.py` & `antgo-0.1.4/antgo/framework/helper/configs/adda/adda_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/configs/distillation/reviewkd_config.py` & `antgo-0.1.4/antgo/framework/helper/configs/distillation/reviewkd_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/configs/semi/dense_config.py` & `antgo-0.1.4/antgo/framework/helper/configs/semi/dense_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/configs/semi/mpl_config.py` & `antgo-0.1.4/antgo/framework/helper/configs/semi/mpl_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/dataset/__init__.py` & `antgo-0.1.4/antgo/framework/helper/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/dataset/builder.py` & `antgo-0.1.4/antgo/framework/helper/dataset/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/dataset/dataset_filter.py` & `antgo-0.1.4/antgo/framework/helper/dataset/dataset_filter.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/dataset/dataset_split.py` & `antgo-0.1.4/antgo/framework/helper/dataset/dataset_split.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/dataset/dataset_wrappers.py` & `antgo-0.1.4/antgo/framework/helper/dataset/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/dataset/kvdataset.py` & `antgo-0.1.4/antgo/framework/helper/dataset/kvdataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/dataset/pipelines/auto_augment.py` & `antgo-0.1.4/antgo/framework/helper/dataset/pipelines/auto_augment.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/dataset/pipelines/builder.py` & `antgo-0.1.4/antgo/framework/helper/dataset/pipelines/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/dataset/pipelines/formatting.py` & `antgo-0.1.4/antgo/framework/helper/dataset/pipelines/formatting.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/dataset/pipelines/transforms.py` & `antgo-0.1.4/antgo/framework/helper/dataset/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/dataset/samplers/__init__.py` & `antgo-0.1.4/antgo/framework/helper/dataset/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/dataset/samplers/class_aware_sampler.py` & `antgo-0.1.4/antgo/framework/helper/dataset/samplers/class_aware_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/dataset/samplers/distributed_sampler.py` & `antgo-0.1.4/antgo/framework/helper/dataset/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/dataset/samplers/group_sampler.py` & `antgo-0.1.4/antgo/framework/helper/dataset/samplers/group_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/dataset/samplers/infinite_sampler.py` & `antgo-0.1.4/antgo/framework/helper/dataset/samplers/infinite_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/dataset/samplers/kv_sampler.py` & `antgo-0.1.4/antgo/framework/helper/dataset/samplers/kv_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/dataset/tfdataset.py` & `antgo-0.1.4/antgo/framework/helper/dataset/tfdataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from email.utils import localtime
 import logging
 import sys
 import numpy as np
 import torch
 import torch.distributed as dist
 from antgo.framework.helper.utils import build_from_cfg
 from antgo.framework.helper.runner.dist_utils import get_dist_info
 from tfrecord.reader import *
 from tfrecord import iterator_utils
 from antgo.framework.helper.dataset.builder import DATASETS
 import copy
 from antgo.dataflow.datasetio import *
+from antgo.framework.helper.fileio.file_client import *
 import threading
 import json
 from pprint import pprint
 
 
 def _cycle(iterator_fn: typing.Callable) -> typing.Iterable[typing.Any]:
     """Create a repeating iterator from an iterator generator."""
@@ -129,29 +131,66 @@
 
     compression_type: str, optional, default=None
         The type of compression used for the tfrecord. Choose either
         'gzip' or None.
 
     """
     def __init__(self,
-                 data_path_list: typing.List[str],
+                 data_folder,
                  ratios: typing.Union[typing.List[float], None]=None,
                  description: typing.Union[typing.List[str], typing.Dict[str, str], None] = None,
                  shuffle_queue_size: typing.Optional[int] = 1024,
                  pipeline: typing.Optional[typing.List]=None, 
                  weak_pipeline: typing.Optional[typing.List]=None, 
                  strong_pipeline: typing.Optional[typing.List]=None, 
                  sequence_description: typing.Union[typing.List[str], typing.Dict[str, str], None] = None,
                  compression_type: typing.Optional[str] = None,
                  infinite: typing.Optional[bool] = False,
                  inputs_def=None,
                  sample_num_equalizer=True,
                  auto_ext_info=[]) -> None:
         super().__init__()
-        self.data_path_list = data_path_list
+        if data_folder is None:
+            # 不允许data_path_list和data_folder同时不设置
+            logging.error('Must set data_folder')
+            return
+
+        # 自动下载指定数据(仅在首次运行时，进行下载)
+        if ':///' in data_folder:
+            terms = data_folder.split('/')
+            dataset_name = terms[-1]
+            if terms[-1] == '*' or terms[-1] == '':
+                dataset_name = terms[-2]
+
+            # 远程存储，自动下载
+            local_temp_folder = f'./temp_{dataset_name}'
+            if not os.path.exists(local_temp_folder):
+                # 创建临时目录
+                os.makedirs(local_temp_folder)
+
+                # 下载
+                file_client_get(data_folder, local_temp_folder)
+
+        # 替换为本地路径
+        if ':///' in data_folder:
+            terms = data_folder.split('/')
+            dataset_name = terms[-1]
+            if terms[-1] == '*' or terms[-1] == '':
+                dataset_name = terms[-2]
+
+            # 使用本地地址替换
+            data_folder = f'./temp_{dataset_name}'
+
+        # 遍历文件夹，发现所有tfrecord数据
+        self.data_path_list = []
+        for tfrecord_file in os.listdir(data_folder):
+            if tfrecord_file.endswith('tfrecord'):
+                tfrecord_file = '-'.join(tfrecord_file.split('/')[-1].split('-')[:-1]+['tfrecord'])
+                self.data_path_list.append(f'{data_folder}/{tfrecord_file}')
+
         self.index_path_list = []
         for i in range(len(self.data_path_list)):
             tfrecord_file = self.data_path_list[i]
             folder = os.path.dirname(tfrecord_file)
             if tfrecord_file.endswith('tfrecord') or tfrecord_file.endswith('index'):
                 index_file = '-'.join(tfrecord_file.split('/')[-1].split('-')[:-1]+['index'])
                 index_file = f'{folder}/{index_file}'
@@ -365,15 +404,18 @@
         # 转换样本
         new_sample = {}
         for k in sample.keys():
             if not k.startswith('__'):
                 if self.raw_description[k] == 'numpy':
                     dtype = numpy_dtype_map[sample[f'__{k}_type'][0]]
                     shape = tuple(sample[f'__{k}_shape'])
-                    new_sample[k] = np.frombuffer(bytearray(sample[k].tobytes()), dtype=dtype).reshape(shape).copy()
+                    if isinstance(sample[k], bytes):
+                        new_sample[k] = np.frombuffer(bytearray(sample[k]), dtype=dtype).reshape(shape).copy()
+                    else:
+                        new_sample[k] = np.frombuffer(bytearray(sample[k].tobytes()), dtype=dtype).reshape(shape).copy()
                 elif self.raw_description[k] == 'str':
                     new_sample[k] = sample[k].tobytes().decode('utf-8')
                 elif self.raw_description[k] == 'dict':
                     new_sample[k] = json.loads(sample[k].tobytes().decode('utf-8'))
                 else:
                     new_sample[k] = sample[k]
         sample = new_sample
```

### Comparing `antgo-0.1.3/antgo/framework/helper/exporter.py` & `antgo-0.1.4/antgo/framework/helper/exporter.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/fileio/__init__.py` & `antgo-0.1.4/antgo/framework/helper/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/fileio/file_client.py` & `antgo-0.1.4/antgo/framework/helper/fileio/file_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1036,40 +1036,34 @@
 
     def upload(self, remote_path, local_path, is_exist=False):
         return self.client.upload(remote_path, local_path, is_exist)
 
 
 def file_client_get(remote_path, local_path):
     status = FileClient.infer_client(uri=remote_path).download(remote_path, local_path)
-    time.sleep(1)
     return status
 
 
 def file_client_put(remote_path, local_path, is_exist=False):
     status = FileClient.infer_client(uri=remote_path).upload(remote_path, local_path, is_exist)
-    time.sleep(1)
     return status
 
 
 def file_client_ls(remote_folder):
     result = FileClient.infer_client(uri=remote_folder).ls(remote_folder)
-    time.sleep(1)
     return result
 
 
 def file_client_mkdir(remote_path, p=False):
     status = FileClient.infer_client(uri=remote_path).mkdir(remote_path, p)
-    time.sleep(1)
     return status
 
 
 def file_client_rm(remote_path):
     status = FileClient.infer_client(uri=remote_path).remove(remote_path)
-    time.sleep(1)
     return status
 
 
 def file_client_exists(remote_path):
     status = FileClient.infer_client(uri=remote_path).exists(remote_path)
-    time.sleep(1)
     return status
```

### Comparing `antgo-0.1.3/antgo/framework/helper/fileio/handlers/base.py` & `antgo-0.1.4/antgo/framework/helper/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/fileio/handlers/json_handler.py` & `antgo-0.1.4/antgo/framework/helper/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/fileio/handlers/pickle_handler.py` & `antgo-0.1.4/antgo/framework/helper/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/fileio/handlers/yaml_handler.py` & `antgo-0.1.4/antgo/framework/helper/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/fileio/io.py` & `antgo-0.1.4/antgo/framework/helper/fileio/io.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/fileio/parse.py` & `antgo-0.1.4/antgo/framework/helper/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/metrics/kp2d.py` & `antgo-0.1.4/antgo/framework/helper/metrics/kp2d.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/metrics/metrics.py` & `antgo-0.1.4/antgo/framework/helper/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/metrics/seg2d.py` & `antgo-0.1.4/antgo/framework/helper/metrics/seg2d.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/activelearning/acnet.py` & `antgo-0.1.4/antgo/framework/helper/models/activelearning/acnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/adda/adda.py` & `antgo-0.1.4/antgo/framework/helper/models/adda/adda.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/builder.py` & `antgo-0.1.4/antgo/framework/helper/models/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/classification/backbones/hrnet.py` & `antgo-0.1.4/antgo/framework/helper/models/classification/backbones/hrnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/classification/backbones/mobilenet_v2.py` & `antgo-0.1.4/antgo/framework/helper/models/classification/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/classification/backbones/resnet.py` & `antgo-0.1.4/antgo/framework/helper/models/classification/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/classification/backbones/resnext.py` & `antgo-0.1.4/antgo/framework/helper/models/classification/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/classification/heads/cls_head.py` & `antgo-0.1.4/antgo/framework/helper/models/classification/heads/cls_head.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/classification/heads/stacked_head.py` & `antgo-0.1.4/antgo/framework/helper/models/classification/heads/stacked_head.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/classification/losses/accuracy.py` & `antgo-0.1.4/antgo/framework/helper/models/classification/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/classification/losses/cross_entropy_loss.py` & `antgo-0.1.4/antgo/framework/helper/models/classification/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/classification/losses/utils.py` & `antgo-0.1.4/antgo/framework/helper/models/classification/losses/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/classification/model/base.py` & `antgo-0.1.4/antgo/framework/helper/models/classification/model/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/classification/model/classifier.py` & `antgo-0.1.4/antgo/framework/helper/models/classification/model/classifier.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/base.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/anchor/__init__.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/anchor/anchor_generator.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/anchor/builder.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/anchor/point_generator.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/point_generator.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/anchor/utils.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/anchor/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/__init__.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/__init__.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/approx_max_iou_assigner.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/approx_max_iou_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/assign_result.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/assign_result.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/atss_assigner.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/atss_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/center_region_assigner.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/center_region_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/grid_assigner.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/grid_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/hungarian_assigner.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/hungarian_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/max_iou_assigner.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/max_iou_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/point_assigner.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/point_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/region_assigner.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/region_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/sim_ota_assigner.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/sim_ota_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/assigners/uniform_assigner.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/assigners/uniform_assigner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/builder.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/coder/__init__.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/coder/bucketing_bbox_coder.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/bucketing_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/coder/delta_xywh_bbox_coder.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/delta_xywh_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/coder/distance_point_bbox_coder.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/distance_point_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/coder/legacy_delta_xywh_bbox_coder.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/legacy_delta_xywh_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/coder/pseudo_bbox_coder.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/pseudo_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/coder/tblr_bbox_coder.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/tblr_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/coder/yolo_bbox_coder.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/coder/yolo_bbox_coder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/iou2d_calculator.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/iou_calculators/iou2d_calculator.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/match_costs/match_cost.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/match_costs/match_cost.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/__init__.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/base_sampler.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/base_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/combined_sampler.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/combined_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/instance_balanced_pos_sampler.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/instance_balanced_pos_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/iou_balanced_neg_sampler.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/iou_balanced_neg_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/ohem_sampler.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/ohem_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/pseudo_sampler.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/pseudo_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/random_sampler.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/sampling_result.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/sampling_result.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/samplers/score_hlr_sampler.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/samplers/score_hlr_sampler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/bbox/transforms.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/bbox/transforms.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/mask/mask_target.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/mask/mask_target.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/mask/structures.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/mask/structures.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/mask/utils.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/mask/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/utils/__init__.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/utils/dist_utils.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/utils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/core/utils/misc.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/core/utils/misc.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/head/base_dense_head.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/head/base_dense_head.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/head/fcos_head.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/head/fcos_head.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,36 +7,18 @@
 from ..utils.gaussian_target import gaussian_radius, gen_gaussian_target
 from ..utils.gaussian_target import (get_local_maximum, get_topk_from_heatmap,
                                      transpose_and_gather_feat)
 from .base_dense_head import BaseDenseHead
 import torch.nn.functional as F
 
 
-def iou_loss(preds, targets):
-    '''
-    Args:
-    preds: [n,4] ltrb
-    targets: [n,4]
-    '''
-    lt = torch.min(preds[:, :2], targets[:, :2])
-    rb = torch.min(preds[:, 2:], targets[:, 2:])
-    wh = (rb + lt).clamp(min=0)
-    overlap = wh[:, 0] * wh[:, 1]  # [n]
-    area1 = (preds[:, 2] + preds[:, 0]) * (preds[:, 3] + preds[:, 1])
-    area2 = (targets[:, 2] + targets[:, 0]) * (targets[:, 3] + targets[:, 1])
-    iou = overlap / (area1 + area2 - overlap)
-    loss = -iou.clamp(min=1e-6).log()
-    return loss.sum()
-
-
 @HEADS.register_module()
 class FcosHead(BaseDenseHead):
     """Objects as Points Head. CenterHead use center_point to indicate object's
     position. Paper link <https://arxiv.org/abs/1904.07850>
-
     Args:
         in_channel (int): Number of channel in the input feature map.
         feat_channel (int): Number of channel in the intermediate feature map.
         num_classes (int): Number of categories excluding the background
             category.
         loss_center_heatmap (dict | None): Config of center heatmap loss.
             Default: GaussianFocalLoss.
@@ -49,33 +31,33 @@
             Default: None
     """
 
     def __init__(self,
                  in_channel,
                  feat_channel,
                  num_classes,
-                 down_stride,
                  rescale=1.0,
                  score_thresh=0.15,
                  loss_ch=dict(
                      type='GaussianFocalLoss', loss_weight=1.0),
+                 loss_wh=dict(type='L1Loss', loss_weight=0.1),
                  train_cfg=None,
                  test_cfg=None,
                  init_cfg=None):
         super(FcosHead, self).__init__(init_cfg)
         self.num_classes = num_classes
         self.rescale_x, self.rescale_y = rescale if type(rescale) == list or type(rescale) == tuple else (rescale, rescale)
         self.score_thresh = score_thresh
-        self.down_stride = down_stride
         self.in_channel = in_channel  
         self.feat_channel = feat_channel
         self._build_head()
         self.loss_center_heatmap=build_loss(loss_ch)
+        self.loss_reg = build_loss(loss_wh)
         self.train_cfg = train_cfg
-        self.test_cfg = test_cfg      
+        self.test_cfg = test_cfg
 
     def _build_head(self):
         self.heatmap_head = nn.Sequential(
             nn.Conv2d(self.in_channel, self.feat_channel, kernel_size=3, stride=1, padding=1),
             nn.ReLU(inplace=True),
             nn.Conv2d(self.feat_channel, self.num_classes, kernel_size=1, bias=True))
 
@@ -106,19 +88,17 @@
             elif isinstance(m, nn.Linear):
                 nn.init.normal_(m.weight, 0, 0.01)
                 if m.bias is not None:
                     nn.init.constant_(m.bias, 0)
 
     def forward(self, feats):
         """Forward features. Notice CenterNet head does not use FPN.
-
         Args:
             feats (tuple[Tensor]): Features from the upstream network, each is
                 a 4D-tensor.
-
         Returns:
             center_heatmap_preds (List[Tensor]): center predict heatmaps for
                 all levels, the channels number is num_classes.
             wh_preds (List[Tensor]): wh predicts for all levels, the channels
                 number is 2.
             offset_preds (List[Tensor]): offset predicts for all levels, the
                channels number is 2.
@@ -128,45 +108,35 @@
         return center_heatmap_pred, reg_pred
 
     def loss(self,
              center_heatmap_pred,
              reg_pred,
              bboxes,
              labels,
-             image_meta, gt_bboxes_ignore=None):
+             image_meta,
+             gt_bboxes_ignore=None):
         target_result, avg_factor = \
             self.get_targets(bboxes, labels, center_heatmap_pred.shape, image_meta, center_heatmap_pred.device)
 
         center_heatmap_target = target_result['center_heatmap_target']
         reg_targets = target_result['reg_targets']
         reg_weights = target_result['reg_weights']
 
-        loss_center_heatmap = \
-            self.loss_center_heatmap(center_heatmap_pred.sigmoid(), center_heatmap_target, avg_factor=avg_factor)
-
-        batch_size = center_heatmap_pred.shape[0]
-        pred = reg_pred.permute(0, 2, 3, 1)
-        pred = torch.reshape(pred, [batch_size, -1, 4])
-
-        gt = reg_targets.permute(0, 2, 3, 1)
-        gt = torch.reshape(gt, [batch_size, -1, 4])
-
-        loss_reg_offset = []
-        for batch_index in range(batch_size):
-            pred_pos = pred[batch_index][reg_weights[batch_index,0].view(-1).to(torch.bool)]  # [num_pos_b,4]
-            target_pos = gt[batch_index][reg_weights[batch_index,0].view(-1).to(torch.bool)]  # [num_pos_b,4]
-            loss_reg_offset.append(iou_loss(pred_pos, target_pos).view(1))
-
-        num_pos = torch.sum(reg_weights).clamp_(min=1).float()
-        loss_reg_offset = torch.cat(loss_reg_offset, dim=0) / num_pos
+        loss_center_heatmap = self.loss_center_heatmap(
+            center_heatmap_pred.sigmoid(), center_heatmap_target, avg_factor=avg_factor)
+        loss_reg_v = self.loss_reg(
+            reg_pred,
+            reg_targets,
+            reg_weights,
+            avg_factor=avg_factor*2)
 
         # 
         total_loss = dict(
             loss_center_heatmap=loss_center_heatmap,
-            loss_reg=loss_reg_offset)
+            loss_reg=loss_reg_v)
 
         return total_loss
 
     def coords_fmap(self, h, w):
         stride = 1
         shifts_x = torch.arange(0, w * stride, stride, dtype=torch.float32)
         shifts_y = torch.arange(0, h * stride, stride, dtype=torch.float32)
@@ -175,21 +145,19 @@
         shift_x = torch.reshape(shift_x, [-1])
         shift_y = torch.reshape(shift_y, [-1])
         coords = torch.stack([shift_x, shift_y], -1) + stride // 2
         return coords
 
     def get_targets(self, gt_bboxes, gt_labels, feat_shape, image_meta, device):
         """Compute regression and classification targets in multiple images.
-
         Args:
             gt_bboxes (list[Tensor]): Ground truth bboxes for each image with
                 shape (num_gts, 4) in [tl_x, tl_y, br_x, br_y] format.
             gt_labels (list[Tensor]): class indices corresponding to each box.
             img_shape (list[int]): image shape in [h, w] format.
-
         Returns:
             tuple[dict,float]: The float value is mean avg_factor, the dict has
                components below:
                - center_heatmap_target (Tensor): targets of center heatmap, \
                    shape (B, num_classes, H, W).
                - wh_target (Tensor): targets of wh predict, shape \
                    (B, 2, H, W).
@@ -211,29 +179,30 @@
         for batch_id in range(bs):
             gt_bbox = gt_bboxes[batch_id]       # gt_bbox shape: Nx4
             if gt_bbox.shape[0] == 0:
                 # 防止无目标样本
                 reg_target_list.append(torch.zeros([4, feat_h, feat_w], dtype=torch.float32, device=device))
                 reg_weight_list.append(torch.zeros([1, feat_h, feat_w], dtype=torch.float32, device=device))
                 continue
-
+            
             coords = self.coords_fmap(h=feat_h, w=feat_w).to(device=center_heatmap_target.device) #[h*w,2]
             x = coords[:, 0]
             y = coords[:, 1]
             l_off = x[:,None] - gt_bbox[...,0][None,:]*width_ratio    #[h*w,1]-[1,m]-->[h*w,m]
             t_off = y[:,None] - gt_bbox[...,1][None,:]*height_ratio
             r_off = gt_bbox[...,2][None,:]*width_ratio - x[:,None]
             b_off = gt_bbox[...,3][None,:]*height_ratio - y[:,None]
             ltrb_off = torch.stack([l_off,t_off,r_off,b_off],dim=-1)                        #[h*w,m,4]
             areas = (ltrb_off[...,0]+ltrb_off[...,2])*(ltrb_off[...,1]+ltrb_off[...,3])     #[h*w,m]
 
             off_min = torch.min(ltrb_off,dim=-1)[0]     #[h*w,m]
             off_max = torch.max(ltrb_off,dim=-1)[0]     #[h*w,m]
+
             mask_in_gtboxes = off_min>0
-            mask_in_level = (off_max>-1)&(off_max<=64)   # 设置最大尺寸和最小尺寸约束 (stride=8)
+            mask_in_level = (off_max>0)&(off_max<=80)   # 设置最大尺寸和最小尺寸约束
 
             radiu = 8 * 1.5
             gt_center_x = (gt_bbox[...,0]+gt_bbox[...,2])*width_ratio/2
             gt_center_y = (gt_bbox[...,1]+gt_bbox[...,3])*height_ratio/2
             c_l_off = x[:,None] - gt_center_x[None,:]#[h*w,1]-[1,m]-->[h*w,m]
             c_t_off = y[:,None] - gt_center_y[None,:]
             c_r_off = gt_center_x[None,:] - x[:,None]
@@ -251,16 +220,16 @@
             mask_pos_2 = mask_pos.long().sum(dim=-1)            #[h*w]
             mask_pos_2 = mask_pos_2 >= 1
             
             reg_target[~(mask_pos_2.to(torch.bool))] = 0
 
             # reshape
             reg_target = reg_target.reshape(feat_h, feat_w, 4).permute(2,0,1)
-
             mask_pos_2 = mask_pos_2.to(torch.float32).reshape(1, feat_h,feat_w)
+
             gt_label = gt_labels[batch_id]
             center_x = (gt_bbox[:, [0]] + gt_bbox[:, [2]]) * width_ratio / 2
             center_y = (gt_bbox[:, [1]] + gt_bbox[:, [3]]) * height_ratio / 2
             gt_centers = torch.cat((center_x, center_y), dim=1)
 
             for j, ct in enumerate(gt_centers):
                 ctx_int, cty_int = ct.int()
@@ -290,29 +259,27 @@
     def get_bboxes(self,
                    center_heatmap_preds,
                    reg_pred,
                    image_meta,
                    rescale=True,
                    with_nms=False):
         """Transform network output for a batch into bbox predictions.
-
         Args:
             center_heatmap_preds (list[Tensor]): Center predict heatmaps for
                 all levels with shape (B, num_classes, H, W).
             wh_preds (list[Tensor]): WH predicts for all levels with
                 shape (B, 2, H, W).
             offset_preds (list[Tensor]): Offset predicts for all levels
                 with shape (B, 2, H, W).
             img_metas (list[dict]): Meta information of each image, e.g.,
                 image size, scaling factor, etc.
             rescale (bool): If True, return boxes in original image space.
                 Default: True.
             with_nms (bool): If True, do nms before return boxes.
                 Default: False.
-
         Returns:
             list[tuple[Tensor, Tensor]]: Each item in result_list is 2-tuple.
                 The first item is an (n, 5) tensor, where 5 represent
                 (tl_x, tl_y, br_x, br_y, score) and the score between 0 and 1.
                 The shape of the second tensor in the tuple is (n,), and
                 each element represents the class label of the corresponding
                 box.
@@ -332,29 +299,27 @@
     def _get_bboxes_single(self,
                            center_heatmap_pred,
                            reg_pred,
                            img_meta,
                            rescale=False,
                            with_nms=True):
         """Transform outputs of a single image into bbox results.
-
         Args:
             center_heatmap_pred (Tensor): Center heatmap for current level with
                 shape (1, num_classes, H, W).
             wh_pred (Tensor): WH heatmap for current level with shape
                 (1, num_classes, H, W).
             offset_pred (Tensor): Offset for current level with shape
                 (1, corner_offset_channels, H, W).
             img_meta (dict): Meta information of current image, e.g.,
                 image size, scaling factor, etc.
             rescale (bool): If True, return boxes in original image space.
                 Default: False.
             with_nms (bool): If True, do nms before return boxes.
                 Default: True.
-
         Returns:
             tuple[Tensor, Tensor]: The first item is an (n, 5) tensor, where
                 5 represent (tl_x, tl_y, br_x, br_y, score) and the score
                 between 0 and 1. The shape of the second tensor in the tuple
                 is (n,), and each element represents the class label of the
                 corresponding box.
         """
@@ -372,15 +337,15 @@
 
         if rescale:
             det_bboxes[..., :4] *= det_bboxes.new_tensor((self.rescale_x, self.rescale_y, self.rescale_x, self.rescale_y))
 
         if 'nms' in self.test_cfg or with_nms:
             det_bboxes, det_labels = \
                 self._bboxes_nms(det_bboxes, det_labels, self.test_cfg)
-
+        
         # only for debug
         # image = cv2.imread(img_meta['image_file'])
         # det_bboxes_numpy = det_bboxes.detach().cpu().numpy()
         # for i in range(det_bboxes_numpy.shape[0]):
         #     x0,y0,x1,y1,_ = det_bboxes_numpy[i]
         #     cv2.rectangle(image, ((int)(x0),(int)(y0)), ((int)(x1),(int)(y1)), (255,0,0), 2)
         # cv2.imwrite('./aa.png', image)
@@ -389,29 +354,26 @@
     def decode_heatmap(self,
                        center_heatmap_pred,
                        reg_pred,
                        img_shape,
                        k=100,
                        kernel=3):
         """Transform outputs into detections raw bbox prediction.
-
         Args:
             center_heatmap_pred (Tensor): center predict heatmap,
                shape (B, num_classes, H, W).
             wh_pred (Tensor): wh predict, shape (B, 2, H, W).
             offset_pred (Tensor): offset predict, shape (B, 2, H, W).
             img_shape (list[int]): image shape in [h, w] format.
             k (int): Get top k center keypoints from heatmap. Default 100.
             kernel (int): Max pooling kernel for extract local maximum pixels.
                Default 3.
-
         Returns:
             tuple[torch.Tensor]: Decoded output of CenterNetHead, containing
                the following Tensors:
-
               - batch_bboxes (Tensor): Coords of each box with shape (B, k, 5)
               - batch_topk_labels (Tensor): Categories of each box with \
                   shape (B, k)
         """
         batch = center_heatmap_pred.shape[0]
         height, width = center_heatmap_pred.shape[2:]
         inp_h, inp_w = img_shape
@@ -451,8 +413,7 @@
             for i in range(bboxes.shape[0]):
                 if bboxes[i,4] > self.score_thresh:
                     remained_index.append(i)
             
             bboxes = bboxes[remained_index]
             labels = labels[remained_index]
         return bboxes, labels
-
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/head/focs_head_ml.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/head/fcos_head_ml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from pydoc import stripid
 import torch
 import torch.nn as nn
 from antgo.framework.helper.cnn import bias_init_with_prob, normal_init
 from antgo.framework.helper.models.builder import HEADS, build_loss
 from antgo.framework.helper.models.detectors.core.utils import multi_apply
 from torchvision.ops import batched_nms 
 from ..utils.gaussian_target import gaussian_radius, gen_gaussian_target
@@ -24,14 +23,38 @@
     overlap = wh[:, 0] * wh[:, 1]  # [n]
     area1 = (preds[:, 2] + preds[:, 0]) * (preds[:, 3] + preds[:, 1])
     area2 = (targets[:, 2] + targets[:, 0]) * (targets[:, 3] + targets[:, 1])
     iou = overlap / (area1 + area2 - overlap)
     loss = -iou.clamp(min=1e-6).log()
     return loss.sum()
 
+def giou_loss(preds, targets):
+    '''
+    Args:
+    preds: [n,4] ltrb
+    targets: [n,4]
+    '''
+    lt_min = torch.min(preds[:, :2], targets[:, :2])
+    rb_min = torch.min(preds[:, 2:], targets[:, 2:])
+    wh_min = (rb_min + lt_min).clamp(min=0)
+    overlap = wh_min[:, 0] * wh_min[:, 1]  # [n]
+    area1 = (preds[:, 2] + preds[:, 0]) * (preds[:, 3] + preds[:, 1])
+    area2 = (targets[:, 2] + targets[:, 0]) * (targets[:, 3] + targets[:, 1])
+    union = (area1 + area2 - overlap)
+    iou = overlap / union
+
+    lt_max = torch.max(preds[:, :2], targets[:, :2])
+    rb_max = torch.max(preds[:, 2:], targets[:, 2:])
+    wh_max = (rb_max + lt_max).clamp(0)
+    G_area = wh_max[:, 0] * wh_max[:, 1]  # [n]
+
+    giou = iou - (G_area - union) / G_area.clamp(1e-10)
+    loss = 1. - giou
+    return loss.sum()
+
 
 @HEADS.register_module()
 class FcosHeadML(BaseDenseHead):
     """Objects as Points Head. CenterHead use center_point to indicate object's
     position. Paper link <https://arxiv.org/abs/1904.07850>
 
     Args:
@@ -46,53 +69,56 @@
         train_cfg (dict | None): Training config. Useless in CenterNet,
             but we keep this variable for SingleStageDetector. Default: None.
         test_cfg (dict | None): Testing config of CenterNet. Default: None.
         init_cfg (dict or list[dict], optional): Initialization config dict.
             Default: None
     """
 
-    def __init__(self,
-                 in_channel,
-                 feat_channel,
-                 num_classes,
-                 down_stride=[8,16],
-                 rescale=1.0,
-                 score_thresh=0.15,
-                 loss_ch=dict(
-                     type='GaussianFocalLoss', loss_weight=1.0),
-                 train_cfg=None,
-                 test_cfg=None,
-                 init_cfg=None):
+    def __init__(
+        self,
+        in_channel,
+        feat_channel,
+        num_classes,
+        down_stride=[8,16],
+        rescale=1.0,
+        score_thresh=0.15,
+        loss_ch=dict(
+            type='GaussianFocalLoss', loss_weight=1.0),
+        loss_rg=dict(
+            type='IouLoss', loss_weight=0.2),
+        train_cfg=dict(
+            limit_range={8:[-1, 64], 16: [64,128], 32: [128,256], 64: [256,512],128: [512, 999999]}),
+        test_cfg=None,
+        init_cfg=dict(
+            type='Xavier', layer='Conv2d', distribution='uniform')):
         super(FcosHeadML, self).__init__(init_cfg)
         self.num_classes = num_classes
         self.rescale_x, self.rescale_y = rescale if type(rescale) == list or type(rescale) == tuple else (rescale, rescale)
         self.score_thresh = score_thresh
         self.down_stride = down_stride
-        self.limit_range = {
-            8: [-1, 64],
-            16: [64,128],
-            32: [128,256],
-            64: [256,512],
-            128: [512, 999999]
-        }
+        self.limit_range = train_cfg.get('limit_range')
 
         self.in_channel = in_channel  
         self.feat_channel = feat_channel
         self._build_head()
         self.loss_center_heatmap=build_loss(loss_ch)
+        
+        self.loss_reg_func = iou_loss if loss_rg.get('type') == 'IouLoss' else giou_loss
+        self.loss_reg_weight = loss_rg.get('loss_weight')
         self.train_cfg = train_cfg
         self.test_cfg = test_cfg      
 
     def _build_head(self):
         self.heatmap_head_list = nn.ModuleList()
         self.reg_head_list = nn.ModuleList()
         for _ in self.down_stride:
             self.heatmap_head_list.append(
-                    nn.Sequential(
+                nn.Sequential(
                     nn.Conv2d(self.in_channel, self.feat_channel, kernel_size=3, stride=1, padding=1),
+                    nn.BatchNorm2d(self.feat_channel),
                     nn.ReLU(inplace=True),
                     nn.Conv2d(self.feat_channel, self.num_classes, kernel_size=1, bias=True)
                 )
             )
 
             self.reg_head_list.append(
                 nn.Sequential(
@@ -195,20 +221,20 @@
         pred_reg_offset_multi_levels = torch.cat(pred_reg_offset_multi_levels, dim=1)
         gt_reg_offset_multi_levels = torch.cat(gt_reg_offset_multi_levels, dim=1)
         mask_multi_levels = torch.cat(mask_multi_levels, dim=1)
 
         for batch_index in range(batch_size):
             pred_pos = pred_reg_offset_multi_levels[batch_index][mask_multi_levels[batch_index].to(torch.bool)]#[num_pos_b,4]
             target_pos=gt_reg_offset_multi_levels[batch_index][mask_multi_levels[batch_index].to(torch.bool)]#[num_pos_b,4]
-            loss_reg_offset_avg.append(iou_loss(pred_pos,target_pos).view(1))
+            loss_reg_offset_avg.append(self.loss_reg_func(pred_pos,target_pos).view(1))
 
         loss_reg_offset_avg = torch.mean(torch.cat(loss_reg_offset_avg))
         total_loss = dict(
             loss_center_heatmap=loss_center_heatmap_avg,
-            loss_reg=loss_reg_offset_avg)
+            loss_reg=loss_reg_offset_avg * self.loss_reg_weight)
 
         return total_loss
 
     def coords_fmap(self, h, w, stride):
         shifts_x = torch.arange(0, w * stride, stride, dtype=torch.float32)
         shifts_y = torch.arange(0, h * stride, stride, dtype=torch.float32)
 
@@ -235,27 +261,29 @@
                - wh_target (Tensor): targets of wh predict, shape \
                    (B, 2, H, W).
                - offset_target (Tensor): targets of offset predict, shape \
                    (B, 2, H, W).
                - wh_offset_target_weight (Tensor): weights of wh and offset \
                    predict, shape (B, 2, H, W).
         """
-        img_h = image_meta[0]['image_shape'][0]
-        img_w = image_meta[0]['image_shape'][1]
+
         bs, _, feat_h, feat_w = feat_shape
 
-        width_ratio = float(feat_w / img_w)
-        height_ratio = float(feat_h / img_h)
+        # img_h = image_meta[0]['image_shape'][0]
+        # img_w = image_meta[0]['image_shape'][1]
+        # width_ratio = float(feat_w / img_w)
+        # height_ratio = float(feat_h / img_h)
 
         center_heatmap_target = torch.zeros([bs, self.num_classes, feat_h, feat_w], dtype=torch.float32, device=device)
         reg_target_list = []
         reg_weight_list = []
         for batch_id in range(bs):
             gt_bbox = gt_bboxes[batch_id]       # gt_bbox shape: Nx4
-            if gt_bbox.shape[0] == 0:
+            num_gt_bbox = gt_bbox.shape[0]
+            if num_gt_bbox == 0:
                 # 防止无目标样本
                 reg_target_list.append(torch.zeros([4, feat_h, feat_w], dtype=torch.float32, device=device))
                 reg_weight_list.append(torch.zeros([1, feat_h, feat_w], dtype=torch.float32, device=device))
                 continue
 
             coords = self.coords_fmap(h=feat_h, w=feat_w, stride=stride).to(device=center_heatmap_target.device) #[h*w,2]
             x = coords[:, 0]
@@ -267,15 +295,15 @@
             ltrb_off = torch.stack([l_off,t_off,r_off,b_off],dim=-1)                        #[h*w,m,4]
             areas = (ltrb_off[...,0]+ltrb_off[...,2])*(ltrb_off[...,1]+ltrb_off[...,3])     #[h*w,m]
 
             off_min = torch.min(ltrb_off,dim=-1)[0]     #[h*w,m]
             off_max = torch.max(ltrb_off,dim=-1)[0]     #[h*w,m]
             mask_in_gtboxes = off_min>0
             mask_in_level = \
-                (off_max>self.limit_range[stride][0])&(off_max<=self.limit_range[stride][1])   # 设置最大尺寸和最小尺寸约束 (stride=8)
+                (off_max>self.limit_range[stride][0])&(off_max<=self.limit_range[stride][1])   # 设置最大尺寸和最小尺寸约束
 
             radiu = stride * 1.5
             gt_center_x = (gt_bbox[...,0]+gt_bbox[...,2])/2
             gt_center_y = (gt_bbox[...,1]+gt_bbox[...,3])/2
             c_l_off = x[:,None] - gt_center_x[None,:]#[h*w,1]-[1,m]-->[h*w,m]
             c_t_off = y[:,None] - gt_center_y[None,:]
             c_r_off = gt_center_x[None,:] - x[:,None]
@@ -284,42 +312,54 @@
             c_off_max = torch.max(c_ltrb_off,dim=-1)[0]
             mask_center = c_off_max<radiu
 
             mask_pos=mask_in_gtboxes&mask_in_level&mask_center      #[h*w,m]
             areas[~mask_pos] = 99999999
             areas_min_ind=torch.min(areas,dim=-1)[1]    #[h*w]
 
-            reg_target = ltrb_off[torch.zeros_like(areas,dtype=torch.bool).scatter_(-1, areas_min_ind.unsqueeze(dim=-1),1)]#[h*w,4]
+            reg_target = ltrb_off[
+                torch.zeros_like(areas,dtype=torch.bool).scatter_(-1, areas_min_ind.unsqueeze(dim=-1),1)]   #[h*w,4]
             reg_target = torch.reshape(reg_target,(-1,4))       #[h*w,4]
             mask_pos_2 = mask_pos.long().sum(dim=-1)            #[h*w]
             mask_pos_2 = mask_pos_2 >= 1
-            
-            reg_target[~(mask_pos_2.to(torch.bool))] = 0
+
+            gt_label = gt_labels[batch_id]  # m
+
+            # 测试不使用高斯
+            gt_label = torch.broadcast_tensors(gt_label[None, :], areas.long())[0]  # [h*w,m]            
+            cls_targets = gt_label[
+                torch.zeros_like(areas,dtype=torch.bool).scatter_(-1, areas_min_ind.unsqueeze(dim=-1), 1)
+            ]
+            cls_targets = F.one_hot(cls_targets, num_classes=self.num_classes)
+            cls_targets[~(mask_pos_2.to(torch.bool))] = 0            
+            cls_targets = torch.permute(cls_targets, (1,0))
+            cls_targets = torch.reshape(cls_targets, (-1, feat_h, feat_w))
+            center_heatmap_target[batch_id] = cls_targets
 
             # reshape
+            reg_target[~(mask_pos_2.to(torch.bool))] = 0            
             reg_target = reg_target.reshape(feat_h, feat_w, 4).permute(2,0,1)
-
             mask_pos_2 = mask_pos_2.to(torch.float32).reshape(1, feat_h,feat_w)
-            gt_label = gt_labels[batch_id]
-            center_x = (gt_bbox[:, [0]] + gt_bbox[:, [2]]) * width_ratio / 2
-            center_y = (gt_bbox[:, [1]] + gt_bbox[:, [3]]) * height_ratio / 2
-            gt_centers = torch.cat((center_x, center_y), dim=1)
-
-            for j, ct in enumerate(gt_centers):
-                ctx_int, cty_int = ct.int()
-                if mask_pos[cty_int*feat_w+ctx_int, j] == 0:
-                    continue
-                scale_box_h = (gt_bbox[j][3] - gt_bbox[j][1]) * height_ratio
-                scale_box_w = (gt_bbox[j][2] - gt_bbox[j][0]) * width_ratio
 
-                radius = gaussian_radius([scale_box_h, scale_box_w], min_overlap=0.3)
-                radius = max(int(1), int(radius))
+            # # 基于高斯构建目标
+            # center_x = (gt_bbox[:, [0]] + gt_bbox[:, [2]]) * width_ratio / 2
+            # center_y = (gt_bbox[:, [1]] + gt_bbox[:, [3]]) * height_ratio / 2
+            # gt_centers = torch.cat((center_x, center_y), dim=1)            
+            # for j, ct in enumerate(gt_centers):
+            #     ctx_int, cty_int = ct.int()
+            #     if mask_pos[cty_int*feat_w+ctx_int, j] == 0:
+            #         continue
+            #     scale_box_h = (gt_bbox[j][3] - gt_bbox[j][1]) * height_ratio
+            #     scale_box_w = (gt_bbox[j][2] - gt_bbox[j][0]) * width_ratio
+
+            #     radius = gaussian_radius([scale_box_h, scale_box_w], min_overlap=0.6)
+            #     radius = max(int(2), int(radius))
 
-                ind = gt_label[j]
-                gen_gaussian_target(center_heatmap_target[batch_id, ind], [ctx_int, cty_int], radius)
+            #     ind = gt_label[j]
+            #     gen_gaussian_target(center_heatmap_target[batch_id, ind], [ctx_int, cty_int], radius)
 
             reg_target_list.append(reg_target)
             reg_weight_list.append(mask_pos_2)
 
         reg_targets = torch.stack(reg_target_list, 0)           #Bx4xHxW
         reg_weights = torch.stack(reg_weight_list, 0)
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/losses/__init__.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 from .accuracy import Accuracy, accuracy
 from .ae_loss import AssociativeEmbeddingLoss
 from .balanced_l1_loss import BalancedL1Loss, balanced_l1_loss
 from .cross_entropy_loss import (CrossEntropyLoss, binary_cross_entropy,
                                  cross_entropy, mask_cross_entropy)
 from .dice_loss import DiceLoss
 from .focal_loss import FocalLoss, sigmoid_focal_loss
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/losses/accuracy.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/accuracy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import torch.nn as nn
 
 
 def accuracy(pred, target, topk=1, thresh=None):
     """Calculate accuracy according to the prediction and target.
 
     Args:
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/losses/ae_loss.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/ae_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from antgo.framework.helper.models.builder import LOSSES
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/losses/balanced_l1_loss.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/balanced_l1_loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import numpy as np
 import torch
 import torch.nn as nn
 
 from antgo.framework.helper.models.builder import LOSSES
 from .utils import weighted_loss
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/losses/cross_entropy_loss.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/cross_entropy_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from antgo.framework.helper.models.builder import LOSSES
 from .utils import weight_reduce_loss
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/losses/dice_loss.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/dice_loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import torch
 import torch.nn as nn
 
 from antgo.framework.helper.models.builder import LOSSES
 from .utils import weight_reduce_loss
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/losses/focal_loss.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/focal_loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 # from mmcv.ops import sigmoid_focal_loss as _sigmoid_focal_loss
 
 from antgo.framework.helper.models.builder import LOSSES
 from .utils import weight_reduce_loss
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/losses/gaussian_focal_loss.py` & `antgo-0.1.4/antgo/framework/helper/models/pose3d/losses/gaussian_focal_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         else:
             loss = neg_loss
     else:
         loss = pos_loss + neg_loss
     return loss
 
 
-@LOSSES.register_module()
 class GaussianFocalLoss(nn.Module):
     """GaussianFocalLoss is a variant of focal loss.
 
     More details can be found in the `paper
     <https://arxiv.org/abs/1808.01244>`_
     Code is modified from `kp_utils.py
     <https://github.com/princeton-vl/CornerNet/blob/master/models/py_utils/kp_utils.py#L152>`_  # noqa: E501
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/losses/gfocal_loss.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/gfocal_loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import torch.nn as nn
 import torch.nn.functional as F
 
 from antgo.framework.helper.models.builder import LOSSES
 from .utils import weighted_loss
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/losses/ghm_loss.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/ghm_loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from antgo.framework.helper.models.builder import LOSSES
 from .utils import weight_reduce_loss
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/losses/iou_loss.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/iou_loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import math
 import warnings
 
 import torch
 import torch.nn as nn
 
 from antgo.framework.helper.models.detectors.core.bbox import bbox_overlaps
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/losses/kd_loss.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/kd_loss.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import torch.nn as nn
 import torch.nn.functional as F
 
 from antgo.framework.helper.models.builder import LOSSES
 from .utils import weighted_loss
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/losses/mse_loss.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/mse_loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import torch.nn as nn
 import torch.nn.functional as F
 
 from antgo.framework.helper.models.builder import LOSSES
 from .utils import weighted_loss
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/losses/pisa_loss.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/pisa_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import torch
 
 from antgo.framework.helper.models.detectors.core.bbox import bbox_overlaps
 
 
 def isr_p(cls_score,
           bbox_pred,
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/losses/seesaw_loss.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/seesaw_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from antgo.framework.helper.models.builder import LOSSES
 from .accuracy import accuracy
 from .cross_entropy_loss import cross_entropy
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/losses/smooth_l1_loss.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/smooth_l1_loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import torch
 import torch.nn as nn
 
 from antgo.framework.helper.models.builder import LOSSES
 from .utils import weighted_loss
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/losses/utils.py` & `antgo-0.1.4/antgo/framework/helper/models/pose3d/losses/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/losses/varifocal_loss.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/varifocal_loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import torch.nn as nn
 import torch.nn.functional as F
 
 from antgo.framework.helper.models.builder import LOSSES
 from .utils import weight_reduce_loss
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/neck/fpn.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/neck/fpn.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/single_stage.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/single_stage.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/utils/gaussian_target.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/utils/gaussian_target.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/utils/util_mixins.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/utils/util_mixins.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/detectors/utils/util_random.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/utils/util_random.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/distillation_model.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/distillation_model.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/ab.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/ab.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/afd.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/afd.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/at.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/at.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/bss.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/bss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/cc.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/cc.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/crd.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/crd.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/dml.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/dml.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/fsp.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/fsp.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/ft.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/ft.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/hcl.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/hcl.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/irg.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/irg.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/logits.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/logits.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/lwm.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/lwm.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/mgd.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/mgd.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/nst.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/nst.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/ofd.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/ofd.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/pkt.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/pkt.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/rkd.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/rkd.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/sobolev.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/sobolev.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/sp.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/sp.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/st.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/st.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/distillation/loss/vid.py` & `antgo-0.1.4/antgo/framework/helper/models/distillation/loss/vid.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/dummy_module.py` & `antgo-0.1.4/antgo/framework/helper/models/dummy_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/ema_module.py` & `antgo-0.1.4/antgo/framework/helper/models/ema_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_layers.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_layers.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_op.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/modules/dynamic_op.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/elastic_nn/utils.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/elastic_nn/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/model_zoo.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/model_zoo.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/ofa/baseline/mobilenet_v3.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/ofa/baseline/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/ofa/networks/ofa_mbv3.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/ofa/networks/ofa_mbv3.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/ofa/training/epoch_based_sampling_runner.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/ofa/training/epoch_based_sampling_runner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/ofa/training/evaluation.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/ofa/training/evaluation.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/ofa/utils.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/ofa/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_dataset.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_predictor.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/search/accuracy_predictor/acc_predictor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/search/accuracy_predictor/arch_encoder.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/search/accuracy_predictor/arch_encoder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/search/efficiency_predictor/__init__.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/search/efficiency_predictor/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/search/efficiency_predictor/latency_lookup_table.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/search/efficiency_predictor/latency_lookup_table.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/search/search_algorithm/evolution.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/search/search_algorithm/evolution.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/test.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/test.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/tutorial/accuracy_predictor.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/accuracy_predictor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/tutorial/evolution_finder.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/evolution_finder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/tutorial/flops_table.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/flops_table.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/tutorial/imagenet_eval_helper.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/imagenet_eval_helper.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/tutorial/latency_table.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/tutorial/latency_table.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/utils/common_tools.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/utils/common_tools.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/utils/flops_counter.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/utils/layers.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/utils/layers.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/utils/my_modules.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/utils/my_modules.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/utils/pytorch_modules.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/utils/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/nas/utils/pytorch_utils.py` & `antgo-0.1.4/antgo/framework/helper/models/nas/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/pose3d/backbone/QNetLite0_alpha.py` & `antgo-0.1.4/antgo/framework/helper/models/pose3d/backbone/QNetLite0_alpha.py`

 * *Files 5% similar despite different names*

```diff
@@ -233,14 +233,36 @@
         self.layer4 = self.make_layer(self.block, 64, self.layers[3], stride=2, dcn=stage_dcn[3])
         self.block.exp = 4
         self.layer5 = self.make_layer(self.block, 96, self.layers[4], stride=1, dcn=stage_dcn[4])
         self.layer6 = self.make_layer(self.block, 128, self.layers[5], stride=2, dcn=stage_dcn[5])
         self.block.exp = 6
         self.layer7 = self.make_layer(self.block, 128, self.layers[6], stride=1, dcn=stage_dcn[6])
         self.layer8 = self.make_layer(self.block, 160, self.layers[7], stride=2, dcn=stage_dcn[7])
+        self.init_weights()
+
+    def init_weights(self):
+        """Initialize weights of the head."""
+        for m in self.modules():
+            if isinstance(m, nn.Conv2d):
+                nn.init.kaiming_normal_(
+                    m.weight, mode='fan_out', nonlinearity='relu')
+            elif isinstance(m, nn.BatchNorm2d):
+                nn.init.constant_(m.weight, 1)
+                if m.bias is not None:
+                    nn.init.constant_(m.bias, 0.0001)
+                nn.init.constant_(m.running_mean, 0)
+            elif isinstance(m, nn.BatchNorm1d):
+                nn.init.constant_(m.weight, 1)
+                if m.bias is not None:
+                    nn.init.constant_(m.bias, 0.0001)
+                nn.init.constant_(m.running_mean, 0)
+            elif isinstance(m, nn.Linear):
+                nn.init.normal_(m.weight, 0, 0.01)
+                if m.bias is not None:
+                    nn.init.constant_(m.bias, 0)
 
     def forward(self, x):
         x = self.relu1(self.bn1(self.conv1(x)))  # 32 * h/4 * w/4
         x = self.layer1(x)
         outs = []
         if 0 in self.out_indices:
             outs.append(x)
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/pose3d/backbone/QNetLite0_beta.py` & `antgo-0.1.4/antgo/framework/helper/models/pose3d/backbone/QNetLite0_beta.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/pose3d/head/handpose_qnet_lite0_pose_heatmap2d.py` & `antgo-0.1.4/antgo/framework/helper/models/pose3d/head/handpose_qnet_lite0_pose_heatmap2d.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/pose3d/head/layer.py` & `antgo-0.1.4/antgo/framework/helper/models/pose3d/head/layer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/pose3d/head/twohand_3dpose_latent.py` & `antgo-0.1.4/antgo/framework/helper/models/pose3d/head/twohand_3dpose_latent.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/pose3d/losses/gaussian_focal_loss.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/gaussian_focal_loss.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import torch
 import torch.nn as nn
 
 from antgo.framework.helper.models.builder import LOSSES
 from .utils import weighted_loss
 
 
@@ -39,14 +38,15 @@
         else:
             loss = neg_loss
     else:
         loss = pos_loss + neg_loss
     return loss
 
 
+@LOSSES.register_module()
 class GaussianFocalLoss(nn.Module):
     """GaussianFocalLoss is a variant of focal loss.
 
     More details can be found in the `paper
     <https://arxiv.org/abs/1808.01244>`_
     Code is modified from `kp_utils.py
     <https://github.com/princeton-vl/CornerNet/blob/master/models/py_utils/kp_utils.py#L152>`_  # noqa: E501
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/pose3d/losses/loss.py` & `antgo-0.1.4/antgo/framework/helper/models/pose3d/losses/loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/pose3d/losses/utils.py` & `antgo-0.1.4/antgo/framework/helper/models/detectors/losses/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import functools
 import torch.nn.functional as F
 
 
 def reduce_loss(loss, reduction):
     """Reduce loss as specified.
```

### Comparing `antgo-0.1.3/antgo/framework/helper/models/pose3d/model/ddr_twohand_pose3d.py` & `antgo-0.1.4/antgo/framework/helper/models/pose3d/model/ddr_twohand_pose3d.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/pose3d/model/keynet_model.py` & `antgo-0.1.4/antgo/framework/helper/models/pose3d/model/keynet_model.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/proxy_module.py` & `antgo-0.1.4/antgo/framework/helper/models/proxy_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/segmentation/backbone/DDRQNetLite0.py` & `antgo-0.1.4/antgo/framework/helper/models/segmentation/backbone/DDRQNetLite0.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/segmentation/head/aspp_head.py` & `antgo-0.1.4/antgo/framework/helper/models/segmentation/head/aspp_head.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/segmentation/head/simple_head.py` & `antgo-0.1.4/antgo/framework/helper/models/segmentation/head/simple_head.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/segmentation/model/encoder_decoder.py` & `antgo-0.1.4/antgo/framework/helper/models/segmentation/model/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/semi/dense.py` & `antgo-0.1.4/antgo/framework/helper/models/semi/dense.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/semi/detmpl.py` & `antgo-0.1.4/antgo/framework/helper/models/semi/detmpl.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/semi/hook/mean_teacher.py` & `antgo-0.1.4/antgo/framework/helper/models/semi/hook/mean_teacher.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/semi/losses/quality_focal_loss.py` & `antgo-0.1.4/antgo/framework/helper/models/semi/losses/quality_focal_loss.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/semi/mpl.py` & `antgo-0.1.4/antgo/framework/helper/models/semi/mpl.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/utils/__init__.py` & `antgo-0.1.4/antgo/framework/helper/models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/utils/box_utils.py` & `antgo-0.1.4/antgo/framework/helper/models/utils/box_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/utils/brick_wrappers.py` & `antgo-0.1.4/antgo/framework/helper/models/utils/brick_wrappers.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/utils/builder.py` & `antgo-0.1.4/antgo/framework/helper/models/utils/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/utils/ckpt_convert.py` & `antgo-0.1.4/antgo/framework/helper/models/utils/ckpt_convert.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/utils/conv_upsample.py` & `antgo-0.1.4/antgo/framework/helper/models/utils/conv_upsample.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/utils/csp_layer.py` & `antgo-0.1.4/antgo/framework/helper/models/utils/csp_layer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/utils/gaussian_target.py` & `antgo-0.1.4/antgo/framework/helper/models/utils/gaussian_target.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/utils/inverted_residual.py` & `antgo-0.1.4/antgo/framework/helper/models/utils/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/utils/make_divisible.py` & `antgo-0.1.4/antgo/framework/helper/models/utils/make_divisible.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/utils/misc.py` & `antgo-0.1.4/antgo/framework/helper/models/utils/misc.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/utils/normed_predictor.py` & `antgo-0.1.4/antgo/framework/helper/models/utils/normed_predictor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/utils/panoptic_gt_processing.py` & `antgo-0.1.4/antgo/framework/helper/models/utils/panoptic_gt_processing.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/utils/positional_encoding.py` & `antgo-0.1.4/antgo/framework/helper/models/utils/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/utils/res_layer.py` & `antgo-0.1.4/antgo/framework/helper/models/utils/res_layer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/utils/se_layer.py` & `antgo-0.1.4/antgo/framework/helper/models/utils/se_layer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/utils/structure_utils.py` & `antgo-0.1.4/antgo/framework/helper/models/utils/structure_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/models/utils/structures.py` & `antgo-0.1.4/antgo/framework/helper/models/utils/structures.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/multi_stream_module.py` & `antgo-0.1.4/antgo/framework/helper/multi_stream_module.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/parallel/_functions.py` & `antgo-0.1.4/antgo/framework/helper/parallel/_functions.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/parallel/collate.py` & `antgo-0.1.4/antgo/framework/helper/parallel/collate.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/parallel/data_container.py` & `antgo-0.1.4/antgo/framework/helper/parallel/data_container.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/parallel/data_parallel.py` & `antgo-0.1.4/antgo/framework/helper/parallel/data_parallel.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,36 +60,36 @@
             return self.module.train_step(*inputs[0], **kwargs[0])
 
         assert len(self.device_ids) == 1, \
             ('MMDataParallel only supports single GPU training, if you need to'
              ' train with multiple GPUs, please use MMDistributedDataParallel'
              ' instead.')
 
-        for t in chain(self.module.parameters(), self.module.buffers()):
-            if t.device != self.src_device_obj:
-                raise RuntimeError(
-                    'module must have its parameters and buffers '
-                    f'on device {self.src_device_obj} (device_ids[0]) but '
-                    f'found one of them on device: {t.device}')
+        # for t in chain(self.module.parameters(), self.module.buffers()):
+        #     if t.device != self.src_device_obj:
+        #         raise RuntimeError(
+        #             'module must have its parameters and buffers '
+        #             f'on device {self.src_device_obj} (device_ids[0]) but '
+        #             f'found one of them on device: {t.device}')
 
         inputs, kwargs = self.scatter(inputs, kwargs, self.device_ids)
         return self.module.train_step(*inputs[0], **kwargs[0])
 
     def val_step(self, *inputs, **kwargs):
         if not self.device_ids:
             # We add the following line thus the module could gather and
             # convert data containers as those in GPU inference
             inputs, kwargs = self.scatter(inputs, kwargs, [-1])
             return self.module.val_step(*inputs[0], **kwargs[0])
 
         assert len(self.device_ids) == 1, \
             ('only supports single GPU training')
 
-        for t in chain(self.module.parameters(), self.module.buffers()):
-            if t.device != self.src_device_obj:
-                raise RuntimeError(
-                    'module must have its parameters and buffers '
-                    f'on device {self.src_device_obj} (device_ids[0]) but '
-                    f'found one of them on device: {t.device}')
+        # for t in chain(self.module.parameters(), self.module.buffers()):
+        #     if t.device != self.src_device_obj:
+        #         raise RuntimeError(
+        #             'module must have its parameters and buffers '
+        #             f'on device {self.src_device_obj} (device_ids[0]) but '
+        #             f'found one of them on device: {t.device}')
 
         inputs, kwargs = self.scatter(inputs, kwargs, self.device_ids)
         return self.module.val_step(*inputs[0], **kwargs[0])
```

### Comparing `antgo-0.1.3/antgo/framework/helper/parallel/distributed.py` & `antgo-0.1.4/antgo/framework/helper/parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/parallel/scatter_gather.py` & `antgo-0.1.4/antgo/framework/helper/parallel/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/parallel/utils.py` & `antgo-0.1.4/antgo/framework/helper/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/reader.py` & `antgo-0.1.4/antgo/framework/helper/reader.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/__init__.py` & `antgo-0.1.4/antgo/framework/helper/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/base_runner.py` & `antgo-0.1.4/antgo/framework/helper/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/builder.py` & `antgo-0.1.4/antgo/framework/helper/runner/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/checkpoint.py` & `antgo-0.1.4/antgo/framework/helper/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/default_constructor.py` & `antgo-0.1.4/antgo/framework/helper/runner/default_constructor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/dist_utils.py` & `antgo-0.1.4/antgo/framework/helper/runner/dist_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/epoch_based_runner.py` & `antgo-0.1.4/antgo/framework/helper/runner/epoch_based_runner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/fp16_utils.py` & `antgo-0.1.4/antgo/framework/helper/runner/fp16_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/__init__.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/checkpoint.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/ema.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/ema.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/evaluation.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/evaluation.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/hook.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/logger/base.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/logger/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/logger/neptune.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/logger/neptune.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/logger/text.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/logger/text.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/lr_updater.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/lr_updater.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Copyright (c) OpenMMLab. All rights reserved.
 import numbers
 from math import cos, pi
 from .hook import HOOKS, Hook
 
 
 class LrUpdaterHook(Hook):
     """LR Scheduler.
```

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/memory.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/memory.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/momentum_updater.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/momentum_updater.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/optimizer.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/optimizer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/profiler.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/profiler.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/sampler_seed.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/sampler_seed.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/samplingmethods/kcenter_greedy.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/samplingmethods/kcenter_greedy.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/samplingmethods/sampling_def.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/samplingmethods/sampling_def.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/submodules_evaluation.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/submodules_evaluation.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/sync_buffer.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/sync_buffer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/hooks/weight_adjust.py` & `antgo-0.1.4/antgo/framework/helper/runner/hooks/weight_adjust.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/iter_based_runner.py` & `antgo-0.1.4/antgo/framework/helper/runner/iter_based_runner.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/log_buffer.py` & `antgo-0.1.4/antgo/framework/helper/runner/log_buffer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/optimizer/builder.py` & `antgo-0.1.4/antgo/framework/helper/runner/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/optimizer/default_constructor.py` & `antgo-0.1.4/antgo/framework/helper/runner/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/priority.py` & `antgo-0.1.4/antgo/framework/helper/runner/priority.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/test.py` & `antgo-0.1.4/antgo/framework/helper/runner/test.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/runner/utils.py` & `antgo-0.1.4/antgo/framework/helper/runner/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/task_flag.py` & `antgo-0.1.4/antgo/framework/helper/task_flag.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/tester.py` & `antgo-0.1.4/antgo/framework/helper/tester.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/tools/evaluate.py` & `antgo-0.1.4/antgo/framework/helper/tools/evaluate.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/tools/exp.py` & `antgo-0.1.4/antgo/framework/helper/tools/exp.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/tools/export_onnx.py` & `antgo-0.1.4/antgo/framework/helper/tools/export_onnx.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/tools/train.py` & `antgo-0.1.4/antgo/framework/helper/tools/train.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/tools/util.py` & `antgo-0.1.4/antgo/framework/helper/tools/util.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/trainer.py` & `antgo-0.1.4/antgo/framework/helper/trainer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/__init__.py` & `antgo-0.1.4/antgo/framework/helper/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/compat_config.py` & `antgo-0.1.4/antgo/framework/helper/utils/compat_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/config.py` & `antgo-0.1.4/antgo/framework/helper/utils/config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/dist_utils.py` & `antgo-0.1.4/antgo/framework/helper/utils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/env.py` & `antgo-0.1.4/antgo/framework/helper/utils/env.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/ext_loader.py` & `antgo-0.1.4/antgo/framework/helper/utils/ext_loader.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/hub.py` & `antgo-0.1.4/antgo/framework/helper/utils/hub.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/logging.py` & `antgo-0.1.4/antgo/framework/helper/utils/logging.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/math_3d.py` & `antgo-0.1.4/antgo/framework/helper/utils/math_3d.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/misc.py` & `antgo-0.1.4/antgo/framework/helper/utils/misc.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/parrots_jit.py` & `antgo-0.1.4/antgo/framework/helper/utils/parrots_jit.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/parrots_wrapper.py` & `antgo-0.1.4/antgo/framework/helper/utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/path.py` & `antgo-0.1.4/antgo/framework/helper/utils/path.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/progressbar.py` & `antgo-0.1.4/antgo/framework/helper/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/registry.py` & `antgo-0.1.4/antgo/framework/helper/utils/registry.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/seed.py` & `antgo-0.1.4/antgo/framework/helper/utils/seed.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/setup_env.py` & `antgo-0.1.4/antgo/framework/helper/utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/testing.py` & `antgo-0.1.4/antgo/framework/helper/utils/testing.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/timer.py` & `antgo-0.1.4/antgo/framework/helper/utils/timer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/trace.py` & `antgo-0.1.4/antgo/framework/helper/utils/trace.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/util_distribution.py` & `antgo-0.1.4/antgo/framework/helper/utils/util_distribution.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/helper/utils/version_utils.py` & `antgo-0.1.4/antgo/framework/helper/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/paddle2torch/mapper/io.py` & `antgo-0.1.4/antgo/framework/paddle2torch/mapper/io.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/paddle2torch/mapper/nn.py` & `antgo-0.1.4/antgo/framework/paddle2torch/mapper/nn.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/paddle2torch/mapper/ops.py` & `antgo-0.1.4/antgo/framework/paddle2torch/mapper/ops.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/paddle2torch/mapper/optimizer.py` & `antgo-0.1.4/antgo/framework/paddle2torch/mapper/optimizer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/paddle2torch/utils.py` & `antgo-0.1.4/antgo/framework/paddle2torch/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/mapper/__init__.py` & `antgo-0.1.4/antgo/framework/torch2paddle/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/mapper/device.py` & `antgo-0.1.4/antgo/framework/torch2paddle/mapper/device.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/mapper/distributed.py` & `antgo-0.1.4/antgo/framework/torch2paddle/mapper/distributed.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/mapper/io.py` & `antgo-0.1.4/antgo/framework/torch2paddle/mapper/io.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/mapper/layer.py` & `antgo-0.1.4/antgo/framework/torch2paddle/mapper/layer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/mapper/nn.py` & `antgo-0.1.4/antgo/framework/torch2paddle/mapper/nn.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/mapper/nn_functional.py` & `antgo-0.1.4/antgo/framework/torch2paddle/mapper/nn_functional.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/mapper/nn_init.py` & `antgo-0.1.4/antgo/framework/torch2paddle/mapper/nn_init.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/mapper/nn_utils.py` & `antgo-0.1.4/antgo/framework/torch2paddle/mapper/nn_utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/mapper/ops.py` & `antgo-0.1.4/antgo/framework/torch2paddle/mapper/ops.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/mapper/optimizer.py` & `antgo-0.1.4/antgo/framework/torch2paddle/mapper/optimizer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/mapper/parambase.py` & `antgo-0.1.4/antgo/framework/torch2paddle/mapper/parambase.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/mapper/tensor.py` & `antgo-0.1.4/antgo/framework/torch2paddle/mapper/tensor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/mapper/varbase.py` & `antgo-0.1.4/antgo/framework/torch2paddle/mapper/varbase.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/tools/ast_update.py` & `antgo-0.1.4/antgo/framework/torch2paddle/tools/ast_update.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/tools/convert.py` & `antgo-0.1.4/antgo/framework/torch2paddle/tools/convert.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/tools/dependency_analyzer.py` & `antgo-0.1.4/antgo/framework/torch2paddle/tools/dependency_analyzer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/tools/utils.py` & `antgo-0.1.4/antgo/framework/torch2paddle/tools/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/utils.py` & `antgo-0.1.4/antgo/framework/torch2paddle/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/vision/datasets.py` & `antgo-0.1.4/antgo/framework/torch2paddle/vision/datasets.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/vision/transforms.py` & `antgo-0.1.4/antgo/framework/torch2paddle/vision/transforms.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/framework/torch2paddle/vision/utils.py` & `antgo-0.1.4/antgo/framework/torch2paddle/vision/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/help.py` & `antgo-0.1.4/antgo/help.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/interactcontext.py` & `antgo-0.1.4/antgo/interactcontext.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/main.py` & `antgo-0.1.4/antgo/main.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/main_backup.py` & `antgo-0.1.4/antgo/main_backup.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/__init__.py` & `antgo-0.1.4/antgo/measures/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/ali_fashion_attribute_error.py` & `antgo-0.1.4/antgo/measures/ali_fashion_attribute_error.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/ali_fashion_landmark_ne.py` & `antgo-0.1.4/antgo/measures/ali_fashion_landmark_ne.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/average_precision.py` & `antgo-0.1.4/antgo/measures/average_precision.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/base.py` & `antgo-0.1.4/antgo/measures/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/binary_c.py` & `antgo-0.1.4/antgo/measures/binary_c.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/binomial_deviance.py` & `antgo-0.1.4/antgo/measures/binomial_deviance.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/confusion_matrix.py` & `antgo-0.1.4/antgo/measures/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/crowdsource.py` & `antgo-0.1.4/antgo/measures/crowdsource.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/deep_analysis.py` & `antgo-0.1.4/antgo/measures/deep_analysis.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/error.py` & `antgo-0.1.4/antgo/measures/error.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/face_task.py` & `antgo-0.1.4/antgo/measures/face_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/kdd_average_precision.py` & `antgo-0.1.4/antgo/measures/kdd_average_precision.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/matting_task.py` & `antgo-0.1.4/antgo/measures/matting_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/moving_statistic.py` & `antgo-0.1.4/antgo/measures/moving_statistic.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/multi_c.py` & `antgo-0.1.4/antgo/measures/multi_c.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/multic_task.py` & `antgo-0.1.4/antgo/measures/multic_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/multil_task.py` & `antgo-0.1.4/antgo/measures/multil_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/objdect_task.py` & `antgo-0.1.4/antgo/measures/objdect_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/pck.py` & `antgo-0.1.4/antgo/measures/pck.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/person_search_task.py` & `antgo-0.1.4/antgo/measures/person_search_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/precision_recall.py` & `antgo-0.1.4/antgo/measures/precision_recall.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/quadratic_weighted_kappa.py` & `antgo-0.1.4/antgo/measures/quadratic_weighted_kappa.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/regression_metric.py` & `antgo-0.1.4/antgo/measures/regression_metric.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/regression_task.py` & `antgo-0.1.4/antgo/measures/regression_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/repeat_statistic.py` & `antgo-0.1.4/antgo/measures/repeat_statistic.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/roc_auc.py` & `antgo-0.1.4/antgo/measures/roc_auc.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/segmentation_task.py` & `antgo-0.1.4/antgo/measures/segmentation_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/significance.py` & `antgo-0.1.4/antgo/measures/significance.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/statistic.py` & `antgo-0.1.4/antgo/measures/statistic.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/topk.py` & `antgo-0.1.4/antgo/measures/topk.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/track_task.py` & `antgo-0.1.4/antgo/measures/track_task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/measures/yesno_crowdsource.py` & `antgo-0.1.4/antgo/measures/yesno_crowdsource.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/engine/__init__.py` & `antgo-0.1.4/antgo/pipeline/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/engine/execution/base_execution.py` & `antgo-0.1.4/antgo/pipeline/engine/execution/base_execution.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/engine/factory.py` & `antgo-0.1.4/antgo/pipeline/engine/factory.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/engine/operator_loader.py` & `antgo-0.1.4/antgo/pipeline/engine/operator_loader.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/engine/operator_registry.py` & `antgo-0.1.4/antgo/pipeline/engine/operator_registry.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/engine/uri.py` & `antgo-0.1.4/antgo/pipeline/engine/uri.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/__init__.py` & `antgo-0.1.4/antgo/pipeline/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/common/util.py` & `antgo-0.1.4/antgo/pipeline/functional/common/util.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/data_collection.py` & `antgo-0.1.4/antgo/pipeline/functional/data_collection.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/entity.py` & `antgo-0.1.4/antgo/pipeline/functional/entity.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/image/__init__.py` & `antgo-0.1.4/antgo/pipeline/functional/image/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/image/io.py` & `antgo-0.1.4/antgo/pipeline/functional/image/io.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/image/plot.py` & `antgo-0.1.4/antgo/pipeline/functional/image/plot.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/image/process.py` & `antgo-0.1.4/antgo/pipeline/functional/image/process.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/mixins/__init__.py` & `antgo-0.1.4/antgo/pipeline/functional/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/mixins/column.py` & `antgo-0.1.4/antgo/pipeline/functional/mixins/column.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/mixins/computer_vision.py` & `antgo-0.1.4/antgo/pipeline/functional/mixins/computer_vision.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/mixins/config.py` & `antgo-0.1.4/antgo/pipeline/functional/mixins/config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/mixins/dag.py` & `antgo-0.1.4/antgo/pipeline/functional/mixins/dag.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/mixins/data_processing.py` & `antgo-0.1.4/antgo/pipeline/functional/mixins/data_processing.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/mixins/dataframe.py` & `antgo-0.1.4/antgo/pipeline/functional/mixins/dataframe.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/mixins/dataset.py` & `antgo-0.1.4/antgo/pipeline/functional/mixins/dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/mixins/demo.py` & `antgo-0.1.4/antgo/pipeline/functional/mixins/demo.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/mixins/dispatcher.py` & `antgo-0.1.4/antgo/pipeline/functional/mixins/dispatcher.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/mixins/list.py` & `antgo-0.1.4/antgo/pipeline/functional/mixins/list.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/mixins/serve.py` & `antgo-0.1.4/antgo/pipeline/functional/mixins/serve.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/mixins/show.py` & `antgo-0.1.4/antgo/pipeline/functional/mixins/show.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/mixins/stream.py` & `antgo-0.1.4/antgo/pipeline/functional/mixins/stream.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/option.py` & `antgo-0.1.4/antgo/pipeline/functional/option.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/functional/storages.py` & `antgo-0.1.4/antgo/pipeline/functional/storages.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/hparam/__init__.py` & `antgo-0.1.4/antgo/pipeline/hparam/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/hparam/hyperparameter.py` & `antgo-0.1.4/antgo/pipeline/hparam/hyperparameter.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/hub/builtin/operators/inference_model_op.py` & `antgo-0.1.4/antgo/pipeline/hub/builtin/operators/inference_model_op.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/hub/builtin/operators/inference_onnx_op.py` & `antgo-0.1.4/antgo/pipeline/hub/builtin/operators/inference_onnx_op.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/hub/builtin/operators/runas_op.py` & `antgo-0.1.4/antgo/pipeline/hub/builtin/operators/runas_op.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/hub/external/mm/detector.py` & `antgo-0.1.4/antgo/pipeline/hub/external/mm/detector.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/hub/external/mm/inpainting.py` & `antgo-0.1.4/antgo/pipeline/hub/external/mm/inpainting.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/hub/external/mm/ocr.py` & `antgo-0.1.4/antgo/pipeline/hub/external/mm/ocr.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/hub/external/mm/pose.py` & `antgo-0.1.4/antgo/pipeline/hub/external/mm/pose.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/hub/external/mm/restoration.py` & `antgo-0.1.4/antgo/pipeline/hub/external/mm/restoration.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/hub/external/mm/segmentor.py` & `antgo-0.1.4/antgo/pipeline/hub/external/mm/segmentor.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/models/cfg/dataset/coco.yaml` & `antgo-0.1.4/antgo/pipeline/models/cfg/dataset/coco.yaml`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/models/cfg/detector/yolov7-e6.yaml` & `antgo-0.1.4/antgo/pipeline/models/cfg/detector/yolov7-e6.yaml`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/models/cfg/detector/yolov7-w6.yaml` & `antgo-0.1.4/antgo/pipeline/models/cfg/detector/yolov7-w6.yaml`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/models/cfg/detector/yolov7.yaml` & `antgo-0.1.4/antgo/pipeline/models/cfg/detector/yolov7.yaml`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/models/cfg/detector/yolov7x.yaml` & `antgo-0.1.4/antgo/pipeline/models/cfg/detector/yolov7x.yaml`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/models/detector/util.py` & `antgo-0.1.4/antgo/pipeline/models/detector/util.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/models/detector/yolov7/util.py` & `antgo-0.1.4/antgo/pipeline/models/detector/yolov7/util.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/models/detector/yolov7/yolov7.py` & `antgo-0.1.4/antgo/pipeline/models/detector/yolov7/yolov7.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/models/utils/common.py` & `antgo-0.1.4/antgo/pipeline/models/utils/common.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/models/utils/preprocess.py` & `antgo-0.1.4/antgo/pipeline/models/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/models/utils/utils.py` & `antgo-0.1.4/antgo/pipeline/models/utils/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/operators/base.py` & `antgo-0.1.4/antgo/pipeline/operators/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/operators/nop.py` & `antgo-0.1.4/antgo/pipeline/operators/nop.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/pipeline/utils/repo_normalize.py` & `antgo-0.1.4/antgo/pipeline/utils/repo_normalize.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/css/359.32c5c11e.css` & `antgo-0.1.4/antgo/resource/app/css/359.32c5c11e.css`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/css/385.1759eef9.css` & `antgo-0.1.4/antgo/resource/app/css/385.1759eef9.css`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/css/chunk-vendors.1944359c.css` & `antgo-0.1.4/antgo/resource/app/css/chunk-vendors.1944359c.css`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/favicon.ico` & `antgo-0.1.4/antgo/resource/app/favicon.ico`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/index.html` & `antgo-0.1.4/antgo/resource/app/index.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/js/359.afb86915.js` & `antgo-0.1.4/antgo/resource/app/js/359.afb86915.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/js/359.afb86915.js.map` & `antgo-0.1.4/antgo/resource/app/js/359.afb86915.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/js/385.90ba0f66.js` & `antgo-0.1.4/antgo/resource/app/js/385.90ba0f66.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/js/385.90ba0f66.js.map` & `antgo-0.1.4/antgo/resource/app/js/385.90ba0f66.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/js/532.f949def3.js` & `antgo-0.1.4/antgo/resource/app/js/532.f949def3.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/js/532.f949def3.js.map` & `antgo-0.1.4/antgo/resource/app/js/532.f949def3.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/js/651.c5601578.js` & `antgo-0.1.4/antgo/resource/app/js/651.c5601578.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/js/651.c5601578.js.map` & `antgo-0.1.4/antgo/resource/app/js/651.c5601578.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/js/769.b7247054.js` & `antgo-0.1.4/antgo/resource/app/js/769.b7247054.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/js/769.b7247054.js.map` & `antgo-0.1.4/antgo/resource/app/js/769.b7247054.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/js/854.d3c0e54f.js` & `antgo-0.1.4/antgo/resource/app/js/854.d3c0e54f.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/js/854.d3c0e54f.js.map` & `antgo-0.1.4/antgo/resource/app/js/854.d3c0e54f.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/js/880.cba02e88.js` & `antgo-0.1.4/antgo/resource/app/js/880.cba02e88.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/js/880.cba02e88.js.map` & `antgo-0.1.4/antgo/resource/app/js/880.cba02e88.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/js/app.f01f9b7a.js` & `antgo-0.1.4/antgo/resource/app/js/app.f01f9b7a.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/js/app.f01f9b7a.js.map` & `antgo-0.1.4/antgo/resource/app/js/app.f01f9b7a.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/js/chunk-vendors.18913786.js` & `antgo-0.1.4/antgo/resource/app/js/chunk-vendors.18913786.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/app/js/chunk-vendors.18913786.js.map` & `antgo-0.1.4/antgo/resource/app/js/chunk-vendors.18913786.js.map`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/dataset/3dpw.txt` & `antgo-0.1.4/antgo/resource/dataset/3dpw.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/dataset/ade20k.txt` & `antgo-0.1.4/antgo/resource/dataset/ade20k.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/dataset/cityscapes.txt` & `antgo-0.1.4/antgo/resource/dataset/cityscapes.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/dataset/coco.txt` & `antgo-0.1.4/antgo/resource/dataset/coco.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/dataset/flic.txt` & `antgo-0.1.4/antgo/resource/dataset/flic.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/dataset/h36m.txt` & `antgo-0.1.4/antgo/resource/dataset/h36m.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/dataset/lfw.txt` & `antgo-0.1.4/antgo/resource/dataset/lfw.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/dataset/lip.txt` & `antgo-0.1.4/antgo/resource/dataset/lip.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/dataset/lsp.txt` & `antgo-0.1.4/antgo/resource/dataset/lsp.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/dataset/mpii.txt` & `antgo-0.1.4/antgo/resource/dataset/mpii.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/dataset/vgg-face2-data.txt` & `antgo-0.1.4/antgo/resource/dataset/vgg-face2-data.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/dataset/vgg-face2-meta.txt` & `antgo-0.1.4/antgo/resource/dataset/vgg-face2-meta.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/dataset/voc.txt` & `antgo-0.1.4/antgo/resource/dataset/voc.txt`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/html.py` & `antgo-0.1.4/antgo/resource/html.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/static/antgo.ico` & `antgo-0.1.4/antgo/resource/static/antgo.ico`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/static/antgo.js` & `antgo-0.1.4/antgo/resource/static/antgo.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/static/apply.png` & `antgo-0.1.4/antgo/resource/static/apply.png`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/static/banner.png` & `antgo-0.1.4/antgo/resource/static/banner.png`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/static/card.png` & `antgo-0.1.4/antgo/resource/static/card.png`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/static/filetree.png` & `antgo-0.1.4/antgo/resource/static/filetree.png`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/static/holder.min.js` & `antgo-0.1.4/antgo/resource/static/holder.min.js`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/static/register.png` & `antgo-0.1.4/antgo/resource/static/register.png`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/static/start-experiment.png` & `antgo-0.1.4/antgo/resource/static/start-experiment.png`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/activelearning.html` & `antgo-0.1.4/antgo/resource/templates/activelearning.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/crowdsource.html` & `antgo-0.1.4/antgo/resource/templates/crowdsource.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/demo.html` & `antgo-0.1.4/antgo/resource/templates/demo.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/mvp/README.md` & `antgo-0.1.4/antgo/resource/templates/mvp/README.md`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/mvp/cifar10/configs/config.py` & `antgo-0.1.4/antgo/resource/templates/mvp/cifar10/configs/config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/mvp/cifar10/dataset.py` & `antgo-0.1.4/antgo/resource/templates/mvp/cifar10/dataset.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/mvp/cifar10/hooks.py` & `antgo-0.1.4/antgo/resource/templates/mvp/cifar10/hooks.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/mvp/cifar10/main.py` & `antgo-0.1.4/antgo/resource/templates/mvp/cifar10/main.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/mvp/cifar10/metrics.py` & `antgo-0.1.4/antgo/resource/templates/mvp/cifar10/metrics.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/mvp/cifar10/models/wideres.py` & `antgo-0.1.4/antgo/resource/templates/mvp/cifar10/models/wideres.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/mvp/coco_config.py` & `antgo-0.1.4/antgo/resource/templates/mvp/coco_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 model = dict(
     type='TTFNet',
     backbone=dict(
         type='ResNet',
         depth=50, 
         in_channels=3, 
         out_indices=[3,2,1]),      
-    neck=dict(type="FPN", in_channels=[512, 1024, 2048], out_channels=256, num_outs=3),
+    neck=dict(type="FPN", in_channels=[512, 1024, 2048], out_channels=256, num_outs=3, upsample_cfg=dict(mode='bilinear', scale_factor=2.0)),
     bbox_head=dict(
         type='FcosHeadML',
         in_channel=256,
         feat_channel=256,
         num_classes=80,
         down_stride=[8,16,32],
         score_thresh=0.05,
@@ -47,17 +47,17 @@
 data=dict(
     train=dict(
         type='COCO2017',
         train_or_test='train',
         dir='./coco_dataset',
         ext_params={'task_type': 'OBJECT-DETECTION'},
         pipeline=[
-            dict(type="Rotation", degree=15),
+            dict(type="Rotation", degree=30),
             dict(type='ResizeByShort', short_size=800, max_size=1333),
-            dict(type='ColorDistort', hue=[-5,5,0.3], saturation=[0.8,1.2,0.3], contrast=[0.8,1.2,0.3], brightness=[0.8,1.2,0.3]),
+            dict(type='ColorDistort', hue=[-5,5,0.5], saturation=[0.7,1.3,0.5], contrast=[0.7,1.3,0.5], brightness=[0.7,1.3,0.5]),
             dict(type='RandomFlipImage', swap_labels=[]),
             dict(type='INormalize', mean=[128.0,128.0,128.0], std=[128.0,128.0,128.0],to_rgb=False, keys=['image']),
             dict(type='Permute', to_bgr=False, channel_first=True)
         ],
         inputs_def=dict(
             fields = ["image", 'bboxes', 'labels', 'image_meta']
         )
```

### Comparing `antgo-0.1.3/antgo/resource/templates/mvp/config.py` & `antgo-0.1.4/antgo/resource/templates/mvp/config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/mvp/lsp_config.py` & `antgo-0.1.4/antgo/resource/templates/mvp/lsp_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/mvp/pascal_voc_config.py` & `antgo-0.1.4/antgo/resource/templates/mvp/pascal_voc_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/mvp/system.py` & `antgo-0.1.4/antgo/resource/templates/mvp/system.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/mvp/visalso_config.py` & `antgo-0.1.4/antgo/resource/templates/mvp/visalso_config.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/project.json` & `antgo-0.1.4/antgo/resource/templates/project.json`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/sample_gt.json` & `antgo-0.1.4/antgo/resource/templates/sample_gt.json`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/statistic-report.html` & `antgo-0.1.4/antgo/resource/templates/statistic-report.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/task_main_file.template` & `antgo-0.1.4/antgo/resource/templates/task_main_file.template`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/task_main_param.template` & `antgo-0.1.4/antgo/resource/templates/task_main_param.template`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/task_shell.template` & `antgo-0.1.4/antgo/resource/templates/task_shell.template`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/trainmaster.html` & `antgo-0.1.4/antgo/resource/templates/trainmaster.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/resource/templates/yesno_crowdsource.html` & `antgo-0.1.4/antgo/resource/templates/yesno_crowdsource.html`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/sandbox/sandbox.py` & `antgo-0.1.4/antgo/sandbox/sandbox.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/script/base.py` & `antgo-0.1.4/antgo/script/base.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/script/create_dataset_share.py` & `antgo-0.1.4/antgo/script/create_dataset_share.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/script/custom_submit.py` & `antgo-0.1.4/antgo/script/custom_submit.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/script/data_convert_cifar10_tfrecord.py` & `antgo-0.1.4/antgo/script/data_convert_cifar10_tfrecord.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/script/data_prepare.py` & `antgo-0.1.4/antgo/script/data_prepare.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/script/local_submit.py` & `antgo-0.1.4/antgo/script/local_submit.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/script/ssh-submit.sh` & `antgo-0.1.4/antgo/script/ssh-submit.sh`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/script/ssh_submit.py` & `antgo-0.1.4/antgo/script/ssh_submit.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/task/task.py` & `antgo-0.1.4/antgo/task/task.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/tools/__init__.py` & `antgo-0.1.4/antgo/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/tools/browser_funcs.py` & `antgo-0.1.4/antgo/tools/browser_funcs.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/tools/download_funcs.py` & `antgo-0.1.4/antgo/tools/download_funcs.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/tools/extract.py` & `antgo-0.1.4/antgo/tools/extract.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/tools/filter_funcs.py` & `antgo-0.1.4/antgo/tools/filter_funcs.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/tools/label_funcs.py` & `antgo-0.1.4/antgo/tools/label_funcs.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/tools/package.py` & `antgo-0.1.4/antgo/tools/package.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/tools/share_funcs.py` & `antgo-0.1.4/antgo/tools/share_funcs.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/_bbox.pyx` & `antgo-0.1.4/antgo/utils/_bbox.pyx`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/_encode_png.pyx` & `antgo-0.1.4/antgo/utils/_encode_png.pyx`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/_mask.pyx` & `antgo-0.1.4/antgo/utils/_mask.pyx`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/args.py` & `antgo-0.1.4/antgo/utils/args.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/argscope.py` & `antgo-0.1.4/antgo/utils/argscope.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/colormap.py` & `antgo-0.1.4/antgo/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/concurrency.py` & `antgo-0.1.4/antgo/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/cpu.py` & `antgo-0.1.4/antgo/utils/cpu.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/encode.py` & `antgo-0.1.4/antgo/utils/encode.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/fs.py` & `antgo-0.1.4/antgo/utils/fs.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/gpu.py` & `antgo-0.1.4/antgo/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/logger.py` & `antgo-0.1.4/antgo/utils/logger.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/mask.py` & `antgo-0.1.4/antgo/utils/mask.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/netvis.py` & `antgo-0.1.4/antgo/utils/netvis.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/parallel_map.py` & `antgo-0.1.4/antgo/utils/parallel_map.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/pickledb.py` & `antgo-0.1.4/antgo/utils/pickledb.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/processbar.py` & `antgo-0.1.4/antgo/utils/processbar.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/sample_gt.py` & `antgo-0.1.4/antgo/utils/sample_gt.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/serialize.py` & `antgo-0.1.4/antgo/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/shared_queue/__init__.py` & `antgo-0.1.4/antgo/utils/shared_queue/__init__.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/shared_queue/queue.py` & `antgo-0.1.4/antgo/utils/shared_queue/queue.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/shared_queue/sharedmemory.py` & `antgo-0.1.4/antgo/utils/shared_queue/sharedmemory.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/timer.py` & `antgo-0.1.4/antgo/utils/timer.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo/utils/utils.py` & `antgo-0.1.4/antgo/utils/utils.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/antgo.egg-info/PKG-INFO` & `antgo-0.1.4/antgo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antgo
-Version: 0.1.3
+Version: 0.1.4
 Summary: machine learning experiment platform
 Home-page: https://github.com/jianzfb/antgo
 Author: jian
 Author-email: jian@mltalker.com
 License-File: LICENSE.md
 
 ======================
```

### Comparing `antgo-0.1.3/antgo.egg-info/SOURCES.txt` & `antgo-0.1.4/antgo.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
 antgo/framework/helper/models/detectors/core/mask/utils.py
 antgo/framework/helper/models/detectors/core/utils/__init__.py
 antgo/framework/helper/models/detectors/core/utils/dist_utils.py
 antgo/framework/helper/models/detectors/core/utils/misc.py
 antgo/framework/helper/models/detectors/head/__init__.py
 antgo/framework/helper/models/detectors/head/base_dense_head.py
 antgo/framework/helper/models/detectors/head/fcos_head.py
-antgo/framework/helper/models/detectors/head/focs_head_ml.py
+antgo/framework/helper/models/detectors/head/fcos_head_ml.py
 antgo/framework/helper/models/detectors/losses/__init__.py
 antgo/framework/helper/models/detectors/losses/accuracy.py
 antgo/framework/helper/models/detectors/losses/ae_loss.py
 antgo/framework/helper/models/detectors/losses/balanced_l1_loss.py
 antgo/framework/helper/models/detectors/losses/cross_entropy_loss.py
 antgo/framework/helper/models/detectors/losses/dice_loss.py
 antgo/framework/helper/models/detectors/losses/focal_loss.py
```

### Comparing `antgo-0.1.3/setup.py` & `antgo-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 def read_requirements(filename):
     return [line.strip() for line in read_file(filename).splitlines()
             if not line.startswith('#')]
 
 
 setup(name='antgo',
-      version='0.1.3',
+      version='0.1.4',
       description='machine learning experiment platform',
       __short_description__='machine learning experiment platform',
       url='https://github.com/jianzfb/antgo',
       author='jian',
       author_email='jian@mltalker.com',
       setup_requires=[
         # Setuptools 18.0 properly handles Cython extensions.
```

### Comparing `antgo-0.1.3/test/test_antgo.py` & `antgo-0.1.4/test/test_antgo.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/test/test_paddle_c.py` & `antgo-0.1.4/test/test_paddle_c.py`

 * *Files identical despite different names*

### Comparing `antgo-0.1.3/test/test_torch_c.py` & `antgo-0.1.4/test/test_torch_c.py`

 * *Files identical despite different names*


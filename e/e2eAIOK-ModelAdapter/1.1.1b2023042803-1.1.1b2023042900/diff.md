# Comparing `tmp/e2eAIOK-ModelAdapter-1.1.1b2023042803.tar.gz` & `tmp/e2eAIOK-ModelAdapter-1.1.1b2023042900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/e2eAIOK-ModelAdapter-1.1.1b2023042803.tar", last modified: Fri Apr 28 03:17:25 2023, max compression
+gzip compressed data, was "dist/e2eAIOK-ModelAdapter-1.1.1b2023042900.tar", last modified: Sat Apr 29 00:21:18 2023, max compression
```

## Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803.tar` & `e2eAIOK-ModelAdapter-1.1.1b2023042900.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/backbone/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/backbone/unet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/backbone/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/dataset/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/dataset/composed_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/dataset/office31.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/default_ma.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/distiller/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/distiller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/distiller/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/distiller/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/finetunner/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/finetunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py
--rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5444 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/training/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/training/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    18985 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/training/train.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/default.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/asr/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/asr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/cv/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/data_builder_asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/data_builder_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/data_builder_nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/data_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/data_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/data_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/data_utils/image_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/data_utils/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/model/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/model/cv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/model/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/model/cv/lenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/model/cv/resnet_cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/model/model_builder_asr.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/model/model_builder_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/model/model_builder_nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/model/model_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/model/model_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/model/model_utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/torch_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/utils/extend_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-28 03:17:21.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 03:17:24.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK_ModelAdapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-28 03:17:24.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK_ModelAdapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-28 03:17:24.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK_ModelAdapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 03:17:24.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK_ModelAdapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 03:17:24.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK_ModelAdapter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 03:17:24.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK_ModelAdapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 03:17:24.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK_ModelAdapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 03:17:25.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-28 03:17:24.000000 e2eAIOK-ModelAdapter-1.1.1b2023042803/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/backbone/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/backbone/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/backbone/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/dataset/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/dataset/composed_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/dataset/office31.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/default_ma.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/traditional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/distiller/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/distiller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/distiller/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/distiller/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/finetunner/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/finetunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5444 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/training/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/training/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18985 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/training/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/default.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/asr/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/asr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/data_builder_asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/data_builder_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/data_builder_nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/data_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/data_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/data_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/data_utils/image_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/data_utils/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/model/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/model/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/model/cv/lenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/model/cv/resnet_cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/model/model_builder_asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/model/model_builder_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/model/model_builder_nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/model/model_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/model/model_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/model/model_utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/torch_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/utils/extend_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-29 00:21:10.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-29 00:21:16.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK_ModelAdapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-29 00:21:17.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK_ModelAdapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK_ModelAdapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:21:17.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK_ModelAdapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:21:17.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK_ModelAdapter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-29 00:21:17.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK_ModelAdapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-29 00:21:17.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK_ModelAdapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 00:21:18.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-29 00:21:16.000000 e2eAIOK-ModelAdapter-1.1.1b2023042900/setup.py
```

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/PKG-INFO` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2eAIOK-ModelAdapter
-Version: 1.1.1b2023042803
+Version: 1.1.1b2023042900
 Summary: Intel® End-to-End AI Optimization Kit
 Home-page: https://github.com/intel/e2eAIOK
 Author: INTEL
 License: Apache License
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/issues
 Description: # [Intel® End-to-End AI Optimization Kit](https://github.com/intel/e2eAIOK)
```

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/README.md` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/README.md`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/backbone/factory.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/backbone/factory.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/backbone/unet/generic_UNet_DA.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/dataset/__init__.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/dataset/cifar.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/dataset/cifar.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/dataset/composed_dataset.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/dataset/composed_dataset.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/dataset/office31.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/dataset/office31.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/default_ma.conf` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/default_ma.conf`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/DA_Loss.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/adversarial_adapter.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/cdan_adapter.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/dann_adapter.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/discriminator.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/adversarial/grl.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/adapter/factory.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/distiller/basic_distiller.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/distiller/dkd.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/distiller/kd.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/distiller/utils/aug_random.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/distiller/utils/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/distiller/utils/deal_logits.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/distiller/utils/manager.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/finetunner/basic_finetunner.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/engine_core/transferrable_model.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/main.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/main.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/training/task.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/training/task.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/ModelAdapter/training/train.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/ModelAdapter/training/train.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/default.conf` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/default.conf`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/asr/data_builder_librispeech.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/cv/data_builder_cifar.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/cv/data_builder_imagenet.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/cv/data_builder_uspsvsminist.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/data_builder_asr.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/data_builder_asr.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/data_builder_cv.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/data_builder_cv.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/data_builder_nlp.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/data_builder_nlp.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/data_utils/data_utils.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/data_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/data_utils/image_list.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/data_utils/image_list.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data/nlp/data_builder_squad.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/data_builder.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/data_builder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/model/cv/lenet.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/model/cv/lenet.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/model/cv/resnet_cifar.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/model/cv/resnet_cifar.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/model/model_utils/model_utils.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/model/model_utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/model_builder.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/model_builder.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/torch_trainer.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/torch_trainer.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/utils/extend_distributed.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/utils/extend_distributed.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/trainer/utils/utils.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/trainer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK/common/utils.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK/common/utils.py`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK_ModelAdapter.egg-info/PKG-INFO` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK_ModelAdapter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2eAIOK-ModelAdapter
-Version: 1.1.1b2023042803
+Version: 1.1.1b2023042900
 Summary: Intel® End-to-End AI Optimization Kit
 Home-page: https://github.com/intel/e2eAIOK
 Author: INTEL
 License: Apache License
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/issues
 Description: # [Intel® End-to-End AI Optimization Kit](https://github.com/intel/e2eAIOK)
```

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/e2eAIOK_ModelAdapter.egg-info/SOURCES.txt` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/e2eAIOK_ModelAdapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e2eAIOK-ModelAdapter-1.1.1b2023042803/setup.py` & `e2eAIOK-ModelAdapter-1.1.1b2023042900/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/hcpdiff-0.2.0.tar.gz` & `tmp/hcpdiff-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcpdiff-0.2.0.tar", last modified: Tue Apr 25 10:12:54 2023, max compression
+gzip compressed data, was "hcpdiff-0.2.1.tar", last modified: Sat Apr 29 03:27:33 2023, max compression
```

## Comparing `hcpdiff-0.2.0.tar` & `hcpdiff-0.2.1.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.134604 hcpdiff-0.2.0/
--rw-rw-rw-   0        0        0    11558 2023-04-11 12:44:40.000000 hcpdiff-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     5477 2023-04-25 10:12:54.133605 hcpdiff-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4740 2023-04-24 07:27:38.000000 hcpdiff-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.077252 hcpdiff-0.2.0/cfgs/
-drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.080242 hcpdiff-0.2.0/cfgs/infer/
--rw-rw-rw-   0        0        0      179 2023-04-11 09:59:00.000000 hcpdiff-0.2.0/cfgs/infer/change_vae.yaml
--rw-rw-rw-   0        0        0      672 2023-04-12 10:04:24.000000 hcpdiff-0.2.0/cfgs/infer/euler_a.yaml
--rw-rw-rw-   0        0        0     1659 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/cfgs/infer/img2img.yaml
--rw-rw-rw-   0        0        0     1804 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/cfgs/infer/img2img_controlnet.yaml
--rw-rw-rw-   0        0        0     1554 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/cfgs/infer/text2img.yaml
--rw-rw-rw-   0        0        0     9971 2023-03-22 01:36:55.000000 hcpdiff-0.2.0/cfgs/te_struct.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.083243 hcpdiff-0.2.0/cfgs/train/
-drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.089254 hcpdiff-0.2.0/cfgs/train/examples/
--rw-rw-rw-   0        0        0     1846 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/cfgs/train/examples/CustomDiffusion.yaml
--rw-rw-rw-   0        0        0     2815 2023-04-15 14:19:44.000000 hcpdiff-0.2.0/cfgs/train/examples/DreamArtist++.yaml
--rw-rw-rw-   0        0        0     1334 2023-04-12 06:39:19.000000 hcpdiff-0.2.0/cfgs/train/examples/DreamArtist.yaml
--rw-rw-rw-   0        0        0     1644 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/cfgs/train/examples/DreamBooth.yaml
--rw-rw-rw-   0        0        0     1124 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/cfgs/train/examples/TextualInversion.yaml
--rw-rw-rw-   0        0        0     1178 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/cfgs/train/examples/fine-tuning.yaml
--rw-rw-rw-   0        0        0     1397 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/cfgs/train/examples/locon.yaml
--rw-rw-rw-   0        0        0     1228 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/cfgs/train/examples/lora_conventional.yaml
--rw-rw-rw-   0        0        0      343 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/cfgs/train/plugin_control.yaml
--rw-rw-rw-   0        0        0     2904 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/cfgs/train/train_base.yaml
--rw-rw-rw-   0        0        0     1241 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/cfgs/train/tuning_base.yaml
--rw-rw-rw-   0        0        0    46121 2023-03-22 01:36:55.000000 hcpdiff-0.2.0/cfgs/unet_struct.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.093458 hcpdiff-0.2.0/hcpdiff/
--rw-rw-rw-   0        0        0        0 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.101451 hcpdiff-0.2.0/hcpdiff/data/
--rw-rw-rw-   0        0        0      138 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/data/__init__.py
--rw-rw-rw-   0        0        0     8678 2023-04-11 12:47:28.000000 hcpdiff-0.2.0/hcpdiff/data/bucket.py
--rw-rw-rw-   0        0        0     5732 2023-04-17 09:36:22.000000 hcpdiff-0.2.0/hcpdiff/data/pair_dataset.py
--rw-rw-rw-   0        0        0     1686 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.109275 hcpdiff-0.2.0/hcpdiff/models/
--rw-rw-rw-   0        0        0      295 2023-04-15 14:19:44.000000 hcpdiff-0.2.0/hcpdiff/models/__init__.py
--rw-rw-rw-   0        0        0     1422 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/models/cfg_context.py
--rw-rw-rw-   0        0        0     7719 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/hcpdiff/models/controlnet.py
--rw-rw-rw-   0        0        0     3068 2023-04-11 12:47:28.000000 hcpdiff-0.2.0/hcpdiff/models/layers.py
--rw-rw-rw-   0        0        0     7949 2023-04-17 08:00:11.000000 hcpdiff-0.2.0/hcpdiff/models/lora_base.py
--rw-rw-rw-   0        0        0     7735 2023-04-17 08:00:11.000000 hcpdiff-0.2.0/hcpdiff/models/lora_layers.py
--rw-rw-rw-   0        0        0     6045 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/hcpdiff/models/plugin.py
--rw-rw-rw-   0        0        0     3957 2023-04-20 07:56:10.000000 hcpdiff-0.2.0/hcpdiff/models/text_emb_ex.py
--rw-rw-rw-   0        0        0     5784 2023-04-20 07:56:10.000000 hcpdiff-0.2.0/hcpdiff/models/textencoder_ex.py
--rw-rw-rw-   0        0        0     2440 2023-04-14 04:04:05.000000 hcpdiff-0.2.0/hcpdiff/models/tokenizer_ex.py
-drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.115275 hcpdiff-0.2.0/hcpdiff/tools/
--rw-rw-rw-   0        0        0        0 2023-04-12 06:39:19.000000 hcpdiff-0.2.0/hcpdiff/tools/__init__.py
--rw-rw-rw-   0        0        0      753 2023-04-12 08:25:47.000000 hcpdiff-0.2.0/hcpdiff/tools/convert_caption_txt2json.py
--rw-rw-rw-   0        0        0     1981 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/tools/create_embedding.py
--rw-rw-rw-   0        0        0     1718 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/tools/gen_from_ptlist.py
--rw-rw-rw-   0        0        0      654 2023-04-12 07:55:01.000000 hcpdiff-0.2.0/hcpdiff/tools/init_proj.py
--rw-rw-rw-   0        0        0     4585 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/tools/merge_model_part.py
--rw-rw-rw-   0        0        0     8536 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/hcpdiff/tools/sd2diffusers.py
--rw-rw-rw-   0        0        0    25035 2023-04-20 07:56:10.000000 hcpdiff-0.2.0/hcpdiff/train_ac.py
--rw-rw-rw-   0        0        0     3683 2023-04-20 07:56:10.000000 hcpdiff-0.2.0/hcpdiff/train_ac_single.py
--rw-rw-rw-   0        0        0     8448 2023-04-20 07:56:10.000000 hcpdiff-0.2.0/hcpdiff/train_colo.py
-drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.121606 hcpdiff-0.2.0/hcpdiff/utils/
--rw-rw-rw-   0        0        0        0 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/utils/__init__.py
--rw-rw-rw-   0        0        0     2865 2023-04-12 06:39:19.000000 hcpdiff-0.2.0/hcpdiff/utils/caption_tools.py
--rw-rw-rw-   0        0        0    11320 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/hcpdiff/utils/cfg_net_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.123604 hcpdiff-0.2.0/hcpdiff/utils/ckpt_manager/
--rw-rw-rw-   0        0        0       82 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/utils/ckpt_manager/__init__.py
--rw-rw-rw-   0        0        0     3197 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/hcpdiff/utils/ckpt_manager/ckpt_pkl.py
--rw-rw-rw-   0        0        0     1884 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/hcpdiff/utils/ckpt_manager/ckpt_safetensor.py
--rw-rw-rw-   0        0        0      860 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/utils/colo_utils.py
--rw-rw-rw-   0        0        0     3065 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/utils/ema.py
--rw-rw-rw-   0        0        0      468 2023-04-17 09:36:22.000000 hcpdiff-0.2.0/hcpdiff/utils/emb_utils.py
--rw-rw-rw-   0        0        0     8680 2023-04-11 12:30:15.000000 hcpdiff-0.2.0/hcpdiff/utils/img_size_tool.py
--rw-rw-rw-   0        0        0     5713 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/hcpdiff/utils/net_utils.py
--rw-rw-rw-   0        0        0     2835 2023-04-20 07:56:10.000000 hcpdiff-0.2.0/hcpdiff/utils/utils.py
--rw-rw-rw-   0        0        0     7299 2023-04-25 10:11:05.000000 hcpdiff-0.2.0/hcpdiff/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.098452 hcpdiff-0.2.0/hcpdiff.egg-info/
--rw-rw-rw-   0        0        0     5477 2023-04-25 10:12:53.000000 hcpdiff-0.2.0/hcpdiff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2263 2023-04-25 10:12:54.000000 hcpdiff-0.2.0/hcpdiff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 10:12:53.000000 hcpdiff-0.2.0/hcpdiff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-04-25 10:12:53.000000 hcpdiff-0.2.0/hcpdiff.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      225 2023-04-25 10:12:53.000000 hcpdiff-0.2.0/hcpdiff.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 10:12:53.000000 hcpdiff-0.2.0/hcpdiff.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.130606 hcpdiff-0.2.0/prompt_tuning_template/
--rw-rw-rw-   0        0        0       14 2023-04-03 03:15:56.000000 hcpdiff-0.2.0/prompt_tuning_template/caption.txt
--rw-rw-rw-   0        0        0       14 2023-02-21 02:34:54.000000 hcpdiff-0.2.0/prompt_tuning_template/name.txt
--rw-rw-rw-   0        0        0       55 2023-02-21 02:36:10.000000 hcpdiff-0.2.0/prompt_tuning_template/name_2pt_caption.txt
--rw-rw-rw-   0        0        0       25 2023-03-22 03:52:13.000000 hcpdiff-0.2.0/prompt_tuning_template/name_caption.txt
--rw-rw-rw-   0        0        0      915 2023-04-02 01:48:02.000000 hcpdiff-0.2.0/prompt_tuning_template/object.txt
--rw-rw-rw-   0        0        0     1212 2023-04-17 05:27:11.000000 hcpdiff-0.2.0/prompt_tuning_template/object_caption.txt
--rw-rw-rw-   0        0        0      890 2023-04-11 08:41:31.000000 hcpdiff-0.2.0/prompt_tuning_template/style.txt
--rw-rw-rw-   0        0        0     1099 2023-04-17 05:27:11.000000 hcpdiff-0.2.0/prompt_tuning_template/style_caption.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 10:12:54.135606 hcpdiff-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1833 2023-04-25 10:12:52.000000 hcpdiff-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 10:12:54.133605 hcpdiff-0.2.0/test/
--rw-rw-rw-   0        0        0     1062 2023-04-19 08:08:17.000000 hcpdiff-0.2.0/test/test_combine.py
--rw-rw-rw-   0        0        0      717 2023-04-25 06:44:29.000000 hcpdiff-0.2.0/test/test_ctnet.py
--rw-rw-rw-   0        0        0      918 2023-04-20 07:07:20.000000 hcpdiff-0.2.0/test/test_paradict.py
--rw-rw-rw-   0        0        0      592 2023-04-13 07:54:04.000000 hcpdiff-0.2.0/test/test_plugin_param.py
+drwxrwxrwx   0        0        0        0 2023-04-29 03:27:33.402979 hcpdiff-0.2.1/
+-rw-rw-rw-   0        0        0    11558 2023-04-11 12:44:40.000000 hcpdiff-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     5507 2023-04-29 03:27:33.401971 hcpdiff-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4770 2023-04-29 03:26:53.000000 hcpdiff-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 03:27:33.337631 hcpdiff-0.2.1/cfgs/
+drwxrwxrwx   0        0        0        0 2023-04-29 03:27:33.342983 hcpdiff-0.2.1/cfgs/infer/
+-rw-rw-rw-   0        0        0      179 2023-04-11 09:59:00.000000 hcpdiff-0.2.1/cfgs/infer/change_vae.yaml
+-rw-rw-rw-   0        0        0      672 2023-04-12 10:04:24.000000 hcpdiff-0.2.1/cfgs/infer/euler_a.yaml
+-rw-rw-rw-   0        0        0     1659 2023-04-25 10:11:05.000000 hcpdiff-0.2.1/cfgs/infer/img2img.yaml
+-rw-rw-rw-   0        0        0     1003 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/cfgs/infer/img2img_controlnet.yaml
+-rw-rw-rw-   0        0        0     1581 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/cfgs/infer/text2img.yaml
+drwxrwxrwx   0        0        0        0 2023-04-29 03:27:33.343971 hcpdiff-0.2.1/cfgs/plugins/
+-rw-rw-rw-   0        0        0      442 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/cfgs/plugins/plugin_controlnet.yaml
+-rw-rw-rw-   0        0        0     9971 2023-03-22 01:36:55.000000 hcpdiff-0.2.1/cfgs/te_struct.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 03:27:33.344971 hcpdiff-0.2.1/cfgs/train/
+drwxrwxrwx   0        0        0        0 2023-04-29 03:27:33.353970 hcpdiff-0.2.1/cfgs/train/examples/
+-rw-rw-rw-   0        0        0     1846 2023-04-11 12:30:15.000000 hcpdiff-0.2.1/cfgs/train/examples/CustomDiffusion.yaml
+-rw-rw-rw-   0        0        0     2815 2023-04-15 14:19:44.000000 hcpdiff-0.2.1/cfgs/train/examples/DreamArtist++.yaml
+-rw-rw-rw-   0        0        0     1334 2023-04-12 06:39:19.000000 hcpdiff-0.2.1/cfgs/train/examples/DreamArtist.yaml
+-rw-rw-rw-   0        0        0     1644 2023-04-11 12:30:15.000000 hcpdiff-0.2.1/cfgs/train/examples/DreamBooth.yaml
+-rw-rw-rw-   0        0        0     1124 2023-04-11 12:30:15.000000 hcpdiff-0.2.1/cfgs/train/examples/TextualInversion.yaml
+-rw-rw-rw-   0        0        0     1046 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/cfgs/train/examples/controlnet.yaml
+-rw-rw-rw-   0        0        0     1178 2023-04-11 12:30:15.000000 hcpdiff-0.2.1/cfgs/train/examples/fine-tuning.yaml
+-rw-rw-rw-   0        0        0     1397 2023-04-11 12:30:15.000000 hcpdiff-0.2.1/cfgs/train/examples/locon.yaml
+-rw-rw-rw-   0        0        0     1228 2023-04-11 12:30:15.000000 hcpdiff-0.2.1/cfgs/train/examples/lora_conventional.yaml
+-rw-rw-rw-   0        0        0     3158 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/cfgs/train/train_base.yaml
+-rw-rw-rw-   0        0        0     1025 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/cfgs/train/tuning_base.yaml
+-rw-rw-rw-   0        0        0    46121 2023-03-22 01:36:55.000000 hcpdiff-0.2.1/cfgs/unet_struct.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 03:27:33.357972 hcpdiff-0.2.1/hcpdiff/
+-rw-rw-rw-   0        0        0        0 2023-04-11 12:30:15.000000 hcpdiff-0.2.1/hcpdiff/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 03:27:33.366970 hcpdiff-0.2.1/hcpdiff/data/
+-rw-rw-rw-   0        0        0      195 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/data/__init__.py
+-rw-rw-rw-   0        0        0     8773 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/data/bucket.py
+-rw-rw-rw-   0        0        0     2390 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/data/cond_pair_dataset.py
+-rw-rw-rw-   0        0        0     5782 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/data/pair_dataset.py
+-rw-rw-rw-   0        0        0     2416 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-29 03:27:33.375979 hcpdiff-0.2.1/hcpdiff/models/
+-rw-rw-rw-   0        0        0      295 2023-04-15 14:19:44.000000 hcpdiff-0.2.1/hcpdiff/models/__init__.py
+-rw-rw-rw-   0        0        0     1422 2023-04-11 12:30:15.000000 hcpdiff-0.2.1/hcpdiff/models/cfg_context.py
+-rw-rw-rw-   0        0        0     7931 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/models/controlnet.py
+-rw-rw-rw-   0        0        0     3068 2023-04-11 12:47:28.000000 hcpdiff-0.2.1/hcpdiff/models/layers.py
+-rw-rw-rw-   0        0        0     6815 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/models/lora_base.py
+-rw-rw-rw-   0        0        0     7801 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/models/lora_layers.py
+-rw-rw-rw-   0        0        0     8973 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/models/plugin.py
+-rw-rw-rw-   0        0        0     3922 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/models/text_emb_ex.py
+-rw-rw-rw-   0        0        0     5807 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/models/textencoder_ex.py
+-rw-rw-rw-   0        0        0     2440 2023-04-14 04:04:05.000000 hcpdiff-0.2.1/hcpdiff/models/tokenizer_ex.py
+drwxrwxrwx   0        0        0        0 2023-04-29 03:27:33.380971 hcpdiff-0.2.1/hcpdiff/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-12 06:39:19.000000 hcpdiff-0.2.1/hcpdiff/tools/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-04-12 08:25:47.000000 hcpdiff-0.2.1/hcpdiff/tools/convert_caption_txt2json.py
+-rw-rw-rw-   0        0        0     1916 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/tools/create_embedding.py
+-rw-rw-rw-   0        0        0     1738 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/tools/gen_from_ptlist.py
+-rw-rw-rw-   0        0        0      658 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/tools/init_proj.py
+-rw-rw-rw-   0        0        0     8536 2023-04-25 10:11:05.000000 hcpdiff-0.2.1/hcpdiff/tools/sd2diffusers.py
+-rw-rw-rw-   0        0        0    26567 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/train_ac.py
+-rw-rw-rw-   0        0        0     4284 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/train_ac_single.py
+-rw-rw-rw-   0        0        0    10421 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/train_colo.py
+drwxrwxrwx   0        0        0        0 2023-04-29 03:27:33.387971 hcpdiff-0.2.1/hcpdiff/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-11 12:30:15.000000 hcpdiff-0.2.1/hcpdiff/utils/__init__.py
+-rw-rw-rw-   0        0        0     2865 2023-04-12 06:39:19.000000 hcpdiff-0.2.1/hcpdiff/utils/caption_tools.py
+-rw-rw-rw-   0        0        0    12403 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/utils/cfg_net_tools.py
+drwxrwxrwx   0        0        0        0 2023-04-29 03:27:33.389980 hcpdiff-0.2.1/hcpdiff/utils/ckpt_manager/
+-rw-rw-rw-   0        0        0       82 2023-04-11 12:30:15.000000 hcpdiff-0.2.1/hcpdiff/utils/ckpt_manager/__init__.py
+-rw-rw-rw-   0        0        0     4266 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/utils/ckpt_manager/ckpt_pkl.py
+-rw-rw-rw-   0        0        0     1884 2023-04-25 10:11:05.000000 hcpdiff-0.2.1/hcpdiff/utils/ckpt_manager/ckpt_safetensor.py
+-rw-rw-rw-   0        0        0      860 2023-04-11 12:30:15.000000 hcpdiff-0.2.1/hcpdiff/utils/colo_utils.py
+-rw-rw-rw-   0        0        0     3065 2023-04-11 12:30:15.000000 hcpdiff-0.2.1/hcpdiff/utils/ema.py
+-rw-rw-rw-   0        0        0     8680 2023-04-11 12:30:15.000000 hcpdiff-0.2.1/hcpdiff/utils/img_size_tool.py
+-rw-rw-rw-   0        0        0     5937 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/utils/net_utils.py
+-rw-rw-rw-   0        0        0     2741 2023-04-29 03:26:21.000000 hcpdiff-0.2.1/hcpdiff/utils/utils.py
+-rw-rw-rw-   0        0        0     7365 2023-04-27 13:09:44.000000 hcpdiff-0.2.1/hcpdiff/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-04-29 03:27:33.362971 hcpdiff-0.2.1/hcpdiff.egg-info/
+-rw-rw-rw-   0        0        0     5507 2023-04-29 03:27:33.000000 hcpdiff-0.2.1/hcpdiff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2277 2023-04-29 03:27:33.000000 hcpdiff-0.2.1/hcpdiff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 03:27:33.000000 hcpdiff-0.2.1/hcpdiff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-04-29 03:27:33.000000 hcpdiff-0.2.1/hcpdiff.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      225 2023-04-29 03:27:33.000000 hcpdiff-0.2.1/hcpdiff.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-29 03:27:33.000000 hcpdiff-0.2.1/hcpdiff.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 03:27:33.397979 hcpdiff-0.2.1/prompt_tuning_template/
+-rw-rw-rw-   0        0        0       14 2023-04-03 03:15:56.000000 hcpdiff-0.2.1/prompt_tuning_template/caption.txt
+-rw-rw-rw-   0        0        0       14 2023-02-21 02:34:54.000000 hcpdiff-0.2.1/prompt_tuning_template/name.txt
+-rw-rw-rw-   0        0        0       55 2023-02-21 02:36:10.000000 hcpdiff-0.2.1/prompt_tuning_template/name_2pt_caption.txt
+-rw-rw-rw-   0        0        0       25 2023-03-22 03:52:13.000000 hcpdiff-0.2.1/prompt_tuning_template/name_caption.txt
+-rw-rw-rw-   0        0        0      915 2023-04-02 01:48:02.000000 hcpdiff-0.2.1/prompt_tuning_template/object.txt
+-rw-rw-rw-   0        0        0     1212 2023-04-17 05:27:11.000000 hcpdiff-0.2.1/prompt_tuning_template/object_caption.txt
+-rw-rw-rw-   0        0        0      890 2023-04-11 08:41:31.000000 hcpdiff-0.2.1/prompt_tuning_template/style.txt
+-rw-rw-rw-   0        0        0     1099 2023-04-17 05:27:11.000000 hcpdiff-0.2.1/prompt_tuning_template/style_caption.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 03:27:33.402979 hcpdiff-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1833 2023-04-29 03:27:25.000000 hcpdiff-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 03:27:33.400981 hcpdiff-0.2.1/test/
+-rw-rw-rw-   0        0        0     1062 2023-04-19 08:08:17.000000 hcpdiff-0.2.1/test/test_combine.py
+-rw-rw-rw-   0        0        0      717 2023-04-25 06:44:29.000000 hcpdiff-0.2.1/test/test_ctnet.py
+-rw-rw-rw-   0        0        0      918 2023-04-20 07:07:20.000000 hcpdiff-0.2.1/test/test_paradict.py
+-rw-rw-rw-   0        0        0      592 2023-04-13 07:54:04.000000 hcpdiff-0.2.1/test/test_plugin_param.py
```

### Comparing `hcpdiff-0.2.0/LICENSE` & `hcpdiff-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/PKG-INFO` & `hcpdiff-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.2.0
+Version: 0.2.1
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -52,14 +52,15 @@
 * Custom words that occupy multiple words
 * Maximum sentence length expansion
 * colossal-AI
 * xformers for unet and text-encoder
 * CLIP skip
 * Tag shuffle and dropout
 * safetensors support
+* Controlnet (support train)
 
 ## Install
 
 Install with pip:
 ```bash
 pip install hcpdiff
 # Start a new project and make initialization
```

### Comparing `hcpdiff-0.2.0/README.md` & `hcpdiff-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 * Custom words that occupy multiple words
 * Maximum sentence length expansion
 * colossal-AI
 * xformers for unet and text-encoder
 * CLIP skip
 * Tag shuffle and dropout
 * safetensors support
+* Controlnet (support train)
 
 ## Install
 
 Install with pip:
 ```bash
 pip install hcpdiff
 # Start a new project and make initialization
```

### Comparing `hcpdiff-0.2.0/cfgs/infer/euler_a.yaml` & `hcpdiff-0.2.1/cfgs/infer/euler_a.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/cfgs/infer/img2img.yaml` & `hcpdiff-0.2.1/cfgs/infer/img2img.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/cfgs/infer/img2img_controlnet.yaml` & `hcpdiff-0.2.1/cfgs/infer/text2img.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -7,63 +7,55 @@
 emb_dir: 'embs/'
 N_repeats: 1
 bs: 4
 num: 1
 seed: null
 fp16: True
 
-condition:
-  type: controlnet
-  image: 'cond_img.png'
+condition: null
 
 save:
   save_cfg: True
   image_type: png
   quality: 95
 #  image_type: webp
 #  quality: 75
 
 infer_args:
-  num_inference_steps: 30
-  strength: 0.75
+  width: 512
+  height: 512
   guidance_scale: 7.5
+  num_inference_steps: 50
 
 new_components: {}
 
 merge: # can be null
   exp_dir: '2023-04-03-10-10-36'
   alpha: 0.8
-  plugin_cfg: cfgs/train/plugin_control.yaml
 
   group1:
     type: 'unet'
     base_model_alpha: 1.0 # base model weight to merge with lora or part
     lora:
       - path: 'exps/${....exp_dir}/ckpts/unet-600.safetensors'
         alpha: ${....alpha}
         layers: 'all'
         mask: [0.5, 1]
       - path: 'exps/${....exp_dir}/ckpts/unet-neg-600.safetensors'
         alpha: 0.65
         layers: 'all'
         mask: [0, 0.5]
     part: null
-    plugin:
-      controlnet1:
-        path: 'exps/controlnet.safetensors'
-        alpha: ${....alpha}
-        layers: 'all'
 
   group2:
     type: 'TE'
     base_model_alpha: 1.0 # base model weight to infer with lora or part
     lora:
       - path: 'exps/${....exp_dir}/ckpts/text_encoder-600.safetensors'
         alpha: ${....alpha}
         layers: 'all'
         mask: [0.5, 1]
       - path: 'exps/${....exp_dir}/ckpts/text_encoder-neg-600.safetensors'
         alpha: 0.65
         layers: 'all'
         mask: [0, 0.5]
-    part: null
-    plugin: null
+    part: null
```

### Comparing `hcpdiff-0.2.0/cfgs/te_struct.txt` & `hcpdiff-0.2.1/cfgs/te_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/cfgs/train/examples/CustomDiffusion.yaml` & `hcpdiff-0.2.1/cfgs/train/examples/CustomDiffusion.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/cfgs/train/examples/DreamArtist++.yaml` & `hcpdiff-0.2.1/cfgs/train/examples/DreamArtist++.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/cfgs/train/examples/DreamArtist.yaml` & `hcpdiff-0.2.1/cfgs/train/examples/DreamArtist.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/cfgs/train/examples/DreamBooth.yaml` & `hcpdiff-0.2.1/cfgs/train/examples/DreamBooth.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/cfgs/train/examples/TextualInversion.yaml` & `hcpdiff-0.2.1/cfgs/train/examples/TextualInversion.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/cfgs/train/examples/fine-tuning.yaml` & `hcpdiff-0.2.1/cfgs/train/examples/fine-tuning.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/cfgs/train/examples/locon.yaml` & `hcpdiff-0.2.1/cfgs/train/examples/locon.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/cfgs/train/examples/lora_conventional.yaml` & `hcpdiff-0.2.1/cfgs/train/examples/lora_conventional.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/cfgs/train/train_base.yaml` & `hcpdiff-0.2.1/cfgs/train/train_base.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -58,14 +58,16 @@
   ema_unet: 0 # 0 to disable
   ema_text_encoder: 0 # 0 to disable
   clip_skip: 0
 
   noise_scheduler: DDPMScheduler
 
 data:
+  _target_: hcpdiff.data.TextImagePairDataset
+  _partial_: True # Not directly instantiate the object here. There are other parameters to be added in the runtime.
   batch_size: 4
   prompt_template: 'prompt_tuning_template/name.txt'
   caption_file: null # path to image captions (file_words)
   cache_latents: True
   att_mask: null
   att_mask_encode: False
   bg_color: [255, 255, 255] # RGB; for ARGB -> RGB
@@ -86,17 +88,20 @@
   bucket:
     _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
     img_root: 'imgs/train' # images directory of train images
     target_area: {_target_: "builtins.eval", _args_: ['512*512']} # Expected area of training images: width * height
     num_bucket: 5
 
 data_class: # for DreamBooth
+  _target_: hcpdiff.data.TextImagePairDataset
+  _partial_: True
   batch_size: 1
   prompt_template: 'prompt_tuning_template/name.txt'
   caption_file: null
+  cache_latents: True
   att_mask: null
   att_mask_encode: False
   bg_color: [255, 255, 255] # RGB; for ARGB -> RGB
   image_transforms: ${..data.image_transforms}
   tag_transforms: ${..data.tag_transforms}
   bucket:
     _target_: hcpdiff.data.bucket.FixedBucket # aspect ratio bucket
```

### Comparing `hcpdiff-0.2.0/cfgs/unet_struct.txt` & `hcpdiff-0.2.1/cfgs/unet_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/hcpdiff/data/bucket.py` & `hcpdiff-0.2.1/hcpdiff/data/bucket.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,25 +27,30 @@
         :return: (file name of image), (target image size)
         '''
         raise NotImplementedError()
 
     def __len__(self):
         raise NotImplementedError()
 
+    def build(self, bs):
+        raise NotImplementedError()
+
     def rest(self, epoch):
         pass
 
     def crop_resize(self, image, size):
         return image
 
 class FixedBucket(BaseBucket):
     def __init__(self, img_root:str, target_size:Union[Tuple[int,int], int]=512):
         self.img_root=img_root
         self.target_size=(target_size, target_size) if isinstance(target_size, int) else target_size
-        self.file_names=[x for x in os.listdir(img_root) if get_file_ext(x) in types_support]
+
+    def build(self, bs):
+        self.file_names=[x for x in os.listdir(self.img_root) if get_file_ext(x) in types_support]
 
     def crop_resize(self, image, size):
         return resize_crop_fix(image, size)
 
     def __getitem__(self, idx) -> Tuple[str, Tuple[int, int]]:
         return os.path.join(self.img_root, self.file_names[idx]), self.target_size
 
@@ -157,15 +162,15 @@
         self.idx_bucket_map = np.empty(len(self.file_names), dtype=int)
         for bidx in range(self.num_bucket):
             bnow = labels == bidx
             self.buckets.append(np.where(bnow)[0].tolist())
             self.idx_bucket_map[bnow]=bidx
         logger.info('buckets info: '+', '.join(f'size:{self.size_buckets[i]}, num:{len(b)}' for i, b in enumerate(self.buckets)))
 
-    def make_arb(self, bs:int):
+    def build(self, bs:int):
         '''
         :param bs: batch_size * n_gpus * accumulation_step
         :param pre_build_arb:
         '''
         self.bs = bs
         if self.pre_build_arb and os.path.exists(self.pre_build_arb):
             return
```

### Comparing `hcpdiff-0.2.0/hcpdiff/data/pair_dataset.py` & `hcpdiff-0.2.1/hcpdiff/data/pair_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     :Name:        text-image pair dataset
     :Author:      Dong Ziyi
     :Affiliation: HCP Lab, SYSU
     :Created:     10/03/2023
     :Licence:     Apache-2.0
 """
 
+from typing import Tuple, Callable, Iterable
 import os.path
 
 import torch
 from PIL import Image
 import cv2
 from torch.utils.data import Dataset
 from .bucket import BaseBucket
@@ -19,51 +20,47 @@
 from hcpdiff.utils.utils import _default, get_file_name, get_file_ext
 from hcpdiff.utils.img_size_tool import types_support
 from tqdm.auto import tqdm
 
 import json
 import yaml
 
+
 class TextImagePairDataset(Dataset):
     """
     A dataset to prepare the instance and class images with the prompts for fine-tuning the model.
     It pre-processes the images and the tokenizes prompts.
     """
 
-    def __init__(
-        self,
-        cfg_data,
-        tokenizer,
-        tokenizer_repeats=1,
-        image_transforms=None,
-        tag_transforms=None,
-        return_path=False
-    ):
+    def __init__(self, prompt_template: str, tokenizer, tokenizer_repeats: int = 1, caption_file: str = None,
+                 att_mask: str = None, att_mask_encode: bool = False, bg_color: Iterable[int] = (255, 255, 255),
+                 image_transforms: Callable = None, tag_transforms: Callable = None, bucket: BaseBucket = None, return_path: bool = False):
         self.return_path = return_path
 
         self.tokenizer = tokenizer
         self.tokenizer_repeats = tokenizer_repeats
 
-        self.bucket: BaseBucket = cfg_data.bucket
-        self.caption_dict = self.load_captions(cfg_data.caption_file)
-        self.att_mask_path = {} if cfg_data.att_mask is None else \
-                {get_file_name(file):os.path.join(cfg_data.att_mask, file) for file in os.listdir(cfg_data.att_mask) if get_file_ext(file) in types_support}
-        self.att_mask_encode = cfg_data.att_mask_encode
-
-        self.prompt_template=self.load_template(cfg_data.prompt_template)
-
-        self.image_transforms = _default(image_transforms, cfg_data.image_transforms)
-        self.tag_transforms = _default(tag_transforms, cfg_data.tag_transforms)
-        self.bg_color = tuple(cfg_data.bg_color)
+        self.bucket: BaseBucket = bucket
+        self.caption_dict = self.load_captions(caption_file)
+        self.att_mask_path = {} if att_mask is None else \
+            {get_file_name(file): os.path.join(att_mask, file) for file in os.listdir(att_mask) if
+             get_file_ext(file) in types_support}
+        self.att_mask_encode = att_mask_encode
+
+        self.prompt_template = self.load_template(prompt_template)
+
+        self.image_transforms = _default(image_transforms, image_transforms)
+        self.tag_transforms = _default(tag_transforms, tag_transforms)
+        self.bg_color = tuple(bg_color)
 
-        self.latents = None # Cache latents for faster training. Works only without image argumentations.
+        self.latents = None  # Cache latents for faster training. Works only without image argumentations.
 
     def load_image(self, path):
         image = Image.open(path)
-        if image.mode=='RGBA':
+        if image.mode == 'RGBA':
             x, y = image.size
             canvas = Image.new('RGBA', image.size, self.bg_color)
             canvas.paste(image, (0, 0, x, y), image)
             image = canvas
         return image.convert("RGB")
 
     def load_captions(self, caption_file):
@@ -86,61 +83,60 @@
     def cache_latents(self, vae, weight_dtype, device, show_prog=True):
         self.latents = {}
         self.bucket.rest(0)
 
         for path, size in tqdm(self.bucket, disable=not show_prog):
             img_name = os.path.basename(path)
             if img_name not in self.latents:
-                image = self.load_image(path)
-                att_mask = self.get_att_map(get_file_name(img_name))
-                image, att_mask = self.process_data(image, att_mask, size)
-
-                image = image.unsqueeze(0).to(device, dtype=weight_dtype)
+                data = self.load_data(path, size)
+                image = data['img'].unsqueeze(0).to(device, dtype=weight_dtype)
                 latents = vae.encode(image).latent_dist.sample().squeeze(0)
-                self.latents[img_name] = [(latents * 0.18215).cpu(), att_mask]
+                data['img'] = (latents * 0.18215).cpu()
+                self.latents[img_name] = data
 
     def get_att_map(self, img_name):
         if img_name not in self.att_mask_path:
             return None
         att_mask = Image.open(self.att_mask_path[img_name]).convert("L")
         np_mask = np.array(att_mask).astype(float)
         np_mask[np_mask <= 127 + 0.1] = (np_mask[np_mask <= 127 + 0.1] / 127.)
         np_mask[np_mask > 127] = ((np_mask[np_mask > 127] - 127) / 128.) * 4 + 1
         return np_mask
 
-    def process_data(self, image, att_mask, size):
+    def load_data(self, path, size):
+        img_name = os.path.basename(path)
+        image = self.load_image(path)
+        att_mask = self.get_att_map(get_file_name(img_name))
         if att_mask is None:
             data = self.bucket.crop_resize({"img": image}, size)
             image = self.image_transforms(data['img'])  # resize to bucket size
             att_mask = torch.ones((size[1] // 8, size[0] // 8))
         else:
             data = self.bucket.crop_resize({"img": image, "mask": att_mask}, size)
             image = self.image_transforms(data['img'])
             att_mask = torch.tensor(cv2.resize(att_mask, (size[0] // 8, size[1] // 8), interpolation=cv2.INTER_LINEAR))
-        return image, att_mask
+        return {'img': image, 'mask': att_mask}
 
     def __len__(self):
         return len(self.bucket)
 
     def __getitem__(self, index):
         path, size = self.bucket[index]
         img_name = os.path.basename(path)
 
         if self.latents is None:
-            image = self.load_image(path)
-            att_mask = self.get_att_map(get_file_name(img_name))
-            image = self.process_data(image, att_mask, size)
+            data = self.load_data(path, size)
         else:
-            image = self.latents[img_name]
+            data = self.latents[img_name]
 
         caption_ist = self.caption_dict[img_name] if img_name in self.caption_dict else None
-        prompt_ist = self.tag_transforms({'prompt':random.choice(self.prompt_template), 'caption':caption_ist})['prompt']
+        prompt_ist = self.tag_transforms({'prompt': random.choice(self.prompt_template), 'caption': caption_ist})['prompt']
 
         # tokenize Sp or (Sn, Sp)
         prompt_ids = self.tokenizer(
             prompt_ist, truncation=True, padding="max_length", return_tensors="pt",
-            max_length=self.tokenizer.model_max_length*self.tokenizer_repeats).input_ids.squeeze()
+            max_length=self.tokenizer.model_max_length * self.tokenizer_repeats).input_ids.squeeze()
 
         if self.return_path:
-            return image, prompt_ids, path
+            return data, prompt_ids, path
         else:
-            return image, prompt_ids
+            return data, prompt_ids
```

### Comparing `hcpdiff-0.2.0/hcpdiff/models/cfg_context.py` & `hcpdiff-0.2.1/hcpdiff/models/cfg_context.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/hcpdiff/models/controlnet.py` & `hcpdiff-0.2.1/hcpdiff/models/controlnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from typing import List, Tuple, Union, Optional, Dict, Any
 
-from diffusers import UNet2DConditionModel, ControlNetModel
+from diffusers import UNet2DConditionModel
 import torch
 from torch import nn
 from copy import deepcopy
 
 from .plugin import MultiPluginBlock, BasePluginBlock
 from hcpdiff.utils.net_utils import remove_all_hooks, remove_layers
 
 class ControlNetPlugin(MultiPluginBlock):
-    def __init__(self, from_layers: List[nn.Module], to_layers: List[nn.Module], host_model: UNet2DConditionModel=None,
-                 pre_hook_to=False, cond_block_channels=(3, 16, 32, 96, 256, 320),
+    def __init__(self, name:str, from_layers: List[Dict[str, Any]], to_layers: List[Dict[str, Any]], host_model: UNet2DConditionModel=None,
+                 cond_block_channels=(3, 16, 32, 96, 256, 320),
                  layers_per_block=2, block_out_channels: Tuple[int] = (320, 640, 1280, 1280)):
-        super().__init__(from_layers, to_layers, pre_hook_to)
-        assert host_model is not None
+        super().__init__(name, from_layers, to_layers, host_model=host_model)
 
         self.register_input_feeder_to(host_model)
 
         self.conv_in = self.copy_block(host_model.conv_in)
         self.time_proj = self.copy_block(host_model.time_proj)
         self.time_embedding = self.copy_block(host_model.time_embedding)
         self.class_embedding = self.copy_block(host_model.class_embedding)
@@ -59,27 +58,32 @@
         def weight_init(m):
             if isinstance(m, nn.Conv2d):
                 nn.init.constant_(m.weight, 0)
         self.controlnet_down_blocks.apply(weight_init)
         self.controlnet_mid_block.apply(weight_init)
         self.cond_head[-1].apply(weight_init)
 
-    def from_layer_hook(self, host, fea_in:Tuple[torch.Tensor], idx: int):
-        assert idx==0
-        self.feat_to = self(*fea_in)
+    def from_layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:Tuple[torch.Tensor], idx: int):
+        if idx==0:
+            self.data_input = fea_in
+        elif idx==1:
+            self.feat_to = self(*self.data_input)
 
     def to_layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:Tuple[torch.Tensor], idx: int):
-        if idx == 0:
-            return fea_out + self.feat_to[0]
+        if idx == 5:
+            sp = fea_in[0].shape[1]//2
+            new_feat = fea_in[0].clone()
+            new_feat[:, sp:, ...] = fea_in[0][:, sp:, ...] + self.feat_to[0]
+            return (new_feat, fea_in[1])
+        elif idx == 3:
+            return (fea_out[0], tuple(fea_out[1][i] + self.feat_to[(idx) * 3 + i+1] for i in range(2)))
         elif idx == 4:
-            return (fea_out[0], tuple(fea_out[1][i] + self.feat_to[(idx-1) * 3 + i+1] for i in range(2)))
-        elif idx == 5:
             return fea_out + self.feat_to[11+1]
         else:
-            return (fea_out[0], tuple(fea_out[1][i]+self.feat_to[(idx-1)*3+i+1] for i in range(3)))
+            return (fea_out[0], tuple(fea_out[1][i]+self.feat_to[(idx)*3+i+1] for i in range(3)))
 
     def feed_input_data(self, data): # get the control image
         if isinstance(data, dict):
             self.cond = data['cond']
 
     def forward(
             self,
```

### Comparing `hcpdiff-0.2.0/hcpdiff/models/layers.py` & `hcpdiff-0.2.1/hcpdiff/models/layers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/hcpdiff/models/lora_base.py` & `hcpdiff-0.2.1/hcpdiff/models/lora_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,29 +7,25 @@
     :Created:     10/03/2023
     :Licence:     Apache-2.0
 """
 
 import torch
 from torch import nn
 
-from hcpdiff.utils.utils import make_mask, low_rank_approximate
+from hcpdiff.utils.utils import make_mask, low_rank_approximate, isinstance_list
 from .plugin import SinglePluginBlock, PluginGroup, BasePluginBlock
 
 from typing import Union, Tuple, Dict, Type
 
 class LoraBlock(SinglePluginBlock):
-    def __init__(self, host:Union[nn.Linear, nn.Conv2d], rank, dropout=0.1, scale=1.0, bias=False, inplace=True,
-                 hook_param=None, **kwargs):
-        super().__init__(host, hook_param)
-        if hasattr(host, 'lora_block'):
-            self.id = len(host.lora_block)
-            host.lora_block.append(self)
-        else:
-            self.id = 0
-            host.lora_block=nn.ModuleList([self])
+    wrapable_classes = [nn.Linear, nn.Conv2d]
+
+    def __init__(self, lora_id:int, host:Union[nn.Linear, nn.Conv2d], rank, dropout=0.1, scale=1.0, bias=False,
+                 inplace=True, hook_param=None, **kwargs):
+        super().__init__(f'lora_block_{lora_id}', host, hook_param)
 
         self.mask_range = None
         self.inplace=inplace
         self.bias=bias
 
         if isinstance(host, nn.Linear):
             self.host_type = 'linear'
@@ -56,33 +52,23 @@
             nn.init.zeros_(self.layer.lora_up.weight)
 
     def forward(self, fea_in:Tuple[torch.Tensor], fea_out:torch.Tensor):
         if self.mask_range is None:
             return fea_out + self.layer(fea_in[0]) * self.scale
         else:
             # for DreamArtist-lora
-            batch_mask = make_mask(self.mask_range[0], self.mask_range[1], fea_out.shape[0])
+            batch_mask = slice(int(self.mask_range[0]*fea_out.shape[0]), int(self.mask_range[1]*fea_out.shape[0]))
             if self.inplace:
                 fea_out[batch_mask, ...] = fea_out[batch_mask, ...] + self.layer(fea_in[0][batch_mask, ...]) * self.scale
                 return fea_out
             else: # colossal-AI dose not support inplace+view
                 new_out = fea_out.clone()
                 new_out[batch_mask, ...] = fea_out[batch_mask, ...] + self.layer(fea_in[0][batch_mask, ...]) * self.scale
                 return new_out
 
-    def remove(self):
-        super().remove()
-        host = self.host()
-        for i in range(len(host.lora_block)):
-            if host.lora_block[i] == self:
-                del host.lora_block[i]
-                break
-        if len(host.lora_block)==0:
-            del host.lora_block
-
     def collapse_to_host(self, alpha=None, base_alpha=1.0):
         if alpha is None:
             alpha = self.scale
 
         host = self.host()
         re_w, re_b = self.get_collapsed_param()
         host.weight = nn.Parameter(
@@ -129,49 +115,40 @@
         def forward(self, x):
             return self.dropout(self.lora_up(self.lora_down(x)))
 
         def get_collapsed_param(self) -> Tuple[torch.Tensor, torch.Tensor]:
             pass
 
     @classmethod
-    def warp_layer(cls, layer: Union[nn.Linear, nn.Conv2d], rank=1, dropout=0.1, scale=1.0, svd_init=False, bias=False, mask=None, **kwargs):# -> LoraBlock:
-        lora_block = cls(layer, rank, dropout, scale, bias=bias, **kwargs)
+    def wrap_layer(cls, lora_id:int, layer: Union[nn.Linear, nn.Conv2d], rank=1, dropout=0.0, scale=1.0, svd_init=False,
+                   bias=False, mask=None, **kwargs):# -> LoraBlock:
+        lora_block = cls(lora_id, layer, rank, dropout, scale, bias=bias, **kwargs)
         lora_block.init_weights(svd_init)
         lora_block.set_mask(mask)
         return lora_block
 
     @classmethod
-    def warp_model(cls, model: nn.Module, rank=1, dropout=0.0, scale=1.0, svd_init=False, bias=False, mask=None, **kwargs):# -> Dict[str, LoraBlock]:
-        lora_block_dict = {}
-        if isinstance(model, nn.Linear) or isinstance(model, nn.Conv2d):
-            lora_block_dict['lora_block'] = cls.warp_layer(model, rank, dropout, scale, svd_init, bias=bias, mask=mask, **kwargs)
-        else:
-            # there maybe multiple lora block, avoid insert lora into lora_block
-            named_modules = {name: layer for name, layer in model.named_modules() if 'lora_block' not in name}
-            for name, layer in named_modules.items():
-                if isinstance(layer, nn.Linear) or isinstance(layer, nn.Conv2d):
-                    lora_block_dict[f'{name}.lora_block'] = cls.warp_layer(layer, rank, dropout, scale, svd_init,
-                                                                bias=bias, mask=mask, **kwargs)
-        return lora_block_dict
+    def wrap_model(cls, lora_id:int, model: nn.Module, **kwargs):# -> Dict[str, LoraBlock]:
+        return super(LoraBlock, cls).wrap_model(lora_id, model, exclude_key='lora_block_', **kwargs)
 
     @staticmethod
     def extract_lora_state(model:nn.Module):
-        return {k:v for k,v in model.state_dict().items() if 'lora_block.' in k}
+        return {k:v for k,v in model.state_dict().items() if 'lora_block_' in k}
 
     @staticmethod
     def extract_state_without_lora(model:nn.Module):
-        return {k:v for k,v in model.state_dict().items() if 'lora_block.' not in k}
+        return {k:v for k,v in model.state_dict().items() if 'lora_block_' not in k}
 
     @staticmethod
     def extract_param_without_lora(model:nn.Module):
-        return {k:v for k,v in model.named_parameters() if 'lora_block.' not in k}
+        return {k:v for k,v in model.named_parameters() if 'lora_block_' not in k}
 
     @staticmethod
     def extract_trainable_state_without_lora(model:nn.Module):
-        trainable_keys = {k for k,v in model.named_parameters() if ('lora_block.' not in k) and v.requires_grad}
+        trainable_keys = {k for k,v in model.named_parameters() if ('lora_block_' not in k) and v.requires_grad}
         return {k: v for k, v in model.state_dict().items() if k in trainable_keys}
 
 class LoraGroup(PluginGroup):
     def set_mask(self, batch_mask):
         for item in self.plugin_dict.values():
             item.set_mask(batch_mask)
 
@@ -182,12 +159,12 @@
     def set_inplace(self, inplace):
         for item in self.plugin_dict.values():
             item.inplace = inplace
 
 def split_state(state_dict):
     sd_base, sd_lora={}, {}
     for k, v in state_dict.items():
-        if 'lora_block.' in k:
+        if 'lora_block_' in k:
             sd_lora[k]=v
         else:
             sd_base[k]=v
     return sd_base, sd_lora
```

### Comparing `hcpdiff-0.2.0/hcpdiff/models/lora_layers.py` & `hcpdiff-0.2.1/hcpdiff/models/lora_layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 from einops import repeat, rearrange, einsum
 from torch import nn
 
 from .lora_base import LoraBlock
 from .layers import GroupLinear
 
 class LoraLayer(LoraBlock):
-    def __init__(self, host, rank=1, dropout=0.1, scale=1.0, bias=False, inplace=True, **kwargs):
-        super().__init__(host, rank, dropout, scale, bias, inplace)
+    def __init__(self, lora_id:int, host, rank=1, dropout=0.1, scale=1.0, bias=False, inplace=True, **kwargs):
+        super().__init__(lora_id, host, rank, dropout, scale, bias, inplace)
 
     class LinearLayer(LoraBlock.LinearLayer):
         def __init__(self, host, rank, bias, dropout, block):
             super().__init__(host, rank, bias, dropout, block)
             self.lora_down = nn.Linear(host.in_features, self.rank, bias=False)
             self.lora_up = nn.Linear(self.rank, host.out_features, bias=bias)
 
@@ -42,17 +42,17 @@
 
         def get_collapsed_param(self):
             w = einsum(self.lora_up.weight.data, self.lora_down.weight.data, 'o r ..., r i ... -> o i ...')
             b = self.lora_up.bias.data if self.bias else None
             return w, b
 
 class LoraLayerGroup(LoraBlock):
-    def __init__(self, host, rank=1, dropout=0.1, scale=1.0, bias=False, inplace=True, rank_groups=1, **kwargs):
+    def __init__(self, lora_id:int, host, rank=1, dropout=0.1, scale=1.0, bias=False, inplace=True, rank_groups=1, **kwargs):
         self.rank_groups_raw = rank_groups
-        super().__init__(host, rank, dropout, scale, bias, inplace)
+        super().__init__(lora_id, host, rank, dropout, scale, bias, inplace)
 
     def collapse_to_host(self, alpha=None, base_alpha=1.0):
         raise NotImplementedError('LoraLayerGroup not support reparameterization.')
 
     class LinearLayer(LoraBlock.LinearLayer):
         def __init__(self, host, rank, bias, dropout, block):
             super().__init__(host, rank, bias, dropout, block)
@@ -86,17 +86,17 @@
 
         def forward(self, x):
             x = self.dropout(self.lora_up(self.lora_down(x)))
             x = torch.prod(rearrange(x, 'b (g c) h w -> b g c h w'), dim=1, dtype=torch.float16) ** (1 / self.rank_groups).to(dtype=x.dtype)
             return x
 
 class LohaLayer(LoraBlock):
-    def __init__(self, host, rank=1, dropout=0.1, scale=1.0, bias=False, inplace=True, rank_groups=2, **kwargs):
+    def __init__(self, lora_id:int, host, rank=1, dropout=0.1, scale=1.0, bias=False, inplace=True, rank_groups=2, **kwargs):
         self.rank_groups_raw = rank_groups
-        super().__init__(host, rank, dropout, scale, bias, inplace, hook_param='weight')
+        super().__init__(lora_id, host, rank, dropout, scale, bias, inplace, hook_param='weight')
 
     def forward(self, host_param: nn.Parameter):
         return host_param + self.layer(host_param) * self.scale
 
     class LinearLayer(LoraBlock.LinearLayer):
         def __init__(self, host, rank, bias, dropout, block):
             super().__init__(host, rank, bias, dropout, block)
```

### Comparing `hcpdiff-0.2.0/hcpdiff/models/text_emb_ex.py` & `hcpdiff-0.2.1/hcpdiff/models/text_emb_ex.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,21 +11,20 @@
 
 import torch
 from torch import nn
 import os
 from loguru import logger
 from einops import rearrange, repeat
 
-from hcpdiff.utils.emb_utils import load_emb
+from ..utils.net_utils import load_emb
 from .plugin import SinglePluginBlock
 
 class EmbeddingPTHook(SinglePluginBlock):
     def __init__(self, token_embedding:nn.Module, N_word=75, N_repeats=3):
-        super().__init__(token_embedding)
-        token_embedding.emb_ex = self
+        super().__init__('emb_ex', token_embedding)
         self.handle_pre = token_embedding.register_forward_pre_hook(self.pre_hook)
 
         self.N_word=N_word
         self.N_repeats=N_repeats
         self.num_embeddings=token_embedding.num_embeddings
         self.emb={}
         self.emb_train=nn.ParameterList()
```

### Comparing `hcpdiff-0.2.0/hcpdiff/models/textencoder_ex.py` & `hcpdiff-0.2.1/hcpdiff/models/textencoder_ex.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         feat_re = rearrange(feat_in[0], 'b (r w) -> (b r) w', r=self.N_repeats) # 使Attention mask的尺寸为N_word+2
         return (feat_re,) if len(feat_in)==1 else (feat_re, *feat_in[1:])
 
     def forward_hook(self, host, feat_in:Tuple[torch.Tensor], feat_out):
         if self.clip_skip>0:
             encoder_hidden_states = feat_out['hidden_states'][-self.clip_skip-1]
             encoder_hidden_states = self.text_enc.text_model.final_layer_norm(encoder_hidden_states)
-            encoder_hidden_states += 0*feat_out['last_hidden_state'] # avoid unused parameters, make gradient checkpointing happy
+            encoder_hidden_states = encoder_hidden_states + 0*feat_out['last_hidden_state'] # avoid unused parameters, make gradient checkpointing happy
         else:
             encoder_hidden_states = feat_out['last_hidden_state']  # Get the text embedding for conditioning
 
         encoder_hidden_states = rearrange(encoder_hidden_states, '(b r) ... -> b r ...', r=self.N_repeats)  # [B, N_repeat, N_word+2, N_emb]
         BOS, EOS = encoder_hidden_states[:, 0, :1, :], encoder_hidden_states[:, -1, -1:, :]
         encoder_hidden_states = torch.cat([BOS, encoder_hidden_states[:, :, 1:-1, :].flatten(1, 2), EOS], dim=1)  # [B, N_repeat*N_word+2, N_emb]
```

### Comparing `hcpdiff-0.2.0/hcpdiff/models/tokenizer_ex.py` & `hcpdiff-0.2.1/hcpdiff/models/tokenizer_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/hcpdiff/tools/convert_caption_txt2json.py` & `hcpdiff-0.2.1/hcpdiff/tools/convert_caption_txt2json.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/hcpdiff/tools/create_embedding.py` & `hcpdiff-0.2.1/hcpdiff/tools/create_embedding.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 import sys
+
 sys.path.append('/')
 
 import argparse
 import os.path
 
 import torch
-from hcpdiff.utils.utils import str2bool, import_model_class_from_model_name_or_path
+from hcpdiff.utils.utils import str2bool
+from hcpdiff.utils.net_utils import import_text_encoder_class, save_emb
 from transformers import AutoTokenizer
-from hcpdiff.utils.emb_utils import save_emb
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='')
     parser.add_argument('pretrained_model_name_or_path', type=str)
     parser.add_argument('name', type=str)
     parser.add_argument('n_word', type=int, default=3)
     parser.add_argument('--init_text', type=str, default='*0.017', help='randn: *sigma (*0.5)')
     parser.add_argument('--root', type=str, default='embs/')
     parser.add_argument('--replace', type=str2bool, default=False)
     args = parser.parse_args()
 
     tokenizer = AutoTokenizer.from_pretrained(
-                args.pretrained_model_name_or_path,
-                subfolder="tokenizer",
-                revision=None,
-                use_fast=False,
-            )
+        args.pretrained_model_name_or_path,
+        subfolder="tokenizer",
+        revision=None,
+        use_fast=False,
+    )
 
-    text_encoder_cls = import_model_class_from_model_name_or_path(args.pretrained_model_name_or_path, None)
+    text_encoder_cls = import_text_encoder_class(args.pretrained_model_name_or_path, None)
     text_encoder = text_encoder_cls.from_pretrained(args.pretrained_model_name_or_path, subfolder="text_encoder", revision=None)
 
     embed_dim = text_encoder.text_model.embeddings.token_embedding.embedding_dim
     if args.init_text.startswith('*'):
         init_embs = torch.randn((args.n_word, embed_dim))
-        if len(args.init_text)>1:
+        if len(args.init_text) > 1:
             init_embs *= float(args.init_text[1:])
     else:
         emb_pt = text_encoder.text_model.embeddings.token_embedding
         prompt_ids = tokenizer(
             args.init_text, truncation=True, padding="max_length", return_tensors="pt",
-            max_length=tokenizer.model_max_length).input_ids[0,1:args.n_word+1]
+            max_length=tokenizer.model_max_length).input_ids[0, 1:args.n_word + 1]
         init_embs = emb_pt(prompt_ids)
     print(init_embs.shape)
     save_emb(os.path.join(args.root, args.name + '.pt'), init_embs, args.replace)
-    print(f'embedding {args.name} is create.')
+    print(f'embedding {args.name} is create.')
```

### Comparing `hcpdiff-0.2.0/hcpdiff/tools/gen_from_ptlist.py` & `hcpdiff-0.2.1/hcpdiff/tools/gen_from_ptlist.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,31 +15,33 @@
 parser.add_argument('--negative_prompt', type=str, default='')
 parser.add_argument('--num', type=int, default=200)
 parser.add_argument('--bs', type=int, default=4)
 args = parser.parse_args()
 
 torch.backends.cudnn.benchmark = True
 
+
 def split_batch(data, bs):
-    return [data[i:i+bs] for i in range(0,len(data),bs)]
+    return [data[i:i + bs] for i in range(0, len(data), bs)]
+
 
 data = pq.read_table(args.prompt_file).to_batches(args.bs)
 pipeline = StableDiffusionPipeline.from_pretrained(args.model, torch_dtype=torch.float16)
 pipeline.requires_safety_checker = False
 pipeline.safety_checker = None
 pipeline.to("cuda")
 pipeline.unet.to(memory_format=torch.channels_last)
 pipeline.enable_xformers_memory_efficient_attention()
 
-count=0
-captions={}
+count = 0
+captions = {}
 with torch.inference_mode():
     for i in tqdm(range(args.num)):
         p_batch = data[i][0].to_pylist()
-        imgs = pipeline(p_batch, negative_prompt=[args.negative_prompt]*len(p_batch)).images
+        imgs = pipeline(p_batch, negative_prompt=[args.negative_prompt] * len(p_batch)).images
         for prompt, img in zip(p_batch, imgs):
-            img.resize((512,512), Image.BILINEAR).save(os.path.join(args.out_dir, f'{count}.png'), format='PNG')
+            img.resize((512, 512), Image.BILINEAR).save(os.path.join(args.out_dir, f'{count}.png'), format='PNG')
             captions[f'{count}.png'] = prompt
-            count+=1
+            count += 1
 
-with open(os.path.join(args.out_dir, f'image_captions.json'),"w") as f:
-    json.dump(captions, f)
+with open(os.path.join(args.out_dir, f'image_captions.json'), "w") as f:
+    json.dump(captions, f)
```

### Comparing `hcpdiff-0.2.0/hcpdiff/tools/init_proj.py` & `hcpdiff-0.2.1/hcpdiff/tools/init_proj.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import sys
 import shutil
 import os
 
+
 def main():
     try:
         if os.path.exists(r'./cfgs'):
             shutil.rmtree(r'./cfgs')
         if os.path.exists(r'./prompt_tuning_template'):
             shutil.rmtree(r'./prompt_tuning_template')
         shutil.copytree(os.path.join(sys.prefix, 'hcpdiff/cfgs'), r'./cfgs')
         shutil.copytree(os.path.join(sys.prefix, 'hcpdiff/prompt_tuning_template'), r'./prompt_tuning_template')
     except:
         shutil.copytree(os.path.join(sys.prefix, '../hcpdiff/cfgs'), r'./cfgs')
-        shutil.copytree(os.path.join(sys.prefix, '../hcpdiff/prompt_tuning_template'), r'./prompt_tuning_template')
+        shutil.copytree(os.path.join(sys.prefix, '../hcpdiff/prompt_tuning_template'), r'./prompt_tuning_template')
```

### Comparing `hcpdiff-0.2.0/hcpdiff/tools/sd2diffusers.py` & `hcpdiff-0.2.1/hcpdiff/tools/sd2diffusers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/hcpdiff/train_ac.py` & `hcpdiff-0.2.1/hcpdiff/train_ac.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,34 +12,36 @@
 import argparse
 import itertools
 import os
 import sys
 
 import torch
 import torch.utils.checkpoint
+import torch.utils.data
 import transformers
 from accelerate import Accelerator, DistributedDataParallelKwargs
 from accelerate.utils import set_seed
 from transformers import AutoTokenizer
 from omegaconf import OmegaConf
 import hydra
 from loguru import logger
 import time
+from functools import partial
 
 import diffusers
 from diffusers import AutoencoderKL, UNet2DConditionModel
 from diffusers.utils.import_utils import is_xformers_available
 
-from hcpdiff.data import TextImagePairDataset, RatioBucket
-from hcpdiff.utils.utils import cycle_data, load_config_with_cli, get_cfg_range
-from hcpdiff.utils.net_utils import get_scheduler, import_text_encoder_class, TEUnetWrapper
+from hcpdiff.data import RatioBucket
+from hcpdiff.utils.utils import load_config_with_cli, get_cfg_range
+from hcpdiff.data.utils import cycle_data
+from hcpdiff.utils.net_utils import get_scheduler, import_text_encoder_class, TEUnetWrapper, load_emb
 from hcpdiff.models import EmbeddingPTHook, TEEXHook, CFGContext, DreamArtistPTContext
 from hcpdiff.utils.ema import ModelEMA
-from hcpdiff.utils.cfg_net_tools import make_hcpdiff
-from hcpdiff.utils.emb_utils import load_emb
+from hcpdiff.utils.cfg_net_tools import make_hcpdiff, make_plugin
 from hcpdiff.data import collate_fn_ft
 from hcpdiff.visualizer import Visualizer
 from hcpdiff.utils.ckpt_manager import CkptManagerPKL, CkptManagerSafe
 
 class Trainer:
     def __init__(self, cfgs_raw):
         cfgs = hydra.utils.instantiate(cfgs_raw)
@@ -63,26 +65,27 @@
             transformers.utils.logging.set_verbosity_warning()
             diffusers.utils.logging.set_verbosity_warning()
         else:
             transformers.utils.logging.set_verbosity_error()
             diffusers.utils.logging.set_verbosity_error()
 
         self.lr=1e-5 # no usage, place set lr in cfgs
-        self.train_TE = (cfgs.text_encoder is not None) or (cfgs.lora_text_encoder is not None)
+        self.train_TE = (cfgs.text_encoder is not None) or (cfgs.lora_text_encoder is not None) or (cfgs.plugin_TE is not None)
 
         self.build_ckpt_manager()
         self.build_model()
         self.make_hooks()
         self.config_model()
         self.cache_latents=False
-        self.train_loader, self.arb_ist=self.build_data(cfgs.data)
+        self.batch_size_list = []
+        self.train_loader=self.build_data(cfgs.data)
         if cfgs.data_class is None:
             self.train_loader_class=None # without DreamBooth
         else:
-            self.train_loader_class, self.arb_class=self.build_data(cfgs.data_class)
+            self.train_loader_class=self.build_data(cfgs.data_class)
         if self.cache_latents:
             self.vae = self.vae.to('cpu')
         self.build_optimizer_scheduler()
         self.criterion = cfgs.train.loss.criterion
 
         self.cfg_scale = get_cfg_range(cfgs.train.cfg_scale)
         if self.cfg_scale[1]==1.0:
@@ -138,17 +141,15 @@
             prepare_name_list.extend(['optimizer_pt', 'lr_scheduler_pt'])
 
         prepared_obj = self.accelerator.prepare(*prepare_obj_list)
         for name, obj in zip(prepare_name_list, prepared_obj):
             setattr(self, name, obj)
 
     def scale_lr(self, parameters):
-        bs = self.cfgs.data.batch_size
-        if self.cfgs.data_class is not None:
-            bs += self.cfgs.data_class.batch_size
+        bs = sum(self.batch_size_list)
         scale_factor = bs * self.world_size * self.cfgs.train.gradient_accumulation_steps
         for param in parameters:
             if 'lr' in param:
                 param['lr'] *= scale_factor
 
     def build_model(self):
         # Load the tokenizer
@@ -194,18 +195,20 @@
         elif self.cfgs.ckpt_type=='safetensors':
             self.ckpt_manager = CkptManagerSafe()
         else:
             raise NotImplementedError(f'Not support ckpt type: {self.cfgs.ckpt_type}')
         if self.is_local_main_process:
             self.ckpt_manager.set_save_dir(os.path.join(self.exp_dir, 'ckpts'), emb_dir=self.cfgs.tokenizer_pt.emb_dir)
 
-    def get_unet_raw(self):
+    @property
+    def unet_raw(self):
         return self.TE_unet.module.unet if self.train_TE else self.unet.module
 
-    def get_text_encoder_raw(self):
+    @property
+    def text_encoder_raw(self):
         return self.TE_unet.module.TE if self.train_TE else self.text_encoder
 
     def config_model(self):
         if self.cfgs.model.enable_xformers:
             if is_xformers_available():
                 self.unet.enable_xformers_memory_efficient_attention()
                 #self.text_enc_hook.enable_xformers()
@@ -251,47 +254,53 @@
         self.embedding_hook, self.ex_words_emb = EmbeddingPTHook.hook_from_dir(
                         self.cfgs.tokenizer_pt.emb_dir, self.tokenizer, self.text_encoder, log=self.is_local_main_process,
                         N_repeats=self.cfgs.model.tokenizer_repeats, device=self.device)
 
         self.text_enc_hook = TEEXHook(self.text_encoder, self.tokenizer, N_repeats=self.cfgs.model.tokenizer_repeats, device=self.device,
                                       clip_skip=self.cfgs.model.clip_skip)
 
-    def build_data(self, cfg_data):
-        train_dataset = TextImagePairDataset(cfg_data, self.tokenizer, tokenizer_repeats=self.cfgs.model.tokenizer_repeats)
-        if isinstance(train_dataset.bucket, RatioBucket):
-            arb=True
-            train_dataset.bucket.make_arb(cfg_data.batch_size*self.world_size)
-        else:
-            arb=False
+
+    def build_data(self, data_builder:partial) -> torch.utils.data.DataLoader:
+        batch_size = data_builder.keywords.pop('batch_size')
+        cache_latents = data_builder.keywords.pop('cache_latents')
+        self.batch_size_list.append(batch_size)
+
+        train_dataset = data_builder(tokenizer=self.tokenizer, tokenizer_repeats=self.cfgs.model.tokenizer_repeats)
+        train_dataset.bucket.build(batch_size * self.world_size)
+        arb = isinstance(train_dataset.bucket, RatioBucket)
         logger.info(f"len(train_dataset): {len(train_dataset)}")
 
-        if cfg_data.cache_latents:
+        if cache_latents:
             self.cache_latents = True
             train_dataset.cache_latents(self.vae, self.weight_dtype, self.device, show_prog=self.is_local_main_process)
 
         # Pytorch Data loader
         train_sampler = torch.utils.data.distributed.DistributedSampler(train_dataset, num_replicas=self.world_size,
                                                                         rank=self.local_rank, shuffle=not arb)
-        train_loader = torch.utils.data.DataLoader(train_dataset, batch_size=cfg_data.batch_size,
+        train_loader = torch.utils.data.DataLoader(train_dataset, batch_size=batch_size,
             num_workers=self.cfgs.train.workers, sampler=train_sampler, collate_fn=collate_fn_ft)
-        return train_loader, arb
+        return train_loader
 
     def get_param_group_train(self):
         # make miniFT and warp with lora
         self.DA_lora = False
         train_params_unet, self.lora_unet = make_hcpdiff(self.unet, self.cfgs.unet, self.cfgs.lora_unet)
         if isinstance(self.lora_unet, tuple): # creat negative lora
             self.DA_lora = True
             self.lora_unet, self.lora_unet_neg = self.lora_unet
+        train_params_unet_plugin, self.all_plugin_unet = make_plugin(self.unet, self.cfgs.plugin_unet)
+        train_params_unet += train_params_unet_plugin
 
         if self.train_TE:
             train_params_text_encoder, self.lora_TE = make_hcpdiff(self.text_encoder, self.cfgs.text_encoder, self.cfgs.lora_text_encoder)
             if isinstance(self.lora_TE, tuple):  # creat negative lora
                 self.DA_lora = True
                 self.lora_TE, self.lora_TE_neg = self.lora_TE
+            train_params_TE_plugin, self.all_plugin_TE = make_plugin(self.text_encoder, self.cfgs.plugin_TE)
+            train_params_text_encoder += train_params_TE_plugin
         else:
             train_params_text_encoder=[]
 
         # params for embedding
         train_params_emb = []
         self.train_pts = {}
         if self.cfgs.tokenizer_pt.train is not None:
@@ -329,32 +338,32 @@
             if self.cfgs.train.scale_lr_pt:
                 self.scale_lr(parameters_pt)
 
             self.optimizer_pt = torch.optim.AdamW(params=parameters_pt, lr=self.lr, weight_decay=cfg_opt.weight_decay_pt)
             self.lr_scheduler_pt = get_scheduler(optimizer=self.optimizer_pt, **self.cfgs.train.scheduler_pt)
 
     def train(self):
-        total_batch_size = self.cfgs.data.batch_size * self.world_size * self.cfgs.train.gradient_accumulation_steps
+        total_batch_size = sum(self.batch_size_list) * self.world_size * self.cfgs.train.gradient_accumulation_steps
 
         logger.info("***** Running training *****")
         logger.info(f"  Num batches each epoch = {len(self.train_loader)}")
         logger.info(f"  Num Steps = {self.cfgs.train.scheduler.num_training_steps}")
-        logger.info(f"  Instantaneous batch size per device = {self.cfgs.data.batch_size}")
+        logger.info(f"  Instantaneous batch size per device = {sum(self.batch_size_list)}")
         logger.info(f"  Total train batch size (w. parallel, distributed & accumulation) = {total_batch_size}")
         logger.info(f"  Gradient Accumulation steps = {self.cfgs.train.gradient_accumulation_steps}")
         self.global_step = 0
         if self.cfgs.train.resume is not None:
             self.global_step = self.cfgs.train.resume.start_step
 
         if self.train_loader_class is not None:
-            self.data_iter_class = iter(cycle_data(self.train_loader_class, arb=self.arb_class))
+            self.data_iter_class = iter(cycle_data(self.train_loader_class))
 
         loss_sum=0
-        for image, att_mask, prompt_ids in cycle_data(self.train_loader, arb=self.arb_ist):
-            loss=self.train_one_step(image, att_mask, prompt_ids)
+        for data, prompt_ids in cycle_data(self.train_loader):
+            loss=self.train_one_step(data, prompt_ids)
             loss_sum+=loss
 
             self.global_step += 1
             if self.is_local_main_process:
                 if self.global_step % self.cfgs.train.save_step == 0:
                     self.save_model()
                 if self.global_step % self.cfgs.train.log_step == 0:
@@ -392,60 +401,71 @@
         timesteps = torch.randint(0, self.noise_scheduler.config.num_train_timesteps, (bsz,), device=latents.device)
         timesteps = timesteps.long()
 
         # Add noise to the latents according to the noise magnitude at each timestep
         # (this is the forward diffusion process)
         return self.noise_scheduler.add_noise(latents, noise, timesteps), noise, timesteps
 
-    def encode_decode(self, prompt_ids, noisy_latents, timesteps):
+    def encode_decode(self, prompt_ids, noisy_latents, timesteps, **kwargs):
         # for DDP support
         if self.train_TE:
-            model_pred = self.TE_unet(prompt_ids, noisy_latents, timesteps)
+            model_pred = self.TE_unet(prompt_ids, noisy_latents, timesteps, **kwargs)
         else:
+            input_all = dict(prompt_ids=prompt_ids, noisy_latents=noisy_latents, timesteps=timesteps, **kwargs)
+            if hasattr(self.text_encoder, 'input_feeder'):
+                for feeder in self.text_encoder.input_feeder:
+                    feeder(input_all)
+            if hasattr(self.unet_raw, 'input_feeder'):
+                for feeder in self.unet_raw.input_feeder:
+                    feeder(input_all)
+
             encoder_hidden_states = self.text_encoder(prompt_ids, output_hidden_states=True)  # Get the text embedding for conditioning
             model_pred = self.unet(noisy_latents, timesteps, encoder_hidden_states).sample  # Predict the noise residual
         return model_pred
 
-    def forward(self, latents, prompt_ids):
+    def forward(self, latents, prompt_ids, **kwargs):
         noisy_latents, noise, timesteps = self.make_noise(latents)
 
         # CFG context for DreamArtist
         noisy_latents, timesteps = self.cfg_context.pre(noisy_latents, timesteps)
-        model_pred = self.encode_decode(prompt_ids, noisy_latents, timesteps)
+        model_pred = self.encode_decode(prompt_ids, noisy_latents, timesteps, **kwargs)
         model_pred = self.cfg_context.post(model_pred)
 
         # Get the target for loss depending on the prediction type
         if self.cfgs.train.loss.type == "eps":
             target = noise
         elif self.cfgs.train.loss.type == "sample":
             target = self.noise_scheduler.step(noise, timesteps, noisy_latents)
             model_pred = self.noise_scheduler.step(model_pred, timesteps, noisy_latents)
         else:
             raise ValueError(f"Unknown loss type {self.cfgs.train.loss.type}")
         return model_pred, target
 
-    def train_one_step(self, image, att_mask, prompt_ids):
-        image=image.to(self.device, dtype=self.weight_dtype)
-        att_mask = att_mask.to(self.device)
+    def train_one_step(self, data, prompt_ids):
+        image = data['img'].to(self.device, dtype=self.weight_dtype)
+        att_mask = data['mask'].to(self.device)
         prompt_ids=prompt_ids.to(self.device)
+        other_datas = {k:v.to(self.device, dtype=self.weight_dtype) for k,v in data.items() if k!='img' and k!='mask'}
+
         with self.accelerator.accumulate(self.unet):
             latents = self.get_latents(image, self.train_loader.dataset)
-            model_pred, target = self.forward(latents, prompt_ids)
+            model_pred, target = self.forward(latents, prompt_ids, **other_datas)
 
             if self.train_loader_class is not None:
                 loss = self.get_loss(model_pred, target, att_mask) # Compute instance loss
                 self.accelerator.backward(loss)
 
                 #DreamBooth prior forward
-                image_cls, att_mask_cls, prompt_ids_cls = next(self.data_iter_class)
-                image_cls = image_cls.to(self.device, dtype=self.weight_dtype)
-                att_mask_cls = att_mask_cls.to(self.device)
+                data_cls, prompt_ids_cls = next(self.data_iter_class)
+                image_cls = data_cls['img'].to(self.device, dtype=self.weight_dtype)
+                att_mask_cls = data_cls['mask'].to(self.device)
                 prompt_ids_cls = prompt_ids_cls.to(self.device)
+                other_datas_cls = {k: v.to(self.device, dtype=self.weight_dtype) for k, v in data_cls.items() if k != 'img' and k != 'mask'}
                 latents_cls = self.get_latents(image_cls, self.train_loader_class.dataset)
-                model_pred_prior, target_prior = self.forward(latents_cls, prompt_ids_cls)
+                model_pred_prior, target_prior = self.forward(latents_cls, prompt_ids_cls, **other_datas_cls)
 
                 prior_loss = self.get_loss(model_pred_prior, target_prior, att_mask_cls) # Compute prior loss
                 loss = self.cfgs.train.loss.prior_loss_weight * prior_loss
                 self.accelerator.backward(loss)
             else:
                 loss = self.get_loss(model_pred, target, att_mask)
                 self.accelerator.backward(loss)
@@ -474,42 +494,46 @@
             return (self.criterion(model_pred.float(), target.float()) * att_mask).mean() \
                + 0*sum(self.embedding_hook.emb_train).mean() # avoid unused parameters, make gradient checkpointing happy
         else:
             return (self.criterion(model_pred.float(), target.float()) * att_mask).mean()
 
     def update_ema(self):
         if hasattr(self, 'ema_unet'):
-            self.ema_unet.step(self.get_unet_raw().named_parameters())
+            self.ema_unet.step(self.unet_raw.named_parameters())
         if hasattr(self, 'ema_text_encoder'):
-            self.ema_text_encoder.step(self.get_text_encoder_raw().named_parameters())
+            self.ema_text_encoder.step(self.text_encoder_raw.named_parameters())
 
     def save_model(self, from_raw=False):
-        unet_raw=self.get_unet_raw()
+        unet_raw=self.unet_raw
         self.ckpt_manager.save_model_with_lora(unet_raw, self.lora_unet, model_ema=getattr(self, 'ema_unet', None),
                                                name='unet', step=self.global_step)
+        self.ckpt_manager.save_plugins(unet_raw, self.all_plugin_unet, name='unet', step=self.global_step,
+                                       model_ema=getattr(self, 'ema_unet', None))
         if self.train_TE:
-            TE_raw = self.get_text_encoder_raw()
+            TE_raw = self.text_encoder_raw
             # exclude_key: embeddings should not save with text-encoder
             self.ckpt_manager.save_model_with_lora(TE_raw, self.lora_TE, model_ema=getattr(self, 'ema_text_encoder', None),
                                                    name='text_encoder', step=self.global_step, exclude_key='emb_ex.')
+            self.ckpt_manager.save_plugins(TE_raw, self.all_plugin_TE, name='text_encoder', step=self.global_step,
+                                           model_ema=getattr(self, 'ema_text_encoder', None))
 
         if self.DA_lora:
             self.ckpt_manager.save_model_with_lora(None, self.lora_unet_neg, name='unet-neg', step=self.global_step)
             if self.train_TE:
                 self.ckpt_manager.save_model_with_lora(None, self.lora_TE_neg, name='text_encoder-neg', step=self.global_step)
 
         self.ckpt_manager.save_embedding(self.train_pts, self.global_step, self.cfgs.tokenizer_pt.replace)
 
         logger.info(f"Saved state, step: {self.global_step}")
 
     def make_vis(self):
         vis_dir = os.path.join(self.exp_dir ,f'vis-{self.global_step}')
         new_components={
-            'unet': self.get_unet_raw(),
-            'text_encoder': self.get_text_encoder_raw(),
+            'unet': self.unet_raw,
+            'text_encoder': self.text_encoder_raw,
             'tokenizer': self.tokenizer,
             'vae': self.vae,
         }
         viser = Visualizer(self.cfgs.model.pretrained_model_name_or_path, new_components=new_components)
         if self.cfgs.vis_info.prompt:
             raise ValueError('vis_info.prompt is None. cannot generate without prompt.')
         viser.vis_to_dir(vis_dir, self.cfgs.vis_prompt)
```

### Comparing `hcpdiff-0.2.0/hcpdiff/train_ac_single.py` & `hcpdiff-0.2.1/hcpdiff/train_ac_single.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import sys
 import torch
 from loguru import logger
+from functools import partial
 
 from accelerate import Accelerator
-from hcpdiff.train_ac import Trainer, TextImagePairDataset, RatioBucket, load_config_with_cli, set_seed
+from hcpdiff.train_ac import Trainer, RatioBucket, load_config_with_cli, set_seed
 from hcpdiff.data import collate_fn_ft
 
 class TrainerSingleCard(Trainer):
     def init_context(self, cfgs_raw):
         self.accelerator = Accelerator(
             gradient_accumulation_steps=self.cfgs.train.gradient_accumulation_steps,
             mixed_precision=self.cfgs.mixed_precision,
@@ -34,51 +35,61 @@
             prepare_obj_list.append(self.text_encoder)
             prepare_name_list.append('text_encoder')
 
         prepared_obj = self.accelerator.prepare(*prepare_obj_list)
         for name, obj in zip(prepare_name_list, prepared_obj):
             setattr(self, name, obj)
 
-    def build_data(self, cfg_data):
-        train_dataset = TextImagePairDataset(cfg_data, self.tokenizer, tokenizer_repeats=self.cfgs.model.tokenizer_repeats)
-        if isinstance(train_dataset.bucket, RatioBucket):
-            arb=True
-            train_dataset.bucket.make_arb(cfg_data.batch_size*self.world_size)
-        else:
-            arb=False
-
+    def build_data(self, data_builder:partial) -> torch.utils.data.DataLoader:
+        batch_size = data_builder.keywords.pop('batch_size')
+        cache_latents = data_builder.keywords.pop('cache_latents')
+        self.batch_size_list.append(batch_size)
+
+        train_dataset = data_builder(tokenizer=self.tokenizer, tokenizer_repeats=self.cfgs.model.tokenizer_repeats)
+        train_dataset.bucket.build(batch_size * self.world_size)
+        arb = isinstance(train_dataset.bucket, RatioBucket)
         logger.info(f"len(train_dataset): {len(train_dataset)}")
 
-        if cfg_data.cache_latents:
+        if cache_latents:
             self.cache_latents = True
-            train_dataset.cache_latents(self.vae, self.weight_dtype, self.device)
+            train_dataset.cache_latents(self.vae, self.weight_dtype, self.device, show_prog=self.is_local_main_process)
 
         # Pytorch Data loader
-        train_loader = torch.utils.data.DataLoader(train_dataset, batch_size=cfg_data.batch_size,
+        train_loader = torch.utils.data.DataLoader(train_dataset, batch_size=batch_size,
             num_workers=self.cfgs.train.workers, shuffle=not arb, collate_fn=collate_fn_ft)
-        return train_loader, arb
+        return train_loader
+
+    def encode_decode(self, prompt_ids, noisy_latents, timesteps, **kwargs):
+        input_all = dict(prompt_ids=prompt_ids, noisy_latents=noisy_latents, timesteps=timesteps, **kwargs)
+        if hasattr(self.text_encoder, 'input_feeder'):
+            for feeder in self.text_encoder.input_feeder:
+                feeder(input_all)
+        if hasattr(self.unet_raw, 'input_feeder'):
+            for feeder in self.unet_raw.input_feeder:
+                feeder(input_all)
 
-    def encode_decode(self, prompt_ids, noisy_latents, timesteps):
         encoder_hidden_states = self.text_encoder(prompt_ids, output_hidden_states=True)  # Get the text embedding for conditioning
         model_pred = self.unet(noisy_latents, timesteps, encoder_hidden_states).sample  # Predict the noise residual
         return model_pred
 
     def get_loss(self, model_pred, target, att_mask):
         return (self.criterion(model_pred.float(), target.float()) * att_mask).mean()
 
     def update_ema(self):
         if hasattr(self, 'ema_unet'):
             self.ema_unet.step(self.unet.named_parameters())
         if hasattr(self, 'ema_text_encoder'):
             self.ema_text_encoder.step(self.text_encoder.named_parameters())
 
-    def get_unet_raw(self):
+    @property
+    def unet_raw(self):
         return self.unet
 
-    def get_text_encoder_raw(self):
+    @property
+    def text_encoder_raw(self):
         return self.text_encoder
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Stable Diffusion Training')
     parser.add_argument('--cfg', type=str, default='cfg/train/demo.yaml')
     args, _ = parser.parse_known_args()
```

### Comparing `hcpdiff-0.2.0/hcpdiff/train_colo.py` & `hcpdiff-0.2.1/hcpdiff/train_colo.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 import colossalai
 import colossalai.tensor
 from colossalai.context.parallel_mode import ParallelMode
 from colossalai.core import global_context as gpc
 from colossalai.nn.parallel.utils import get_static_torch_model
 from colossalai.utils import get_current_device
 from colossalai.utils.model.colo_init_context import ColoInitContext
+from colossalai.utils.model.colo_init_context import _convert_to_coloparam
+from colossalai.tensor import ColoParameter
 
 from hcpdiff.train_ac import Trainer, get_scheduler, ModelEMA
 from diffusers import UNet2DConditionModel
 from hcpdiff.utils.colo_utils import gemini_zero_dpp, GeminiAdamOptimizerP
 from hcpdiff.utils.utils import load_config_with_cli
 from hcpdiff.utils.net_utils import import_text_encoder_class, TEUnetWrapper
 
@@ -74,17 +76,48 @@
 
     def build_ema(self):
         if self.cfgs.model.ema_unet>0:
             self.ema_unet = ModelEMA(get_static_torch_model(self.unet).named_parameters(), self.cfgs.model.ema_unet)
         if self.train_TE and self.cfgs.model.ema_text_encoder>0:
             self.ema_text_encoder = ModelEMA(self.text_encoder.named_parameters(), self.cfgs.model.ema_text_encoder)
 
+    def convert_emb_param(self, cinit):
+        name_list = []
+        for name, param in self.embedding_hook.named_parameters():
+            if type(param) is ColoParameter:
+                continue
+
+            split = name.rfind('.')
+            if split >= 0:  # param in submodule
+                module_name = name[:split]
+                param_name = name[split + 1:]
+            else:
+                module_name = ''  # param in current module
+                param_name = name
+            name_list.append((module_name, param_name))
+
+        replaced_tensors = dict(
+        )  # record mapping between (torch.Tensor, ColoTensor) to distinguish the same reference
+        for module_name, param_name in name_list:
+            submodule = self.embedding_hook.get_submodule(module_name)
+            param = submodule.get_parameter(param_name)
+            if param in replaced_tensors:
+                colo_param = replaced_tensors[param]
+            else:
+                colo_param = _convert_to_coloparam(param, cinit._device, cinit._dtype, cinit._default_pg,
+                                                   cinit._default_dist_spec)
+                replaced_tensors[param] = colo_param
+            delattr(submodule, param_name)
+            setattr(submodule, param_name, colo_param)
+            colo_param.shared_param_modules.append(submodule)
+
     def get_param_group_train(self):
-        with ColoInitContext(device=self.device):
+        with ColoInitContext(device=self.device) as cinit:
             params = super().get_param_group_train()
+            self.convert_emb_param(cinit)
 
         self.lora_unet.set_inplace(False)
         if self.DA_lora:
             self.lora_unet_neg.set_inplace(False)
         if self.train_TE:
             self.lora_TE.set_inplace(False)
             if self.DA_lora:
@@ -110,31 +143,33 @@
         if len(parameters_pt)>0: # do prompt-tuning
             if self.cfgs.train.scale_lr_pt:
                 self.scale_lr(parameters_pt)
 
             self.optimizer_pt = torch.optim.AdamW(params=parameters_pt, lr=self.lr, weight_decay=cfg_opt.weight_decay_pt)
             self.lr_scheduler_pt = get_scheduler(optimizer=self.optimizer_pt, **self.cfgs.train.scheduler_pt)
 
-    def train_one_step(self, image, att_mask, prompt_ids):
+    def train_one_step(self, data, prompt_ids):
         torch.cuda.reset_peak_memory_stats()
-        image = image.to(self.device, dtype=self.weight_dtype, non_blocking=True)
-        att_mask = att_mask.to(self.device, non_blocking=True)
+        image = data['img'].to(self.device, dtype=self.weight_dtype, non_blocking=True)
+        att_mask = data['mask'].to(self.device, non_blocking=True)
         prompt_ids = prompt_ids.to(self.device, non_blocking=True)
+        other_datas = {k: v.to(self.device, dtype=self.weight_dtype, non_blocking=True) for k, v in data.items() if k != 'img' and k != 'mask'}
 
         latents = self.get_latents(image, self.train_loader.dataset)
-        model_pred, target = self.forward(latents, prompt_ids)
+        model_pred, target = self.forward(latents, prompt_ids, **other_datas)
 
         if self.train_loader_class is not None:
             # DreamBooth prior forward
-            image_cls, att_mask_cls, prompt_ids_cls = next(self.data_iter_class)
-            image_cls = image_cls.to(self.device, dtype=self.weight_dtype)
-            att_mask_cls = att_mask_cls.to(self.device)
-            prompt_ids_cls = prompt_ids_cls.to(self.device)
+            data_cls, prompt_ids_cls = next(self.data_iter_class)
+            image_cls = data_cls['img'].to(self.device, dtype=self.weight_dtype, non_blocking=True)
+            att_mask_cls = data_cls['mask'].to(self.device, non_blocking=True)
+            prompt_ids_cls = prompt_ids_cls.to(self.device, non_blocking=True)
+            other_datas_cls = {k: v.to(self.device, dtype=self.weight_dtype, non_blocking=True) for k, v in data_cls.items() if k != 'img' and k != 'mask'}
             latents_cls = self.get_latents(image_cls, self.train_loader_class.dataset)
-            model_pred_prior, target_prior = self.forward(latents_cls, prompt_ids_cls)
+            model_pred_prior, target_prior = self.forward(latents_cls, prompt_ids_cls, **other_datas_cls)
 
             loss = self.get_loss(model_pred, target, att_mask)  # Compute instance loss
             prior_loss = self.get_loss(model_pred_prior, target_prior, att_mask_cls)  # Compute prior loss
             loss = loss + self.cfgs.train.loss.prior_loss_weight * prior_loss
         else:
             loss = self.get_loss(model_pred, target, att_mask)
 
@@ -158,25 +193,27 @@
 
     def update_ema(self):
         if hasattr(self, 'ema_unet'):
             self.ema_unet.step(get_static_torch_model(self.unet).named_parameters())
         if hasattr(self, 'ema_text_encoder'):
             self.ema_text_encoder.step(self.text_encoder.named_parameters())
 
-    def get_unet_raw(self):
+    @property
+    def unet_raw(self):
         if self.train_TE:
             unet = get_static_torch_model(self.TE_unet).unet
         else:
             unet = get_static_torch_model(self.unet)
         req_grad_dict = {k:v.requires_grad for k,v in self.unet.named_parameters()}
         for k,v in unet.named_parameters():
             v.requires_grad = req_grad_dict[k]
         return unet
 
-    def get_text_encoder_raw(self):
+    @property
+    def text_encoder_raw(self):
         if self.train_TE:
             TE = get_static_torch_model(self.TE_unet).TE
             req_grad_dict = {k: v.requires_grad for k, v in self.text_encoder.named_parameters()}
             for k, v in TE.named_parameters():
                 v.requires_grad = req_grad_dict[k]
         else:
             TE = self.text_encoder
```

### Comparing `hcpdiff-0.2.0/hcpdiff/utils/caption_tools.py` & `hcpdiff-0.2.1/hcpdiff/utils/caption_tools.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/hcpdiff/utils/cfg_net_tools.py` & `hcpdiff-0.2.1/hcpdiff/utils/cfg_net_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,205 +5,240 @@
     :Author:      Dong Ziyi
     :Affiliation: HCP Lab, SYSU
     :Created:     10/03/2023
     :Licence:     Apache-2.0
 """
 
 
-from typing import Dict, List, Iterable, Tuple, Union
+from typing import Dict, List, Iterable, Tuple, Union, Any
 
 import re
 import torch
 from torch import nn
 
-from .utils import dict_get
+from .utils import net_path_join
 from hcpdiff.models.lora_base import LoraBlock, LoraGroup
 from hcpdiff.models import lora_layers
 from hcpdiff.models.plugin import SinglePluginBlock, MultiPluginBlock, PluginBlock, PluginGroup
 from .ckpt_manager import CkptManagerPKL, CkptManagerSafe
 
 def get_class_match_layer(class_name, block:nn.Module):
     if type(block).__name__==class_name:
         return ['']
     else:
         return ['.'+name for name, layer in block.named_modules() if type(layer).__name__==class_name]
 
-def get_match_layers(layers, all_layers):
+def get_match_layers(layers, all_layers, return_metas=False) -> Union[List[str], List[Dict[str, Any]]]:
     res=[]
     for name in layers:
-        if isinstance(name, str):
-            if name.startswith('re:'):
-                pattern = re.compile(name[3:])
-                res.extend(filter(lambda x: pattern.match(x) != None, all_layers.keys()))
-            else:
-                res.append(name)
-        else:
-            pattern = re.compile(name[0][3:])
+        metas = name.split(':')
+
+        use_re = False
+        pre_hook = False
+        cls_filter = None
+        for meta in metas[:-1]:
+            if meta=='re':
+                use_re=True
+            elif meta=='pre_hook':
+                pre_hook=True
+            elif meta.startswith('cls('):
+                cls_filter=meta[4:-1]
+
+        name = metas[-1]
+        if use_re:
+            pattern = re.compile(name)
             match_layers = filter(lambda x: pattern.match(x) != None, all_layers.keys())
+        else:
+            match_layers = [name]
+
+        if cls_filter is not None:
+            match_layers_new = []
             for layer in match_layers:
-                res.extend([layer+x for x in get_class_match_layer(name[1], all_layers[layer])])
+                match_layers_new.extend([layer + x for x in get_class_match_layer(name[1], all_layers[layer])])
+            match_layers = match_layers_new
 
-    return sorted(set(res), key=res.index) # Remove duplicates and keep the original order
+        for layer in match_layers:
+            if return_metas:
+                res.append({'layer': layer, 'pre_hook': pre_hook})
+            else:
+                res.append(layer)
 
-def get_layers_with_block(named_modules:Dict[str, nn.Module], block_names:Iterable[str], cond:List=None):
-    layers=[]
-    for blk in block_names:
-        if type(named_modules[blk]) in cond:
-            layers.append(blk)
-        for name, layer in named_modules[blk].named_modules():
-            if type(named_modules[blk]) in cond:
-                layers.append(f'{blk}.{name}')
-    return layers
+    # Remove duplicates and keep the original order
+    if return_metas:
+        layer_set=set()
+        res_unique = []
+        for item in res:
+            if item['layer'] not in layer_set:
+                layer_set.add(item['layer'])
+                res_unique.append(item)
+        return res_unique
+    else:
+        return sorted(set(res), key=res.index)
+
+def get_lora_rank_and_cls(lora_state):
+    rank_groups = getattr(lora_state, 'layer.rank_groups', 1)
+    if rank_groups > 1:
+        if len(lora_state['layer.lora_down.weight'].shape) == 3:
+            rank = rank_groups * lora_state['layer.lora_down.weight'].shape[2]
+        else:
+            rank = lora_state['layer.lora_down.weight'].shape[0]
+        lora_layer_cls = lora_layers.layer_map['loha_group']
+    else:
+        rank = lora_state['layer.lora_down.weight'].shape[0]
+        lora_layer_cls = lora_layers.layer_map['lora']
+    return lora_layer_cls, rank, rank_groups
 
 def make_hcpdiff(model, cfg_model, cfg_lora, default_lr=1e-5) -> Tuple[List[Dict], Union[LoraGroup, Tuple[LoraGroup, LoraGroup]]]:
     named_modules = {k:v for k,v in model.named_modules()}
 
     train_params=[]
     all_lora_blocks={}
     all_lora_blocks_neg={}
 
     if cfg_model is not None:
         for item in cfg_model:
             for layer_name in get_match_layers(item.layers, named_modules):
                 layer = named_modules[layer_name]
                 layer.requires_grad_(True)
                 layer.train()
-                train_params.append({'params':list(LoraBlock.extract_param_without_lora(layer).values()), 'lr':dict_get(item, 'lr', default_lr)})
+                train_params.append({'params':list(LoraBlock.extract_param_without_lora(layer).values()), 'lr':getattr(item, 'lr', default_lr)})
 
     if cfg_lora is not None:
-        for item in cfg_lora:
+        for lora_id, item in enumerate(cfg_lora):
             for layer_name in get_match_layers(item.layers, named_modules):
                 layer = named_modules[layer_name]
                 arg_dict = {k:v for k,v in item.items() if k!='layers'}
-                lora_block_dict = lora_layers.layer_map[getattr(arg_dict, 'type', 'lora')].warp_model(layer, **arg_dict)
+                lora_block_dict = lora_layers.layer_map[getattr(arg_dict, 'type', 'lora')].wrap_model(lora_id, layer, **arg_dict)
+
+                params_group = []
                 block_branch = getattr(item, 'branch', None) # for DreamArtist-lora
                 for k,v in lora_block_dict.items():
+                    block_path = net_path_join(layer_name, k)
                     if block_branch is None:
-                        all_lora_blocks[f'{layer_name}.{k}'] = v
+                        all_lora_blocks[block_path] = v
                     elif block_branch=='p':
-                        all_lora_blocks[f'{layer_name}.{k}'] = v
+                        all_lora_blocks[block_path] = v
                         v.set_mask((0.5, 1))
                     elif block_branch == 'n':
-                        all_lora_blocks_neg[f'{layer_name}.{k}']=v
+                        all_lora_blocks_neg[block_path]=v
                         v.set_mask((0, 0.5))
+                    else:
+                        raise NotImplementedError(f'Unsupported branch "{block_branch}"')
+                    v.requires_grad_(True)
+                    v.train()
+                    params_group.extend(v.parameters())
 
-                params_group=[]
-                for block in lora_block_dict.values():
-                    block.requires_grad_(True)
-                    block.train()
-                    params_group.extend(block.parameters())
-                train_params.append({'params': params_group, 'lr':dict_get(item, 'lr', default_lr)})
+                train_params.append({'params': params_group, 'lr':getattr(item, 'lr', default_lr)})
 
     if len(all_lora_blocks_neg)>0:
         return train_params, (LoraGroup(all_lora_blocks), LoraGroup(all_lora_blocks_neg))
     else:
         return train_params, LoraGroup(all_lora_blocks)
 
-def make_plugin(model, cfg_plugin, default_lr=1e-5):
-    named_modules = {k:v for k,v in model.named_modules()}
-
+def make_plugin(model, cfg_plugin, default_lr=1e-5) -> Tuple[List, Dict[str, PluginGroup]]:
     train_params=[]
-    all_plugin_blocks={}
+    all_plugin_group={}
+
+    if cfg_plugin is None:
+        return train_params, all_plugin_group
+
+    named_modules = {k: v for k, v in model.named_modules()}
 
     # builder: functools.partial
     for plugin_name, builder in cfg_plugin.items():
-        lr = getattr(builder.keywords, 'lr', default_lr)
-        if 'lr' in builder.keywords:
-            del builder.keywords['lr']
+        all_plugin_blocks={}
+
+        lr = builder.keywords.pop('lr') if 'lr' in builder.keywords else default_lr
         plugin_class = getattr(builder.func, '__self__', builder.func) # support static or class method
 
         if issubclass(plugin_class, MultiPluginBlock):
-            from_layers = [named_modules[item] for item in get_match_layers(builder.keywords['from_layers'], named_modules)]
-            to_layers = [named_modules[item] for item in get_match_layers(builder.keywords['to_layers'], named_modules)]
-            del builder.keywords['from_layers']
-            del builder.keywords['to_layers']
+            from_layers = [{**item, 'layer':named_modules[item['layer']]} for item in get_match_layers(builder.keywords.pop('from_layers'), named_modules, return_metas=True)]
+            to_layers = [{**item, 'layer':named_modules[item['layer']]} for item in get_match_layers(builder.keywords.pop('to_layers'), named_modules, return_metas=True)]
 
-            layer = builder(host_model=model, from_layers=from_layers, to_layers=to_layers)
+            layer = builder(name=plugin_name, host_model=model, from_layers=from_layers, to_layers=to_layers)
             layer.requires_grad_(True)
             layer.train()
-            setattr(model, plugin_name, layer)
             train_params.append({'params': layer.parameters(), 'lr': lr})
-            all_plugin_blocks[plugin_name] = layer
+            all_plugin_blocks[''] = layer
         elif issubclass(plugin_class, SinglePluginBlock):
-            layers_name = builder.keywords['layers']
-            del builder.keywords['layers']
+            layers_name = builder.keywords.pop('layers')
             for layer_name in get_match_layers(layers_name, named_modules):
-                layer = builder(host_model=model, host=named_modules[layer_name])
+                blocks = builder(name=plugin_name, host_model=model, host=named_modules[layer_name])
+                if not isinstance(blocks, dict):
+                    blocks={'':blocks}
+
+                params_group = []
+                for k,v in blocks.items():
+                    all_plugin_blocks[net_path_join(layer_name, k)] = v
+                    v.requires_grad_(True)
+                    v.train()
+                train_params.append({'params': params_group, 'lr': lr})
+        elif issubclass(plugin_class, PluginBlock):
+            from_layer = get_match_layers(builder.keywords.pop('from_layer'), named_modules, return_metas=True)
+            to_layer = get_match_layers(builder.keywords.pop('to_layer'), named_modules, return_metas=True)
+
+            for from_layer_meta, to_layer_meta in zip(from_layer, to_layer):
+                from_layer_name=from_layer_meta['layer']
+                from_layer_meta['layer']=named_modules[from_layer_name]
+                to_layer_meta['layer']=named_modules[to_layer_meta['layer']]
+                layer = builder(name=plugin_name, host_model=model, from_layer=from_layer_meta, to_layer=to_layer_meta)
                 layer.requires_grad_(True)
                 layer.train()
-                setattr(named_modules[layer_name], plugin_name, layer)
                 train_params.append({'params': layer.parameters(), 'lr': lr})
-                all_plugin_blocks[f'{layer_name}.{plugin_name}'] = layer
-        elif issubclass(plugin_class, PluginBlock):
-            from_layer_name = builder.keywords['from_layer']
-            from_layer = named_modules[from_layer_name]
-            to_layer = named_modules[builder.keywords['to_layer']]
-            del builder.keywords['from_layer']
-            del builder.keywords['to_layer']
-
-            layer = builder(host_model=model, from_layer=from_layer, to_layer=to_layer)
-            layer.requires_grad_(True)
-            layer.train()
-            setattr(from_layer, plugin_name, layer)
-            train_params.append({'params': layer.parameters(), 'lr': lr})
-            all_plugin_blocks[f'{from_layer_name}.{plugin_name}'] = layer
+                all_plugin_blocks[from_layer_name] = layer
         else:
             raise NotImplementedError(f'Unknown plugin {plugin_class}')
-    return train_params, PluginGroup(all_plugin_blocks)
+        all_plugin_group[plugin_name] = PluginGroup(all_plugin_blocks)
+    return train_params, all_plugin_group
 
 @torch.no_grad()
 def load_hcpdiff(model:nn.Module, cfg_merge):
     named_modules = {k: v for k, v in model.named_modules()}
     named_params = {k: v for k, v in model.named_parameters()}
     all_lora_blocks = {}
 
     ckpt_manager_torch = CkptManagerPKL()
     ckpt_manager_safe = CkptManagerSafe()
 
     def get_ckpt_manager(path:str):
         return ckpt_manager_safe if path.endswith('.safetensors') else ckpt_manager_torch
 
     if "lora" in cfg_merge and cfg_merge.lora is not None:
-        for item in cfg_merge.lora:
+        for lora_id, item in enumerate(cfg_merge.lora):
             lora_state = get_ckpt_manager(item.path).load_ckpt(item.path, map_location='cpu')['lora']
             lora_block_state = {}
             # get all layers in the lora_state
             for name, p in lora_state.items():
-                lbidx = name.rfind('lora_block.')
-                if lbidx != -1:
-                    prefix = name[:lbidx - 1]
-                    if prefix not in lora_block_state:
-                        lora_block_state[prefix] = {}
-                    lora_block_state[prefix][name[lbidx + len('lora_block.'):]] = p
+                # lora_block. is the old format
+                prefix, block_name = name.split('.___.' if name.rfind('lora_block.')==-1 else '.lora_block.', 1)
+                if prefix not in lora_block_state:
+                    lora_block_state[prefix] = {}
+                lora_block_state[prefix][block_name] = p
             # get selected layers
             if item.layers != 'all':
                 match_blocks = get_match_layers(item.layers, named_modules)
-                match_layers = get_layers_with_block(named_modules, match_blocks, [nn.Linear, nn.Conv2d])
-                lora_block_state = {k: v for k, v in lora_block_state.items() if k in match_layers}
+                lora_state_new = {}
+                for k, v in lora_block_state.items():
+                    for mk in match_blocks:
+                        if k.startswith(mk):
+                            lora_state_new[k]=v
+                            break
+                lora_block_state = lora_state_new
             # add lora to host and load weights
             for host_name, lora_state in lora_block_state.items():
-                rank_groups=dict_get(lora_state, 'layer.rank_groups', 1)
-                if rank_groups>1:
-                    if len(lora_state['layer.lora_down.weight'].shape)==3:
-                        rank = rank_groups*lora_state['layer.lora_down.weight'].shape[2]
-                    else:
-                        rank = lora_state['layer.lora_down.weight'].shape[0]
-                    lora_layer = lora_layers.layer_map['loha_group']
-                else:
-                    rank = lora_state['layer.lora_down.weight'].shape[0]
-                    lora_layer = lora_layers.layer_map['lora']
+                lora_layer_cls, rank, rank_groups = get_lora_rank_and_cls(lora_state)
                 del lora_state['scale']
 
-                lora_block_dict = lora_layer.warp_model(named_modules[host_name], rank=rank, dropout=dict_get(item, 'dropout', 0.0),
-                                                 scale=dict_get(item, 'alpha', 1.0), bias='layer.lora_up.bias' in lora_state,
-                                                 rank_groups=rank_groups)
-                all_lora_blocks[f'{host_name}.lora_block'] = lora_block_dict['lora_block']
-                lora_block_dict['lora_block'].load_state_dict(lora_state, strict=False)
-                lora_block_dict['lora_block'].set_mask(dict_get(item, 'mask', None))
-                lora_block_dict['lora_block'].to(model.device)
+                lora_block = lora_layer_cls.wrap_layer(lora_id, named_modules[host_name], rank=rank, dropout=getattr(item, 'dropout', 0.0),
+                                                        scale=getattr(item, 'alpha', 1.0), bias='layer.lora_up.bias' in lora_state,
+                                                        rank_groups=rank_groups)
+                all_lora_blocks[f'{host_name}.{lora_block.name}'] = lora_block
+                lora_block.load_state_dict(lora_state, strict=False)
+                lora_block.set_mask(getattr(item, 'mask', None))
+                lora_block.to(model.device)
 
     if "part" in cfg_merge and cfg_merge.part is not None:
         for item in cfg_merge.part:
             part_state = get_ckpt_manager(item.path).load_ckpt(item.path, map_location='cpu')['base']
             if item.layers == 'all':
                 for k, v in part_state.items():
                     named_params[k].data = cfg_merge.base_model_alpha * named_params[k].data + item.alpha * v
```

### Comparing `hcpdiff-0.2.0/hcpdiff/utils/ckpt_manager/ckpt_pkl.py` & `hcpdiff-0.2.1/hcpdiff/utils/ckpt_manager/ckpt_pkl.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,79 +4,100 @@
     :Name:        save model with torch
     :Author:      Dong Ziyi
     :Affiliation: HCP Lab, SYSU
     :Created:     8/04/2023
     :Licence:     MIT
 """
 
+from typing import Dict
+import os
+
 import torch
 from torch import nn
-import os
+
 from hcpdiff.models.lora_base import LoraBlock, LoraGroup, split_state
-from hcpdiff.utils.emb_utils import save_emb
+from hcpdiff.models.plugin import PluginGroup, BasePluginBlock
+from hcpdiff.utils.net_utils import save_emb
+
 
 class CkptManagerPKL:
-    def __init__(self, lora_from_raw=False):
-        self.lora_from_raw = lora_from_raw
+    def __init__(self, plugin_from_raw=False):
+        self.plugin_from_raw = plugin_from_raw
 
     def set_save_dir(self, save_dir, emb_dir=None):
         os.makedirs(save_dir, exist_ok=True)
         self.save_dir = save_dir
         self.emb_dir = emb_dir
 
     def exclude_state(self, state, key):
         if key is None:
             return state
         else:
-            return {k:v for k,v in state.items() if key in k}
+            return {k: v for k, v in state.items() if key in k}
 
     def save_model(self, model: nn.Module, name, step, model_ema=None, exclude_key=None):
         sd_model = {
             'base': self.exclude_state(LoraBlock.extract_trainable_state_without_lora(model), exclude_key),
         }
         if model_ema is not None:
             sd_ema, sd_ema_lora = split_state(model_ema.state_dict())
             sd_model['base_ema'] = self.exclude_state(sd_ema, exclude_key)
         self._save_ckpt(sd_model, name, step)
 
-    def save_model_with_lora(self, model: nn.Module, lora_blocks: LoraGroup, name, step, model_ema=None,
+    def save_plugins(self, host_model: nn.Module, plugins: Dict[str, PluginGroup], name:str, step:int, model_ema=None):
+        if len(plugins)>0:
+            sd_plugin={}
+            for plugin_name, plugin in plugins.items():
+                sd_plugin['plugin'] = plugin.state_dict(host_model if self.plugin_from_raw else None)
+                if model_ema is not None:
+                    sd_plugin['plugin_ema'] = plugin.state_dict(model_ema)
+                self._save_ckpt(sd_plugin, f'{name}-{plugin_name}', step)
+
+    def save_model_with_lora(self, model: nn.Module, lora_blocks: LoraGroup, name:str, step:int, model_ema=None,
                              exclude_key=None):
         sd_model = {
-            'base': self.exclude_state(LoraBlock.extract_trainable_state_without_lora(model), exclude_key),
+            'base': self.exclude_state(BasePluginBlock.extract_state_without_plugin(model, trainable=True), exclude_key),
         } if model is not None else {}
-        if not lora_blocks.empty():
-            sd_model['lora']=lora_blocks.state_dict(model if self.lora_from_raw else None)
+        if (lora_blocks is not None) and (not lora_blocks.empty()):
+            sd_model['lora'] = lora_blocks.state_dict(model if self.plugin_from_raw else None)
 
         if model_ema is not None:
-            sd_ema, sd_ema_lora = split_state(model_ema.state_dict())
-            sd_model['base_ema'] = self.exclude_state(sd_ema, exclude_key)
-            if not lora_blocks.empty():
-                sd_model['lora_ema'] = {sd_ema_lora[k] for k in sd_model['lora'].keys()}
+            ema_state = model_ema.state_dict()
+            if model is not None:
+                sd_ema = {k:ema_state[k] for k in sd_model['base'].keys()}
+                sd_model['base_ema'] = self.exclude_state(sd_ema, exclude_key)
+            if (lora_blocks is not None) and (not lora_blocks.empty()):
+                sd_model['lora_ema'] = {k:ema_state[k] for k in sd_model['lora'].keys()}
 
         self._save_ckpt(sd_model, name, step)
 
     def _save_ckpt(self, sd_model, name, step, save_path=None):
         if save_path is None:
             save_path = os.path.join(self.save_dir, f"{name}-{step}.ckpt")
         torch.save(sd_model, save_path)
 
     def load_ckpt(self, ckpt_path, map_location='cpu'):
         return torch.load(ckpt_path, map_location=map_location)
 
-    def load_ckpt_to_model(self, model:nn.Module, ckpt_path, model_ema=None):
+    def load_ckpt_to_model(self, model: nn.Module, ckpt_path, model_ema=None):
         sd = self.load_ckpt(ckpt_path)
         if 'base' in sd:
             model.load_state_dict(sd['base'], strict=False)
         if 'lora' in sd:
             model.load_state_dict(sd['lora'], strict=False)
+        if 'plugin' in sd:
+            model.load_state_dict(sd['plugin'], strict=False)
 
         if model_ema is not None:
-            model_ema.load_state_dict(sd['base_ema'])
-            model_ema.load_state_dict(sd['lora_ema'])
-
+            if 'base' in sd:
+                model_ema.load_state_dict(sd['base_ema'])
+            if 'lora' in sd:
+                model_ema.load_state_dict(sd['lora_ema'])
+            if 'plugin' in sd:
+                model_ema.load_state_dict(sd['plugin_ema'])
 
     def save_embedding(self, train_pts, step, replace):
         for k, v in train_pts.items():
             save_path = os.path.join(self.save_dir, f"{k}-{step}.pt")
             save_emb(save_path, v.data, replace=True)
             if replace:
-                save_emb(f'{k}.pt', v.data, replace=True)
+                save_emb(f'{k}.pt', v.data, replace=True)
```

### Comparing `hcpdiff-0.2.0/hcpdiff/utils/ckpt_manager/ckpt_safetensor.py` & `hcpdiff-0.2.1/hcpdiff/utils/ckpt_manager/ckpt_safetensor.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/hcpdiff/utils/colo_utils.py` & `hcpdiff-0.2.1/hcpdiff/utils/colo_utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/hcpdiff/utils/ema.py` & `hcpdiff-0.2.1/hcpdiff/utils/ema.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/hcpdiff/utils/img_size_tool.py` & `hcpdiff-0.2.1/hcpdiff/utils/img_size_tool.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/hcpdiff/utils/net_utils.py` & `hcpdiff-0.2.1/hcpdiff/utils/net_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import os
 from typing import Optional, Union, Tuple, Dict, Callable
 
+import torch
 from torch import nn
 from torch.optim import lr_scheduler
 from diffusers.optimization import SchedulerType, TYPE_TO_SCHEDULER_FUNCTION, Optimizer
 from transformers import PretrainedConfig
 from collections import OrderedDict
 
 class TEUnetWrapper(nn.Module):
@@ -106,21 +108,30 @@
 
         return RobertaSeriesModelWithTransformation
     else:
         raise ValueError(f"{model_class} is not supported.")
 
 def remove_all_hooks(model: nn.Module) -> None:
     for name, child in model.named_modules():
-        if hasattr(child, "_forward_hooks"):
-            child._forward_hooks: Dict[int, Callable] = OrderedDict()
-        elif hasattr(child, "_forward_pre_hooks"):
-            child._forward_pre_hooks: Dict[int, Callable] = OrderedDict()
-        elif hasattr(child, "_backward_hooks"):
-            child._backward_hooks: Dict[int, Callable] = OrderedDict()
+        child._forward_hooks.clear()
+        child._forward_pre_hooks.clear()
+        child._backward_hooks.clear()
 
 def remove_layers(model: nn.Module, layer_class):
     named_modules = {k: v for k, v in model.named_modules()}
     for k,v in named_modules.items():
         if isinstance(v, layer_class):
             parent, name = named_modules[k.rsplit('.', 1)]
             delattr(parent, name)
             del v
+
+def load_emb(path):
+    emb=torch.load(path, map_location='cpu')['string_to_param']['*']
+    emb.requires_grad_(False)
+    return emb
+
+def save_emb(path, emb:torch.Tensor, replace=False):
+    name = os.path.basename(path)
+    if os.path.exists(path) and not replace:
+        raise FileExistsError(f'embedding "{name}" already exist.')
+    name=name[:name.rfind('.')]
+    torch.save({'string_to_param':{'*':emb}, 'name':name}, path)
```

### Comparing `hcpdiff-0.2.0/hcpdiff/utils/utils.py` & `hcpdiff-0.2.1/hcpdiff/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, Tuple
+from typing import Tuple
 
 import re
 import torch
 from omegaconf import OmegaConf
 
 def str2bool(v):
     return v.lower() in ("yes", "true", "t", "1")
@@ -46,26 +46,14 @@
     cfg_cli = OmegaConf.from_cli(args_list)
     cfg = OmegaConf.merge(cfg, cfg_cli)
     return cfg
 
 def _default(v, default):
     return default if v is None else v
 
-def dict_get(data, key, default):
-    return data[key] if key in data else default
-
-def cycle_data(data_loader, arb=False):
-    epoch=0
-    while True:
-        if arb:
-            data_loader.dataset.bucket.rest(epoch)
-        for data in data_loader:
-            yield data
-        epoch+=1
-
 def get_cfg_range(cfg_text:str):
     dy_cfg_f='ln'
     if cfg_text.find(':')!=-1:
         cfg_text, dy_cfg_f = cfg_text.split(':')
 
     if cfg_text.find('-')!=-1:
         l, h = cfg_text.split('-')
@@ -91,8 +79,17 @@
 
 def factorization(dimension: int, factor:int=-1) -> Tuple[int, int]:
     find_one = lambda x: len(x) - (x.rfind('1') + 1)
     dim_bin = bin(dimension)
     num = find_one(dim_bin)
     f_max = (len(dim_bin)-3)>>1 if factor<0 else find_one(bin(factor))
     num = min(num, f_max)
-    return dimension>>num, 1<<num
+    return dimension>>num, 1<<num
+
+def isinstance_list(obj, cls_list):
+    for cls in cls_list:
+        if isinstance(obj, cls):
+            return True
+    return False
+
+def net_path_join(*args):
+    return '.'.join(args).strip('.').replace('..', '.')
```

### Comparing `hcpdiff-0.2.0/hcpdiff/visualizer.py` & `hcpdiff-0.2.1/hcpdiff/visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 class UnetHook(): # for controlnet
     def __init__(self, unet):
         self.unet = unet
         self.call_raw = UNet2DConditionModel.__call__
         UNet2DConditionModel.__call__ = self.unet_call
 
     def unet_call(self, sample, timestep, encoder_hidden_states, **kwargs):
-        return self.call_raw(self.unet, sample, timestep, encoder_hidden_states, **kwargs)
+        return self.call_raw(self.unet, sample, timestep, encoder_hidden_states)
 
 class Visualizer:
     def __init__(self, cfgs):
         self.cfgs_raw = cfgs
         self.cfgs = hydra.utils.instantiate(self.cfgs_raw)
         self.cfg_merge = self.cfgs.merge
 
@@ -61,15 +61,16 @@
                 return StableDiffusionPipeline
             else:
                 raise NotImplementedError(f'No condition type named {self.cfgs.condition.type}')
 
     def merge_model(self):
         if 'plugin_cfg' in self.cfg_merge: # Build plugins
             plugin_cfg = hydra.utils.instantiate(load_config(self.cfg_merge.plugin_cfg))
-            make_plugin(self.pipe.unet, plugin_cfg.plugin)
+            make_plugin(self.pipe.unet, plugin_cfg.plugin_unet)
+            make_plugin(self.pipe.text_encoder, plugin_cfg.plugin_TE)
 
         for cfg_group in self.cfg_merge.values():
             if hasattr(cfg_group, 'type'):
                 if cfg_group.type == 'unet':
                     load_hcpdiff(self.pipe.unet, cfg_group)
                 elif cfg_group.type == 'TE':
                     load_hcpdiff(self.pipe.text_encoder, cfg_group)
```

### Comparing `hcpdiff-0.2.0/hcpdiff.egg-info/PKG-INFO` & `hcpdiff-0.2.1/hcpdiff.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.2.0
+Version: 0.2.1
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -52,14 +52,15 @@
 * Custom words that occupy multiple words
 * Maximum sentence length expansion
 * colossal-AI
 * xformers for unet and text-encoder
 * CLIP skip
 * Tag shuffle and dropout
 * safetensors support
+* Controlnet (support train)
 
 ## Install
 
 Install with pip:
 ```bash
 pip install hcpdiff
 # Start a new project and make initialization
```

### Comparing `hcpdiff-0.2.0/hcpdiff.egg-info/SOURCES.txt` & `hcpdiff-0.2.1/hcpdiff.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 cfgs/te_struct.txt
 cfgs/unet_struct.txt
 cfgs/infer/change_vae.yaml
 cfgs/infer/euler_a.yaml
 cfgs/infer/img2img.yaml
 cfgs/infer/img2img_controlnet.yaml
 cfgs/infer/text2img.yaml
-cfgs/train/plugin_control.yaml
+cfgs/plugins/plugin_controlnet.yaml
 cfgs/train/train_base.yaml
 cfgs/train/tuning_base.yaml
 cfgs/train/examples/CustomDiffusion.yaml
 cfgs/train/examples/DreamArtist++.yaml
 cfgs/train/examples/DreamArtist.yaml
 cfgs/train/examples/DreamBooth.yaml
 cfgs/train/examples/TextualInversion.yaml
+cfgs/train/examples/controlnet.yaml
 cfgs/train/examples/fine-tuning.yaml
 cfgs/train/examples/locon.yaml
 cfgs/train/examples/lora_conventional.yaml
 hcpdiff/__init__.py
 hcpdiff/train_ac.py
 hcpdiff/train_ac_single.py
 hcpdiff/train_colo.py
@@ -28,14 +29,15 @@
 hcpdiff.egg-info/SOURCES.txt
 hcpdiff.egg-info/dependency_links.txt
 hcpdiff.egg-info/entry_points.txt
 hcpdiff.egg-info/requires.txt
 hcpdiff.egg-info/top_level.txt
 hcpdiff/data/__init__.py
 hcpdiff/data/bucket.py
+hcpdiff/data/cond_pair_dataset.py
 hcpdiff/data/pair_dataset.py
 hcpdiff/data/utils.py
 hcpdiff/models/__init__.py
 hcpdiff/models/cfg_context.py
 hcpdiff/models/controlnet.py
 hcpdiff/models/layers.py
 hcpdiff/models/lora_base.py
@@ -45,22 +47,20 @@
 hcpdiff/models/textencoder_ex.py
 hcpdiff/models/tokenizer_ex.py
 hcpdiff/tools/__init__.py
 hcpdiff/tools/convert_caption_txt2json.py
 hcpdiff/tools/create_embedding.py
 hcpdiff/tools/gen_from_ptlist.py
 hcpdiff/tools/init_proj.py
-hcpdiff/tools/merge_model_part.py
 hcpdiff/tools/sd2diffusers.py
 hcpdiff/utils/__init__.py
 hcpdiff/utils/caption_tools.py
 hcpdiff/utils/cfg_net_tools.py
 hcpdiff/utils/colo_utils.py
 hcpdiff/utils/ema.py
-hcpdiff/utils/emb_utils.py
 hcpdiff/utils/img_size_tool.py
 hcpdiff/utils/net_utils.py
 hcpdiff/utils/utils.py
 hcpdiff/utils/ckpt_manager/__init__.py
 hcpdiff/utils/ckpt_manager/ckpt_pkl.py
 hcpdiff/utils/ckpt_manager/ckpt_safetensor.py
 prompt_tuning_template/caption.txt
```

### Comparing `hcpdiff-0.2.0/prompt_tuning_template/object.txt` & `hcpdiff-0.2.1/prompt_tuning_template/object.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/prompt_tuning_template/object_caption.txt` & `hcpdiff-0.2.1/prompt_tuning_template/object_caption.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/prompt_tuning_template/style.txt` & `hcpdiff-0.2.1/prompt_tuning_template/style.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/prompt_tuning_template/style_caption.txt` & `hcpdiff-0.2.1/prompt_tuning_template/style_caption.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/setup.py` & `hcpdiff-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             file_dict[prefix+root].append(os.path.join(root, name))
     return [(k, v) for k, v in file_dict.items()]
 
 
 setuptools.setup(
     name="hcpdiff",
     py_modules=["hcpdiff"],
-    version="0.2.0",
+    version="0.2.1",
     author="Ziyi Dong",
     author_email="dzy7eu7d7@gmail.com",
     description="A universal Stable-Diffusion toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/7eu7d7/HCP-Diffusion",
     packages=setuptools.find_packages(),
```

### Comparing `hcpdiff-0.2.0/test/test_combine.py` & `hcpdiff-0.2.1/test/test_combine.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/test/test_ctnet.py` & `hcpdiff-0.2.1/test/test_ctnet.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/test/test_paradict.py` & `hcpdiff-0.2.1/test/test_paradict.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.2.0/test/test_plugin_param.py` & `hcpdiff-0.2.1/test/test_plugin_param.py`

 * *Files identical despite different names*


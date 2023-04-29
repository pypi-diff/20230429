# Comparing `tmp/classy_imaginary-0.5.6.tar.gz` & `tmp/classy_imaginary-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classy_imaginary-0.5.6.tar", max compression
+gzip compressed data, was "classy_imaginary-0.5.7.tar", max compression
```

## Comparing `classy_imaginary-0.5.6.tar` & `classy_imaginary-0.5.7.tar`

### file list

```diff
@@ -1,227 +1,228 @@
--rw-r--r--   0        0        0     1160 2023-01-01 18:59:37.438650 classy_imaginary-0.5.6/LICENSE
--rw-r--r--   0        0        0       93 2023-01-02 15:20:36.641278 classy_imaginary-0.5.6/README.md
--rw-r--r--   0        0        0     2043 2023-04-21 09:08:07.571186 classy_imaginary-0.5.6/classy_imaginary/Caption.py
--rw-r--r--   0        0        0      626 2023-04-02 11:44:50.071771 classy_imaginary-0.5.6/classy_imaginary/FixFaces.py
--rw-r--r--   0        0        0     4198 2023-03-19 16:37:49.495325 classy_imaginary-0.5.6/classy_imaginary/Imagine.py
--rw-r--r--   0        0        0      672 2023-04-02 11:38:50.249560 classy_imaginary-0.5.6/classy_imaginary/Upscaler.py
--rw-r--r--   0        0        0      286 2023-02-04 14:48:22.568510 classy_imaginary-0.5.6/classy_imaginary/__init__.py
--rw-r--r--   0        0        0     3873 2023-03-19 16:33:37.082877 classy_imaginary-0.5.6/classy_imaginary/animations.py
--rwxr-xr-x   0        0        0    28771 2023-04-02 11:44:50.095772 classy_imaginary-0.5.6/classy_imaginary/api.py
--rw-r--r--   0        0        0      143 2023-03-19 15:49:53.552654 classy_imaginary-0.5.6/classy_imaginary/bin/aimg
--rw-r--r--   0        0        0      153 2023-03-19 15:49:53.540653 classy_imaginary-0.5.6/classy_imaginary/bin/imagine
--rw-r--r--   0        0        0        0 2023-03-18 11:53:39.545078 classy_imaginary-0.5.6/classy_imaginary/cli/__init__.py
--rw-r--r--   0        0        0     1588 2023-03-19 15:50:31.837328 classy_imaginary-0.5.6/classy_imaginary/cli/colorize.py
--rw-r--r--   0        0        0      674 2023-03-19 15:50:38.637448 classy_imaginary-0.5.6/classy_imaginary/cli/describe.py
--rw-r--r--   0        0        0     3199 2023-03-19 15:51:05.949929 classy_imaginary-0.5.6/classy_imaginary/cli/edit.py
--rw-r--r--   0        0        0      985 2023-03-19 15:51:17.810138 classy_imaginary-0.5.6/classy_imaginary/cli/edit_demo.py
--rw-r--r--   0        0        0     3083 2023-03-19 15:51:24.066248 classy_imaginary-0.5.6/classy_imaginary/cli/imagine.py
--rw-r--r--   0        0        0     2582 2023-03-19 15:51:44.050600 classy_imaginary-0.5.6/classy_imaginary/cli/main.py
--rw-r--r--   0        0        0    15230 2023-03-19 15:52:44.039657 classy_imaginary-0.5.6/classy_imaginary/cli/shared.py
--rw-r--r--   0        0        0     8197 2023-03-19 15:53:34.780551 classy_imaginary-0.5.6/classy_imaginary/cli/train.py
--rw-r--r--   0        0        0     1627 2023-03-19 15:53:47.464774 classy_imaginary-0.5.6/classy_imaginary/cli/upscale.py
--rw-r--r--   0        0        0     1385 2023-03-19 16:41:57.663698 classy_imaginary-0.5.6/classy_imaginary/colorize.py
--rw-r--r--   0        0        0    14609 2023-03-26 11:32:04.673850 classy_imaginary-0.5.6/classy_imaginary/config.py
--rw-r--r--   0        0        0     2036 2023-02-25 11:37:14.631990 classy_imaginary-0.5.6/classy_imaginary/configs/control-net-v15.yaml
--rw-r--r--   0        0        0     1855 2023-02-11 14:49:23.869154 classy_imaginary-0.5.6/classy_imaginary/configs/graphicArt_graphicArtBeta.yaml
--rw-r--r--   0        0        0     1855 2023-01-31 15:58:02.862557 classy_imaginary-0.5.6/classy_imaginary/configs/instruct-pix2pix.yaml
--rw-r--r--   0        0        0     2055 2023-01-02 12:25:06.421175 classy_imaginary-0.5.6/classy_imaginary/configs/stable-diffusion-v1-inpaint.yaml
--rw-r--r--   0        0        0     1998 2023-01-31 15:58:02.862557 classy_imaginary-0.5.6/classy_imaginary/configs/stable-diffusion-v1.yaml
--rw-r--r--   0        0        0     1855 2023-02-11 14:49:23.881155 classy_imaginary-0.5.6/classy_imaginary/configs/stable-diffusion-v2-inference-v.yaml
--rw-r--r--   0        0        0     1829 2023-01-02 12:25:06.405175 classy_imaginary-0.5.6/classy_imaginary/configs/stable-diffusion-v2-inference.yaml
--rw-r--r--   0        0        0     4489 2023-01-02 12:25:06.369174 classy_imaginary-0.5.6/classy_imaginary/configs/stable-diffusion-v2-inpainting-inference.yaml
--rw-r--r--   0        0        0     1921 2023-01-02 12:25:06.489176 classy_imaginary-0.5.6/classy_imaginary/configs/stable-diffusion-v2-midas-inference.yaml
--rw-r--r--   0        0        0     1835 2023-01-31 15:57:51.570357 classy_imaginary-0.5.6/classy_imaginary/configs/stable-diffusion-v2-modern-buildings.yaml
--rw-r--r--   0        0        0     2265 2023-01-02 12:23:06.747039 classy_imaginary-0.5.6/classy_imaginary/configs/stable-diffusion-x4-upscaling.yaml
--rw-r--r--   0        0        0   757076 2023-01-31 15:58:02.866557 classy_imaginary-0.5.6/classy_imaginary/data/DejaVuSans.ttf
--rw-r--r--   0        0        0     1402 2023-03-19 16:50:17.952505 classy_imaginary-0.5.6/classy_imaginary/debug_info.py
--rw-r--r--   0        0        0        0 2023-01-01 18:59:37.466651 classy_imaginary-0.5.6/classy_imaginary/enhancers/__init__.py
--rw-r--r--   0        0        0      444 2023-02-04 16:14:10.370494 classy_imaginary-0.5.6/classy_imaginary/enhancers/blur_detect.py
--rw-r--r--   0        0        0     5114 2023-01-01 18:59:37.466651 classy_imaginary-0.5.6/classy_imaginary/enhancers/bool_masker.py
--rw-r--r--   0        0        0     3157 2023-01-02 12:25:06.525177 classy_imaginary-0.5.6/classy_imaginary/enhancers/clip_masking.py
--rw-r--r--   0        0        0     1838 2023-01-31 15:58:02.866557 classy_imaginary-0.5.6/classy_imaginary/enhancers/describe_image_blip.py
--rw-r--r--   0        0        0     2071 2023-01-31 15:58:02.866557 classy_imaginary-0.5.6/classy_imaginary/enhancers/describe_image_clip.py
--rw-r--r--   0        0        0     3376 2023-02-25 11:41:27.819950 classy_imaginary-0.5.6/classy_imaginary/enhancers/face_restoration_codeformer.py
--rw-r--r--   0        0        0     1908 2023-02-04 16:14:10.362493 classy_imaginary-0.5.6/classy_imaginary/enhancers/facecrop.py
--rw-r--r--   0        0        0        0 2023-01-01 18:59:37.470651 classy_imaginary-0.5.6/classy_imaginary/enhancers/phraselists/__init__.py
--rw-r--r--   0        0        0   169986 2023-03-18 11:53:39.549078 classy_imaginary-0.5.6/classy_imaginary/enhancers/phraselists/art-scene.txt
--rw-r--r--   0        0        0      102 2023-01-01 18:59:37.470651 classy_imaginary-0.5.6/classy_imaginary/enhancers/phraselists/color.txt
--rw-r--r--   0        0        0      249 2023-03-19 15:55:30.014581 classy_imaginary-0.5.6/classy_imaginary/enhancers/phraselists/desktop-background.txt
--rw-r--r--   0        0        0      571 2023-03-18 11:53:39.549078 classy_imaginary-0.5.6/classy_imaginary/enhancers/phraselists/interior-style.txt
--rw-r--r--   0        0        0      238 2023-03-18 11:53:39.549078 classy_imaginary-0.5.6/classy_imaginary/enhancers/phraselists/painting-style.txt
--rw-r--r--   0        0        0      226 2023-01-01 18:59:37.470651 classy_imaginary-0.5.6/classy_imaginary/enhancers/phraselists/spaceship.txt
--rw-r--r--   0        0        0     8941 2023-01-31 15:58:02.866557 classy_imaginary-0.5.6/classy_imaginary/enhancers/prompt_expansion.py
--rw-r--r--   0        0        0     1133 2023-01-31 15:58:02.866557 classy_imaginary-0.5.6/classy_imaginary/enhancers/upscale_realesrgan.py
--rw-r--r--   0        0        0    11254 2023-03-19 16:00:45.324136 classy_imaginary-0.5.6/classy_imaginary/enhancers/upscale_riverwing.py
--rw-r--r--   0        0        0     6920 2023-03-19 16:50:17.960506 classy_imaginary-0.5.6/classy_imaginary/feather_tile.py
--rw-r--r--   0        0        0        0 2023-02-25 11:33:31.076460 classy_imaginary-0.5.6/classy_imaginary/img_processors/__init__.py
--rw-r--r--   0        0        0     4590 2023-02-25 13:14:32.287913 classy_imaginary-0.5.6/classy_imaginary/img_processors/control_modes.py
--rw-r--r--   0        0        0     7312 2023-02-25 13:14:32.271913 classy_imaginary-0.5.6/classy_imaginary/img_processors/hed_boundary.py
--rw-r--r--   0        0        0    29586 2023-03-19 16:02:08.369599 classy_imaginary-0.5.6/classy_imaginary/img_processors/openpose.py
--rw-r--r--   0        0        0     5090 2023-02-25 13:27:31.053289 classy_imaginary-0.5.6/classy_imaginary/img_utils.py
--rw-r--r--   0        0        0     9341 2023-02-25 12:30:37.397944 classy_imaginary-0.5.6/classy_imaginary/log_utils.py
--rw-r--r--   0        0        0     4153 2023-01-31 15:58:02.866557 classy_imaginary-0.5.6/classy_imaginary/lr_scheduler.py
--rw-r--r--   0        0        0    15329 2023-03-19 16:50:17.940505 classy_imaginary-0.5.6/classy_imaginary/model_manager.py
--rw-r--r--   0        0        0        0 2023-01-01 18:59:37.470651 classy_imaginary-0.5.6/classy_imaginary/modules/__init__.py
--rw-r--r--   0        0        0    16627 2023-03-25 10:32:03.625304 classy_imaginary-0.5.6/classy_imaginary/modules/attention.py
--rw-r--r--   0        0        0    23309 2023-03-19 16:04:52.700495 classy_imaginary-0.5.6/classy_imaginary/modules/autoencoder.py
--rw-r--r--   0        0        0    20318 2023-03-19 16:05:30.533161 classy_imaginary-0.5.6/classy_imaginary/modules/cldm.py
--rw-r--r--   0        0        0     3651 2023-01-31 15:58:02.866557 classy_imaginary-0.5.6/classy_imaginary/modules/clip_embedders.py
--rw-r--r--   0        0        0        0 2023-01-01 18:59:37.470651 classy_imaginary-0.5.6/classy_imaginary/modules/diffusion/__init__.py
--rw-r--r--   0        0        0    81030 2023-03-19 16:07:16.747033 classy_imaginary-0.5.6/classy_imaginary/modules/diffusion/ddpm.py
--rw-r--r--   0        0        0    34779 2023-03-25 10:31:46.085010 classy_imaginary-0.5.6/classy_imaginary/modules/diffusion/model.py
--rw-r--r--   0        0        0    31716 2023-01-31 15:58:02.870557 classy_imaginary-0.5.6/classy_imaginary/modules/diffusion/openaimodel.py
--rw-r--r--   0        0        0     3599 2023-01-02 12:23:06.791039 classy_imaginary-0.5.6/classy_imaginary/modules/diffusion/upscaling.py
--rw-r--r--   0        0        0     9799 2023-02-25 11:53:22.130967 classy_imaginary-0.5.6/classy_imaginary/modules/diffusion/util.py
--rw-r--r--   0        0        0     1651 2023-01-01 18:59:37.474651 classy_imaginary-0.5.6/classy_imaginary/modules/distributions.py
--rw-r--r--   0        0        0     3290 2023-01-01 18:59:37.474651 classy_imaginary-0.5.6/classy_imaginary/modules/ema.py
--rw-r--r--   0        0        0     8089 2023-01-31 15:58:02.870557 classy_imaginary-0.5.6/classy_imaginary/modules/encoders.py
--rw-r--r--   0        0        0        0 2023-01-01 18:59:37.474651 classy_imaginary-0.5.6/classy_imaginary/modules/midas/__init__.py
--rw-r--r--   0        0        0     6606 2023-02-25 11:53:22.102967 classy_imaginary-0.5.6/classy_imaginary/modules/midas/api.py
--rw-r--r--   0        0        0        0 2023-01-01 18:59:37.474651 classy_imaginary-0.5.6/classy_imaginary/modules/midas/midas/__init__.py
--rw-r--r--   0        0        0      567 2023-01-31 15:58:02.870557 classy_imaginary-0.5.6/classy_imaginary/modules/midas/midas/base_model.py
--rw-r--r--   0        0        0     9817 2023-01-01 18:59:37.474651 classy_imaginary-0.5.6/classy_imaginary/modules/midas/midas/blocks.py
--rw-r--r--   0        0        0     3082 2023-03-19 16:07:16.759033 classy_imaginary-0.5.6/classy_imaginary/modules/midas/midas/dpt_depth.py
--rw-r--r--   0        0        0     2716 2023-01-31 15:58:02.870557 classy_imaginary-0.5.6/classy_imaginary/modules/midas/midas/midas_net.py
--rw-r--r--   0        0        0     5885 2023-01-31 15:58:02.870557 classy_imaginary-0.5.6/classy_imaginary/modules/midas/midas/midas_net_custom.py
--rw-r--r--   0        0        0     7845 2023-01-01 18:59:37.474651 classy_imaginary-0.5.6/classy_imaginary/modules/midas/midas/transforms.py
--rw-r--r--   0        0        0    14588 2023-01-31 15:58:02.870557 classy_imaginary-0.5.6/classy_imaginary/modules/midas/midas/vit.py
--rw-r--r--   0        0        0     5058 2023-02-25 11:53:22.078966 classy_imaginary-0.5.6/classy_imaginary/modules/midas/utils.py
--rw-r--r--   0        0        0     7679 2023-02-25 12:35:44.323298 classy_imaginary-0.5.6/classy_imaginary/outpaint.py
--rw-r--r--   0        0        0       53 2023-01-01 18:59:37.474651 classy_imaginary-0.5.6/classy_imaginary/paths.py
--rw-r--r--   0        0        0     2279 2023-01-31 15:58:02.870557 classy_imaginary-0.5.6/classy_imaginary/prompt_schedules.py
--rw-r--r--   0        0        0     3371 2023-01-31 15:58:02.870557 classy_imaginary-0.5.6/classy_imaginary/roi_utils.py
--rw-r--r--   0        0        0     5945 2023-02-04 14:58:22.938902 classy_imaginary-0.5.6/classy_imaginary/safety.py
--rw-r--r--   0        0        0      681 2023-01-02 12:25:06.565178 classy_imaginary-0.5.6/classy_imaginary/samplers/__init__.py
--rw-r--r--   0        0        0     5957 2023-01-02 12:23:07.087045 classy_imaginary-0.5.6/classy_imaginary/samplers/base.py
--rw-r--r--   0        0        0     7277 2023-03-19 16:09:15.349122 classy_imaginary-0.5.6/classy_imaginary/samplers/ddim.py
--rw-r--r--   0        0        0     1974 2023-02-04 16:14:10.354493 classy_imaginary-0.5.6/classy_imaginary/samplers/editing.py
--rw-r--r--   0        0        0     7989 2023-03-19 16:09:45.945661 classy_imaginary-0.5.6/classy_imaginary/samplers/kdiff.py
--rw-r--r--   0        0        0     8444 2023-03-19 16:10:47.082738 classy_imaginary-0.5.6/classy_imaginary/samplers/plms.py
--rw-r--r--   0        0        0    13620 2023-03-19 16:50:17.916505 classy_imaginary-0.5.6/classy_imaginary/schema.py
--rw-r--r--   0        0        0     7368 2023-01-31 15:58:02.870557 classy_imaginary-0.5.6/classy_imaginary/surprise_me.py
--rw-r--r--   0        0        0    18313 2023-03-19 16:52:01.450327 classy_imaginary-0.5.6/classy_imaginary/train.py
--rw-r--r--   0        0        0        0 2023-01-31 15:58:02.870557 classy_imaginary-0.5.6/classy_imaginary/training_tools/__init__.py
--rw-r--r--   0        0        0     6197 2023-03-19 16:11:55.303940 classy_imaginary-0.5.6/classy_imaginary/training_tools/image_prep.py
--rw-r--r--   0        0        0     1061 2023-01-31 15:58:02.870557 classy_imaginary-0.5.6/classy_imaginary/training_tools/prune_model.py
--rw-r--r--   0        0        0     4311 2023-01-31 15:58:02.870557 classy_imaginary-0.5.6/classy_imaginary/training_tools/single_concept.py
--rw-r--r--   0        0        0     5757 2023-03-19 16:52:01.470327 classy_imaginary-0.5.6/classy_imaginary/utils.py
--rw-r--r--   0        0        0        0 2023-01-01 18:59:37.474651 classy_imaginary-0.5.6/classy_imaginary/vendored/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 17:05:50.960915 classy_imaginary-0.5.6/classy_imaginary/vendored/basicsr/__init__.py
--rw-r--r--   0        0        0     2526 2023-03-19 17:05:59.969074 classy_imaginary-0.5.6/classy_imaginary/vendored/basicsr/arch_util.py
--rw-r--r--   0        0        0     6458 2023-01-31 15:58:02.870557 classy_imaginary-0.5.6/classy_imaginary/vendored/basicsr/img_util.py
--rw-r--r--   0        0        0     4723 2023-01-31 15:58:02.870557 classy_imaginary-0.5.6/classy_imaginary/vendored/basicsr/rrdbnet_arch.py
--rw-r--r--   0        0        0        0 2023-01-01 18:59:37.474651 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/__init__.py
--rw-r--r--   0        0        0     9915 2023-03-19 16:14:08.290284 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/blip.py
--rw-r--r--   0        0        0     2838 2023-03-19 16:14:08.278283 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/blip_itm.py
--rw-r--r--   0        0        0     4082 2023-03-19 16:14:12.958366 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/blip_nlvr.py
--rw-r--r--   0        0        0    15525 2023-01-31 15:58:02.874557 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/blip_pretrain.py
--rw-r--r--   0        0        0    13191 2023-01-31 15:58:02.874557 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/blip_retrieval.py
--rw-r--r--   0        0        0     8040 2023-03-19 16:14:26.014596 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/blip_vqa.py
--rw-r--r--   0        0        0      485 2023-01-01 18:59:37.478651 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/configs/bert_config.json
--rw-r--r--   0        0        0      651 2023-01-01 18:59:37.478651 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/configs/caption_coco.yaml
--rw-r--r--   0        0        0      485 2023-01-01 18:59:37.478651 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/configs/med_config.json
--rw-r--r--   0        0        0      441 2023-01-01 18:59:37.478651 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/configs/nlvr.yaml
--rw-r--r--   0        0        0      352 2023-01-01 18:59:37.478651 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/configs/nocaps.yaml
--rw-r--r--   0        0        0      479 2023-01-01 18:59:37.478651 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/configs/pretrain.yaml
--rw-r--r--   0        0        0      655 2023-01-01 18:59:37.478651 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/configs/retrieval_coco.yaml
--rw-r--r--   0        0        0      658 2023-01-01 18:59:37.478651 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/configs/retrieval_flickr.yaml
--rw-r--r--   0        0        0      354 2023-01-01 18:59:37.478651 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/configs/retrieval_msrvtt.yaml
--rw-r--r--   0        0        0      639 2023-01-01 18:59:37.478651 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/configs/vqa.yaml
--rw-r--r--   0        0        0    42958 2023-03-19 16:14:34.590747 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/med.py
--rw-r--r--   0        0        0    37835 2023-03-19 16:14:34.570747 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/nlvr_encoder.py
--rw-r--r--   0        0        0    15645 2023-01-31 15:58:02.874557 classy_imaginary-0.5.6/classy_imaginary/vendored/blip/vit.py
--rw-r--r--   0        0        0       20 2023-01-01 18:59:37.478651 classy_imaginary-0.5.6/classy_imaginary/vendored/clip/__init__.py
--rw-r--r--   0        0        0  1356917 2023-01-01 18:59:37.482651 classy_imaginary-0.5.6/classy_imaginary/vendored/clip/bpe_simple_vocab_16e6.txt.gz
--rw-r--r--   0        0        0       41 2023-01-01 18:59:37.482651 classy_imaginary-0.5.6/classy_imaginary/vendored/clip/clip-commit-hash.txt
--rw-r--r--   0        0        0    10014 2023-01-31 15:58:02.874557 classy_imaginary-0.5.6/classy_imaginary/vendored/clip/clip.py
--rw-r--r--   0        0        0    18818 2023-01-31 15:58:02.874557 classy_imaginary-0.5.6/classy_imaginary/vendored/clip/model.py
--rw-r--r--   0        0        0       45 2023-01-01 18:59:37.482651 classy_imaginary-0.5.6/classy_imaginary/vendored/clip/readme.txt
--rw-r--r--   0        0        0     4847 2023-01-31 15:58:02.874557 classy_imaginary-0.5.6/classy_imaginary/vendored/clip/simple_tokenizer.py
--rw-r--r--   0        0        0        0 2023-01-01 18:59:37.482651 classy_imaginary-0.5.6/classy_imaginary/vendored/clip/version.py
--rwxr-xr-x   0        0        0    23543 2023-03-19 16:17:11.917519 classy_imaginary-0.5.6/classy_imaginary/vendored/clipseg/__init__.py
--rw-r--r--   0        0        0  4720707 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/clipseg/rd64-uni-refined.pth
--rw-r--r--   0        0        0        0 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/codeformer/__init__.py
--rw-r--r--   0        0        0    11250 2023-01-31 15:58:02.874557 classy_imaginary-0.5.6/classy_imaginary/vendored/codeformer/codeformer_arch.py
--rw-r--r--   0        0        0       93 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/codeformer/readme.txt
--rw-r--r--   0        0        0    16223 2023-01-31 15:58:02.874557 classy_imaginary-0.5.6/classy_imaginary/vendored/codeformer/vqgan_arch.py
--rw-r--r--   0        0        0     1061 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/LICENSE
--rw-r--r--   0        0        0        0 2023-01-31 15:58:02.874557 classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/__init__.py
--rw-r--r--   0        0        0     3728 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/augmentation.py
--rw-r--r--   0        0        0        0 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/config.py
--rw-r--r--   0        0        0        0 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/evaluation.py
--rw-r--r--   0        0        0     7279 2023-01-31 15:58:02.874557 classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/external.py
--rw-r--r--   0        0        0     4222 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/gns.py
--rw-r--r--   0        0        0     9529 2023-01-31 15:58:02.874557 classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/layers.py
--rw-r--r--   0        0        0        0 2023-01-31 15:58:02.874557 classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/models/__init__.py
--rw-r--r--   0        0        0    10250 2023-02-25 11:55:32.781366 classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/models/image_v1.py
--rw-r--r--   0        0        0       55 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/readme.txt
--rw-r--r--   0        0        0    30751 2023-03-25 16:05:32.735835 classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/sampling.py
--rw-r--r--   0        0        0       41 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/source-commit-hash.txt
--rw-r--r--   0        0        0    13415 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/utils.py
--rw-r--r--   0        0        0        0 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/version.py
--rw-r--r--   0        0        0      343 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/3d-term.txt.gz
--rw-r--r--   0        0        0     1072 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/LICENSE
--rw-r--r--   0        0        0      826 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/adj-architecture.txt.gz
--rw-r--r--   0        0        0      441 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/adj-beauty.txt.gz
--rw-r--r--   0        0        0      223 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/adj-detailed.txt.gz
--rw-r--r--   0        0        0      307 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/adj-emotion.txt.gz
--rw-r--r--   0        0        0     4854 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/adj-general.txt.gz
--rw-r--r--   0        0        0      262 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/adj-horror.txt.gz
--rw-r--r--   0        0        0     9976 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/animal.txt.gz
--rw-r--r--   0        0        0     1174 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/art-movement.txt.gz
--rw-r--r--   0        0        0      192 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/art-site.txt.gz
--rw-r--r--   0        0        0      368 2023-01-01 18:59:37.518652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/artist-botanical.txt.gz
--rw-r--r--   0        0        0      615 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/artist-surreal.txt.gz
--rw-r--r--   0        0        0    15701 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/artist.txt.gz
--rw-r--r--   0        0        0      148 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/aspect-ratio.txt.gz
--rw-r--r--   0        0        0     1593 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/bird.txt.gz
--rw-r--r--   0        0        0      366 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/body-of-water.txt.gz
--rw-r--r--   0        0        0      273 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/body-pose.txt.gz
--rw-r--r--   0        0        0       98 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/camera-brand.txt.gz
--rw-r--r--   0        0        0      580 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/camera-model.txt.gz
--rw-r--r--   0        0        0      393 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/cosmic-galaxy.txt.gz
--rw-r--r--   0        0        0      671 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/cosmic-nebula.txt.gz
--rw-r--r--   0        0        0      453 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/cosmic-star.txt.gz
--rw-r--r--   0        0        0      811 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/cosmic-term.txt.gz
--rw-r--r--   0        0        0     2561 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/dinosaur.txt.gz
--rw-r--r--   0        0        0      157 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/eyecolor.txt.gz
--rw-r--r--   0        0        0       67 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/f-stop.txt.gz
--rw-r--r--   0        0        0      211 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/fantasy-creature.txt.gz
--rw-r--r--   0        0        0      814 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/fantasy-setting.txt.gz
--rw-r--r--   0        0        0     5084 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/fish.txt.gz
--rw-r--r--   0        0        0     1580 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/flower.txt.gz
--rw-r--r--   0        0        0      149 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/focal-length.txt.gz
--rw-r--r--   0        0        0     1807 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/food.txt.gz
--rw-r--r--   0        0        0     1737 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/fruit.txt.gz
--rw-r--r--   0        0        0      460 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/gen-modifier.txt.gz
--rw-r--r--   0        0        0      206 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/hair.txt.gz
--rw-r--r--   0        0        0       88 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/hd.txt.gz
--rw-r--r--   0        0        0       86 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/iso-stop.txt.gz
--rw-r--r--   0        0        0      741 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/landscape-type.txt.gz
--rw-r--r--   0        0        0      504 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/national-park.txt.gz
--rw-r--r--   0        0        0     1107 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/nationality.txt.gz
--rw-r--r--   0        0        0      227 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/neg-weight.txt.gz
--rw-r--r--   0        0        0      413 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/noun-beauty.txt.gz
--rw-r--r--   0        0        0      617 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/noun-fantasy.txt.gz
--rw-r--r--   0        0        0     4665 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/noun-general.txt.gz
--rw-r--r--   0        0        0      548 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/noun-horror.txt.gz
--rw-r--r--   0        0        0      747 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/occupation.txt.gz
--rw-r--r--   0        0        0      106 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/photo-term.txt.gz
--rw-r--r--   0        0        0     1439 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/pop-culture.txt.gz
--rw-r--r--   0        0        0      776 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/pop-location.txt.gz
--rw-r--r--   0        0        0      148 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/punk-style.txt.gz
--rw-r--r--   0        0        0      102 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/quantity.txt.gz
--rw-r--r--   0        0        0     4015 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/rpg-Item.txt.gz
--rw-r--r--   0        0        0     1631 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/scenario-desc.txt.gz
--rw-r--r--   0        0        0      148 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/skin-color.txt.gz
--rw-r--r--   0        0        0      336 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/style.txt.gz
--rw-r--r--   0        0        0      357 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/tree-species.txt.gz
--rw-r--r--   0        0        0      458 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/trippy.txt.gz
--rw-r--r--   0        0        0     1183 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/video-game.txt.gz
--rw-r--r--   0        0        0    17465 2023-01-01 18:59:37.522652 classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/world-heritage-site.txt.gz
--rw-r--r--   0        0        0    12945 2023-03-19 16:12:18.612351 classy_imaginary-0.5.6/classy_imaginary/vendored/realesrgan.py
--rw-r--r--   0        0        0    13019 2023-01-31 15:58:02.874557 classy_imaginary-0.5.6/classy_imaginary/vendored/smart_crop.py
--rw-r--r--   0        0        0      184 2023-02-04 15:01:22.910016 classy_imaginary-0.5.6/classy_imaginary/version.py
--rw-r--r--   0        0        0     1166 2023-04-21 09:14:23.425749 classy_imaginary-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 classy_imaginary-0.5.6/setup.py
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 classy_imaginary-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1160 2023-01-01 18:59:37.438650 classy_imaginary-0.5.7/LICENSE
+-rw-r--r--   0        0        0       93 2023-01-02 15:20:36.641278 classy_imaginary-0.5.7/README.md
+-rw-r--r--   0        0        0     2043 2023-04-21 09:08:07.571186 classy_imaginary-0.5.7/classy_imaginary/Caption.py
+-rw-r--r--   0        0        0      626 2023-04-02 11:44:50.071771 classy_imaginary-0.5.7/classy_imaginary/FixFaces.py
+-rw-r--r--   0        0        0     4198 2023-03-19 16:37:49.495325 classy_imaginary-0.5.7/classy_imaginary/Imagine.py
+-rw-r--r--   0        0        0      672 2023-04-02 11:38:50.249560 classy_imaginary-0.5.7/classy_imaginary/Upscaler.py
+-rw-r--r--   0        0        0      286 2023-02-04 14:48:22.568510 classy_imaginary-0.5.7/classy_imaginary/__init__.py
+-rw-r--r--   0        0        0     3873 2023-03-19 16:33:37.082877 classy_imaginary-0.5.7/classy_imaginary/animations.py
+-rwxr-xr-x   0        0        0    28771 2023-04-02 11:44:50.095772 classy_imaginary-0.5.7/classy_imaginary/api.py
+-rw-r--r--   0        0        0      143 2023-03-19 15:49:53.552654 classy_imaginary-0.5.7/classy_imaginary/bin/aimg
+-rw-r--r--   0        0        0      153 2023-03-19 15:49:53.540653 classy_imaginary-0.5.7/classy_imaginary/bin/imagine
+-rw-r--r--   0        0        0        0 2023-03-18 11:53:39.545078 classy_imaginary-0.5.7/classy_imaginary/cli/__init__.py
+-rw-r--r--   0        0        0     1588 2023-03-19 15:50:31.837328 classy_imaginary-0.5.7/classy_imaginary/cli/colorize.py
+-rw-r--r--   0        0        0      674 2023-03-19 15:50:38.637448 classy_imaginary-0.5.7/classy_imaginary/cli/describe.py
+-rw-r--r--   0        0        0     3199 2023-03-19 15:51:05.949929 classy_imaginary-0.5.7/classy_imaginary/cli/edit.py
+-rw-r--r--   0        0        0      985 2023-03-19 15:51:17.810138 classy_imaginary-0.5.7/classy_imaginary/cli/edit_demo.py
+-rw-r--r--   0        0        0     3083 2023-03-19 15:51:24.066248 classy_imaginary-0.5.7/classy_imaginary/cli/imagine.py
+-rw-r--r--   0        0        0     2582 2023-03-19 15:51:44.050600 classy_imaginary-0.5.7/classy_imaginary/cli/main.py
+-rw-r--r--   0        0        0    15230 2023-03-19 15:52:44.039657 classy_imaginary-0.5.7/classy_imaginary/cli/shared.py
+-rw-r--r--   0        0        0     8197 2023-03-19 15:53:34.780551 classy_imaginary-0.5.7/classy_imaginary/cli/train.py
+-rw-r--r--   0        0        0     1627 2023-03-19 15:53:47.464774 classy_imaginary-0.5.7/classy_imaginary/cli/upscale.py
+-rw-r--r--   0        0        0     1385 2023-03-19 16:41:57.663698 classy_imaginary-0.5.7/classy_imaginary/colorize.py
+-rw-r--r--   0        0        0    13672 2023-04-29 16:52:07.373607 classy_imaginary-0.5.7/classy_imaginary/config.py
+-rw-r--r--   0        0        0     2036 2023-02-25 11:37:14.631990 classy_imaginary-0.5.7/classy_imaginary/configs/control-net-v15.yaml
+-rw-r--r--   0        0        0     1854 2023-04-29 16:42:42.135057 classy_imaginary-0.5.7/classy_imaginary/configs/graphicArt_graphicArtBeta.yaml
+-rw-r--r--   0        0        0     1855 2023-01-31 15:58:02.862557 classy_imaginary-0.5.7/classy_imaginary/configs/instruct-pix2pix.yaml
+-rw-r--r--   0        0        0     1854 2023-04-29 16:42:42.135057 classy_imaginary-0.5.7/classy_imaginary/configs/realismEngine_v10.yaml
+-rw-r--r--   0        0        0     2055 2023-01-02 12:25:06.421175 classy_imaginary-0.5.7/classy_imaginary/configs/stable-diffusion-v1-inpaint.yaml
+-rw-r--r--   0        0        0     1998 2023-01-31 15:58:02.862557 classy_imaginary-0.5.7/classy_imaginary/configs/stable-diffusion-v1.yaml
+-rw-r--r--   0        0        0     1855 2023-02-11 14:49:23.881155 classy_imaginary-0.5.7/classy_imaginary/configs/stable-diffusion-v2-inference-v.yaml
+-rw-r--r--   0        0        0     1829 2023-01-02 12:25:06.405175 classy_imaginary-0.5.7/classy_imaginary/configs/stable-diffusion-v2-inference.yaml
+-rw-r--r--   0        0        0     4489 2023-01-02 12:25:06.369174 classy_imaginary-0.5.7/classy_imaginary/configs/stable-diffusion-v2-inpainting-inference.yaml
+-rw-r--r--   0        0        0     1921 2023-01-02 12:25:06.489176 classy_imaginary-0.5.7/classy_imaginary/configs/stable-diffusion-v2-midas-inference.yaml
+-rw-r--r--   0        0        0     1835 2023-01-31 15:57:51.570357 classy_imaginary-0.5.7/classy_imaginary/configs/stable-diffusion-v2-modern-buildings.yaml
+-rw-r--r--   0        0        0     2265 2023-01-02 12:23:06.747039 classy_imaginary-0.5.7/classy_imaginary/configs/stable-diffusion-x4-upscaling.yaml
+-rw-r--r--   0        0        0   757076 2023-01-31 15:58:02.866557 classy_imaginary-0.5.7/classy_imaginary/data/DejaVuSans.ttf
+-rw-r--r--   0        0        0     1402 2023-03-19 16:50:17.952505 classy_imaginary-0.5.7/classy_imaginary/debug_info.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:59:37.466651 classy_imaginary-0.5.7/classy_imaginary/enhancers/__init__.py
+-rw-r--r--   0        0        0      444 2023-02-04 16:14:10.370494 classy_imaginary-0.5.7/classy_imaginary/enhancers/blur_detect.py
+-rw-r--r--   0        0        0     5114 2023-01-01 18:59:37.466651 classy_imaginary-0.5.7/classy_imaginary/enhancers/bool_masker.py
+-rw-r--r--   0        0        0     3157 2023-01-02 12:25:06.525177 classy_imaginary-0.5.7/classy_imaginary/enhancers/clip_masking.py
+-rw-r--r--   0        0        0     1838 2023-01-31 15:58:02.866557 classy_imaginary-0.5.7/classy_imaginary/enhancers/describe_image_blip.py
+-rw-r--r--   0        0        0     2071 2023-01-31 15:58:02.866557 classy_imaginary-0.5.7/classy_imaginary/enhancers/describe_image_clip.py
+-rw-r--r--   0        0        0     3376 2023-02-25 11:41:27.819950 classy_imaginary-0.5.7/classy_imaginary/enhancers/face_restoration_codeformer.py
+-rw-r--r--   0        0        0     1908 2023-02-04 16:14:10.362493 classy_imaginary-0.5.7/classy_imaginary/enhancers/facecrop.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:59:37.470651 classy_imaginary-0.5.7/classy_imaginary/enhancers/phraselists/__init__.py
+-rw-r--r--   0        0        0   169986 2023-03-18 11:53:39.549078 classy_imaginary-0.5.7/classy_imaginary/enhancers/phraselists/art-scene.txt
+-rw-r--r--   0        0        0      102 2023-01-01 18:59:37.470651 classy_imaginary-0.5.7/classy_imaginary/enhancers/phraselists/color.txt
+-rw-r--r--   0        0        0      249 2023-03-19 15:55:30.014581 classy_imaginary-0.5.7/classy_imaginary/enhancers/phraselists/desktop-background.txt
+-rw-r--r--   0        0        0      571 2023-03-18 11:53:39.549078 classy_imaginary-0.5.7/classy_imaginary/enhancers/phraselists/interior-style.txt
+-rw-r--r--   0        0        0      238 2023-03-18 11:53:39.549078 classy_imaginary-0.5.7/classy_imaginary/enhancers/phraselists/painting-style.txt
+-rw-r--r--   0        0        0      226 2023-01-01 18:59:37.470651 classy_imaginary-0.5.7/classy_imaginary/enhancers/phraselists/spaceship.txt
+-rw-r--r--   0        0        0     8941 2023-01-31 15:58:02.866557 classy_imaginary-0.5.7/classy_imaginary/enhancers/prompt_expansion.py
+-rw-r--r--   0        0        0     1133 2023-01-31 15:58:02.866557 classy_imaginary-0.5.7/classy_imaginary/enhancers/upscale_realesrgan.py
+-rw-r--r--   0        0        0    11254 2023-03-19 16:00:45.324136 classy_imaginary-0.5.7/classy_imaginary/enhancers/upscale_riverwing.py
+-rw-r--r--   0        0        0     6920 2023-03-19 16:50:17.960506 classy_imaginary-0.5.7/classy_imaginary/feather_tile.py
+-rw-r--r--   0        0        0        0 2023-02-25 11:33:31.076460 classy_imaginary-0.5.7/classy_imaginary/img_processors/__init__.py
+-rw-r--r--   0        0        0     4590 2023-02-25 13:14:32.287913 classy_imaginary-0.5.7/classy_imaginary/img_processors/control_modes.py
+-rw-r--r--   0        0        0     7312 2023-02-25 13:14:32.271913 classy_imaginary-0.5.7/classy_imaginary/img_processors/hed_boundary.py
+-rw-r--r--   0        0        0    29586 2023-03-19 16:02:08.369599 classy_imaginary-0.5.7/classy_imaginary/img_processors/openpose.py
+-rw-r--r--   0        0        0     5090 2023-02-25 13:27:31.053289 classy_imaginary-0.5.7/classy_imaginary/img_utils.py
+-rw-r--r--   0        0        0     9341 2023-02-25 12:30:37.397944 classy_imaginary-0.5.7/classy_imaginary/log_utils.py
+-rw-r--r--   0        0        0     4153 2023-01-31 15:58:02.866557 classy_imaginary-0.5.7/classy_imaginary/lr_scheduler.py
+-rw-r--r--   0        0        0    15329 2023-03-19 16:50:17.940505 classy_imaginary-0.5.7/classy_imaginary/model_manager.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:59:37.470651 classy_imaginary-0.5.7/classy_imaginary/modules/__init__.py
+-rw-r--r--   0        0        0    16627 2023-03-25 10:32:03.625304 classy_imaginary-0.5.7/classy_imaginary/modules/attention.py
+-rw-r--r--   0        0        0    23309 2023-03-19 16:04:52.700495 classy_imaginary-0.5.7/classy_imaginary/modules/autoencoder.py
+-rw-r--r--   0        0        0    20318 2023-03-19 16:05:30.533161 classy_imaginary-0.5.7/classy_imaginary/modules/cldm.py
+-rw-r--r--   0        0        0     3651 2023-01-31 15:58:02.866557 classy_imaginary-0.5.7/classy_imaginary/modules/clip_embedders.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:59:37.470651 classy_imaginary-0.5.7/classy_imaginary/modules/diffusion/__init__.py
+-rw-r--r--   0        0        0    81030 2023-03-19 16:07:16.747033 classy_imaginary-0.5.7/classy_imaginary/modules/diffusion/ddpm.py
+-rw-r--r--   0        0        0    34779 2023-03-25 10:31:46.085010 classy_imaginary-0.5.7/classy_imaginary/modules/diffusion/model.py
+-rw-r--r--   0        0        0    31716 2023-01-31 15:58:02.870557 classy_imaginary-0.5.7/classy_imaginary/modules/diffusion/openaimodel.py
+-rw-r--r--   0        0        0     3599 2023-01-02 12:23:06.791039 classy_imaginary-0.5.7/classy_imaginary/modules/diffusion/upscaling.py
+-rw-r--r--   0        0        0     9799 2023-02-25 11:53:22.130967 classy_imaginary-0.5.7/classy_imaginary/modules/diffusion/util.py
+-rw-r--r--   0        0        0     1651 2023-01-01 18:59:37.474651 classy_imaginary-0.5.7/classy_imaginary/modules/distributions.py
+-rw-r--r--   0        0        0     3290 2023-01-01 18:59:37.474651 classy_imaginary-0.5.7/classy_imaginary/modules/ema.py
+-rw-r--r--   0        0        0     8089 2023-01-31 15:58:02.870557 classy_imaginary-0.5.7/classy_imaginary/modules/encoders.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:59:37.474651 classy_imaginary-0.5.7/classy_imaginary/modules/midas/__init__.py
+-rw-r--r--   0        0        0     6606 2023-02-25 11:53:22.102967 classy_imaginary-0.5.7/classy_imaginary/modules/midas/api.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:59:37.474651 classy_imaginary-0.5.7/classy_imaginary/modules/midas/midas/__init__.py
+-rw-r--r--   0        0        0      567 2023-01-31 15:58:02.870557 classy_imaginary-0.5.7/classy_imaginary/modules/midas/midas/base_model.py
+-rw-r--r--   0        0        0     9817 2023-01-01 18:59:37.474651 classy_imaginary-0.5.7/classy_imaginary/modules/midas/midas/blocks.py
+-rw-r--r--   0        0        0     3082 2023-03-19 16:07:16.759033 classy_imaginary-0.5.7/classy_imaginary/modules/midas/midas/dpt_depth.py
+-rw-r--r--   0        0        0     2716 2023-01-31 15:58:02.870557 classy_imaginary-0.5.7/classy_imaginary/modules/midas/midas/midas_net.py
+-rw-r--r--   0        0        0     5885 2023-01-31 15:58:02.870557 classy_imaginary-0.5.7/classy_imaginary/modules/midas/midas/midas_net_custom.py
+-rw-r--r--   0        0        0     7845 2023-01-01 18:59:37.474651 classy_imaginary-0.5.7/classy_imaginary/modules/midas/midas/transforms.py
+-rw-r--r--   0        0        0    14588 2023-01-31 15:58:02.870557 classy_imaginary-0.5.7/classy_imaginary/modules/midas/midas/vit.py
+-rw-r--r--   0        0        0     5058 2023-02-25 11:53:22.078966 classy_imaginary-0.5.7/classy_imaginary/modules/midas/utils.py
+-rw-r--r--   0        0        0     7679 2023-02-25 12:35:44.323298 classy_imaginary-0.5.7/classy_imaginary/outpaint.py
+-rw-r--r--   0        0        0       53 2023-01-01 18:59:37.474651 classy_imaginary-0.5.7/classy_imaginary/paths.py
+-rw-r--r--   0        0        0     2279 2023-01-31 15:58:02.870557 classy_imaginary-0.5.7/classy_imaginary/prompt_schedules.py
+-rw-r--r--   0        0        0     3371 2023-01-31 15:58:02.870557 classy_imaginary-0.5.7/classy_imaginary/roi_utils.py
+-rw-r--r--   0        0        0     5945 2023-02-04 14:58:22.938902 classy_imaginary-0.5.7/classy_imaginary/safety.py
+-rw-r--r--   0        0        0      681 2023-01-02 12:25:06.565178 classy_imaginary-0.5.7/classy_imaginary/samplers/__init__.py
+-rw-r--r--   0        0        0     5957 2023-01-02 12:23:07.087045 classy_imaginary-0.5.7/classy_imaginary/samplers/base.py
+-rw-r--r--   0        0        0     7277 2023-03-19 16:09:15.349122 classy_imaginary-0.5.7/classy_imaginary/samplers/ddim.py
+-rw-r--r--   0        0        0     1974 2023-02-04 16:14:10.354493 classy_imaginary-0.5.7/classy_imaginary/samplers/editing.py
+-rw-r--r--   0        0        0     7989 2023-03-19 16:09:45.945661 classy_imaginary-0.5.7/classy_imaginary/samplers/kdiff.py
+-rw-r--r--   0        0        0     8444 2023-03-19 16:10:47.082738 classy_imaginary-0.5.7/classy_imaginary/samplers/plms.py
+-rw-r--r--   0        0        0    13620 2023-03-19 16:50:17.916505 classy_imaginary-0.5.7/classy_imaginary/schema.py
+-rw-r--r--   0        0        0     7368 2023-01-31 15:58:02.870557 classy_imaginary-0.5.7/classy_imaginary/surprise_me.py
+-rw-r--r--   0        0        0    18313 2023-03-19 16:52:01.450327 classy_imaginary-0.5.7/classy_imaginary/train.py
+-rw-r--r--   0        0        0        0 2023-01-31 15:58:02.870557 classy_imaginary-0.5.7/classy_imaginary/training_tools/__init__.py
+-rw-r--r--   0        0        0     6197 2023-03-19 16:11:55.303940 classy_imaginary-0.5.7/classy_imaginary/training_tools/image_prep.py
+-rw-r--r--   0        0        0     1061 2023-01-31 15:58:02.870557 classy_imaginary-0.5.7/classy_imaginary/training_tools/prune_model.py
+-rw-r--r--   0        0        0     4311 2023-01-31 15:58:02.870557 classy_imaginary-0.5.7/classy_imaginary/training_tools/single_concept.py
+-rw-r--r--   0        0        0     5757 2023-03-19 16:52:01.470327 classy_imaginary-0.5.7/classy_imaginary/utils.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:59:37.474651 classy_imaginary-0.5.7/classy_imaginary/vendored/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-19 17:05:50.960915 classy_imaginary-0.5.7/classy_imaginary/vendored/basicsr/__init__.py
+-rw-r--r--   0        0        0     2526 2023-03-19 17:05:59.969074 classy_imaginary-0.5.7/classy_imaginary/vendored/basicsr/arch_util.py
+-rw-r--r--   0        0        0     6458 2023-01-31 15:58:02.870557 classy_imaginary-0.5.7/classy_imaginary/vendored/basicsr/img_util.py
+-rw-r--r--   0        0        0     4723 2023-01-31 15:58:02.870557 classy_imaginary-0.5.7/classy_imaginary/vendored/basicsr/rrdbnet_arch.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:59:37.474651 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/__init__.py
+-rw-r--r--   0        0        0     9915 2023-03-19 16:14:08.290284 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/blip.py
+-rw-r--r--   0        0        0     2838 2023-03-19 16:14:08.278283 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/blip_itm.py
+-rw-r--r--   0        0        0     4082 2023-03-19 16:14:12.958366 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/blip_nlvr.py
+-rw-r--r--   0        0        0    15525 2023-01-31 15:58:02.874557 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/blip_pretrain.py
+-rw-r--r--   0        0        0    13191 2023-01-31 15:58:02.874557 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/blip_retrieval.py
+-rw-r--r--   0        0        0     8040 2023-03-19 16:14:26.014596 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/blip_vqa.py
+-rw-r--r--   0        0        0      485 2023-01-01 18:59:37.478651 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/configs/bert_config.json
+-rw-r--r--   0        0        0      651 2023-01-01 18:59:37.478651 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/configs/caption_coco.yaml
+-rw-r--r--   0        0        0      485 2023-01-01 18:59:37.478651 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/configs/med_config.json
+-rw-r--r--   0        0        0      441 2023-01-01 18:59:37.478651 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/configs/nlvr.yaml
+-rw-r--r--   0        0        0      352 2023-01-01 18:59:37.478651 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/configs/nocaps.yaml
+-rw-r--r--   0        0        0      479 2023-01-01 18:59:37.478651 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/configs/pretrain.yaml
+-rw-r--r--   0        0        0      655 2023-01-01 18:59:37.478651 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/configs/retrieval_coco.yaml
+-rw-r--r--   0        0        0      658 2023-01-01 18:59:37.478651 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/configs/retrieval_flickr.yaml
+-rw-r--r--   0        0        0      354 2023-01-01 18:59:37.478651 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/configs/retrieval_msrvtt.yaml
+-rw-r--r--   0        0        0      639 2023-01-01 18:59:37.478651 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/configs/vqa.yaml
+-rw-r--r--   0        0        0    42958 2023-03-19 16:14:34.590747 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/med.py
+-rw-r--r--   0        0        0    37835 2023-03-19 16:14:34.570747 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/nlvr_encoder.py
+-rw-r--r--   0        0        0    15645 2023-01-31 15:58:02.874557 classy_imaginary-0.5.7/classy_imaginary/vendored/blip/vit.py
+-rw-r--r--   0        0        0       20 2023-01-01 18:59:37.478651 classy_imaginary-0.5.7/classy_imaginary/vendored/clip/__init__.py
+-rw-r--r--   0        0        0  1356917 2023-01-01 18:59:37.482651 classy_imaginary-0.5.7/classy_imaginary/vendored/clip/bpe_simple_vocab_16e6.txt.gz
+-rw-r--r--   0        0        0       41 2023-01-01 18:59:37.482651 classy_imaginary-0.5.7/classy_imaginary/vendored/clip/clip-commit-hash.txt
+-rw-r--r--   0        0        0    10014 2023-01-31 15:58:02.874557 classy_imaginary-0.5.7/classy_imaginary/vendored/clip/clip.py
+-rw-r--r--   0        0        0    18818 2023-01-31 15:58:02.874557 classy_imaginary-0.5.7/classy_imaginary/vendored/clip/model.py
+-rw-r--r--   0        0        0       45 2023-01-01 18:59:37.482651 classy_imaginary-0.5.7/classy_imaginary/vendored/clip/readme.txt
+-rw-r--r--   0        0        0     4847 2023-01-31 15:58:02.874557 classy_imaginary-0.5.7/classy_imaginary/vendored/clip/simple_tokenizer.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:59:37.482651 classy_imaginary-0.5.7/classy_imaginary/vendored/clip/version.py
+-rwxr-xr-x   0        0        0    23543 2023-03-19 16:17:11.917519 classy_imaginary-0.5.7/classy_imaginary/vendored/clipseg/__init__.py
+-rw-r--r--   0        0        0  4720707 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/clipseg/rd64-uni-refined.pth
+-rw-r--r--   0        0        0        0 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/codeformer/__init__.py
+-rw-r--r--   0        0        0    11250 2023-01-31 15:58:02.874557 classy_imaginary-0.5.7/classy_imaginary/vendored/codeformer/codeformer_arch.py
+-rw-r--r--   0        0        0       93 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/codeformer/readme.txt
+-rw-r--r--   0        0        0    16223 2023-01-31 15:58:02.874557 classy_imaginary-0.5.7/classy_imaginary/vendored/codeformer/vqgan_arch.py
+-rw-r--r--   0        0        0     1061 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/LICENSE
+-rw-r--r--   0        0        0        0 2023-01-31 15:58:02.874557 classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/__init__.py
+-rw-r--r--   0        0        0     3728 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/augmentation.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/config.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/evaluation.py
+-rw-r--r--   0        0        0     7279 2023-01-31 15:58:02.874557 classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/external.py
+-rw-r--r--   0        0        0     4222 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/gns.py
+-rw-r--r--   0        0        0     9529 2023-01-31 15:58:02.874557 classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/layers.py
+-rw-r--r--   0        0        0        0 2023-01-31 15:58:02.874557 classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/models/__init__.py
+-rw-r--r--   0        0        0    10250 2023-02-25 11:55:32.781366 classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/models/image_v1.py
+-rw-r--r--   0        0        0       55 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/readme.txt
+-rw-r--r--   0        0        0    30751 2023-03-25 16:05:32.735835 classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/sampling.py
+-rw-r--r--   0        0        0       41 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/source-commit-hash.txt
+-rw-r--r--   0        0        0    13415 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/utils.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/version.py
+-rw-r--r--   0        0        0      343 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/3d-term.txt.gz
+-rw-r--r--   0        0        0     1072 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/LICENSE
+-rw-r--r--   0        0        0      826 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/adj-architecture.txt.gz
+-rw-r--r--   0        0        0      441 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/adj-beauty.txt.gz
+-rw-r--r--   0        0        0      223 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/adj-detailed.txt.gz
+-rw-r--r--   0        0        0      307 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/adj-emotion.txt.gz
+-rw-r--r--   0        0        0     4854 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/adj-general.txt.gz
+-rw-r--r--   0        0        0      262 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/adj-horror.txt.gz
+-rw-r--r--   0        0        0     9976 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/animal.txt.gz
+-rw-r--r--   0        0        0     1174 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/art-movement.txt.gz
+-rw-r--r--   0        0        0      192 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/art-site.txt.gz
+-rw-r--r--   0        0        0      368 2023-01-01 18:59:37.518652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/artist-botanical.txt.gz
+-rw-r--r--   0        0        0      615 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/artist-surreal.txt.gz
+-rw-r--r--   0        0        0    15701 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/artist.txt.gz
+-rw-r--r--   0        0        0      148 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/aspect-ratio.txt.gz
+-rw-r--r--   0        0        0     1593 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/bird.txt.gz
+-rw-r--r--   0        0        0      366 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/body-of-water.txt.gz
+-rw-r--r--   0        0        0      273 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/body-pose.txt.gz
+-rw-r--r--   0        0        0       98 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/camera-brand.txt.gz
+-rw-r--r--   0        0        0      580 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/camera-model.txt.gz
+-rw-r--r--   0        0        0      393 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/cosmic-galaxy.txt.gz
+-rw-r--r--   0        0        0      671 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/cosmic-nebula.txt.gz
+-rw-r--r--   0        0        0      453 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/cosmic-star.txt.gz
+-rw-r--r--   0        0        0      811 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/cosmic-term.txt.gz
+-rw-r--r--   0        0        0     2561 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/dinosaur.txt.gz
+-rw-r--r--   0        0        0      157 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/eyecolor.txt.gz
+-rw-r--r--   0        0        0       67 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/f-stop.txt.gz
+-rw-r--r--   0        0        0      211 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/fantasy-creature.txt.gz
+-rw-r--r--   0        0        0      814 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/fantasy-setting.txt.gz
+-rw-r--r--   0        0        0     5084 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/fish.txt.gz
+-rw-r--r--   0        0        0     1580 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/flower.txt.gz
+-rw-r--r--   0        0        0      149 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/focal-length.txt.gz
+-rw-r--r--   0        0        0     1807 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/food.txt.gz
+-rw-r--r--   0        0        0     1737 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/fruit.txt.gz
+-rw-r--r--   0        0        0      460 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/gen-modifier.txt.gz
+-rw-r--r--   0        0        0      206 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/hair.txt.gz
+-rw-r--r--   0        0        0       88 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/hd.txt.gz
+-rw-r--r--   0        0        0       86 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/iso-stop.txt.gz
+-rw-r--r--   0        0        0      741 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/landscape-type.txt.gz
+-rw-r--r--   0        0        0      504 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/national-park.txt.gz
+-rw-r--r--   0        0        0     1107 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/nationality.txt.gz
+-rw-r--r--   0        0        0      227 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/neg-weight.txt.gz
+-rw-r--r--   0        0        0      413 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/noun-beauty.txt.gz
+-rw-r--r--   0        0        0      617 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/noun-fantasy.txt.gz
+-rw-r--r--   0        0        0     4665 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/noun-general.txt.gz
+-rw-r--r--   0        0        0      548 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/noun-horror.txt.gz
+-rw-r--r--   0        0        0      747 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/occupation.txt.gz
+-rw-r--r--   0        0        0      106 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/photo-term.txt.gz
+-rw-r--r--   0        0        0     1439 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/pop-culture.txt.gz
+-rw-r--r--   0        0        0      776 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/pop-location.txt.gz
+-rw-r--r--   0        0        0      148 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/punk-style.txt.gz
+-rw-r--r--   0        0        0      102 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/quantity.txt.gz
+-rw-r--r--   0        0        0     4015 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/rpg-Item.txt.gz
+-rw-r--r--   0        0        0     1631 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/scenario-desc.txt.gz
+-rw-r--r--   0        0        0      148 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/skin-color.txt.gz
+-rw-r--r--   0        0        0      336 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/style.txt.gz
+-rw-r--r--   0        0        0      357 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/tree-species.txt.gz
+-rw-r--r--   0        0        0      458 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/trippy.txt.gz
+-rw-r--r--   0        0        0     1183 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/video-game.txt.gz
+-rw-r--r--   0        0        0    17465 2023-01-01 18:59:37.522652 classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/world-heritage-site.txt.gz
+-rw-r--r--   0        0        0    12945 2023-03-19 16:12:18.612351 classy_imaginary-0.5.7/classy_imaginary/vendored/realesrgan.py
+-rw-r--r--   0        0        0    13019 2023-01-31 15:58:02.874557 classy_imaginary-0.5.7/classy_imaginary/vendored/smart_crop.py
+-rw-r--r--   0        0        0      184 2023-02-04 15:01:22.910016 classy_imaginary-0.5.7/classy_imaginary/version.py
+-rw-r--r--   0        0        0     1166 2023-04-29 16:52:42.618265 classy_imaginary-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 classy_imaginary-0.5.7/setup.py
+-rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 classy_imaginary-0.5.7/PKG-INFO
```

### Comparing `classy_imaginary-0.5.6/LICENSE` & `classy_imaginary-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/Caption.py` & `classy_imaginary-0.5.7/classy_imaginary/Caption.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/FixFaces.py` & `classy_imaginary-0.5.7/classy_imaginary/FixFaces.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/Imagine.py` & `classy_imaginary-0.5.7/classy_imaginary/Imagine.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/Upscaler.py` & `classy_imaginary-0.5.7/classy_imaginary/Upscaler.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/animations.py` & `classy_imaginary-0.5.7/classy_imaginary/animations.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/api.py` & `classy_imaginary-0.5.7/classy_imaginary/api.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/cli/colorize.py` & `classy_imaginary-0.5.7/classy_imaginary/cli/colorize.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/cli/describe.py` & `classy_imaginary-0.5.7/classy_imaginary/cli/describe.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/cli/edit.py` & `classy_imaginary-0.5.7/classy_imaginary/cli/edit.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/cli/edit_demo.py` & `classy_imaginary-0.5.7/classy_imaginary/cli/edit_demo.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/cli/imagine.py` & `classy_imaginary-0.5.7/classy_imaginary/cli/imagine.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/cli/main.py` & `classy_imaginary-0.5.7/classy_imaginary/cli/main.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/cli/shared.py` & `classy_imaginary-0.5.7/classy_imaginary/cli/shared.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/cli/train.py` & `classy_imaginary-0.5.7/classy_imaginary/cli/train.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/cli/upscale.py` & `classy_imaginary-0.5.7/classy_imaginary/cli/upscale.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/colorize.py` & `classy_imaginary-0.5.7/classy_imaginary/colorize.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/config.py` & `classy_imaginary-0.5.7/classy_imaginary/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,23 +131,14 @@
         weights_url="https://huggingface.co/imaginairy/instruct-pix2pix/resolve/ea0009b3d0d4888f410a40bd06d69516d0b5a577/instruct-pix2pix-00-22000-pruned.ckpt",
         default_image_size=512,
         default_negative_prompt="",
         alias="edit",
     ),
     # --- Custom model --#
     ModelConfig(
-        description="OpenJourney V1",
-        short_name="openjourney-v1",
-        config_path="configs/stable-diffusion-v1.yaml",
-        weights_url="https://huggingface.co/prompthero/openjourney/resolve/7428477dad893424c92f6ea1cc29d45f6d1448c1/mdjrny-v4.safetensors",
-        default_image_size=512,
-        default_negative_prompt="",
-        alias="oj1",
-    ),
-    ModelConfig(
         description="OpenJourney V2",
         short_name="openjourney-v2",
         config_path="configs/stable-diffusion-v1.yaml",
         weights_url="https://huggingface.co/prompthero/openjourney-v2/resolve/47257274a40e93dab7fbc0cd2cfd5f5704cfeb60/openjourney-v2.ckpt",
         default_image_size=512,
         default_negative_prompt="",
         alias="oj2",
@@ -157,105 +148,97 @@
         short_name="MidJourney-PaperCut",
         config_path="configs/stable-diffusion-v1.yaml",
         weights_url="https://huggingface.co/ShadoWxShinigamI/MidJourney-PaperCut/resolve/main/Mdjrny-pprct_step_7000.ckpt",
         default_image_size=512,
         alias="mjpc"
     ),
     ModelConfig(
-        description="OpenJourney",
-        short_name="Openjourney",
+        description="Synthwave Punk",
+        short_name="SynthwavePunk",
         config_path="configs/stable-diffusion-v1.yaml",
-        # config_path="configs/stable-diffusion-v2-inference-v.yaml",
-        # weights_url="https://civitai.com/api/download/models/96",
-        weights_url="https://huggingface.co/prompthero/openjourney-v2/resolve/main/openjourney-v2-unpruned.ckpt",
+        weights_url="https://huggingface.co/zipp425/synthwavePunk/resolve/main/synthwavePunk_v2.ckpt",
         default_image_size=512,
-        alias="ojc"
     ),
     ModelConfig(
-        description="Protogen Anime",
-        short_name="Protogen-Anime",
-        config_path="configs/stable-diffusion-v1.yaml",
-        weights_url="https://civitai.com/api/download/models/4007",
-        default_image_size=512,
-        alias="proa"
+        description="Graphic Art",
+        short_name="graphic-art",
+        config_path="configs/graphicArt_graphicArtBeta.yaml",
+        weights_url="https://fakewebsite.com/models/graphicArt_graphicArtBeta11.safetensors",
+        default_image_size=768,
     ),
     ModelConfig(
-        description="Protogen Photo",
-        short_name="Protogen-Photo",
+        description="Realism Engine",
+        short_name="realism-engine",
+        config_path="configs/realismEngine_v10.yaml",
+        weights_url="https://fakewebsite.com/models/realismEngine_v10.safetensors",
+        default_image_size=768,
+    ),
+    ModelConfig(
+        description="Counterfeit V30",
+        short_name="counterfeit",
         config_path="configs/stable-diffusion-v1.yaml",
-        weights_url="https://huggingface.co/darkstorm2150/Protogen_x3.4_Official_Release/resolve/main/ProtoGen_X3.4.ckpt",
+        weights_url="https://fakewebsite.com/models/CounterfeitV30_v30.safetensors",
         default_image_size=512,
-        alias="prop"
     ),
     ModelConfig(
-        description="Protogen Photo V2",
-        short_name="Protogen-PhotoV2",
+        description="Counterfeit V30",
+        short_name="counterfeit",
         config_path="configs/stable-diffusion-v1.yaml",
-        weights_url="https://huggingface.co/darkstorm2150/Protogen_v5.3_Official_Release/resolve/main/ProtoGen_X5.3.ckpt",
+        weights_url="https://fakewebsite.com/models/CounterfeitV30_v30.safetensors",
         default_image_size=512,
-        alias="prop2"
     ),
     ModelConfig(
-        description="Role Playing Game",
-        short_name="RPG",
+        description="Deliberate",
+        short_name="deliberate",
         config_path="configs/stable-diffusion-v1.yaml",
-        weights_url="https://huggingface.co/Anashel/rpg/resolve/main/RPG-V4-Model-Download/RPG-v4.safetensors",
+        weights_url="https://fakewebsite.com/models/eliberate_v2.safetensors",
         default_image_size=512,
-        alias="rpg"
     ),
     ModelConfig(
-        description="Synthwave Punk",
-        short_name="SynthwavePunk",
-        config_path="configs/stable-diffusion-v1.yaml",
-        weights_url="https://huggingface.co/zipp425/synthwavePunk/resolve/main/synthwavePunk_v2.ckpt",
+        description="Deliberate Inpainting",
+        short_name="deliberate-inpainting",
+        config_path="configs/stable-diffusion-v1-inpaint.yaml",
+        weights_url="https://fakewebsite.com/models/Deliberate-inpainting.safetensors",
         default_image_size=512,
     ),
     ModelConfig(
-        description="Modern Disney",
-        short_name="ModernDisney",
+        description="Dreamshaper",
+        short_name="dreamshaper",
         config_path="configs/stable-diffusion-v1.yaml",
-        weights_url="https://huggingface.co/nitrosocke/mo-di-diffusion/resolve/main/moDi-v1-pruned.ckpt",
+        weights_url="https://fakewebsite.com/models/dreamshaper_5BakedVae.safetensors",
         default_image_size=512,
     ),
     ModelConfig(
-        description="Art Diffusion",
-        short_name="Art-Diffusion",
+        description="Dreamshaper",
+        short_name="dreamshaper",
         config_path="configs/stable-diffusion-v1.yaml",
-        weights_url="https://huggingface.co/DGSpitzer/DGSpitzer-Art-Diffusion/resolve/main/DGSpitzer-Art-Diffusion.ckpt",
+        weights_url="https://fakewebsite.com/models/dreamshaper_5BakedVae.safetensors",
         default_image_size=512,
     ),
     ModelConfig(
-        description="Graphic Art",
-        short_name="graphic-art",
-        config_path="configs/graphicArt_graphicArtBeta.yaml",
-        weights_url="https://civitai.com/api/download/models/9297?type=Model&format=PickleTensor",
-        default_image_size=768,
+        description="Neurogen",
+        short_name="neurogen",
+        config_path="configs/stable-diffusion-v1.yaml",
+        weights_url="https://fakewebsite.com/models/neurogenV11_v11.safetensors",
+        default_image_size=512,
     ),
     ModelConfig(
-        description="DreamLike Humans",
-        short_name="DreamLikeHumans",
+        description="Neverending Dream",
+        short_name="neverending-dream",
         config_path="configs/stable-diffusion-v1.yaml",
-        weights_url="https://huggingface.co/dreamlike-art/dreamlike-photoreal-2.0/resolve/main/dreamlike-photoreal-2.0.ckpt",
+        weights_url="https://fakewebsite.com/models/neverendingDreamNED_bakedVae.safetensors",
         default_image_size=512,
-        alias="dlh"
     ),
     ModelConfig(
-        description="DreamLike Diffusion",
-        short_name="DreamLikeDiffusion",
+        description="Realistic Vision",
+        short_name="realistic-vision",
         config_path="configs/stable-diffusion-v1.yaml",
-        weights_url="https://huggingface.co/dreamlike-art/dreamlike-diffusion-1.0/resolve/main/dreamlike-diffusion-1.0.ckpt",
-        default_image_size=640,
-        alias="dld"
+        weights_url="https://fakewebsite.com/models/realisticVisionV20_v20.safetensors",
+        default_image_size=512,
     ),
-    # ModelConfig(
-    #     short_name="SD-2.0-upscale",
-    #     config_path="configs/stable-diffusion-v2-upscaling.yaml",
-    #     weights_url="https://huggingface.co/stabilityai/stable-diffusion-x4-upscaler/resolve/main/x4-upscaler-ema.ckpt",
-    #     default_image_size=512,
-    # ),
 ]
 
 MODEL_CONFIG_SHORTCUTS = {m.short_name: m for m in MODEL_CONFIGS}
 for m in MODEL_CONFIGS:
     if m.alias:
         MODEL_CONFIG_SHORTCUTS[m.alias] = m
```

### Comparing `classy_imaginary-0.5.6/classy_imaginary/configs/control-net-v15.yaml` & `classy_imaginary-0.5.7/classy_imaginary/configs/control-net-v15.yaml`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/configs/graphicArt_graphicArtBeta.yaml` & `classy_imaginary-0.5.7/classy_imaginary/configs/stable-diffusion-v2-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/configs/instruct-pix2pix.yaml` & `classy_imaginary-0.5.7/classy_imaginary/configs/instruct-pix2pix.yaml`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/configs/stable-diffusion-v1-inpaint.yaml` & `classy_imaginary-0.5.7/classy_imaginary/configs/stable-diffusion-v1-inpaint.yaml`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/configs/stable-diffusion-v1.yaml` & `classy_imaginary-0.5.7/classy_imaginary/configs/stable-diffusion-v1.yaml`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/configs/stable-diffusion-v2-inference-v.yaml` & `classy_imaginary-0.5.7/classy_imaginary/configs/graphicArt_graphicArtBeta.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     scale_factor: 0.18215
     use_ema: False # we set this to false because this is an inference only config
 
     unet_config:
       target: classy_imaginary.modules.diffusion.openaimodel.UNetModel
       params:
         use_checkpoint: True
-        use_fp16: False
+        use_fp16: True
         image_size: 32 # unused
         in_channels: 4
         out_channels: 4
         model_channels: 320
         attention_resolutions: [ 4, 2, 1 ]
         num_res_blocks: 2
         channel_mult: [ 1, 2, 4, 4 ]
```

### Comparing `classy_imaginary-0.5.6/classy_imaginary/configs/stable-diffusion-v2-inference.yaml` & `classy_imaginary-0.5.7/classy_imaginary/configs/stable-diffusion-v2-inference.yaml`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/configs/stable-diffusion-v2-inpainting-inference.yaml` & `classy_imaginary-0.5.7/classy_imaginary/configs/stable-diffusion-v2-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/configs/stable-diffusion-v2-midas-inference.yaml` & `classy_imaginary-0.5.7/classy_imaginary/configs/stable-diffusion-v2-midas-inference.yaml`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/configs/stable-diffusion-v2-modern-buildings.yaml` & `classy_imaginary-0.5.7/classy_imaginary/configs/stable-diffusion-v2-modern-buildings.yaml`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/configs/stable-diffusion-x4-upscaling.yaml` & `classy_imaginary-0.5.7/classy_imaginary/configs/stable-diffusion-x4-upscaling.yaml`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/data/DejaVuSans.ttf` & `classy_imaginary-0.5.7/classy_imaginary/data/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/debug_info.py` & `classy_imaginary-0.5.7/classy_imaginary/debug_info.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/enhancers/bool_masker.py` & `classy_imaginary-0.5.7/classy_imaginary/enhancers/bool_masker.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/enhancers/clip_masking.py` & `classy_imaginary-0.5.7/classy_imaginary/enhancers/clip_masking.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/enhancers/describe_image_blip.py` & `classy_imaginary-0.5.7/classy_imaginary/enhancers/describe_image_blip.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/enhancers/describe_image_clip.py` & `classy_imaginary-0.5.7/classy_imaginary/enhancers/describe_image_clip.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/enhancers/face_restoration_codeformer.py` & `classy_imaginary-0.5.7/classy_imaginary/enhancers/face_restoration_codeformer.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/enhancers/facecrop.py` & `classy_imaginary-0.5.7/classy_imaginary/enhancers/facecrop.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/enhancers/phraselists/art-scene.txt` & `classy_imaginary-0.5.7/classy_imaginary/enhancers/phraselists/art-scene.txt`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/enhancers/phraselists/interior-style.txt` & `classy_imaginary-0.5.7/classy_imaginary/enhancers/phraselists/interior-style.txt`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/enhancers/prompt_expansion.py` & `classy_imaginary-0.5.7/classy_imaginary/enhancers/prompt_expansion.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/enhancers/upscale_realesrgan.py` & `classy_imaginary-0.5.7/classy_imaginary/enhancers/upscale_realesrgan.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/enhancers/upscale_riverwing.py` & `classy_imaginary-0.5.7/classy_imaginary/enhancers/upscale_riverwing.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/feather_tile.py` & `classy_imaginary-0.5.7/classy_imaginary/feather_tile.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/img_processors/control_modes.py` & `classy_imaginary-0.5.7/classy_imaginary/img_processors/control_modes.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/img_processors/hed_boundary.py` & `classy_imaginary-0.5.7/classy_imaginary/img_processors/hed_boundary.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/img_processors/openpose.py` & `classy_imaginary-0.5.7/classy_imaginary/img_processors/openpose.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/img_utils.py` & `classy_imaginary-0.5.7/classy_imaginary/img_utils.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/log_utils.py` & `classy_imaginary-0.5.7/classy_imaginary/log_utils.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/lr_scheduler.py` & `classy_imaginary-0.5.7/classy_imaginary/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/model_manager.py` & `classy_imaginary-0.5.7/classy_imaginary/model_manager.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/attention.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/attention.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/autoencoder.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/autoencoder.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/cldm.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/cldm.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/clip_embedders.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/clip_embedders.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/diffusion/ddpm.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/diffusion/ddpm.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/diffusion/model.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/diffusion/model.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/diffusion/openaimodel.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/diffusion/openaimodel.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/diffusion/upscaling.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/diffusion/upscaling.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/diffusion/util.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/diffusion/util.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/distributions.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/distributions.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/ema.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/ema.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/encoders.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/midas/api.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/midas/api.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/midas/midas/base_model.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/midas/midas/base_model.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/midas/midas/blocks.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/midas/midas/dpt_depth.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/midas/midas/midas_net.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/midas/midas/midas_net_custom.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/midas/midas/transforms.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/midas/midas/vit.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/modules/midas/utils.py` & `classy_imaginary-0.5.7/classy_imaginary/modules/midas/utils.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/outpaint.py` & `classy_imaginary-0.5.7/classy_imaginary/outpaint.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/prompt_schedules.py` & `classy_imaginary-0.5.7/classy_imaginary/prompt_schedules.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/roi_utils.py` & `classy_imaginary-0.5.7/classy_imaginary/roi_utils.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/safety.py` & `classy_imaginary-0.5.7/classy_imaginary/safety.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/samplers/__init__.py` & `classy_imaginary-0.5.7/classy_imaginary/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/samplers/base.py` & `classy_imaginary-0.5.7/classy_imaginary/samplers/base.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/samplers/ddim.py` & `classy_imaginary-0.5.7/classy_imaginary/samplers/ddim.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/samplers/editing.py` & `classy_imaginary-0.5.7/classy_imaginary/samplers/editing.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/samplers/kdiff.py` & `classy_imaginary-0.5.7/classy_imaginary/samplers/kdiff.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/samplers/plms.py` & `classy_imaginary-0.5.7/classy_imaginary/samplers/plms.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/schema.py` & `classy_imaginary-0.5.7/classy_imaginary/schema.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/surprise_me.py` & `classy_imaginary-0.5.7/classy_imaginary/surprise_me.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/train.py` & `classy_imaginary-0.5.7/classy_imaginary/train.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/training_tools/image_prep.py` & `classy_imaginary-0.5.7/classy_imaginary/training_tools/image_prep.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/training_tools/prune_model.py` & `classy_imaginary-0.5.7/classy_imaginary/training_tools/prune_model.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/training_tools/single_concept.py` & `classy_imaginary-0.5.7/classy_imaginary/training_tools/single_concept.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/utils.py` & `classy_imaginary-0.5.7/classy_imaginary/utils.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/basicsr/arch_util.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/basicsr/arch_util.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/basicsr/img_util.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/basicsr/img_util.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/basicsr/rrdbnet_arch.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/basicsr/rrdbnet_arch.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/blip/blip.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/blip/blip.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/blip/blip_itm.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/blip/blip_itm.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/blip/blip_nlvr.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/blip/blip_nlvr.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/blip/blip_pretrain.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/blip/blip_pretrain.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/blip/blip_retrieval.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/blip/blip_retrieval.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/blip/blip_vqa.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/blip/blip_vqa.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/blip/configs/caption_coco.yaml` & `classy_imaginary-0.5.7/classy_imaginary/vendored/blip/configs/caption_coco.yaml`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/blip/configs/retrieval_coco.yaml` & `classy_imaginary-0.5.7/classy_imaginary/vendored/blip/configs/retrieval_coco.yaml`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/blip/configs/retrieval_flickr.yaml` & `classy_imaginary-0.5.7/classy_imaginary/vendored/blip/configs/retrieval_flickr.yaml`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/blip/configs/vqa.yaml` & `classy_imaginary-0.5.7/classy_imaginary/vendored/blip/configs/vqa.yaml`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/blip/med.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/blip/med.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/blip/nlvr_encoder.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/blip/nlvr_encoder.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/blip/vit.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/blip/vit.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/clip/bpe_simple_vocab_16e6.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/clip/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/clip/clip.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/clip/clip.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/clip/model.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/clip/model.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/clip/simple_tokenizer.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/clip/simple_tokenizer.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/clipseg/__init__.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/clipseg/__init__.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/clipseg/rd64-uni-refined.pth` & `classy_imaginary-0.5.7/classy_imaginary/vendored/clipseg/rd64-uni-refined.pth`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/codeformer/codeformer_arch.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/codeformer/codeformer_arch.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/codeformer/vqgan_arch.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/codeformer/vqgan_arch.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/LICENSE` & `classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/LICENSE`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/augmentation.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/augmentation.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/external.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/external.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/gns.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/gns.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/layers.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/layers.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/models/image_v1.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/models/image_v1.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/sampling.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/sampling.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/k_diffusion/utils.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/k_diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/LICENSE` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/LICENSE`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/adj-architecture.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/adj-architecture.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/adj-general.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/adj-general.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/animal.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/animal.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/art-movement.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/art-movement.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/artist-surreal.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/artist-surreal.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/artist.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/artist.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/bird.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/bird.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/camera-model.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/camera-model.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/cosmic-nebula.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/cosmic-nebula.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/cosmic-term.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/cosmic-term.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/dinosaur.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/dinosaur.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/fantasy-setting.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/fantasy-setting.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/fish.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/fish.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/flower.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/flower.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/food.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/food.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/fruit.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/fruit.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/landscape-type.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/landscape-type.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/nationality.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/nationality.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/noun-fantasy.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/noun-fantasy.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/noun-general.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/noun-general.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/noun-horror.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/noun-horror.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/occupation.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/occupation.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/pop-culture.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/pop-culture.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/pop-location.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/pop-location.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/rpg-Item.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/rpg-Item.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/scenario-desc.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/scenario-desc.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/video-game.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/video-game.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/noodle_soup_prompts/world-heritage-site.txt.gz` & `classy_imaginary-0.5.7/classy_imaginary/vendored/noodle_soup_prompts/world-heritage-site.txt.gz`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/realesrgan.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/realesrgan.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/classy_imaginary/vendored/smart_crop.py` & `classy_imaginary-0.5.7/classy_imaginary/vendored/smart_crop.py`

 * *Files identical despite different names*

### Comparing `classy_imaginary-0.5.6/pyproject.toml` & `classy_imaginary-0.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "classy-imaginary"
-version = "0.5.6"
+version = "0.5.7"
 description = "This is not a useful package. It is a wrapper around imaginary to provide a Class interface."
 authors = ["Hanoush <hanoush87@gmail.com>"]
 readme = "README.md"
 packages = [{include = "classy_imaginary"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `classy_imaginary-0.5.6/setup.py` & `classy_imaginary-0.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
  'classy_imaginary.vendored.blip': ['configs/*']}
 
 install_requires = \
 ['imaginAIry==11.1.0']
 
 setup_kwargs = {
     'name': 'classy-imaginary',
-    'version': '0.5.6',
+    'version': '0.5.7',
     'description': 'This is not a useful package. It is a wrapper around imaginary to provide a Class interface.',
     'long_description': 'This is not a useful package. It is a wrapper around imaginary to provide a Class interface.\n',
     'author': 'Hanoush',
     'author_email': 'hanoush87@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `classy_imaginary-0.5.6/PKG-INFO` & `classy_imaginary-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classy-imaginary
-Version: 0.5.6
+Version: 0.5.7
 Summary: This is not a useful package. It is a wrapper around imaginary to provide a Class interface.
 Author: Hanoush
 Author-email: hanoush87@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


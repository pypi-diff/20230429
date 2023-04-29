# Comparing `tmp/deepfloyd_if-1.0.1rc0.tar.gz` & `tmp/deepfloyd_if-1.0.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepfloyd_if-1.0.1rc0.tar", last modified: Thu Apr 27 14:48:49 2023, max compression
+gzip compressed data, was "deepfloyd_if-1.0.2rc0.tar", last modified: Sat Apr 29 11:11:39 2023, max compression
```

## Comparing `deepfloyd_if-1.0.1rc0.tar` & `deepfloyd_if-1.0.2rc0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-27 14:48:49.164382 deepfloyd_if-1.0.1rc0/
--rw-r--r--   0 shonenkov   (501) staff       (20)     1504 2023-04-26 14:57:02.000000 deepfloyd_if-1.0.1rc0/LICENSE
--rw-r--r--   0 shonenkov   (501) staff       (20)    11615 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.1rc0/LICENSE-MODEL
--rw-r--r--   0 shonenkov   (501) staff       (20)    14255 2023-04-27 14:48:49.164502 deepfloyd_if-1.0.1rc0/PKG-INFO
--rw-r--r--   0 shonenkov   (501) staff       (20)    14004 2023-04-27 14:00:43.000000 deepfloyd_if-1.0.1rc0/README.md
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-27 14:48:49.153882 deepfloyd_if-1.0.1rc0/deepfloyd_if/
--rw-r--r--   0 shonenkov   (501) staff       (20)       50 2023-04-27 13:01:50.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/__init__.py
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-27 14:48:49.157235 deepfloyd_if-1.0.1rc0/deepfloyd_if/model/
--rw-r--r--   0 shonenkov   (501) staff       (20)      118 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/model/__init__.py
--rw-r--r--   0 shonenkov   (501) staff       (20)    35223 2023-03-09 17:58:29.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/model/gaussian_diffusion.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     2587 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/model/losses.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     5965 2023-01-10 14:02:27.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/model/nn.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     2001 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/model/resample.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     6379 2023-01-10 14:02:27.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/model/respace.py
--rw-r--r--   0 shonenkov   (501) staff       (20)    27952 2023-01-28 11:21:37.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/model/unet.py
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-27 14:48:49.159932 deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/
--rw-r--r--   0 shonenkov   (501) staff       (20)      321 2023-04-26 15:11:36.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/__init__.py
--rw-r--r--   0 shonenkov   (501) staff       (20)    15411 2023-04-26 15:11:36.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/base.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     1977 2023-04-27 14:00:15.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/stage_I.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     1939 2023-04-17 00:13:08.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/stage_II.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     1962 2023-04-17 00:13:08.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/stage_III.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     3126 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/stage_III_sd_x4.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     9421 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/t5.py
--rw-r--r--   0 shonenkov   (501) staff       (20)      742 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/utils.py
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-27 14:48:49.161469 deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/
--rw-r--r--   0 shonenkov   (501) staff       (20)      247 2023-03-19 16:24:39.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/__init__.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     5565 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/dream.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     4522 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/inpainting.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     4443 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/style_transfer.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     1722 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/super_resolution.py
--rw-r--r--   0 shonenkov   (501) staff       (20)      709 2023-03-18 20:13:21.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/utils.py
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-27 14:48:49.162582 deepfloyd_if-1.0.1rc0/deepfloyd_if/resources/
--rw-r--r--   0 shonenkov   (501) staff       (20)     3588 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/resources/p_head_v1.npz
--rw-r--r--   0 shonenkov   (501) staff       (20)     3588 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/resources/w_head_v1.npz
--rw-r--r--   0 shonenkov   (501) staff       (20)      947 2023-01-12 23:07:13.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/resources/wm.png
--rw-r--r--   0 shonenkov   (501) staff       (20)   630912 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/resources/zero_t5-v1_1-xxl_vector.npy
--rw-r--r--   0 shonenkov   (501) staff       (20)     2390 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/utils.py
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-27 14:48:49.154763 deepfloyd_if-1.0.1rc0/deepfloyd_if.egg-info/
--rw-r--r--   0 shonenkov   (501) staff       (20)    14255 2023-04-27 14:48:49.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if.egg-info/PKG-INFO
--rw-r--r--   0 shonenkov   (501) staff       (20)     1123 2023-04-27 14:48:49.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if.egg-info/SOURCES.txt
--rw-r--r--   0 shonenkov   (501) staff       (20)        1 2023-04-27 14:48:49.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if.egg-info/dependency_links.txt
--rw-r--r--   0 shonenkov   (501) staff       (20)      228 2023-04-27 14:48:49.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if.egg-info/requires.txt
--rw-r--r--   0 shonenkov   (501) staff       (20)       99 2023-04-27 14:48:49.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if.egg-info/top_level.txt
--rw-r--r--   0 shonenkov   (501) staff       (20)      281 2023-04-27 14:48:49.165027 deepfloyd_if-1.0.1rc0/setup.cfg
--rw-r--r--   0 shonenkov   (501) staff       (20)     2018 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.1rc0/setup.py
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-29 11:11:39.814243 deepfloyd_if-1.0.2rc0/
+-rw-r--r--   0 shonenkov   (501) staff       (20)     1504 2023-04-26 14:57:02.000000 deepfloyd_if-1.0.2rc0/LICENSE
+-rw-r--r--   0 shonenkov   (501) staff       (20)    11615 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.2rc0/LICENSE-MODEL
+-rw-r--r--   0 shonenkov   (501) staff       (20)    15662 2023-04-29 11:11:39.814336 deepfloyd_if-1.0.2rc0/PKG-INFO
+-rw-r--r--   0 shonenkov   (501) staff       (20)    15411 2023-04-29 11:10:24.000000 deepfloyd_if-1.0.2rc0/README.md
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-29 11:11:39.806879 deepfloyd_if-1.0.2rc0/deepfloyd_if/
+-rw-r--r--   0 shonenkov   (501) staff       (20)       51 2023-04-29 11:10:24.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/__init__.py
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-29 11:11:39.809127 deepfloyd_if-1.0.2rc0/deepfloyd_if/model/
+-rw-r--r--   0 shonenkov   (501) staff       (20)      118 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/model/__init__.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)    35223 2023-03-09 17:58:29.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/model/gaussian_diffusion.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     2587 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/model/losses.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     5965 2023-01-10 14:02:27.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/model/nn.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     2001 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/model/resample.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     6379 2023-01-10 14:02:27.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/model/respace.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)    27952 2023-01-28 11:21:37.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/model/unet.py
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-29 11:11:39.810982 deepfloyd_if-1.0.2rc0/deepfloyd_if/modules/
+-rw-r--r--   0 shonenkov   (501) staff       (20)      321 2023-04-26 15:11:36.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/modules/__init__.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)    15411 2023-04-26 15:11:36.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/modules/base.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     1977 2023-04-27 14:00:15.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/modules/stage_I.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     1939 2023-04-17 00:13:08.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/modules/stage_II.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     1962 2023-04-17 00:13:08.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/modules/stage_III.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     3126 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/modules/stage_III_sd_x4.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     9935 2023-04-29 11:11:16.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/modules/t5.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)      742 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/modules/utils.py
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-29 11:11:39.812003 deepfloyd_if-1.0.2rc0/deepfloyd_if/pipelines/
+-rw-r--r--   0 shonenkov   (501) staff       (20)      247 2023-03-19 16:24:39.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/pipelines/__init__.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     5565 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/pipelines/dream.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     4522 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/pipelines/inpainting.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     4443 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/pipelines/style_transfer.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     1722 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/pipelines/super_resolution.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)      709 2023-03-18 20:13:21.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/pipelines/utils.py
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-29 11:11:39.812866 deepfloyd_if-1.0.2rc0/deepfloyd_if/resources/
+-rw-r--r--   0 shonenkov   (501) staff       (20)     3588 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/resources/p_head_v1.npz
+-rw-r--r--   0 shonenkov   (501) staff       (20)     3588 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/resources/w_head_v1.npz
+-rw-r--r--   0 shonenkov   (501) staff       (20)      947 2023-01-12 23:07:13.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/resources/wm.png
+-rw-r--r--   0 shonenkov   (501) staff       (20)   630912 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/resources/zero_t5-v1_1-xxl_vector.npy
+-rw-r--r--   0 shonenkov   (501) staff       (20)     2390 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if/utils.py
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-29 11:11:39.807551 deepfloyd_if-1.0.2rc0/deepfloyd_if.egg-info/
+-rw-r--r--   0 shonenkov   (501) staff       (20)    15662 2023-04-29 11:11:39.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if.egg-info/PKG-INFO
+-rw-r--r--   0 shonenkov   (501) staff       (20)     1123 2023-04-29 11:11:39.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if.egg-info/SOURCES.txt
+-rw-r--r--   0 shonenkov   (501) staff       (20)        1 2023-04-29 11:11:39.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if.egg-info/dependency_links.txt
+-rw-r--r--   0 shonenkov   (501) staff       (20)      228 2023-04-29 11:11:39.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if.egg-info/requires.txt
+-rw-r--r--   0 shonenkov   (501) staff       (20)       99 2023-04-29 11:11:39.000000 deepfloyd_if-1.0.2rc0/deepfloyd_if.egg-info/top_level.txt
+-rw-r--r--   0 shonenkov   (501) staff       (20)      281 2023-04-29 11:11:39.814673 deepfloyd_if-1.0.2rc0/setup.cfg
+-rw-r--r--   0 shonenkov   (501) staff       (20)     2018 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.2rc0/setup.py
```

### Comparing `deepfloyd_if-1.0.1rc0/LICENSE` & `deepfloyd_if-1.0.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/LICENSE-MODEL` & `deepfloyd_if-1.0.2rc0/LICENSE-MODEL`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/PKG-INFO` & `deepfloyd_if-1.0.2rc0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: deepfloyd_if
-Version: 1.0.1rc0
+Version: 1.0.2rc0
 Summary: DeepFloyd-IF (Imagen Free)
 Author: DeepFloyd, StabilityAI
 Author-email: shonenkov@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE-MODEL
 
 [![License](https://img.shields.io/badge/Code_License-Modified_MIT-blue.svg)](LICENSE)
 [![License](https://img.shields.io/badge/Weights_License-DeepFloyd_IF-orange.svg)](LICENSE-MODEL)
 [![Downloads](https://pepy.tech/badge/deepfloyd_if)](https://pepy.tech/project/deepfloyd_if)
+[![Discord](https://img.shields.io/badge/Discord-%237289DA.svg?logo=discord&logoColor=white)](https://discord.gg/umz62Mgr)
+[![Twitter](https://img.shields.io/badge/Twitter-%231DA1F2.svg?logo=twitter&logoColor=white)](https://twitter.com/deepfloydai)
+[![Linktree](https://img.shields.io/badge/Linktree-%2339E09B.svg?logo=linktree&logoColor=white)](http://linktr.ee/deepfloyd)
 
-# IF by DeepFloyd Lab at [StabilityAI](https://stability.ai/)
+# IF by [DeepFloyd Lab](https://deepfloyd.ai) at [StabilityAI](https://stability.ai/)
 
 <p align="center">
   <img src="./pics/nabla.jpg" width="100%">
 </p>
 
 We introduce DeepFloyd IF, a novel state-of-the-art open-source text-to-image model with a high degree of photorealism and language understanding. DeepFloyd IF is a modular composed of a frozen text encoder and three cascaded pixel diffusion modules: a base model that generates 64x64 px image based on text prompt and two super-resolution models, each designed to generate images of increasing resolution: 256x256 px and 1024x1024 px. All stages of the model utilize a frozen text encoder based on the T5 transformer to extract text embeddings, which are then fed into a UNet architecture enhanced with cross-attention and attention pooling. The result is a highly efficient model that outperforms current state-of-the-art models, achieving a zero-shot FID score of 6.66 on the COCO dataset. Our work underscores the potential of larger UNet architectures in the first stage of cascaded diffusion models and depicts a promising future for text-to-image synthesis.
 
@@ -33,22 +36,26 @@
 
 
 ## Quick Start
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/deepfloyd_if_free_tier_google_colab.ipynb)
 [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/DeepFloyd/IF)
 
 ```shell
-pip install deepfloyd_if==1.0.1rc
+pip install deepfloyd_if==1.0.2rc0
 pip install xformers==0.0.16
 pip install git+https://github.com/openai/CLIP.git --no-deps
 ```
 
-## Local notebook and UI demo
+## Local notebooks
+[![Jupyter Notebook](https://img.shields.io/badge/jupyter_notebook-%23FF7A01.svg?logo=jupyter&logoColor=white)](https://huggingface.co/DeepFloyd/IF-notebooks/blob/main/pipes-DeepFloyd-IF-v1.0.ipynb)
+[![Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/code/shonenkov/deepfloyd-if-4-3b-generator-of-pictures)
+
+The Dream, Style Transfer, Super Resolution or Inpainting modes are avaliable in a Jupyter Notebook [here](https://huggingface.co/DeepFloyd/IF-notebooks/blob/main/pipes-DeepFloyd-IF-v1.0.ipynb).
+
 
-The Dream, Style Transfer, Super Resolution or Inpainting modes are avaliable as in a Jupyter Notebook at `IF/notebooks/pipes-DeepFloyd-IF.ipynb`.
 
 ## Integration with 🤗 Diffusers
 
 IF is also integrated with the 🤗 Hugging Face [Diffusers library](https://github.com/huggingface/diffusers/).
 
 Diffusers runs each stage individually allowing the user to customize the image generation process as well as allowing to inspect intermediate results easily.
 
@@ -131,15 +138,15 @@
 ```
 
  There are multiple ways to speed up the inference time and lower the memory consumption even more with `diffusers`. To do so, please have a look at the Diffusers docs:
 
 - 🚀 [Optimizing for inference time](https://huggingface.co/docs/diffusers/api/pipelines/if#optimizing-for-speed)
 - ⚙️ [Optimizing for low memory during inference](https://huggingface.co/docs/diffusers/api/pipelines/if#optimizing-for-memory)
 
-For more in-detail information about how to use IF, please have a look at [the IF blog post](https://huggingface.co/blog/if) 📖.
+For more in-detail information about how to use IF, please have a look at [the IF blog post](https://huggingface.co/blog/if) and [the documentation](https://huggingface.co/docs/diffusers/main/en/api/pipelines/if) 📖.
 
 ## Run the code locally
 
 ### Loading the models into VRAM
 
 ```python
 from deepfloyd_if.modules import IFStageI, IFStageII, StableStageIII
@@ -318,33 +325,37 @@
 
 ## License
 
 The code in this repository is released under the bespoke license (see added [point two](https://github.com/deep-floyd/IF/blob/main/LICENSE#L13)).
 
 The weights will be available soon via [the DeepFloyd organization at Hugging Face](https://huggingface.co/DeepFloyd) and have their own LICENSE.
 
+**Disclaimer:** *The initial release of the IF model is under a restricted research-purposes-only license temporarily to gather feedback, and after that we intend to release a fully open-source model in line with other Stability AI models.*
+
 ## Limitations and Biases
 
 The models available in this codebase have known limitations and biases. Please refer to [the model card](https://huggingface.co/DeepFloyd/IF-I-L-v1.0) for more information.
 
 
 ## 🎓 DeepFloyd IF creators:
-- [Alex Shonenkov](https://github.com/shonenkov)
-- [Misha Konstantinov](https://github.com/zeroshot-ai)
-- [Daria Bakshandaeva](https://github.com/Gugutse)
-- [Christoph Schuhmann](https://github.com/christophschuhmann)
-- [Ksenia Ivanova](https://github.com/ivksu)
-- [Nadiia Klokova](https://github.com/vauimpuls)
+
+- Alex Shonenkov [GitHub](https://github.com/shonenkov) | [Linktr](https://linktr.ee/shonenkovAI)
+- Misha Konstantinov [GitHub](https://github.com/zeroshot-ai) | [Twitter](https://twitter.com/_bra_ket)
+- Daria Bakshandaeva [GitHub](https://github.com/Gugutse) | [Twitter](https://twitter.com/_gugutse_)
+- Christoph Schuhmann [GitHub](https://github.com/christophschuhmann) | [Twitter](https://twitter.com/laion_ai)
+- Ksenia Ivanova [GitHub](https://github.com/ivksu) | [Twitter](https://twitter.com/susiaiv)
+- Nadiia Klokova [GitHub](https://github.com/vauimpuls) | [Twitter](https://twitter.com/vauimpuls)
+
 
 ## 📄 Research Paper (Soon)
 
 ## Acknowledgements
 
 Special thanks to [StabilityAI](http://stability.ai) and its CEO [Emad Mostaque](https://twitter.com/emostaque) for invaluable support, providing GPU compute and infrastructure to train the models (our gratitude goes to [Richard Vencu](https://github.com/rvencu)); thanks to [LAION](https://laion.ai) and [Christoph Schuhmann](https://github.com/christophschuhmann) in particular for contribution to the project and well-prepared datasets; thanks to [Huggingface](https://huggingface.co) teams for optimizing models' speed and memory consumption during inference, creating demos and giving cool advice!
 
 ## 🚀 External Contributors 🚀
 - The Biggest Thanks [@Apolinário](https://github.com/apolinario), for ideas, consultations, help and support on all stages to make IF available in open-source; for writing a lot of documentation and instructions; for creating a friendly atmosphere in difficult moments 🦉;
 - Thanks, [@patrickvonplaten](https://github.com/patrickvonplaten), for improving loading time of unet models by 80%;
 for integration Stable-Diffusion-x4 as native pipeline 💪;
 - Thanks, [@williamberman](https://github.com/williamberman) and [@patrickvonplaten](https://github.com/patrickvonplaten) for diffusers integration 🙌;
 - Thanks, [@hysts](https://github.com/hysts) and [@Apolinário](https://github.com/apolinario) for creating [the best gradio demo with IF](https://huggingface.co/spaces/DeepFloyd/IF) 🚀;
-- Thanks, [@Dango233](https://github.com/Dango233), for adaptation IF with xformers memory efficient attention 💪;
+- Thanks, [@Dango233](https://github.com/Dango233), for adapting IF with xformers memory efficient attention 💪;
```

### Comparing `deepfloyd_if-1.0.1rc0/README.md` & `deepfloyd_if-1.0.2rc0/deepfloyd_if.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,25 @@
+Metadata-Version: 2.1
+Name: deepfloyd-if
+Version: 1.0.2rc0
+Summary: DeepFloyd-IF (Imagen Free)
+Author: DeepFloyd, StabilityAI
+Author-email: shonenkov@gmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE-MODEL
+
 [![License](https://img.shields.io/badge/Code_License-Modified_MIT-blue.svg)](LICENSE)
 [![License](https://img.shields.io/badge/Weights_License-DeepFloyd_IF-orange.svg)](LICENSE-MODEL)
 [![Downloads](https://pepy.tech/badge/deepfloyd_if)](https://pepy.tech/project/deepfloyd_if)
+[![Discord](https://img.shields.io/badge/Discord-%237289DA.svg?logo=discord&logoColor=white)](https://discord.gg/umz62Mgr)
+[![Twitter](https://img.shields.io/badge/Twitter-%231DA1F2.svg?logo=twitter&logoColor=white)](https://twitter.com/deepfloydai)
+[![Linktree](https://img.shields.io/badge/Linktree-%2339E09B.svg?logo=linktree&logoColor=white)](http://linktr.ee/deepfloyd)
 
-# IF by DeepFloyd Lab at [StabilityAI](https://stability.ai/)
+# IF by [DeepFloyd Lab](https://deepfloyd.ai) at [StabilityAI](https://stability.ai/)
 
 <p align="center">
   <img src="./pics/nabla.jpg" width="100%">
 </p>
 
 We introduce DeepFloyd IF, a novel state-of-the-art open-source text-to-image model with a high degree of photorealism and language understanding. DeepFloyd IF is a modular composed of a frozen text encoder and three cascaded pixel diffusion modules: a base model that generates 64x64 px image based on text prompt and two super-resolution models, each designed to generate images of increasing resolution: 256x256 px and 1024x1024 px. All stages of the model utilize a frozen text encoder based on the T5 transformer to extract text embeddings, which are then fed into a UNet architecture enhanced with cross-attention and attention pooling. The result is a highly efficient model that outperforms current state-of-the-art models, achieving a zero-shot FID score of 6.66 on the COCO dataset. Our work underscores the potential of larger UNet architectures in the first stage of cascaded diffusion models and depicts a promising future for text-to-image synthesis.
 
@@ -23,22 +36,26 @@
 
 
 ## Quick Start
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/deepfloyd_if_free_tier_google_colab.ipynb)
 [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/DeepFloyd/IF)
 
 ```shell
-pip install deepfloyd_if==1.0.1rc
+pip install deepfloyd_if==1.0.2rc0
 pip install xformers==0.0.16
 pip install git+https://github.com/openai/CLIP.git --no-deps
 ```
 
-## Local notebook and UI demo
+## Local notebooks
+[![Jupyter Notebook](https://img.shields.io/badge/jupyter_notebook-%23FF7A01.svg?logo=jupyter&logoColor=white)](https://huggingface.co/DeepFloyd/IF-notebooks/blob/main/pipes-DeepFloyd-IF-v1.0.ipynb)
+[![Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/code/shonenkov/deepfloyd-if-4-3b-generator-of-pictures)
+
+The Dream, Style Transfer, Super Resolution or Inpainting modes are avaliable in a Jupyter Notebook [here](https://huggingface.co/DeepFloyd/IF-notebooks/blob/main/pipes-DeepFloyd-IF-v1.0.ipynb).
+
 
-The Dream, Style Transfer, Super Resolution or Inpainting modes are avaliable as in a Jupyter Notebook at `IF/notebooks/pipes-DeepFloyd-IF.ipynb`.
 
 ## Integration with 🤗 Diffusers
 
 IF is also integrated with the 🤗 Hugging Face [Diffusers library](https://github.com/huggingface/diffusers/).
 
 Diffusers runs each stage individually allowing the user to customize the image generation process as well as allowing to inspect intermediate results easily.
 
@@ -121,15 +138,15 @@
 ```
 
  There are multiple ways to speed up the inference time and lower the memory consumption even more with `diffusers`. To do so, please have a look at the Diffusers docs:
 
 - 🚀 [Optimizing for inference time](https://huggingface.co/docs/diffusers/api/pipelines/if#optimizing-for-speed)
 - ⚙️ [Optimizing for low memory during inference](https://huggingface.co/docs/diffusers/api/pipelines/if#optimizing-for-memory)
 
-For more in-detail information about how to use IF, please have a look at [the IF blog post](https://huggingface.co/blog/if) 📖.
+For more in-detail information about how to use IF, please have a look at [the IF blog post](https://huggingface.co/blog/if) and [the documentation](https://huggingface.co/docs/diffusers/main/en/api/pipelines/if) 📖.
 
 ## Run the code locally
 
 ### Loading the models into VRAM
 
 ```python
 from deepfloyd_if.modules import IFStageI, IFStageII, StableStageIII
@@ -308,33 +325,37 @@
 
 ## License
 
 The code in this repository is released under the bespoke license (see added [point two](https://github.com/deep-floyd/IF/blob/main/LICENSE#L13)).
 
 The weights will be available soon via [the DeepFloyd organization at Hugging Face](https://huggingface.co/DeepFloyd) and have their own LICENSE.
 
+**Disclaimer:** *The initial release of the IF model is under a restricted research-purposes-only license temporarily to gather feedback, and after that we intend to release a fully open-source model in line with other Stability AI models.*
+
 ## Limitations and Biases
 
 The models available in this codebase have known limitations and biases. Please refer to [the model card](https://huggingface.co/DeepFloyd/IF-I-L-v1.0) for more information.
 
 
 ## 🎓 DeepFloyd IF creators:
-- [Alex Shonenkov](https://github.com/shonenkov)
-- [Misha Konstantinov](https://github.com/zeroshot-ai)
-- [Daria Bakshandaeva](https://github.com/Gugutse)
-- [Christoph Schuhmann](https://github.com/christophschuhmann)
-- [Ksenia Ivanova](https://github.com/ivksu)
-- [Nadiia Klokova](https://github.com/vauimpuls)
+
+- Alex Shonenkov [GitHub](https://github.com/shonenkov) | [Linktr](https://linktr.ee/shonenkovAI)
+- Misha Konstantinov [GitHub](https://github.com/zeroshot-ai) | [Twitter](https://twitter.com/_bra_ket)
+- Daria Bakshandaeva [GitHub](https://github.com/Gugutse) | [Twitter](https://twitter.com/_gugutse_)
+- Christoph Schuhmann [GitHub](https://github.com/christophschuhmann) | [Twitter](https://twitter.com/laion_ai)
+- Ksenia Ivanova [GitHub](https://github.com/ivksu) | [Twitter](https://twitter.com/susiaiv)
+- Nadiia Klokova [GitHub](https://github.com/vauimpuls) | [Twitter](https://twitter.com/vauimpuls)
+
 
 ## 📄 Research Paper (Soon)
 
 ## Acknowledgements
 
 Special thanks to [StabilityAI](http://stability.ai) and its CEO [Emad Mostaque](https://twitter.com/emostaque) for invaluable support, providing GPU compute and infrastructure to train the models (our gratitude goes to [Richard Vencu](https://github.com/rvencu)); thanks to [LAION](https://laion.ai) and [Christoph Schuhmann](https://github.com/christophschuhmann) in particular for contribution to the project and well-prepared datasets; thanks to [Huggingface](https://huggingface.co) teams for optimizing models' speed and memory consumption during inference, creating demos and giving cool advice!
 
 ## 🚀 External Contributors 🚀
 - The Biggest Thanks [@Apolinário](https://github.com/apolinario), for ideas, consultations, help and support on all stages to make IF available in open-source; for writing a lot of documentation and instructions; for creating a friendly atmosphere in difficult moments 🦉;
 - Thanks, [@patrickvonplaten](https://github.com/patrickvonplaten), for improving loading time of unet models by 80%;
 for integration Stable-Diffusion-x4 as native pipeline 💪;
 - Thanks, [@williamberman](https://github.com/williamberman) and [@patrickvonplaten](https://github.com/patrickvonplaten) for diffusers integration 🙌;
 - Thanks, [@hysts](https://github.com/hysts) and [@Apolinário](https://github.com/apolinario) for creating [the best gradio demo with IF](https://huggingface.co/spaces/DeepFloyd/IF) 🚀;
-- Thanks, [@Dango233](https://github.com/Dango233), for adaptation IF with xformers memory efficient attention 💪;
+- Thanks, [@Dango233](https://github.com/Dango233), for adapting IF with xformers memory efficient attention 💪;
```

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/model/gaussian_diffusion.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/model/gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/model/losses.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/model/losses.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/model/nn.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/model/nn.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/model/resample.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/model/resample.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/model/respace.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/model/respace.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/model/unet.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/model/unet.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/base.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/modules/base.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/stage_I.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/modules/stage_I.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/stage_II.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/modules/stage_II.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/stage_III.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/modules/stage_III.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/stage_III_sd_x4.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/modules/stage_III_sd_x4.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/t5.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/modules/t5.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,26 +58,34 @@
                 t5_model_kwargs['device_map'] = {'shared': self.device, 'encoder': self.device}
 
         self.use_text_preprocessing = use_text_preprocessing
         self.hf_token = hf_token
         self.cache_dir = cache_dir or os.path.expanduser('~/.cache/IF_')
         self.dir_or_name = dir_or_name
 
-        path = dir_or_name
+        tokenizer_path, path = dir_or_name, dir_or_name
         if dir_or_name in self.available_models:
             cache_dir = os.path.join(self.cache_dir, dir_or_name)
             for filename in [
                 'config.json', 'special_tokens_map.json', 'spiece.model', 'tokenizer_config.json',
                 'pytorch_model.bin.index.json', 'pytorch_model-00001-of-00002.bin', 'pytorch_model-00002-of-00002.bin'
             ]:
                 hf_hub_download(repo_id=f'DeepFloyd/{dir_or_name}', filename=filename, cache_dir=cache_dir,
                                 force_filename=filename, token=self.hf_token)
-            path = cache_dir
+            tokenizer_path, path = cache_dir, cache_dir
+        else:
+            cache_dir = os.path.join(self.cache_dir, 't5-v1_1-xxl')
+            for filename in [
+                'config.json', 'special_tokens_map.json', 'spiece.model', 'tokenizer_config.json',
+            ]:
+                hf_hub_download(repo_id='DeepFloyd/t5-v1_1-xxl', filename=filename, cache_dir=cache_dir,
+                                force_filename=filename, token=self.hf_token)
+            tokenizer_path = cache_dir
 
-        self.tokenizer = AutoTokenizer.from_pretrained(path)
+        self.tokenizer = AutoTokenizer.from_pretrained(tokenizer_path)
         self.model = T5EncoderModel.from_pretrained(path, **t5_model_kwargs).eval()
 
     def get_text_embeddings(self, texts):
         texts = [self.text_preprocessing(text) for text in texts]
 
         text_tokens_and_mask = self.tokenizer(
             texts,
```

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/utils.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/modules/utils.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/dream.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/pipelines/dream.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/inpainting.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/pipelines/inpainting.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/style_transfer.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/pipelines/style_transfer.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/super_resolution.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/pipelines/super_resolution.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/utils.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/resources/p_head_v1.npz` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/resources/p_head_v1.npz`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/resources/w_head_v1.npz` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/resources/w_head_v1.npz`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/resources/wm.png` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/resources/wm.png`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/resources/zero_t5-v1_1-xxl_vector.npy` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/resources/zero_t5-v1_1-xxl_vector.npy`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if/utils.py` & `deepfloyd_if-1.0.2rc0/deepfloyd_if/utils.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if.egg-info/PKG-INFO` & `deepfloyd_if-1.0.2rc0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,15 @@
-Metadata-Version: 2.1
-Name: deepfloyd-if
-Version: 1.0.1rc0
-Summary: DeepFloyd-IF (Imagen Free)
-Author: DeepFloyd, StabilityAI
-Author-email: shonenkov@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: LICENSE-MODEL
-
 [![License](https://img.shields.io/badge/Code_License-Modified_MIT-blue.svg)](LICENSE)
 [![License](https://img.shields.io/badge/Weights_License-DeepFloyd_IF-orange.svg)](LICENSE-MODEL)
 [![Downloads](https://pepy.tech/badge/deepfloyd_if)](https://pepy.tech/project/deepfloyd_if)
+[![Discord](https://img.shields.io/badge/Discord-%237289DA.svg?logo=discord&logoColor=white)](https://discord.gg/umz62Mgr)
+[![Twitter](https://img.shields.io/badge/Twitter-%231DA1F2.svg?logo=twitter&logoColor=white)](https://twitter.com/deepfloydai)
+[![Linktree](https://img.shields.io/badge/Linktree-%2339E09B.svg?logo=linktree&logoColor=white)](http://linktr.ee/deepfloyd)
 
-# IF by DeepFloyd Lab at [StabilityAI](https://stability.ai/)
+# IF by [DeepFloyd Lab](https://deepfloyd.ai) at [StabilityAI](https://stability.ai/)
 
 <p align="center">
   <img src="./pics/nabla.jpg" width="100%">
 </p>
 
 We introduce DeepFloyd IF, a novel state-of-the-art open-source text-to-image model with a high degree of photorealism and language understanding. DeepFloyd IF is a modular composed of a frozen text encoder and three cascaded pixel diffusion modules: a base model that generates 64x64 px image based on text prompt and two super-resolution models, each designed to generate images of increasing resolution: 256x256 px and 1024x1024 px. All stages of the model utilize a frozen text encoder based on the T5 transformer to extract text embeddings, which are then fed into a UNet architecture enhanced with cross-attention and attention pooling. The result is a highly efficient model that outperforms current state-of-the-art models, achieving a zero-shot FID score of 6.66 on the COCO dataset. Our work underscores the potential of larger UNet architectures in the first stage of cascaded diffusion models and depicts a promising future for text-to-image synthesis.
 
@@ -33,22 +26,26 @@
 
 
 ## Quick Start
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/deepfloyd_if_free_tier_google_colab.ipynb)
 [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/DeepFloyd/IF)
 
 ```shell
-pip install deepfloyd_if==1.0.1rc
+pip install deepfloyd_if==1.0.2rc0
 pip install xformers==0.0.16
 pip install git+https://github.com/openai/CLIP.git --no-deps
 ```
 
-## Local notebook and UI demo
+## Local notebooks
+[![Jupyter Notebook](https://img.shields.io/badge/jupyter_notebook-%23FF7A01.svg?logo=jupyter&logoColor=white)](https://huggingface.co/DeepFloyd/IF-notebooks/blob/main/pipes-DeepFloyd-IF-v1.0.ipynb)
+[![Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/code/shonenkov/deepfloyd-if-4-3b-generator-of-pictures)
+
+The Dream, Style Transfer, Super Resolution or Inpainting modes are avaliable in a Jupyter Notebook [here](https://huggingface.co/DeepFloyd/IF-notebooks/blob/main/pipes-DeepFloyd-IF-v1.0.ipynb).
+
 
-The Dream, Style Transfer, Super Resolution or Inpainting modes are avaliable as in a Jupyter Notebook at `IF/notebooks/pipes-DeepFloyd-IF.ipynb`.
 
 ## Integration with 🤗 Diffusers
 
 IF is also integrated with the 🤗 Hugging Face [Diffusers library](https://github.com/huggingface/diffusers/).
 
 Diffusers runs each stage individually allowing the user to customize the image generation process as well as allowing to inspect intermediate results easily.
 
@@ -131,15 +128,15 @@
 ```
 
  There are multiple ways to speed up the inference time and lower the memory consumption even more with `diffusers`. To do so, please have a look at the Diffusers docs:
 
 - 🚀 [Optimizing for inference time](https://huggingface.co/docs/diffusers/api/pipelines/if#optimizing-for-speed)
 - ⚙️ [Optimizing for low memory during inference](https://huggingface.co/docs/diffusers/api/pipelines/if#optimizing-for-memory)
 
-For more in-detail information about how to use IF, please have a look at [the IF blog post](https://huggingface.co/blog/if) 📖.
+For more in-detail information about how to use IF, please have a look at [the IF blog post](https://huggingface.co/blog/if) and [the documentation](https://huggingface.co/docs/diffusers/main/en/api/pipelines/if) 📖.
 
 ## Run the code locally
 
 ### Loading the models into VRAM
 
 ```python
 from deepfloyd_if.modules import IFStageI, IFStageII, StableStageIII
@@ -318,33 +315,37 @@
 
 ## License
 
 The code in this repository is released under the bespoke license (see added [point two](https://github.com/deep-floyd/IF/blob/main/LICENSE#L13)).
 
 The weights will be available soon via [the DeepFloyd organization at Hugging Face](https://huggingface.co/DeepFloyd) and have their own LICENSE.
 
+**Disclaimer:** *The initial release of the IF model is under a restricted research-purposes-only license temporarily to gather feedback, and after that we intend to release a fully open-source model in line with other Stability AI models.*
+
 ## Limitations and Biases
 
 The models available in this codebase have known limitations and biases. Please refer to [the model card](https://huggingface.co/DeepFloyd/IF-I-L-v1.0) for more information.
 
 
 ## 🎓 DeepFloyd IF creators:
-- [Alex Shonenkov](https://github.com/shonenkov)
-- [Misha Konstantinov](https://github.com/zeroshot-ai)
-- [Daria Bakshandaeva](https://github.com/Gugutse)
-- [Christoph Schuhmann](https://github.com/christophschuhmann)
-- [Ksenia Ivanova](https://github.com/ivksu)
-- [Nadiia Klokova](https://github.com/vauimpuls)
+
+- Alex Shonenkov [GitHub](https://github.com/shonenkov) | [Linktr](https://linktr.ee/shonenkovAI)
+- Misha Konstantinov [GitHub](https://github.com/zeroshot-ai) | [Twitter](https://twitter.com/_bra_ket)
+- Daria Bakshandaeva [GitHub](https://github.com/Gugutse) | [Twitter](https://twitter.com/_gugutse_)
+- Christoph Schuhmann [GitHub](https://github.com/christophschuhmann) | [Twitter](https://twitter.com/laion_ai)
+- Ksenia Ivanova [GitHub](https://github.com/ivksu) | [Twitter](https://twitter.com/susiaiv)
+- Nadiia Klokova [GitHub](https://github.com/vauimpuls) | [Twitter](https://twitter.com/vauimpuls)
+
 
 ## 📄 Research Paper (Soon)
 
 ## Acknowledgements
 
 Special thanks to [StabilityAI](http://stability.ai) and its CEO [Emad Mostaque](https://twitter.com/emostaque) for invaluable support, providing GPU compute and infrastructure to train the models (our gratitude goes to [Richard Vencu](https://github.com/rvencu)); thanks to [LAION](https://laion.ai) and [Christoph Schuhmann](https://github.com/christophschuhmann) in particular for contribution to the project and well-prepared datasets; thanks to [Huggingface](https://huggingface.co) teams for optimizing models' speed and memory consumption during inference, creating demos and giving cool advice!
 
 ## 🚀 External Contributors 🚀
 - The Biggest Thanks [@Apolinário](https://github.com/apolinario), for ideas, consultations, help and support on all stages to make IF available in open-source; for writing a lot of documentation and instructions; for creating a friendly atmosphere in difficult moments 🦉;
 - Thanks, [@patrickvonplaten](https://github.com/patrickvonplaten), for improving loading time of unet models by 80%;
 for integration Stable-Diffusion-x4 as native pipeline 💪;
 - Thanks, [@williamberman](https://github.com/williamberman) and [@patrickvonplaten](https://github.com/patrickvonplaten) for diffusers integration 🙌;
 - Thanks, [@hysts](https://github.com/hysts) and [@Apolinário](https://github.com/apolinario) for creating [the best gradio demo with IF](https://huggingface.co/spaces/DeepFloyd/IF) 🚀;
-- Thanks, [@Dango233](https://github.com/Dango233), for adaptation IF with xformers memory efficient attention 💪;
+- Thanks, [@Dango233](https://github.com/Dango233), for adapting IF with xformers memory efficient attention 💪;
```

### Comparing `deepfloyd_if-1.0.1rc0/deepfloyd_if.egg-info/SOURCES.txt` & `deepfloyd_if-1.0.2rc0/deepfloyd_if.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1rc0/setup.py` & `deepfloyd_if-1.0.2rc0/setup.py`

 * *Files identical despite different names*


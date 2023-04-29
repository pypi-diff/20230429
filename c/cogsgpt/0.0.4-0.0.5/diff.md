# Comparing `tmp/cogsgpt-0.0.4.tar.gz` & `tmp/cogsgpt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogsgpt-0.0.4.tar", last modified: Fri Apr 28 16:47:43 2023, max compression
+gzip compressed data, was "cogsgpt-0.0.5.tar", last modified: Sat Apr 29 15:12:37 2023, max compression
```

## Comparing `cogsgpt-0.0.4.tar` & `cogsgpt-0.0.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-28 16:47:43.289645 cogsgpt-0.0.4/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1065 2023-04-12 05:29:48.000000 cogsgpt-0.0.4/LICENSE
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-24 05:08:50.000000 cogsgpt-0.0.4/MANIFEST.in
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     6757 2023-04-28 16:47:43.289645 cogsgpt-0.0.4/PKG-INFO
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5013 2023-04-28 16:42:52.000000 cogsgpt-0.0.4/README.md
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-28 16:47:43.285645 cogsgpt-0.0.4/cogsgpt/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      154 2023-04-24 07:01:19.000000 cogsgpt-0.0.4/cogsgpt/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)    13508 2023-04-28 11:43:48.000000 cogsgpt-0.0.4/cogsgpt/awesome_chat.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-28 16:47:43.285645 cogsgpt-0.0.4/cogsgpt/cogsmodel/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       92 2023-04-13 04:29:18.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      202 2023-04-25 03:24:15.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/base_model.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-28 16:47:43.285645 cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1058 2023-04-26 07:16:38.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1869 2023-04-26 01:40:24.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/background_remover.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     5601 2023-04-28 13:34:38.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/form_recognizer.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     7020 2023-04-27 02:47:18.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/image_analysis_v3.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     6544 2023-04-27 04:13:01.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/image_analysis_v4.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2581 2023-04-28 05:26:48.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/utils.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-28 16:47:43.285645 cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      599 2023-04-28 03:04:51.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3504 2023-04-27 03:53:31.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/text_analysis.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1823 2023-04-28 03:12:03.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/text_generation.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2219 2023-04-27 03:51:10.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/text_summarize.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1710 2023-04-27 04:05:31.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/text_translation.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-28 16:47:43.285645 cogsgpt-0.0.4/cogsgpt/cogsmodel/speech/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       73 2023-04-12 13:18:32.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/speech/__init__.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     3926 2023-04-27 03:48:02.000000 cogsgpt-0.0.4/cogsgpt/cogsmodel/speech/speech.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2835 2023-04-24 07:40:16.000000 cogsgpt-0.0.4/cogsgpt/llm.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      445 2023-04-24 03:37:51.000000 cogsgpt-0.0.4/cogsgpt/logger.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-28 16:47:43.285645 cogsgpt-0.0.4/cogsgpt/metas/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      316 2023-04-12 04:35:32.000000 cogsgpt-0.0.4/cogsgpt/metas/generate_response_presteps.json
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2861 2023-04-28 03:41:32.000000 cogsgpt-0.0.4/cogsgpt/metas/parse_task_presteps.json
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2047 2023-04-28 01:19:48.000000 cogsgpt-0.0.4/cogsgpt/metas/prompts.yaml
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     4718 2023-04-28 13:35:33.000000 cogsgpt-0.0.4/cogsgpt/metas/task_metas.yaml
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      369 2023-04-27 02:28:37.000000 cogsgpt-0.0.4/cogsgpt/schema.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      892 2023-04-24 07:01:19.000000 cogsgpt-0.0.4/cogsgpt/utils.py
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-28 16:47:43.285645 cogsgpt-0.0.4/cogsgpt.egg-info/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     6757 2023-04-28 16:47:43.000000 cogsgpt-0.0.4/cogsgpt.egg-info/PKG-INFO
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1261 2023-04-28 16:47:43.000000 cogsgpt-0.0.4/cogsgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)        1 2023-04-28 16:47:43.000000 cogsgpt-0.0.4/cogsgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      189 2023-04-28 16:47:43.000000 cogsgpt-0.0.4/cogsgpt.egg-info/requires.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)        8 2023-04-28 16:47:43.000000 cogsgpt-0.0.4/cogsgpt.egg-info/top_level.txt
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      934 2023-04-25 07:16:49.000000 cogsgpt-0.0.4/pyproject.toml
--rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-28 16:47:43.289645 cogsgpt-0.0.4/setup.cfg
-drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-28 16:47:43.285645 cogsgpt-0.0.4/tests/
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1763 2023-04-28 13:14:29.000000 cogsgpt-0.0.4/tests/test_awesome_chat.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      550 2023-04-26 01:38:49.000000 cogsgpt-0.0.4/tests/test_bg_remove.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     2840 2023-04-27 02:44:47.000000 cogsgpt-0.0.4/tests/test_form_recognizer.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     4952 2023-04-27 01:52:52.000000 cogsgpt-0.0.4/tests/test_image_analisys.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)      602 2023-04-26 14:09:19.000000 cogsgpt-0.0.4/tests/test_speech.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1632 2023-04-26 14:18:48.000000 cogsgpt-0.0.4/tests/test_text_analysis.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1232 2023-04-28 03:12:51.000000 cogsgpt-0.0.4/tests/test_text_generation.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1971 2023-04-24 07:02:12.000000 cogsgpt-0.0.4/tests/test_text_summarize.py
--rw-rw-r--   0 weitian   (1000) weitian   (1000)     1195 2023-04-27 04:15:40.000000 cogsgpt-0.0.4/tests/test_text_translation.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-29 15:12:37.917924 cogsgpt-0.0.5/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1065 2023-04-12 05:29:48.000000 cogsgpt-0.0.5/LICENSE
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-24 05:08:50.000000 cogsgpt-0.0.5/MANIFEST.in
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     7365 2023-04-29 15:12:37.917924 cogsgpt-0.0.5/PKG-INFO
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5622 2023-04-29 15:09:38.000000 cogsgpt-0.0.5/README.md
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-29 15:12:37.901924 cogsgpt-0.0.5/cogsgpt/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      154 2023-04-29 15:01:53.000000 cogsgpt-0.0.5/cogsgpt/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)    13639 2023-04-29 07:10:23.000000 cogsgpt-0.0.5/cogsgpt/awesome_chat.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-29 15:12:37.901924 cogsgpt-0.0.5/cogsgpt/cogsmodel/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       92 2023-04-13 04:29:18.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      202 2023-04-25 03:24:15.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/base_model.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-29 15:12:37.905924 cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1058 2023-04-26 07:16:38.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1869 2023-04-26 01:40:24.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/background_remover.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     5601 2023-04-28 13:34:38.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/form_recognizer.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     7020 2023-04-27 02:47:18.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/image_analysis_v3.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     6544 2023-04-27 04:13:01.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/image_analysis_v4.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2581 2023-04-28 05:26:48.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/utils.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-29 15:12:37.909924 cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      599 2023-04-28 03:04:51.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3504 2023-04-27 03:53:31.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/text_analysis.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1823 2023-04-28 03:12:03.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/text_generation.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2219 2023-04-27 03:51:10.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/text_summarize.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1710 2023-04-27 04:05:31.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/text_translation.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-29 15:12:37.909924 cogsgpt-0.0.5/cogsgpt/cogsmodel/speech/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       73 2023-04-12 13:18:32.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/speech/__init__.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     3926 2023-04-27 03:48:02.000000 cogsgpt-0.0.5/cogsgpt/cogsmodel/speech/speech.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2835 2023-04-24 07:40:16.000000 cogsgpt-0.0.5/cogsgpt/llm.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      460 2023-04-29 14:44:13.000000 cogsgpt-0.0.5/cogsgpt/logger.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-29 15:12:37.909924 cogsgpt-0.0.5/cogsgpt/metas/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      316 2023-04-12 04:35:32.000000 cogsgpt-0.0.5/cogsgpt/metas/generate_response_presteps.json
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2861 2023-04-28 03:41:32.000000 cogsgpt-0.0.5/cogsgpt/metas/parse_task_presteps.json
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2047 2023-04-28 01:19:48.000000 cogsgpt-0.0.5/cogsgpt/metas/prompts.yaml
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     4718 2023-04-28 13:35:33.000000 cogsgpt-0.0.5/cogsgpt/metas/task_metas.yaml
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      369 2023-04-27 02:28:37.000000 cogsgpt-0.0.5/cogsgpt/schema.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      892 2023-04-24 07:01:19.000000 cogsgpt-0.0.5/cogsgpt/utils.py
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-29 15:12:37.901924 cogsgpt-0.0.5/cogsgpt.egg-info/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     7365 2023-04-29 15:12:37.000000 cogsgpt-0.0.5/cogsgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1261 2023-04-29 15:12:37.000000 cogsgpt-0.0.5/cogsgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)        1 2023-04-29 15:12:37.000000 cogsgpt-0.0.5/cogsgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      189 2023-04-29 15:12:37.000000 cogsgpt-0.0.5/cogsgpt.egg-info/requires.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)        8 2023-04-29 15:12:37.000000 cogsgpt-0.0.5/cogsgpt.egg-info/top_level.txt
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      932 2023-04-29 15:02:06.000000 cogsgpt-0.0.5/pyproject.toml
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)       38 2023-04-29 15:12:37.917924 cogsgpt-0.0.5/setup.cfg
+drwxrwxr-x   0 weitian   (1000) weitian   (1000)        0 2023-04-29 15:12:37.913924 cogsgpt-0.0.5/tests/
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1763 2023-04-28 13:14:29.000000 cogsgpt-0.0.5/tests/test_awesome_chat.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      550 2023-04-26 01:38:49.000000 cogsgpt-0.0.5/tests/test_bg_remove.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     2840 2023-04-27 02:44:47.000000 cogsgpt-0.0.5/tests/test_form_recognizer.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     4952 2023-04-27 01:52:52.000000 cogsgpt-0.0.5/tests/test_image_analisys.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)      602 2023-04-26 14:09:19.000000 cogsgpt-0.0.5/tests/test_speech.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1632 2023-04-26 14:18:48.000000 cogsgpt-0.0.5/tests/test_text_analysis.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1232 2023-04-28 03:12:51.000000 cogsgpt-0.0.5/tests/test_text_generation.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1971 2023-04-24 07:02:12.000000 cogsgpt-0.0.5/tests/test_text_summarize.py
+-rw-rw-r--   0 weitian   (1000) weitian   (1000)     1195 2023-04-27 04:15:40.000000 cogsgpt-0.0.5/tests/test_text_translation.py
```

### Comparing `cogsgpt-0.0.4/LICENSE` & `cogsgpt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/PKG-INFO` & `cogsgpt-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogsgpt
-Version: 0.0.4
+Version: 0.0.5
 Summary: A multi-modal LLM integrated ChatGPT with Azure Cognitive Service
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,46 +31,51 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CogsGPT
-A multi-modal LLM which integrates ChatGPT with Azure Cognitive Service.
+A conversational system which integrates ChatGPT with Azure Cognitive Services to achieve multimodal capabilities.
 
-**Now you can go to [CogsGPT on HuggingFace Space](https://huggingface.co/spaces/whiskyboy/CogsGPT) to experice the full capabilities of CogsGPT!!!**
-
-*If you find this repo useful, please consider giving it a star!*
-
-![](./docs/imgs/CogsGPT-demo.png)
+<a src="https://img.shields.io/badge/%F0%9F%A4%97-Open%20in%20Spaces-blue" href="https://huggingface.co/spaces/whiskyboy/CogsGPT">
+    <img src="https://img.shields.io/badge/%F0%9F%A4%97-Open%20in%20Spaces-blue" alt="Open in Spaces">
+</a>
+
+*If you find this repo useful, please consider giving it a star! :)*
+
+## Updates
+- [2023.04.28] **Now you can go to [CogsGPT on Hugging Face Space](https://huggingface.co/spaces/whiskyboy/CogsGPT) to experience the full capabilities of CogsGPT!!!** We are offering an Azure Cognitive Service resource for FREE to use in the demo. All you need is an OpenAI API key to get started chatting with CogsGPT!
+- [2023.04.25] CogsGPT now supports **image** type output! You can ask CogsGPT to crop a thumbnail of an image, or remove its background.
+- [2023.04.18] Release the first version of CogsGPT!
 
 ## Overview
 
 ### What is Azure Cognitive Service
 *(Answered by ChatGPT)*
 
 > Azure Cognitive Services is a collection of pre-built machine learning models that developers can use to add intelligent features to their applications without requiring extensive knowledge of data science or machine learning. These services include vision, speech, language, and decision-making capabilities, such as text translation, speech recognition, image recognition, and sentiment analysis. Azure Cognitive Services allows developers to quickly and easily incorporate advanced AI features into their applications, reducing the time and cost of building such features from scratch. It also provides enterprise-level security, scalability, and availability for applications that require high levels of reliability and performance.
 
 ### What is CogsGPT
-CogsGPT is a multi-modal LLM which utilizes the ChatGPT model as the controller and integrates with Azure Cognitive Services as collaborative executors to achieve multimodal capabilities to some extent. Using CogsGPT, you can simply access Azure Cognitive Services via natural language to process image or audio inputs, without any knowledge of the underlying APIs. You can even ask CogsGPT to perform some complex tasks such as summarizing a long speech into a short audio clip while retaining the main information. CogsGPT will automatically decide which services to use and how to use them to achieve the goal.
+CogsGPT is a conversational system which utilizes the ChatGPT model as the controller and integrates with Azure Cognitive Services as collaborative executors to achieve multimodal capabilities to some extent. Using CogsGPT, you can simply access Azure Cognitive Services via natural language to process image or audio inputs, without any knowledge of the underlying APIs. You can even ask CogsGPT to perform some complex tasks such as summarizing a long speech into a short audio clip while retaining the main information. CogsGPT will automatically decide which services to use and how to use them to achieve the goal.
 
-### How does it work
+### How does CogsGPT work
 
 The workflow of CogsGPT consists of three stages:
-1. Task Planing Stage: In this stage, CogsGPT will leverage ChatGPT to first think of the user's request carefully, and then parse it into a sequence of Cognitive Service tasks which have the most potentials to solve user's request. Each task may depend on the execution result of previous tasks.
-2. Task Execution Stage: In this stage, CogsGPT will execute the tasks one by one. The execution result will be stored for future reference.
+1. Task Planing Stage: In this stage, CogsGPT will leverage ChatGPT to parse user's input into a sequence of Azure Cognitive Service tasks which have the most potentials to solve user's request. Each task may depend on the execution result of previous tasks.
+2. Task Execution Stage: In this stage, CogsGPT will execute the tasks sequentially. The execution results will be stored for future reference.
 3. Response Generation Stage: In this stage, CogsGPT will leverage ChatGPT again to generate a final response to user's request based on the execution results of the second stage. The response may be a text, an image, an audio, or a combination of them.
 
 ## Getting Started
 
 ### Prerequisites
 
 - Python 3.8+
 - OpenAI API key
-- Azure Cognitive Multi-Service deployment ([How to deploy](https://learn.microsoft.com/en-us/azure/cognitive-services/cognitive-services-apis-create-account?tabs=multiservice%2Canomaly-detector%2Clanguage-service%2Ccomputer-vision%2Clinux#create-a-new-azure-cognitive-services-resource))
+- Azure Cognitive Multi-Services resource ([How to deploy](https://learn.microsoft.com/en-us/azure/cognitive-services/cognitive-services-apis-create-account?tabs=multiservice%2Canomaly-detector%2Clanguage-service%2Ccomputer-vision%2Clinux#create-a-new-azure-cognitive-services-resource))
 - Set the following environment variables:
     ```bash
     # OpenAI
     export OPENAI_API_TYPE="openai"
     export OPENAI_API_KEY="<OpenAI API Key>"
 
     # Azure Cognitive Service
@@ -91,29 +96,29 @@
 ```python
 from cogsgpt import CogsGPT
 
 agent = CogsGPT(model_name="gpt-3.5-turbo")
 agent.chat("What's the content in a.jpg?")
 ```
 
-For more details on the usage, please refer to the [API Reference](https://whiskyboy.github.io/cogsgpt/awesome_chat.html)
+For more details of the usage, please refer to the [API Reference](https://whiskyboy.github.io/cogsgpt/awesome_chat.html)
 
 ### Gradio Demo
 
-The CogsGPT Gradio demo is now available on [HuggingFace Space](https://huggingface.co/spaces/whiskyboy/CogsGPT)! To make it easier and more affordable to try out the capabilities of CogsGPT, we are offering an Azure Cognitive Service resource for FREE to use in the demo! All you need is an OpenAI API key to get started chatting with CogsGPT!
+The CogsGPT Gradio demo is now available on [Hugging Face Space](https://huggingface.co/spaces/whiskyboy/CogsGPT)! To make it easier and more affordable to try out the capabilities of CogsGPT, we are offering an Azure Cognitive Service resource for FREE to use in the demo! All you need is an OpenAI API key to get started chatting with CogsGPT!
 
-You can also use the following commands to run the demo locally with your own Azure Cognitive Service (Don't forget to set the environment variables first!):
+You can also use the following commands to run the demo locally with your own Azure Cognitive Service resources (Don't forget to set the environment variables first!):
 ```bash
 pip install gradio
 python app.py
 ```
 
 Now open your favorite browser and ENJOY YOUR CHAT!
 
-## Acknowledgments
+## Acknowledgment
 
 This project is inspired by [HuggingGPT](https://github.com/microsoft/JARVIS), and is built on top of [LangChain](https://github.com/hwchase17/langchain).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
```

### Comparing `cogsgpt-0.0.4/README.md` & `cogsgpt-0.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 # CogsGPT
-A multi-modal LLM which integrates ChatGPT with Azure Cognitive Service.
+A conversational system which integrates ChatGPT with Azure Cognitive Services to achieve multimodal capabilities.
 
-**Now you can go to [CogsGPT on HuggingFace Space](https://huggingface.co/spaces/whiskyboy/CogsGPT) to experice the full capabilities of CogsGPT!!!**
-
-*If you find this repo useful, please consider giving it a star!*
-
-![](./docs/imgs/CogsGPT-demo.png)
+<a src="https://img.shields.io/badge/%F0%9F%A4%97-Open%20in%20Spaces-blue" href="https://huggingface.co/spaces/whiskyboy/CogsGPT">
+    <img src="https://img.shields.io/badge/%F0%9F%A4%97-Open%20in%20Spaces-blue" alt="Open in Spaces">
+</a>
+
+*If you find this repo useful, please consider giving it a star! :)*
+
+## Updates
+- [2023.04.28] **Now you can go to [CogsGPT on Hugging Face Space](https://huggingface.co/spaces/whiskyboy/CogsGPT) to experience the full capabilities of CogsGPT!!!** We are offering an Azure Cognitive Service resource for FREE to use in the demo. All you need is an OpenAI API key to get started chatting with CogsGPT!
+- [2023.04.25] CogsGPT now supports **image** type output! You can ask CogsGPT to crop a thumbnail of an image, or remove its background.
+- [2023.04.18] Release the first version of CogsGPT!
 
 ## Overview
 
 ### What is Azure Cognitive Service
 *(Answered by ChatGPT)*
 
 > Azure Cognitive Services is a collection of pre-built machine learning models that developers can use to add intelligent features to their applications without requiring extensive knowledge of data science or machine learning. These services include vision, speech, language, and decision-making capabilities, such as text translation, speech recognition, image recognition, and sentiment analysis. Azure Cognitive Services allows developers to quickly and easily incorporate advanced AI features into their applications, reducing the time and cost of building such features from scratch. It also provides enterprise-level security, scalability, and availability for applications that require high levels of reliability and performance.
 
 ### What is CogsGPT
-CogsGPT is a multi-modal LLM which utilizes the ChatGPT model as the controller and integrates with Azure Cognitive Services as collaborative executors to achieve multimodal capabilities to some extent. Using CogsGPT, you can simply access Azure Cognitive Services via natural language to process image or audio inputs, without any knowledge of the underlying APIs. You can even ask CogsGPT to perform some complex tasks such as summarizing a long speech into a short audio clip while retaining the main information. CogsGPT will automatically decide which services to use and how to use them to achieve the goal.
+CogsGPT is a conversational system which utilizes the ChatGPT model as the controller and integrates with Azure Cognitive Services as collaborative executors to achieve multimodal capabilities to some extent. Using CogsGPT, you can simply access Azure Cognitive Services via natural language to process image or audio inputs, without any knowledge of the underlying APIs. You can even ask CogsGPT to perform some complex tasks such as summarizing a long speech into a short audio clip while retaining the main information. CogsGPT will automatically decide which services to use and how to use them to achieve the goal.
 
-### How does it work
+### How does CogsGPT work
 
 The workflow of CogsGPT consists of three stages:
-1. Task Planing Stage: In this stage, CogsGPT will leverage ChatGPT to first think of the user's request carefully, and then parse it into a sequence of Cognitive Service tasks which have the most potentials to solve user's request. Each task may depend on the execution result of previous tasks.
-2. Task Execution Stage: In this stage, CogsGPT will execute the tasks one by one. The execution result will be stored for future reference.
+1. Task Planing Stage: In this stage, CogsGPT will leverage ChatGPT to parse user's input into a sequence of Azure Cognitive Service tasks which have the most potentials to solve user's request. Each task may depend on the execution result of previous tasks.
+2. Task Execution Stage: In this stage, CogsGPT will execute the tasks sequentially. The execution results will be stored for future reference.
 3. Response Generation Stage: In this stage, CogsGPT will leverage ChatGPT again to generate a final response to user's request based on the execution results of the second stage. The response may be a text, an image, an audio, or a combination of them.
 
 ## Getting Started
 
 ### Prerequisites
 
 - Python 3.8+
 - OpenAI API key
-- Azure Cognitive Multi-Service deployment ([How to deploy](https://learn.microsoft.com/en-us/azure/cognitive-services/cognitive-services-apis-create-account?tabs=multiservice%2Canomaly-detector%2Clanguage-service%2Ccomputer-vision%2Clinux#create-a-new-azure-cognitive-services-resource))
+- Azure Cognitive Multi-Services resource ([How to deploy](https://learn.microsoft.com/en-us/azure/cognitive-services/cognitive-services-apis-create-account?tabs=multiservice%2Canomaly-detector%2Clanguage-service%2Ccomputer-vision%2Clinux#create-a-new-azure-cognitive-services-resource))
 - Set the following environment variables:
     ```bash
     # OpenAI
     export OPENAI_API_TYPE="openai"
     export OPENAI_API_KEY="<OpenAI API Key>"
 
     # Azure Cognitive Service
@@ -55,36 +60,36 @@
 ```python
 from cogsgpt import CogsGPT
 
 agent = CogsGPT(model_name="gpt-3.5-turbo")
 agent.chat("What's the content in a.jpg?")
 ```
 
-For more details on the usage, please refer to the [API Reference](https://whiskyboy.github.io/cogsgpt/awesome_chat.html)
+For more details of the usage, please refer to the [API Reference](https://whiskyboy.github.io/cogsgpt/awesome_chat.html)
 
 ### Gradio Demo
 
-The CogsGPT Gradio demo is now available on [HuggingFace Space](https://huggingface.co/spaces/whiskyboy/CogsGPT)! To make it easier and more affordable to try out the capabilities of CogsGPT, we are offering an Azure Cognitive Service resource for FREE to use in the demo! All you need is an OpenAI API key to get started chatting with CogsGPT!
+The CogsGPT Gradio demo is now available on [Hugging Face Space](https://huggingface.co/spaces/whiskyboy/CogsGPT)! To make it easier and more affordable to try out the capabilities of CogsGPT, we are offering an Azure Cognitive Service resource for FREE to use in the demo! All you need is an OpenAI API key to get started chatting with CogsGPT!
 
-You can also use the following commands to run the demo locally with your own Azure Cognitive Service (Don't forget to set the environment variables first!):
+You can also use the following commands to run the demo locally with your own Azure Cognitive Service resources (Don't forget to set the environment variables first!):
 ```bash
 pip install gradio
 python app.py
 ```
 
 Now open your favorite browser and ENJOY YOUR CHAT!
 
-## Acknowledgments
+## Acknowledgment
 
 This project is inspired by [HuggingGPT](https://github.com/microsoft/JARVIS), and is built on top of [LangChain](https://github.com/hwchase17/langchain).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
 
 ## Contributing
 
 As an open source project, we welcome contributions and suggestions. Please follow the [fork and pull request](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) workflow to contribute to this project. Please do not try to push directly to this repo unless you are maintainer.
 
 ## Contact
 
-If you have any questions, please feel free to contact us via <weitian.bnu@gmail.com>
+If you have any questions, please feel free to contact us via <weitian.bnu@gmail.com>
```

### Comparing `cogsgpt-0.0.4/cogsgpt/awesome_chat.py` & `cogsgpt-0.0.5/cogsgpt/awesome_chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,35 +154,38 @@
                        system_prompt: str = "", system_prompt_vars: List[str] = [],
                        user_prompt: str = "", user_prompt_vars: List[str] = [], 
                        presteps: List[Dict] = [], presteps_vars: List[str] = []) -> ChatPromptTemplate:
         system_message_prompt = SystemMessagePromptTemplate(
             prompt=PromptTemplate(
                 template=system_prompt,
                 input_variables=system_prompt_vars,
-                template_format="jinja2"
+                template_format="jinja2",
+                validate_template=False
             )
         )
 
         human_message_prompt = HumanMessagePromptTemplate(
             prompt=PromptTemplate(
                 template=user_prompt,
                 input_variables=user_prompt_vars,
-                template_format="jinja2"
+                template_format="jinja2",
+                validate_template=False
             )
         )
 
         presteps_message_prompts = []
         for prestep in presteps:
             role_message_prompt_template = AIMessagePromptTemplate if prestep["role"] == "assistant" else HumanMessagePromptTemplate
             presteps_message_prompts.append(
                 role_message_prompt_template(
                     prompt=PromptTemplate(
                         template=prestep["content"],
                         input_variables=presteps_vars,
-                        template_format="jinja2"
+                        template_format="jinja2",
+                        validate_template=False
                     )
                 )
             )
 
         return ChatPromptTemplate.from_messages([system_message_prompt, *presteps_message_prompts, human_message_prompt])
 
     def _format_parse_task_prompt(self, human_input: str) -> PromptValue:
```

### Comparing `cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/__init__.py` & `cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/__init__.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/background_remover.py` & `cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/background_remover.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/form_recognizer.py` & `cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/form_recognizer.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/image_analysis_v3.py` & `cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/image_analysis_v3.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/image_analysis_v4.py` & `cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/image_analysis_v4.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/cogsgpt/cogsmodel/cv/utils.py` & `cogsgpt-0.0.5/cogsgpt/cogsmodel/cv/utils.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/__init__.py` & `cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/text_analysis.py` & `cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/text_analysis.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/text_generation.py` & `cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/text_generation.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/text_summarize.py` & `cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/text_summarize.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/cogsgpt/cogsmodel/nlp/text_translation.py` & `cogsgpt-0.0.5/cogsgpt/cogsmodel/nlp/text_translation.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/cogsgpt/cogsmodel/speech/speech.py` & `cogsgpt-0.0.5/cogsgpt/cogsmodel/speech/speech.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/cogsgpt/llm.py` & `cogsgpt-0.0.5/cogsgpt/llm.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/cogsgpt/metas/parse_task_presteps.json` & `cogsgpt-0.0.5/cogsgpt/metas/parse_task_presteps.json`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/cogsgpt/metas/prompts.yaml` & `cogsgpt-0.0.5/cogsgpt/metas/prompts.yaml`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/cogsgpt/metas/task_metas.yaml` & `cogsgpt-0.0.5/cogsgpt/metas/task_metas.yaml`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/cogsgpt/utils.py` & `cogsgpt-0.0.5/cogsgpt/utils.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/cogsgpt.egg-info/PKG-INFO` & `cogsgpt-0.0.5/cogsgpt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogsgpt
-Version: 0.0.4
+Version: 0.0.5
 Summary: A multi-modal LLM integrated ChatGPT with Azure Cognitive Service
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,46 +31,51 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CogsGPT
-A multi-modal LLM which integrates ChatGPT with Azure Cognitive Service.
+A conversational system which integrates ChatGPT with Azure Cognitive Services to achieve multimodal capabilities.
 
-**Now you can go to [CogsGPT on HuggingFace Space](https://huggingface.co/spaces/whiskyboy/CogsGPT) to experice the full capabilities of CogsGPT!!!**
-
-*If you find this repo useful, please consider giving it a star!*
-
-![](./docs/imgs/CogsGPT-demo.png)
+<a src="https://img.shields.io/badge/%F0%9F%A4%97-Open%20in%20Spaces-blue" href="https://huggingface.co/spaces/whiskyboy/CogsGPT">
+    <img src="https://img.shields.io/badge/%F0%9F%A4%97-Open%20in%20Spaces-blue" alt="Open in Spaces">
+</a>
+
+*If you find this repo useful, please consider giving it a star! :)*
+
+## Updates
+- [2023.04.28] **Now you can go to [CogsGPT on Hugging Face Space](https://huggingface.co/spaces/whiskyboy/CogsGPT) to experience the full capabilities of CogsGPT!!!** We are offering an Azure Cognitive Service resource for FREE to use in the demo. All you need is an OpenAI API key to get started chatting with CogsGPT!
+- [2023.04.25] CogsGPT now supports **image** type output! You can ask CogsGPT to crop a thumbnail of an image, or remove its background.
+- [2023.04.18] Release the first version of CogsGPT!
 
 ## Overview
 
 ### What is Azure Cognitive Service
 *(Answered by ChatGPT)*
 
 > Azure Cognitive Services is a collection of pre-built machine learning models that developers can use to add intelligent features to their applications without requiring extensive knowledge of data science or machine learning. These services include vision, speech, language, and decision-making capabilities, such as text translation, speech recognition, image recognition, and sentiment analysis. Azure Cognitive Services allows developers to quickly and easily incorporate advanced AI features into their applications, reducing the time and cost of building such features from scratch. It also provides enterprise-level security, scalability, and availability for applications that require high levels of reliability and performance.
 
 ### What is CogsGPT
-CogsGPT is a multi-modal LLM which utilizes the ChatGPT model as the controller and integrates with Azure Cognitive Services as collaborative executors to achieve multimodal capabilities to some extent. Using CogsGPT, you can simply access Azure Cognitive Services via natural language to process image or audio inputs, without any knowledge of the underlying APIs. You can even ask CogsGPT to perform some complex tasks such as summarizing a long speech into a short audio clip while retaining the main information. CogsGPT will automatically decide which services to use and how to use them to achieve the goal.
+CogsGPT is a conversational system which utilizes the ChatGPT model as the controller and integrates with Azure Cognitive Services as collaborative executors to achieve multimodal capabilities to some extent. Using CogsGPT, you can simply access Azure Cognitive Services via natural language to process image or audio inputs, without any knowledge of the underlying APIs. You can even ask CogsGPT to perform some complex tasks such as summarizing a long speech into a short audio clip while retaining the main information. CogsGPT will automatically decide which services to use and how to use them to achieve the goal.
 
-### How does it work
+### How does CogsGPT work
 
 The workflow of CogsGPT consists of three stages:
-1. Task Planing Stage: In this stage, CogsGPT will leverage ChatGPT to first think of the user's request carefully, and then parse it into a sequence of Cognitive Service tasks which have the most potentials to solve user's request. Each task may depend on the execution result of previous tasks.
-2. Task Execution Stage: In this stage, CogsGPT will execute the tasks one by one. The execution result will be stored for future reference.
+1. Task Planing Stage: In this stage, CogsGPT will leverage ChatGPT to parse user's input into a sequence of Azure Cognitive Service tasks which have the most potentials to solve user's request. Each task may depend on the execution result of previous tasks.
+2. Task Execution Stage: In this stage, CogsGPT will execute the tasks sequentially. The execution results will be stored for future reference.
 3. Response Generation Stage: In this stage, CogsGPT will leverage ChatGPT again to generate a final response to user's request based on the execution results of the second stage. The response may be a text, an image, an audio, or a combination of them.
 
 ## Getting Started
 
 ### Prerequisites
 
 - Python 3.8+
 - OpenAI API key
-- Azure Cognitive Multi-Service deployment ([How to deploy](https://learn.microsoft.com/en-us/azure/cognitive-services/cognitive-services-apis-create-account?tabs=multiservice%2Canomaly-detector%2Clanguage-service%2Ccomputer-vision%2Clinux#create-a-new-azure-cognitive-services-resource))
+- Azure Cognitive Multi-Services resource ([How to deploy](https://learn.microsoft.com/en-us/azure/cognitive-services/cognitive-services-apis-create-account?tabs=multiservice%2Canomaly-detector%2Clanguage-service%2Ccomputer-vision%2Clinux#create-a-new-azure-cognitive-services-resource))
 - Set the following environment variables:
     ```bash
     # OpenAI
     export OPENAI_API_TYPE="openai"
     export OPENAI_API_KEY="<OpenAI API Key>"
 
     # Azure Cognitive Service
@@ -91,29 +96,29 @@
 ```python
 from cogsgpt import CogsGPT
 
 agent = CogsGPT(model_name="gpt-3.5-turbo")
 agent.chat("What's the content in a.jpg?")
 ```
 
-For more details on the usage, please refer to the [API Reference](https://whiskyboy.github.io/cogsgpt/awesome_chat.html)
+For more details of the usage, please refer to the [API Reference](https://whiskyboy.github.io/cogsgpt/awesome_chat.html)
 
 ### Gradio Demo
 
-The CogsGPT Gradio demo is now available on [HuggingFace Space](https://huggingface.co/spaces/whiskyboy/CogsGPT)! To make it easier and more affordable to try out the capabilities of CogsGPT, we are offering an Azure Cognitive Service resource for FREE to use in the demo! All you need is an OpenAI API key to get started chatting with CogsGPT!
+The CogsGPT Gradio demo is now available on [Hugging Face Space](https://huggingface.co/spaces/whiskyboy/CogsGPT)! To make it easier and more affordable to try out the capabilities of CogsGPT, we are offering an Azure Cognitive Service resource for FREE to use in the demo! All you need is an OpenAI API key to get started chatting with CogsGPT!
 
-You can also use the following commands to run the demo locally with your own Azure Cognitive Service (Don't forget to set the environment variables first!):
+You can also use the following commands to run the demo locally with your own Azure Cognitive Service resources (Don't forget to set the environment variables first!):
 ```bash
 pip install gradio
 python app.py
 ```
 
 Now open your favorite browser and ENJOY YOUR CHAT!
 
-## Acknowledgments
+## Acknowledgment
 
 This project is inspired by [HuggingGPT](https://github.com/microsoft/JARVIS), and is built on top of [LangChain](https://github.com/hwchase17/langchain).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
```

### Comparing `cogsgpt-0.0.4/cogsgpt.egg-info/SOURCES.txt` & `cogsgpt-0.0.5/cogsgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/pyproject.toml` & `cogsgpt-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cogsgpt"
-version = "0.0.4"
+version = "0.0.5"
 description = "A multi-modal LLM integrated ChatGPT with Azure Cognitive Service"
 readme = "README.md"
 authors = [{ name = "weitian", email = "weitian.bnu@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["chatgpt", "cognitive service", "llm"]
 dependencies = [
     "azure-ai-vision",
     "azure-cognitiveservices-vision-computervision",
     "azure-ai-formrecognizer",
-    "azure-ai-textanalytics == 5.3.0b1",
+    "azure-ai-textanalytics==5.3.0b1",
     "azure-cognitiveservices-speech",
     "colorlog",
     "jinja2",
     "langchain",
     "openai",
     "pillow",
 ]
```

### Comparing `cogsgpt-0.0.4/tests/test_awesome_chat.py` & `cogsgpt-0.0.5/tests/test_awesome_chat.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/tests/test_bg_remove.py` & `cogsgpt-0.0.5/tests/test_bg_remove.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/tests/test_form_recognizer.py` & `cogsgpt-0.0.5/tests/test_form_recognizer.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/tests/test_image_analisys.py` & `cogsgpt-0.0.5/tests/test_image_analisys.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/tests/test_speech.py` & `cogsgpt-0.0.5/tests/test_speech.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/tests/test_text_analysis.py` & `cogsgpt-0.0.5/tests/test_text_analysis.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/tests/test_text_generation.py` & `cogsgpt-0.0.5/tests/test_text_generation.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/tests/test_text_summarize.py` & `cogsgpt-0.0.5/tests/test_text_summarize.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-0.0.4/tests/test_text_translation.py` & `cogsgpt-0.0.5/tests/test_text_translation.py`

 * *Files identical despite different names*


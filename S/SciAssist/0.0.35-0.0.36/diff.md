# Comparing `tmp/SciAssist-0.0.35.tar.gz` & `tmp/SciAssist-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SciAssist-0.0.35.tar", last modified: Sat Apr 29 15:41:22 2023, max compression
+gzip compressed data, was "SciAssist-0.0.36.tar", last modified: Sat Apr 29 16:26:43 2023, max compression
```

## Comparing `SciAssist-0.0.35.tar` & `SciAssist-0.0.36.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.491485 SciAssist-0.0.35/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    21150 2022-09-28 02:29:12.000000 SciAssist-0.0.35/LICENSE
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       38 2022-09-28 02:29:12.000000 SciAssist-0.0.35/MANIFEST.in
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-29 15:41:22.491485 SciAssist-0.0.35/PKG-INFO
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6208 2022-11-05 13:55:02.000000 SciAssist-0.0.35/README.md
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1451 2023-04-29 15:40:48.000000 SciAssist-0.0.35/pyproject.toml
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      635 2023-04-29 15:41:22.491485 SciAssist-0.0.35/setup.cfg
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       96 2022-09-28 02:29:12.000000 SciAssist-0.0.35/setup.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.483485 SciAssist-0.0.35/src/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.483485 SciAssist-0.0.35/src/SciAssist/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      818 2023-04-14 07:10:04.000000 SciAssist-0.0.35/src/SciAssist/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.487485 SciAssist-0.0.35/src/SciAssist/bin/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      668 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.487485 SciAssist-0.0.35/src/SciAssist/bin/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      916 2023-03-15 13:25:23.000000 SciAssist-0.0.35/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.487485 SciAssist-0.0.35/src/SciAssist/bin/doc2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    11558 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/LICENSE
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.487485 SciAssist-0.0.35/src/SciAssist/bin/doc2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      158 2023-03-15 13:25:23.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/__pycache__/__init__.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.487485 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.487485 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      167 2023-03-15 13:25:23.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      227 2023-03-15 13:25:23.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/__pycache__/config.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    15546 2023-03-15 13:25:23.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       59 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/config.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.487485 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.487485 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      179 2023-03-15 13:25:23.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2874 2023-03-15 13:25:23.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    15434 2023-03-15 13:25:23.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.487485 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4449 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.487485 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      186 2023-03-15 13:25:23.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6183 2023-03-15 13:25:23.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5972 2023-03-15 13:25:23.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6614 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1019 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2736 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     9058 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        8 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/pdf_to_tei.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3622 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    27209 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    16382 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/s2orc.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.487485 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.487485 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      173 2023-03-15 13:25:23.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2743 2023-03-15 13:25:23.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     8839 2023-03-15 13:25:23.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3531 2023-03-15 13:25:23.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3144 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    11737 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6935 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4235 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      585 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.487485 SciAssist-0.0.35/src/SciAssist/bin/doc2json/scripts/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       73 2022-10-04 11:07:26.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/scripts/run_grobid_linux.sh
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      751 2022-10-04 11:09:22.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      275 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/bin/doc2json/setup.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.491485 SciAssist-0.0.35/src/SciAssist/datamodules/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/datamodules/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4113 2023-03-26 03:08:44.000000 SciAssist-0.0.35/src/SciAssist/datamodules/acl_datamodule.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.491485 SciAssist-0.0.35/src/SciAssist/datamodules/components/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/datamodules/components/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      370 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/datamodules/components/cora_label.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3112 2022-11-05 13:55:02.000000 SciAssist-0.0.35/src/SciAssist/datamodules/cora_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3357 2023-04-14 07:10:04.000000 SciAssist-0.0.35/src/SciAssist/datamodules/dataset_extraction_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3198 2022-11-10 14:45:14.000000 SciAssist-0.0.35/src/SciAssist/datamodules/fid_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2948 2022-11-27 14:04:32.000000 SciAssist-0.0.35/src/SciAssist/datamodules/general_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4331 2022-12-14 08:45:15.000000 SciAssist-0.0.35/src/SciAssist/datamodules/longsumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3179 2023-04-02 03:32:15.000000 SciAssist-0.0.35/src/SciAssist/datamodules/mup_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     7753 2023-03-18 16:34:11.000000 SciAssist-0.0.35/src/SciAssist/datamodules/mup_mup_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6862 2023-04-29 14:42:50.000000 SciAssist-0.0.35/src/SciAssist/datamodules/mup_scisumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5991 2023-04-25 15:59:38.000000 SciAssist-0.0.35/src/SciAssist/datamodules/mup_scisumm_noctrl_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5865 2023-04-14 07:09:42.000000 SciAssist-0.0.35/src/SciAssist/datamodules/scisumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4850 2023-02-23 16:55:34.000000 SciAssist-0.0.35/src/SciAssist/datamodules/test_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4211 2022-12-18 15:08:30.000000 SciAssist-0.0.35/src/SciAssist/datamodules/xsum_datamodule.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.491485 SciAssist-0.0.35/src/SciAssist/models/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/models/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.491485 SciAssist-0.0.35/src/SciAssist/models/components/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/models/components/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1554 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/models/components/bart_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2845 2023-04-14 07:10:04.000000 SciAssist-0.0.35/src/SciAssist/models/components/bert_dataset_extraction.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1547 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/models/components/bert_token_classifier.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1728 2023-04-17 15:52:16.000000 SciAssist-0.0.35/src/SciAssist/models/components/flant5_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6869 2022-11-19 15:12:24.000000 SciAssist-0.0.35/src/SciAssist/models/cora_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     8632 2023-04-14 07:10:04.000000 SciAssist-0.0.35/src/SciAssist/models/dataset_extraction_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    13319 2023-04-02 03:32:15.000000 SciAssist-0.0.35/src/SciAssist/models/mup_bart_module.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.491485 SciAssist-0.0.35/src/SciAssist/pipelines/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3876 2023-04-26 07:13:45.000000 SciAssist-0.0.35/src/SciAssist/pipelines/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    12872 2023-04-14 07:10:04.000000 SciAssist-0.0.35/src/SciAssist/pipelines/dataset_extraction.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2056 2022-11-05 13:55:02.000000 SciAssist-0.0.35/src/SciAssist/pipelines/pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    13826 2022-11-05 13:55:02.000000 SciAssist-0.0.35/src/SciAssist/pipelines/reference_string_parsing.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    14045 2023-04-29 14:44:31.000000 SciAssist-0.0.35/src/SciAssist/pipelines/summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1950 2023-02-20 05:27:12.000000 SciAssist-0.0.35/src/SciAssist/pipelines/testing_pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4003 2022-11-05 13:55:02.000000 SciAssist-0.0.35/src/SciAssist/pipelines/training_pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      786 2022-09-28 02:29:12.000000 SciAssist-0.0.35/src/SciAssist/test.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2022-10-02 15:49:40.000000 SciAssist-0.0.35/src/SciAssist/train.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2852 2022-11-27 16:49:31.000000 SciAssist-0.0.35/src/SciAssist/training_args.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.491485 SciAssist-0.0.35/src/SciAssist/utils/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4733 2023-02-03 14:21:07.000000 SciAssist-0.0.35/src/SciAssist/utils/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.491485 SciAssist-0.0.35/src/SciAssist/utils/collators/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2323 2022-11-10 14:30:40.000000 SciAssist-0.0.35/src/SciAssist/utils/collators/CollatorForFid.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-11-06 14:22:00.000000 SciAssist-0.0.35/src/SciAssist/utils/collators/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1232 2023-01-11 16:34:32.000000 SciAssist-0.0.35/src/SciAssist/utils/data_reader.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    53624 2023-04-29 14:37:32.000000 SciAssist-0.0.35/src/SciAssist/utils/data_utils.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2899 2023-04-22 06:46:59.000000 SciAssist-0.0.35/src/SciAssist/utils/extract_keywords_flant5.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5722 2023-04-22 06:20:33.000000 SciAssist-0.0.35/src/SciAssist/utils/pdf2text.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2423 2023-04-29 15:40:40.000000 SciAssist-0.0.35/src/SciAssist/utils/windows_pdf2text.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.483485 SciAssist-0.0.35/src/SciAssist.egg-info/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-29 15:41:22.000000 SciAssist-0.0.35/src/SciAssist.egg-info/PKG-INFO
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4822 2023-04-29 15:41:22.000000 SciAssist-0.0.35/src/SciAssist.egg-info/SOURCES.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        1 2023-04-29 15:41:22.000000 SciAssist-0.0.35/src/SciAssist.egg-info/dependency_links.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       98 2023-04-29 15:41:22.000000 SciAssist-0.0.35/src/SciAssist.egg-info/entry_points.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      396 2023-04-29 15:41:22.000000 SciAssist-0.0.35/src/SciAssist.egg-info/requires.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       34 2023-04-29 15:41:22.000000 SciAssist-0.0.35/src/SciAssist.egg-info/top_level.txt
--rwxrwxr-x   0 yixi      (1025) yixi      (1027)      690 2022-12-10 17:44:58.000000 SciAssist-0.0.35/src/process.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 15:41:22.491485 SciAssist-0.0.35/tests/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1095 2022-12-11 12:29:46.000000 SciAssist-0.0.35/tests/test_rsp.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1129 2022-12-11 12:29:46.000000 SciAssist-0.0.35/tests/test_summ.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.164286 SciAssist-0.0.36/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    21150 2022-09-28 02:29:12.000000 SciAssist-0.0.36/LICENSE
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       38 2022-09-28 02:29:12.000000 SciAssist-0.0.36/MANIFEST.in
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-29 16:26:43.164286 SciAssist-0.0.36/PKG-INFO
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6208 2022-11-05 13:55:02.000000 SciAssist-0.0.36/README.md
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1451 2023-04-29 16:26:23.000000 SciAssist-0.0.36/pyproject.toml
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      635 2023-04-29 16:26:43.164286 SciAssist-0.0.36/setup.cfg
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       96 2022-09-28 02:29:12.000000 SciAssist-0.0.36/setup.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.156285 SciAssist-0.0.36/src/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.156285 SciAssist-0.0.36/src/SciAssist/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      818 2023-04-14 07:10:04.000000 SciAssist-0.0.36/src/SciAssist/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.156285 SciAssist-0.0.36/src/SciAssist/bin/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      668 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.156285 SciAssist-0.0.36/src/SciAssist/bin/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      916 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.156285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    11558 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/LICENSE
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.156285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      158 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/__pycache__/__init__.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.156285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      167 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      227 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/__pycache__/config.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    15546 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       59 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/config.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      179 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2874 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    15434 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4449 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      186 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6183 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5972 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6614 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1019 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2736 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     9058 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        8 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/pdf_to_tei.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3622 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    27209 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    16382 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/s2orc.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      173 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2743 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     8839 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3531 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3144 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    11737 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6935 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4235 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      585 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/scripts/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       73 2022-10-04 11:07:26.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/scripts/run_grobid_linux.sh
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      751 2022-10-04 11:09:22.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      275 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/setup.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/datamodules/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/datamodules/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4113 2023-03-26 03:08:44.000000 SciAssist-0.0.36/src/SciAssist/datamodules/acl_datamodule.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/datamodules/components/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/datamodules/components/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      370 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/datamodules/components/cora_label.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3112 2022-11-05 13:55:02.000000 SciAssist-0.0.36/src/SciAssist/datamodules/cora_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3357 2023-04-14 07:10:04.000000 SciAssist-0.0.36/src/SciAssist/datamodules/dataset_extraction_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3198 2022-11-10 14:45:14.000000 SciAssist-0.0.36/src/SciAssist/datamodules/fid_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2948 2022-11-27 14:04:32.000000 SciAssist-0.0.36/src/SciAssist/datamodules/general_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4331 2022-12-14 08:45:15.000000 SciAssist-0.0.36/src/SciAssist/datamodules/longsumm_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3179 2023-04-02 03:32:15.000000 SciAssist-0.0.36/src/SciAssist/datamodules/mup_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     7753 2023-03-18 16:34:11.000000 SciAssist-0.0.36/src/SciAssist/datamodules/mup_mup_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6862 2023-04-29 14:42:50.000000 SciAssist-0.0.36/src/SciAssist/datamodules/mup_scisumm_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5991 2023-04-25 15:59:38.000000 SciAssist-0.0.36/src/SciAssist/datamodules/mup_scisumm_noctrl_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5865 2023-04-14 07:09:42.000000 SciAssist-0.0.36/src/SciAssist/datamodules/scisumm_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4850 2023-02-23 16:55:34.000000 SciAssist-0.0.36/src/SciAssist/datamodules/test_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4211 2022-12-18 15:08:30.000000 SciAssist-0.0.36/src/SciAssist/datamodules/xsum_datamodule.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.164286 SciAssist-0.0.36/src/SciAssist/models/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/models/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.164286 SciAssist-0.0.36/src/SciAssist/models/components/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/models/components/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1554 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/models/components/bart_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2845 2023-04-14 07:10:04.000000 SciAssist-0.0.36/src/SciAssist/models/components/bert_dataset_extraction.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1547 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/models/components/bert_token_classifier.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1728 2023-04-17 15:52:16.000000 SciAssist-0.0.36/src/SciAssist/models/components/flant5_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6869 2022-11-19 15:12:24.000000 SciAssist-0.0.36/src/SciAssist/models/cora_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     8632 2023-04-14 07:10:04.000000 SciAssist-0.0.36/src/SciAssist/models/dataset_extraction_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    13319 2023-04-02 03:32:15.000000 SciAssist-0.0.36/src/SciAssist/models/mup_bart_module.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.164286 SciAssist-0.0.36/src/SciAssist/pipelines/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3876 2023-04-26 07:13:45.000000 SciAssist-0.0.36/src/SciAssist/pipelines/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    12872 2023-04-14 07:10:04.000000 SciAssist-0.0.36/src/SciAssist/pipelines/dataset_extraction.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2056 2022-11-05 13:55:02.000000 SciAssist-0.0.36/src/SciAssist/pipelines/pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    13826 2022-11-05 13:55:02.000000 SciAssist-0.0.36/src/SciAssist/pipelines/reference_string_parsing.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    14045 2023-04-29 14:44:31.000000 SciAssist-0.0.36/src/SciAssist/pipelines/summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1950 2023-02-20 05:27:12.000000 SciAssist-0.0.36/src/SciAssist/pipelines/testing_pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4003 2022-11-05 13:55:02.000000 SciAssist-0.0.36/src/SciAssist/pipelines/training_pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      786 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/test.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2022-10-02 15:49:40.000000 SciAssist-0.0.36/src/SciAssist/train.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2852 2022-11-27 16:49:31.000000 SciAssist-0.0.36/src/SciAssist/training_args.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.164286 SciAssist-0.0.36/src/SciAssist/utils/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4733 2023-02-03 14:21:07.000000 SciAssist-0.0.36/src/SciAssist/utils/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.164286 SciAssist-0.0.36/src/SciAssist/utils/collators/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2323 2022-11-10 14:30:40.000000 SciAssist-0.0.36/src/SciAssist/utils/collators/CollatorForFid.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-11-06 14:22:00.000000 SciAssist-0.0.36/src/SciAssist/utils/collators/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1232 2023-01-11 16:34:32.000000 SciAssist-0.0.36/src/SciAssist/utils/data_reader.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    53624 2023-04-29 14:37:32.000000 SciAssist-0.0.36/src/SciAssist/utils/data_utils.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2899 2023-04-22 06:46:59.000000 SciAssist-0.0.36/src/SciAssist/utils/extract_keywords_flant5.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5722 2023-04-22 06:20:33.000000 SciAssist-0.0.36/src/SciAssist/utils/pdf2text.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2432 2023-04-29 16:24:14.000000 SciAssist-0.0.36/src/SciAssist/utils/windows_pdf2text.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.156285 SciAssist-0.0.36/src/SciAssist.egg-info/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-29 16:26:43.000000 SciAssist-0.0.36/src/SciAssist.egg-info/PKG-INFO
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4822 2023-04-29 16:26:43.000000 SciAssist-0.0.36/src/SciAssist.egg-info/SOURCES.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        1 2023-04-29 16:26:43.000000 SciAssist-0.0.36/src/SciAssist.egg-info/dependency_links.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       98 2023-04-29 16:26:43.000000 SciAssist-0.0.36/src/SciAssist.egg-info/entry_points.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      396 2023-04-29 16:26:43.000000 SciAssist-0.0.36/src/SciAssist.egg-info/requires.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       34 2023-04-29 16:26:43.000000 SciAssist-0.0.36/src/SciAssist.egg-info/top_level.txt
+-rwxrwxr-x   0 yixi      (1025) yixi      (1027)      690 2022-12-10 17:44:58.000000 SciAssist-0.0.36/src/process.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.164286 SciAssist-0.0.36/tests/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1095 2022-12-11 12:29:46.000000 SciAssist-0.0.36/tests/test_rsp.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1129 2022-12-11 12:29:46.000000 SciAssist-0.0.36/tests/test_summ.py
```

### Comparing `SciAssist-0.0.35/LICENSE` & `SciAssist-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/PKG-INFO` & `SciAssist-0.0.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciAssist
-Version: 0.0.35
+Version: 0.0.36
 Summary: A toolkit for Scientific Document Processing
 Author-email: WING-NUS <dingyixi@hotmail.com>
 Maintainer-email: Yixi Ding <dingyixi@hotmail.com>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
```

### Comparing `SciAssist-0.0.35/README.md` & `SciAssist-0.0.36/README.md`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/pyproject.toml` & `SciAssist-0.0.36/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SciAssist"
-version = "0.0.35"
+version = "0.0.36"
 authors = [
   { name="WING-NUS", email="dingyixi@hotmail.com" },
 ]
 maintainers = [
   { name="Yixi Ding", email="dingyixi@hotmail.com" },
 ]
 description = "A toolkit for Scientific Document Processing"
```

### Comparing `SciAssist-0.0.35/setup.cfg` & `SciAssist-0.0.36/setup.cfg`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/__init__.py` & `SciAssist-0.0.36/src/SciAssist/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/__init__.py` & `SciAssist-0.0.36/src/SciAssist/bin/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc` & `SciAssist-0.0.36/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/LICENSE` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/LICENSE`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/s2orc.py` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/s2orc.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh` & `SciAssist-0.0.36/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/datamodules/acl_datamodule.py` & `SciAssist-0.0.36/src/SciAssist/datamodules/acl_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/datamodules/cora_datamodule.py` & `SciAssist-0.0.36/src/SciAssist/datamodules/cora_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/datamodules/dataset_extraction_datamodule.py` & `SciAssist-0.0.36/src/SciAssist/datamodules/dataset_extraction_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/datamodules/fid_datamodule.py` & `SciAssist-0.0.36/src/SciAssist/datamodules/fid_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/datamodules/general_datamodule.py` & `SciAssist-0.0.36/src/SciAssist/datamodules/general_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/datamodules/longsumm_datamodule.py` & `SciAssist-0.0.36/src/SciAssist/datamodules/longsumm_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/datamodules/mup_datamodule.py` & `SciAssist-0.0.36/src/SciAssist/datamodules/mup_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/datamodules/mup_mup_datamodule.py` & `SciAssist-0.0.36/src/SciAssist/datamodules/mup_mup_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/datamodules/mup_scisumm_datamodule.py` & `SciAssist-0.0.36/src/SciAssist/datamodules/mup_scisumm_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/datamodules/mup_scisumm_noctrl_datamodule.py` & `SciAssist-0.0.36/src/SciAssist/datamodules/mup_scisumm_noctrl_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/datamodules/scisumm_datamodule.py` & `SciAssist-0.0.36/src/SciAssist/datamodules/scisumm_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/datamodules/test_datamodule.py` & `SciAssist-0.0.36/src/SciAssist/datamodules/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/datamodules/xsum_datamodule.py` & `SciAssist-0.0.36/src/SciAssist/datamodules/xsum_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/models/components/bart_summarization.py` & `SciAssist-0.0.36/src/SciAssist/models/components/bart_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/models/components/bert_dataset_extraction.py` & `SciAssist-0.0.36/src/SciAssist/models/components/bert_dataset_extraction.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/models/components/bert_token_classifier.py` & `SciAssist-0.0.36/src/SciAssist/models/components/bert_token_classifier.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/models/components/flant5_summarization.py` & `SciAssist-0.0.36/src/SciAssist/models/components/flant5_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/models/cora_module.py` & `SciAssist-0.0.36/src/SciAssist/models/cora_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/models/dataset_extraction_module.py` & `SciAssist-0.0.36/src/SciAssist/models/dataset_extraction_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/models/mup_bart_module.py` & `SciAssist-0.0.36/src/SciAssist/models/mup_bart_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/pipelines/__init__.py` & `SciAssist-0.0.36/src/SciAssist/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/pipelines/dataset_extraction.py` & `SciAssist-0.0.36/src/SciAssist/pipelines/dataset_extraction.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/pipelines/pipeline.py` & `SciAssist-0.0.36/src/SciAssist/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/pipelines/reference_string_parsing.py` & `SciAssist-0.0.36/src/SciAssist/pipelines/reference_string_parsing.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/pipelines/summarization.py` & `SciAssist-0.0.36/src/SciAssist/pipelines/summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/pipelines/testing_pipeline.py` & `SciAssist-0.0.36/src/SciAssist/pipelines/testing_pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/pipelines/training_pipeline.py` & `SciAssist-0.0.36/src/SciAssist/pipelines/training_pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/test.py` & `SciAssist-0.0.36/src/SciAssist/test.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/train.py` & `SciAssist-0.0.36/src/SciAssist/train.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/training_args.py` & `SciAssist-0.0.36/src/SciAssist/training_args.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/utils/__init__.py` & `SciAssist-0.0.36/src/SciAssist/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/utils/collators/CollatorForFid.py` & `SciAssist-0.0.36/src/SciAssist/utils/collators/CollatorForFid.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/utils/data_reader.py` & `SciAssist-0.0.36/src/SciAssist/utils/data_reader.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/utils/data_utils.py` & `SciAssist-0.0.36/src/SciAssist/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/utils/extract_keywords_flant5.py` & `SciAssist-0.0.36/src/SciAssist/utils/extract_keywords_flant5.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/utils/pdf2text.py` & `SciAssist-0.0.36/src/SciAssist/utils/pdf2text.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/SciAssist/utils/windows_pdf2text.py` & `SciAssist-0.0.36/src/SciAssist/utils/windows_pdf2text.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,48 +6,48 @@
 
 path="test.pdf"
 def process_pdf(path):
     raw_text = []
     res = {
         "title":"",
         "author":[],
+        "abstract":[],
         "body_text":[],
         "reference":[]
     }
     print(path)
     fp = open(path, 'rb')
     for page_layout in extract_pages(path):
         for element in page_layout:
-            print(element)
             if "get_text" in dir(element):
                 text = element.get_text().replace("\n","")
                 text = text.strip()
                 if text.isdigit() == False and text != "":
                     raw_text.append(text)
     fp.close()
     res["title"] = raw_text[0]
 
     i = 1 # the index of the current text in raw_text
 
     while i<len(raw_text):
-        if raw_text[i].replace(" ","") in ["abstract","Abstract", "ABSTRACT"]:
+        if raw_text[i].strip().replace(" ","")[:8] in ["abstract","Abstract", "ABSTRACT"]:
             i += 1
             break
         res["author"].append(raw_text[i])
         i += 1
 
     while i<len(raw_text):
-        if raw_text[i][:2] in ["1 ", "1.", "1\n"]\
-                or raw_text[i].replace(" ","") in ["Introdution","INTRODUCTION"]:
+        if raw_text[i].strip()[:2] in ["1 ", "1."] or \
+                raw_text[i].strip().replace(" ","")[:12] in ["Introduction","INTRODUCTION"]:
             break
         res["abstract"].append(raw_text[i])
         i += 1
 
     while i<len(raw_text):
-        if raw_text[i].replace(" ","") in ["References","Reference", "REFERENCE", "REFERENCES"]:
+        if raw_text[i].strip().replace(" ","")[:9] in ["Reference", "REFERENCE"]:
             i += 1
             break
         res["body_text"].append(raw_text[i])
         i += 1
 
     while i<len(raw_text):
         if "Appendix" in raw_text[i]:
```

### Comparing `SciAssist-0.0.35/src/SciAssist.egg-info/PKG-INFO` & `SciAssist-0.0.36/src/SciAssist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciAssist
-Version: 0.0.35
+Version: 0.0.36
 Summary: A toolkit for Scientific Document Processing
 Author-email: WING-NUS <dingyixi@hotmail.com>
 Maintainer-email: Yixi Ding <dingyixi@hotmail.com>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
```

### Comparing `SciAssist-0.0.35/src/SciAssist.egg-info/SOURCES.txt` & `SciAssist-0.0.36/src/SciAssist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/src/process.py` & `SciAssist-0.0.36/src/process.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/tests/test_rsp.py` & `SciAssist-0.0.36/tests/test_rsp.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.35/tests/test_summ.py` & `SciAssist-0.0.36/tests/test_summ.py`

 * *Files identical despite different names*


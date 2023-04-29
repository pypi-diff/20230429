# Comparing `tmp/SciAssist-0.0.33.tar.gz` & `tmp/SciAssist-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SciAssist-0.0.33.tar", last modified: Wed Apr 26 07:19:02 2023, max compression
+gzip compressed data, was "SciAssist-0.0.34.tar", last modified: Sat Apr 29 14:50:37 2023, max compression
```

## Comparing `SciAssist-0.0.33.tar` & `SciAssist-0.0.34.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.032155 SciAssist-0.0.33/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    21150 2022-09-28 02:29:12.000000 SciAssist-0.0.33/LICENSE
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       38 2022-09-28 02:29:12.000000 SciAssist-0.0.33/MANIFEST.in
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-26 07:19:02.032155 SciAssist-0.0.33/PKG-INFO
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6208 2022-11-05 13:55:02.000000 SciAssist-0.0.33/README.md
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1451 2023-04-26 07:13:56.000000 SciAssist-0.0.33/pyproject.toml
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      635 2023-04-26 07:19:02.036155 SciAssist-0.0.33/setup.cfg
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       96 2022-09-28 02:29:12.000000 SciAssist-0.0.33/setup.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.000154 SciAssist-0.0.33/src/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.004154 SciAssist-0.0.33/src/SciAssist/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      818 2023-04-14 07:10:04.000000 SciAssist-0.0.33/src/SciAssist/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.004154 SciAssist-0.0.33/src/SciAssist/bin/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      668 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.004154 SciAssist-0.0.33/src/SciAssist/bin/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      916 2023-03-15 13:25:23.000000 SciAssist-0.0.33/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.008154 SciAssist-0.0.33/src/SciAssist/bin/doc2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    11558 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/LICENSE
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.008154 SciAssist-0.0.33/src/SciAssist/bin/doc2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      158 2023-03-15 13:25:23.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/__pycache__/__init__.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.008154 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.008154 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      167 2023-03-15 13:25:23.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      227 2023-03-15 13:25:23.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/__pycache__/config.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    15546 2023-03-15 13:25:23.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       59 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/config.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.012154 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.012154 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      179 2023-03-15 13:25:23.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2874 2023-03-15 13:25:23.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    15434 2023-03-15 13:25:23.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.012154 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4449 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.016154 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      186 2023-03-15 13:25:23.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6183 2023-03-15 13:25:23.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5972 2023-03-15 13:25:23.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6614 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1019 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2736 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     9058 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        8 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/pdf_to_tei.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3622 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    27209 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    16382 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/s2orc.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.016154 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.020155 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      173 2023-03-15 13:25:23.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2743 2023-03-15 13:25:23.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     8839 2023-03-15 13:25:23.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3531 2023-03-15 13:25:23.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3144 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    11737 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6935 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4235 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      585 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.020155 SciAssist-0.0.33/src/SciAssist/bin/doc2json/scripts/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       73 2022-10-04 11:07:26.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/scripts/run_grobid_linux.sh
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      751 2022-10-04 11:09:22.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      275 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/bin/doc2json/setup.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.024155 SciAssist-0.0.33/src/SciAssist/datamodules/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/datamodules/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4113 2023-03-26 03:08:44.000000 SciAssist-0.0.33/src/SciAssist/datamodules/acl_datamodule.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.024155 SciAssist-0.0.33/src/SciAssist/datamodules/components/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/datamodules/components/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      370 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/datamodules/components/cora_label.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3112 2022-11-05 13:55:02.000000 SciAssist-0.0.33/src/SciAssist/datamodules/cora_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3357 2023-04-14 07:10:04.000000 SciAssist-0.0.33/src/SciAssist/datamodules/dataset_extraction_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3198 2022-11-10 14:45:14.000000 SciAssist-0.0.33/src/SciAssist/datamodules/fid_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2948 2022-11-27 14:04:32.000000 SciAssist-0.0.33/src/SciAssist/datamodules/general_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4331 2022-12-14 08:45:15.000000 SciAssist-0.0.33/src/SciAssist/datamodules/longsumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3179 2023-04-02 03:32:15.000000 SciAssist-0.0.33/src/SciAssist/datamodules/mup_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     7753 2023-03-18 16:34:11.000000 SciAssist-0.0.33/src/SciAssist/datamodules/mup_mup_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6978 2023-04-20 07:49:03.000000 SciAssist-0.0.33/src/SciAssist/datamodules/mup_scisumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5991 2023-04-25 15:59:38.000000 SciAssist-0.0.33/src/SciAssist/datamodules/mup_scisumm_noctrl_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5865 2023-04-14 07:09:42.000000 SciAssist-0.0.33/src/SciAssist/datamodules/scisumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4850 2023-02-23 16:55:34.000000 SciAssist-0.0.33/src/SciAssist/datamodules/test_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4211 2022-12-18 15:08:30.000000 SciAssist-0.0.33/src/SciAssist/datamodules/xsum_datamodule.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.024155 SciAssist-0.0.33/src/SciAssist/models/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/models/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.028155 SciAssist-0.0.33/src/SciAssist/models/components/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/models/components/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1554 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/models/components/bart_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2845 2023-04-14 07:10:04.000000 SciAssist-0.0.33/src/SciAssist/models/components/bert_dataset_extraction.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1547 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/models/components/bert_token_classifier.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1728 2023-04-17 15:52:16.000000 SciAssist-0.0.33/src/SciAssist/models/components/flant5_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6869 2022-11-19 15:12:24.000000 SciAssist-0.0.33/src/SciAssist/models/cora_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     8632 2023-04-14 07:10:04.000000 SciAssist-0.0.33/src/SciAssist/models/dataset_extraction_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    13319 2023-04-02 03:32:15.000000 SciAssist-0.0.33/src/SciAssist/models/mup_bart_module.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.028155 SciAssist-0.0.33/src/SciAssist/pipelines/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3876 2023-04-26 07:13:45.000000 SciAssist-0.0.33/src/SciAssist/pipelines/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    12872 2023-04-14 07:10:04.000000 SciAssist-0.0.33/src/SciAssist/pipelines/dataset_extraction.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2056 2022-11-05 13:55:02.000000 SciAssist-0.0.33/src/SciAssist/pipelines/pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    13826 2022-11-05 13:55:02.000000 SciAssist-0.0.33/src/SciAssist/pipelines/reference_string_parsing.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    14059 2023-04-26 07:11:07.000000 SciAssist-0.0.33/src/SciAssist/pipelines/summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1950 2023-02-20 05:27:12.000000 SciAssist-0.0.33/src/SciAssist/pipelines/testing_pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4003 2022-11-05 13:55:02.000000 SciAssist-0.0.33/src/SciAssist/pipelines/training_pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      786 2022-09-28 02:29:12.000000 SciAssist-0.0.33/src/SciAssist/test.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2022-10-02 15:49:40.000000 SciAssist-0.0.33/src/SciAssist/train.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2852 2022-11-27 16:49:31.000000 SciAssist-0.0.33/src/SciAssist/training_args.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.032155 SciAssist-0.0.33/src/SciAssist/utils/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4733 2023-02-03 14:21:07.000000 SciAssist-0.0.33/src/SciAssist/utils/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.032155 SciAssist-0.0.33/src/SciAssist/utils/collators/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2323 2022-11-10 14:30:40.000000 SciAssist-0.0.33/src/SciAssist/utils/collators/CollatorForFid.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-11-06 14:22:00.000000 SciAssist-0.0.33/src/SciAssist/utils/collators/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1232 2023-01-11 16:34:32.000000 SciAssist-0.0.33/src/SciAssist/utils/data_reader.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    74367 2023-04-26 07:10:09.000000 SciAssist-0.0.33/src/SciAssist/utils/data_utils.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2899 2023-04-22 06:46:59.000000 SciAssist-0.0.33/src/SciAssist/utils/extract_keywords_flant5.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5722 2023-04-22 06:20:33.000000 SciAssist-0.0.33/src/SciAssist/utils/pdf2text.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2261 2023-03-27 00:48:06.000000 SciAssist-0.0.33/src/SciAssist/utils/windows_pdf2text.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.004154 SciAssist-0.0.33/src/SciAssist.egg-info/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-26 07:19:01.000000 SciAssist-0.0.33/src/SciAssist.egg-info/PKG-INFO
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4822 2023-04-26 07:19:01.000000 SciAssist-0.0.33/src/SciAssist.egg-info/SOURCES.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        1 2023-04-26 07:19:01.000000 SciAssist-0.0.33/src/SciAssist.egg-info/dependency_links.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       98 2023-04-26 07:19:01.000000 SciAssist-0.0.33/src/SciAssist.egg-info/entry_points.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      396 2023-04-26 07:19:01.000000 SciAssist-0.0.33/src/SciAssist.egg-info/requires.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       34 2023-04-26 07:19:01.000000 SciAssist-0.0.33/src/SciAssist.egg-info/top_level.txt
--rwxrwxr-x   0 yixi      (1025) yixi      (1027)      690 2022-12-10 17:44:58.000000 SciAssist-0.0.33/src/process.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-26 07:19:02.032155 SciAssist-0.0.33/tests/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1095 2022-12-11 12:29:46.000000 SciAssist-0.0.33/tests/test_rsp.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1129 2022-12-11 12:29:46.000000 SciAssist-0.0.33/tests/test_summ.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.231426 SciAssist-0.0.34/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    21150 2022-09-28 02:29:12.000000 SciAssist-0.0.34/LICENSE
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       38 2022-09-28 02:29:12.000000 SciAssist-0.0.34/MANIFEST.in
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-29 14:50:37.231426 SciAssist-0.0.34/PKG-INFO
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6208 2022-11-05 13:55:02.000000 SciAssist-0.0.34/README.md
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1451 2023-04-29 14:43:07.000000 SciAssist-0.0.34/pyproject.toml
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      635 2023-04-29 14:50:37.231426 SciAssist-0.0.34/setup.cfg
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       96 2022-09-28 02:29:12.000000 SciAssist-0.0.34/setup.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.223425 SciAssist-0.0.34/src/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.223425 SciAssist-0.0.34/src/SciAssist/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      818 2023-04-14 07:10:04.000000 SciAssist-0.0.34/src/SciAssist/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.223425 SciAssist-0.0.34/src/SciAssist/bin/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      668 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.223425 SciAssist-0.0.34/src/SciAssist/bin/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      916 2023-03-15 13:25:23.000000 SciAssist-0.0.34/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.223425 SciAssist-0.0.34/src/SciAssist/bin/doc2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    11558 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/LICENSE
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.223425 SciAssist-0.0.34/src/SciAssist/bin/doc2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      158 2023-03-15 13:25:23.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/__pycache__/__init__.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.223425 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.223425 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      167 2023-03-15 13:25:23.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      227 2023-03-15 13:25:23.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/__pycache__/config.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    15546 2023-03-15 13:25:23.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       59 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/config.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.223425 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.227426 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      179 2023-03-15 13:25:23.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2874 2023-03-15 13:25:23.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    15434 2023-03-15 13:25:23.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.227426 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4449 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.227426 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      186 2023-03-15 13:25:23.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6183 2023-03-15 13:25:23.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5972 2023-03-15 13:25:23.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6614 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1019 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2736 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     9058 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        8 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/pdf_to_tei.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3622 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    27209 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    16382 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/s2orc.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.227426 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.227426 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      173 2023-03-15 13:25:23.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2743 2023-03-15 13:25:23.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     8839 2023-03-15 13:25:23.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3531 2023-03-15 13:25:23.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3144 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    11737 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6935 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4235 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      585 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.227426 SciAssist-0.0.34/src/SciAssist/bin/doc2json/scripts/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       73 2022-10-04 11:07:26.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/scripts/run_grobid_linux.sh
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      751 2022-10-04 11:09:22.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      275 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/bin/doc2json/setup.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.227426 SciAssist-0.0.34/src/SciAssist/datamodules/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/datamodules/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4113 2023-03-26 03:08:44.000000 SciAssist-0.0.34/src/SciAssist/datamodules/acl_datamodule.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.227426 SciAssist-0.0.34/src/SciAssist/datamodules/components/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/datamodules/components/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      370 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/datamodules/components/cora_label.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3112 2022-11-05 13:55:02.000000 SciAssist-0.0.34/src/SciAssist/datamodules/cora_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3357 2023-04-14 07:10:04.000000 SciAssist-0.0.34/src/SciAssist/datamodules/dataset_extraction_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3198 2022-11-10 14:45:14.000000 SciAssist-0.0.34/src/SciAssist/datamodules/fid_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2948 2022-11-27 14:04:32.000000 SciAssist-0.0.34/src/SciAssist/datamodules/general_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4331 2022-12-14 08:45:15.000000 SciAssist-0.0.34/src/SciAssist/datamodules/longsumm_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3179 2023-04-02 03:32:15.000000 SciAssist-0.0.34/src/SciAssist/datamodules/mup_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     7753 2023-03-18 16:34:11.000000 SciAssist-0.0.34/src/SciAssist/datamodules/mup_mup_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6862 2023-04-29 14:42:50.000000 SciAssist-0.0.34/src/SciAssist/datamodules/mup_scisumm_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5991 2023-04-25 15:59:38.000000 SciAssist-0.0.34/src/SciAssist/datamodules/mup_scisumm_noctrl_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5865 2023-04-14 07:09:42.000000 SciAssist-0.0.34/src/SciAssist/datamodules/scisumm_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4850 2023-02-23 16:55:34.000000 SciAssist-0.0.34/src/SciAssist/datamodules/test_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4211 2022-12-18 15:08:30.000000 SciAssist-0.0.34/src/SciAssist/datamodules/xsum_datamodule.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.227426 SciAssist-0.0.34/src/SciAssist/models/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/models/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.231426 SciAssist-0.0.34/src/SciAssist/models/components/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/models/components/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1554 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/models/components/bart_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2845 2023-04-14 07:10:04.000000 SciAssist-0.0.34/src/SciAssist/models/components/bert_dataset_extraction.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1547 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/models/components/bert_token_classifier.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1728 2023-04-17 15:52:16.000000 SciAssist-0.0.34/src/SciAssist/models/components/flant5_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6869 2022-11-19 15:12:24.000000 SciAssist-0.0.34/src/SciAssist/models/cora_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     8632 2023-04-14 07:10:04.000000 SciAssist-0.0.34/src/SciAssist/models/dataset_extraction_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    13319 2023-04-02 03:32:15.000000 SciAssist-0.0.34/src/SciAssist/models/mup_bart_module.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.231426 SciAssist-0.0.34/src/SciAssist/pipelines/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3876 2023-04-26 07:13:45.000000 SciAssist-0.0.34/src/SciAssist/pipelines/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    12872 2023-04-14 07:10:04.000000 SciAssist-0.0.34/src/SciAssist/pipelines/dataset_extraction.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2056 2022-11-05 13:55:02.000000 SciAssist-0.0.34/src/SciAssist/pipelines/pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    13826 2022-11-05 13:55:02.000000 SciAssist-0.0.34/src/SciAssist/pipelines/reference_string_parsing.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    14045 2023-04-29 14:44:31.000000 SciAssist-0.0.34/src/SciAssist/pipelines/summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1950 2023-02-20 05:27:12.000000 SciAssist-0.0.34/src/SciAssist/pipelines/testing_pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4003 2022-11-05 13:55:02.000000 SciAssist-0.0.34/src/SciAssist/pipelines/training_pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      786 2022-09-28 02:29:12.000000 SciAssist-0.0.34/src/SciAssist/test.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2022-10-02 15:49:40.000000 SciAssist-0.0.34/src/SciAssist/train.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2852 2022-11-27 16:49:31.000000 SciAssist-0.0.34/src/SciAssist/training_args.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.231426 SciAssist-0.0.34/src/SciAssist/utils/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4733 2023-02-03 14:21:07.000000 SciAssist-0.0.34/src/SciAssist/utils/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.231426 SciAssist-0.0.34/src/SciAssist/utils/collators/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2323 2022-11-10 14:30:40.000000 SciAssist-0.0.34/src/SciAssist/utils/collators/CollatorForFid.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-11-06 14:22:00.000000 SciAssist-0.0.34/src/SciAssist/utils/collators/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1232 2023-01-11 16:34:32.000000 SciAssist-0.0.34/src/SciAssist/utils/data_reader.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    53624 2023-04-29 14:37:32.000000 SciAssist-0.0.34/src/SciAssist/utils/data_utils.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2899 2023-04-22 06:46:59.000000 SciAssist-0.0.34/src/SciAssist/utils/extract_keywords_flant5.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5722 2023-04-22 06:20:33.000000 SciAssist-0.0.34/src/SciAssist/utils/pdf2text.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2260 2023-04-29 14:34:01.000000 SciAssist-0.0.34/src/SciAssist/utils/windows_pdf2text.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.223425 SciAssist-0.0.34/src/SciAssist.egg-info/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-29 14:50:37.000000 SciAssist-0.0.34/src/SciAssist.egg-info/PKG-INFO
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4822 2023-04-29 14:50:37.000000 SciAssist-0.0.34/src/SciAssist.egg-info/SOURCES.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        1 2023-04-29 14:50:37.000000 SciAssist-0.0.34/src/SciAssist.egg-info/dependency_links.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       98 2023-04-29 14:50:37.000000 SciAssist-0.0.34/src/SciAssist.egg-info/entry_points.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      396 2023-04-29 14:50:37.000000 SciAssist-0.0.34/src/SciAssist.egg-info/requires.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       34 2023-04-29 14:50:37.000000 SciAssist-0.0.34/src/SciAssist.egg-info/top_level.txt
+-rwxrwxr-x   0 yixi      (1025) yixi      (1027)      690 2022-12-10 17:44:58.000000 SciAssist-0.0.34/src/process.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 14:50:37.231426 SciAssist-0.0.34/tests/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1095 2022-12-11 12:29:46.000000 SciAssist-0.0.34/tests/test_rsp.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1129 2022-12-11 12:29:46.000000 SciAssist-0.0.34/tests/test_summ.py
```

### Comparing `SciAssist-0.0.33/LICENSE` & `SciAssist-0.0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/PKG-INFO` & `SciAssist-0.0.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciAssist
-Version: 0.0.33
+Version: 0.0.34
 Summary: A toolkit for Scientific Document Processing
 Author-email: WING-NUS <dingyixi@hotmail.com>
 Maintainer-email: Yixi Ding <dingyixi@hotmail.com>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
```

### Comparing `SciAssist-0.0.33/README.md` & `SciAssist-0.0.34/README.md`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/pyproject.toml` & `SciAssist-0.0.34/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SciAssist"
-version = "0.0.33"
+version = "0.0.34"
 authors = [
   { name="WING-NUS", email="dingyixi@hotmail.com" },
 ]
 maintainers = [
   { name="Yixi Ding", email="dingyixi@hotmail.com" },
 ]
 description = "A toolkit for Scientific Document Processing"
```

### Comparing `SciAssist-0.0.33/setup.cfg` & `SciAssist-0.0.34/setup.cfg`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/__init__.py` & `SciAssist-0.0.34/src/SciAssist/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/__init__.py` & `SciAssist-0.0.34/src/SciAssist/bin/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc` & `SciAssist-0.0.34/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/LICENSE` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/LICENSE`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/s2orc.py` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/s2orc.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh` & `SciAssist-0.0.34/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/datamodules/acl_datamodule.py` & `SciAssist-0.0.34/src/SciAssist/datamodules/acl_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/datamodules/cora_datamodule.py` & `SciAssist-0.0.34/src/SciAssist/datamodules/cora_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/datamodules/dataset_extraction_datamodule.py` & `SciAssist-0.0.34/src/SciAssist/datamodules/dataset_extraction_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/datamodules/fid_datamodule.py` & `SciAssist-0.0.34/src/SciAssist/datamodules/fid_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/datamodules/general_datamodule.py` & `SciAssist-0.0.34/src/SciAssist/datamodules/general_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/datamodules/longsumm_datamodule.py` & `SciAssist-0.0.34/src/SciAssist/datamodules/longsumm_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/datamodules/mup_datamodule.py` & `SciAssist-0.0.34/src/SciAssist/datamodules/mup_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/datamodules/mup_mup_datamodule.py` & `SciAssist-0.0.34/src/SciAssist/datamodules/mup_mup_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/datamodules/mup_scisumm_datamodule.py` & `SciAssist-0.0.34/src/SciAssist/datamodules/mup_scisumm_datamodule.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,26 +48,23 @@
                         'I05-3025', 'J06-1003', 'J08-2005', 'H91-1026', 'C94-1032', 'C94-1027', 'H93-1051', 'C88-2147',
                         'H92-1045', 'C90-3063', 'C90-3044', 'C94-2174', 'D07-1074', 'H93-1052', 'N03-2021', 'C88-2121',
                         'C92-2070', 'C00-2137', 'W97-0703', 'H94-1020', 'C90-3030', 'H01-1035', 'C96-1055', 'H93-1061',
                         'C96-1005', 'C00-1044', 'C92-1038', 'C00-2163', 'C90-3052', 'J94-2003', 'C04-1073']
         texts = []
         summaries = []
         keywords = []
-        with open("/home/yixi/project/scisumm-corpus/data/Training-Set-2019/Task2/From-ScisummNet-2019/forecite.csv",
+        with open("/home/yixi/project/scisumm-corpus/data/Training-Set-2019/Task2/From-ScisummNet-2019/scisumm.csv",
                   'r', newline='', encoding='ISO-8859-1') as f:
             rows = csv.reader(f)
             # Get Column names
             keys = next(rows)
             # Add values by column
             for row in rows:
-                if row[1].strip() == "":
-                    id2kw[row[0]] = None
-                else:
-                    k_list = row[1].split(",")
-                    id2kw[row[0]] = [k.strip() for k in k_list]
+                k_list = row[1].split(",")
+                id2kw[row[0]] = [k.strip() for k in k_list]
 
         file_list = []
         root_dir = "/home/yixi/project/scisumm-corpus/data/Training-Set-2019/Task2/From-ScisummNet-2019"
         for dirpath, dirnames, files in os.walk(root_dir):
             file_list = dirnames
             break
```

### Comparing `SciAssist-0.0.33/src/SciAssist/datamodules/mup_scisumm_noctrl_datamodule.py` & `SciAssist-0.0.34/src/SciAssist/datamodules/mup_scisumm_noctrl_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/datamodules/scisumm_datamodule.py` & `SciAssist-0.0.34/src/SciAssist/datamodules/scisumm_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/datamodules/test_datamodule.py` & `SciAssist-0.0.34/src/SciAssist/datamodules/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/datamodules/xsum_datamodule.py` & `SciAssist-0.0.34/src/SciAssist/datamodules/xsum_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/models/components/bart_summarization.py` & `SciAssist-0.0.34/src/SciAssist/models/components/bart_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/models/components/bert_dataset_extraction.py` & `SciAssist-0.0.34/src/SciAssist/models/components/bert_dataset_extraction.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/models/components/bert_token_classifier.py` & `SciAssist-0.0.34/src/SciAssist/models/components/bert_token_classifier.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/models/components/flant5_summarization.py` & `SciAssist-0.0.34/src/SciAssist/models/components/flant5_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/models/cora_module.py` & `SciAssist-0.0.34/src/SciAssist/models/cora_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/models/dataset_extraction_module.py` & `SciAssist-0.0.34/src/SciAssist/models/dataset_extraction_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/models/mup_bart_module.py` & `SciAssist-0.0.34/src/SciAssist/models/mup_bart_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/pipelines/__init__.py` & `SciAssist-0.0.34/src/SciAssist/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/pipelines/dataset_extraction.py` & `SciAssist-0.0.34/src/SciAssist/pipelines/dataset_extraction.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/pipelines/pipeline.py` & `SciAssist-0.0.34/src/SciAssist/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/pipelines/reference_string_parsing.py` & `SciAssist-0.0.34/src/SciAssist/pipelines/reference_string_parsing.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/pipelines/summarization.py` & `SciAssist-0.0.34/src/SciAssist/pipelines/summarization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # main developer: Yixi Ding <dingyixi@hotmail.com>
 import json
 import math
 import os
 from typing import List, Tuple, Optional, Dict
 
-import torch
 from datasets import Dataset
 
 from SciAssist import BASE_TEMP_DIR, BASE_OUTPUT_DIR
 from SciAssist.pipelines.pipeline import Pipeline
 from SciAssist.pipelines.testing_pipeline import test
 from SciAssist.utils.pdf2text import process_pdf_file, get_bodytext
 from SciAssist.utils.windows_pdf2text import windows_get_bodytext
```

### Comparing `SciAssist-0.0.33/src/SciAssist/pipelines/testing_pipeline.py` & `SciAssist-0.0.34/src/SciAssist/pipelines/testing_pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/pipelines/training_pipeline.py` & `SciAssist-0.0.34/src/SciAssist/pipelines/training_pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/test.py` & `SciAssist-0.0.34/src/SciAssist/test.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/train.py` & `SciAssist-0.0.34/src/SciAssist/train.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/training_args.py` & `SciAssist-0.0.34/src/SciAssist/training_args.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/utils/__init__.py` & `SciAssist-0.0.34/src/SciAssist/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/utils/collators/CollatorForFid.py` & `SciAssist-0.0.34/src/SciAssist/utils/collators/CollatorForFid.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/utils/data_reader.py` & `SciAssist-0.0.34/src/SciAssist/utils/data_reader.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/utils/data_utils.py` & `SciAssist-0.0.34/src/SciAssist/utils/data_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import List, Dict
 
-import os
 import nltk
 import numpy as np
 import torch
 from torch.utils.data import DataLoader, Dataset
 from transformers import AutoTokenizer
 from transformers import DataCollatorForSeq2Seq
 
@@ -612,340 +611,14 @@
             batch_size=8,
             collate_fn=self.collator(),
         )
 
         return dataloader
 
 
-# class DataUtilsForFiD():
-#     """
-#
-#     Args:
-#         tokenizer (`PretrainedTokenizer`, default to None):
-#             The tokenizer for tokenization.
-#         checkpoint (`str`):
-#             The checkpoint from which the tokenizer is loaded.
-#         model_max_length (`int`, *optional*): The max sequence length the model accepts.
-#         max_source_length (`int`, *optional*): The max length of the input text.
-#         max_target_length (`int`, *optional*): The max length of the generated summary.
-#     """
-#
-#     def __init__(self, tokenizer = None, model_class = FiDT5,
-#                  checkpoint = "google/flan-t5-large",
-#                  model_max_length = 64,
-#                  max_source_length = 64,
-#                  max_target_length = 128,
-#                  ):
-#
-#         self.checkpoint = checkpoint
-#         self.model_max_length = model_max_length
-#         self.max_source_length = max_source_length
-#         self.max_target_length = max_target_length
-#         self.model_class = model_class
-#
-#         if tokenizer is None:
-#             self.tokenizer = AutoTokenizer.from_pretrained(
-#                 self.checkpoint,
-#                 model_max_length = self.model_max_length,
-#                 cache_dir=BASE_CACHE_DIR,
-#             )
-#         else:
-#             self.tokenizer = tokenizer
-#
-#
-#     def tokenize_and_align_labels(self, examples, inputs_column="text", labels_column="summary", token_per_paragraph=50):
-#
-#         """
-#
-#         Process the dataset for model input, for example, do tokenization and prepare label_ids.
-#
-#         Args:
-#             examples (`Dataset`): { "text": [s1, s2, ...], "summary": [l1, l2, ...]}
-#             inputs (`str`): The name of input column
-#             labels (`str`): The name of target column
-#
-#         Returns:
-#             `Dict`: {"input_ids": input_ids, "attention_mask": attention_mask, "labels": label_ids }
-#
-#         """
-#
-#         # Select input column
-#         inputs = examples[inputs_column]
-#         dataset = {"paragraphs": []}
-#
-#         for input in inputs:
-#             texts = ["Please give a summary of the following text: "]
-#             tokens = input.split(" ")
-#             index = 0
-#             while index+token_per_paragraph < min(len(tokens),120*token_per_paragraph):
-#                 p = " ".join(tokens[index:index+token_per_paragraph])
-#                 texts.append(p)
-#                 index += token_per_paragraph
-#             texts.append(" ".join(tokens[index:index+token_per_paragraph]))
-#             dataset["paragraphs"].append(texts)
-#
-#
-#         # Select target column
-#         if labels_column in examples.keys():
-#             labels = examples[labels_column]
-#             dataset["labels"] = labels
-#
-#         return dataset
-#
-#     def collator(self):
-#
-#         """
-#
-#         The collating function.
-#
-#         Returns:
-#             `function`: A collating function.
-#
-#             For example, **DataCollatorForSeq2Seq(...)**.
-#
-#             You can also custom a collating function, but remember that `collator()` needs to return a **function**.
-#         """
-#
-#         from SciAssist.utils.collators.CollatorForFid import DataCollatorForFid
-#
-#         return DataCollatorForFid(self.max_source_length, self.tokenizer, self.max_target_length)
-#
-#     def postprocess(self, preds, labels):
-#
-#         """
-#         Process model's outputs and get the final results rather than simple ids.
-#
-#         Args:
-#             preds (Tensor): Prediction labels, the output of the model.
-#             labels (Tensor): True labels
-#
-#         Returns:
-#             `(LongTensor, LongTensor)`: decoded_preds, decoded_labels
-#
-#         """
-#
-#         decoded_preds = self.tokenizer.batch_decode(preds, skip_special_tokens=True)
-#
-#         labels = np.array(labels.to("cpu"))
-#         # Replace -100 in the labels as we can't decode them.
-#         labels = np.where(labels != -100, labels, self.tokenizer.pad_token_id)
-#
-#         decoded_labels = self.tokenizer.batch_decode(labels, skip_special_tokens=True)
-#
-#         decoded_preds = [pred.strip() for pred in decoded_preds]
-#         decoded_labels = [label.strip() for label in decoded_labels]
-#
-#         # rougeLSum expects newline after each sentence
-#         decoded_preds = ["\n".join(nltk.sent_tokenize(pred)) for pred in decoded_preds]
-#         decoded_labels = ["\n".join(nltk.sent_tokenize(label)) for label in decoded_labels]
-#
-#         return decoded_preds, decoded_labels
-#
-#     def get_dataloader(self, dataset, inputs_column="text", labels_column="summary"):
-#
-#         """
-#         Generate DataLoader for a dataset.
-#
-#         Args:
-#             dataset (`Dataset`): The raw dataset.
-#             inputs_column (`str`): Column name of the inputs.
-#             labels_column (`str`): Column name of the labels.
-#
-#         Returns:
-#             `DataLoader`: A dataloader for the dataset. Will be used for inference.
-#         """
-#
-#         tokenized_example = dataset.map(
-#             lambda x: self.tokenize_and_align_labels(x, inputs_column=inputs_column, labels_column=labels_column),
-#             batched=True,
-#             remove_columns=dataset.column_names
-#         )
-#         dataloader = DataLoader(
-#             dataset=tokenized_example,
-#             batch_size=8,
-#             collate_fn=self.collator(),
-#         )
-#
-#         return dataloader
-#
-# #
-#
-# class DataUtilsForFrost():
-#     """
-#
-#     Args:
-#         tokenizer (`PretrainedTokenizer`, default to None):
-#             The tokenizer for tokenization.
-#         checkpoint (`str`):
-#             The checkpoint from which the tokenizer is loaded.
-#         model_max_length (`int`, *optional*): The max sequence length the model accepts.
-#         max_source_length (`int`, *optional*): The max length of the input text.
-#         max_target_length (`int`, *optional*): The max length of the generated summary.
-#     """
-#
-#
-#     def __init__(self, tokenizer = None, model_class = FrostForSummarization,
-#                  checkpoint = "pegasus/frost",
-#                  model_max_length = 1024,
-#                  max_source_length = 1024,
-#                  max_target_length = 128,
-#                  ):
-#
-#         self.checkpoint = checkpoint
-#         self.model_max_length = model_max_length
-#         self.max_source_length = max_source_length
-#         self.max_target_length = max_target_length
-#         self.model_class = model_class
-#
-#         if tokenizer is None:
-#             self.tokenizer = PegasusTokenizer.from_pretrained(
-#                 self.checkpoint,
-#                 cache_dir=BASE_CACHE_DIR,
-#                 model_max_length=self.model_max_length,
-#             )
-#         else:
-#             self.tokenizer = tokenizer
-#
-#         # FROST Constants
-#         self.ENTITYCHAIN_START_TOKEN = "[CONTENT]"
-#         self.SUMMARY_START_TOKEN = "[SUMMARY]"
-#         self.ENTITY_SEPARATOR = " | "
-#         self.ENTITY_SENTENCE_SEPARATOR = " ||| "
-#
-#         # Prepare Spacy processor
-#         self.SPACY_MODEL_OR_PATH = "en_core_web_sm"
-#         self.SPACY_PROCESSOR = spacy.load(self.SPACY_MODEL_OR_PATH)
-#
-#     def get_frost_labels(self, text):
-#         """Gets Spacy Frost processor."""
-#         entity_plans = []
-#         for text_sent in self.SPACY_PROCESSOR(text.replace("\n", " ")).sents:
-#             entity_plans.append(
-#                 self.ENTITY_SEPARATOR.join(
-#                     [entity.text for entity in self.SPACY_PROCESSOR(text_sent.text).ents]))
-#         text_with_entityplans = (
-#                 self.ENTITYCHAIN_START_TOKEN + " " +
-#                 self.ENTITY_SENTENCE_SEPARATOR.join(entity_plans) + " " +
-#                 self.SUMMARY_START_TOKEN + " " + text)
-#         return text_with_entityplans
-#
-#
-#     def tokenize_and_align_labels(self, examples, inputs_column="text", labels_column="summary"):
-#
-#         """
-#
-#         Process the dataset for model input, for example, do tokenization and prepare label_ids.
-#
-#         Args:
-#             examples (`Dataset`): { "text": [s1, s2, ...], "summary": [l1, l2, ...]}
-#             inputs (`str`): The name of input column
-#             labels (`str`): The name of target column
-#
-#         Returns:
-#             `Dict`: {"input_ids": input_ids, "attention_mask": attention_mask, "labels": label_ids }
-#
-#         """
-#
-#         # Select input column
-#         inputs = examples[inputs_column]
-#
-#         # Setup the tokenizer for inputs
-#         model_inputs = self.tokenizer(inputs, max_length=self.max_target_length, padding="max_length", truncation=True)
-#
-#         # Select target column
-#         if labels_column in examples.keys():
-#             labels = examples[labels_column]
-#             labels = [self.get_frost_labels(label) for label in labels]
-#
-#             # Setup the tokenizer for targets
-#             with self.tokenizer.as_target_tokenizer():
-#                 labels = self.tokenizer(labels, max_length=self.max_target_length, padding="max_length", truncation=True)
-#                 # Ignore padding in the loss
-#                 labels["input_ids"] = [
-#                     [(l if l != self.tokenizer.pad_token_id else -100) for l in label] for label in labels["input_ids"]
-#                 ]
-#
-#             model_inputs["labels"] = labels["input_ids"]
-#
-#         return model_inputs
-#
-#     def collator(self):
-#
-#         """
-#
-#         The collating function.
-#
-#         Returns:
-#             `function`: A collating function.
-#
-#             For example, **DataCollatorForSeq2Seq(...)**.
-#
-#             You can also custom a collating function, but remember that `collator()` needs to return a **function**.
-#         """
-#
-#
-#         return DataCollatorForSeq2Seq(self.tokenizer, model=self.model_class, pad_to_multiple_of=8)
-#
-#     def postprocess(self, preds, labels):
-#
-#         """
-#         Process model's outputs and get the final results rather than simple ids.
-#
-#         Args:
-#             preds (Tensor): Prediction labels, the output of the model.
-#             labels (Tensor): True labels
-#
-#         Returns:
-#             `(LongTensor, LongTensor)`: decoded_preds, decoded_labels
-#
-#         """
-#
-#         decoded_preds = self.tokenizer.batch_decode(preds, skip_special_tokens=True)
-#
-#         labels = np.array(labels.to("cpu"))
-#         # Replace -100 in the labels as we can't decode them.
-#         labels = np.where(labels != -100, labels, self.tokenizer.pad_token_id)
-#
-#         decoded_labels = self.tokenizer.batch_decode(labels, skip_special_tokens=False)
-#
-#         decoded_preds = [pred.strip() for pred in decoded_preds]
-#         decoded_labels = [label.strip() for label in decoded_labels]
-#
-#         # rougeLSum expects newline after each sentence
-#         decoded_preds = ["\n".join(nltk.sent_tokenize(pred)) for pred in decoded_preds]
-#         decoded_labels = ["\n".join(nltk.sent_tokenize(label)) for label in decoded_labels]
-#
-#         return decoded_preds, decoded_labels
-#
-#     def get_dataloader(self, dataset, inputs_column="text", labels_column="summary"):
-#
-#         """
-#         Generate DataLoader for a dataset.
-#
-#         Args:
-#             dataset (`Dataset`): The raw dataset.
-#             inputs_column (`str`): Column name of the inputs.
-#             labels_column (`str`): Column name of the labels.
-#
-#         Returns:
-#             `DataLoader`: A dataloader for the dataset. Will be used for inference.
-#         """
-#
-#         tokenized_example = dataset.map(
-#             lambda x: self.tokenize_and_align_labels(x, inputs_column=inputs_column, labels_column=labels_column),
-#             batched=True,
-#             remove_columns=dataset.column_names
-#         )
-#         dataloader = DataLoader(
-#             dataset=tokenized_example,
-#             batch_size=8,
-#             collate_fn=self.collator(),
-#         )
-#
-#         return dataloader
 
 class DataUtilsForT5():
     """
 
     Args:
         tokenizer (`PretrainedTokenizer`, default to None):
             The tokenizer for tokenization.
@@ -1763,214 +1436,7 @@
             collate_fn=self.collator(),
         )
 
         return dataloader
 
 
 
-class DataUtilsForCTRLSum():
-    """
-
-    Args:
-        tokenizer (`PretrainedTokenizer`, default to None):
-            The tokenizer for tokenization.
-        checkpoint (`str`):
-            The checkpoint from which the tokenizer is loaded.
-        model_max_length (`int`, *optional*): The max sequence length the model accepts.
-        max_source_length (`int`, *optional*): The max length of the input text.
-        max_target_length (`int`, *optional*): The max length of the generated summary.
-    """
-
-
-    def __init__(self, tokenizer = None,
-                 model_class = FlanT5ForSummarization,
-                 checkpoint = "google/flan-t5-base",
-                 prompt = "Please give a summary of the following text ",
-                 model_max_length = 1024,
-                 max_source_length = 1024,
-                 max_target_length = 500,
-                 ):
-
-        self.checkpoint = checkpoint
-        self.model_max_length = model_max_length
-        self.max_source_length = max_source_length
-        self.max_target_length = max_target_length
-        self.model_class = model_class
-        self.prompt = prompt
-
-        if tokenizer is None:
-            self.tokenizer = AutoTokenizer.from_pretrained(
-                self.checkpoint,
-                model_max_length = self.model_max_length,
-                cache_dir=BASE_CACHE_DIR,
-                use_fast=True
-            )
-        else:
-            self.tokenizer = tokenizer
-
-
-    def tokenize_and_align_labels(self, examples, inputs_column="text", labels_column="summary"):
-
-        """
-
-        Process the dataset for model input, for example, do tokenization and prepare label_ids.
-
-        Args:
-            examples (`Dataset`): { "text": [s1, s2, ...], "summary": [l1, l2, ...]}
-            inputs (`str`): The name of input column
-            labels (`str`): The name of target column
-
-        Returns:
-            `Dict`: {"input_ids": input_ids, "attention_mask": attention_mask, "labels": label_ids }
-
-        """
-
-        inputs = examples[inputs_column]
-        prompts = [ self.prompt for i in inputs ]
-
-        # kw_instructions = ["{}"]
-        def kw(prompt, keyword):
-            # i = randint(1,10)
-            return "Keywords: " + str(", ".join(keyword)) + ". " + prompt + "talking about these keywords " if keyword is not None else prompt
-
-            # return prompt + "that focuses on " + str(", ".join(keyword)) + " " if keyword is not None else prompt
-        def leng(prompt, length):
-            return prompt + ", which has less than " + str(length) + " words " if length is not None else prompt
-
-        # if "keywords" in examples.keys():
-        #     keywords = examples["keywords"]
-        #     if keywords is not None:
-        #         prompts = [ kw(prompt,keyword) for (prompt,keyword) in zip(prompts,keywords) ]
-        if "length" in examples.keys():
-            if examples["length"] is not None:
-                lengths = examples["length"]
-                prompts = [ leng(prompt,length) for (prompt,length) in zip(prompts,lengths)]
-        # kwords = ["" for i in inputs]
-        # if "keywords" in examples.keys():
-        #     keywords = examples["keywords"]
-        #     if keywords is not None:
-        #         keywords = [ keyword if keyword is not None else [] for keyword in keywords ]
-        #         # print(keywords)
-        #         kwords = [ " ".join(keyword) for keyword in keywords ]
-        inputs = [ prompt + ": " + raw_text for (prompt,raw_text) in zip(prompts, inputs) ]
-        # inputs = [ f"Which entity is this text about? {text} Entity:".format(text) for text in inputs]
-        print(inputs[0][:200])
-
-
-
-        # if "keywords" in examples.keys():
-        #     keywords = examples["keywords"]
-        #     if keywords is not None and keywords[0] is not None:
-        #         prompts = [ prompt + "that focuses on " + str(", ".join(keyword)) + " " for (prompt,keyword) in zip(prompts,keywords) ]
-        # if "length" in examples.keys():
-        #     if examples["length"] is not None and examples["length"][0] is not None:
-        #         lengths = [l for l in examples["length"]]
-        #         prompts = [ prompt + ", which has less than " + str(length) + " words " for (prompt,length) in zip(prompts,lengths)]
-        # inputs = [ prompt + ": " + raw_text for (prompt,raw_text) in zip(prompts,inputs) ]
-        # print(inputs[0][:200])
-        #
-
-
-        # if labels_column in examples.keys():
-        #     lengths = [len(s.split(" ")) for s in examples[labels_column]]
-        #     lengths = [ 10*math.ceil(s/10) for s in lengths]
-
-        # Select input column
-        # inputs = examples[inputs_column]
-        # inputs = [ self.prompt + "which has less than " + str(length) + " words: " + raw_text for (raw_text,length) in zip(inputs,lengths) ]
-        # inputs = [ "| " + str(length) + " words | " + "summarize: " + raw_text for (raw_text, length) in
-        #           zip(inputs, lengths)]
-
-        # Setup the tokenizer for inputs
-
-        model_inputs = self.tokenizer(inputs, max_length=self.max_source_length, padding="max_length", truncation=True)
-
-        # Select target column
-        if labels_column in examples.keys():
-            labels = examples[labels_column]
-            # Setup the tokenizer for targets
-            with self.tokenizer.as_target_tokenizer():
-                labels = self.tokenizer(labels, max_length=self.max_target_length, padding="max_length", truncation=True)
-                # Ignore padding in the loss
-                labels["input_ids"] = [
-                    [(l if l != self.tokenizer.pad_token_id else -100) for l in label] for label in labels["input_ids"]
-                ]
-            model_inputs["labels"] = labels["input_ids"]
-
-
-        return model_inputs
-
-    def collator(self):
-
-        """
-
-        The collating function.
-
-        Returns:
-            `function`: A collating function.
-
-            For example, **DataCollatorForSeq2Seq(...)**.
-
-            You can also custom a collating function, but remember that `collator()` needs to return a **function**.
-        """
-
-
-        return DataCollatorForSeq2Seq(self.tokenizer, model=self.model_class, pad_to_multiple_of=8)
-
-    def postprocess(self, preds, labels):
-
-        """
-        Process model's outputs and get the final results rather than simple ids.
-
-        Args:
-            preds (Tensor): Prediction labels, the output of the model.
-            labels (Tensor): True labels
-
-        Returns:
-            `(LongTensor, LongTensor)`: decoded_preds, decoded_labels
-
-        """
-
-        decoded_preds = self.tokenizer.batch_decode(preds, skip_special_tokens=True)
-
-        labels = np.array(labels.to("cpu"))
-        # Replace -100 in the labels as we can't decode them.
-        labels = np.where(labels != -100, labels, self.tokenizer.pad_token_id)
-
-        decoded_labels = self.tokenizer.batch_decode(labels, skip_special_tokens=True)
-
-        decoded_preds = [pred.strip() for pred in decoded_preds]
-        decoded_labels = [label.strip() for label in decoded_labels]
-
-        # rougeLSum expects newline after each sentence
-        decoded_preds = ["\n".join(nltk.sent_tokenize(pred)) for pred in decoded_preds]
-        decoded_labels = ["\n".join(nltk.sent_tokenize(label)) for label in decoded_labels]
-
-        return decoded_preds, decoded_labels
-
-    def get_dataloader(self, dataset, inputs_column="text", labels_column="summary"):
-
-        """
-        Generate DataLoader for a dataset.
-
-        Args:
-            dataset (`Dataset`): The raw dataset.
-            inputs_column (`str`): Column name of the inputs.
-            labels_column (`str`): Column name of the labels.
-
-        Returns:
-            `DataLoader`: A dataloader for the dataset. Will be used for inference.
-        """
-
-        tokenized_example = dataset.map(
-            lambda x: self.tokenize_and_align_labels(x, inputs_column=inputs_column, labels_column=labels_column),
-            batched=True,
-            remove_columns=dataset.column_names
-        )
-
-        dataloader = DataLoader(
-            dataset=tokenized_example,
-            batch_size=8,
-            collate_fn=self.collator(),
-        )
-
-        return dataloader
```

### Comparing `SciAssist-0.0.33/src/SciAssist/utils/extract_keywords_flant5.py` & `SciAssist-0.0.34/src/SciAssist/utils/extract_keywords_flant5.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/utils/pdf2text.py` & `SciAssist-0.0.34/src/SciAssist/utils/pdf2text.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/SciAssist/utils/windows_pdf2text.py` & `SciAssist-0.0.34/src/SciAssist/utils/windows_pdf2text.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,39 +24,38 @@
                     raw_text.append(text)
     fp.close()
     res["title"] = raw_text[0]
 
     i = 1 # the index of the current text in raw_text
 
     while i<len(raw_text):
-        if raw_text[i] in ["abstract","Abstract", "ABSTRACT"]:
+        if raw_text[i].replace(" ","") in ["abstract","Abstract", "ABSTRACT"]:
             i += 1
             break
         res["author"].append(raw_text[i])
         i += 1
 
     while i<len(raw_text):
-        if "Introduction" in raw_text[i] or "INTRODUCTION" in raw_text[i]:
+        if raw_text[i][:2] in ["1 ", "1."]:
             break
         i += 1
 
     while i<len(raw_text):
-        if raw_text[i] in ["References","Reference", "REFERENCE", "REFERENCES"]:
+        if raw_text[i].replace(" ","") in ["References","Reference", "REFERENCE", "REFERENCES"]:
             i += 1
             break
         res["body_text"].append(raw_text[i])
         i += 1
 
     while i<len(raw_text):
         if "Appendix" in raw_text[i]:
             i += 1
             break
         res["reference"].append(raw_text[i])
         i += 1
-
     return res
 
 
 def windows_get_reference(path, output_dir: str = BASE_OUTPUT_DIR):
 
     os.makedirs(output_dir, exist_ok=True)
```

### Comparing `SciAssist-0.0.33/src/SciAssist.egg-info/PKG-INFO` & `SciAssist-0.0.34/src/SciAssist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciAssist
-Version: 0.0.33
+Version: 0.0.34
 Summary: A toolkit for Scientific Document Processing
 Author-email: WING-NUS <dingyixi@hotmail.com>
 Maintainer-email: Yixi Ding <dingyixi@hotmail.com>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
```

### Comparing `SciAssist-0.0.33/src/SciAssist.egg-info/SOURCES.txt` & `SciAssist-0.0.34/src/SciAssist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/src/process.py` & `SciAssist-0.0.34/src/process.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/tests/test_rsp.py` & `SciAssist-0.0.34/tests/test_rsp.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.33/tests/test_summ.py` & `SciAssist-0.0.34/tests/test_summ.py`

 * *Files identical despite different names*


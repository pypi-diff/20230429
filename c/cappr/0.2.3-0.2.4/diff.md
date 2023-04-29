# Comparing `tmp/cappr-0.2.3.tar.gz` & `tmp/cappr-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cappr-0.2.3.tar", last modified: Thu Apr 27 21:27:34 2023, max compression
+gzip compressed data, was "cappr-0.2.4.tar", last modified: Fri Apr 28 23:56:05 2023, max compression
```

## Comparing `cappr-0.2.3.tar` & `cappr-0.2.4.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.303793 cappr-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.287793 cappr-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.287793 cappr-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-27 21:27:19.000000 cappr-0.2.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-27 21:27:19.000000 cappr-0.2.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 21:27:19.000000 cappr-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-27 21:27:19.000000 cappr-0.2.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 21:27:19.000000 cappr-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-04-27 21:27:34.299793 cappr-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14820 2023-04-27 21:27:19.000000 cappr-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.291793 cappr-0.2.3/demos/
--rw-r--r--   0 runner    (1001) docker     (123)  2760040 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/computational_analysis.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.295793 cappr-0.2.3/demos/raft/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/ade.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/b77.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/nis.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/ose.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/over.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/sot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/sri.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15611 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/tai.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/tc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/teh.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/tos.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.295793 cappr-0.2.3/demos/superglue/
--rw-r--r--   0 runner    (1001) docker     (123)    64027 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/superglue/copa.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    42865 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/superglue/wsc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.295793 cappr-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/1_is_for_me.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/2_motivation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/3_installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/4_user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/5_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/6_computational_performance.rst
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/7_future_research.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/_static/github-mark.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/docs/source/_static/scaling_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    53692 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/_static/scaling_classes/batch_size_32.png
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/cappr.huggingface.classify.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/cappr.huggingface.classify_no_cache.rst
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/cappr.huggingface.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/cappr.openai.api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/cappr.openai.classify.rst
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/cappr.openai.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/cappr.rst
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/cappr.utils.classify.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/cappr.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/related_work.rst
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/research.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/walkthrough.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-27 21:27:20.000000 cappr-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 21:27:34.303793 cappr-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-27 21:27:20.000000 cappr-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.287793 cappr-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/src/cappr/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/src/cappr/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/huggingface/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34123 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/huggingface/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)    27937 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/huggingface/classify_no_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/src/cappr/openai/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25167 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/openai/classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/src/cappr/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/utils/_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/utils/_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/utils/classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/src/cappr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-04-27 21:27:34.000000 cappr-0.2.3/src/cappr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-27 21:27:34.000000 cappr-0.2.3/src/cappr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:27:34.000000 cappr-0.2.3/src/cappr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-27 21:27:34.000000 cappr-0.2.3/src/cappr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 21:27:34.000000 cappr-0.2.3/src/cappr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-27 21:27:20.000000 cappr-0.2.3/tests/_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/tests/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-04-27 21:27:20.000000 cappr-0.2.3/tests/huggingface/test_huggingface_classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-27 21:27:20.000000 cappr-0.2.3/tests/openai/test_openai_classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-27 21:27:20.000000 cappr-0.2.3/tests/utils/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-27 21:27:20.000000 cappr-0.2.3/tests/utils/test_utils_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.020650 cappr-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.024650 cappr-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-28 23:55:54.000000 cappr-0.2.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-28 23:55:54.000000 cappr-0.2.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-28 23:55:54.000000 cappr-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-28 23:55:54.000000 cappr-0.2.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 23:55:54.000000 cappr-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-04-28 23:56:05.032650 cappr-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14820 2023-04-28 23:55:54.000000 cappr-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.024650 cappr-0.2.4/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)  2760040 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/computational_analysis.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.028650 cappr-0.2.4/demos/raft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/ade.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/b77.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/nis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/ose.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/over.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/sot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/sri.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15611 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/tai.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/tc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/teh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/tos.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.028650 cappr-0.2.4/demos/superglue/
+-rw-r--r--   0 runner    (1001) docker     (123)    64027 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/superglue/copa.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    42865 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/superglue/wsc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.028650 cappr-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.028650 cappr-0.2.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/1_is_for_me.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/2_motivation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/3_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/4_user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/5_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/6_computational_performance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/7_future_research.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.028650 cappr-0.2.4/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/_static/github-mark.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/docs/source/_static/scaling_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    53692 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/_static/scaling_classes/batch_size_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/cappr.huggingface.classify.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/cappr.huggingface.classify_no_cache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/cappr.huggingface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/cappr.openai.api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/cappr.openai.classify.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/cappr.openai.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/cappr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/cappr.utils.classify.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/cappr.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/related_work.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/research.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/walkthrough.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-28 23:55:54.000000 cappr-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:56:05.032650 cappr-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-28 23:55:54.000000 cappr-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.020650 cappr-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/src/cappr/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/src/cappr/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/huggingface/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34123 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/huggingface/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27937 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/huggingface/classify_no_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/src/cappr/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25351 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/openai/classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/src/cappr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/utils/_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/utils/_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/utils/classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/src/cappr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-04-28 23:56:04.000000 cappr-0.2.4/src/cappr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-28 23:56:05.000000 cappr-0.2.4/src/cappr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:56:04.000000 cappr-0.2.4/src/cappr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-28 23:56:04.000000 cappr-0.2.4/src/cappr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 23:56:04.000000 cappr-0.2.4/src/cappr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-28 23:55:54.000000 cappr-0.2.4/tests/_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/tests/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-04-28 23:55:54.000000 cappr-0.2.4/tests/huggingface/test_huggingface_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-28 23:55:54.000000 cappr-0.2.4/tests/openai/test_openai_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-28 23:55:54.000000 cappr-0.2.4/tests/utils/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-28 23:55:54.000000 cappr-0.2.4/tests/utils/test_utils_classify.py
```

### Comparing `cappr-0.2.3/.github/workflows/python-publish.yml` & `cappr-0.2.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/.github/workflows/test.yml` & `cappr-0.2.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/LICENSE` & `cappr-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/PKG-INFO` & `cappr-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cappr
-Version: 0.2.3
+Version: 0.2.4
 Summary: Zero-shot text classification using autoregressive language models.
 Home-page: https://github.com/kddubey/cappr/
 Author-email: kushdubey63@gmail.com
 License: Apache License 2.0
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: hf
```

### Comparing `cappr-0.2.3/README.md` & `cappr-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/demos/computational_analysis.ipynb` & `cappr-0.2.4/demos/computational_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/demos/raft/README.md` & `cappr-0.2.4/demos/raft/README.md`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/demos/raft/ade.ipynb` & `cappr-0.2.4/demos/raft/ade.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/demos/raft/b77.ipynb` & `cappr-0.2.4/demos/raft/b77.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/demos/raft/nis.ipynb` & `cappr-0.2.4/demos/raft/nis.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/demos/raft/ose.ipynb` & `cappr-0.2.4/demos/raft/ose.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/demos/raft/over.ipynb` & `cappr-0.2.4/demos/raft/over.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/demos/raft/sot.ipynb` & `cappr-0.2.4/demos/raft/sot.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/demos/raft/sri.ipynb` & `cappr-0.2.4/demos/raft/sri.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/demos/raft/tai.ipynb` & `cappr-0.2.4/demos/raft/tai.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/demos/raft/tc.ipynb` & `cappr-0.2.4/demos/raft/tc.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/demos/raft/teh.ipynb` & `cappr-0.2.4/demos/raft/teh.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/demos/raft/tos.ipynb` & `cappr-0.2.4/demos/raft/tos.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/demos/superglue/copa.ipynb` & `cappr-0.2.4/demos/superglue/copa.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/demos/superglue/wsc.ipynb` & `cappr-0.2.4/demos/superglue/wsc.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/demos/utils.py` & `cappr-0.2.4/demos/utils.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/docs/Makefile` & `cappr-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/docs/make.bat` & `cappr-0.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/docs/source/1_is_for_me.rst` & `cappr-0.2.4/docs/source/1_is_for_me.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/docs/source/2_motivation.rst` & `cappr-0.2.4/docs/source/2_motivation.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/docs/source/3_installation.rst` & `cappr-0.2.4/docs/source/3_installation.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/docs/source/4_user_guide.rst` & `cappr-0.2.4/docs/source/4_user_guide.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/docs/source/6_computational_performance.rst` & `cappr-0.2.4/docs/source/6_computational_performance.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/docs/source/7_future_research.rst` & `cappr-0.2.4/docs/source/7_future_research.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/docs/source/_static/github-mark.png` & `cappr-0.2.4/docs/source/_static/github-mark.png`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/docs/source/_static/scaling_classes/batch_size_32.png` & `cappr-0.2.4/docs/source/_static/scaling_classes/batch_size_32.png`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/docs/source/conf.py` & `cappr-0.2.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/docs/source/index.rst` & `cappr-0.2.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/docs/source/related_work.rst` & `cappr-0.2.4/docs/source/related_work.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/setup.py` & `cappr-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/src/cappr/_example.py` & `cappr-0.2.4/src/cappr/_example.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/src/cappr/huggingface/_utils.py` & `cappr-0.2.4/src/cappr/huggingface/_utils.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/src/cappr/huggingface/classify.py` & `cappr-0.2.4/src/cappr/huggingface/classify.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/src/cappr/huggingface/classify_no_cache.py` & `cappr-0.2.4/src/cappr/huggingface/classify_no_cache.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/src/cappr/openai/api.py` & `cappr-0.2.4/src/cappr/openai/api.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/src/cappr/openai/classify.py` & `cappr-0.2.4/src/cappr/openai/classify.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,30 +63,32 @@
     for i, log_probs_text in zip(idxs_multiple_tokens, log_probs_texts):
         log_probs[i] = log_probs_text
     return log_probs
 
 
 def _slice_completions(
     completions: Sequence[str],
+    end_of_prompt: str,
     log_probs: Sequence[Sequence[float]],
     model: openai.api.Model,
 ) -> list[list[float]]:
     """
-    TODO: convert docstring to numpy style
+    TODO: convert docstring to numpy style, expose
 
     Returns a list `log_probs_completions` where `log_probs_completions[i]` is a list of
-    conditional log-probablities for each token in `completions[i]`, extracted by
-    slicing `log_probs[i]`.
+    conditional log-probablities for each token in `end_of_prompt + completions[i]`,
+    extracted by slicing `log_probs[i]`.
     """
     if len(completions) != len(log_probs):
         raise ValueError(
             "Different number of completions and log_probs: "
             f"{len(completions)}, {len(log_probs)}."
         )
     tokenizer = tiktoken.encoding_for_model(model)
+    completions = [end_of_prompt + completion for completion in completions]
     completion_lengths = [len(tokens) for tokens in tokenizer.encode_batch(completions)]
     return [
         log_probs_text[-num_completion_tokens:]
         for num_completion_tokens, log_probs_text in zip(completion_lengths, log_probs)
     ]
 
 
@@ -171,15 +173,15 @@
         for prompt in prompts
         for completion in completions
     ]
     log_probs = token_logprobs(texts, model=model, ask_if_ok=ask_if_ok)
     ## Since log_probs is a flat list, we'll need to batch them by the size and order of
     ## completions to fulfill the spec.
     return [
-        _slice_completions(completions, log_probs_batch, model)
+        _slice_completions(completions, end_of_prompt, log_probs_batch, model)
         for log_probs_batch in _batch.constant(log_probs, size=len(completions))
     ]
 
 
 def log_probs_conditional_examples(
     examples: Sequence[Example], model: openai.api.Model, ask_if_ok: bool = False
 ) -> list[list[list[float]]]:
@@ -250,18 +252,20 @@
         example.prompt + example.end_of_prompt + completion
         for example in examples
         for completion in example.completions
     ]
     log_probs_all = token_logprobs(texts, model=model, ask_if_ok=ask_if_ok)
     ## Flatten completions in same order as examples were flattened
     completions_all = [
-        completion for example in examples for completion in example.completions
+        example.end_of_prompt + completion
+        for example in examples
+        for completion in example.completions
     ]
     log_probs_completions_all = _slice_completions(
-        completions_all, log_probs_all, model
+        completions_all, "", log_probs_all, model
     )
     ## Batch by completions to fulfill the spec
     num_completions_per_prompt = [len(example.completions) for example in examples]
     return list(
         _batch.variable(log_probs_completions_all, sizes=num_completions_per_prompt)
     )
```

### Comparing `cappr-0.2.3/src/cappr/utils/_batch.py` & `cappr-0.2.4/src/cappr/utils/_batch.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/src/cappr/utils/_check.py` & `cappr-0.2.4/src/cappr/utils/_check.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/src/cappr/utils/classify.py` & `cappr-0.2.4/src/cappr/utils/classify.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/src/cappr.egg-info/PKG-INFO` & `cappr-0.2.4/src/cappr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cappr
-Version: 0.2.3
+Version: 0.2.4
 Summary: Zero-shot text classification using autoregressive language models.
 Home-page: https://github.com/kddubey/cappr/
 Author-email: kushdubey63@gmail.com
 License: Apache License 2.0
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: hf
```

### Comparing `cappr-0.2.3/src/cappr.egg-info/SOURCES.txt` & `cappr-0.2.4/src/cappr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/tests/_test.py` & `cappr-0.2.4/tests/_test.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/tests/huggingface/test_huggingface_classify.py` & `cappr-0.2.4/tests/huggingface/test_huggingface_classify.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/tests/openai/test_openai_classify.py` & `cappr-0.2.4/tests/openai/test_openai_classify.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,17 @@
     texts = ["a b c", "d e"]
     log_probs = classify.token_logprobs(texts, model)
     assert log_probs == [[0, 1, 2], [0, 1]]
 
 
 def test__slice_completions(completions, model):
     log_probs = [[0, 1, 2], [0, 1]]
-    log_probs_completions = classify._slice_completions(completions, log_probs, model)
+    log_probs_completions = classify._slice_completions(
+        completions, "", log_probs, model
+    )
     assert log_probs_completions == [[1, 2], [1]]
 
 
 def test_log_probs_conditional(prompts, completions, model):
     log_probs_conditional = classify.log_probs_conditional(prompts, completions, model)
     expected = [[[10, 11], [10]], [[5, 6], [5]], [[5, 6], [5]], [[8, 9], [8]]]
     assert log_probs_conditional == expected
```

### Comparing `cappr-0.2.3/tests/utils/test_batch.py` & `cappr-0.2.4/tests/utils/test_batch.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.3/tests/utils/test_utils_classify.py` & `cappr-0.2.4/tests/utils/test_utils_classify.py`

 * *Files identical despite different names*


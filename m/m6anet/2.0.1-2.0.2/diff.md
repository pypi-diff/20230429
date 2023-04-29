# Comparing `tmp/m6anet-2.0.1.tar.gz` & `tmp/m6anet-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/m6anet/m6anet/dist/.tmp-kepktkn1/m6anet-2.0.1.tar", last modified: Thu Mar 16 15:11:31 2023, max compression
+gzip compressed data, was "/home/runner/work/m6anet/m6anet/dist/.tmp-rpj6yx_5/m6anet-2.0.2.tar", last modified: Sat Apr 29 13:17:58 2023, max compression
```

## Comparing `m6anet-2.0.1.tar` & `m6anet-2.0.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 15:11:31.000000 m6anet-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-16 15:11:20.000000 m6anet-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-16 15:11:31.000000 m6anet-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-03-16 15:11:20.000000 m6anet-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 15:11:31.000000 m6anet-2.0.1/m6anet/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 15:11:31.000000 m6anet-2.0.1/m6anet/deprecated/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/deprecated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/deprecated/compute_norm_factors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/deprecated/dataprep.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/deprecated/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/deprecated/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 15:11:31.000000 m6anet-2.0.1/m6anet/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 15:11:31.000000 m6anet-2.0.1/m6anet/model/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 15:11:31.000000 m6anet-2.0.1/m6anet/model/configs/model_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/model/configs/model_configs/m6anet.toml
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 15:11:31.000000 m6anet-2.0.1/m6anet/model/model_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/model/model_blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/model/model_blocks/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/model/model_blocks/pooling_blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 15:11:31.000000 m6anet-2.0.1/m6anet/model/model_states/
--rw-r--r--   0 runner    (1001) docker     (123)    37083 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/model/model_states/human_hct116.pt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 15:11:31.000000 m6anet-2.0.1/m6anet/model/norm_factors/
--rw-r--r--   0 runner    (1001) docker     (123)   179264 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/model/norm_factors/norm_factors_hct116.joblib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 15:11:31.000000 m6anet-2.0.1/m6anet/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/scripts/compute_norm_factors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/scripts/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/scripts/dataprep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/scripts/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 15:11:31.000000 m6anet-2.0.1/m6anet/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/utils/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    27787 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26928 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/utils/dataprep_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/utils/inference_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 15:11:31.000000 m6anet-2.0.1/m6anet/utils/loss_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/utils/loss_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/utils/loss_functions/loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/utils/norm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/utils/sampler_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-03-16 15:11:20.000000 m6anet-2.0.1/m6anet/utils/training_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 15:11:31.000000 m6anet-2.0.1/m6anet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-16 15:11:31.000000 m6anet-2.0.1/m6anet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-03-16 15:11:31.000000 m6anet-2.0.1/m6anet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 15:11:31.000000 m6anet-2.0.1/m6anet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-16 15:11:31.000000 m6anet-2.0.1/m6anet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-16 15:11:31.000000 m6anet-2.0.1/m6anet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-16 15:11:31.000000 m6anet-2.0.1/m6anet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 15:11:31.000000 m6anet-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-03-16 15:11:20.000000 m6anet-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:17:58.000000 m6anet-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-29 13:17:49.000000 m6anet-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-29 13:17:58.000000 m6anet-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-29 13:17:49.000000 m6anet-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:17:58.000000 m6anet-2.0.2/m6anet/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:17:58.000000 m6anet-2.0.2/m6anet/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/deprecated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/deprecated/compute_norm_factors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/deprecated/dataprep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/deprecated/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/deprecated/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:17:58.000000 m6anet-2.0.2/m6anet/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:17:58.000000 m6anet-2.0.2/m6anet/model/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:17:58.000000 m6anet-2.0.2/m6anet/model/configs/model_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/model/configs/model_configs/m6anet.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:17:58.000000 m6anet-2.0.2/m6anet/model/model_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/model/model_blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/model/model_blocks/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/model/model_blocks/pooling_blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:17:58.000000 m6anet-2.0.2/m6anet/model/model_states/
+-rw-r--r--   0 runner    (1001) docker     (123)    37083 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/model/model_states/human_hct116.pt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:17:58.000000 m6anet-2.0.2/m6anet/model/norm_factors/
+-rw-r--r--   0 runner    (1001) docker     (123)   179264 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/model/norm_factors/norm_factors_hct116.joblib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:17:58.000000 m6anet-2.0.2/m6anet/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/scripts/compute_norm_factors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/scripts/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/scripts/dataprep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/scripts/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:17:58.000000 m6anet-2.0.2/m6anet/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/utils/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27787 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26928 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/utils/dataprep_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/utils/inference_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:17:58.000000 m6anet-2.0.2/m6anet/utils/loss_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/utils/loss_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/utils/loss_functions/loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/utils/norm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/utils/sampler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-04-29 13:17:49.000000 m6anet-2.0.2/m6anet/utils/training_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:17:58.000000 m6anet-2.0.2/m6anet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-29 13:17:58.000000 m6anet-2.0.2/m6anet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-29 13:17:58.000000 m6anet-2.0.2/m6anet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:17:58.000000 m6anet-2.0.2/m6anet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-29 13:17:58.000000 m6anet-2.0.2/m6anet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-29 13:17:58.000000 m6anet-2.0.2/m6anet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 13:17:58.000000 m6anet-2.0.2/m6anet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 13:17:58.000000 m6anet-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-29 13:17:49.000000 m6anet-2.0.2/setup.py
```

### Comparing `m6anet-2.0.1/LICENSE` & `m6anet-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/PKG-INFO` & `m6anet-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: m6anet
-Version: 2.0.1
+Version: 2.0.2
 Summary: m6anet is a python package for detection of m6a modifications from Nanopore direct RNA sequencing data.
 Home-page: https://github.com/GoekeLab/m6anet
 Author: Christopher Hendra
 Maintainer-email: christopher.hendra@u.nus.edu
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.7
+Requires-Python: >=3.7, <3.9
 License-File: LICENSE
 
 # m6anet
 ![alt text](https://github.com/GoekeLab/m6anet/blob/master/figures/m6anet_logo.png "m6anet")
 
 m6anet is a python tool that leverages Multiple Instance Learning framework to detect m6a modifications from Nanopore Direct RNA Sequencing data
```

### Comparing `m6anet-2.0.1/README.md` & `m6anet-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/__init__.py` & `m6anet-2.0.2/m6anet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
 from m6anet.scripts import dataprep, inference, train, \
         compute_norm_factors, convert
 
 
 modules = ['dataprep', 'inference', 'train', 'compute_norm_factors', 'convert']
 
-__version__ = "2.0.1"
+__version__ = "2.0.2"
 
 
 def main():
     parser = ArgumentParser(prog='m6anet',
                             formatter_class=ArgumentDefaultsHelpFormatter)
 
     parser.add_argument('-v', '--version', action='version',
```

### Comparing `m6anet-2.0.1/m6anet/deprecated/compute_norm_factors.py` & `m6anet-2.0.2/m6anet/deprecated/compute_norm_factors.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/deprecated/dataprep.py` & `m6anet-2.0.2/m6anet/deprecated/dataprep.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/deprecated/inference.py` & `m6anet-2.0.2/m6anet/deprecated/inference.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/deprecated/train.py` & `m6anet-2.0.2/m6anet/deprecated/train.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/model/configs/model_configs/m6anet.toml` & `m6anet-2.0.2/m6anet/model/configs/model_configs/m6anet.toml`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/model/model.py` & `m6anet-2.0.2/m6anet/model/model.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/model/model_blocks/__init__.py` & `m6anet-2.0.2/m6anet/model/model_blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/model/model_blocks/blocks.py` & `m6anet-2.0.2/m6anet/model/model_blocks/blocks.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/model/model_blocks/pooling_blocks.py` & `m6anet-2.0.2/m6anet/model/model_blocks/pooling_blocks.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/model/model_states/human_hct116.pt` & `m6anet-2.0.2/m6anet/model/model_states/human_hct116.pt`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/model/norm_factors/norm_factors_hct116.joblib` & `m6anet-2.0.2/m6anet/model/norm_factors/norm_factors_hct116.joblib`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/scripts/compute_norm_factors.py` & `m6anet-2.0.2/m6anet/scripts/compute_norm_factors.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/scripts/convert.py` & `m6anet-2.0.2/m6anet/scripts/convert.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/scripts/dataprep.py` & `m6anet-2.0.2/m6anet/scripts/dataprep.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/scripts/inference.py` & `m6anet-2.0.2/m6anet/scripts/inference.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/scripts/train.py` & `m6anet-2.0.2/m6anet/scripts/train.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/utils/builder.py` & `m6anet-2.0.2/m6anet/utils/builder.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/utils/constants.py` & `m6anet-2.0.2/m6anet/utils/constants.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/utils/data_utils.py` & `m6anet-2.0.2/m6anet/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/utils/dataprep_utils.py` & `m6anet-2.0.2/m6anet/utils/dataprep_utils.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/utils/helper.py` & `m6anet-2.0.2/m6anet/utils/helper.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/utils/inference_utils.py` & `m6anet-2.0.2/m6anet/utils/inference_utils.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/utils/loss_functions/loss_functions.py` & `m6anet-2.0.2/m6anet/utils/loss_functions/loss_functions.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/utils/norm_utils.py` & `m6anet-2.0.2/m6anet/utils/norm_utils.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/utils/sampler_utils.py` & `m6anet-2.0.2/m6anet/utils/sampler_utils.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet/utils/training_utils.py` & `m6anet-2.0.2/m6anet/utils/training_utils.py`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/m6anet.egg-info/PKG-INFO` & `m6anet-2.0.2/m6anet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: m6anet
-Version: 2.0.1
+Version: 2.0.2
 Summary: m6anet is a python package for detection of m6a modifications from Nanopore direct RNA sequencing data.
 Home-page: https://github.com/GoekeLab/m6anet
 Author: Christopher Hendra
 Maintainer-email: christopher.hendra@u.nus.edu
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.7
+Requires-Python: >=3.7, <3.9
 License-File: LICENSE
 
 # m6anet
 ![alt text](https://github.com/GoekeLab/m6anet/blob/master/figures/m6anet_logo.png "m6anet")
 
 m6anet is a python tool that leverages Multiple Instance Learning framework to detect m6a modifications from Nanopore Direct RNA Sequencing data
```

### Comparing `m6anet-2.0.1/m6anet.egg-info/SOURCES.txt` & `m6anet-2.0.2/m6anet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m6anet-2.0.1/setup.py` & `m6anet-2.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,25 +22,27 @@
     license="MIT",
     description='m6anet is a python package for detection of m6a modifications from Nanopore direct RNA sequencing data.',
     version=__version__,
     long_description=README,
     url='https://github.com/GoekeLab/m6anet',
     packages=find_packages(),
     package_data={'m6anet.model': ['model_states/human_hct116.pt', 'configs/model_configs/m6anet.toml', 'norm_factors/norm_factors_hct116.joblib']},
-    python_requires=">=3.7",
+    python_requires=">=3.7, <3.9",
     install_requires=[
-            'numpy==1.18.0',
-            'pandas==0.25.3',
-            'scikit-learn==0.24.1',
-            'scipy==1.4.1',
-            'ujson',
-            'torch==1.6.0',
-            'toml==0.10.2',
-            'tqdm',
-            'typing-extensions'
+            "numpy>=1.18.0",
+            "pandas>=0.25.3",
+            "scikit-learn>=0.24.0, <1.1.0; python_version=='3.7'",
+            "scikit-learn>=0.24.0; python_version=='3.8'",
+            "scipy>=1.4.1, <1.8.0; python_version=='3.7'",
+            "scipy>=1.4.1; python_version=='3.8'",
+            "ujson",
+            "torch==1.6.0",
+            "toml>=0.10.2",
+            "tqdm",
+            "typing-extensions"
             ],
     entry_points = {
         'console_scripts': [
             '{0} = {0}:main'.format(__pkg_name__),
             "m6anet-dataprep={}.deprecated.dataprep:main".format(__pkg_name__),
             "m6anet-run_inference={}.deprecated.inference:main".format(__pkg_name__),
             "m6anet-compute_norm_factors={}.deprecated.compute_norm_factors:main".format(__pkg_name__),
```


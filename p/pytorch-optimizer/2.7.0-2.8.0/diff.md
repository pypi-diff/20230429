# Comparing `tmp/pytorch_optimizer-2.7.0.tar.gz` & `tmp/pytorch_optimizer-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_optimizer-2.7.0.tar", max compression
+gzip compressed data, was "pytorch_optimizer-2.8.0.tar", max compression
```

## Comparing `pytorch_optimizer-2.7.0.tar` & `pytorch_optimizer-2.8.0.tar`

### file list

```diff
@@ -1,54 +1,65 @@
--rw-r--r--   0        0        0    11357 2023-04-26 06:31:20.902848 pytorch_optimizer-2.7.0/LICENSE
--rw-r--r--   0        0        0    30085 2023-04-26 06:31:20.902848 pytorch_optimizer-2.7.0/README.rst
--rw-r--r--   0        0        0     3698 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pyproject.toml
--rw-r--r--   0        0        0     6133 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/base/__init__.py
--rw-r--r--   0        0        0     1583 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/base/exception.py
--rw-r--r--   0        0        0     4183 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/base/optimizer.py
--rw-r--r--   0        0        0     2761 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/base/scheduler.py
--rw-r--r--   0        0        0      491 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/base/types.py
--rw-r--r--   0        0        0        0 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/experimental/__init__.py
--rw-r--r--   0        0        0     1595 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py
--rw-r--r--   0        0        0      131 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/lr_scheduler/__init__.py
--rw-r--r--   0        0        0      971 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/lr_scheduler/chebyshev.py
--rw-r--r--   0        0        0     4034 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/lr_scheduler/cosine_anealing.py
--rw-r--r--   0        0        0     1255 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/lr_scheduler/linear_warmup.py
--rw-r--r--   0        0        0     1400 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/lr_scheduler/proportion.py
--rw-r--r--   0        0        0        0 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/__init__.py
--rw-r--r--   0        0        0     7547 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adabelief.py
--rw-r--r--   0        0        0     5515 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adabound.py
--rw-r--r--   0        0        0     8416 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adafactor.py
--rw-r--r--   0        0        0     6037 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adai.py
--rw-r--r--   0        0        0     6169 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adamp.py
--rw-r--r--   0        0        0     6089 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adams.py
--rw-r--r--   0        0        0     6544 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adan.py
--rw-r--r--   0        0        0     5424 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adanorm.py
--rw-r--r--   0        0        0     6142 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adapnm.py
--rw-r--r--   0        0        0      781 2023-04-26 06:31:20.906848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/agc.py
--rw-r--r--   0        0        0     3873 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/alig.py
--rw-r--r--   0        0        0     5498 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/apollo.py
--rw-r--r--   0        0        0    24966 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/dadapt.py
--rw-r--r--   0        0        0     7250 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/diffgrad.py
--rw-r--r--   0        0        0    10702 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/fp16.py
--rw-r--r--   0        0        0      474 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/gc.py
--rw-r--r--   0        0        0     7601 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/gsam.py
--rw-r--r--   0        0        0     8607 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/lamb.py
--rw-r--r--   0        0        0     3923 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/lars.py
--rw-r--r--   0        0        0     2972 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/lion.py
--rw-r--r--   0        0        0     4178 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/lookahead.py
--rw-r--r--   0        0        0     6550 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/madgrad.py
--rw-r--r--   0        0        0     3639 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/nero.py
--rw-r--r--   0        0        0     4188 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/novograd.py
--rw-r--r--   0        0        0     4314 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/pcgrad.py
--rw-r--r--   0        0        0     3615 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/pnm.py
--rw-r--r--   0        0        0     5748 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/radam.py
--rw-r--r--   0        0        0     6969 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/ranger.py
--rw-r--r--   0        0        0    12435 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/ranger21.py
--rw-r--r--   0        0        0    15565 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/rotograd.py
--rw-r--r--   0        0        0     4718 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/sam.py
--rw-r--r--   0        0        0     3907 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/sgdp.py
--rw-r--r--   0        0        0    15801 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/shampoo.py
--rw-r--r--   0        0        0    20180 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/shampoo_utils.py
--rw-r--r--   0        0        0     5123 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/sm3.py
--rw-r--r--   0        0        0     8880 2023-04-26 06:31:20.910848 pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/utils.py
--rw-r--r--   0        0        0    32201 1970-01-01 00:00:00.000000 pytorch_optimizer-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-29 08:52:01.235538 pytorch_optimizer-2.8.0/LICENSE
+-rw-r--r--   0        0        0    38338 2023-04-29 08:52:01.235538 pytorch_optimizer-2.8.0/README.rst
+-rw-r--r--   0        0        0     3807 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6858 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/base/__init__.py
+-rw-r--r--   0        0        0     1583 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/base/exception.py
+-rw-r--r--   0        0        0     5782 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/base/optimizer.py
+-rw-r--r--   0        0        0     2761 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/base/scheduler.py
+-rw-r--r--   0        0        0      491 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/base/types.py
+-rw-r--r--   0        0        0        0 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/experimental/__init__.py
+-rw-r--r--   0        0        0     1595 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py
+-rw-r--r--   0        0        0      131 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/lr_scheduler/__init__.py
+-rw-r--r--   0        0        0      971 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/lr_scheduler/chebyshev.py
+-rw-r--r--   0        0        0     4034 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/lr_scheduler/cosine_anealing.py
+-rw-r--r--   0        0        0     1255 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/lr_scheduler/linear_warmup.py
+-rw-r--r--   0        0        0     1400 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/lr_scheduler/proportion.py
+-rw-r--r--   0        0        0        0 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/__init__.py
+-rw-r--r--   0        0        0     4401 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/a2grad.py
+-rw-r--r--   0        0        0     7547 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adabelief.py
+-rw-r--r--   0        0        0     5515 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adabound.py
+-rw-r--r--   0        0        0     8416 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adafactor.py
+-rw-r--r--   0        0        0     6037 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adai.py
+-rw-r--r--   0        0        0     4543 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adamod.py
+-rw-r--r--   0        0        0     6166 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adamp.py
+-rw-r--r--   0        0        0     6089 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adams.py
+-rw-r--r--   0        0        0     6544 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adan.py
+-rw-r--r--   0        0        0     5438 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adanorm.py
+-rw-r--r--   0        0        0     6142 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adapnm.py
+-rw-r--r--   0        0        0      781 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/agc.py
+-rw-r--r--   0        0        0     3113 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/aggmo.py
+-rw-r--r--   0        0        0     3873 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/alig.py
+-rw-r--r--   0        0        0     5498 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/apollo.py
+-rw-r--r--   0        0        0    24966 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/dadapt.py
+-rw-r--r--   0        0        0     7250 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/diffgrad.py
+-rw-r--r--   0        0        0    10702 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/fp16.py
+-rw-r--r--   0        0        0     2861 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/fromage.py
+-rw-r--r--   0        0        0      474 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/gc.py
+-rw-r--r--   0        0        0     7601 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/gsam.py
+-rw-r--r--   0        0        0     8607 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/lamb.py
+-rw-r--r--   0        0        0     3923 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/lars.py
+-rw-r--r--   0        0        0     4228 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/lion.py
+-rw-r--r--   0        0        0     4178 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/lookahead.py
+-rw-r--r--   0        0        0     6550 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/madgrad.py
+-rw-r--r--   0        0        0     3264 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/msvag.py
+-rw-r--r--   0        0        0     3639 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/nero.py
+-rw-r--r--   0        0        0     4188 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/novograd.py
+-rw-r--r--   0        0        0     4314 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/pcgrad.py
+-rw-r--r--   0        0        0     4146 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/pid.py
+-rw-r--r--   0        0        0     3615 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/pnm.py
+-rw-r--r--   0        0        0     4810 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/qhadam.py
+-rw-r--r--   0        0        0     3286 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/qhm.py
+-rw-r--r--   0        0        0     5748 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/radam.py
+-rw-r--r--   0        0        0     6969 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/ranger.py
+-rw-r--r--   0        0        0    12435 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/ranger21.py
+-rw-r--r--   0        0        0    15565 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/rotograd.py
+-rw-r--r--   0        0        0     4722 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/sam.py
+-rw-r--r--   0        0        0    10706 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/sgd.py
+-rw-r--r--   0        0        0     3921 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/sgdp.py
+-rw-r--r--   0        0        0    15801 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/shampoo.py
+-rw-r--r--   0        0        0    20180 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/shampoo_utils.py
+-rw-r--r--   0        0        0     5123 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/sm3.py
+-rw-r--r--   0        0        0     7169 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/swats.py
+-rw-r--r--   0        0        0     8880 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/utils.py
+-rw-r--r--   0        0        0     5115 2023-04-29 08:52:01.243538 pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/yogi.py
+-rw-r--r--   0        0        0    40454 1970-01-01 00:00:00.000000 pytorch_optimizer-2.8.0/PKG-INFO
```

### Comparing `pytorch_optimizer-2.7.0/LICENSE` & `pytorch_optimizer-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/README.rst` & `pytorch_optimizer-2.8.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -10,23 +10,28 @@
 | Package      | |PyPI version| |PyPI pyversions|         |
 +--------------+------------------------------------------+
 | Status       | |PyPi download| |PyPi month download|    |
 +--------------+------------------------------------------+
 | License      | |apache|                                 |
 +--------------+------------------------------------------+
 
-| **pytorch-optimizer** is bunch of optimizer collections in PyTorch. Also, including useful optimization ideas.
-| Most of the implementations are based on the original paper, but I added some tweaks.
+| **pytorch-optimizer** is optimizer & lr scheduler collections in PyTorch.
+| I just re-implemented (speed & memory tweaks, plug-ins) the algorithm while based on the original paper. Also, It includes useful and practical optimization ideas.
+| Currently, 43 optimizers, 6 lr schedulers are supported!
+|
 | Highly inspired by `pytorch-optimizer <https://github.com/jettify/pytorch-optimizer>`__.
 
 Getting Started
 ---------------
 
 For more, see the `documentation <https://pytorch-optimizers.readthedocs.io/en/latest/>`__.
 
+Most optimizers are under MIT or Apache 2.0 license, but a few optimizers like `Fromage` have BY-NC-SA 4.0 license, which is non-commercial.
+So, please double-check the license before using it at your work.
+
 Installation
 ~~~~~~~~~~~~
 
 ::
 
     $ pip3 install -U pytorch-optimizer
 
@@ -140,14 +145,38 @@
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 | SM3          | *Memory-Efficient Adaptive Optimization*                                                        | `github <https://github.com/google-research/google-research/tree/master/sm3>`__   | `https://arxiv.org/abs/1901.11150 <https://arxiv.org/abs/1901.11150>`__                       |
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 | AdaNorm      | *Adaptive Gradient Norm Correction based Optimizer for CNNs*                                    | `github <https://github.com/shivram1987/AdaNorm>`__                               | `https://arxiv.org/abs/2210.06364 <https://arxiv.org/abs/2210.06364>`__                       |
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 | RotoGrad     | *Gradient Homogenization in Multitask Learning*                                                 | `github <https://github.com/adrianjav/rotograd>`__                                | `https://openreview.net/pdf?id=T8wHz4rnuGL <https://openreview.net/pdf?id=T8wHz4rnuGL>`__     |
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| A2Grad       | *Optimal Adaptive and Accelerated Stochastic Gradient Descent*                                  | `github <https://github.com/severilov/A2Grad_optimizer>`__                        | `https://arxiv.org/abs/1810.00553 <https://arxiv.org/abs/1810.00553>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| AccSGD       | *Accelerating Stochastic Gradient Descent For Least Squares Regression*                         | `github <https://github.com/rahulkidambi/AccSGD>`__                               | `https://arxiv.org/abs/1704.08227 <https://arxiv.org/abs/1704.08227>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| SGDW         | *Decoupled Weight Decay Regularization*                                                         | `github <https://github.com/loshchil/AdamW-and-SGDW>`__                           | `https://arxiv.org/abs/1711.05101 <https://arxiv.org/abs/1711.05101>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| ASGD         | *Adaptive Gradient Descent without Descent*                                                     | `github <https://github.com/ymalitsky/adaptive_GD>`__                             | `https://arxiv.org/abs/1910.09529 <https://arxiv.org/abs/1910.09529>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| Yogi         | *Adaptive Methods for Nonconvex Optimization*                                                   |                                                                                   | `NIPS 2018 <https://papers.nips.cc/paper/8186-adaptive-methods-for-nonconvex-optimization>`__ |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| SWATS        | *Improving Generalization Performance by Switching from Adam to SGD*                            |                                                                                   | `https://arxiv.org/abs/1712.07628 <https://arxiv.org/abs/1712.07628>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| Fromage      | *On the distance between two neural networks and the stability of learning*                     | `github <https://github.com/jxbz/fromage>`__                                      | `https://arxiv.org/abs/2002.03432 <https://arxiv.org/abs/2002.03432>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| MSVAG        | *Dissecting Adam: The Sign, Magnitude and Variance of Stochastic Gradients*                     | `github <https://github.com/lballes/msvag>`__                                     | `https://arxiv.org/abs/1705.07774 <https://arxiv.org/abs/1705.07774>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| AdaMod       | *An Adaptive and Momental Bound Method for Stochastic Learning*                                 | `github <https://github.com/lancopku/AdaMod>`__                                   | `https://arxiv.org/abs/1910.12249 <https://arxiv.org/abs/1910.12249>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| AggMo        | *Aggregated Momentum: Stability Through Passive Damping*                                        | `github <https://github.com/AtheMathmo/AggMo>`__                                  | `https://arxiv.org/abs/1804.00325 <https://arxiv.org/abs/1804.00325>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| QHAdam       | *Quasi-hyperbolic momentum and Adam for deep learning*                                          | `github <https://github.com/facebookresearch/qhoptim>`__                          | `https://arxiv.org/abs/1810.06801 <https://arxiv.org/abs/1810.06801>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| PID          | *A PID Controller Approach for Stochastic Optimization of Deep Networks*                        | `github <https://github.com/tensorboy/PIDOptimizer>`__                            | `CVPR 18 <http://www4.comp.polyu.edu.hk/~cslzhang/paper/CVPR18_PID.pdf>`__                    |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 
 Useful Resources
 ----------------
 
 Several optimization ideas to regularize & stabilize the training. Most
 of the ideas are applied in ``Ranger21`` optimizer.
 
@@ -351,26 +380,50 @@
 
 `SM3 <https://ui.adsabs.harvard.edu/abs/2019arXiv190111150A/exportcitation>`__
 
 `AdaNorm <https://github.com/shivram1987/AdaNorm/tree/main#citation>`__
 
 `RotoGrad <https://github.com/adrianjav/rotograd#citing>`__
 
+`A2Grad <https://ui.adsabs.harvard.edu/abs/2018arXiv181000553D/exportcitation>`__
+
+`AccSGD <https://github.com/rahulkidambi/AccSGD#citation>`__
+
+`SGDW <https://github.com/loshchil/AdamW-and-SGDW#contact>`__
+
+`Adaptive SGD <https://github.com/ymalitsky/adaptive_GD#reference>`__
+
+`Yogi <https://proceedings.neurips.cc/paper_files/paper/2018/hash/90365351ccc7437a1309dc64e4db32a3-Abstract.html>`__
+
+`SWATS <https://ui.adsabs.harvard.edu/abs/2017arXiv171207628S/exportcitation>`__
+
+`Fromage <https://github.com/jxbz/fromage#citation>`__
+
+`MSVAG <https://github.com/lballes/msvag#citation>`__
+
+`AdaMod <https://github.com/lancopku/AdaMod#citation>`__
+
+`AggMo <https://ui.adsabs.harvard.edu/abs/2018arXiv180400325L/exportcitation>`__
+
+`QHAdam <https://github.com/facebookresearch/qhoptim#reference>`__
+
+`PID <https://github.com/tensorboy/PIDOptimizer#citation>`__
+
 Citation
 --------
 
 Please cite original authors of optimization algorithms. If you use this software, please cite it as below.
 Or you can get from "cite this repository" button.
 
 ::
 
-    @software{Kim_pytorch_optimizer_Bunch_of_2022,
+    @software{Kim_pytorch_optimizer_Optimizer_and_2022,
         author = {Kim, Hyeongchan},
         month = {1},
-        title = {{pytorch_optimizer: optimizer & lr scheduler implementations in PyTorch}},
+        title = {{pytorch_optimizer: optimizer and lr scheduler collections in PyTorch}},
         version = {1.0.0},
         year = {2022}
     }
 
 Author
 ------
```

### Comparing `pytorch_optimizer-2.7.0/pyproject.toml` & `pytorch_optimizer-2.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytorch_optimizer"
-version = "2.7.0"
+version = "2.8.0"
 description = "optimizer & lr scheduler implementations in PyTorch with clean-code, strict types. Also, including useful optimization ideas."
 license = "Apache-2.0"
 authors = ["kozistr <kozistr@gmail.com>"]
 maintainers = ["kozistr <kozistr@gmail.com>"]
 readme = "README.rst"
 homepage = "https://github.com/kozistr/pytorch_optimizer"
 repository = "https://github.com/kozistr/pytorch_optimizer"
@@ -87,25 +87,27 @@
 "./tests/__init__.py" = ["D"]
 "./tests/constants.py" = ["D"]
 "./tests/utils.py" = ["D"]
 "./tests/test_utils.py" = ["D", "S101"]
 "./tests/test_gradients.py" = ["D", "S101"]
 "./tests/test_optimizers.py" = ["D", "S101"]
 "./tests/test_optimizer_parameters.py" = ["D", "S101"]
+"./tests/test_general_optimizer_parameters.py" = ["D", "S101"]
 "./tests/test_load_optimizers.py" = ["D", "S101"]
 "./tests/test_load_lr_schedulers.py" = ["D", "S101"]
 "./tests/test_lr_schedulers.py" = ["D"]
 "./tests/test_lr_scheduler_parameters.py" = ["D", "S101"]
 "./tests/test_create_optimizer.py" = ["D"]
 "./pytorch_optimizer/__init__.py" = ["F401"]
 "./pytorch_optimizer/lr_scheduler/__init__.py" = ["F401"]
 
 [tool.coverage.run]
 omit = [
     "./pytorch_optimizer/optimizer/gsam.py",
     "./pytorch_optimizer/optimizer/fp16.py",
     "./pytorch_optimizer/optimizer/rotograd.py",
+    "./pytorch_optimizer/optimizer/swats.py",
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/__init__.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,45 +12,54 @@
     CyclicLR,
     OneCycleLR,
 )
 from pytorch_optimizer.lr_scheduler.chebyshev import get_chebyshev_schedule
 from pytorch_optimizer.lr_scheduler.cosine_anealing import CosineAnnealingWarmupRestarts
 from pytorch_optimizer.lr_scheduler.linear_warmup import CosineScheduler, LinearScheduler, PolyScheduler
 from pytorch_optimizer.lr_scheduler.proportion import ProportionScheduler
+from pytorch_optimizer.optimizer.a2grad import A2Grad
 from pytorch_optimizer.optimizer.adabelief import AdaBelief
 from pytorch_optimizer.optimizer.adabound import AdaBound
 from pytorch_optimizer.optimizer.adafactor import AdaFactor
 from pytorch_optimizer.optimizer.adai import Adai
+from pytorch_optimizer.optimizer.adamod import AdaMod
 from pytorch_optimizer.optimizer.adamp import AdamP
 from pytorch_optimizer.optimizer.adams import AdamS
 from pytorch_optimizer.optimizer.adan import Adan
 from pytorch_optimizer.optimizer.adanorm import AdaNorm
 from pytorch_optimizer.optimizer.adapnm import AdaPNM
 from pytorch_optimizer.optimizer.agc import agc
+from pytorch_optimizer.optimizer.aggmo import AggMo
 from pytorch_optimizer.optimizer.alig import AliG
 from pytorch_optimizer.optimizer.apollo import Apollo
 from pytorch_optimizer.optimizer.dadapt import DAdaptAdaGrad, DAdaptAdam, DAdaptAdan, DAdaptSGD
 from pytorch_optimizer.optimizer.diffgrad import DiffGrad
 from pytorch_optimizer.optimizer.fp16 import DynamicLossScaler, SafeFP16Optimizer
+from pytorch_optimizer.optimizer.fromage import Fromage
 from pytorch_optimizer.optimizer.gc import centralize_gradient
 from pytorch_optimizer.optimizer.gsam import GSAM
 from pytorch_optimizer.optimizer.lamb import Lamb
 from pytorch_optimizer.optimizer.lars import LARS
 from pytorch_optimizer.optimizer.lion import Lion
 from pytorch_optimizer.optimizer.lookahead import Lookahead
 from pytorch_optimizer.optimizer.madgrad import MADGRAD
+from pytorch_optimizer.optimizer.msvag import MSVAG
 from pytorch_optimizer.optimizer.nero import Nero
 from pytorch_optimizer.optimizer.novograd import NovoGrad
 from pytorch_optimizer.optimizer.pcgrad import PCGrad
+from pytorch_optimizer.optimizer.pid import PID
 from pytorch_optimizer.optimizer.pnm import PNM
+from pytorch_optimizer.optimizer.qhadam import QHAdam
+from pytorch_optimizer.optimizer.qhm import QHM
 from pytorch_optimizer.optimizer.radam import RAdam
 from pytorch_optimizer.optimizer.ranger import Ranger
 from pytorch_optimizer.optimizer.ranger21 import Ranger21
 from pytorch_optimizer.optimizer.rotograd import RotoGrad
 from pytorch_optimizer.optimizer.sam import SAM
+from pytorch_optimizer.optimizer.sgd import ASGD, SGDW, AccSGD
 from pytorch_optimizer.optimizer.sgdp import SGDP
 from pytorch_optimizer.optimizer.shampoo import ScalableShampoo, Shampoo
 from pytorch_optimizer.optimizer.shampoo_utils import (
     AdaGradGraft,
     BlockPartitioner,
     Graft,
     LayerWiseGrafting,
@@ -61,56 +70,71 @@
     SQRTNGraft,
     compute_power_schur_newton,
     compute_power_svd,
     merge_small_dims,
     power_iteration,
 )
 from pytorch_optimizer.optimizer.sm3 import SM3
+from pytorch_optimizer.optimizer.swats import SWATS
 from pytorch_optimizer.optimizer.utils import (
     clip_grad_norm,
     disable_running_stats,
     enable_running_stats,
     get_global_gradient_norm,
     get_optimizer_parameters,
     normalize_gradient,
     reduce_max_except_dim,
     unit_norm,
 )
+from pytorch_optimizer.optimizer.yogi import Yogi
 
 OPTIMIZER_LIST: List[OPTIMIZER] = [
     AdaBelief,
     AdaBound,
+    PID,
     AdamP,
     Adai,
     Adan,
+    AdaMod,
     AdaPNM,
     DiffGrad,
     Lamb,
     LARS,
+    QHAdam,
+    QHM,
     MADGRAD,
     Nero,
     PNM,
+    MSVAG,
     RAdam,
     Ranger,
     Ranger21,
     SGDP,
     Shampoo,
     ScalableShampoo,
     DAdaptAdaGrad,
+    Fromage,
+    AggMo,
     DAdaptAdam,
     DAdaptSGD,
     DAdaptAdan,
     AdamS,
     AdaFactor,
     Apollo,
+    SWATS,
     NovoGrad,
     Lion,
     AliG,
     SM3,
     AdaNorm,
+    A2Grad,
+    AccSGD,
+    SGDW,
+    Yogi,
+    ASGD,
 ]
 OPTIMIZERS: Dict[str, OPTIMIZER] = {str(optimizer.__name__).lower(): optimizer for optimizer in OPTIMIZER_LIST}
 
 LR_SCHEDULER_LIST: List[SCHEDULER] = [
     CosineAnnealingWarmupRestarts,
     ConstantLR,
     CosineAnnealingLR,
```

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/base/exception.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/base/exception.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/base/optimizer.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/base/optimizer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC, abstractmethod
+from typing import Tuple, Union
 
 import torch
 
 from pytorch_optimizer.base.exception import NegativeLRError, NegativeStepError
 from pytorch_optimizer.base.types import BETAS
 
 
@@ -107,14 +108,55 @@
             raise ValueError(f'[-] norm {norm} must be positive')
 
     @staticmethod
     def validate_rebound(rebound: str):
         if rebound not in ('constant', 'belief'):
             raise ValueError(f'[-] rebound {rebound} must be one of (\'constant\' or \'belief\')')
 
+    @staticmethod
+    def validate_lipschitz_constant(lips: float):
+        if lips < 0:
+            raise ValueError(f'[-] Lipschitz constant {lips} must be non-negative')
+
+    @staticmethod
+    def validate_a2grad_variant(variant: str):
+        if variant not in ('uni', 'inc', 'exp'):
+            raise ValueError(f'[-] A2Grad variant {variant} must be one of (\'uni\' or \'inc\' or \'exp\')')
+
+    @staticmethod
+    def validate_kappa(kappa: float):
+        if kappa < 0.0:
+            raise ValueError(f'[-] kappa {kappa} must be non-negative')
+
+    @staticmethod
+    def validate_xi(xi: float):
+        if xi < 0.0:
+            raise ValueError(f'[-] xi {xi} must be non-negative')
+
+    @staticmethod
+    def validate_constant(constant: float, boundary: float):
+        if constant > boundary:
+            raise ValueError(f'[-] constant {constant} must be in a range of (-inf, {boundary}]')
+
+    @staticmethod
+    def validate_amplifier(amplifier: float):
+        if amplifier < 0.0:
+            raise ValueError(f'[-] amplifier {amplifier} must be non-negative')
+
+    @staticmethod
+    def validate_nus(nus: Union[float, Tuple[float, float]]):
+        if isinstance(nus, float):
+            if not 0.0 <= nus <= 1.0:
+                raise ValueError(f'[-] nus {nus} must be in the range [0, 1]')
+        else:
+            if not 0.0 <= nus[0] <= 1.0:
+                raise ValueError(f'[-] nus1 {nus[0]} must be in the range [0, 1]')
+            if not 0.0 <= nus[1] <= 1.0:
+                raise ValueError(f'[-] nus2 {nus[1]} must be in the range [0, 1]')
+
     @abstractmethod
     def validate_parameters(self):
         raise NotImplementedError
 
     @abstractmethod
     @torch.no_grad()
     def reset(self):
```

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/base/scheduler.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/base/scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/experimental/deberta_v3_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/lr_scheduler/chebyshev.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/lr_scheduler/chebyshev.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/lr_scheduler/cosine_anealing.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/lr_scheduler/cosine_anealing.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/lr_scheduler/linear_warmup.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/lr_scheduler/linear_warmup.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/lr_scheduler/proportion.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/lr_scheduler/proportion.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adabelief.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adabelief.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adabound.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adabound.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adafactor.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adafactor.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adai.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adai.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adamp.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
                     if exp_grad_norm > grad_norm:
                         s_grad *= exp_grad_norm / grad_norm
 
                 exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
                 exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
-                inv_de_nom = 1.0 / (exp_avg_sq.sqrt() / bias_correction2_sq).add_(group['eps'])
+                inv_de_nom = exp_avg_sq.rsqrt().add_(group['eps']).mul_(bias_correction2_sq)
 
                 perturb = exp_avg.clone()
                 if group['nesterov']:
                     perturb.mul_(beta1).addcmul_(grad, inv_de_nom, value=1.0 - beta1)
                 else:
                     perturb.mul_(inv_de_nom)
```

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adams.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adams.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adan.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adan.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adanorm.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adanorm.py`

 * *Files 5% similar despite different names*

```diff
@@ -130,17 +130,17 @@
                 exp_avg, exp_avg_var = state['exp_avg'], state['exp_avg_var']
                 exp_avg.mul_(beta1).add_(s_grad, alpha=1.0 - beta1)
                 exp_avg_var.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
 
                 if group['amsgrad']:
                     max_exp_avg_var = state['max_exp_avg_var']
                     torch.max(max_exp_avg_var, exp_avg_var, out=max_exp_avg_var)
-                    de_nom = max_exp_avg_var.add(self.eps).sqrt()
+                    de_nom = max_exp_avg_var.sqrt().add_(group['eps'])
                 else:
-                    de_nom = exp_avg_var.add(self.eps).sqrt()
+                    de_nom = exp_avg_var.sqrt().add_(group['eps'])
 
-                de_nom.div_(bias_correction2_sq).add_(self.eps)
+                de_nom.div_(bias_correction2_sq).add_(group['eps'])
 
                 step_size = group['lr'] if group['adam_debias'] else group['lr'] / bias_correction1
                 p.addcdiv_(exp_avg, de_nom, value=-step_size)
 
         return loss
```

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/adapnm.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/adapnm.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/agc.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/agc.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/alig.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/alig.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/apollo.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/apollo.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/dadapt.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/dadapt.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/diffgrad.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/diffgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/fp16.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/fp16.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/gsam.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/gsam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/lamb.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/lamb.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/lars.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/lars.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/lion.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/aggmo.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 from torch.optim.optimizer import Optimizer
 
 from pytorch_optimizer.base.exception import NoSparseGradientError
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
 
 
-class Lion(Optimizer, BaseOptimizer):
-    r"""Symbolic Discovery of Optimization Algorithms.
+class AggMo(Optimizer, BaseOptimizer):
+    r"""Aggregated Momentum: Stability Through Passive Damping.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
-        lr: float = 1e-4,
-        betas: BETAS = (0.9, 0.99),
+        lr: float = 1e-3,
+        betas: BETAS = (0.0, 0.9, 0.99),
         weight_decay: float = 0.0,
-        weight_decouple: bool = True,
+        weight_decouple: bool = False,
     ):
         self.lr = lr
         self.betas = betas
         self.weight_decay = weight_decay
 
         self.validate_parameters()
 
@@ -40,54 +40,58 @@
 
     def validate_parameters(self):
         self.validate_learning_rate(self.lr)
         self.validate_betas(self.betas)
         self.validate_weight_decay(self.weight_decay)
 
     def __str__(self) -> str:
-        return 'Lion'
+        return 'AggMo'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
-                state['exp_avg'] = torch.zeros_like(p)
+                state['momentum_buffer'] = {beta: torch.zeros_like(p) for beta in group['betas']}
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
-            beta1, beta2 = group['betas']
-            weight_decay = group['weight_decay']
+            if 'step' in group:
+                group['step'] += 1
+            else:
+                group['step'] = 1
+
+            betas = group['betas']
+
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
                 if grad.is_sparse:
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
 
                 if len(state) == 0:
-                    state['exp_avg'] = torch.zeros_like(p)
-
-                update = exp_avg = state['exp_avg']
-
-                if weight_decay > 0.0:
-                    if group['weight_decouple']:
-                        p.mul_(1.0 - group['lr'] * weight_decay)
-                    else:
-                        grad.add_(p, alpha=weight_decay)
+                    state['momentum_buffer'] = {beta: torch.zeros_like(p) for beta in betas}
 
-                update.mul_(beta1).add_(grad, alpha=1.0 - beta1)
-                exp_avg.mul_(beta2).add_(grad, alpha=1.0 - beta2)
+                if group['weight_decouple']:
+                    p.mul_(1.0 - group['weight_decay'] * group['lr'])
+                elif group['weight_decay'] > 0.0:
+                    grad.add_(p, alpha=group['weight_decay'])
+
+                for beta in betas:
+                    buf = state['momentum_buffer'][beta]
+                    buf.mul_(beta).add_(grad)
 
-                p.add_(update.sign(), alpha=-group['lr'])
+                    p.add_(buf, alpha=-group['lr'] / len(betas))
 
         return loss
```

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/lookahead.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/lookahead.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/madgrad.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/madgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/nero.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/nero.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/novograd.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/novograd.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/pcgrad.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/pcgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/pnm.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/pnm.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/radam.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/radam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/ranger.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/ranger.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/ranger21.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/ranger21.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/rotograd.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/rotograd.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/sam.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/sam.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,18 +44,18 @@
 
             for input, output in data:
                 loss = loss_function(output, model(input))
                 loss.backward()
                 optimizer.step(closure)
                 optimizer.zero_grad()
 
-    :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups
-    :param base_optimizer: Optimizer. base optimizer
-    :param rho: float. size of the neighborhood for computing the max loss
-    :param adaptive: bool. element-wise Adaptive SAM
+    :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
+    :param base_optimizer: Optimizer. base optimizer.
+    :param rho: float. size of the neighborhood for computing the max loss.
+    :param adaptive: bool. element-wise Adaptive SAM.
     :param kwargs: Dict. parameters for optimizer.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         base_optimizer: OPTIMIZER,
```

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/sgdp.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/sgdp.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,17 +90,17 @@
                 state = self.state[p]
                 if len(state) == 0:
                     state['momentum'] = torch.zeros_like(p)
 
                 buf = state['momentum']
                 buf.mul_(momentum).add_(grad, alpha=1.0 - group['dampening'])
 
-                d_p = buf
+                d_p = buf.clone()
                 if group['nesterov']:
-                    d_p.mul_(momentum).add_(grad)
+                    d_p = d_p.mul_(momentum).add_(grad)
 
                 wd_ratio: float = 1.0
                 if len(p.shape) > 1:
                     d_p, wd_ratio = projection(
                         p,
                         grad,
                         d_p,
```

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/shampoo.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/shampoo.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/shampoo_utils.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/shampoo_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/sm3.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/sm3.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/pytorch_optimizer/optimizer/utils.py` & `pytorch_optimizer-2.8.0/pytorch_optimizer/optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.7.0/PKG-INFO` & `pytorch_optimizer-2.8.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-optimizer
-Version: 2.7.0
+Version: 2.8.0
 Summary: optimizer & lr scheduler implementations in PyTorch with clean-code, strict types. Also, including useful optimization ideas.
 Home-page: https://github.com/kozistr/pytorch_optimizer
 License: Apache-2.0
 Keywords: pytorch,deep-learning,optimizer,lr scheduler
 Author: kozistr
 Author-email: kozistr@gmail.com
 Maintainer: kozistr
@@ -53,23 +53,28 @@
 | Package      | |PyPI version| |PyPI pyversions|         |
 +--------------+------------------------------------------+
 | Status       | |PyPi download| |PyPi month download|    |
 +--------------+------------------------------------------+
 | License      | |apache|                                 |
 +--------------+------------------------------------------+
 
-| **pytorch-optimizer** is bunch of optimizer collections in PyTorch. Also, including useful optimization ideas.
-| Most of the implementations are based on the original paper, but I added some tweaks.
+| **pytorch-optimizer** is optimizer & lr scheduler collections in PyTorch.
+| I just re-implemented (speed & memory tweaks, plug-ins) the algorithm while based on the original paper. Also, It includes useful and practical optimization ideas.
+| Currently, 43 optimizers, 6 lr schedulers are supported!
+|
 | Highly inspired by `pytorch-optimizer <https://github.com/jettify/pytorch-optimizer>`__.
 
 Getting Started
 ---------------
 
 For more, see the `documentation <https://pytorch-optimizers.readthedocs.io/en/latest/>`__.
 
+Most optimizers are under MIT or Apache 2.0 license, but a few optimizers like `Fromage` have BY-NC-SA 4.0 license, which is non-commercial.
+So, please double-check the license before using it at your work.
+
 Installation
 ~~~~~~~~~~~~
 
 ::
 
     $ pip3 install -U pytorch-optimizer
 
@@ -183,14 +188,38 @@
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 | SM3          | *Memory-Efficient Adaptive Optimization*                                                        | `github <https://github.com/google-research/google-research/tree/master/sm3>`__   | `https://arxiv.org/abs/1901.11150 <https://arxiv.org/abs/1901.11150>`__                       |
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 | AdaNorm      | *Adaptive Gradient Norm Correction based Optimizer for CNNs*                                    | `github <https://github.com/shivram1987/AdaNorm>`__                               | `https://arxiv.org/abs/2210.06364 <https://arxiv.org/abs/2210.06364>`__                       |
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 | RotoGrad     | *Gradient Homogenization in Multitask Learning*                                                 | `github <https://github.com/adrianjav/rotograd>`__                                | `https://openreview.net/pdf?id=T8wHz4rnuGL <https://openreview.net/pdf?id=T8wHz4rnuGL>`__     |
 +--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| A2Grad       | *Optimal Adaptive and Accelerated Stochastic Gradient Descent*                                  | `github <https://github.com/severilov/A2Grad_optimizer>`__                        | `https://arxiv.org/abs/1810.00553 <https://arxiv.org/abs/1810.00553>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| AccSGD       | *Accelerating Stochastic Gradient Descent For Least Squares Regression*                         | `github <https://github.com/rahulkidambi/AccSGD>`__                               | `https://arxiv.org/abs/1704.08227 <https://arxiv.org/abs/1704.08227>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| SGDW         | *Decoupled Weight Decay Regularization*                                                         | `github <https://github.com/loshchil/AdamW-and-SGDW>`__                           | `https://arxiv.org/abs/1711.05101 <https://arxiv.org/abs/1711.05101>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| ASGD         | *Adaptive Gradient Descent without Descent*                                                     | `github <https://github.com/ymalitsky/adaptive_GD>`__                             | `https://arxiv.org/abs/1910.09529 <https://arxiv.org/abs/1910.09529>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| Yogi         | *Adaptive Methods for Nonconvex Optimization*                                                   |                                                                                   | `NIPS 2018 <https://papers.nips.cc/paper/8186-adaptive-methods-for-nonconvex-optimization>`__ |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| SWATS        | *Improving Generalization Performance by Switching from Adam to SGD*                            |                                                                                   | `https://arxiv.org/abs/1712.07628 <https://arxiv.org/abs/1712.07628>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| Fromage      | *On the distance between two neural networks and the stability of learning*                     | `github <https://github.com/jxbz/fromage>`__                                      | `https://arxiv.org/abs/2002.03432 <https://arxiv.org/abs/2002.03432>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| MSVAG        | *Dissecting Adam: The Sign, Magnitude and Variance of Stochastic Gradients*                     | `github <https://github.com/lballes/msvag>`__                                     | `https://arxiv.org/abs/1705.07774 <https://arxiv.org/abs/1705.07774>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| AdaMod       | *An Adaptive and Momental Bound Method for Stochastic Learning*                                 | `github <https://github.com/lancopku/AdaMod>`__                                   | `https://arxiv.org/abs/1910.12249 <https://arxiv.org/abs/1910.12249>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| AggMo        | *Aggregated Momentum: Stability Through Passive Damping*                                        | `github <https://github.com/AtheMathmo/AggMo>`__                                  | `https://arxiv.org/abs/1804.00325 <https://arxiv.org/abs/1804.00325>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| QHAdam       | *Quasi-hyperbolic momentum and Adam for deep learning*                                          | `github <https://github.com/facebookresearch/qhoptim>`__                          | `https://arxiv.org/abs/1810.06801 <https://arxiv.org/abs/1810.06801>`__                       |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
+| PID          | *A PID Controller Approach for Stochastic Optimization of Deep Networks*                        | `github <https://github.com/tensorboy/PIDOptimizer>`__                            | `CVPR 18 <http://www4.comp.polyu.edu.hk/~cslzhang/paper/CVPR18_PID.pdf>`__                    |
++--------------+-------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+
 
 Useful Resources
 ----------------
 
 Several optimization ideas to regularize & stabilize the training. Most
 of the ideas are applied in ``Ranger21`` optimizer.
 
@@ -394,26 +423,50 @@
 
 `SM3 <https://ui.adsabs.harvard.edu/abs/2019arXiv190111150A/exportcitation>`__
 
 `AdaNorm <https://github.com/shivram1987/AdaNorm/tree/main#citation>`__
 
 `RotoGrad <https://github.com/adrianjav/rotograd#citing>`__
 
+`A2Grad <https://ui.adsabs.harvard.edu/abs/2018arXiv181000553D/exportcitation>`__
+
+`AccSGD <https://github.com/rahulkidambi/AccSGD#citation>`__
+
+`SGDW <https://github.com/loshchil/AdamW-and-SGDW#contact>`__
+
+`Adaptive SGD <https://github.com/ymalitsky/adaptive_GD#reference>`__
+
+`Yogi <https://proceedings.neurips.cc/paper_files/paper/2018/hash/90365351ccc7437a1309dc64e4db32a3-Abstract.html>`__
+
+`SWATS <https://ui.adsabs.harvard.edu/abs/2017arXiv171207628S/exportcitation>`__
+
+`Fromage <https://github.com/jxbz/fromage#citation>`__
+
+`MSVAG <https://github.com/lballes/msvag#citation>`__
+
+`AdaMod <https://github.com/lancopku/AdaMod#citation>`__
+
+`AggMo <https://ui.adsabs.harvard.edu/abs/2018arXiv180400325L/exportcitation>`__
+
+`QHAdam <https://github.com/facebookresearch/qhoptim#reference>`__
+
+`PID <https://github.com/tensorboy/PIDOptimizer#citation>`__
+
 Citation
 --------
 
 Please cite original authors of optimization algorithms. If you use this software, please cite it as below.
 Or you can get from "cite this repository" button.
 
 ::
 
-    @software{Kim_pytorch_optimizer_Bunch_of_2022,
+    @software{Kim_pytorch_optimizer_Optimizer_and_2022,
         author = {Kim, Hyeongchan},
         month = {1},
-        title = {{pytorch_optimizer: optimizer & lr scheduler implementations in PyTorch}},
+        title = {{pytorch_optimizer: optimizer and lr scheduler collections in PyTorch}},
         version = {1.0.0},
         year = {2022}
     }
 
 Author
 ------
```


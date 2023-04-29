# Comparing `tmp/torchlayers-nightly-1682554018.tar.gz` & `tmp/torchlayers-nightly-1682640451.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchlayers-nightly-1682554018.tar", last modified: Thu Apr 27 00:07:08 2023, max compression
+gzip compressed data, was "dist/torchlayers-nightly-1682640451.tar", last modified: Fri Apr 28 00:07:36 2023, max compression
```

## Comparing `torchlayers-nightly-1682554018.tar` & `torchlayers-nightly-1682640451.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:07:08.000000 torchlayers-nightly-1682554018/
--rw-r--r--   0 runner    (1001) docker     (123)    17559 2023-04-27 00:07:08.000000 torchlayers-nightly-1682554018/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 00:07:08.000000 torchlayers-nightly-1682554018/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:07:08.000000 torchlayers-nightly-1682554018/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/tests/activations_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/tests/attributes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/tests/convolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/tests/general_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/tests/jit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/tests/linear_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/tests/normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/tests/padding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/tests/pickle_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/tests/preprocessing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/tests/recurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/tests/regularization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/tests/torchlayers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:07:08.000000 torchlayers-nightly-1682554018/torchlayers/
--rw-r--r--   0 runner    (1001) docker     (123)    24781 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/torchlayers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:07:08.000000 torchlayers-nightly-1682554018/torchlayers/_dev_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/torchlayers/_dev_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/torchlayers/_dev_utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/torchlayers/_dev_utils/infer.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/torchlayers/_name.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/torchlayers/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/torchlayers/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    36698 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/torchlayers/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/torchlayers/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/torchlayers/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/torchlayers/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/torchlayers/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/torchlayers/regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-27 00:06:58.000000 torchlayers-nightly-1682554018/torchlayers/upsample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:07:08.000000 torchlayers-nightly-1682554018/torchlayers_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17559 2023-04-27 00:07:07.000000 torchlayers-nightly-1682554018/torchlayers_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-27 00:07:08.000000 torchlayers-nightly-1682554018/torchlayers_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 00:07:07.000000 torchlayers-nightly-1682554018/torchlayers_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 00:07:07.000000 torchlayers-nightly-1682554018/torchlayers_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 00:07:07.000000 torchlayers-nightly-1682554018/torchlayers_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:07:36.000000 torchlayers-nightly-1682640451/
+-rw-r--r--   0 runner    (1001) docker     (123)    17559 2023-04-28 00:07:36.000000 torchlayers-nightly-1682640451/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 00:07:36.000000 torchlayers-nightly-1682640451/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:07:36.000000 torchlayers-nightly-1682640451/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/tests/activations_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/tests/attributes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/tests/convolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/tests/general_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/tests/jit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/tests/linear_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/tests/normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/tests/padding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/tests/pickle_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/tests/preprocessing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/tests/recurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/tests/regularization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/tests/torchlayers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:07:36.000000 torchlayers-nightly-1682640451/torchlayers/
+-rw-r--r--   0 runner    (1001) docker     (123)    24781 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/torchlayers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:07:36.000000 torchlayers-nightly-1682640451/torchlayers/_dev_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/torchlayers/_dev_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/torchlayers/_dev_utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/torchlayers/_dev_utils/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/torchlayers/_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/torchlayers/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/torchlayers/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36698 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/torchlayers/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/torchlayers/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/torchlayers/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/torchlayers/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/torchlayers/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/torchlayers/regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-28 00:07:31.000000 torchlayers-nightly-1682640451/torchlayers/upsample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:07:36.000000 torchlayers-nightly-1682640451/torchlayers_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17559 2023-04-28 00:07:36.000000 torchlayers-nightly-1682640451/torchlayers_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-28 00:07:36.000000 torchlayers-nightly-1682640451/torchlayers_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:07:36.000000 torchlayers-nightly-1682640451/torchlayers_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 00:07:36.000000 torchlayers-nightly-1682640451/torchlayers_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 00:07:36.000000 torchlayers-nightly-1682640451/torchlayers_nightly.egg-info/top_level.txt
```

### Comparing `torchlayers-nightly-1682554018/PKG-INFO` & `torchlayers-nightly-1682640451/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlayers-nightly
-Version: 1682554018
+Version: 1682640451
 Summary: Input shape inference and SOTA custom layers for PyTorch.
 Home-page: https://github.com/pypa/torchlayers
 Author: Szymon Maszke
 Author-email: szymon.maszke@protonmail.com
 License: MIT
 Project-URL: Website, https://szymonmaszke.github.io/torchlayers
 Project-URL: Documentation, https://szymonmaszke.github.io/torchlayers/#torchlayers
```

### Comparing `torchlayers-nightly-1682554018/README.md` & `torchlayers-nightly-1682640451/README.md`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/setup.py` & `torchlayers-nightly-1682640451/setup.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/tests/convolution_test.py` & `torchlayers-nightly-1682640451/tests/convolution_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/tests/general_test.py` & `torchlayers-nightly-1682640451/tests/general_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/tests/jit_test.py` & `torchlayers-nightly-1682640451/tests/jit_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/tests/pickle_test.py` & `torchlayers-nightly-1682640451/tests/pickle_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/tests/preprocessing_test.py` & `torchlayers-nightly-1682640451/tests/preprocessing_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/tests/regularization_test.py` & `torchlayers-nightly-1682640451/tests/regularization_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/tests/torchlayers_test.py` & `torchlayers-nightly-1682640451/tests/torchlayers_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/torchlayers/__init__.py` & `torchlayers-nightly-1682640451/torchlayers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/torchlayers/_dev_utils/helpers.py` & `torchlayers-nightly-1682640451/torchlayers/_dev_utils/helpers.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/torchlayers/_dev_utils/infer.py` & `torchlayers-nightly-1682640451/torchlayers/_dev_utils/infer.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/torchlayers/activations.py` & `torchlayers-nightly-1682640451/torchlayers/activations.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/torchlayers/convolution.py` & `torchlayers-nightly-1682640451/torchlayers/convolution.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/torchlayers/module.py` & `torchlayers-nightly-1682640451/torchlayers/module.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/torchlayers/normalization.py` & `torchlayers-nightly-1682640451/torchlayers/normalization.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/torchlayers/pooling.py` & `torchlayers-nightly-1682640451/torchlayers/pooling.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/torchlayers/preprocessing.py` & `torchlayers-nightly-1682640451/torchlayers/preprocessing.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/torchlayers/regularization.py` & `torchlayers-nightly-1682640451/torchlayers/regularization.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/torchlayers/upsample.py` & `torchlayers-nightly-1682640451/torchlayers/upsample.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1682554018/torchlayers_nightly.egg-info/PKG-INFO` & `torchlayers-nightly-1682640451/torchlayers_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlayers-nightly
-Version: 1682554018
+Version: 1682640451
 Summary: Input shape inference and SOTA custom layers for PyTorch.
 Home-page: https://github.com/pypa/torchlayers
 Author: Szymon Maszke
 Author-email: szymon.maszke@protonmail.com
 License: MIT
 Project-URL: Website, https://szymonmaszke.github.io/torchlayers
 Project-URL: Documentation, https://szymonmaszke.github.io/torchlayers/#torchlayers
```

### Comparing `torchlayers-nightly-1682554018/torchlayers_nightly.egg-info/SOURCES.txt` & `torchlayers-nightly-1682640451/torchlayers_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/transformers_gradients-0.0.8.tar.gz` & `tmp/transformers_gradients-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers_gradients-0.0.8.tar", last modified: Sat Apr 15 18:42:17 2023, max compression
+gzip compressed data, was "transformers_gradients-0.0.9.tar", last modified: Sun Apr 16 17:03:07 2023, max compression
```

## Comparing `transformers_gradients-0.0.8.tar` & `transformers_gradients-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     8893 2023-04-15 18:42:07.809083 transformers_gradients-0.0.8/Readme.md
--rw-r--r--   0        0        0     4439 2023-04-15 18:42:07.809083 transformers_gradients-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      597 2023-04-15 18:42:07.809083 transformers_gradients-0.0.8/src/transformers_gradients/__init__.py
--rw-r--r--   0        0        0     3135 2023-04-15 18:42:07.809083 transformers_gradients-0.0.8/src/transformers_gradients/functions.py
--rw-r--r--   0        0        0      792 2023-04-15 18:42:07.809083 transformers_gradients-0.0.8/src/transformers_gradients/logging_utils.py
--rw-r--r--   0        0        0     2640 2023-04-15 18:42:07.809083 transformers_gradients-0.0.8/src/transformers_gradients/model_utils.py
--rw-r--r--   0        0        0     7351 2023-04-15 18:42:07.809083 transformers_gradients-0.0.8/src/transformers_gradients/plotting.py
--rw-r--r--   0        0        0       64 2023-04-15 18:42:07.809083 transformers_gradients-0.0.8/src/transformers_gradients/py.typed
--rw-r--r--   0        0        0        0 2023-04-15 18:42:07.809083 transformers_gradients-0.0.8/src/transformers_gradients/text_classification/__init__.py
--rw-r--r--   0        0        0    16496 2023-04-15 18:42:07.809083 transformers_gradients-0.0.8/src/transformers_gradients/text_classification/huggingface.py
--rw-r--r--   0        0        0     8777 2023-04-15 18:42:07.809083 transformers_gradients-0.0.8/src/transformers_gradients/text_classification/tensor_rt.py
--rw-r--r--   0        0        0     5775 2023-04-15 18:42:07.809083 transformers_gradients-0.0.8/src/transformers_gradients/types.py
--rw-r--r--   0        0        0     1677 2023-04-15 18:42:07.809083 transformers_gradients-0.0.8/src/transformers_gradients/util.py
--rw-r--r--   0        0        0    10161 1970-01-01 00:00:00.000000 transformers_gradients-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     8893 2023-04-16 17:02:59.752821 transformers_gradients-0.0.9/Readme.md
+-rw-r--r--   0        0        0     4439 2023-04-16 17:02:59.756821 transformers_gradients-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      597 2023-04-16 17:02:59.756821 transformers_gradients-0.0.9/src/transformers_gradients/__init__.py
+-rw-r--r--   0        0        0     3135 2023-04-16 17:02:59.756821 transformers_gradients-0.0.9/src/transformers_gradients/functions.py
+-rw-r--r--   0        0        0      792 2023-04-16 17:02:59.756821 transformers_gradients-0.0.9/src/transformers_gradients/logging_utils.py
+-rw-r--r--   0        0        0     2640 2023-04-16 17:02:59.756821 transformers_gradients-0.0.9/src/transformers_gradients/model_utils.py
+-rw-r--r--   0        0        0     7351 2023-04-16 17:02:59.756821 transformers_gradients-0.0.9/src/transformers_gradients/plotting.py
+-rw-r--r--   0        0        0       64 2023-04-16 17:02:59.756821 transformers_gradients-0.0.9/src/transformers_gradients/py.typed
+-rw-r--r--   0        0        0        0 2023-04-16 17:02:59.756821 transformers_gradients-0.0.9/src/transformers_gradients/text_classification/__init__.py
+-rw-r--r--   0        0        0    16496 2023-04-16 17:02:59.756821 transformers_gradients-0.0.9/src/transformers_gradients/text_classification/huggingface.py
+-rw-r--r--   0        0        0     8777 2023-04-16 17:02:59.756821 transformers_gradients-0.0.9/src/transformers_gradients/text_classification/tensor_rt.py
+-rw-r--r--   0        0        0     5775 2023-04-16 17:02:59.756821 transformers_gradients-0.0.9/src/transformers_gradients/types.py
+-rw-r--r--   0        0        0     1738 2023-04-16 17:02:59.756821 transformers_gradients-0.0.9/src/transformers_gradients/util.py
+-rw-r--r--   0        0        0    10161 1970-01-01 00:00:00.000000 transformers_gradients-0.0.9/PKG-INFO
```

### Comparing `transformers_gradients-0.0.8/Readme.md` & `transformers_gradients-0.0.9/Readme.md`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.8/pyproject.toml` & `transformers_gradients-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "transformers_gradients"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.8"  # Required
+version = "0.0.9"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Gradient-based XAI methods for TensorFlow transformers."  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `transformers_gradients-0.0.8/src/transformers_gradients/__init__.py` & `transformers_gradients-0.0.9/src/transformers_gradients/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.8/src/transformers_gradients/functions.py` & `transformers_gradients-0.0.9/src/transformers_gradients/functions.py`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.8/src/transformers_gradients/logging_utils.py` & `transformers_gradients-0.0.9/src/transformers_gradients/logging_utils.py`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.8/src/transformers_gradients/model_utils.py` & `transformers_gradients-0.0.9/src/transformers_gradients/model_utils.py`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.8/src/transformers_gradients/plotting.py` & `transformers_gradients-0.0.9/src/transformers_gradients/plotting.py`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.8/src/transformers_gradients/text_classification/huggingface.py` & `transformers_gradients-0.0.9/src/transformers_gradients/text_classification/huggingface.py`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.8/src/transformers_gradients/text_classification/tensor_rt.py` & `transformers_gradients-0.0.9/src/transformers_gradients/text_classification/tensor_rt.py`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.8/src/transformers_gradients/types.py` & `transformers_gradients-0.0.9/src/transformers_gradients/types.py`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.8/src/transformers_gradients/util.py` & `transformers_gradients-0.0.9/src/transformers_gradients/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import platform
 from functools import wraps
 from typing import TypeVar, Callable, Dict, List, Tuple
 
 import tensorflow as tf
 from transformers import PreTrainedTokenizerBase
 
+from transformers_gradients.functions import bounding_shape
+
 T = TypeVar("T")
 
 
 def encode_inputs(
     tokenizer: PreTrainedTokenizerBase, x_batch: List[str]
 ) -> Tuple[tf.Tensor, tf.Tensor | None]:
     """Do batch encode, unpack input ids and other forward-pass kwargs."""
```

### Comparing `transformers_gradients-0.0.8/PKG-INFO` & `transformers_gradients-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers_gradients
-Version: 0.0.8
+Version: 0.0.9
 Summary: Gradient-based XAI methods for TensorFlow transformers.
 Keywords: explainable ai,xai,machine learning,deep learning
 Author-email: Artem Sereda <artem.sereda@campus.tu-berlin.de>
 Maintainer-email: Artem Sereda <artem.sereda@campus.tu-berlin.de>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transformers_gradients Version: 0.0.8 Summary:
+Metadata-Version: 2.1 Name: transformers_gradients Version: 0.0.9 Summary:
 Gradient-based XAI methods for TensorFlow transformers. Keywords: explainable
 ai,xai,machine learning,deep learning Author-email: Artem Sereda
 sereda@campus.tu-berlin.de> Maintainer-email: Artem Sereda
 sereda@campus.tu-berlin.de> Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
```


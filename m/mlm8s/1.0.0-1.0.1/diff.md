# Comparing `tmp/mlm8s-1.0.0.tar.gz` & `tmp/mlm8s-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlm8s-1.0.0.tar", max compression
+gzip compressed data, was "mlm8s-1.0.1.tar", max compression
```

## Comparing `mlm8s-1.0.0.tar` & `mlm8s-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,24 @@
--rw-r--r--   0        0        0    35149 2023-03-22 02:25:13.814125 mlm8s-1.0.0/LICENSE
--rw-r--r--   0        0        0     2061 2023-03-22 02:25:13.814125 mlm8s-1.0.0/README.md
--rw-r--r--   0        0        0      312 2023-03-22 02:25:13.814125 mlm8s-1.0.0/mlm8s/__init__.py
--rw-r--r--   0        0        0     1436 2023-03-22 02:25:13.814125 mlm8s-1.0.0/mlm8s/chaos.py
--rw-r--r--   0        0        0      609 2023-03-22 02:25:13.814125 mlm8s-1.0.0/mlm8s/connect.py
--rw-r--r--   0        0        0     2235 2023-03-22 02:25:13.814125 mlm8s-1.0.0/mlm8s/custom_metrices.py
--rw-r--r--   0        0        0     1626 2023-03-22 02:25:13.814125 mlm8s-1.0.0/mlm8s/generator.py
--rw-r--r--   0        0        0     1751 2023-03-22 02:25:13.814125 mlm8s-1.0.0/mlm8s/helpers.py
--rw-r--r--   0        0        0     2683 2023-03-22 02:25:13.814125 mlm8s-1.0.0/mlm8s/hypermodel.py
--rw-r--r--   0        0        0     4208 2023-03-22 02:25:13.814125 mlm8s-1.0.0/mlm8s/lattice.py
--rw-r--r--   0        0        0      808 2023-03-22 02:25:13.814125 mlm8s-1.0.0/mlm8s/numeric.py
--rw-r--r--   0        0        0     1001 2023-03-22 02:25:13.814125 mlm8s-1.0.0/mlm8s/overview - metrics
--rw-r--r--   0        0        0     2124 2023-03-22 02:25:13.814125 mlm8s-1.0.0/mlm8s/paths.py
--rw-r--r--   0        0        0      907 2023-03-22 02:25:13.814125 mlm8s-1.0.0/mlm8s/plot.py
--rw-r--r--   0        0        0     1004 2023-03-22 02:25:13.814125 mlm8s-1.0.0/mlm8s/rounding_loss.py
--rw-r--r--   0        0        0     6658 2023-03-22 02:25:13.814125 mlm8s-1.0.0/mlm8s/spiral.py
--rw-r--r--   0        0        0     5352 2023-03-22 02:25:13.814125 mlm8s-1.0.0/mlm8s/voltera.py
--rw-r--r--   0        0        0      993 2023-03-22 02:25:13.814125 mlm8s-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2427 1970-01-01 00:00:00.000000 mlm8s-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-29 12:39:38.358629 mlm8s-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2301 2023-04-29 12:39:38.358629 mlm8s-1.0.1/README.md
+-rw-r--r--   0        0        0      425 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/__init__.py
+-rw-r--r--   0        0        0     1436 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/chaos.py
+-rw-r--r--   0        0        0      609 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/connect.py
+-rw-r--r--   0        0        0     2235 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/custom_metrices.py
+-rw-r--r--   0        0        0     1626 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/generator.py
+-rw-r--r--   0        0        0     1751 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/helpers.py
+-rw-r--r--   0        0        0     2683 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/hypermodel.py
+-rw-r--r--   0        0        0     4208 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/lattice.py
+-rw-r--r--   0        0        0      808 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/numeric.py
+-rw-r--r--   0        0        0     1001 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/overview - metrics
+-rw-r--r--   0        0        0     2124 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/paths.py
+-rw-r--r--   0        0        0      907 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/plot.py
+-rw-r--r--   0        0        0     5936 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/polynom.py
+-rw-r--r--   0        0        0     1004 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/rounding_loss.py
+-rw-r--r--   0        0        0     3539 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/sparse.py
+-rw-r--r--   0        0        0     6658 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/spiral.py
+-rw-r--r--   0        0        0     5444 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/text.py
+-rw-r--r--   0        0        0      872 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/training.py
+-rw-r--r--   0        0        0      757 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/triangle.py
+-rw-r--r--   0        0        0     5352 2023-04-29 12:39:38.358629 mlm8s-1.0.1/mlm8s/voltera.py
+-rw-r--r--   0        0        0     1172 2023-04-29 12:39:38.358629 mlm8s-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2946 1970-01-01 00:00:00.000000 mlm8s-1.0.1/PKG-INFO
```

### Comparing `mlm8s-1.0.0/LICENSE` & `mlm8s-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.0/README.md` & `mlm8s-1.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 # mlm8s
 
 ###### miscellaneous for machine-learning in TensorFlow
+
+```
+pip install keras_tuner
+pip install mlm8s
+```
+
 #### Imports:
 ```
 from mlm8s import ListedPaths, paths2labels, strings2onehot, paths2label_dicts, map_via_dict
 from mlm8s import GeneratorDataset, HyperModel, connect
 from mlm8s import standardize, normalize, stretch, rotate_deg, flatten, correlate
 from mlm8s import create_meshgrid, span_polar_basis
 from mlm8s import group_unique
 from mlm8s import print_plot_play
+from mlm8s import get_sampling_matrix, soft_threshold, deadzone_l1_loss, lasso_l1, norm_l0, huber_loss
+from mlm8s import lipschitz_grad_lasso, nesterov_momentum, ista_prox_lasso, fista
 ```
 <br>
 
 #### Labels from Paths:
 
 ```
 from mlm8s import ListedPaths, paths2label_dicts, map_via_dict
@@ -23,15 +31,15 @@
 label_dict = paths2label_dicts(paths(), seperators=['/', '.'], indices=[-2, 0])
 labels = map_via_dict(paths2labels(paths()), label_dict)
 ```
 <br>
 
 #### Class - GeneratorDataset:
 
-Enables changing results of tf.random* -calls, from within
+Enables alternating results of tf.random* -calls, from within
 the generator of tf.data.Dataset.from_generator*.
 
 ```
 kwargs = dict()
 kwargs['paths'] = paths
 kwargs['seperators'] = ['/', '.']
 kwargs['indices'] = [-2, 0]
```

### Comparing `mlm8s-1.0.0/mlm8s/chaos.py` & `mlm8s-1.0.1/mlm8s/chaos.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.0/mlm8s/connect.py` & `mlm8s-1.0.1/mlm8s/connect.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.0/mlm8s/custom_metrices.py` & `mlm8s-1.0.1/mlm8s/custom_metrices.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.0/mlm8s/generator.py` & `mlm8s-1.0.1/mlm8s/generator.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.0/mlm8s/helpers.py` & `mlm8s-1.0.1/mlm8s/helpers.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.0/mlm8s/hypermodel.py` & `mlm8s-1.0.1/mlm8s/hypermodel.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.0/mlm8s/lattice.py` & `mlm8s-1.0.1/mlm8s/lattice.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.0/mlm8s/numeric.py` & `mlm8s-1.0.1/mlm8s/numeric.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.0/mlm8s/overview - metrics` & `mlm8s-1.0.1/mlm8s/overview - metrics`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.0/mlm8s/paths.py` & `mlm8s-1.0.1/mlm8s/paths.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.0/mlm8s/plot.py` & `mlm8s-1.0.1/mlm8s/plot.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.0/mlm8s/rounding_loss.py` & `mlm8s-1.0.1/mlm8s/rounding_loss.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.0/mlm8s/spiral.py` & `mlm8s-1.0.1/mlm8s/spiral.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.0/mlm8s/voltera.py` & `mlm8s-1.0.1/mlm8s/voltera.py`

 * *Files identical despite different names*

### Comparing `mlm8s-1.0.0/pyproject.toml` & `mlm8s-1.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 [tool.poetry]
 name = "mlm8s"
-version = "1.0.0"
+#version = "0.0.2.8"
+version = "1.0.1"
 description = "utils & misc 4 mlm8s"
+license = "GPL-3.0-only"
 authors = ["2mrwolke"]
 readme = "README.md"
 packages = [{include = "mlm8s"}]
+homepage = "https://mlm8s.org/"
 
 [tool.poetry.dependencies]
 # These packages are mandatory and form the core of this package’s distribution.
-python = "^3.9"
+python = "^3.6"
+#keras_tuner = "^1.0"
+#oldest-supported-numpy = "^2022.11.18"
 
 [build-system]
 requires = ["poetry-core"]
+#requires = ["oldest-supported-numpy"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = "pyproject.toml:version" # version location
 branch = "main"                             # branch to make releases of
 changelog_file = "CHANGELOG.md"             # changelog file
 build_command = "poetry build"              # build dists
 dist_path = "dist/"                         # where to put dists
 upload_to_release = true                    # auto-create GitHub release
-upload_to_pypi = true                       # auto-upload to PyPI
+upload_to_pypi = false                      # auto-upload to PyPI
 remove_dist = false                         # don't remove dists
 patch_without_tag = false                   # patch release by default
```

### Comparing `mlm8s-1.0.0/PKG-INFO` & `mlm8s-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 Metadata-Version: 2.1
 Name: mlm8s
-Version: 1.0.0
+Version: 1.0.1
 Summary: utils & misc 4 mlm8s
+Home-page: https://mlm8s.org/
+License: GPL-3.0-only
 Author: 2mrwolke
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.6,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # mlm8s
 
 ###### miscellaneous for machine-learning in TensorFlow
+
+```
+pip install keras_tuner
+pip install mlm8s
+```
+
 #### Imports:
 ```
 from mlm8s import ListedPaths, paths2labels, strings2onehot, paths2label_dicts, map_via_dict
 from mlm8s import GeneratorDataset, HyperModel, connect
 from mlm8s import standardize, normalize, stretch, rotate_deg, flatten, correlate
 from mlm8s import create_meshgrid, span_polar_basis
 from mlm8s import group_unique
 from mlm8s import print_plot_play
+from mlm8s import get_sampling_matrix, soft_threshold, deadzone_l1_loss, lasso_l1, norm_l0, huber_loss
+from mlm8s import lipschitz_grad_lasso, nesterov_momentum, ista_prox_lasso, fista
 ```
 <br>
 
 #### Labels from Paths:
 
 ```
 from mlm8s import ListedPaths, paths2label_dicts, map_via_dict
@@ -35,15 +49,15 @@
 label_dict = paths2label_dicts(paths(), seperators=['/', '.'], indices=[-2, 0])
 labels = map_via_dict(paths2labels(paths()), label_dict)
 ```
 <br>
 
 #### Class - GeneratorDataset:
 
-Enables changing results of tf.random* -calls, from within
+Enables alternating results of tf.random* -calls, from within
 the generator of tf.data.Dataset.from_generator*.
 
 ```
 kwargs = dict()
 kwargs['paths'] = paths
 kwargs['seperators'] = ['/', '.']
 kwargs['indices'] = [-2, 0]
```


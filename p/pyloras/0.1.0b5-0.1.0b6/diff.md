# Comparing `tmp/pyloras-0.1.0b5.tar.gz` & `tmp/pyloras-0.1.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloras-0.1.0b5.tar", max compression
+gzip compressed data, was "pyloras-0.1.0b6.tar", last modified: Sat Apr 29 21:48:24 2023, max compression
```

## Comparing `pyloras-0.1.0b5.tar` & `pyloras-0.1.0b6.tar`

### file list

```diff
@@ -1,10 +1,23 @@
--rw-r--r--   0        0        0     1514 2021-09-23 11:41:13.332860 pyloras-0.1.0b5/LICENSE
--rw-r--r--   0        0        0     3419 2021-09-23 11:41:13.332860 pyloras-0.1.0b5/README.md
--rw-r--r--   0        0        0      112 2021-09-23 11:41:13.332860 pyloras-0.1.0b5/pyloras/__init__.py
--rw-r--r--   0        0        0      649 2021-09-23 11:41:13.332860 pyloras-0.1.0b5/pyloras/_common.py
--rw-r--r--   0        0        0     8122 2021-09-23 11:41:13.332860 pyloras-0.1.0b5/pyloras/_gamus.py
--rw-r--r--   0        0        0     8837 2021-09-23 11:41:13.332860 pyloras-0.1.0b5/pyloras/_loras.py
--rw-r--r--   0        0        0    10239 2021-09-23 11:41:13.332860 pyloras-0.1.0b5/pyloras/_prowras.py
--rw-r--r--   0        0        0     1127 2021-09-23 11:41:13.332860 pyloras-0.1.0b5/pyproject.toml
--rw-r--r--   0        0        0     4219 2021-09-23 11:41:54.187978 pyloras-0.1.0b5/setup.py
--rw-r--r--   0        0        0     4641 2021-09-23 11:41:54.188534 pyloras-0.1.0b5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 21:48:24.263450 pyloras-0.1.0b6/
+-rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-04-29 21:47:57.000000 pyloras-0.1.0b6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-04-29 21:47:57.000000 pyloras-0.1.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-29 21:47:57.000000 pyloras-0.1.0b6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      353 2023-04-29 21:47:57.000000 pyloras-0.1.0b6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     4449 2023-04-29 21:48:24.263450 pyloras-0.1.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3465 2023-04-29 21:47:57.000000 pyloras-0.1.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 21:48:24.263450 pyloras-0.1.0b6/pyloras/
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-04-29 21:47:57.000000 pyloras-0.1.0b6/pyloras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      648 2023-04-29 21:47:57.000000 pyloras-0.1.0b6/pyloras/_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8122 2023-04-29 21:47:57.000000 pyloras-0.1.0b6/pyloras/_gamus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8851 2023-04-29 21:47:57.000000 pyloras-0.1.0b6/pyloras/_loras.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10239 2023-04-29 21:47:57.000000 pyloras-0.1.0b6/pyloras/_prowras.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-04-29 21:48:24.000000 pyloras-0.1.0b6/pyloras/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 21:48:24.263450 pyloras-0.1.0b6/pyloras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4449 2023-04-29 21:48:24.000000 pyloras-0.1.0b6/pyloras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-04-29 21:48:24.000000 pyloras-0.1.0b6/pyloras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-29 21:48:24.000000 pyloras-0.1.0b6/pyloras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-04-29 21:48:24.000000 pyloras-0.1.0b6/pyloras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-29 21:48:24.000000 pyloras-0.1.0b6/pyloras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1286 2023-04-29 21:47:57.000000 pyloras-0.1.0b6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-04-29 21:47:57.000000 pyloras-0.1.0b6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-29 21:48:24.263450 pyloras-0.1.0b6/setup.cfg
```

### Comparing `pyloras-0.1.0b5/LICENSE` & `pyloras-0.1.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloras-0.1.0b5/README.md` & `pyloras-0.1.0b6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,39 +3,38 @@
 [![CI][3]](https://github.com/zoj613/pyloras/actions/workflows/build-and-test.yml)
 [![Codecov][4]](https://codecov.io/gh/zoj613/pyloras/)
 [![PyPI][5]](https://pypi.org/project/pyloras/#history)
 
 Localized Random Affine Shadowsampling
 
 This repo provides a python implementation of an imbalanced dataset oversampling
-technique known as Localized Random Affine Shadowsampling (LoRAS). This implementation 
-piggybacks off the package ``imbalanced-learn`` and thus aims to be as compatible
-as possible with it.
+technique known as Localized Random Affine Shadowsampling (LoRAS). It also provides
+implementations of several other over/under-sampling algorithms not yet available in
+the ``imbalanced-learn`` package. These implementations piggybacks off of ``imbalanced-learn``
+and thus aim to be as compatible as possible with it.
 
 
 ## Dependencies
-- `Python >= 3.6`
-- `numpy >= 1.17.0`
-- `imbalanced-learn`
+- `Python >= 3.8`
+- `numpy >= 1.17.3`
+- `imbalanced-learn < 1.0.0`
 
 
 ## Installation
 
 Using `pip`:
 ```shell
 $ pip install -U pyloras
 ```
 
-Installing from source requires an installation of [poetry][1] and the following shell commands:
+Alternatively, one can install from source with the following shell commands:
 ```shell
 $ git clone https://github.com/zoj613/pyloras.git
 $ cd pyloras/
-$ poetry install
-# add package to python's path
-$ export PYTHONPATH=$PWD:$PYTHONPATH 
+$ pip install .
 ```
 
 ## Usage
 
 ```python
 from collections import Counter
 from pyloras import LORAS
```

### Comparing `pyloras-0.1.0b5/pyloras/_common.py` & `pyloras-0.1.0b6/pyloras/_common.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     """
     To be used with sklearn Estimators that expect a random_state argument.
 
     This safely passes the required ``np.random.RandomState`` instance to the
     estimator when the user has a ``np.random.Generator`` instead.
     """
     if isinstance(random_state, np.random.Generator):
-        return np.random.RandomState(random_state._bit_generator)
+        return np.random.RandomState(random_state.bit_generator)
     return random_state
```

### Comparing `pyloras-0.1.0b5/pyloras/_gamus.py` & `pyloras-0.1.0b6/pyloras/_gamus.py`

 * *Files identical despite different names*

### Comparing `pyloras-0.1.0b5/pyloras/_loras.py` & `pyloras-0.1.0b6/pyloras/_loras.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         """Initialize the parameter values to their appropriate values."""
         f_size = X.shape[1]
         self.n_affine_ = f_size if self.n_affine is None else self.n_affine
 
         if self.manifold_learner:
             self.manifold_learner_ = self._check_2d_manifold_learner()
         else:
-            self.manifold_learner_ = TSNE(n_components=2)
+            self.manifold_learner_ = TSNE(n_components=2, perplexity=5)
         if self.manifold_learner_params is not None:
             self.manifold_learner_.set_params(**self.manifold_learner_params)
         try:
             self.manifold_learner_.set_params(random_state=safe_random_state(rng))
         except ValueError:
             pass
```

### Comparing `pyloras-0.1.0b5/pyloras/_prowras.py` & `pyloras-0.1.0b6/pyloras/_prowras.py`

 * *Files identical despite different names*

### Comparing `pyloras-0.1.0b5/pyproject.toml` & `pyloras-0.1.0b6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-[tool.poetry]
+[project]
 name = "pyloras"
-version = "0.1.0-beta.5"
-description = "LoRAS: An oversampling approach for imbalanced datasets"
-authors = ["Zolisa Bleki <zolisa.bleki@gmail.com>"]
-license = "BSD-3-Clause"
-readme = 'README.md'
-repository = "https://github.com/zoj613/pyloras/"
+authors = [
+    {name = "Zolisa Bleki", email = "zolisa.bleki@gmail.com"}
+]
+description = "Experimental implementations of several (over/under)-sampling techniques not yet available in the imbalanced-learn library."
+readme = "README.md"
+dynamic = ["version"]
+requires-python = ">=3.8"
+dependencies = ["numpy >= 1.17.3", "imbalanced-learn < 1.0.0"]
+license = {text = "BSD 3-Clause License"}
 keywords = [
     'loras',
     'imbalanced datasets',
     'oversampling',
     'machine learning',
     'localized affine random shadowsampling'
 ]
@@ -19,25 +22,21 @@
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "Operating System :: MacOS :: MacOS X",
 ]
-include = [
-    "LICENSE",
-]
-
-[tool.poetry.dependencies]
-python = "^3.6"
-numpy = "^1.17.0"
-imbalanced-learn = "^0.7.0"
 
-[tool.poetry.dev-dependencies]
-imbalanced-learn = "^0.7.0"
-numpy = "1.17.3"
-pytest-cov = "*"
-toml = "^0.10.2"
+[project.urls]
+source = "https://github.com/zoj613/pyloras"
+tracker = "https://github.com/zoj613/pyloras/issues"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["wheel", "setuptools>=61.0.0", "setuptools-scm[toml]>=6.2"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools]
+packages = ["pyloras"]
+
+[tool.setuptools_scm]
+write_to = "pyloras/_version.py"
```

### Comparing `pyloras-0.1.0b5/setup.py` & `pyloras-0.1.0b6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,107 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['pyloras']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['imbalanced-learn>=0.7.0,<0.8.0', 'numpy>=1.17.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'pyloras',
-    'version': '0.1.0b5',
-    'description': 'LoRAS: An oversampling approach for imbalanced datasets',
-    'long_description': '# LoRAS\n\n[![CI][3]](https://github.com/zoj613/pyloras/actions/workflows/build-and-test.yml)\n[![Codecov][4]](https://codecov.io/gh/zoj613/pyloras/)\n[![PyPI][5]](https://pypi.org/project/pyloras/#history)\n\nLocalized Random Affine Shadowsampling\n\nThis repo provides a python implementation of an imbalanced dataset oversampling\ntechnique known as Localized Random Affine Shadowsampling (LoRAS). This implementation \npiggybacks off the package ``imbalanced-learn`` and thus aims to be as compatible\nas possible with it.\n\n\n## Dependencies\n- `Python >= 3.6`\n- `numpy >= 1.17.0`\n- `imbalanced-learn`\n\n\n## Installation\n\nUsing `pip`:\n```shell\n$ pip install -U pyloras\n```\n\nInstalling from source requires an installation of [poetry][1] and the following shell commands:\n```shell\n$ git clone https://github.com/zoj613/pyloras.git\n$ cd pyloras/\n$ poetry install\n# add package to python\'s path\n$ export PYTHONPATH=$PWD:$PYTHONPATH \n```\n\n## Usage\n\n```python\nfrom collections import Counter\nfrom pyloras import LORAS\nfrom sklearn.datasets import make_classification\n\nX, y = make_classification(n_samples=20000, n_features=5, n_informative=5,\n                           n_redundant=0, n_repeated=0, n_classes=3,\n                           n_clusters_per_class=1,\n                           weights=[0.01, 0.05, 0.94],\n                           class_sep=0.8, random_state=0)\n\nlrs = LORAS(random_state=0, manifold_learner_params={\'perplexity\': 35, \'n_iter\': 250})\nprint(sorted(Counter(y).items()))\n# [(0, 270), (1, 1056), (2, 18674)]\nX_resampled, y_resampled = lrs.fit_resample(X, y)\nprint(sorted(Counter(y_resampled.astype(int)).items()))\n# [(0, 18674), (1, 18674), (2, 18674)]\n\n# one can also use any custom 2d manifold learner via the ``manifold_learner` parameter\nfrom umap import UMAP\nLORAS(manifold_learner=UMAP()).fit_resample(X, y)\n\n```\n\n## Visualization\n\nBelow is a comparision of `imbalanced-learn`\'s `SMOTE` implementation with `LORAS`\non the dummy data used in [this doc page][2] using the default parameters.\n\n![](./scripts/img/resampled_data.svg)\n![](./scripts/img/decision_fn.svg)\n![](./scripts/img/particularities.svg)\n\nThe plots can be reproduced by running:\n```\n$ python scripts/compare_oversamplers.py --n_neighbors=<optional> --n_shadow=<optional> --n_affine=<optional>\n```\n\n## References\n- Bej, S., Davtyan, N., Wolfien, M. et al. LoRAS: an oversampling approach for imbalanced datasets. Mach Learn 110, 279–301 (2021). https://doi.org/10.1007/s10994-020-05913-4\n- Bej, S., Schultz, K., Srivastava, P., Wolfien, M., & Wolkenhauer, O. (2021). A multi-schematic classifier-independent oversampling approach for imbalanced datasets. ArXiv, abs/2107.07349.\n- A. Tripathi, R. Chakraborty and S. K. Kopparapu, "A Novel Adaptive Minority Oversampling Technique for Improved Classification in Data Imbalanced Scenarios," 2020 25th International Conference on Pattern Recognition (ICPR), 2021, pp. 10650-10657, doi: 10.1109/ICPR48806.2021.9413002.\n\n\n[1]: https://python-poetry.org/docs/pyproject/\n[2]: https://imbalanced-learn.org/stable/auto_examples/over-sampling/plot_comparison_over_sampling.html#more-advanced-over-sampling-using-adasyn-and-smote\n[3]: https://img.shields.io/github/workflow/status/zoj613/pyloras/CI/main?style=flat-square\n[4]: https://img.shields.io/codecov/c/github/zoj613/pyloras?style=flat-square\n[5]: https://img.shields.io/github/v/release/zoj613/pyloras?include_prereleases&style=flat-square\n',
-    'author': 'Zolisa Bleki',
-    'author_email': 'zolisa.bleki@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/zoj613/pyloras/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: pyloras
+Version: 0.1.0b6
+Summary: Experimental implementations of several (over/under)-sampling techniques not yet available in the imbalanced-learn library.
+Author-email: Zolisa Bleki <zolisa.bleki@gmail.com>
+License: BSD 3-Clause License
+Project-URL: source, https://github.com/zoj613/pyloras
+Project-URL: tracker, https://github.com/zoj613/pyloras/issues
+Keywords: loras,imbalanced datasets,oversampling,machine learning,localized affine random shadowsampling
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: MacOS :: MacOS X
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# LoRAS
+
+[![CI][3]](https://github.com/zoj613/pyloras/actions/workflows/build-and-test.yml)
+[![Codecov][4]](https://codecov.io/gh/zoj613/pyloras/)
+[![PyPI][5]](https://pypi.org/project/pyloras/#history)
+
+Localized Random Affine Shadowsampling
+
+This repo provides a python implementation of an imbalanced dataset oversampling
+technique known as Localized Random Affine Shadowsampling (LoRAS). It also provides
+implementations of several other over/under-sampling algorithms not yet available in
+the ``imbalanced-learn`` package. These implementations piggybacks off of ``imbalanced-learn``
+and thus aim to be as compatible as possible with it.
+
+
+## Dependencies
+- `Python >= 3.8`
+- `numpy >= 1.17.3`
+- `imbalanced-learn < 1.0.0`
+
+
+## Installation
+
+Using `pip`:
+```shell
+$ pip install -U pyloras
+```
+
+Alternatively, one can install from source with the following shell commands:
+```shell
+$ git clone https://github.com/zoj613/pyloras.git
+$ cd pyloras/
+$ pip install .
+```
+
+## Usage
+
+```python
+from collections import Counter
+from pyloras import LORAS
+from sklearn.datasets import make_classification
+
+X, y = make_classification(n_samples=20000, n_features=5, n_informative=5,
+                           n_redundant=0, n_repeated=0, n_classes=3,
+                           n_clusters_per_class=1,
+                           weights=[0.01, 0.05, 0.94],
+                           class_sep=0.8, random_state=0)
+
+lrs = LORAS(random_state=0, manifold_learner_params={'perplexity': 35, 'n_iter': 250})
+print(sorted(Counter(y).items()))
+# [(0, 270), (1, 1056), (2, 18674)]
+X_resampled, y_resampled = lrs.fit_resample(X, y)
+print(sorted(Counter(y_resampled.astype(int)).items()))
+# [(0, 18674), (1, 18674), (2, 18674)]
+
+# one can also use any custom 2d manifold learner via the ``manifold_learner` parameter
+from umap import UMAP
+LORAS(manifold_learner=UMAP()).fit_resample(X, y)
+
+```
+
+## Visualization
+
+Below is a comparision of `imbalanced-learn`'s `SMOTE` implementation with `LORAS`
+on the dummy data used in [this doc page][2] using the default parameters.
+
+![](./scripts/img/resampled_data.svg)
+![](./scripts/img/decision_fn.svg)
+![](./scripts/img/particularities.svg)
+
+The plots can be reproduced by running:
+```
+$ python scripts/compare_oversamplers.py --n_neighbors=<optional> --n_shadow=<optional> --n_affine=<optional>
+```
+
+## References
+- Bej, S., Davtyan, N., Wolfien, M. et al. LoRAS: an oversampling approach for imbalanced datasets. Mach Learn 110, 279–301 (2021). https://doi.org/10.1007/s10994-020-05913-4
+- Bej, S., Schultz, K., Srivastava, P., Wolfien, M., & Wolkenhauer, O. (2021). A multi-schematic classifier-independent oversampling approach for imbalanced datasets. ArXiv, abs/2107.07349.
+- A. Tripathi, R. Chakraborty and S. K. Kopparapu, "A Novel Adaptive Minority Oversampling Technique for Improved Classification in Data Imbalanced Scenarios," 2020 25th International Conference on Pattern Recognition (ICPR), 2021, pp. 10650-10657, doi: 10.1109/ICPR48806.2021.9413002.
+
+
+[1]: https://python-poetry.org/docs/pyproject/
+[2]: https://imbalanced-learn.org/stable/auto_examples/over-sampling/plot_comparison_over_sampling.html#more-advanced-over-sampling-using-adasyn-and-smote
+[3]: https://img.shields.io/github/workflow/status/zoj613/pyloras/CI/main?style=flat-square
+[4]: https://img.shields.io/codecov/c/github/zoj613/pyloras?style=flat-square
+[5]: https://img.shields.io/github/v/release/zoj613/pyloras?include_prereleases&style=flat-square
```

### Comparing `pyloras-0.1.0b5/PKG-INFO` & `pyloras-0.1.0b6/pyloras.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,61 @@
 Metadata-Version: 2.1
 Name: pyloras
-Version: 0.1.0b5
-Summary: LoRAS: An oversampling approach for imbalanced datasets
-Home-page: https://github.com/zoj613/pyloras/
-License: BSD-3-Clause
+Version: 0.1.0b6
+Summary: Experimental implementations of several (over/under)-sampling techniques not yet available in the imbalanced-learn library.
+Author-email: Zolisa Bleki <zolisa.bleki@gmail.com>
+License: BSD 3-Clause License
+Project-URL: source, https://github.com/zoj613/pyloras
+Project-URL: tracker, https://github.com/zoj613/pyloras/issues
 Keywords: loras,imbalanced datasets,oversampling,machine learning,localized affine random shadowsampling
-Author: Zolisa Bleki
-Author-email: zolisa.bleki@gmail.com
-Requires-Python: >=3.6,<4.0
 Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering
-Requires-Dist: imbalanced-learn (>=0.7.0,<0.8.0)
-Requires-Dist: numpy (>=1.17.0,<2.0.0)
-Project-URL: Repository, https://github.com/zoj613/pyloras/
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: MacOS :: MacOS X
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # LoRAS
 
 [![CI][3]](https://github.com/zoj613/pyloras/actions/workflows/build-and-test.yml)
 [![Codecov][4]](https://codecov.io/gh/zoj613/pyloras/)
 [![PyPI][5]](https://pypi.org/project/pyloras/#history)
 
 Localized Random Affine Shadowsampling
 
 This repo provides a python implementation of an imbalanced dataset oversampling
-technique known as Localized Random Affine Shadowsampling (LoRAS). This implementation 
-piggybacks off the package ``imbalanced-learn`` and thus aims to be as compatible
-as possible with it.
+technique known as Localized Random Affine Shadowsampling (LoRAS). It also provides
+implementations of several other over/under-sampling algorithms not yet available in
+the ``imbalanced-learn`` package. These implementations piggybacks off of ``imbalanced-learn``
+and thus aim to be as compatible as possible with it.
 
 
 ## Dependencies
-- `Python >= 3.6`
-- `numpy >= 1.17.0`
-- `imbalanced-learn`
+- `Python >= 3.8`
+- `numpy >= 1.17.3`
+- `imbalanced-learn < 1.0.0`
 
 
 ## Installation
 
 Using `pip`:
 ```shell
 $ pip install -U pyloras
 ```
 
-Installing from source requires an installation of [poetry][1] and the following shell commands:
+Alternatively, one can install from source with the following shell commands:
 ```shell
 $ git clone https://github.com/zoj613/pyloras.git
 $ cd pyloras/
-$ poetry install
-# add package to python's path
-$ export PYTHONPATH=$PWD:$PYTHONPATH 
+$ pip install .
 ```
 
 ## Usage
 
 ```python
 from collections import Counter
 from pyloras import LORAS
@@ -109,8 +101,7 @@
 
 
 [1]: https://python-poetry.org/docs/pyproject/
 [2]: https://imbalanced-learn.org/stable/auto_examples/over-sampling/plot_comparison_over_sampling.html#more-advanced-over-sampling-using-adasyn-and-smote
 [3]: https://img.shields.io/github/workflow/status/zoj613/pyloras/CI/main?style=flat-square
 [4]: https://img.shields.io/codecov/c/github/zoj613/pyloras?style=flat-square
 [5]: https://img.shields.io/github/v/release/zoj613/pyloras?include_prereleases&style=flat-square
-
```


# Comparing `tmp/autora-synthetic-data-1.0.0a0.tar.gz` & `tmp/autora-synthetic-data-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-synthetic-data-1.0.0a0.tar", last modified: Fri Apr 28 20:50:16 2023, max compression
+gzip compressed data, was "autora-synthetic-data-1.0.0a1.tar", last modified: Fri Apr 28 22:10:21 2023, max compression
```

## Comparing `autora-synthetic-data-1.0.0a0.tar` & `autora-synthetic-data-1.0.0a1.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:50:16.265471 autora-synthetic-data-1.0.0a0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:50:16.253471 autora-synthetic-data-1.0.0a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:50:16.257471 autora-synthetic-data-1.0.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:50:16.257471 autora-synthetic-data-1.0.0a0/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-28 20:50:16.265471 autora-synthetic-data-1.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:50:16.257471 autora-synthetic-data-1.0.0a0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   171200 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/docs/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:50:16.257471 autora-synthetic-data-1.0.0a0/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:50:16.261471 autora-synthetic-data-1.0.0a0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/mkdocs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 20:50:16.265471 autora-synthetic-data-1.0.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:50:16.253471 autora-synthetic-data-1.0.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:50:16.253471 autora-synthetic-data-1.0.0a0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:50:16.261471 autora-synthetic-data-1.0.0a0/src/autora/synthetic/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/src/autora/synthetic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:50:16.261471 autora-synthetic-data-1.0.0a0/src/autora/synthetic/data/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/src/autora/synthetic/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/src/autora/synthetic/data/expected_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/src/autora/synthetic/data/prospect_theory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/src/autora/synthetic/data/weber_fechner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/src/autora/synthetic/inventory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:50:16.265471 autora-synthetic-data-1.0.0a0/src/autora_synthetic_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-28 20:50:16.000000 autora-synthetic-data-1.0.0a0/src/autora_synthetic_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-28 20:50:16.000000 autora-synthetic-data-1.0.0a0/src/autora_synthetic_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 20:50:16.000000 autora-synthetic-data-1.0.0a0/src/autora_synthetic_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 20:50:16.000000 autora-synthetic-data-1.0.0a0/src/autora_synthetic_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 20:50:16.000000 autora-synthetic-data-1.0.0a0/src/autora_synthetic_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:50:16.265471 autora-synthetic-data-1.0.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-28 20:50:04.000000 autora-synthetic-data-1.0.0a0/tests/test_synthetic_inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.768044 autora-synthetic-data-1.0.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.760044 autora-synthetic-data-1.0.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.764044 autora-synthetic-data-1.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.764044 autora-synthetic-data-1.0.0a1/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-28 22:10:21.768044 autora-synthetic-data-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.764044 autora-synthetic-data-1.0.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   200744 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/docs/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.764044 autora-synthetic-data-1.0.0a1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.764044 autora-synthetic-data-1.0.0a1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/mkdocs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:10:21.768044 autora-synthetic-data-1.0.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.760044 autora-synthetic-data-1.0.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.760044 autora-synthetic-data-1.0.0a1/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.764044 autora-synthetic-data-1.0.0a1/src/autora/synthetic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/src/autora/synthetic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.764044 autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/expected_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/prospect_theory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/template_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/weber_fechner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/src/autora/synthetic/inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.768044 autora-synthetic-data-1.0.0a1/src/autora_synthetic_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-28 22:10:21.000000 autora-synthetic-data-1.0.0a1/src/autora_synthetic_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-28 22:10:21.000000 autora-synthetic-data-1.0.0a1/src/autora_synthetic_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:10:21.000000 autora-synthetic-data-1.0.0a1/src/autora_synthetic_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 22:10:21.000000 autora-synthetic-data-1.0.0a1/src/autora_synthetic_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 22:10:21.000000 autora-synthetic-data-1.0.0a1/src/autora_synthetic_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.768044 autora-synthetic-data-1.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/tests/test_synthetic_inventory.py
```

### Comparing `autora-synthetic-data-1.0.0a0/.github/workflows/python-publish.yml` & `autora-synthetic-data-1.0.0a1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a0/.gitignore` & `autora-synthetic-data-1.0.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a0/.pre-commit-config.yaml` & `autora-synthetic-data-1.0.0a1/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,15 @@
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         args:
         - "--max-line-length=100"
         - "--extend-ignore=E203"
+        - "--per-file-ignores=__init__.py:F401"
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: "v0.991"
     hooks:
       - id: mypy
         additional_dependencies: [types-requests]
         language_version: python3.8
 default_language_version:
```

### Comparing `autora-synthetic-data-1.0.0a0/docs/example.ipynb` & `autora-synthetic-data-1.0.0a1/docs/example.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9873697916666666%*

 * *Differences: {"'cells'": "{1: {'execution_count': 1, 'metadata': {'ExecuteTime': {'start_time': "*

 * *            "'2023-04-28T17:42:23.289816Z', 'end_time': '2023-04-28T17:42:23.303951Z'}}}, 4: "*

 * *            "{'execution_count': 3, 'outputs': [OrderedDict([('data', OrderedDict([('text/plain', "*

 * *            "'<Figure size 640x480 with 1 Axes>'), ('image/png', "*

 * *            "'iVBORw0KGgoAAAANSUhEUgAAAjIAAAHHCAYAAACle7JuAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9 […]*

```diff
@@ -1,49 +1,80 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {
+                "collapsed": false
+            },
+            "source": [
+                "# Synthetic Experiment Examples"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 1,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-28T16:19:36.348756Z",
-                    "start_time": "2023-04-28T16:19:36.313460Z"
+                    "end_time": "2023-04-28T17:42:23.303951Z",
+                    "start_time": "2023-04-28T17:42:23.289816Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "# Uncomment the following line when running on Google Colab\n",
                 "# !pip install autora-synthetic-data"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": 2,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2023-04-28T17:42:23.394904Z",
+                    "start_time": "2023-04-28T17:42:23.306156Z"
+                },
+                "collapsed": false
+            },
+            "outputs": [],
+            "source": [
+                "from autora.synthetic import retrieve, describe\n",
+                "import numpy as np"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
                 "The registry is accessed using the `retrieve` function, optionally setting parameters:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 3,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-28T16:19:36.349420Z",
-                    "start_time": "2023-04-28T16:19:36.318746Z"
+                    "end_time": "2023-04-28T17:42:23.696577Z",
+                    "start_time": "2023-04-28T17:42:23.395394Z"
                 },
                 "collapsed": false
             },
-            "outputs": [],
-            "source": [
-                "from autora.synthetic import retrieve, describe\n",
-                "import numpy as np"
-            ]
+            "outputs": [
+                {
+                    "data": {
+                        "image/png": "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qRN79+7l2LFjBY7Zt2/fQq+HKerrWZRcTz/9NBaLJf96mzZtsNlsHDp0qFBZRRyVFvuKmGjv3r2kpqYSFBR02duTk5MLXP/rmxuAv78/AKGhoZfd/vd1Ni4uLtSqVavAtnr16gH840emL168yIQJE5g9ezbHjh0rsKYmNTX1ivf70969e4E/3qAv53Il43LCw8Pp0KHDVffr2bMnn376KUuWLOHpp5+mffv2l92vbt26l2yrV68en3/+OQD79u3DMAxGjBjBiBEjLnuM5OTkAmWoZs2ahflRgKK/nkXJ9ffHKl++fIFjijgrFRkRE9ntdoKCgpgzZ85lb69UqVKB61f6n/6VthtXWcRbWP3792f27NkMGjSIW265BX9/fywWCz179sRut1/1/n/u88knnxASEnLJ7a6uxftP0dmzZ9m8eTPwx0fC7XY7Li7XPgD9Z+7nn3+eTp06XXafOnXqFLj+19Grqynq61mUXCX9OyJiFhUZERPVrl2b5cuXEx0dfU1vgEVlt9vZv39//igMwJ49ewD+8bwvX3zxBb179+att97K35aVlUVKSkqB/f46dfFXtWvXBiAoKKhQIyrXKzY2lvT0dCZMmMCwYcOYPHkyQ4YMuWS/P0eK/mrPnj35z8Wfo1dubm43JHdhlVSuK71+Io5Ma2RETNSjRw9sNhtjx4695La8vLxLikJxiIuLy/+zYRjExcXh5uZ2xekX+ON/83//n/u0adOw2WwFtnl7ewNckrtTp074+fkxfvx4cnNzLzn+Xz8GfL2++OILPvvsMyZOnMjQoUPp2bMnw4cPzy9sf7Vo0aICa0k2btzIhg0buOuuu4A/ile7du2YNWsWJ06cKNHc16Kkcnl7e5fI75xISdKIjIiJ2rZty7///W8mTJhAYmIid955J25ubuzdu5cFCxYwZcqUYj0BnKenJ99//z29e/emVatWLF26lCVLlvDyyy9fMo31V126dOGTTz7B39+fRo0asW7dOpYvX06FChUK7NesWTOsViuvv/46qampeHh4cMcddxAUFMSMGTN49NFHiYqKomfPnlSqVInDhw+zZMkSoqOjCxSsK1m9ejVZWVmXbG/atClNmzYlOTmZZ555httvvz1/UXNcXBwrV66kT58+rFmzpsAUU506dbj11lt55plnyM7OZvLkyVSoUIEXX3wxf5/p06dz6623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2wEoX748FouFPn368PHHH1OhQgWys7ML/Exdu3bl0UcfLeZnSkSuh4qMiJSYjz76CG9vbzZs2MCkSZN49dVXWbZsGQCbNm0CYPbs2Zw4cSL/+urVq3nssccYOHAgO3bsYNasWXz44YeMGzeuwLHHjBlDjx492Lp1K3fffTcPP/ww586dA2DEiBHs2LGDpUuXsnPnTmbMmEHFihUvyRcaGsqXX34JwO7duzlx4gRTpkyhe/fu2Gy2AuUoOTmZJUuW6FuKRRyMioyIlJimTZsyatQo6taty2OPPUaLFi1YsWIFAJUqVQIgICCAkJCQ/Otjxoxh6NCh9O7dm1q1atGxY0fGjh3LrFmzChy7T58+9OrVizp16jB+/HguXLjAxo0bATh8+DCRkZG0aNGCsLAwOnTowD333HNJPqvVSmBgIABBQUGEhITg7++Pl5cXMTEx+aM4AJ9++inVq1enXbt2xf48iUjRaY2MiJSYpk2bFrheuXJlkpOT//E+W7ZsYe3atQVGYGw2G1lZWWRmZlKuXLlLju3t7Y2fn1/+sZ955hkeeOAB4uPjufPOO+natSutW7e+pux9+/alZcuWHDt2jKpVq/Lhhx/Sp08fLBbLNR1HREqWioyIlBg3N7cC1y0WC3a7/R/vc+HCBcaMGcP9999/yW2enp6FOvZdd93FoUOH+O6771i2bBnt27cnNjaWN998s9DZIyMjiYiI4OOPP+bOO+9k+/btLFmypND3F5EbQ0VGREzj5uaGzWYrsC0qKordu3dTp06d6zp2pUqV6N27N71796ZNmza88MILly0y7u7uAJfkAHjqqaeYPHkyx44do0OHDoSGhl5XJhEpflojIyKmCQsLY8WKFZw8eZLz588DMHLkSD7++GPGjBnD9u3b2blzJ/Pnz2f48OGFPu7IkSNZvHgx+/btY/v27Xz77bc0bNjwsvvWqFEDi8XCt99+y+nTp7lw4UL+bTExMRw9epT3339fi3xFHJSKjIiY5q233mLZsmWEhoYSGRkJQKdOnfj222/58ccfadmyJTfffDPvvPMONWrUKPRx3d3dGTZsGE2bNuW2227DarUyf/78y+5btWrV/AXGwcHB9OvXL/82f39/HnjgAXx8fK7pRH8icuNYDMMwzA4hIuKo2rdvT+PGjZk6darZUUTkMlRkREQu4/z586xatYoHH3yQHTt2UL9+fbMjichlaLGviMhlREZGcv78eV5//XWVGBEHphEZERERcVpa7CsiIiJOS0VGREREnJaKjIiIiDgtFRkRERFxWioyIiIi4rRUZERERMRpqciIiIiI01KREREREaelIiMiIiJO6/8BAr89BR5J2vAAAAAASUVORK5CYII=",
+                        "text/plain": "<Figure size 640x480 with 1 Axes>"
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                }
+            ],
+            "source": []
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
```

### Comparing `autora-synthetic-data-1.0.0a0/mkdocs/base.yml` & `autora-synthetic-data-1.0.0a1/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a0/mkdocs/gen_ref_pages.py` & `autora-synthetic-data-1.0.0a1/mkdocs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a0/pyproject.toml` & `autora-synthetic-data-1.0.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a0/src/autora/synthetic/__init__.py` & `autora-synthetic-data-1.0.0a1/src/autora/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a0/src/autora/synthetic/data/expected_value.py` & `autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/expected_value.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a0/src/autora/synthetic/data/prospect_theory.py` & `autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/prospect_theory.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a0/src/autora/synthetic/data/weber_fechner.py` & `autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/weber_fechner.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,9 +149,11 @@
         domain=domain,
         plotter=plotter,
         params=params,
     )
     return collection
 
 
-register("weber-fechner", weber_fechner_law)  # todo: make a better interface for multiple aliases
+register(
+    "weber-fechner", weber_fechner_law
+)  # todo: make a better interface for multiple aliases
 register("weber_fechner", weber_fechner_law)
```

### Comparing `autora-synthetic-data-1.0.0a0/src/autora/synthetic/inventory.py` & `autora-synthetic-data-1.0.0a1/src/autora/synthetic/inventory.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a0/src/autora_synthetic_data.egg-info/SOURCES.txt` & `autora-synthetic-data-1.0.0a1/src/autora_synthetic_data.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 README.md
 mkdocs.yml
 pyproject.toml
 .github/workflows/docs-publish.yml
 .github/workflows/python-publish.yml
 .idea/.gitignore
 .idea/misc.xml
+.idea/modules.xml
+.idea/vcs.xml
 docs/example.ipynb
 docs/index.md
-docs/quickstart.md
 docs/javascripts/mathjax.js
 mkdocs/base.yml
 mkdocs/gen_ref_pages.py
 src/autora/synthetic/__init__.py
 src/autora/synthetic/inventory.py
 src/autora/synthetic/data/__init__.py
 src/autora/synthetic/data/expected_value.py
 src/autora/synthetic/data/prospect_theory.py
+src/autora/synthetic/data/template_experiment.py
 src/autora/synthetic/data/weber_fechner.py
 src/autora_synthetic_data.egg-info/PKG-INFO
 src/autora_synthetic_data.egg-info/SOURCES.txt
 src/autora_synthetic_data.egg-info/dependency_links.txt
 src/autora_synthetic_data.egg-info/requires.txt
 src/autora_synthetic_data.egg-info/top_level.txt
 tests/README.md
```

### Comparing `autora-synthetic-data-1.0.0a0/tests/README.md` & `autora-synthetic-data-1.0.0a1/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a0/tests/test_synthetic_inventory.py` & `autora-synthetic-data-1.0.0a1/tests/test_synthetic_inventory.py`

 * *Files identical despite different names*


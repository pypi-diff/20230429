# Comparing `tmp/bayesian-models-0.1.0.tar.gz` & `tmp/bayesian-models-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesian-models-0.1.0.tar", last modified: Wed Apr  5 09:13:35 2023, max compression
+gzip compressed data, was "bayesian-models-0.1.1.tar", last modified: Sat Apr 29 06:54:36 2023, max compression
```

## Comparing `bayesian-models-0.1.0.tar` & `bayesian-models-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        0 2023-04-05 09:13:35.513081 bayesian-models-0.1.0/
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    11345 2023-04-05 07:25:49.000000 bayesian-models-0.1.0/LICENSE
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)       38 2023-02-20 09:01:11.000000 bayesian-models-0.1.0/MANIFEST.in
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     2751 2023-04-05 09:13:35.512589 bayesian-models-0.1.0/PKG-INFO
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     1787 2023-04-05 09:05:08.000000 bayesian-models-0.1.0/README.md
-drwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        0 2023-04-05 09:13:35.419417 bayesian-models-0.1.0/bayesian_models/
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        1 2023-04-05 07:25:44.000000 bayesian-models-0.1.0/bayesian_models/__init__.py
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    59828 2023-04-05 07:25:49.000000 bayesian-models-0.1.0/bayesian_models/core.py
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)   129623 2023-04-05 07:25:49.000000 bayesian-models-0.1.0/bayesian_models/data.py
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     3708 2023-04-05 07:25:49.000000 bayesian-models-0.1.0/bayesian_models/math.py
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    63312 2023-04-05 07:25:49.000000 bayesian-models-0.1.0/bayesian_models/models.py
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)      979 2023-04-05 07:25:49.000000 bayesian-models-0.1.0/bayesian_models/typing.py
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     4831 2023-04-05 07:25:49.000000 bayesian-models-0.1.0/bayesian_models/utilities.py
-drwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        0 2023-04-05 09:13:35.511446 bayesian-models-0.1.0/bayesian_models.egg-info/
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     2751 2023-04-05 09:13:35.000000 bayesian-models-0.1.0/bayesian_models.egg-info/PKG-INFO
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)      419 2023-04-05 09:13:35.000000 bayesian-models-0.1.0/bayesian_models.egg-info/SOURCES.txt
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        1 2023-04-05 09:13:35.000000 bayesian-models-0.1.0/bayesian_models.egg-info/dependency_links.txt
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)      123 2023-04-05 09:13:35.000000 bayesian-models-0.1.0/bayesian_models.egg-info/requires.txt
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)       16 2023-04-05 09:13:35.000000 bayesian-models-0.1.0/bayesian_models.egg-info/top_level.txt
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     1247 2023-04-05 09:13:08.000000 bayesian-models-0.1.0/pyproject.toml
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)       38 2023-04-05 09:13:35.513225 bayesian-models-0.1.0/setup.cfg
+drwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        0 2023-04-29 06:54:36.866457 bayesian-models-0.1.1/
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    11345 2023-04-05 10:48:24.000000 bayesian-models-0.1.1/LICENSE
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)       38 2023-02-20 09:01:11.000000 bayesian-models-0.1.1/MANIFEST.in
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     2759 2023-04-29 06:54:36.866064 bayesian-models-0.1.1/PKG-INFO
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     1787 2023-04-05 10:48:24.000000 bayesian-models-0.1.1/README.md
+drwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        0 2023-04-29 06:54:36.860743 bayesian-models-0.1.1/bayesian_models/
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        1 2023-04-05 10:48:24.000000 bayesian-models-0.1.1/bayesian_models/__init__.py
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    59828 2023-04-29 06:49:27.000000 bayesian-models-0.1.1/bayesian_models/core.py
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)   129623 2023-04-29 06:49:27.000000 bayesian-models-0.1.1/bayesian_models/data.py
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     3708 2023-04-05 10:48:24.000000 bayesian-models-0.1.1/bayesian_models/math.py
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    63312 2023-04-29 06:53:57.000000 bayesian-models-0.1.1/bayesian_models/models.py
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)      979 2023-04-29 06:49:27.000000 bayesian-models-0.1.1/bayesian_models/typing.py
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     4831 2023-04-29 06:49:27.000000 bayesian-models-0.1.1/bayesian_models/utilities.py
+drwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        0 2023-04-29 06:54:36.865160 bayesian-models-0.1.1/bayesian_models.egg-info/
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     2759 2023-04-29 06:54:36.000000 bayesian-models-0.1.1/bayesian_models.egg-info/PKG-INFO
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)      419 2023-04-29 06:54:36.000000 bayesian-models-0.1.1/bayesian_models.egg-info/SOURCES.txt
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        1 2023-04-29 06:54:36.000000 bayesian-models-0.1.1/bayesian_models.egg-info/dependency_links.txt
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)      123 2023-04-29 06:54:36.000000 bayesian-models-0.1.1/bayesian_models.egg-info/requires.txt
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)       16 2023-04-29 06:54:36.000000 bayesian-models-0.1.1/bayesian_models.egg-info/top_level.txt
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     1255 2023-04-29 06:49:27.000000 bayesian-models-0.1.1/pyproject.toml
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)       38 2023-04-29 06:54:36.866590 bayesian-models-0.1.1/setup.cfg
```

### Comparing `bayesian-models-0.1.0/LICENSE` & `bayesian-models-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.0/PKG-INFO` & `bayesian-models-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: bayesian-models
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for building common bayesian models in pymc
 Author-email: Alexander Rodis <alexanderrhodis@gmail.com>
 Maintainer-email: Alexander Rodis <alexanderrhodis@gmail.com>
 Project-URL: Homepage, https://github.com/AlexRodis/bayesian_models
 Project-URL: Bug Tracker, https://github.com/AlexRodis/bayesian_models/issues
 Project-URL: Documentation, https://bayesian-models.readthedocs.io/en/latest/
 Keywords: bayesian,models,statistics,pymc
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 Provides-Extra: GPU
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `bayesian-models-0.1.0/README.md` & `bayesian-models-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.0/bayesian_models/core.py` & `bayesian-models-0.1.1/bayesian_models/core.py`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.0/bayesian_models/data.py` & `bayesian-models-0.1.1/bayesian_models/data.py`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.0/bayesian_models/math.py` & `bayesian-models-0.1.1/bayesian_models/math.py`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.0/bayesian_models/models.py` & `bayesian-models-0.1.1/bayesian_models/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 #   This module contains model definitions
 
-import pymc as pymc, pm
+import pymc as pm, pymc
 import typing
 from typing import Any, Union, Callable, Optional
 from abc import ABC, abstractmethod
 import pandas as pd
 import numpy as np
 import xarray as xr
 import arviz as az
```

### Comparing `bayesian-models-0.1.0/bayesian_models/typing.py` & `bayesian-models-0.1.1/bayesian_models/typing.py`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.0/bayesian_models/utilities.py` & `bayesian-models-0.1.1/bayesian_models/utilities.py`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.0/bayesian_models.egg-info/PKG-INFO` & `bayesian-models-0.1.1/bayesian_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: bayesian-models
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for building common bayesian models in pymc
 Author-email: Alexander Rodis <alexanderrhodis@gmail.com>
 Maintainer-email: Alexander Rodis <alexanderrhodis@gmail.com>
 Project-URL: Homepage, https://github.com/AlexRodis/bayesian_models
 Project-URL: Bug Tracker, https://github.com/AlexRodis/bayesian_models/issues
 Project-URL: Documentation, https://bayesian-models.readthedocs.io/en/latest/
 Keywords: bayesian,models,statistics,pymc
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 Provides-Extra: GPU
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `bayesian-models-0.1.0/pyproject.toml` & `bayesian-models-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "bayesian-models"
 
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Alexander Rodis", email="alexanderrhodis@gmail.com" },
 ]
 
 maintainers = [
     { name="Alexander Rodis", email="alexanderrhodis@gmail.com" },
 ]
@@ -15,15 +15,15 @@
 
 readme = 'README.md'
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: Apache Software License",
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Healthcare Industry",
     "Intended Audience :: Developers",
 
 ]
 
 keywords = ["bayesian", "models", "statistics", "pymc"]
```


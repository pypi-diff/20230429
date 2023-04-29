# Comparing `tmp/statinf-1.2.2.tar.gz` & `tmp/statinf-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statinf-1.2.2.tar", last modified: Mon Apr 10 12:25:05 2023, max compression
+gzip compressed data, was "statinf-1.2.3.tar", last modified: Sat Apr 29 17:49:44 2023, max compression
```

## Comparing `statinf-1.2.2.tar` & `statinf-1.2.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-10 12:25:05.507358 statinf-1.2.2/
--rw-r--r--   0 florian   (1000) florian   (1000)     1070 2020-10-01 18:31:13.000000 statinf-1.2.2/LICENSE
--rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-04-10 12:25:05.507358 statinf-1.2.2/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     8337 2020-10-01 18:31:13.000000 statinf-1.2.2/README.md
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-04-10 12:25:05.507358 statinf-1.2.2/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)      781 2020-10-01 18:31:13.000000 statinf-1.2.2/setup.py
--rw-r--r--   0 florian   (1000) florian   (1000)      889 2023-04-10 12:25:05.000000 statinf-1.2.2/setup_new.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-10 12:25:05.487358 statinf-1.2.2/statinf/
--rw-r--r--   0 florian   (1000) florian   (1000)       22 2023-04-10 12:25:05.000000 statinf-1.2.2/statinf/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-10 12:25:05.497358 statinf-1.2.2/statinf/data/
--rw-r--r--   0 florian   (1000) florian   (1000)     2701 2023-02-03 18:48:52.000000 statinf-1.2.2/statinf/data/GenerateData.py
--rw-r--r--   0 florian   (1000) florian   (1000)    27132 2021-03-24 14:33:31.000000 statinf-1.2.2/statinf/data/ProcessData.py
--rw-r--r--   0 florian   (1000) florian   (1000)       55 2020-10-01 18:31:13.000000 statinf-1.2.2/statinf/data/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-10 12:25:05.497358 statinf-1.2.2/statinf/distributions/
--rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-02-03 18:27:09.000000 statinf-1.2.2/statinf/distributions/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    22636 2023-04-10 12:16:43.000000 statinf-1.2.2/statinf/distributions/discrete.py
--rw-r--r--   0 florian   (1000) florian   (1000)       26 2021-06-27 12:48:10.000000 statinf-1.2.2/statinf/init_template.py
--rw-r--r--   0 florian   (1000) florian   (1000)     5107 2021-06-27 13:22:48.000000 statinf-1.2.2/statinf/misc.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-10 12:25:05.497358 statinf-1.2.2/statinf/ml/
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2020-10-01 18:31:13.000000 statinf-1.2.2/statinf/ml/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2522 2021-03-07 06:24:49.000000 statinf-1.2.2/statinf/ml/activations.py
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2020-10-17 16:20:51.000000 statinf-1.2.2/statinf/ml/generative.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2892 2021-03-07 06:09:35.000000 statinf-1.2.2/statinf/ml/initializations.py
--rw-r--r--   0 florian   (1000) florian   (1000)     3152 2021-03-07 06:45:42.000000 statinf-1.2.2/statinf/ml/losses.py
--rw-r--r--   0 florian   (1000) florian   (1000)    16863 2022-08-21 10:47:32.000000 statinf-1.2.2/statinf/ml/neuralnetwork.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11152 2021-03-07 08:40:43.000000 statinf-1.2.2/statinf/ml/optimizers.py
--rw-r--r--   0 florian   (1000) florian   (1000)     6141 2021-06-27 13:22:59.000000 statinf-1.2.2/statinf/ml/performance.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-10 12:25:05.497358 statinf-1.2.2/statinf/nonparametrics/
--rw-r--r--   0 florian   (1000) florian   (1000)       23 2020-11-01 11:38:35.000000 statinf-1.2.2/statinf/nonparametrics/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)      842 2020-11-01 18:05:22.000000 statinf-1.2.2/statinf/nonparametrics/kernels.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-10 12:25:05.507358 statinf-1.2.2/statinf/regressions/
--rw-r--r--   0 florian   (1000) florian   (1000)    19249 2021-03-24 15:58:55.000000 statinf-1.2.2/statinf/regressions/LinearModels.py
--rw-r--r--   0 florian   (1000) florian   (1000)       51 2023-02-03 18:26:31.000000 statinf-1.2.2/statinf/regressions/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    18168 2021-03-24 15:54:37.000000 statinf-1.2.2/statinf/regressions/glm.py
--rw-r--r--   0 florian   (1000) florian   (1000)     7060 2020-10-01 18:31:13.000000 statinf-1.2.2/statinf/regressions/glm_test.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-10 12:25:05.507358 statinf-1.2.2/statinf/stats/
--rw-r--r--   0 florian   (1000) florian   (1000)      126 2020-11-01 12:20:16.000000 statinf-1.2.2/statinf/stats/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     6950 2020-11-01 18:03:36.000000 statinf-1.2.2/statinf/stats/bayesian.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4185 2020-10-01 18:31:13.000000 statinf-1.2.2/statinf/stats/descriptive.py
--rw-r--r--   0 florian   (1000) florian   (1000)    21520 2023-02-03 18:58:48.000000 statinf-1.2.2/statinf/stats/tests.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11524 2020-10-27 02:35:31.000000 statinf-1.2.2/statinf/stats/timeseries.py
--rw-r--r--   0 florian   (1000) florian   (1000)    10469 2020-11-01 18:02:58.000000 statinf-1.2.2/statinf/stats/unsupervised.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-10 12:25:05.497358 statinf-1.2.2/statinf.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-04-10 12:25:05.000000 statinf-1.2.2/statinf.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      966 2023-04-10 12:25:05.000000 statinf-1.2.2/statinf.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-04-10 12:25:05.000000 statinf-1.2.2/statinf.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      101 2023-04-10 12:25:05.000000 statinf-1.2.2/statinf.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-04-10 12:25:05.000000 statinf-1.2.2/statinf.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-29 17:49:44.373417 statinf-1.2.3/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1070 2020-10-01 18:31:13.000000 statinf-1.2.3/LICENSE
+-rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-04-29 17:49:44.373417 statinf-1.2.3/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     8337 2020-10-01 18:31:13.000000 statinf-1.2.3/README.md
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-04-29 17:49:44.373417 statinf-1.2.3/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)      781 2020-10-01 18:31:13.000000 statinf-1.2.3/setup.py
+-rw-r--r--   0 florian   (1000) florian   (1000)      889 2023-04-29 17:49:43.000000 statinf-1.2.3/setup_new.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-29 17:49:44.363417 statinf-1.2.3/statinf/
+-rw-r--r--   0 florian   (1000) florian   (1000)       22 2023-04-29 17:49:43.000000 statinf-1.2.3/statinf/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-29 17:49:44.363417 statinf-1.2.3/statinf/data/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2701 2023-02-03 18:48:52.000000 statinf-1.2.3/statinf/data/GenerateData.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    27132 2021-03-24 14:33:31.000000 statinf-1.2.3/statinf/data/ProcessData.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       55 2020-10-01 18:31:13.000000 statinf-1.2.3/statinf/data/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-29 17:49:44.363417 statinf-1.2.3/statinf/distributions/
+-rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-02-03 18:27:09.000000 statinf-1.2.3/statinf/distributions/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    20379 2023-04-29 16:28:26.000000 statinf-1.2.3/statinf/distributions/discrete.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       26 2021-06-27 12:48:10.000000 statinf-1.2.3/statinf/init_template.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     5107 2021-06-27 13:22:48.000000 statinf-1.2.3/statinf/misc.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-29 17:49:44.373417 statinf-1.2.3/statinf/ml/
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2020-10-01 18:31:13.000000 statinf-1.2.3/statinf/ml/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2522 2021-03-07 06:24:49.000000 statinf-1.2.3/statinf/ml/activations.py
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2020-10-17 16:20:51.000000 statinf-1.2.3/statinf/ml/generative.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2892 2021-03-07 06:09:35.000000 statinf-1.2.3/statinf/ml/initializations.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     3152 2021-03-07 06:45:42.000000 statinf-1.2.3/statinf/ml/losses.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    16863 2022-08-21 10:47:32.000000 statinf-1.2.3/statinf/ml/neuralnetwork.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11152 2021-03-07 08:40:43.000000 statinf-1.2.3/statinf/ml/optimizers.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     6141 2021-06-27 13:22:59.000000 statinf-1.2.3/statinf/ml/performance.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-29 17:49:44.373417 statinf-1.2.3/statinf/nonparametrics/
+-rw-r--r--   0 florian   (1000) florian   (1000)       23 2020-11-01 11:38:35.000000 statinf-1.2.3/statinf/nonparametrics/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)      842 2020-11-01 18:05:22.000000 statinf-1.2.3/statinf/nonparametrics/kernels.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-29 17:49:44.373417 statinf-1.2.3/statinf/regressions/
+-rw-r--r--   0 florian   (1000) florian   (1000)    19249 2021-03-24 15:58:55.000000 statinf-1.2.3/statinf/regressions/LinearModels.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       51 2023-02-03 18:26:31.000000 statinf-1.2.3/statinf/regressions/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    18168 2021-03-24 15:54:37.000000 statinf-1.2.3/statinf/regressions/glm.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     7060 2020-10-01 18:31:13.000000 statinf-1.2.3/statinf/regressions/glm_test.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-29 17:49:44.373417 statinf-1.2.3/statinf/stats/
+-rw-r--r--   0 florian   (1000) florian   (1000)      126 2020-11-01 12:20:16.000000 statinf-1.2.3/statinf/stats/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     6950 2020-11-01 18:03:36.000000 statinf-1.2.3/statinf/stats/bayesian.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4185 2020-10-01 18:31:13.000000 statinf-1.2.3/statinf/stats/descriptive.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    21520 2023-02-03 18:58:48.000000 statinf-1.2.3/statinf/stats/tests.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11524 2020-10-27 02:35:31.000000 statinf-1.2.3/statinf/stats/timeseries.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    10469 2020-11-01 18:02:58.000000 statinf-1.2.3/statinf/stats/unsupervised.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-29 17:49:44.363417 statinf-1.2.3/statinf.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-04-29 17:49:44.000000 statinf-1.2.3/statinf.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      966 2023-04-29 17:49:44.000000 statinf-1.2.3/statinf.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-04-29 17:49:44.000000 statinf-1.2.3/statinf.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      101 2023-04-29 17:49:44.000000 statinf-1.2.3/statinf.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-04-29 17:49:44.000000 statinf-1.2.3/statinf.egg-info/top_level.txt
```

### Comparing `statinf-1.2.2/LICENSE` & `statinf-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/PKG-INFO` & `statinf-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statinf
-Version: 1.2.2
+Version: 1.2.3
 Summary: A library for statistics and causal inference
 Home-page: https://www.florianfelice.com/statinf
 Author: Florian Felice
 Author-email: florian.felice@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `statinf-1.2.2/README.md` & `statinf-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/setup.py` & `statinf-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/setup_new.py` & `statinf-1.2.3/setup_new.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="statinf",
-    version="1.2.2",
+    version="1.2.3",
     author="Florian Felice",
     author_email="florian.felice@outlook.com",
     description="A library for statistics and causal inference",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.florianfelice.com/statinf",
     packages=setuptools.find_packages(),
```

### Comparing `statinf-1.2.2/statinf/data/GenerateData.py` & `statinf-1.2.3/statinf/data/GenerateData.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/statinf/data/ProcessData.py` & `statinf-1.2.3/statinf/data/ProcessData.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/statinf/distributions/discrete.py` & `statinf-1.2.3/statinf/distributions/discrete.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from scipy import optimize
 import warnings
 
 
 scipy_methods = ['BFGS', 'L-BFGS-B', 'Newton-CG', 'CG', 'Powell', 'Nelder-Mead']
 
 # Empty object with future attributes
-class Object(object):
+class _Object(object):
     pass
 
 
 # Generic Discrete class for discrete probability functions
 class Discrete:
     def __init__(self) -> None:
         """A generic class for discrete probability distributions
@@ -67,15 +67,15 @@
         # _pmf = [_p for _p in _pmf if _p > 10e-8]
 
         _seed = seed if seed else datetime.datetime.now().microsecond
         np.random.seed(_seed)
         return [self._generate(_pmf, seed=_seed + i) for i in range(size)]
 
     def _fast_fit(self):
-        return ValueError('Fast or auto fit is not allowed for this distribution, please chose another value')
+        raise NotImplementedError('Fast or auto fit is not allowed for this distribution, please chose another value')
 
     def _fit(self, data, bounds=None, init_params=np.array([1]), verbose=False, method='auto', args=()):
         if method.lower() in ['auto', 'fast']:
             res = self._fast_fit(data)
         elif method in scipy_methods:
             if args == ():
                 nll_args = (data,)
@@ -106,30 +106,30 @@
         :formula: The probability mass function is defined by
 
             .. math:: \\mathbb{P}(X = x | \\lambda) = \\dfrac{\\lambda^{x}}{x!} e^{- \\lambda}
 
         The distribution assumes equi-dispersion, meaning that :math:`\\mathbb{E}(X) = \\mathbb{V}(X)`.
 
         :param lambda\\_: Parameter :math:`\\lambda` representing the both location (:math:`\\mathbb{E}(X)`) and the scale (:math:`\\mathbb{V}(X)`) parameters, defaults to None
-        :type lambda\\_: :obj:`obj`, optional
+        :type lambda\\_: :obj:`float`, optional
 
         :example:
 
         >>> from statinf.distributions import Poisson
         >>> # Let us generate a random sample of size 1000
         >>> x = Poisson(lambda_=2.5).sample(size=1000)
         >>> # We can also estimate the parameter from the generated sample
         >>> # We just need to initialize the class...
         >>> poiss = Poisson()
         >>> # ... and we can fit from the generated sample. The function returns a dictionary
         >>> poiss.fit(x)
         ... {'lambda_': 2.46}
         >>> # The class stores the value of the estimated parameters
         >>> print(poiss.lambda_)
-        ... 2.76
+        ... 2.46
         >>> # So we can generate more samples using the fitted parameters
         >>> y = poiss.sample(200)
 
         :reference: * DeGroot, M. H., & Schervish, M. J. (2012). `Probability and statistics <https://www.stat.cmu.edu/~mark/degroot/index.html>`_. Pearson Education.
         """
         super(Poisson, self).__init__(*args, **kwargs)
         self.lambda_ = lambda_
@@ -205,35 +205,36 @@
 
         :param data: Data to estimate the paramter from
         :type data: :obj:`numpy.array` or :obj:`list` or :obj:`pandas.Series`
 
         :return: Estmated parameters
         :rtype: :obj:`dict`
         """
-        res = Object()
+        res = _Object()
         data = np.asarray(data)
         res.x = [data.mean()]
         return res
 
     def fit(self, data, method='fast', **kwargs) -> dict:
         """Estimates the parameter :math:`\\lambda` of the distribution from empirical data based on Maximum Likelihood Estimation.
 
-        The Maximum Likihood Estimator also corresponds to the emprical mean
+        The Maximum Likihood Estimator also corresponds to the emprical mean:
 
             .. math:: \\hat{\\lambda}_{\\text{MLE}} = \\dfrac{1}{n} \\sum_{i=1}^{n} x_i
 
-        The 'fast' :obj:`method` is available to estimate the parameter directly from the emprical mean.
+        The `method = 'fast'` is available to estimate the parameter directly from the emprical mean.
+        Any other value for the parameter `method` will use classical MLE.
 
         :param data: Data to fit and estimate parameters from.
         :type data: :obj:`numpy.array` or :obj:`list` or :obj:`pandas.Series`
         :param method: Optimization method to estimate the parameters as in the scipy library (allows 'fast' value), defaults to 'L-BFGS-B'
-        :type method: obj:`str`, optional
+        :type method: :obj:`str`, optional
 
         :return: Estimated parameter
-        :rtype: obj:`dict`
+        :rtype: :obj:`dict`
         """
         bounds = [(self.eps, None)]
         init_params = np.array([1])
 
         res = self._fit(data=data, bounds=bounds, method=method, init_params=init_params, **kwargs)
         self.lambda_ = res.x[0]
 
@@ -242,31 +243,31 @@
         if method in scipy_methods:
             out.update({'nll': self.nll})
 
         return out
 
 
 class CMPoisson(Discrete):
-    def __init__(self, lambda_=None, nu_=None, j=250, *args, **kwargs) -> None:
+    def __init__(self, lambda_=None, nu_=None, j=500, *args, **kwargs) -> None:
         """Conway-Maxwell Poisson distribution.
         This class allows to generate a random variable based on selected parameters and size but also to fit some data and estimate the parameters by means of Maximum Likelihood Estimation (MLE).
 
         Introduced by Conway and Maxwell (1962), the Conway-Maxwell Poisson (aka CMP) is a generalization of the common Poisson distribution
         (:class:`statinf.distributions.discrete.Poisson`).
         The distribution can handle non equi-dispersion cases where :math:`\\mathbb{E}(X) \\neq \\mathbb{V}(X)`.
         The level of dispersion is captured by :math:`\\nu` such that underdispersion is captured when :math:`\\nu > 1`,
-        equidispersions :math:`\\nu = 1` and overdispersion when :math:`\\nu < 1`.
+        equidispersion :math:`\\nu = 1` and overdispersion when :math:`\\nu < 1`.
 
         :formulae: The probability mass function (pmf) is defined by
 
             .. math:: \\mathbb{P}(X = x | \\lambda, \\nu) = \\dfrac{\\lambda^{x}}{(x!)^{\\nu}} \\dfrac{1}{Z(\\lambda, \\nu)}
 
             where :math:`Z(\\lambda, \\nu) = \\sum_{j=0}^{\\infty} \\dfrac{\\lambda^{j}}{(j!)^{\\nu}}` is calculated in :py:meth:`statinf.distributions.discrete.CMPoisson.Z`.
 
-        Special cases of the CMP distribution include well-known distributions
+        Special cases of the CMP distribution include well-known distributions.
 
             * When :math:`\\nu = 1`, one recovers the Poisson distribution with parameter :math:`\\lambda`
             * When :math:`\\nu = 0` and :math:`\\lambda < 1` one recovers the geometric distribution with parameter :math:`p = 1 - \\lambda` for the probability of success
             * When :math:`\\nu \\rightarrow \\infty`, one finds the Bernoulli distribution with parameter :math:`p = \\frac{\\lambda}{1 + \\lambda}` for the probability of success
 
         :param lambda\\_: Parameter :math:`\\lambda` representing the generalized expectation, defaults to None
         :type lambda\\_: :obj:`float`, optional
@@ -306,20 +307,20 @@
 
         self._Z = None
 
         if (self.lambda_ is not None) & (self.nu_ is not None):
             assert self.lambda_ >= 0, ValueError('Value for parameter lambda must be strictly greater to 0 (lambda_ > 0)')
             assert self.nu_ >= 0, ValueError('Value for parameter nu must be greater or equal to 0 (nu_ >= 0)')
             warnings.filterwarnings("error")
-            self._Z = self.Z(lambda_=self.lambda_, nu_=self.nu_, j=self.j, approx=True)
+            self._Z = self.Z(lambda_=self.lambda_, nu_=self.nu_, j=self.j)
             warnings.resetwarnings()
 
-        self.nll_fun = lambda params, data, j, approx: self.nloglike(params=params, data=data, j=j, approx=approx, Z=self.Z)
+        self.nll_fun = lambda params, data, j: self.nloglike(params=params, data=data, j=j, Z=self.Z)
 
-    def Z(self, lambda_, nu_, j=None, approx=False, log=False) -> float:
+    def Z(self, lambda_, nu_, j=None, log=False) -> float:
         """Compute the :math:`Z` factor, normalizing constant.
 
         The factor :math:`Z(\\lambda, \\nu)` serves as a normalizing constant such that the distribution satisfies the basic probability axioms (i.e. the probability mass function sums up to 1).
 
         .. math::
 
             Z(\\lambda, \\nu) = \\sum_{j=0}^{\\infty} \\dfrac{\\lambda^{j}}{(j!)^{\\nu}}
@@ -333,83 +334,39 @@
 
         :param lambda\\_: First parameter :math:`\\lambda > 0` of the distribution
         :type lambda\\_: :obj:`float`, optional
         :param nu\\_: Second parameter :math:`\\nu > 0` of the distribution
         :type nu\\_: :obj:`float`, optional
         :param j: Length of the sum for the normalizing constant, if :obj:`None` then we use the value from the :obj:`__init__` method, defaults to None
         :type j: :obj:`int`, optional
-        :param approx: Use approximation form for computing :math:`Z(\\lambda, \\nu)`, defaults to False
-        :type approx: :obj:`bool`
-        :param approx: Compute :math:`Z(\\lambda, \\nu)`, defaults to False
-        :type approx: :obj:`bool`
+        :param log: Compute :math:`\\log(Z(\\lambda, \\nu))`, defaults to False
+        :type log: :obj:`bool`
 
-        :return: Z factor
+        :return: Normalizing factor :math:`Z`
         :rtype: :obj:`float`
         """
         j = j if j else self.j
 
-        if (nu_ > 1 - self.eps) & (nu_ < 1 + self.eps):
-            # ## Poisson distribution
-            # When nu = 1, then we have a Poisson distribution
-            z_i = math.exp(lambda_)
-        elif (nu_ > 0) & (nu_ < 0 + self.eps):
-            # ## Geometric distribution
-            # When nu = 0, then we have a geometric distribution
-            z_i = 1 / (1 - lambda_)
-        elif (approx) & ((nu_ < 1 + self.eps) or (lambda_ > (10 ** nu_))):
-            # ## Approximation
-            # If we want the approximation and it verifies the assumptions (for nu > 1 and lambda > 10^nu), we use approximation
-            _dec = False
-            # Compute numerator
-            try:
-                _num = math.exp(nu_ * (lambda_ ** (1 / nu_)))
-            except RuntimeWarning:
-                # If runtime warning it is similar to overflow error (i.e. output is too long), use Decimal format
-                _pow = Decimal(lambda_) ** Decimal(1 / nu_)
-                _num = Decimal(math.exp(Decimal(nu_) * _pow))
-                _dec = True
-
-            # Compute denominator
-            try:
-                _denom = lambda_ ** ((nu_ - 1) / (2 * nu_))
-                _denom *= (2 * math.pi) ** ((nu_ - 1) / 2)
-                _denom *= math.sqrt(nu_)
-                _o_lambda = 1 / (lambda_ ** (1 / nu_))
-            except RuntimeWarning:
-                _denom = Decimal(lambda_) ** Decimal((nu_ - 1) / (2 * nu_))
-                _denom *= Decimal(2 * math.pi) ** Decimal((nu_ - 1) / 2)
-                _denom *= Decimal(math.sqrt(nu_))
-                _o_lambda = Decimal(1) / (Decimal(lambda_) ** Decimal(1 / nu_))
-                _dec = True
-
-            if _dec:
-                _denom = Decimal(_denom)
-                _num = Decimal(_num)
-                _o_lambda = Decimal(_o_lambda)
-
-            # Compute the ratio
-            z_i = float(_num / _denom) * (1 + float(_o_lambda))
-        else:
-            # ## Almost exact form
-            z_i = - np.inf
-            z_last = 0
-            current_j = 0
-
-            while (np.abs(z_i - z_last) > self.eps) & (current_j < j):
-                z_last = z_i
-                _log_fact = np.sum(np.log(range(1, current_j)))
-                z_i = self.log_sum(z_i, current_j * math.log(lambda_) - nu_ * _log_fact)
-                current_j += 1
+        # ## Almost exact form
+        z_i = - np.inf
+        z_last = 0
+        current_j = 0
+
+        while (np.abs(z_i - z_last) > self.eps) & (current_j < j):
+            z_last = z_i
+            _log_fact = np.sum(np.log(range(1, current_j)))
+            z_i = self._log_sum(z_i, current_j * math.log(lambda_) - nu_ * _log_fact)
+            current_j += 1
 
-            if not log:
-                z_i = math.exp(z_i)
+        if not log:
+            z_i = math.exp(z_i)
 
         return float(np.sum(z_i))
 
-    def log_sum(self, x, y):
+    def _log_sum(self, x, y):
         if x == -np.inf:
             return y
         elif y == -np.inf:
             return x
         elif x > y:
             return x + math.log(1 + math.exp(y - x))
         else:
@@ -441,80 +398,79 @@
         except OverflowError:
             # Inf the integers to compute are too large, we use decimal format
             # Ref: https://stackoverflow.com/questions/16174399/overflowerror-long-int-too-large-to-convert-to-float-in-python
             _pow = [Decimal(p) for p in _pow]
             _dec = True
 
         # Compute $(x!)^{\nu}$
-        _fact = [pow(math.factorial(_x), self.nu_) for _x in x]
-        if _dec:
-            # If decimal was used for power calculations, we have to use the same for factorial
-            _fact = [Decimal(p) for p in _fact]
+        _fact = [pow(np.exp(np.sum(np.log(range(1, _x)))), self.nu_) for _x in x]
 
         a = np.array([float(p / f) for p, f in zip(_pow, _fact)])
         return a * (1 / self._Z)
 
     @staticmethod
-    def nloglike(params, data, Z, j=100, approx=False) -> float:
+    def nloglike(params, data, Z, j=100) -> float:
         """Static method to estumate the negative likelihood (used in :meth:`statinf.distributions.discrete.CMPoisson.fit` method).
 
         :formula: The log-likelihood function :math:`l` is defined by
 
             .. math:: \\mathcal{l}(x_1, ..., x_n | \\lambda, \\nu) = \\log (\\lambda) \\sum_{i}^{n} {x_i} - \\nu \\sum_{i}^{n} {\\log (x_i!)} - n \\log (Z(\\lambda, \\nu))
 
         :param params: List of parameters :math:`\\lambda` and :math:`\\nu`
         :type params: :obj:`list`
         :param data: Data to evaluate the netative log-likelihood on
         :type data: :obj:`numpy.array` or :obj:`list` or :obj:`pandas.Series`
         :param j: Length of the inifinite sum for the normalizing factor :math:`Z`, defaults to 100
         :type j: :obj:`int`, optional
-        :param approx: Use approximation form for computing :math:`Z(\\lambda, \\nu)`, defaults to False
-        :type approx: :obj:`bool`
 
         :return: Negative log-likelihood
         :rtype: :obj:`float`
         """
         lambda_ = params[0]
         nu_ = params[1]
         X = np.asarray(data)
+        n = len(X)
 
         # Compute log(Z)
-        log_Z = Z(lambda_=lambda_, nu_=nu_, j=j, approx=approx, log=True)
+        log_Z = Z(lambda_=lambda_, nu_=nu_, j=j, log=True)
 
         _log_fact = np.asarray([math.log(math.factorial(_x)) for _x in X])
-        ll = (math.log(lambda_) * np.sum(X)) - (nu_ * np.sum(_log_fact)) - (len(X) * log_Z)
+        ll = (math.log(lambda_) * np.sum(X)) - (nu_ * np.sum(_log_fact)) - (n * log_Z)
         return -ll
 
-    def fit(self, data, method='L-BFGS-B', init_params=np.array([1., 1.]), j=None, approx=False) -> dict:
+    def fit(self, data, method='L-BFGS-B', init_params='auto', j=None) -> dict:
         """Estimates the parameters :math:`\\lambda` and :math:`\\nu` of the distribution from empirical data based on Maximum Likelihood Estimation.
 
         .. note::
 
             There is no close form to estimate the parameters nor a direct relation between the empirical moments (:math:`\\bar{X}`) and the theoretical ones.
             Therefore, only MLE is available (no fast method).
 
         :param data: Data to fit and estimate parameters from.
         :type data: :obj:`numpy.array` or :obj:`list` or :obj:`pandas.Series`
         :param method: Optimization method to estimate the parameters, defaults to 'L-BFGS-B'
-        :type method: obj:`str`, optional
+        :type method: :obj:`str`, optional
         :param init_params: Initial parameters for the optimization method, defaults to obj:`np.array([1., 1.])`
-        :type init_params: obj:`numpy.array`, optional
+        :type init_params: :obj:`numpy.array`, optional
 
         :return: Estimated parameters
-        :rtype: obj:`dict`
+        :rtype: :obj:`dict`
         """
         # We transform warnings as error (for overflow) to handle in try / except: https://stackoverflow.com/questions/5644836/
         j = j if j else self.j
         bounds = [(self.eps, None), (self.eps, None)]
+        if init_params == 'auto':
+            _disp = data.std() / data.mean()
+            init_params = np.array([1., _disp])
 
-        res = self._fit(data=data, bounds=bounds, method=method, init_params=init_params, args=(j, approx))
+        res = self._fit(data=data, bounds=bounds, method=method, init_params=init_params, args=(j,))
         self.lambda_ = res.x[0]
         self.nu_ = res.x[1]
         warnings.filterwarnings("error")
-        self._Z = self.Z(lambda_=self.lambda_, nu_=self.nu_, j=j, approx=approx)
+        self._Z = self.Z(lambda_=self.lambda_, nu_=self.nu_, j=j)
         warnings.resetwarnings()
 
         out = {'lambda_': self.lambda_, 'nu_': self.nu_, 'convergence': res.success}
 
         if method in scipy_methods:
             out.update({'nll': self.nll})
```

### Comparing `statinf-1.2.2/statinf/misc.py` & `statinf-1.2.3/statinf/misc.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/statinf/ml/activations.py` & `statinf-1.2.3/statinf/ml/activations.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/statinf/ml/initializations.py` & `statinf-1.2.3/statinf/ml/initializations.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/statinf/ml/losses.py` & `statinf-1.2.3/statinf/ml/losses.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/statinf/ml/neuralnetwork.py` & `statinf-1.2.3/statinf/ml/neuralnetwork.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/statinf/ml/optimizers.py` & `statinf-1.2.3/statinf/ml/optimizers.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/statinf/ml/performance.py` & `statinf-1.2.3/statinf/ml/performance.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/statinf/nonparametrics/kernels.py` & `statinf-1.2.3/statinf/nonparametrics/kernels.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/statinf/regressions/LinearModels.py` & `statinf-1.2.3/statinf/regressions/LinearModels.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/statinf/regressions/glm.py` & `statinf-1.2.3/statinf/regressions/glm.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/statinf/regressions/glm_test.py` & `statinf-1.2.3/statinf/regressions/glm_test.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/statinf/stats/bayesian.py` & `statinf-1.2.3/statinf/stats/bayesian.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/statinf/stats/descriptive.py` & `statinf-1.2.3/statinf/stats/descriptive.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/statinf/stats/tests.py` & `statinf-1.2.3/statinf/stats/tests.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/statinf/stats/timeseries.py` & `statinf-1.2.3/statinf/stats/timeseries.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/statinf/stats/unsupervised.py` & `statinf-1.2.3/statinf/stats/unsupervised.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.2/statinf.egg-info/PKG-INFO` & `statinf-1.2.3/statinf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statinf
-Version: 1.2.2
+Version: 1.2.3
 Summary: A library for statistics and causal inference
 Home-page: https://www.florianfelice.com/statinf
 Author: Florian Felice
 Author-email: florian.felice@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `statinf-1.2.2/statinf.egg-info/SOURCES.txt` & `statinf-1.2.3/statinf.egg-info/SOURCES.txt`

 * *Files identical despite different names*


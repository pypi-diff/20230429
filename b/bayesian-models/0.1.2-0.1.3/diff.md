# Comparing `tmp/bayesian-models-0.1.2.tar.gz` & `tmp/bayesian-models-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesian-models-0.1.2.tar", last modified: Sat Apr 29 07:08:35 2023, max compression
+gzip compressed data, was "bayesian-models-0.1.3.tar", last modified: Sat Apr 29 10:43:35 2023, max compression
```

## Comparing `bayesian-models-0.1.2.tar` & `bayesian-models-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        0 2023-04-29 07:08:35.565791 bayesian-models-0.1.2/
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    11345 2023-04-29 07:04:58.000000 bayesian-models-0.1.2/LICENSE
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)       38 2023-02-20 09:01:11.000000 bayesian-models-0.1.2/MANIFEST.in
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     2759 2023-04-29 07:08:35.565295 bayesian-models-0.1.2/PKG-INFO
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     1787 2023-04-29 07:04:58.000000 bayesian-models-0.1.2/README.md
-drwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        0 2023-04-29 07:08:35.559721 bayesian-models-0.1.2/bayesian_models/
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        1 2023-04-29 07:04:58.000000 bayesian-models-0.1.2/bayesian_models/__init__.py
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    59828 2023-04-29 07:04:58.000000 bayesian-models-0.1.2/bayesian_models/core.py
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)   129623 2023-04-29 07:04:58.000000 bayesian-models-0.1.2/bayesian_models/data.py
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     3708 2023-04-29 07:04:58.000000 bayesian-models-0.1.2/bayesian_models/math.py
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    63312 2023-04-29 07:04:58.000000 bayesian-models-0.1.2/bayesian_models/models.py
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)      979 2023-04-29 07:04:58.000000 bayesian-models-0.1.2/bayesian_models/typing.py
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    29311 2023-04-29 07:06:28.000000 bayesian-models-0.1.2/bayesian_models/utilities.py
-drwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        0 2023-04-29 07:08:35.564357 bayesian-models-0.1.2/bayesian_models.egg-info/
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     2759 2023-04-29 07:08:35.000000 bayesian-models-0.1.2/bayesian_models.egg-info/PKG-INFO
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)      419 2023-04-29 07:08:35.000000 bayesian-models-0.1.2/bayesian_models.egg-info/SOURCES.txt
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        1 2023-04-29 07:08:35.000000 bayesian-models-0.1.2/bayesian_models.egg-info/dependency_links.txt
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)      123 2023-04-29 07:08:35.000000 bayesian-models-0.1.2/bayesian_models.egg-info/requires.txt
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)       16 2023-04-29 07:08:35.000000 bayesian-models-0.1.2/bayesian_models.egg-info/top_level.txt
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     1255 2023-04-29 07:07:51.000000 bayesian-models-0.1.2/pyproject.toml
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)       38 2023-04-29 07:08:35.565933 bayesian-models-0.1.2/setup.cfg
+drwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        0 2023-04-29 10:43:35.977339 bayesian-models-0.1.3/
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    11345 2023-04-29 07:04:58.000000 bayesian-models-0.1.3/LICENSE
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)       38 2023-02-20 09:01:11.000000 bayesian-models-0.1.3/MANIFEST.in
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     2759 2023-04-29 10:43:35.976972 bayesian-models-0.1.3/PKG-INFO
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     1787 2023-04-29 07:04:58.000000 bayesian-models-0.1.3/README.md
+drwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        0 2023-04-29 10:43:35.969655 bayesian-models-0.1.3/bayesian_models/
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        1 2023-04-29 07:04:58.000000 bayesian-models-0.1.3/bayesian_models/__init__.py
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    59828 2023-04-29 07:39:47.000000 bayesian-models-0.1.3/bayesian_models/core.py
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)   129623 2023-04-29 07:39:47.000000 bayesian-models-0.1.3/bayesian_models/data.py
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     3708 2023-04-29 07:04:58.000000 bayesian-models-0.1.3/bayesian_models/math.py
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    63346 2023-04-29 10:12:10.000000 bayesian-models-0.1.3/bayesian_models/models.py
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)      979 2023-04-29 07:39:47.000000 bayesian-models-0.1.3/bayesian_models/typing.py
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    29311 2023-04-29 07:39:47.000000 bayesian-models-0.1.3/bayesian_models/utilities.py
+drwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        0 2023-04-29 10:43:35.976055 bayesian-models-0.1.3/bayesian_models.egg-info/
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     2759 2023-04-29 10:43:35.000000 bayesian-models-0.1.3/bayesian_models.egg-info/PKG-INFO
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)      419 2023-04-29 10:43:35.000000 bayesian-models-0.1.3/bayesian_models.egg-info/SOURCES.txt
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        1 2023-04-29 10:43:35.000000 bayesian-models-0.1.3/bayesian_models.egg-info/dependency_links.txt
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)      123 2023-04-29 10:43:35.000000 bayesian-models-0.1.3/bayesian_models.egg-info/requires.txt
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)       16 2023-04-29 10:43:35.000000 bayesian-models-0.1.3/bayesian_models.egg-info/top_level.txt
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     1255 2023-04-29 10:42:46.000000 bayesian-models-0.1.3/pyproject.toml
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)       38 2023-04-29 10:43:35.977463 bayesian-models-0.1.3/setup.cfg
```

### Comparing `bayesian-models-0.1.2/LICENSE` & `bayesian-models-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.2/PKG-INFO` & `bayesian-models-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayesian-models
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for building common bayesian models in pymc
 Author-email: Alexander Rodis <alexanderrhodis@gmail.com>
 Maintainer-email: Alexander Rodis <alexanderrhodis@gmail.com>
 Project-URL: Homepage, https://github.com/AlexRodis/bayesian_models
 Project-URL: Bug Tracker, https://github.com/AlexRodis/bayesian_models/issues
 Project-URL: Documentation, https://bayesian-models.readthedocs.io/en/latest/
 Keywords: bayesian,models,statistics,pymc
```

### Comparing `bayesian-models-0.1.2/README.md` & `bayesian-models-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.2/bayesian_models/core.py` & `bayesian-models-0.1.3/bayesian_models/core.py`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.2/bayesian_models/data.py` & `bayesian-models-0.1.3/bayesian_models/data.py`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.2/bayesian_models/math.py` & `bayesian-models-0.1.3/bayesian_models/math.py`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.2/bayesian_models/models.py` & `bayesian-models-0.1.3/bayesian_models/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1401,18 +1401,19 @@
                     floats defining the probability threshold for the
                     credible interval. Is applied to all features for
                     each variable in :code:`var_names`
 
                 - | multilevel_on:str='[' := A separator defining the
                     multilevel index. :code:`pymc` by default
                     concatinates the label according to the form:
-                    {var_name}[{feature_label}]. The argument will
-                    reindex them in a multilevel fashion of the form
-                    (var_name, feature_label) in the resulting
-                    dataframe. Set to None to disable this behavior.
+                    :code:`{var_name}[{feature_label}]`. The argument
+                    will reindex them in a multilevel fashion of the
+                    form :code:`(var_name, feature_label)` in the
+                    resulting dataframe. Set to None to disable this
+                    behavior.
 
                 - | extend_summary:bool=True := If True the new
                     Significance column extends the summary dataframe.
                     Else return a new  dataframe containing only the
                     Significance results. Optional. Defaults to True and
                     returns an extended version of the summary.
                     
@@ -1450,22 +1451,22 @@
         if not all(
             (len(var_names) != len(ropes), len(ropes)!=len(hdis))
             ):
             from warnings import warn
             warn(("Length of variables, ropes and hdis not equal. The"
                   " shortest value will be considered"))
         results=dict()
-        null_interval = interval(0,0)
+        null_interval = interval()
         for var_name, rope,hdi in zip(var_names,ropes, hdis):
             raw_summary = az.summary(self.idata, var_names=[var_name],
             filter_vars='like', hdi_prob=hdi)
-            rope=interval(*rope)
+            rope=interval(rope)
             out=[]
             for idx,row in raw_summary.iterrows():
-                ci=interval(row[2], row[3])
+                ci=interval([row[2], row[3]])
                 if ci in rope:
                     out.append("Not Significant")
                 elif ci & rope != null_interval:
                     out.append("Indeterminate")
                 else:
                     out.append("Significant")
             significance = pd.DataFrame(data=np.asarray(out),
```

### Comparing `bayesian-models-0.1.2/bayesian_models/typing.py` & `bayesian-models-0.1.3/bayesian_models/typing.py`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.2/bayesian_models/utilities.py` & `bayesian-models-0.1.3/bayesian_models/utilities.py`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.2/bayesian_models.egg-info/PKG-INFO` & `bayesian-models-0.1.3/bayesian_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayesian-models
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for building common bayesian models in pymc
 Author-email: Alexander Rodis <alexanderrhodis@gmail.com>
 Maintainer-email: Alexander Rodis <alexanderrhodis@gmail.com>
 Project-URL: Homepage, https://github.com/AlexRodis/bayesian_models
 Project-URL: Bug Tracker, https://github.com/AlexRodis/bayesian_models/issues
 Project-URL: Documentation, https://bayesian-models.readthedocs.io/en/latest/
 Keywords: bayesian,models,statistics,pymc
```

### Comparing `bayesian-models-0.1.2/pyproject.toml` & `bayesian-models-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "bayesian-models"
 
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Alexander Rodis", email="alexanderrhodis@gmail.com" },
 ]
 
 maintainers = [
     { name="Alexander Rodis", email="alexanderrhodis@gmail.com" },
 ]
```


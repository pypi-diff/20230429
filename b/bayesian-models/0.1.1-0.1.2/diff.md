# Comparing `tmp/bayesian-models-0.1.1.tar.gz` & `tmp/bayesian-models-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesian-models-0.1.1.tar", last modified: Sat Apr 29 06:54:36 2023, max compression
+gzip compressed data, was "bayesian-models-0.1.2.tar", last modified: Sat Apr 29 07:08:35 2023, max compression
```

## Comparing `bayesian-models-0.1.1.tar` & `bayesian-models-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        0 2023-04-29 06:54:36.866457 bayesian-models-0.1.1/
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    11345 2023-04-05 10:48:24.000000 bayesian-models-0.1.1/LICENSE
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)       38 2023-02-20 09:01:11.000000 bayesian-models-0.1.1/MANIFEST.in
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     2759 2023-04-29 06:54:36.866064 bayesian-models-0.1.1/PKG-INFO
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     1787 2023-04-05 10:48:24.000000 bayesian-models-0.1.1/README.md
-drwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        0 2023-04-29 06:54:36.860743 bayesian-models-0.1.1/bayesian_models/
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        1 2023-04-05 10:48:24.000000 bayesian-models-0.1.1/bayesian_models/__init__.py
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    59828 2023-04-29 06:49:27.000000 bayesian-models-0.1.1/bayesian_models/core.py
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)   129623 2023-04-29 06:49:27.000000 bayesian-models-0.1.1/bayesian_models/data.py
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     3708 2023-04-05 10:48:24.000000 bayesian-models-0.1.1/bayesian_models/math.py
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    63312 2023-04-29 06:53:57.000000 bayesian-models-0.1.1/bayesian_models/models.py
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)      979 2023-04-29 06:49:27.000000 bayesian-models-0.1.1/bayesian_models/typing.py
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     4831 2023-04-29 06:49:27.000000 bayesian-models-0.1.1/bayesian_models/utilities.py
-drwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        0 2023-04-29 06:54:36.865160 bayesian-models-0.1.1/bayesian_models.egg-info/
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     2759 2023-04-29 06:54:36.000000 bayesian-models-0.1.1/bayesian_models.egg-info/PKG-INFO
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)      419 2023-04-29 06:54:36.000000 bayesian-models-0.1.1/bayesian_models.egg-info/SOURCES.txt
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        1 2023-04-29 06:54:36.000000 bayesian-models-0.1.1/bayesian_models.egg-info/dependency_links.txt
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)      123 2023-04-29 06:54:36.000000 bayesian-models-0.1.1/bayesian_models.egg-info/requires.txt
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)       16 2023-04-29 06:54:36.000000 bayesian-models-0.1.1/bayesian_models.egg-info/top_level.txt
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     1255 2023-04-29 06:49:27.000000 bayesian-models-0.1.1/pyproject.toml
--rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)       38 2023-04-29 06:54:36.866590 bayesian-models-0.1.1/setup.cfg
+drwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        0 2023-04-29 07:08:35.565791 bayesian-models-0.1.2/
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    11345 2023-04-29 07:04:58.000000 bayesian-models-0.1.2/LICENSE
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)       38 2023-02-20 09:01:11.000000 bayesian-models-0.1.2/MANIFEST.in
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     2759 2023-04-29 07:08:35.565295 bayesian-models-0.1.2/PKG-INFO
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     1787 2023-04-29 07:04:58.000000 bayesian-models-0.1.2/README.md
+drwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        0 2023-04-29 07:08:35.559721 bayesian-models-0.1.2/bayesian_models/
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        1 2023-04-29 07:04:58.000000 bayesian-models-0.1.2/bayesian_models/__init__.py
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    59828 2023-04-29 07:04:58.000000 bayesian-models-0.1.2/bayesian_models/core.py
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)   129623 2023-04-29 07:04:58.000000 bayesian-models-0.1.2/bayesian_models/data.py
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     3708 2023-04-29 07:04:58.000000 bayesian-models-0.1.2/bayesian_models/math.py
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    63312 2023-04-29 07:04:58.000000 bayesian-models-0.1.2/bayesian_models/models.py
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)      979 2023-04-29 07:04:58.000000 bayesian-models-0.1.2/bayesian_models/typing.py
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)    29311 2023-04-29 07:06:28.000000 bayesian-models-0.1.2/bayesian_models/utilities.py
+drwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        0 2023-04-29 07:08:35.564357 bayesian-models-0.1.2/bayesian_models.egg-info/
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     2759 2023-04-29 07:08:35.000000 bayesian-models-0.1.2/bayesian_models.egg-info/PKG-INFO
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)      419 2023-04-29 07:08:35.000000 bayesian-models-0.1.2/bayesian_models.egg-info/SOURCES.txt
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)        1 2023-04-29 07:08:35.000000 bayesian-models-0.1.2/bayesian_models.egg-info/dependency_links.txt
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)      123 2023-04-29 07:08:35.000000 bayesian-models-0.1.2/bayesian_models.egg-info/requires.txt
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)       16 2023-04-29 07:08:35.000000 bayesian-models-0.1.2/bayesian_models.egg-info/top_level.txt
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)     1255 2023-04-29 07:07:51.000000 bayesian-models-0.1.2/pyproject.toml
+-rwxrwxrwx   0 alexander-fyrogenis  (1000) alexander-fyrogenis  (1000)       38 2023-04-29 07:08:35.565933 bayesian-models-0.1.2/setup.cfg
```

### Comparing `bayesian-models-0.1.1/LICENSE` & `bayesian-models-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.1/PKG-INFO` & `bayesian-models-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayesian-models
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for building common bayesian models in pymc
 Author-email: Alexander Rodis <alexanderrhodis@gmail.com>
 Maintainer-email: Alexander Rodis <alexanderrhodis@gmail.com>
 Project-URL: Homepage, https://github.com/AlexRodis/bayesian_models
 Project-URL: Bug Tracker, https://github.com/AlexRodis/bayesian_models/issues
 Project-URL: Documentation, https://bayesian-models.readthedocs.io/en/latest/
 Keywords: bayesian,models,statistics,pymc
```

### Comparing `bayesian-models-0.1.1/README.md` & `bayesian-models-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.1/bayesian_models/core.py` & `bayesian-models-0.1.2/bayesian_models/core.py`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.1/bayesian_models/data.py` & `bayesian-models-0.1.2/bayesian_models/data.py`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.1/bayesian_models/math.py` & `bayesian-models-0.1.2/bayesian_models/math.py`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.1/bayesian_models/models.py` & `bayesian-models-0.1.2/bayesian_models/models.py`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.1/bayesian_models/typing.py` & `bayesian-models-0.1.2/bayesian_models/typing.py`

 * *Files identical despite different names*

### Comparing `bayesian-models-0.1.1/bayesian_models.egg-info/PKG-INFO` & `bayesian-models-0.1.2/bayesian_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayesian-models
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for building common bayesian models in pymc
 Author-email: Alexander Rodis <alexanderrhodis@gmail.com>
 Maintainer-email: Alexander Rodis <alexanderrhodis@gmail.com>
 Project-URL: Homepage, https://github.com/AlexRodis/bayesian_models
 Project-URL: Bug Tracker, https://github.com/AlexRodis/bayesian_models/issues
 Project-URL: Documentation, https://bayesian-models.readthedocs.io/en/latest/
 Keywords: bayesian,models,statistics,pymc
```

### Comparing `bayesian-models-0.1.1/pyproject.toml` & `bayesian-models-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "bayesian-models"
 
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Alexander Rodis", email="alexanderrhodis@gmail.com" },
 ]
 
 maintainers = [
     { name="Alexander Rodis", email="alexanderrhodis@gmail.com" },
 ]
```


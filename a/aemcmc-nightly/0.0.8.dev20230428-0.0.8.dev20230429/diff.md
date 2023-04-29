# Comparing `tmp/aemcmc-nightly-0.0.8.dev20230428.tar.gz` & `tmp/aemcmc-nightly-0.0.8.dev20230429.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aemcmc-nightly-0.0.8.dev20230428.tar", last modified: Fri Apr 28 00:59:27 2023, max compression
+gzip compressed data, was "aemcmc-nightly-0.0.8.dev20230429.tar", last modified: Sat Apr 29 00:56:18 2023, max compression
```

## Comparing `aemcmc-nightly-0.0.8.dev20230428.tar` & `aemcmc-nightly-0.0.8.dev20230429.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:59:27.112957 aemcmc-nightly-0.0.8.dev20230428/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-28 00:59:27.112957 aemcmc-nightly-0.0.8.dev20230428/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:59:27.116957 aemcmc-nightly-0.0.8.dev20230428/aemcmc/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/aemcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 00:59:27.116957 aemcmc-nightly-0.0.8.dev20230428/aemcmc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/aemcmc/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/aemcmc/conjugates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/aemcmc/dists.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/aemcmc/ffbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24238 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/aemcmc/gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/aemcmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/aemcmc/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/aemcmc/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/aemcmc/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/aemcmc/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/aemcmc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:59:27.112957 aemcmc-nightly-0.0.8.dev20230428/aemcmc_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-28 00:59:27.000000 aemcmc-nightly-0.0.8.dev20230428/aemcmc_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-28 00:59:27.000000 aemcmc-nightly-0.0.8.dev20230428/aemcmc_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:59:27.000000 aemcmc-nightly-0.0.8.dev20230428/aemcmc_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:59:26.000000 aemcmc-nightly-0.0.8.dev20230428/aemcmc_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-28 00:59:27.000000 aemcmc-nightly-0.0.8.dev20230428/aemcmc_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 00:59:27.000000 aemcmc-nightly-0.0.8.dev20230428/aemcmc_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-28 00:59:27.116957 aemcmc-nightly-0.0.8.dev20230428/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:59:27.112957 aemcmc-nightly-0.0.8.dev20230428/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/tests/test_conjugates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/tests/test_dists.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/tests/test_ffbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/tests/test_gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/tests/test_nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/tests/test_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-04-28 00:59:12.000000 aemcmc-nightly-0.0.8.dev20230428/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:56:18.435619 aemcmc-nightly-0.0.8.dev20230429/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-29 00:56:18.435619 aemcmc-nightly-0.0.8.dev20230429/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:56:18.435619 aemcmc-nightly-0.0.8.dev20230429/aemcmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/aemcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-29 00:56:18.435619 aemcmc-nightly-0.0.8.dev20230429/aemcmc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/aemcmc/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/aemcmc/conjugates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/aemcmc/dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/aemcmc/ffbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24238 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/aemcmc/gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/aemcmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/aemcmc/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/aemcmc/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/aemcmc/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/aemcmc/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/aemcmc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:56:18.435619 aemcmc-nightly-0.0.8.dev20230429/aemcmc_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-29 00:56:18.000000 aemcmc-nightly-0.0.8.dev20230429/aemcmc_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-29 00:56:18.000000 aemcmc-nightly-0.0.8.dev20230429/aemcmc_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:56:18.000000 aemcmc-nightly-0.0.8.dev20230429/aemcmc_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:56:18.000000 aemcmc-nightly-0.0.8.dev20230429/aemcmc_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-29 00:56:18.000000 aemcmc-nightly-0.0.8.dev20230429/aemcmc_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 00:56:18.000000 aemcmc-nightly-0.0.8.dev20230429/aemcmc_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-29 00:56:18.435619 aemcmc-nightly-0.0.8.dev20230429/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:56:18.435619 aemcmc-nightly-0.0.8.dev20230429/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/tests/test_conjugates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/tests/test_dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/tests/test_ffbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/tests/test_gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/tests/test_nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/tests/test_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-04-29 00:56:07.000000 aemcmc-nightly-0.0.8.dev20230429/versioneer.py
```

### Comparing `aemcmc-nightly-0.0.8.dev20230428/LICENSE` & `aemcmc-nightly-0.0.8.dev20230429/LICENSE`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/PKG-INFO` & `aemcmc-nightly-0.0.8.dev20230429/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aemcmc-nightly
-Version: 0.0.8.dev20230428
+Version: 0.0.8.dev20230429
 Summary: Miscellaneous MCMC samplers written in Aesara
 Home-page: http://github.com/aesara-devs/aemcmc
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: math,probability,numerical,symbolic,MCMC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aemcmc-nightly-0.0.8.dev20230428/README.md` & `aemcmc-nightly-0.0.8.dev20230429/README.md`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/aemcmc/basic.py` & `aemcmc-nightly-0.0.8.dev20230429/aemcmc/basic.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/aemcmc/conjugates.py` & `aemcmc-nightly-0.0.8.dev20230429/aemcmc/conjugates.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/aemcmc/dists.py` & `aemcmc-nightly-0.0.8.dev20230429/aemcmc/dists.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/aemcmc/ffbs.py` & `aemcmc-nightly-0.0.8.dev20230429/aemcmc/ffbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/aemcmc/gibbs.py` & `aemcmc-nightly-0.0.8.dev20230429/aemcmc/gibbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/aemcmc/nuts.py` & `aemcmc-nightly-0.0.8.dev20230429/aemcmc/nuts.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/aemcmc/rewriting.py` & `aemcmc-nightly-0.0.8.dev20230429/aemcmc/rewriting.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/aemcmc/sample.py` & `aemcmc-nightly-0.0.8.dev20230429/aemcmc/sample.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/aemcmc/transforms.py` & `aemcmc-nightly-0.0.8.dev20230429/aemcmc/transforms.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/aemcmc/types.py` & `aemcmc-nightly-0.0.8.dev20230429/aemcmc/types.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/aemcmc/utils.py` & `aemcmc-nightly-0.0.8.dev20230429/aemcmc/utils.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/aemcmc_nightly.egg-info/PKG-INFO` & `aemcmc-nightly-0.0.8.dev20230429/aemcmc_nightly.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aemcmc-nightly
-Version: 0.0.8.dev20230428
+Version: 0.0.8.dev20230429
 Summary: Miscellaneous MCMC samplers written in Aesara
 Home-page: http://github.com/aesara-devs/aemcmc
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: math,probability,numerical,symbolic,MCMC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aemcmc-nightly-0.0.8.dev20230428/aemcmc_nightly.egg-info/SOURCES.txt` & `aemcmc-nightly-0.0.8.dev20230429/aemcmc_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/setup.cfg` & `aemcmc-nightly-0.0.8.dev20230429/setup.cfg`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/setup.py` & `aemcmc-nightly-0.0.8.dev20230429/setup.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/tests/test_basic.py` & `aemcmc-nightly-0.0.8.dev20230429/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/tests/test_conjugates.py` & `aemcmc-nightly-0.0.8.dev20230429/tests/test_conjugates.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/tests/test_dists.py` & `aemcmc-nightly-0.0.8.dev20230429/tests/test_dists.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/tests/test_ffbs.py` & `aemcmc-nightly-0.0.8.dev20230429/tests/test_ffbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/tests/test_gibbs.py` & `aemcmc-nightly-0.0.8.dev20230429/tests/test_gibbs.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/tests/test_nuts.py` & `aemcmc-nightly-0.0.8.dev20230429/tests/test_nuts.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/tests/test_rewriting.py` & `aemcmc-nightly-0.0.8.dev20230429/tests/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/tests/test_sample.py` & `aemcmc-nightly-0.0.8.dev20230429/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/tests/test_transforms.py` & `aemcmc-nightly-0.0.8.dev20230429/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/tests/test_utils.py` & `aemcmc-nightly-0.0.8.dev20230429/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aemcmc-nightly-0.0.8.dev20230428/versioneer.py` & `aemcmc-nightly-0.0.8.dev20230429/versioneer.py`

 * *Files identical despite different names*


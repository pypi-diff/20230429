# Comparing `tmp/alethiometer-1.0.8.tar.gz` & `tmp/alethiometer-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alethiometer-1.0.8.tar", last modified: Fri Apr 28 22:21:56 2023, max compression
+gzip compressed data, was "alethiometer-1.0.9.tar", last modified: Fri Apr 28 22:29:29 2023, max compression
```

## Comparing `alethiometer-1.0.8.tar` & `alethiometer-1.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:21:56.112996 alethiometer-1.0.8/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    11357 2023-04-07 16:49:02.000000 alethiometer-1.0.8/LICENSE
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6663 2023-04-28 22:21:56.112996 alethiometer-1.0.8/PKG-INFO
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5953 2023-04-28 22:00:25.000000 alethiometer-1.0.8/README.md
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:21:56.108996 alethiometer-1.0.8/alethiometer/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      313 2023-04-11 12:10:43.000000 alethiometer-1.0.8/alethiometer/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      245 2023-04-28 22:20:39.000000 alethiometer-1.0.8/alethiometer/__version__.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:21:56.108996 alethiometer-1.0.8/alethiometer/datasets/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      254 2023-04-07 17:54:55.000000 alethiometer-1.0.8/alethiometer/datasets/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4853 2023-04-17 13:10:20.000000 alethiometer-1.0.8/alethiometer/datasets/dataset.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2174 2023-04-07 17:54:22.000000 alethiometer-1.0.8/alethiometer/datasets/h5py_dataset.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5109 2023-04-07 17:55:28.000000 alethiometer-1.0.8/alethiometer/datasets/imagenet16.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1077 2023-04-07 15:01:32.000000 alethiometer-1.0.8/alethiometer/utils.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4968 2023-04-28 22:17:58.000000 alethiometer-1.0.8/alethiometer/zc_proxy.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:21:56.108996 alethiometer-1.0.8/alethiometer/zero_cost_metrics/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1660 2023-04-28 21:23:03.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1475 2023-04-07 17:10:09.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/grad_norm.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3624 2023-04-07 17:13:08.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/grasp.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2926 2023-04-11 16:57:48.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/naswot.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2079 2023-04-28 20:46:05.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/naswot_relu.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2023 2023-04-07 17:09:49.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/snip.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1928 2023-04-07 17:06:05.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/synflow.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    15593 2023-04-28 22:16:08.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/tenas.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3420 2023-04-28 21:42:23.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/zen.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2412 2023-04-23 12:05:26.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/zico.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:21:56.108996 alethiometer-1.0.8/alethiometer.egg-info/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6663 2023-04-28 22:21:56.000000 alethiometer-1.0.8/alethiometer.egg-info/PKG-INFO
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      898 2023-04-28 22:21:56.000000 alethiometer-1.0.8/alethiometer.egg-info/SOURCES.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)        1 2023-04-28 22:21:56.000000 alethiometer-1.0.8/alethiometer.egg-info/dependency_links.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       37 2023-04-28 22:21:56.000000 alethiometer-1.0.8/alethiometer.egg-info/requires.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       13 2023-04-28 22:21:56.000000 alethiometer-1.0.8/alethiometer.egg-info/top_level.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       38 2023-04-28 22:21:56.112996 alethiometer-1.0.8/setup.cfg
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6031 2023-04-07 18:04:03.000000 alethiometer-1.0.8/setup.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:21:56.108996 alethiometer-1.0.8/tests/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1219 2023-04-25 09:05:55.000000 alethiometer-1.0.8/tests/test_nwot_api.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3098 2023-04-28 22:20:47.000000 alethiometer-1.0.8/tests/test_zc.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:29:29.938750 alethiometer-1.0.9/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    11357 2023-04-07 16:49:02.000000 alethiometer-1.0.9/LICENSE
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     7068 2023-04-28 22:29:29.934750 alethiometer-1.0.9/PKG-INFO
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6358 2023-04-28 22:29:04.000000 alethiometer-1.0.9/README.md
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:29:29.934750 alethiometer-1.0.9/alethiometer/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      313 2023-04-11 12:10:43.000000 alethiometer-1.0.9/alethiometer/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      245 2023-04-28 22:28:17.000000 alethiometer-1.0.9/alethiometer/__version__.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:29:29.934750 alethiometer-1.0.9/alethiometer/datasets/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      254 2023-04-07 17:54:55.000000 alethiometer-1.0.9/alethiometer/datasets/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4853 2023-04-17 13:10:20.000000 alethiometer-1.0.9/alethiometer/datasets/dataset.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2174 2023-04-07 17:54:22.000000 alethiometer-1.0.9/alethiometer/datasets/h5py_dataset.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5109 2023-04-07 17:55:28.000000 alethiometer-1.0.9/alethiometer/datasets/imagenet16.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1077 2023-04-07 15:01:32.000000 alethiometer-1.0.9/alethiometer/utils.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4968 2023-04-28 22:17:58.000000 alethiometer-1.0.9/alethiometer/zc_proxy.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:29:29.934750 alethiometer-1.0.9/alethiometer/zero_cost_metrics/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1660 2023-04-28 21:23:03.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1475 2023-04-07 17:10:09.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/grad_norm.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3624 2023-04-07 17:13:08.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/grasp.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2926 2023-04-11 16:57:48.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/naswot.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2079 2023-04-28 20:46:05.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/naswot_relu.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2023 2023-04-07 17:09:49.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/snip.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1928 2023-04-07 17:06:05.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/synflow.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    15593 2023-04-28 22:16:08.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/tenas.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3420 2023-04-28 21:42:23.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/zen.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2412 2023-04-23 12:05:26.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/zico.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:29:29.934750 alethiometer-1.0.9/alethiometer.egg-info/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     7068 2023-04-28 22:29:29.000000 alethiometer-1.0.9/alethiometer.egg-info/PKG-INFO
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      898 2023-04-28 22:29:29.000000 alethiometer-1.0.9/alethiometer.egg-info/SOURCES.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)        1 2023-04-28 22:29:29.000000 alethiometer-1.0.9/alethiometer.egg-info/dependency_links.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       37 2023-04-28 22:29:29.000000 alethiometer-1.0.9/alethiometer.egg-info/requires.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       13 2023-04-28 22:29:29.000000 alethiometer-1.0.9/alethiometer.egg-info/top_level.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       38 2023-04-28 22:29:29.938750 alethiometer-1.0.9/setup.cfg
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6031 2023-04-07 18:04:03.000000 alethiometer-1.0.9/setup.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:29:29.934750 alethiometer-1.0.9/tests/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1219 2023-04-25 09:05:55.000000 alethiometer-1.0.9/tests/test_nwot_api.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3098 2023-04-28 22:20:47.000000 alethiometer-1.0.9/tests/test_zc.py
```

### Comparing `alethiometer-1.0.8/LICENSE` & `alethiometer-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/PKG-INFO` & `alethiometer-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alethiometer
-Version: 1.0.8
+Version: 1.0.9
 Summary: ZC proxies calculation repo, altered from foresight package.
 Home-page: https://github.com/iViolinSolo/zero-cost-proxies
 Author: ViolinSolo
 Author-email: i.violinsolo@gmail.com
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <!--
  * @Author: ViolinSolo
  * @Date: 2023-03-26 10:11:01
- * @LastEditTime: 2023-04-28 22:59:20
+ * @LastEditTime: 2023-04-28 23:29:03
  * @LastEditors: ViolinSolo
  * @Description: Readme
  * @FilePath: /zero-cost-proxies/README.md
 -->
 # zero-cost-proxies
 Independent ZC proxies only for testing on it. 
 
@@ -52,31 +52,39 @@
 =-------------------------------------------------------=
 = zen,                                                  =
 =      Your network need have attribute fn:             =
 =         `forward_before_global_avg_pool(inputs)`      =
 =      to calculate zenas score                         =
 =      (see sample code in tests/test_zc.py)            =
 =-------------------------------------------------------=
+= tenas,                                                =
+=      must work in `gpu` env,                          =
+=      might encouter bug on `cpu`.                     =
+=      also contains metrics:                           =
+= ntk,                                                  =
+= lrn,                                                  = 
 =========================================================
 ```
 
 
 ## 1. Tests
 ImageNet16-120 cannot be automatically downloaded. Using script under `scripts/download_data.sh` to download:
 ```bash
 source scripts/download_data.sh nb201 ImageNet16-120
 # do not use `bash`, use `source` instead
 ```
 ## 2. Versions
-- V1.0.8
-fix bug in `nwot_relu` for wrong for/backward fn register,
-fix bug in `zen` for missed necessary attribute check, add test sample for `zen` metric,
-fix bug in `zen` for return value have not .item() attribute,
+- V1.0.9  
+fix readme format, no code change.
+- V1.0.8  
+fix bug in `nwot_relu` for wrong for/backward fn register,  
+fix bug in `zen` for missed necessary attribute check, add test sample for `zen` metric,  
+fix bug in `zen` for return value have not .item() attribute,  
 add `tenas` metric, which calculates TE-NAS score. (`tenas`, `ntk`, `lrn`)
-- V1.0.7
+- V1.0.7  
 add `zen` metric, which calculates ZenNAS score.
 - V1.0.6  
 add original `naswot` implements based on RELU, can be calculated using metirc `nwot_relu`, also fix potential oom bug, and more reliable GPU memory cache removal code snippets.  
 - V1.0.5  
 add `naswot, lnwot` into mats
 - V1.0.4  
 fix bugs in calculation, add more test codes.
```

### Comparing `alethiometer-1.0.8/README.md` & `alethiometer-1.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!--
  * @Author: ViolinSolo
  * @Date: 2023-03-26 10:11:01
- * @LastEditTime: 2023-04-28 22:59:20
+ * @LastEditTime: 2023-04-28 23:29:03
  * @LastEditors: ViolinSolo
  * @Description: Readme
  * @FilePath: /zero-cost-proxies/README.md
 -->
 # zero-cost-proxies
 Independent ZC proxies only for testing on it. 
 
@@ -33,31 +33,39 @@
 =-------------------------------------------------------=
 = zen,                                                  =
 =      Your network need have attribute fn:             =
 =         `forward_before_global_avg_pool(inputs)`      =
 =      to calculate zenas score                         =
 =      (see sample code in tests/test_zc.py)            =
 =-------------------------------------------------------=
+= tenas,                                                =
+=      must work in `gpu` env,                          =
+=      might encouter bug on `cpu`.                     =
+=      also contains metrics:                           =
+= ntk,                                                  =
+= lrn,                                                  = 
 =========================================================
 ```
 
 
 ## 1. Tests
 ImageNet16-120 cannot be automatically downloaded. Using script under `scripts/download_data.sh` to download:
 ```bash
 source scripts/download_data.sh nb201 ImageNet16-120
 # do not use `bash`, use `source` instead
 ```
 ## 2. Versions
-- V1.0.8
-fix bug in `nwot_relu` for wrong for/backward fn register,
-fix bug in `zen` for missed necessary attribute check, add test sample for `zen` metric,
-fix bug in `zen` for return value have not .item() attribute,
+- V1.0.9  
+fix readme format, no code change.
+- V1.0.8  
+fix bug in `nwot_relu` for wrong for/backward fn register,  
+fix bug in `zen` for missed necessary attribute check, add test sample for `zen` metric,  
+fix bug in `zen` for return value have not .item() attribute,  
 add `tenas` metric, which calculates TE-NAS score. (`tenas`, `ntk`, `lrn`)
-- V1.0.7
+- V1.0.7  
 add `zen` metric, which calculates ZenNAS score.
 - V1.0.6  
 add original `naswot` implements based on RELU, can be calculated using metirc `nwot_relu`, also fix potential oom bug, and more reliable GPU memory cache removal code snippets.  
 - V1.0.5  
 add `naswot, lnwot` into mats
 - V1.0.4  
 fix bugs in calculation, add more test codes.
```

### Comparing `alethiometer-1.0.8/alethiometer/datasets/dataset.py` & `alethiometer-1.0.9/alethiometer/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/alethiometer/datasets/h5py_dataset.py` & `alethiometer-1.0.9/alethiometer/datasets/h5py_dataset.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/alethiometer/datasets/imagenet16.py` & `alethiometer-1.0.9/alethiometer/datasets/imagenet16.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/alethiometer/utils.py` & `alethiometer-1.0.9/alethiometer/utils.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/alethiometer/zc_proxy.py` & `alethiometer-1.0.9/alethiometer/zc_proxy.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/alethiometer/zero_cost_metrics/__init__.py` & `alethiometer-1.0.9/alethiometer/zero_cost_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/alethiometer/zero_cost_metrics/grad_norm.py` & `alethiometer-1.0.9/alethiometer/zero_cost_metrics/grad_norm.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/alethiometer/zero_cost_metrics/grasp.py` & `alethiometer-1.0.9/alethiometer/zero_cost_metrics/grasp.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/alethiometer/zero_cost_metrics/naswot.py` & `alethiometer-1.0.9/alethiometer/zero_cost_metrics/naswot.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/alethiometer/zero_cost_metrics/naswot_relu.py` & `alethiometer-1.0.9/alethiometer/zero_cost_metrics/naswot_relu.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/alethiometer/zero_cost_metrics/snip.py` & `alethiometer-1.0.9/alethiometer/zero_cost_metrics/snip.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/alethiometer/zero_cost_metrics/synflow.py` & `alethiometer-1.0.9/alethiometer/zero_cost_metrics/synflow.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/alethiometer/zero_cost_metrics/tenas.py` & `alethiometer-1.0.9/alethiometer/zero_cost_metrics/tenas.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/alethiometer/zero_cost_metrics/zen.py` & `alethiometer-1.0.9/alethiometer/zero_cost_metrics/zen.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/alethiometer/zero_cost_metrics/zico.py` & `alethiometer-1.0.9/alethiometer/zero_cost_metrics/zico.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/alethiometer.egg-info/PKG-INFO` & `alethiometer-1.0.9/alethiometer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alethiometer
-Version: 1.0.8
+Version: 1.0.9
 Summary: ZC proxies calculation repo, altered from foresight package.
 Home-page: https://github.com/iViolinSolo/zero-cost-proxies
 Author: ViolinSolo
 Author-email: i.violinsolo@gmail.com
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <!--
  * @Author: ViolinSolo
  * @Date: 2023-03-26 10:11:01
- * @LastEditTime: 2023-04-28 22:59:20
+ * @LastEditTime: 2023-04-28 23:29:03
  * @LastEditors: ViolinSolo
  * @Description: Readme
  * @FilePath: /zero-cost-proxies/README.md
 -->
 # zero-cost-proxies
 Independent ZC proxies only for testing on it. 
 
@@ -52,31 +52,39 @@
 =-------------------------------------------------------=
 = zen,                                                  =
 =      Your network need have attribute fn:             =
 =         `forward_before_global_avg_pool(inputs)`      =
 =      to calculate zenas score                         =
 =      (see sample code in tests/test_zc.py)            =
 =-------------------------------------------------------=
+= tenas,                                                =
+=      must work in `gpu` env,                          =
+=      might encouter bug on `cpu`.                     =
+=      also contains metrics:                           =
+= ntk,                                                  =
+= lrn,                                                  = 
 =========================================================
 ```
 
 
 ## 1. Tests
 ImageNet16-120 cannot be automatically downloaded. Using script under `scripts/download_data.sh` to download:
 ```bash
 source scripts/download_data.sh nb201 ImageNet16-120
 # do not use `bash`, use `source` instead
 ```
 ## 2. Versions
-- V1.0.8
-fix bug in `nwot_relu` for wrong for/backward fn register,
-fix bug in `zen` for missed necessary attribute check, add test sample for `zen` metric,
-fix bug in `zen` for return value have not .item() attribute,
+- V1.0.9  
+fix readme format, no code change.
+- V1.0.8  
+fix bug in `nwot_relu` for wrong for/backward fn register,  
+fix bug in `zen` for missed necessary attribute check, add test sample for `zen` metric,  
+fix bug in `zen` for return value have not .item() attribute,  
 add `tenas` metric, which calculates TE-NAS score. (`tenas`, `ntk`, `lrn`)
-- V1.0.7
+- V1.0.7  
 add `zen` metric, which calculates ZenNAS score.
 - V1.0.6  
 add original `naswot` implements based on RELU, can be calculated using metirc `nwot_relu`, also fix potential oom bug, and more reliable GPU memory cache removal code snippets.  
 - V1.0.5  
 add `naswot, lnwot` into mats
 - V1.0.4  
 fix bugs in calculation, add more test codes.
```

### Comparing `alethiometer-1.0.8/alethiometer.egg-info/SOURCES.txt` & `alethiometer-1.0.9/alethiometer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/setup.py` & `alethiometer-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/tests/test_nwot_api.py` & `alethiometer-1.0.9/tests/test_nwot_api.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.8/tests/test_zc.py` & `alethiometer-1.0.9/tests/test_zc.py`

 * *Files identical despite different names*


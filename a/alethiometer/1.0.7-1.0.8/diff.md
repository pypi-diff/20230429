# Comparing `tmp/alethiometer-1.0.7.tar.gz` & `tmp/alethiometer-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alethiometer-1.0.7.tar", last modified: Fri Apr 28 16:12:53 2023, max compression
+gzip compressed data, was "alethiometer-1.0.8.tar", last modified: Fri Apr 28 22:21:56 2023, max compression
```

## Comparing `alethiometer-1.0.7.tar` & `alethiometer-1.0.8.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 16:12:53.177044 alethiometer-1.0.7/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    11357 2023-04-07 16:49:02.000000 alethiometer-1.0.7/LICENSE
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2995 2023-04-28 16:12:53.177044 alethiometer-1.0.7/PKG-INFO
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2286 2023-04-28 16:12:01.000000 alethiometer-1.0.7/README.md
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 16:12:53.173044 alethiometer-1.0.7/alethiometer/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      313 2023-04-11 12:10:43.000000 alethiometer-1.0.7/alethiometer/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      245 2023-04-28 16:08:33.000000 alethiometer-1.0.7/alethiometer/__version__.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 16:12:53.173044 alethiometer-1.0.7/alethiometer/datasets/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      254 2023-04-07 17:54:55.000000 alethiometer-1.0.7/alethiometer/datasets/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4853 2023-04-17 13:10:20.000000 alethiometer-1.0.7/alethiometer/datasets/dataset.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2174 2023-04-07 17:54:22.000000 alethiometer-1.0.7/alethiometer/datasets/h5py_dataset.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5109 2023-04-07 17:55:28.000000 alethiometer-1.0.7/alethiometer/datasets/imagenet16.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1077 2023-04-07 15:01:32.000000 alethiometer-1.0.7/alethiometer/utils.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4676 2023-04-28 16:07:32.000000 alethiometer-1.0.7/alethiometer/zc_proxy.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 16:12:53.177044 alethiometer-1.0.7/alethiometer/zero_cost_metrics/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1582 2023-04-28 16:06:51.000000 alethiometer-1.0.7/alethiometer/zero_cost_metrics/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1475 2023-04-07 17:10:09.000000 alethiometer-1.0.7/alethiometer/zero_cost_metrics/grad_norm.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3624 2023-04-07 17:13:08.000000 alethiometer-1.0.7/alethiometer/zero_cost_metrics/grasp.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2926 2023-04-11 16:57:48.000000 alethiometer-1.0.7/alethiometer/zero_cost_metrics/naswot.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2025 2023-04-28 13:53:18.000000 alethiometer-1.0.7/alethiometer/zero_cost_metrics/naswot_relu.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4991 2023-04-24 09:28:34.000000 alethiometer-1.0.7/alethiometer/zero_cost_metrics/ntk.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2023 2023-04-07 17:09:49.000000 alethiometer-1.0.7/alethiometer/zero_cost_metrics/snip.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1928 2023-04-07 17:06:05.000000 alethiometer-1.0.7/alethiometer/zero_cost_metrics/synflow.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2920 2023-04-28 16:06:02.000000 alethiometer-1.0.7/alethiometer/zero_cost_metrics/zen.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2412 2023-04-23 12:05:26.000000 alethiometer-1.0.7/alethiometer/zero_cost_metrics/zico.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 16:12:53.173044 alethiometer-1.0.7/alethiometer.egg-info/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2995 2023-04-28 16:12:53.000000 alethiometer-1.0.7/alethiometer.egg-info/PKG-INFO
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      873 2023-04-28 16:12:53.000000 alethiometer-1.0.7/alethiometer.egg-info/SOURCES.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)        1 2023-04-28 16:12:53.000000 alethiometer-1.0.7/alethiometer.egg-info/dependency_links.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       37 2023-04-28 16:12:53.000000 alethiometer-1.0.7/alethiometer.egg-info/requires.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       13 2023-04-28 16:12:53.000000 alethiometer-1.0.7/alethiometer.egg-info/top_level.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       38 2023-04-28 16:12:53.177044 alethiometer-1.0.7/setup.cfg
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6031 2023-04-07 18:04:03.000000 alethiometer-1.0.7/setup.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 16:12:53.177044 alethiometer-1.0.7/tests/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1851 2023-04-11 17:20:25.000000 alethiometer-1.0.7/tests/test_zc.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:21:56.112996 alethiometer-1.0.8/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    11357 2023-04-07 16:49:02.000000 alethiometer-1.0.8/LICENSE
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6663 2023-04-28 22:21:56.112996 alethiometer-1.0.8/PKG-INFO
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5953 2023-04-28 22:00:25.000000 alethiometer-1.0.8/README.md
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:21:56.108996 alethiometer-1.0.8/alethiometer/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      313 2023-04-11 12:10:43.000000 alethiometer-1.0.8/alethiometer/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      245 2023-04-28 22:20:39.000000 alethiometer-1.0.8/alethiometer/__version__.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:21:56.108996 alethiometer-1.0.8/alethiometer/datasets/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      254 2023-04-07 17:54:55.000000 alethiometer-1.0.8/alethiometer/datasets/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4853 2023-04-17 13:10:20.000000 alethiometer-1.0.8/alethiometer/datasets/dataset.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2174 2023-04-07 17:54:22.000000 alethiometer-1.0.8/alethiometer/datasets/h5py_dataset.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5109 2023-04-07 17:55:28.000000 alethiometer-1.0.8/alethiometer/datasets/imagenet16.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1077 2023-04-07 15:01:32.000000 alethiometer-1.0.8/alethiometer/utils.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4968 2023-04-28 22:17:58.000000 alethiometer-1.0.8/alethiometer/zc_proxy.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:21:56.108996 alethiometer-1.0.8/alethiometer/zero_cost_metrics/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1660 2023-04-28 21:23:03.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1475 2023-04-07 17:10:09.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/grad_norm.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3624 2023-04-07 17:13:08.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/grasp.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2926 2023-04-11 16:57:48.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/naswot.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2079 2023-04-28 20:46:05.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/naswot_relu.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2023 2023-04-07 17:09:49.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/snip.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1928 2023-04-07 17:06:05.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/synflow.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    15593 2023-04-28 22:16:08.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/tenas.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3420 2023-04-28 21:42:23.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/zen.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2412 2023-04-23 12:05:26.000000 alethiometer-1.0.8/alethiometer/zero_cost_metrics/zico.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:21:56.108996 alethiometer-1.0.8/alethiometer.egg-info/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6663 2023-04-28 22:21:56.000000 alethiometer-1.0.8/alethiometer.egg-info/PKG-INFO
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      898 2023-04-28 22:21:56.000000 alethiometer-1.0.8/alethiometer.egg-info/SOURCES.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)        1 2023-04-28 22:21:56.000000 alethiometer-1.0.8/alethiometer.egg-info/dependency_links.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       37 2023-04-28 22:21:56.000000 alethiometer-1.0.8/alethiometer.egg-info/requires.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       13 2023-04-28 22:21:56.000000 alethiometer-1.0.8/alethiometer.egg-info/top_level.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       38 2023-04-28 22:21:56.112996 alethiometer-1.0.8/setup.cfg
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6031 2023-04-07 18:04:03.000000 alethiometer-1.0.8/setup.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:21:56.108996 alethiometer-1.0.8/tests/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1219 2023-04-25 09:05:55.000000 alethiometer-1.0.8/tests/test_nwot_api.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3098 2023-04-28 22:20:47.000000 alethiometer-1.0.8/tests/test_zc.py
```

### Comparing `alethiometer-1.0.7/LICENSE` & `alethiometer-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.7/alethiometer/datasets/dataset.py` & `alethiometer-1.0.8/alethiometer/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.7/alethiometer/datasets/h5py_dataset.py` & `alethiometer-1.0.8/alethiometer/datasets/h5py_dataset.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.7/alethiometer/datasets/imagenet16.py` & `alethiometer-1.0.8/alethiometer/datasets/imagenet16.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.7/alethiometer/utils.py` & `alethiometer-1.0.8/alethiometer/utils.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.7/alethiometer/zc_proxy.py` & `alethiometer-1.0.8/alethiometer/zc_proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 Author: ViolinSolo
 Date: 2023-04-06 18:35:04
-LastEditTime: 2023-04-28 17:07:31
+LastEditTime: 2023-04-28 23:16:16
 LastEditors: ViolinSolo
 Description: entry program
 FilePath: /zero-cost-proxies/alethiometer/zc_proxy.py
 '''
 import types
 import copy
 import torch
@@ -29,14 +29,17 @@
     'nwot_Kmats',   # return(Kmats, logdet) our conv and fc based NASWOT, but return Kmats and its logdet
     'lnwot',        # layer-wise our conv and fc based NASWOT
     'lnwot_Kmats',  # return(Kmats, logdet) layer-wise our conv and fc based NASWOT, but return Kmats and its logdet
     'snip',         # snip
     'synflow',      # synflow
     'synflow_bn',   # synflow with bn
     'zen',          # ZenNAS: https://github.com/idstcv/ZenNAS/blob/main/ZeroShotProxy/compute_zen_score.py
+    'tenas',        # tenas.py contains three metrics: lrn, ntk, tenas
+    'ntk',          # NTK
+    'lrn',          # LRN
 ]
 
 def no_op(self, x):
     return x
 
 def copynet(self, bn):
     net = copy.deepcopy(self)
@@ -116,15 +119,17 @@
         if hasattr(arr, '__len__'):  # ignore some cases like str or tuple.
             for i in range(len(arr)):
                 val = arr[i]
                 val = val if type(val) is torch.Tensor else torch.tensor(val)
                 sum += torch.sum(val)
         else:
             sum = arr
-        return sum.item()
+        # print('sum type', type(sum))
+        return sum.item() if hasattr(sum, 'item') else sum  #fix bug when sum is neither tensor nor numpy.float32 nor numpy.float64
     
     results = {}
     for k, v in mt_vals.items():
+        # print('k', k)
         results[k] = v if not aggregate else sum_arr(v)
 
     return results
 # end def
```

### Comparing `alethiometer-1.0.7/alethiometer/zero_cost_metrics/__init__.py` & `alethiometer-1.0.8/alethiometer/zero_cost_metrics/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 Author: ViolinSolo
 Date: 2023-04-06 17:43:34
-LastEditTime: 2023-04-28 17:06:51
+LastEditTime: 2023-04-28 21:48:59
 LastEditors: ViolinSolo
 Description: init files 
 FilePath: /zero-cost-proxies/alethiometer/zero_cost_metrics/__init__.py
 '''
 
 import gc
 import torch
@@ -46,7 +46,8 @@
 from . import snip
 from . import synflow
 from . import grasp
 from . import grad_norm
 from . import naswot # this is our NASWOT implementation (layer-wise or not, based on conv and fc)
 from . import naswot_relu  # this is original RELU based NASWOT implementation
 from . import zen 
+from . import tenas # this is TENAS implementation, including lrn, ntk, tenas
```

### Comparing `alethiometer-1.0.7/alethiometer/zero_cost_metrics/grad_norm.py` & `alethiometer-1.0.8/alethiometer/zero_cost_metrics/grad_norm.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.7/alethiometer/zero_cost_metrics/grasp.py` & `alethiometer-1.0.8/alethiometer/zero_cost_metrics/grasp.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.7/alethiometer/zero_cost_metrics/naswot.py` & `alethiometer-1.0.8/alethiometer/zero_cost_metrics/naswot.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.7/alethiometer/zero_cost_metrics/naswot_relu.py` & `alethiometer-1.0.8/alethiometer/zero_cost_metrics/naswot_relu.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 Author: ViolinSolo
 Date: 2023-04-26 12:23:01
-LastEditTime: 2023-04-28 14:53:18
+LastEditTime: 2023-04-28 21:44:16
 LastEditors: ViolinSolo
 Description: original RELU based NASWOT implementation.
 FilePath: /zero-cost-proxies/alethiometer/zero_cost_metrics/naswot_relu.py
 '''
 import torch
 import torch.nn as nn
 import numpy as np
@@ -18,49 +18,50 @@
 
 def safe_hooklogdet(K):
     s, ld = np.linalg.slogdet(K)
     return 0 if (np.isneginf(ld) and s==0) else ld
 
 @metric('nwot_relu', bn=True)
 @metric('nwot_relu_Kmats', bn=True, return_Kmats=True)
-def compute_naswot(net, inputs, targets, loss_fn, split_data=1, return_Kmats=False):
+def compute_naswot(net, inputs, targets, loss_fn, split_data=1, 
+                   return_Kmats=False):
     """
     This is the original RELU based NASWOT implementation.
     Based on v2 paper, and its repo link: 
     https://github.com/BayesWatch/nas-without-training/blob/master/score_networks.py
     """
     net.eval()
 
 
     net.K = 0. # **naswot matrix**, NONE-layer-wise | e (mat,) ===> using torch broadcasting tech to init zero-like matrix
     def counting_forward_hook(module, inp, out):
-        try:
-            if not module.visited_backwards:
-                return
-            if isinstance(inp, tuple):
-                inp = inp[0]
-            inp = inp.view(inp.size(0), -1)
-            x = (inp > 0).float()
-            K = x @ x.t()
-            K2 = (1.-x) @ (1.-x.t())
-            net.K = net.K + K.cpu().numpy() + K2.cpu().numpy()
-        except:
-            pass
+        # try:
+        #    if not module.visited_backwards:
+        #        return
+        if isinstance(inp, tuple):
+            inp = inp[0]
+        inp = inp.view(inp.size(0), -1)
+        x = (inp > 0).float()
+        K = x @ x.t()
+        K2 = (1.-x) @ (1.-x.t())
+        net.K = net.K + K.cpu().numpy() + K2.cpu().numpy()  # remove this original code, since we want use broadcasting tech
+        # except:
+        #     pass
 
 
     def counting_backward_hook(module, inp, out):
         module.visited_backwards = True
 
 
     for name, module in net.named_modules():
         if 'ReLU' in str(type(module)):
             #hooks[name] = module.register_forward_hook(counting_hook)
             module.register_forward_hook(counting_forward_hook)
-            module.register_backward_hook(counting_backward_hook)
+            # module.register_backward_hook(counting_backward_hook)
 
 
     with torch.no_grad():
         net(inputs)
 
     K_mat = net.K
-    K_mat_logdet = safe_hooklogdet(K_mat.cpu().numpy())
+    K_mat_logdet = safe_hooklogdet(K_mat)
     return (K_mat, K_mat_logdet) if return_Kmats else K_mat_logdet
```

### Comparing `alethiometer-1.0.7/alethiometer/zero_cost_metrics/snip.py` & `alethiometer-1.0.8/alethiometer/zero_cost_metrics/snip.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.7/alethiometer/zero_cost_metrics/synflow.py` & `alethiometer-1.0.8/alethiometer/zero_cost_metrics/synflow.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.7/alethiometer/zero_cost_metrics/zen.py` & `alethiometer-1.0.8/alethiometer/zero_cost_metrics/zen.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 Author: ViolinSolo
 Date: 2023-04-23 12:57:36
-LastEditTime: 2023-04-28 17:04:40
+LastEditTime: 2023-04-28 22:42:23
 LastEditors: ViolinSolo
 Description: zen
 FilePath: /zero-cost-proxies/alethiometer/zero_cost_metrics/zen.py
 '''
 
 # =============================================================================
 #   Copyright (C) 2010-2021 Alibaba Group Holding Limited.
@@ -52,14 +52,18 @@
     with torch.no_grad():
         for repeat_count in range(repeat):
             network_weight_gaussian_init(net)
             input = torch.randn(size=list(inputs.shape), device=device, dtype=dtype)
             input2 = torch.randn(size=list(inputs.shape), device=device, dtype=dtype)
             mixup_input = input + mixup_gamma * input2
 
+            if not hasattr(net, 'forward_before_global_avg_pool'):
+                suggestion_msg = "\n\tPlease implement forward_before_global_avg_pool() in your network.\n\tYou can follow implementation of fn:`forward_pre_GAP()` in ZenNet:\n\thttps://github.com/idstcv/ZenNAS/blob/2629dc5692b3d9d01ef94b559e6bd4a4b114b617/Masternet.py#L98"
+                raise NotImplementedError(suggestion_msg)
+
             output = net.forward_before_global_avg_pool(input)
             mixup_output = net.forward_before_global_avg_pool(mixup_input)
 
             nas_score = torch.sum(torch.abs(output - mixup_output), dim=[1, 2, 3])
             nas_score = torch.mean(nas_score)
 
             # compute BN scaling
@@ -72,10 +76,11 @@
             pass
             nas_score = torch.log(nas_score) + log_bn_scaling_factor
             nas_score_list.append(float(nas_score))
 
     ## 95% confidence interval of NAS score
     # std_nas_score = np.std(nas_score_list)
     # avg_precision = float(1.96 * std_nas_score / np.sqrt(len(nas_score_list)))
-    avg_nas_score = float(np.mean(nas_score_list))
+    # avg_nas_score = float(np.mean(nas_score_list))
+    avg_nas_score = np.mean(nas_score_list)  # fix bug when calling .item() on this return value
 
     return avg_nas_score
```

### Comparing `alethiometer-1.0.7/alethiometer/zero_cost_metrics/zico.py` & `alethiometer-1.0.8/alethiometer/zero_cost_metrics/zico.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.7/alethiometer.egg-info/SOURCES.txt` & `alethiometer-1.0.8/alethiometer.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -15,13 +15,14 @@
 alethiometer/datasets/h5py_dataset.py
 alethiometer/datasets/imagenet16.py
 alethiometer/zero_cost_metrics/__init__.py
 alethiometer/zero_cost_metrics/grad_norm.py
 alethiometer/zero_cost_metrics/grasp.py
 alethiometer/zero_cost_metrics/naswot.py
 alethiometer/zero_cost_metrics/naswot_relu.py
-alethiometer/zero_cost_metrics/ntk.py
 alethiometer/zero_cost_metrics/snip.py
 alethiometer/zero_cost_metrics/synflow.py
+alethiometer/zero_cost_metrics/tenas.py
 alethiometer/zero_cost_metrics/zen.py
 alethiometer/zero_cost_metrics/zico.py
+tests/test_nwot_api.py
 tests/test_zc.py
```

### Comparing `alethiometer-1.0.7/setup.py` & `alethiometer-1.0.8/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/saliency_maps_metrics-0.0.8.tar.gz` & `tmp/saliency_maps_metrics-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saliency_maps_metrics-0.0.8.tar", last modified: Wed Feb  1 18:08:02 2023, max compression
+gzip compressed data, was "saliency_maps_metrics-0.0.9.tar", last modified: Wed Feb  1 18:36:41 2023, max compression
```

## Comparing `saliency_maps_metrics-0.0.8.tar` & `saliency_maps_metrics-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 E144069X  (1003) E144069X  (1003)        0 2023-02-01 18:08:02.180560 saliency_maps_metrics-0.0.8/
--rw-rw-r--   0 E144069X  (1003) E144069X  (1003)     1074 2023-01-27 12:28:26.000000 saliency_maps_metrics-0.0.8/LICENSE
--rw-rw-r--   0 E144069X  (1003) E144069X  (1003)      217 2023-02-01 07:53:29.000000 saliency_maps_metrics-0.0.8/MANIFEST.in
--rw-rw-r--   0 E144069X  (1003) E144069X  (1003)     5480 2023-02-01 18:08:02.180560 saliency_maps_metrics-0.0.8/PKG-INFO
--rw-rw-r--   0 E144069X  (1003) E144069X  (1003)     4778 2023-02-01 09:50:44.000000 saliency_maps_metrics-0.0.8/README.md
--rw-rw-r--   0 E144069X  (1003) E144069X  (1003)      774 2023-02-01 18:07:33.000000 saliency_maps_metrics-0.0.8/pyproject.toml
-drwxrwxr-x   0 E144069X  (1003) E144069X  (1003)        0 2023-02-01 18:08:02.180560 saliency_maps_metrics-0.0.8/saliency_maps_metrics/
--rw-rw-r--   0 E144069X  (1003) E144069X  (1003)        0 2023-01-27 12:22:21.000000 saliency_maps_metrics-0.0.8/saliency_maps_metrics/__init__.py
--rw-rw-r--   0 E144069X  (1003) E144069X  (1003)      860 2023-02-01 15:10:35.000000 saliency_maps_metrics-0.0.8/saliency_maps_metrics/data_replace.py
--rw-rw-r--   0 E144069X  (1003) E144069X  (1003)     6232 2023-02-01 17:02:40.000000 saliency_maps_metrics-0.0.8/saliency_maps_metrics/multi_step_metrics.py
--rw-rw-r--   0 E144069X  (1003) E144069X  (1003)     2852 2023-02-01 17:06:49.000000 saliency_maps_metrics-0.0.8/saliency_maps_metrics/single_step_metrics.py
-drwxrwxr-x   0 E144069X  (1003) E144069X  (1003)        0 2023-02-01 18:08:02.180560 saliency_maps_metrics-0.0.8/saliency_maps_metrics.egg-info/
--rw-rw-r--   0 E144069X  (1003) E144069X  (1003)     5480 2023-02-01 18:08:02.000000 saliency_maps_metrics-0.0.8/saliency_maps_metrics.egg-info/PKG-INFO
--rw-rw-r--   0 E144069X  (1003) E144069X  (1003)      394 2023-02-01 18:08:02.000000 saliency_maps_metrics-0.0.8/saliency_maps_metrics.egg-info/SOURCES.txt
--rw-rw-r--   0 E144069X  (1003) E144069X  (1003)        1 2023-02-01 18:08:02.000000 saliency_maps_metrics-0.0.8/saliency_maps_metrics.egg-info/dependency_links.txt
--rw-rw-r--   0 E144069X  (1003) E144069X  (1003)       22 2023-02-01 18:08:02.000000 saliency_maps_metrics-0.0.8/saliency_maps_metrics.egg-info/top_level.txt
--rw-rw-r--   0 E144069X  (1003) E144069X  (1003)       38 2023-02-01 18:08:02.180560 saliency_maps_metrics-0.0.8/setup.cfg
--rw-rw-r--   0 E144069X  (1003) E144069X  (1003)       79 2023-02-01 10:17:40.000000 saliency_maps_metrics-0.0.8/setup.py
+drwxrwxr-x   0 E144069X  (1003) E144069X  (1003)        0 2023-02-01 18:36:41.517226 saliency_maps_metrics-0.0.9/
+-rw-rw-r--   0 E144069X  (1003) E144069X  (1003)     1074 2023-01-27 12:28:26.000000 saliency_maps_metrics-0.0.9/LICENSE
+-rw-rw-r--   0 E144069X  (1003) E144069X  (1003)      217 2023-02-01 07:53:29.000000 saliency_maps_metrics-0.0.9/MANIFEST.in
+-rw-rw-r--   0 E144069X  (1003) E144069X  (1003)     5480 2023-02-01 18:36:41.517226 saliency_maps_metrics-0.0.9/PKG-INFO
+-rw-rw-r--   0 E144069X  (1003) E144069X  (1003)     4778 2023-02-01 09:50:44.000000 saliency_maps_metrics-0.0.9/README.md
+-rw-rw-r--   0 E144069X  (1003) E144069X  (1003)      774 2023-02-01 18:36:28.000000 saliency_maps_metrics-0.0.9/pyproject.toml
+drwxrwxr-x   0 E144069X  (1003) E144069X  (1003)        0 2023-02-01 18:36:41.517226 saliency_maps_metrics-0.0.9/saliency_maps_metrics/
+-rw-rw-r--   0 E144069X  (1003) E144069X  (1003)        0 2023-01-27 12:22:21.000000 saliency_maps_metrics-0.0.9/saliency_maps_metrics/__init__.py
+-rw-rw-r--   0 E144069X  (1003) E144069X  (1003)      860 2023-02-01 15:10:35.000000 saliency_maps_metrics-0.0.9/saliency_maps_metrics/data_replace.py
+-rw-rw-r--   0 E144069X  (1003) E144069X  (1003)     6240 2023-02-01 18:32:32.000000 saliency_maps_metrics-0.0.9/saliency_maps_metrics/multi_step_metrics.py
+-rw-rw-r--   0 E144069X  (1003) E144069X  (1003)     2861 2023-02-01 18:31:56.000000 saliency_maps_metrics-0.0.9/saliency_maps_metrics/single_step_metrics.py
+drwxrwxr-x   0 E144069X  (1003) E144069X  (1003)        0 2023-02-01 18:36:41.517226 saliency_maps_metrics-0.0.9/saliency_maps_metrics.egg-info/
+-rw-rw-r--   0 E144069X  (1003) E144069X  (1003)     5480 2023-02-01 18:36:41.000000 saliency_maps_metrics-0.0.9/saliency_maps_metrics.egg-info/PKG-INFO
+-rw-rw-r--   0 E144069X  (1003) E144069X  (1003)      394 2023-02-01 18:36:41.000000 saliency_maps_metrics-0.0.9/saliency_maps_metrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 E144069X  (1003) E144069X  (1003)        1 2023-02-01 18:36:41.000000 saliency_maps_metrics-0.0.9/saliency_maps_metrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 E144069X  (1003) E144069X  (1003)       22 2023-02-01 18:36:41.000000 saliency_maps_metrics-0.0.9/saliency_maps_metrics.egg-info/top_level.txt
+-rw-rw-r--   0 E144069X  (1003) E144069X  (1003)       38 2023-02-01 18:36:41.517226 saliency_maps_metrics-0.0.9/setup.cfg
+-rw-rw-r--   0 E144069X  (1003) E144069X  (1003)       79 2023-02-01 10:17:40.000000 saliency_maps_metrics-0.0.9/setup.py
```

### Comparing `saliency_maps_metrics-0.0.8/LICENSE` & `saliency_maps_metrics-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `saliency_maps_metrics-0.0.8/PKG-INFO` & `saliency_maps_metrics-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saliency_maps_metrics
-Version: 0.0.8
+Version: 0.0.9
 Summary: This repository implements the faithfulness metrics mentionned in the paper --Computing and evaluating saliency maps for image classification: a tutorial-- in Pytorch.
 Author-email: Tristan Gomez <tristan.gomez@univ-nantes.fr>
 Project-URL: Homepage, https://github.com/TristanGomez44/metrics-saliency-maps
 Project-URL: Bug Tracker, https://github.com/TristanGomez44/metrics-saliency-maps/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saliency_maps_metrics-0.0.8/README.md` & `saliency_maps_metrics-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `saliency_maps_metrics-0.0.8/pyproject.toml` & `saliency_maps_metrics-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "saliency_maps_metrics"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Tristan Gomez", email="tristan.gomez@univ-nantes.fr" },
 ]
 description = "This repository implements the faithfulness metrics mentionned in the paper --Computing and evaluating saliency maps for image classification: a tutorial-- in Pytorch."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `saliency_maps_metrics-0.0.8/saliency_maps_metrics/data_replace.py` & `saliency_maps_metrics-0.0.9/saliency_maps_metrics/data_replace.py`

 * *Files identical despite different names*

### Comparing `saliency_maps_metrics-0.0.8/saliency_maps_metrics/multi_step_metrics.py` & `saliency_maps_metrics-0.0.9/saliency_maps_metrics/multi_step_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,16 +110,16 @@
                     
                 iter_nb += 1
                 left_pixel_nb -= pixel_removed_per_step
 
             all_score_list.append(score_list)
             all_sal_score_list.append(saliency_score_list)
 
-        all_score_list = np.array(all_score_list)
-        all_sal_score_list = np.array(all_sal_score_list)
+        all_score_list = torch.tensor(all_score_list)
+        all_sal_score_list = torch.tensor(all_sal_score_list)
 
         return all_score_list,all_sal_score_list
 
     def __call__(self,model,data,explanations,class_to_explain_list=None,masking_data=None):
         all_score_list,all_sal_score_list = self.compute_scores(model,data,explanations,class_to_explain_list,masking_data)
         mean_auc_metric = compute_auc_metric(all_score_list)
         mean_calibration_metric = self.compute_calibration_metric(all_score_list, all_sal_score_list)
```

### Comparing `saliency_maps_metrics-0.0.8/saliency_maps_metrics/single_step_metrics.py` & `saliency_maps_metrics-0.0.9/saliency_maps_metrics/single_step_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         score_masked_list = []
         for i in range(len(data)):
             if class_to_explain_list is None:
                 class_to_explain = torch.argmax(model(data[i:i+1]),axis=1)[0]
             else:
                 class_to_explain = class_to_explain_list[i]
         
-            score = model(data[i:i+1])[0,class_to_explain]
+            score = model(data[i:i+1])[0,class_to_explain].item()  
             score_masked = model(data_masked[i:i+1])[0,class_to_explain].item()          
             score_list.append(score)
             score_masked_list.append(score_masked)
 
         score_list = torch.tensor(score_list)
         score_masked_list = torch.tensor(score_masked_list)
```

### Comparing `saliency_maps_metrics-0.0.8/saliency_maps_metrics.egg-info/PKG-INFO` & `saliency_maps_metrics-0.0.9/saliency_maps_metrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saliency-maps-metrics
-Version: 0.0.8
+Version: 0.0.9
 Summary: This repository implements the faithfulness metrics mentionned in the paper --Computing and evaluating saliency maps for image classification: a tutorial-- in Pytorch.
 Author-email: Tristan Gomez <tristan.gomez@univ-nantes.fr>
 Project-URL: Homepage, https://github.com/TristanGomez44/metrics-saliency-maps
 Project-URL: Bug Tracker, https://github.com/TristanGomez44/metrics-saliency-maps/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


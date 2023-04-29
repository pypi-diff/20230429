# Comparing `tmp/pyPhasesML-0.5.0.tar.gz` & `tmp/pyPhasesML-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.5.0.tar", last modified: Fri Apr 28 10:07:37 2023, max compression
+gzip compressed data, was "pyPhasesML-0.5.1.tar", last modified: Sat Apr 29 13:58:16 2023, max compression
```

## Comparing `pyPhasesML-0.5.0.tar` & `pyPhasesML-0.5.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:07:37.060189 pyPhasesML-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3691 2023-04-28 10:07:37.060189 pyPhasesML-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3184 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:07:37.053188 pyPhasesML-0.5.0/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2348 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     3065 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/DataversionManager.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)     4368 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4558 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:07:37.056188 pyPhasesML-0.5.0/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10212 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)    17734 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/adapter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:07:37.058188 pyPhasesML-0.5.0/pyPhasesML/datapipes/
--rw-rw-rw-   0 root         (0) root         (0)      464 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/datapipes/Augmentor.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/datapipes/DatasetXY.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/datapipes/FoldMapper.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/datapipes/RecordMap.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/datapipes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:07:37.059188 pyPhasesML-0.5.0/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5358 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:07:37.060189 pyPhasesML-0.5.0/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    19178 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:07:37.055188 pyPhasesML-0.5.0/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3691 2023-04-28 10:07:36.000000 pyPhasesML-0.5.0/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1041 2023-04-28 10:07:37.000000 pyPhasesML-0.5.0/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 10:07:36.000000 pyPhasesML-0.5.0/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-28 10:07:36.000000 pyPhasesML-0.5.0/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-28 10:07:36.000000 pyPhasesML-0.5.0/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 10:07:37.061189 pyPhasesML-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-04-28 10:07:13.000000 pyPhasesML-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:58:16.513744 pyPhasesML-0.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-04-29 13:58:16.513744 pyPhasesML-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3184 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:58:16.506744 pyPhasesML-0.5.1/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3870 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/DataversionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4368 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4558 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:58:16.509744 pyPhasesML-0.5.1/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10212 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7116 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    17785 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/adapter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:58:16.511744 pyPhasesML-0.5.1/pyPhasesML/datapipes/
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/datapipes/Augmentor.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/datapipes/DatasetXY.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/datapipes/FoldMapper.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/datapipes/RecordMap.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/datapipes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:58:16.512745 pyPhasesML-0.5.1/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5358 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:58:16.513744 pyPhasesML-0.5.1/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    19178 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 13:58:16.508744 pyPhasesML-0.5.1/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-04-29 13:58:16.000000 pyPhasesML-0.5.1/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-04-29 13:58:16.000000 pyPhasesML-0.5.1/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 13:58:16.000000 pyPhasesML-0.5.1/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-29 13:58:16.000000 pyPhasesML-0.5.1/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-29 13:58:16.000000 pyPhasesML-0.5.1/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-29 13:57:53.000000 pyPhasesML-0.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 13:58:16.514745 pyPhasesML-0.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-04-29 13:57:55.000000 pyPhasesML-0.5.1/setup.py
```

### Comparing `pyPhasesML-0.5.0/LICENSE` & `pyPhasesML-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.0/PKG-INFO` & `pyPhasesML-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.5.0/README.md` & `pyPhasesML-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.0/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.5.1/pyPhasesML/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.0/pyPhasesML/DataSet.py` & `pyPhasesML-0.5.1/pyPhasesML/DataSet.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.0/pyPhasesML/DataversionManager.py` & `pyPhasesML-0.5.1/pyPhasesML/DataversionManager.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ast import main
 import numpy as np
 from pyPhases import classLogger
 
 
 class NotUniqueException(Exception):
     pass
 
@@ -9,32 +10,41 @@
 class NotCompleteException(Exception):
     pass
 
 
 @classLogger
 class DataversionManager:
     def __init__(self, groupedRecords, splits, seed=None) -> None:
-        self.splits = splits
+        # make sure that the orginal splits dont get manipulated
+        self.splits = splits.copy()
         self.seed = seed
         self.removedRecords = {}
+        self.splitHasSubs = []
 
         # shuffle the records
         groups = list(groupedRecords.keys())
         if seed is not None:
             np.random.seed(seed)
             np.random.shuffle(groups)
             groupedRecords = {g: groupedRecords[g] for g in groups}
 
         self.groupedRecords = groupedRecords
 
     def groupDatasetBySplit(self, datasetName, splits, groupedRecords, removedRecords=None):
-        sliceForDataset = slice(*[int(index) for index in splits[datasetName][0].split(":")])
-        groups = list(groupedRecords.keys())[sliceForDataset]
+        split = splits[datasetName]
+        # check if split is a list of recordids
+        if isinstance(split, dict):
+            mainSplit = split["mainsplit"]
+            mainRecordIds = self.getRecordsForSplit(mainSplit)
+            recordIds = [mainRecordIds[i] for i in split["indexes"]]
+        else:
+            sliceForDataset = slice(*[int(index) for index in splits[datasetName][0].split(":")])
+            groups = list(groupedRecords.keys())[sliceForDataset]
+            recordIds = [record for group in groups for record in groupedRecords[group]]
 
-        recordIds = [record for group in groups for record in groupedRecords[group]]
         if bool(removedRecords):
             recordIds = [record for index, record in enumerate(recordIds) if index not in removedRecords]
 
         return recordIds
 
     def groupDatasetsBySplit(self, datasetNames, splits, groupedRecords):
         recordSlices = {}
@@ -43,17 +53,19 @@
 
         return recordSlices
 
     def getRecordsForSplit(self, datasetName):
         removedRecords = self.removedRecords.get(datasetName, None)
         return self.groupDatasetBySplit(datasetName, self.splits, self.groupedRecords, removedRecords)
 
-    def validatDatasetVersion(self, datasetNames, raiseException=True):
+    def validatDatasetVersion(self, raiseException=True):
         allDBRecordIds = self.groupedRecords
-        splits = self.splits
+        # remove splits keys that have subsplits
+        splits = {k: v for k, v in self.splits.items() if k not in self.splitHasSubs}
+        datasetNames = list(splits.keys())
 
         recordSlices = self.groupDatasetsBySplit(datasetNames, splits, allDBRecordIds)
 
         flattenAllRecords = [r for elem in allDBRecordIds.values() for r in elem]
         flattenUsedRecords = [r for elem in recordSlices.values() for r in elem]
 
         # check if all records are unique and present in the dataset splits
@@ -76,7 +88,11 @@
                 raise NotCompleteException(error)
 
         if complete and unique:
             self.logSuccess("All records are unique and present in the dataset splits")
 
     def removeRecordIndexesFromSplit(self, datasetName, recordIndexes):
         self.removedRecords[datasetName] = recordIndexes
+
+    def addVirtualSplitByMainSplitIndexes(self, mainsplit, datasetName, recordIndexes):
+        self.splitHasSubs.append(mainsplit)
+        self.splits[datasetName] = {"mainsplit": mainsplit, "indexes": list(recordIndexes)}
```

### Comparing `pyPhasesML-0.5.0/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.5.1/pyPhasesML/FeatureExtraction.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.0/pyPhasesML/Model.py` & `pyPhasesML-0.5.1/pyPhasesML/Model.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.0/pyPhasesML/ModelManager.py` & `pyPhasesML-0.5.1/pyPhasesML/ModelManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.0/pyPhasesML/Plugin.py` & `pyPhasesML-0.5.1/pyPhasesML/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.0/pyPhasesML/SignalPreprocessing.py` & `pyPhasesML-0.5.1/pyPhasesML/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.0/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.5.1/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.0/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.5.1/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.0/pyPhasesML/adapter/ModelTorchAdapter.py` & `pyPhasesML-0.5.1/pyPhasesML/adapter/ModelTorchAdapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,14 +392,15 @@
             minLr = lr_find_lr[np.argmin(lr_find_loss)]
             print("Lowest Loss LR: %f" % minLr)
             print("Suggested LR range max bound: %f" % minLr)
             self.lr_find_lr = lr_find_lr
             self.lr_find_loss = lr_find_loss
 
         self.fullEpochs = i_epoch
+        self.metricDefinitions = metricDefinitions
         return lastImprovdModel
 
     def getModelPath(self):
         return self.logPath
 
     def build(self):
         torchSeed = 2
```

### Comparing `pyPhasesML-0.5.0/pyPhasesML/config.yaml` & `pyPhasesML-0.5.1/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.0/pyPhasesML/datapipes/DatasetXY.py` & `pyPhasesML-0.5.1/pyPhasesML/datapipes/DatasetXY.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.0/pyPhasesML/datapipes/FoldMapper.py` & `pyPhasesML-0.5.1/pyPhasesML/datapipes/FoldMapper.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.0/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.5.1/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.0/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.5.1/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.0/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.5.1/pyPhasesML/scorer/Scorer.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     assert true.shape == pred.shape
 
     size = len(labels)
     classes = np.arange(size)
     confmat = np.zeros((size, size))
 
     for i, j in itertools.product(range(size), range(size)):
-        confmat[i, j] = np.sum((true == classes[i]) & (pred == classes[j]))
+        confmat[i, j] = ((true == classes[i]) & (pred == classes[j])).sum()
 
     return confmat
 
 
 class Scorer:
     title = "Segmentbasiert"
     cmScaleByClass = 4
```

### Comparing `pyPhasesML-0.5.0/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.5.1/pyPhasesML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.5.0/pyPhasesML.egg-info/SOURCES.txt` & `pyPhasesML-0.5.1/pyPhasesML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.5.0/setup.py` & `pyPhasesML-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.5.0"[1:],
+    version="v0.5.1"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
```


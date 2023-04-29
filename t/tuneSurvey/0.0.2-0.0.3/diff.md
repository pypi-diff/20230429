# Comparing `tmp/tunesurvey-0.0.2.tar.gz` & `tmp/tunesurvey-0.0.3.tar.gz`

## Comparing `tunesurvey-0.0.2.tar` & `tunesurvey-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tunesurvey-0.0.2/src/tuneSurvey/__init__.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 tunesurvey-0.0.2/src/tuneSurvey/sklearn_modelList.py
--rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 tunesurvey-0.0.2/src/tuneSurvey/vectorized_search_by_term.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 tunesurvey-0.0.2/LICENSE
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 tunesurvey-0.0.2/README.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 tunesurvey-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 tunesurvey-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/demo.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/src/tuneSurvey/__init__.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/src/tuneSurvey/cleansing.py
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/src/tuneSurvey/skLists.py
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/src/tuneSurvey/tsReshape.py
+-rw-r--r--   0        0        0     8065 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/src/tuneSurvey/ts_torchLists.py
+-rw-r--r--   0        0        0     7540 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/src/tuneSurvey/vectorized_search_by_term.py
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/tuneSurvey.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/tuneSurvey.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/tuneSurvey.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/tuneSurvey.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/README.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 tunesurvey-0.0.3/PKG-INFO
```

### Comparing `tunesurvey-0.0.2/src/tuneSurvey/vectorized_search_by_term.py` & `tunesurvey-0.0.3/src/tuneSurvey/tsReshape.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from sklearn.model_selection import GridSearchCV
 def vectorized_Search_hyperparameter(model, parameters, X, Y,cv =  5,search_function = GridSearchCV,verbose =False):
     """
     # model - type of model (SVR(), randomForest()...)
     # X - predictor - all rows of X are used for prediction, but each model only gives on entry in Y
     # Y - matrix containing n_var number of column vectors as target of the prediction
     # cv - cross validation type (scikit-learn obj) passed in to model selection type.
     # cv is either a number for k fold or a model selection obj for esample, cv = TimeSeriesSplit(n_splits=2, max_train_size=None, test_size=2, gap=0)
@@ -14,15 +15,15 @@
     for i in range(n_var):
         if verbose:
             print("working on:" + str(modelName),"model",i)
         m_Yi.append(search_function(model, param_grid = parameters, cv=cv).fit(X,Y[:,i]))
     return m_Yi
 
 
-def saveModelList_s(modelList,X,Y,path="sklModels",verbose=verbose):
+def saveModelList_s(modelList,X,Y,path="sklModels",verbose=False):
     """save a list of model named by modelSequence() convention"""
     pgd = ParameterGrid(modelList['par'])
     if verbose:
         print("Permutating models and saving")
     for i, pars in enumerate(pgd):
         m = deepcopy(modelList['modelInit'])
         if verbose:
```

### Comparing `tunesurvey-0.0.2/LICENSE` & `tunesurvey-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tunesurvey-0.0.2/README.md` & `tunesurvey-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tunesurvey-0.0.2/pyproject.toml` & `tunesurvey-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "tuneSurvey"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Hao Li", email="lhrcplanes@qq.com" },
 ]
 description = "Automatic tuning of machine learning models and surveying on the performance across subsets, variables, features, hyperparameters and pipelines"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `tunesurvey-0.0.2/PKG-INFO` & `tunesurvey-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneSurvey
-Version: 0.0.2
+Version: 0.0.3
 Summary: Automatic tuning of machine learning models and surveying on the performance across subsets, variables, features, hyperparameters and pipelines
 Project-URL: Homepage, https://pypi.org/project/tuneSurvey/0.0.1/
 Project-URL: Bug Tracker, https://github.com/HaoLi111/tuneSurvey/issues
 Author-email: Hao Li <lhrcplanes@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


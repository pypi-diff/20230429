# Comparing `tmp/protloc_mex1-0.0.1.tar.gz` & `tmp/protloc_mex1-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protloc_mex1-0.0.1.tar", last modified: Fri Apr 28 11:54:26 2023, max compression
+gzip compressed data, was "protloc_mex1-0.0.2.tar", last modified: Fri Apr 28 14:13:36 2023, max compression
```

## Comparing `protloc_mex1-0.0.1.tar` & `protloc_mex1-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 11:54:26.634986 protloc_mex1-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-04-25 08:38:35.000000 protloc_mex1-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1143 2023-04-28 11:54:26.627385 protloc_mex1-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      536 2023-04-26 08:22:56.000000 protloc_mex1-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 11:54:26.594816 protloc_mex1-0.0.1/protloc_mex1/
--rw-rw-rw-   0        0        0    12015 2023-04-25 09:31:12.000000 protloc_mex1-0.0.1/protloc_mex1/AA_count.py
--rw-rw-rw-   0        0        0     7581 2023-04-26 07:57:22.000000 protloc_mex1-0.0.1/protloc_mex1/GO_count.py
--rw-rw-rw-   0        0        0     4597 2023-03-13 09:02:36.000000 protloc_mex1-0.0.1/protloc_mex1/SHAP_conduct.py
--rw-rw-rw-   0        0        0    28400 2023-03-29 08:47:08.000000 protloc_mex1-0.0.1/protloc_mex1/SHAP_plus.py
--rw-rw-rw-   0        0        0       37 2023-04-24 09:24:54.000000 protloc_mex1-0.0.1/protloc_mex1/__init__.py
--rw-rw-rw-   0        0        0    10409 2023-04-25 10:52:28.000000 protloc_mex1-0.0.1/protloc_mex1/classifier_evalute.py
-drwxrwxrwx   0        0        0        0 2023-04-28 11:54:26.627385 protloc_mex1-0.0.1/protloc_mex1.egg-info/
--rw-rw-rw-   0        0        0     1143 2023-04-28 11:54:26.000000 protloc_mex1-0.0.1/protloc_mex1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-04-28 11:54:26.000000 protloc_mex1-0.0.1/protloc_mex1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 11:54:26.000000 protloc_mex1-0.0.1/protloc_mex1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-04-28 11:54:26.000000 protloc_mex1-0.0.1/protloc_mex1.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-28 11:54:26.000000 protloc_mex1-0.0.1/protloc_mex1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      916 2023-04-28 11:53:19.000000 protloc_mex1-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 11:54:26.634986 protloc_mex1-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 14:13:36.417240 protloc_mex1-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-25 08:38:35.000000 protloc_mex1-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1143 2023-04-28 14:13:36.417240 protloc_mex1-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2023-04-26 08:22:56.000000 protloc_mex1-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 14:13:36.387072 protloc_mex1-0.0.2/protloc_mex1/
+-rw-rw-rw-   0        0        0    12015 2023-04-25 09:31:12.000000 protloc_mex1-0.0.2/protloc_mex1/AA_count.py
+-rw-rw-rw-   0        0        0     7581 2023-04-26 07:57:22.000000 protloc_mex1-0.0.2/protloc_mex1/GO_count.py
+-rw-rw-rw-   0        0        0     4597 2023-03-13 09:02:36.000000 protloc_mex1-0.0.2/protloc_mex1/SHAP_conduct.py
+-rw-rw-rw-   0        0        0    28400 2023-03-29 08:47:08.000000 protloc_mex1-0.0.2/protloc_mex1/SHAP_plus.py
+-rw-rw-rw-   0        0        0       37 2023-04-24 09:24:54.000000 protloc_mex1-0.0.2/protloc_mex1/__init__.py
+-rw-rw-rw-   0        0        0    10409 2023-04-25 10:52:28.000000 protloc_mex1-0.0.2/protloc_mex1/classifier_evalute.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:13:36.417240 protloc_mex1-0.0.2/protloc_mex1.egg-info/
+-rw-rw-rw-   0        0        0     1143 2023-04-28 14:13:36.000000 protloc_mex1-0.0.2/protloc_mex1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-04-28 14:13:36.000000 protloc_mex1-0.0.2/protloc_mex1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 14:13:36.000000 protloc_mex1-0.0.2/protloc_mex1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2023-04-28 14:13:36.000000 protloc_mex1-0.0.2/protloc_mex1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-28 14:13:36.000000 protloc_mex1-0.0.2/protloc_mex1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      909 2023-04-28 14:13:08.000000 protloc_mex1-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 14:13:36.417240 protloc_mex1-0.0.2/setup.cfg
```

### Comparing `protloc_mex1-0.0.1/LICENSE.txt` & `protloc_mex1-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.1/PKG-INFO` & `protloc_mex1-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protloc_mex1
-Version: 0.0.1
+Version: 0.0.2
 Summary: ...
 Author-email: Ze Yu Luo <1024226968@qq.com>
 Project-URL: Homepage, https://github.com/yujuan-zhang/ProtLoc-mexl
 Project-URL: Bug Tracker, https://github.com/yujuan-zhang/ProtLoc-mexl/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `protloc_mex1-0.0.1/README.md` & `protloc_mex1-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.1/protloc_mex1/AA_count.py` & `protloc_mex1-0.0.2/protloc_mex1/AA_count.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.1/protloc_mex1/GO_count.py` & `protloc_mex1-0.0.2/protloc_mex1/GO_count.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.1/protloc_mex1/SHAP_conduct.py` & `protloc_mex1-0.0.2/protloc_mex1/SHAP_conduct.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.1/protloc_mex1/SHAP_plus.py` & `protloc_mex1-0.0.2/protloc_mex1/SHAP_plus.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.1/protloc_mex1/classifier_evalute.py` & `protloc_mex1-0.0.2/protloc_mex1/classifier_evalute.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.1/protloc_mex1.egg-info/PKG-INFO` & `protloc_mex1-0.0.2/protloc_mex1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protloc-mex1
-Version: 0.0.1
+Version: 0.0.2
 Summary: ...
 Author-email: Ze Yu Luo <1024226968@qq.com>
 Project-URL: Homepage, https://github.com/yujuan-zhang/ProtLoc-mexl
 Project-URL: Bug Tracker, https://github.com/yujuan-zhang/ProtLoc-mexl/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `protloc_mex1-0.0.1/pyproject.toml` & `protloc_mex1-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "protloc_mex1"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ze Yu Luo", email="1024226968@qq.com" },
 ]
 description = "..."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -16,20 +16,20 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
         "biopython~=1.79",
-        "numpy~=1.20.3",
-        "pandas~=1.4.1",
-        "scikit-learn~=1.0.2",
-        "seaborn~=0.11.2",
-        "matplotlib~=3.5.1",
+        "numpy>=1.20.3",
+        "pandas>=1.4.1",
+        "seaborn>=0.11.2",
+        "matplotlib>=3.5.1",
+        "scikit-learn",
         "shap~=0.41.0",
-        "gensim~=4.2.0"
+        "gensim>=4.2.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/yujuan-zhang/ProtLoc-mexl"
 "Bug Tracker" = "https://github.com/yujuan-zhang/ProtLoc-mexl/issues"
```


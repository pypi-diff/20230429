# Comparing `tmp/cdk8s-operator-0.1.96.tar.gz` & `tmp/cdk8s-operator-0.1.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-operator-0.1.96.tar", last modified: Fri Apr 28 00:30:09 2023, max compression
+gzip compressed data, was "cdk8s-operator-0.1.97.tar", last modified: Sat Apr 29 00:28:42 2023, max compression
```

## Comparing `cdk8s-operator-0.1.96.tar` & `cdk8s-operator-0.1.97.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:30:09.040801 cdk8s-operator-0.1.96/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-28 00:29:57.000000 cdk8s-operator-0.1.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 00:29:57.000000 cdk8s-operator-0.1.96/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-28 00:30:09.040801 cdk8s-operator-0.1.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-28 00:29:57.000000 cdk8s-operator-0.1.96/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-28 00:29:57.000000 cdk8s-operator-0.1.96/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 00:30:09.040801 cdk8s-operator-0.1.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-28 00:29:57.000000 cdk8s-operator-0.1.96/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:30:09.036801 cdk8s-operator-0.1.96/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:30:09.040801 cdk8s-operator-0.1.96/src/cdk8s_operator/
--rw-r--r--   0 runner    (1001) docker     (123)    18320 2023-04-28 00:29:57.000000 cdk8s-operator-0.1.96/src/cdk8s_operator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:30:09.040801 cdk8s-operator-0.1.96/src/cdk8s_operator/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-28 00:29:57.000000 cdk8s-operator-0.1.96/src/cdk8s_operator/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:30:09.040801 cdk8s-operator-0.1.96/src/cdk8s_operator/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-28 00:29:57.000000 cdk8s-operator-0.1.96/src/cdk8s_operator/_jsii/bin/cdk8s-server
--rw-r--r--   0 runner    (1001) docker     (123)   123591 2023-04-28 00:29:57.000000 cdk8s-operator-0.1.96/src/cdk8s_operator/_jsii/cdk8s-operator@0.1.96.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:29:57.000000 cdk8s-operator-0.1.96/src/cdk8s_operator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:30:09.040801 cdk8s-operator-0.1.96/src/cdk8s_operator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-28 00:30:09.000000 cdk8s-operator-0.1.96/src/cdk8s_operator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-28 00:30:09.000000 cdk8s-operator-0.1.96/src/cdk8s_operator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:30:09.000000 cdk8s-operator-0.1.96/src/cdk8s_operator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 00:30:09.000000 cdk8s-operator-0.1.96/src/cdk8s_operator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 00:30:09.000000 cdk8s-operator-0.1.96/src/cdk8s_operator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:28:42.241809 cdk8s-operator-0.1.97/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-29 00:28:29.000000 cdk8s-operator-0.1.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-29 00:28:29.000000 cdk8s-operator-0.1.97/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-29 00:28:42.241809 cdk8s-operator-0.1.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-29 00:28:29.000000 cdk8s-operator-0.1.97/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-29 00:28:29.000000 cdk8s-operator-0.1.97/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 00:28:42.241809 cdk8s-operator-0.1.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-29 00:28:29.000000 cdk8s-operator-0.1.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:28:42.237809 cdk8s-operator-0.1.97/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:28:42.241809 cdk8s-operator-0.1.97/src/cdk8s_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)    18320 2023-04-29 00:28:29.000000 cdk8s-operator-0.1.97/src/cdk8s_operator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:28:42.241809 cdk8s-operator-0.1.97/src/cdk8s_operator/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-29 00:28:29.000000 cdk8s-operator-0.1.97/src/cdk8s_operator/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:28:42.241809 cdk8s-operator-0.1.97/src/cdk8s_operator/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-29 00:28:29.000000 cdk8s-operator-0.1.97/src/cdk8s_operator/_jsii/bin/cdk8s-server
+-rw-r--r--   0 runner    (1001) docker     (123)   123588 2023-04-29 00:28:29.000000 cdk8s-operator-0.1.97/src/cdk8s_operator/_jsii/cdk8s-operator@0.1.97.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:28:29.000000 cdk8s-operator-0.1.97/src/cdk8s_operator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:28:42.241809 cdk8s-operator-0.1.97/src/cdk8s_operator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-29 00:28:42.000000 cdk8s-operator-0.1.97/src/cdk8s_operator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-29 00:28:42.000000 cdk8s-operator-0.1.97/src/cdk8s_operator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:28:42.000000 cdk8s-operator-0.1.97/src/cdk8s_operator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-29 00:28:42.000000 cdk8s-operator-0.1.97/src/cdk8s_operator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-29 00:28:42.000000 cdk8s-operator-0.1.97/src/cdk8s_operator.egg-info/top_level.txt
```

### Comparing `cdk8s-operator-0.1.96/LICENSE` & `cdk8s-operator-0.1.97/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-operator-0.1.96/PKG-INFO` & `cdk8s-operator-0.1.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-operator
-Version: 0.1.96
+Version: 0.1.97
 Summary: Create Kubernetes CRD Operators using CDK8s Constructs
 Home-page: https://github.com/cdk8s-team/cdk8s-operator.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-operator.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-operator-0.1.96/README.md` & `cdk8s-operator-0.1.97/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-operator-0.1.96/setup.py` & `cdk8s-operator-0.1.97/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-operator",
-    "version": "0.1.96",
+    "version": "0.1.97",
     "description": "Create Kubernetes CRD Operators using CDK8s Constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-operator.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk8s_operator",
         "cdk8s_operator._jsii"
     ],
     "package_data": {
         "cdk8s_operator._jsii": [
-            "cdk8s-operator@0.1.96.jsii.tgz"
+            "cdk8s-operator@0.1.97.jsii.tgz"
         ],
         "cdk8s_operator": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk8s-operator-0.1.96/src/cdk8s_operator/__init__.py` & `cdk8s-operator-0.1.97/src/cdk8s_operator/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-operator-0.1.96/src/cdk8s_operator.egg-info/PKG-INFO` & `cdk8s-operator-0.1.97/src/cdk8s_operator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-operator
-Version: 0.1.96
+Version: 0.1.97
 Summary: Create Kubernetes CRD Operators using CDK8s Constructs
 Home-page: https://github.com/cdk8s-team/cdk8s-operator.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-operator.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```


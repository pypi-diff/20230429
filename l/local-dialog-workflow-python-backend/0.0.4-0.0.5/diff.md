# Comparing `tmp/local-dialog-workflow-python-backend-0.0.4.tar.gz` & `tmp/local-dialog-workflow-python-backend-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local-dialog-workflow-python-backend-0.0.4.tar", last modified: Fri Apr 28 23:14:52 2023, max compression
+gzip compressed data, was "local-dialog-workflow-python-backend-0.0.5.tar", last modified: Fri Apr 28 23:19:56 2023, max compression
```

## Comparing `local-dialog-workflow-python-backend-0.0.4.tar` & `local-dialog-workflow-python-backend-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:14:52.221615 local-dialog-workflow-python-backend-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-28 23:14:52.221615 local-dialog-workflow-python-backend-0.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:14:52.221615 local-dialog-workflow-python-backend-0.0.4/dialog_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    19852 2023-04-28 23:14:41.000000 local-dialog-workflow-python-backend-0.0.4/dialog_workflow/Act.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-28 23:14:41.000000 local-dialog-workflow-python-backend-0.0.4/dialog_workflow/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-28 23:14:41.000000 local-dialog-workflow-python-backend-0.0.4/dialog_workflow/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-28 23:14:41.000000 local-dialog-workflow-python-backend-0.0.4/dialog_workflow/TablesAsObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 23:14:41.000000 local-dialog-workflow-python-backend-0.0.4/dialog_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-28 23:14:41.000000 local-dialog-workflow-python-backend-0.0.4/dialog_workflow/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-04-28 23:14:41.000000 local-dialog-workflow-python-backend-0.0.4/dialog_workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:14:52.221615 local-dialog-workflow-python-backend-0.0.4/local_dialog_workflow_python_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-28 23:14:52.000000 local-dialog-workflow-python-backend-0.0.4/local_dialog_workflow_python_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-28 23:14:52.000000 local-dialog-workflow-python-backend-0.0.4/local_dialog_workflow_python_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:14:52.000000 local-dialog-workflow-python-backend-0.0.4/local_dialog_workflow_python_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 23:14:52.000000 local-dialog-workflow-python-backend-0.0.4/local_dialog_workflow_python_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-28 23:14:41.000000 local-dialog-workflow-python-backend-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:14:52.221615 local-dialog-workflow-python-backend-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-28 23:14:41.000000 local-dialog-workflow-python-backend-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:19:56.826454 local-dialog-workflow-python-backend-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-28 23:19:56.826454 local-dialog-workflow-python-backend-0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:19:56.826454 local-dialog-workflow-python-backend-0.0.5/dialog_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    19852 2023-04-28 23:19:44.000000 local-dialog-workflow-python-backend-0.0.5/dialog_workflow/Act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-28 23:19:44.000000 local-dialog-workflow-python-backend-0.0.5/dialog_workflow/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-28 23:19:44.000000 local-dialog-workflow-python-backend-0.0.5/dialog_workflow/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-28 23:19:44.000000 local-dialog-workflow-python-backend-0.0.5/dialog_workflow/TablesAsObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 23:19:44.000000 local-dialog-workflow-python-backend-0.0.5/dialog_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-28 23:19:44.000000 local-dialog-workflow-python-backend-0.0.5/dialog_workflow/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-04-28 23:19:44.000000 local-dialog-workflow-python-backend-0.0.5/dialog_workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:19:56.826454 local-dialog-workflow-python-backend-0.0.5/local_dialog_workflow_python_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-28 23:19:56.000000 local-dialog-workflow-python-backend-0.0.5/local_dialog_workflow_python_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-28 23:19:56.000000 local-dialog-workflow-python-backend-0.0.5/local_dialog_workflow_python_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:19:56.000000 local-dialog-workflow-python-backend-0.0.5/local_dialog_workflow_python_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 23:19:56.000000 local-dialog-workflow-python-backend-0.0.5/local_dialog_workflow_python_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-28 23:19:44.000000 local-dialog-workflow-python-backend-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:19:56.826454 local-dialog-workflow-python-backend-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-28 23:19:44.000000 local-dialog-workflow-python-backend-0.0.5/setup.py
```

### Comparing `local-dialog-workflow-python-backend-0.0.4/dialog_workflow/Act.py` & `local-dialog-workflow-python-backend-0.0.5/dialog_workflow/Act.py`

 * *Files identical despite different names*

### Comparing `local-dialog-workflow-python-backend-0.0.4/dialog_workflow/Constants.py` & `local-dialog-workflow-python-backend-0.0.5/dialog_workflow/Constants.py`

 * *Files identical despite different names*

### Comparing `local-dialog-workflow-python-backend-0.0.4/dialog_workflow/DialogWorkflow.py` & `local-dialog-workflow-python-backend-0.0.5/dialog_workflow/DialogWorkflow.py`

 * *Files identical despite different names*

### Comparing `local-dialog-workflow-python-backend-0.0.4/dialog_workflow/TablesAsObjects.py` & `local-dialog-workflow-python-backend-0.0.5/dialog_workflow/TablesAsObjects.py`

 * *Files identical despite different names*

### Comparing `local-dialog-workflow-python-backend-0.0.4/dialog_workflow/test.py` & `local-dialog-workflow-python-backend-0.0.5/dialog_workflow/test.py`

 * *Files identical despite different names*

### Comparing `local-dialog-workflow-python-backend-0.0.4/dialog_workflow/utils.py` & `local-dialog-workflow-python-backend-0.0.5/dialog_workflow/utils.py`

 * *Files identical despite different names*

### Comparing `local-dialog-workflow-python-backend-0.0.4/setup.py` & `local-dialog-workflow-python-backend-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='local-dialog-workflow-python-backend',  
-     version='0.0.4',
+     version='0.0.5',
      author="Circles",
      author_email="info@circle.life",
      description="PyPI Package for dialog workflow",
      long_description="This is a package for running the dialog workflow",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```


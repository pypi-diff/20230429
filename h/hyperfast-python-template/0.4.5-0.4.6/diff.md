# Comparing `tmp/hyperfast_python_template-0.4.5.tar.gz` & `tmp/hyperfast_python_template-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfast_python_template-0.4.5.tar", max compression
+gzip compressed data, was "hyperfast_python_template-0.4.6.tar", max compression
```

## Comparing `hyperfast_python_template-0.4.5.tar` & `hyperfast_python_template-0.4.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-04-28 11:17:50.029489 hyperfast_python_template-0.4.5/LICENSE
--rw-r--r--   0        0        0     1991 2023-04-28 11:17:50.029489 hyperfast_python_template-0.4.5/README.md
--rw-r--r--   0        0        0     2968 2023-04-28 11:18:08.973772 hyperfast_python_template-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      323 2023-04-28 11:17:50.033489 hyperfast_python_template-0.4.5/src/hyperfastpy/__cli__.py
--rw-r--r--   0        0        0      135 2023-04-28 11:17:50.033489 hyperfast_python_template-0.4.5/src/hyperfastpy/__init__.py
--rw-r--r--   0        0        0       22 2023-04-28 11:18:08.917771 hyperfast_python_template-0.4.5/src/hyperfastpy/_version.py
--rw-r--r--   0        0        0      272 2023-04-28 11:18:08.917771 hyperfast_python_template-0.4.5/src/hyperfastpy/conf/about/__init__.yaml
--rw-r--r--   0        0        0      243 2023-04-28 11:17:50.033489 hyperfast_python_template-0.4.5/src/hyperfastpy/project.toml
--rw-r--r--   0        0        0        0 2023-04-28 11:17:50.033489 hyperfast_python_template-0.4.5/src/hyperfastpy/py.typed
--rw-r--r--   0        0        0      242 2023-04-28 11:17:50.033489 hyperfast_python_template-0.4.5/src/hyperfastpy/pyproject.toml
--rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 hyperfast_python_template-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-29 10:14:38.487161 hyperfast_python_template-0.4.6/LICENSE
+-rw-r--r--   0        0        0     2573 2023-04-29 10:14:38.487161 hyperfast_python_template-0.4.6/README.md
+-rw-r--r--   0        0        0     2968 2023-04-29 10:14:55.363051 hyperfast_python_template-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0      323 2023-04-29 10:14:38.491161 hyperfast_python_template-0.4.6/src/hyperfastpy/__cli__.py
+-rw-r--r--   0        0        0      135 2023-04-29 10:14:38.491161 hyperfast_python_template-0.4.6/src/hyperfastpy/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-29 10:14:55.315051 hyperfast_python_template-0.4.6/src/hyperfastpy/_version.py
+-rw-r--r--   0        0        0      272 2023-04-29 10:14:55.315051 hyperfast_python_template-0.4.6/src/hyperfastpy/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      243 2023-04-29 10:14:38.491161 hyperfast_python_template-0.4.6/src/hyperfastpy/project.toml
+-rw-r--r--   0        0        0        0 2023-04-29 10:14:38.491161 hyperfast_python_template-0.4.6/src/hyperfastpy/py.typed
+-rw-r--r--   0        0        0      242 2023-04-29 10:14:38.491161 hyperfast_python_template-0.4.6/src/hyperfastpy/pyproject.toml
+-rw-r--r--   0        0        0     3239 1970-01-01 00:00:00.000000 hyperfast_python_template-0.4.6/PKG-INFO
```

### Comparing `hyperfast_python_template-0.4.5/LICENSE` & `hyperfast_python_template-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.4.5/pyproject.toml` & `hyperfast_python_template-0.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperfast-python-template"
-version = "0.4.5"
+version = "0.4.6"
 description = "A python template that helps you jump start your project"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyperfast-python.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyperfast-python-template"
 readme = "README.md"
 packages = [{ include = "hyperfastpy", from = "src" }]
```


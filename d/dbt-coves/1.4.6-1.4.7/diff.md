# Comparing `tmp/dbt_coves-1.4.6.tar.gz` & `tmp/dbt_coves-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_coves-1.4.6.tar", max compression
+gzip compressed data, was "dbt_coves-1.4.7.tar", max compression
```

## Comparing `dbt_coves-1.4.6.tar` & `dbt_coves-1.4.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    11357 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/LICENSE
--rw-r--r--   0        0        0    21434 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/README.md
--rw-r--r--   0        0        0       22 2023-04-17 20:45:54.736232 dbt_coves-1.4.6/dbt_coves/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/config/__init__.py
--rw-r--r--   0        0        0     9689 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/config/config.py
--rw-r--r--   0        0        0        0 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/core/__init__.py
--rw-r--r--   0        0        0      650 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/core/exceptions.py
--rw-r--r--   0        0        0     4914 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/core/main.py
--rw-r--r--   0        0        0        0 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/__init__.py
--rw-r--r--   0        0        0     2956 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/base.py
--rw-r--r--   0        0        0     4996 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/dbt/main.py
--rw-r--r--   0        0        0        0 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/extract/__init__.py
--rw-r--r--   0        0        0    11765 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/extract/airbyte.py
--rw-r--r--   0        0        0      475 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/extract/base.py
--rw-r--r--   0        0        0     4512 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/extract/fivetran.py
--rw-r--r--   0        0        0      963 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/extract/main.py
--rw-r--r--   0        0        0        0 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/generate/__init__.py
--rw-r--r--   0        0        0    18472 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/generate/base.py
--rw-r--r--   0        0        0     1520 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/generate/main.py
--rw-r--r--   0        0        0    10562 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/generate/metadata.py
--rw-r--r--   0        0        0     8880 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/generate/properties.py
--rw-r--r--   0        0        0    13956 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/generate/sources.py
--rw-r--r--   0        0        0     2653 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/generate/templates.py
--rw-r--r--   0        0        0        0 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/load/__init__.py
--rw-r--r--   0        0        0    22617 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/load/airbyte.py
--rw-r--r--   0        0        0     2153 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/load/base.py
--rw-r--r--   0        0        0    17204 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/load/fivetran.py
--rw-r--r--   0        0        0      946 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/load/main.py
--rw-r--r--   0        0        0        0 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/setup/__init__.py
--rw-r--r--   0        0        0     1744 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/setup/all.py
--rw-r--r--   0        0        0     4215 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/setup/dbt.py
--rw-r--r--   0        0        0     6689 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/setup/git.py
--rw-r--r--   0        0        0     1183 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/setup/main.py
--rw-r--r--   0        0        0    10142 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/setup/ssh.py
--rw-r--r--   0        0        0      685 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/tasks/setup/utils.py
--rw-r--r--   0        0        0      255 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/templates/model_props.yml
--rw-r--r--   0        0        0      214 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/templates/source_props.yml
--rw-r--r--   0        0        0     1201 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/templates/staging_model.sql
--rw-r--r--   0        0        0      495 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/templates/staging_model_props.yml
--rw-r--r--   0        0        0        0 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/ui/__init__.py
--rw-r--r--   0        0        0     1202 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/ui/traceback.py
--rw-r--r--   0        0        0        0 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/utils/__init__.py
--rw-r--r--   0        0        0     4608 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/utils/airbyte_api.py
--rw-r--r--   0        0        0    12118 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/utils/api_caller.py
--rw-r--r--   0        0        0    13863 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/utils/flags.py
--rw-r--r--   0        0        0     1132 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/utils/jinja.py
--rw-r--r--   0        0        0      785 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/utils/log.py
--rw-r--r--   0        0        0      791 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/utils/shell.py
--rw-r--r--   0        0        0     1010 2023-04-17 20:45:07.863387 dbt_coves-1.4.6/dbt_coves/utils/yaml.py
--rw-r--r--   0        0        0     3520 2023-04-17 20:45:54.736232 dbt_coves-1.4.6/pyproject.toml
--rw-r--r--   0        0        0    23417 1970-01-01 00:00:00.000000 dbt_coves-1.4.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/LICENSE
+-rw-r--r--   0        0        0    21719 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/README.md
+-rw-r--r--   0        0        0       22 2023-04-28 23:05:18.171683 dbt_coves-1.4.7/dbt_coves/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/config/__init__.py
+-rw-r--r--   0        0        0     9689 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/config/config.py
+-rw-r--r--   0        0        0        0 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/core/__init__.py
+-rw-r--r--   0        0        0      650 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/core/exceptions.py
+-rw-r--r--   0        0        0     4914 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/core/main.py
+-rw-r--r--   0        0        0        0 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/tasks/__init__.py
+-rw-r--r--   0        0        0     2956 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/tasks/base.py
+-rw-r--r--   0        0        0     4994 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/tasks/dbt/main.py
+-rw-r--r--   0        0        0        0 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/tasks/extract/__init__.py
+-rw-r--r--   0        0        0    11765 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/tasks/extract/airbyte.py
+-rw-r--r--   0        0        0      475 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/tasks/extract/base.py
+-rw-r--r--   0        0        0     4512 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/tasks/extract/fivetran.py
+-rw-r--r--   0        0        0      963 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/tasks/extract/main.py
+-rw-r--r--   0        0        0        0 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/tasks/generate/__init__.py
+-rw-r--r--   0        0        0    18472 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/tasks/generate/base.py
+-rw-r--r--   0        0        0     1520 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/tasks/generate/main.py
+-rw-r--r--   0        0        0    10562 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/tasks/generate/metadata.py
+-rw-r--r--   0        0        0     8880 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/tasks/generate/properties.py
+-rw-r--r--   0        0        0    13956 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/tasks/generate/sources.py
+-rw-r--r--   0        0        0     2653 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/tasks/generate/templates.py
+-rw-r--r--   0        0        0        0 2023-04-28 23:04:32.031608 dbt_coves-1.4.7/dbt_coves/tasks/load/__init__.py
+-rw-r--r--   0        0        0    22617 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/tasks/load/airbyte.py
+-rw-r--r--   0        0        0     2153 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/tasks/load/base.py
+-rw-r--r--   0        0        0    17204 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/tasks/load/fivetran.py
+-rw-r--r--   0        0        0      946 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/tasks/load/main.py
+-rw-r--r--   0        0        0        0 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/tasks/setup/__init__.py
+-rw-r--r--   0        0        0     1744 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/tasks/setup/all.py
+-rw-r--r--   0        0        0     4215 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/tasks/setup/dbt.py
+-rw-r--r--   0        0        0     6689 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/tasks/setup/git.py
+-rw-r--r--   0        0        0     1183 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/tasks/setup/main.py
+-rw-r--r--   0        0        0    10142 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/tasks/setup/ssh.py
+-rw-r--r--   0        0        0      685 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/tasks/setup/utils.py
+-rw-r--r--   0        0        0      255 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/templates/model_props.yml
+-rw-r--r--   0        0        0      214 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/templates/source_props.yml
+-rw-r--r--   0        0        0     1201 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/templates/staging_model.sql
+-rw-r--r--   0        0        0      495 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/templates/staging_model_props.yml
+-rw-r--r--   0        0        0        0 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/ui/__init__.py
+-rw-r--r--   0        0        0     1202 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/ui/traceback.py
+-rw-r--r--   0        0        0        0 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/utils/__init__.py
+-rw-r--r--   0        0        0     4608 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/utils/airbyte_api.py
+-rw-r--r--   0        0        0    12118 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/utils/api_caller.py
+-rw-r--r--   0        0        0    13863 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/utils/flags.py
+-rw-r--r--   0        0        0     1132 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/utils/jinja.py
+-rw-r--r--   0        0        0      785 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/utils/log.py
+-rw-r--r--   0        0        0      791 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/utils/shell.py
+-rw-r--r--   0        0        0     1010 2023-04-28 23:04:32.035608 dbt_coves-1.4.7/dbt_coves/utils/yaml.py
+-rw-r--r--   0        0        0     3520 2023-04-28 23:05:18.171683 dbt_coves-1.4.7/pyproject.toml
+-rw-r--r--   0        0        0    23702 1970-01-01 00:00:00.000000 dbt_coves-1.4.7/PKG-INFO
```

### Comparing `dbt_coves-1.4.6/LICENSE` & `dbt_coves-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/README.md` & `dbt_coves-1.4.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 # dbt-coves
 
-[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/datacoves/dbt-coves/graphs/commit-activity)
-[![PyPI version
-fury.io](https://badge.fury.io/py/dbt-coves.svg)](https://pypi.python.org/pypi/dbt-coves/)
-[![Code
-Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
-[![Imports:
-isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-[![Imports:
-python](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)
-[![Build](https://github.com/datacoves/dbt-coves/actions/workflows/main_ci.yml/badge.svg)](https://github.com/datacoves/dbt-coves/actions/workflows/main_ci.yml/badge.svg)
+## Sponsor
 
-<!-- [![codecov](https://codecov.io/gh/datacoves/dbt-coves/branch/main/graph/badge.svg?token=JB0E0LZDW1)](https://codecov.io/gh/datacoves/dbt-coves) -->
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="images/datacoves-dark.png">
+  <img alt="Datacoves" src="images/datacoves-light.png" width="150">
+</picture>
 
-[![Maintainability](https://api.codeclimate.com/v1/badges/1e6a887de605ef8e0eca/maintainability)](https://codeclimate.com/github/datacoves/dbt-coves/maintainability)
-[![Downloads](https://pepy.tech/badge/dbt-coves)](https://pepy.tech/project/dbt-coves)
+The turnkey analytics stack, find out more at [Datacoves.com](https://datacoves.com/).
 
 ## What is dbt-coves?
 
 dbt-coves is a CLI tool that automates certain tasks for [dbt](https://www.getdbt.com), making life simpler for the dbt user.
 
 dbt-coves generates dbt sources, staging models and property(yml) files by analyzing information from the data warehouse and creating the necessary files (sql and yml).
 
@@ -576,7 +569,25 @@
 - Bruno Antonellini -- [Datacoves](https://datacoves.com/)
 
 # About
 
 Learn more about [Datacoves](https://datacoves.com).
 
 ⚠️ **dbt-coves is still in development, make sure to test it for your dbt project version and DW before using in production and please submit any issues you find. We also welcome any contributions from the community**
+
+# Metrics
+
+[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/datacoves/dbt-coves/graphs/commit-activity)
+[![PyPI version
+fury.io](https://badge.fury.io/py/dbt-coves.svg)](https://pypi.python.org/pypi/dbt-coves/)
+[![Code
+Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+[![Imports:
+isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Imports:
+python](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)
+[![Build](https://github.com/datacoves/dbt-coves/actions/workflows/main_ci.yml/badge.svg)](https://github.com/datacoves/dbt-coves/actions/workflows/main_ci.yml/badge.svg)
+
+<!-- [![codecov](https://codecov.io/gh/datacoves/dbt-coves/branch/main/graph/badge.svg?token=JB0E0LZDW1)](https://codecov.io/gh/datacoves/dbt-coves) -->
+
+[![Maintainability](https://api.codeclimate.com/v1/badges/1e6a887de605ef8e0eca/maintainability)](https://codeclimate.com/github/datacoves/dbt-coves/maintainability)
+[![Downloads](https://pepy.tech/badge/dbt-coves)](https://pepy.tech/project/dbt-coves)
```

### Comparing `dbt_coves-1.4.6/dbt_coves/config/config.py` & `dbt_coves-1.4.7/dbt_coves/config/config.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/core/exceptions.py` & `dbt_coves-1.4.7/dbt_coves/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/core/main.py` & `dbt_coves-1.4.7/dbt_coves/core/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/base.py` & `dbt_coves-1.4.7/dbt_coves/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/dbt/main.py` & `dbt_coves-1.4.7/dbt_coves/tasks/dbt/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
     @classmethod
     def register_parser(cls, sub_parsers, base_subparser):
         ext_subparser = sub_parsers.add_parser(
             "dbt",
             parents=[base_subparser],
             # help="Run dbt on an isolated environment",
-            help="""Use this command to run dbt commands on special environments 
-            such as Airflow, or CI workers. When a read-write copy needs to be 
+            help="""Use this command to run dbt commands on special environments
+            such as Airflow, or CI workers. When a read-write copy needs to be
             created, its path can be found in DBT_COVES__CLONE_PATH.""",
         )
         ext_subparser.set_defaults(cls=cls, which="dbt")
         cls.arg_parser = ext_subparser
         ext_subparser.add_argument(
             "--virtualenv",
             type=str,
```

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/extract/airbyte.py` & `dbt_coves-1.4.7/dbt_coves/tasks/extract/airbyte.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/extract/fivetran.py` & `dbt_coves-1.4.7/dbt_coves/tasks/extract/fivetran.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/extract/main.py` & `dbt_coves-1.4.7/dbt_coves/tasks/extract/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/generate/base.py` & `dbt_coves-1.4.7/dbt_coves/tasks/generate/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/generate/main.py` & `dbt_coves-1.4.7/dbt_coves/tasks/generate/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/generate/metadata.py` & `dbt_coves-1.4.7/dbt_coves/tasks/generate/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/generate/properties.py` & `dbt_coves-1.4.7/dbt_coves/tasks/generate/properties.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/generate/sources.py` & `dbt_coves-1.4.7/dbt_coves/tasks/generate/sources.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/generate/templates.py` & `dbt_coves-1.4.7/dbt_coves/tasks/generate/templates.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/load/airbyte.py` & `dbt_coves-1.4.7/dbt_coves/tasks/load/airbyte.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/load/base.py` & `dbt_coves-1.4.7/dbt_coves/tasks/load/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/load/fivetran.py` & `dbt_coves-1.4.7/dbt_coves/tasks/load/fivetran.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/load/main.py` & `dbt_coves-1.4.7/dbt_coves/tasks/load/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/setup/all.py` & `dbt_coves-1.4.7/dbt_coves/tasks/setup/all.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/setup/dbt.py` & `dbt_coves-1.4.7/dbt_coves/tasks/setup/dbt.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/setup/git.py` & `dbt_coves-1.4.7/dbt_coves/tasks/setup/git.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/setup/main.py` & `dbt_coves-1.4.7/dbt_coves/tasks/setup/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/setup/ssh.py` & `dbt_coves-1.4.7/dbt_coves/tasks/setup/ssh.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/tasks/setup/utils.py` & `dbt_coves-1.4.7/dbt_coves/tasks/setup/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/templates/staging_model.sql` & `dbt_coves-1.4.7/dbt_coves/templates/staging_model.sql`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/ui/traceback.py` & `dbt_coves-1.4.7/dbt_coves/ui/traceback.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/utils/airbyte_api.py` & `dbt_coves-1.4.7/dbt_coves/utils/airbyte_api.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/utils/api_caller.py` & `dbt_coves-1.4.7/dbt_coves/utils/api_caller.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/utils/flags.py` & `dbt_coves-1.4.7/dbt_coves/utils/flags.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/utils/jinja.py` & `dbt_coves-1.4.7/dbt_coves/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/utils/log.py` & `dbt_coves-1.4.7/dbt_coves/utils/log.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/utils/shell.py` & `dbt_coves-1.4.7/dbt_coves/utils/shell.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/dbt_coves/utils/yaml.py` & `dbt_coves-1.4.7/dbt_coves/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.6/pyproject.toml` & `dbt_coves-1.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt_coves"
-version = "1.4.6"
+version = "1.4.7"
 description = "CLI tool for dbt users adopting analytics engineering best practices."
 authors = ["Datacoves <hello@datacoves.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Information Technology",
```

### Comparing `dbt_coves-1.4.6/PKG-INFO` & `dbt_coves-1.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-coves
-Version: 1.4.6
+Version: 1.4.7
 Summary: CLI tool for dbt users adopting analytics engineering best practices.
 Home-page: https://datacoves.com
 License: Apache 2.0
 Keywords: data engineering,analytics engineering,dbt,ETL,data modelling
 Author: Datacoves
 Author-email: hello@datacoves.com
 Requires-Python: >=3.7.2,<3.11
@@ -41,29 +41,22 @@
 Requires-Dist: yamlloader (>=1.0.0,<2.0.0)
 Project-URL: Documentation, https://datacoves.gitbook.io/dbt-coves/
 Project-URL: Repository, https://github.com/datacoves/dbt-coves
 Description-Content-Type: text/markdown
 
 # dbt-coves
 
-[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/datacoves/dbt-coves/graphs/commit-activity)
-[![PyPI version
-fury.io](https://badge.fury.io/py/dbt-coves.svg)](https://pypi.python.org/pypi/dbt-coves/)
-[![Code
-Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
-[![Imports:
-isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-[![Imports:
-python](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)
-[![Build](https://github.com/datacoves/dbt-coves/actions/workflows/main_ci.yml/badge.svg)](https://github.com/datacoves/dbt-coves/actions/workflows/main_ci.yml/badge.svg)
+## Sponsor
 
-<!-- [![codecov](https://codecov.io/gh/datacoves/dbt-coves/branch/main/graph/badge.svg?token=JB0E0LZDW1)](https://codecov.io/gh/datacoves/dbt-coves) -->
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="images/datacoves-dark.png">
+  <img alt="Datacoves" src="images/datacoves-light.png" width="150">
+</picture>
 
-[![Maintainability](https://api.codeclimate.com/v1/badges/1e6a887de605ef8e0eca/maintainability)](https://codeclimate.com/github/datacoves/dbt-coves/maintainability)
-[![Downloads](https://pepy.tech/badge/dbt-coves)](https://pepy.tech/project/dbt-coves)
+The turnkey analytics stack, find out more at [Datacoves.com](https://datacoves.com/).
 
 ## What is dbt-coves?
 
 dbt-coves is a CLI tool that automates certain tasks for [dbt](https://www.getdbt.com), making life simpler for the dbt user.
 
 dbt-coves generates dbt sources, staging models and property(yml) files by analyzing information from the data warehouse and creating the necessary files (sql and yml).
 
@@ -622,7 +615,25 @@
 
 # About
 
 Learn more about [Datacoves](https://datacoves.com).
 
 ⚠️ **dbt-coves is still in development, make sure to test it for your dbt project version and DW before using in production and please submit any issues you find. We also welcome any contributions from the community**
 
+# Metrics
+
+[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/datacoves/dbt-coves/graphs/commit-activity)
+[![PyPI version
+fury.io](https://badge.fury.io/py/dbt-coves.svg)](https://pypi.python.org/pypi/dbt-coves/)
+[![Code
+Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+[![Imports:
+isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Imports:
+python](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)
+[![Build](https://github.com/datacoves/dbt-coves/actions/workflows/main_ci.yml/badge.svg)](https://github.com/datacoves/dbt-coves/actions/workflows/main_ci.yml/badge.svg)
+
+<!-- [![codecov](https://codecov.io/gh/datacoves/dbt-coves/branch/main/graph/badge.svg?token=JB0E0LZDW1)](https://codecov.io/gh/datacoves/dbt-coves) -->
+
+[![Maintainability](https://api.codeclimate.com/v1/badges/1e6a887de605ef8e0eca/maintainability)](https://codeclimate.com/github/datacoves/dbt-coves/maintainability)
+[![Downloads](https://pepy.tech/badge/dbt-coves)](https://pepy.tech/project/dbt-coves)
+
```


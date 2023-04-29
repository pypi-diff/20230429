# Comparing `tmp/poetry_plugin_compose-0.1.0.tar.gz` & `tmp/poetry_plugin_compose-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_compose-0.1.0.tar", max compression
+gzip compressed data, was "poetry_plugin_compose-0.1.1.tar", max compression
```

## Comparing `poetry_plugin_compose-0.1.0.tar` & `poetry_plugin_compose-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     3043 2023-04-29 11:07:43.469899 poetry_plugin_compose-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-09 22:22:48.699457 poetry_plugin_compose-0.1.0/poetry_plugin_compose/__init__.py
--rw-r--r--   0        0        0     2499 2023-04-29 11:00:13.820256 poetry_plugin_compose-0.1.0/poetry_plugin_compose/compose_command.py
--rw-r--r--   0        0        0     1355 2023-04-29 11:00:13.820507 poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_command_list.py
--rw-r--r--   0        0        0        0 2023-04-09 23:11:55.579203 poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/__init__.py
--rw-r--r--   0        0        0     1131 2023-04-29 11:00:13.821165 poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_add_command.py
--rw-r--r--   0        0        0      848 2023-04-29 11:00:13.821406 poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_build_command.py
--rw-r--r--   0        0        0      862 2023-04-29 11:00:13.821638 poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_check_command.py
--rw-r--r--   0        0        0     3651 2023-04-29 11:00:13.821968 poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_command.py
--rw-r--r--   0        0        0      218 2023-04-29 11:00:13.822441 poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_command_utils.py
--rw-r--r--   0        0        0      907 2023-04-29 11:00:13.822846 poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_install_command.py
--rw-r--r--   0        0        0      840 2023-04-29 11:00:13.823132 poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_lock_command.py
--rw-r--r--   0        0        0      864 2023-04-29 11:00:13.823612 poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_publish_command.py
--rw-r--r--   0        0        0     1167 2023-04-29 11:00:13.823871 poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_remove_command.py
--rw-r--r--   0        0        0      903 2023-04-29 11:00:13.824363 poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_run_command.py
--rw-r--r--   0        0        0      897 2023-04-29 11:00:13.824612 poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_update_command.py
--rw-r--r--   0        0        0      905 2023-04-29 11:00:13.824969 poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/dependency_order_command.py
--rw-r--r--   0        0        0     1271 2023-04-29 11:00:13.825347 poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/package_filter.py
--rw-r--r--   0        0        0      515 2023-04-29 11:00:13.825956 poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/sub_command_runner.py
--rw-r--r--   0        0        0        0 2023-04-29 11:00:13.826113 poetry_plugin_compose-0.1.0/poetry_plugin_compose/packages/__init__.py
--rw-r--r--   0        0        0     1087 2023-04-29 11:00:13.827657 poetry_plugin_compose-0.1.0/poetry_plugin_compose/packages/build_dependency_graph.py
--rw-r--r--   0        0        0     1015 2023-04-29 11:00:13.828651 poetry_plugin_compose-0.1.0/poetry_plugin_compose/packages/discover_packages.py
--rw-r--r--   0        0        0      821 2023-04-29 11:00:13.833010 poetry_plugin_compose-0.1.0/poetry_plugin_compose/packages/get_package_dependencies.py
--rw-r--r--   0        0        0      436 2023-04-29 11:00:13.834611 poetry_plugin_compose-0.1.0/poetry_plugin_compose/packages/get_package_descriptor.py
--rw-r--r--   0        0        0      124 2023-04-29 11:00:13.835880 poetry_plugin_compose-0.1.0/poetry_plugin_compose/packages/sub_package_contains.py
--rw-r--r--   0        0        0      318 2023-04-29 11:00:13.836803 poetry_plugin_compose-0.1.0/poetry_plugin_compose/packages/sub_package_has_dependency.py
--rw-r--r--   0        0        0      947 2023-04-10 19:09:13.625373 poetry_plugin_compose-0.1.0/poetry_plugin_compose/plugin.py
--rw-r--r--   0        0        0        0 2023-04-29 11:00:13.836957 poetry_plugin_compose-0.1.0/poetry_plugin_compose/toposort/__init__.py
--rw-r--r--   0        0        0     3567 2023-04-29 11:00:13.838018 poetry_plugin_compose-0.1.0/poetry_plugin_compose/toposort/graph.py
--rw-r--r--   0        0        0      698 2023-04-29 11:00:13.838965 poetry_plugin_compose-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3517 1970-01-01 00:00:00.000000 poetry_plugin_compose-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3065 2023-04-29 11:44:07.318735 poetry_plugin_compose-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 22:22:48.699457 poetry_plugin_compose-0.1.1/poetry_plugin_compose/__init__.py
+-rw-r--r--   0        0        0     2499 2023-04-29 11:00:13.820256 poetry_plugin_compose-0.1.1/poetry_plugin_compose/compose_command.py
+-rw-r--r--   0        0        0     1355 2023-04-29 11:00:13.820507 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_command_list.py
+-rw-r--r--   0        0        0        0 2023-04-09 23:11:55.579203 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/__init__.py
+-rw-r--r--   0        0        0     1122 2023-04-29 11:43:36.561486 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_add_command.py
+-rw-r--r--   0        0        0      848 2023-04-29 11:00:13.821406 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_build_command.py
+-rw-r--r--   0        0        0      862 2023-04-29 11:00:13.821638 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_check_command.py
+-rw-r--r--   0        0        0     3673 2023-04-29 11:28:13.459985 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_command.py
+-rw-r--r--   0        0        0      218 2023-04-29 11:00:13.822441 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_command_utils.py
+-rw-r--r--   0        0        0      907 2023-04-29 11:00:13.822846 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_install_command.py
+-rw-r--r--   0        0        0      840 2023-04-29 11:00:13.823132 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_lock_command.py
+-rw-r--r--   0        0        0      864 2023-04-29 11:00:13.823612 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_publish_command.py
+-rw-r--r--   0        0        0     1167 2023-04-29 11:00:13.823871 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_remove_command.py
+-rw-r--r--   0        0        0      903 2023-04-29 11:00:13.824363 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_run_command.py
+-rw-r--r--   0        0        0      897 2023-04-29 11:00:13.824612 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_update_command.py
+-rw-r--r--   0        0        0      905 2023-04-29 11:00:13.824969 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/dependency_order_command.py
+-rw-r--r--   0        0        0     1271 2023-04-29 11:00:13.825347 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/package_filter.py
+-rw-r--r--   0        0        0      515 2023-04-29 11:00:13.825956 poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/sub_command_runner.py
+-rw-r--r--   0        0        0        0 2023-04-29 11:00:13.826113 poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/__init__.py
+-rw-r--r--   0        0        0     1087 2023-04-29 11:00:13.827657 poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/build_dependency_graph.py
+-rw-r--r--   0        0        0     1015 2023-04-29 11:00:13.828651 poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/discover_packages.py
+-rw-r--r--   0        0        0      821 2023-04-29 11:00:13.833010 poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/get_package_dependencies.py
+-rw-r--r--   0        0        0      436 2023-04-29 11:00:13.834611 poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/get_package_descriptor.py
+-rw-r--r--   0        0        0      124 2023-04-29 11:00:13.835880 poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/sub_package_contains.py
+-rw-r--r--   0        0        0      318 2023-04-29 11:00:13.836803 poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/sub_package_has_dependency.py
+-rw-r--r--   0        0        0      947 2023-04-10 19:09:13.625373 poetry_plugin_compose-0.1.1/poetry_plugin_compose/plugin.py
+-rw-r--r--   0        0        0        0 2023-04-29 11:00:13.836957 poetry_plugin_compose-0.1.1/poetry_plugin_compose/toposort/__init__.py
+-rw-r--r--   0        0        0     3567 2023-04-29 11:00:13.838018 poetry_plugin_compose-0.1.1/poetry_plugin_compose/toposort/graph.py
+-rw-r--r--   0        0        0      698 2023-04-29 11:44:12.545215 poetry_plugin_compose-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 poetry_plugin_compose-0.1.1/PKG-INFO
```

### Comparing `poetry_plugin_compose-0.1.0/README.md` & `poetry_plugin_compose-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,14 @@
 ### Documentation
 
 Documentation is mostly generated from the command themselves.
 Also the root readme of the project serves as the welcome page of the docs.
 In order to sync the doc runs the following
 ```
 cd scripts
-poetry run python generate_doc.py
+poetry compose run -d scripts -- python generate_doc.py
 ```
 
 Then to deploy
 ```
 poetry compose run -d doc -- mkdocs gh-deploy
 ```
```

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/compose_command.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/compose_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_command_list.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_command_list.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_add_command.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_add_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,11 +21,11 @@
         {
             "description": "add flake8 as a dev dependency to every subpackage where black is installed",
             "output": "poetry compose install -i black -- flake8 --group-dev",
         },
     ]
 
     def run(self, args, package):
-        self._write_line("Running add " + join(args) + " in " + " in " + package)
+        self._write_line("Running add " + join(args) + " in " + package)
         return_code = run_sub_command_sync(["poetry", "add", *args], package)
         self.report_output(return_code)
         return return_code
```

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_build_command.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_build_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_check_command.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_check_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_command.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,17 @@
     def _write_line(self, line: str):
         self.io.write_line("<info>" + self.get_log_intro() + line + "</info>")
 
     def _write_success(self):
         self.io.write_line("<comment>" + self.get_log_intro() + " success</comment>")
 
     def _write_error(self, error):
-        self.io.write_line("<error>" + self.get_log_intro() + error + " failure</error>")
+        self.io.write_line(
+            "<error>" + self.get_log_intro() + error + " failure</error>"
+        )
 
     def _write_failure(self):
         self._write_error("failure")
 
     def _get_package_filters(self, options):
         filters = []
         if options.contains:
```

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_install_command.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_install_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_lock_command.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_lock_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_publish_command.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_publish_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_remove_command.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_remove_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_run_command.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_run_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/composed_update_command.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/composed_update_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/dependency_order_command.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/dependency_order_command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/package_filter.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/package_filter.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/composed_commands/sub_command_runner.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/composed_commands/sub_command_runner.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/packages/build_dependency_graph.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/build_dependency_graph.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/packages/discover_packages.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/discover_packages.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/packages/get_package_dependencies.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/packages/get_package_dependencies.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/plugin.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.0/poetry_plugin_compose/toposort/graph.py` & `poetry_plugin_compose-0.1.1/poetry_plugin_compose/toposort/graph.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_compose-0.1.0/pyproject.toml` & `poetry_plugin_compose-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-compose"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Max <maximilienlarue@gmail.com>"]
 readme = "README.md"
 packages = [{include = "poetry_plugin_compose"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `poetry_plugin_compose-0.1.0/PKG-INFO` & `poetry_plugin_compose-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-compose
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Max
 Author-email: maximilienlarue@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -144,14 +144,14 @@
 ### Documentation
 
 Documentation is mostly generated from the command themselves.
 Also the root readme of the project serves as the welcome page of the docs.
 In order to sync the doc runs the following
 ```
 cd scripts
-poetry run python generate_doc.py
+poetry compose run -d scripts -- python generate_doc.py
 ```
 
 Then to deploy
 ```
 poetry compose run -d doc -- mkdocs gh-deploy
 ```
```


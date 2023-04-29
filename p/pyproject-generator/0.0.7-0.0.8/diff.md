# Comparing `tmp/pyproject-generator-0.0.7.tar.gz` & `tmp/pyproject-generator-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-generator-0.0.7.tar", last modified: Sat Apr 29 20:44:28 2023, max compression
+gzip compressed data, was "pyproject-generator-0.0.8.tar", last modified: Sat Apr 29 21:03:23 2023, max compression
```

## Comparing `pyproject-generator-0.0.7.tar` & `pyproject-generator-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 20:44:28.594156 pyproject-generator-0.0.7/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-29 20:44:28.594668 pyproject-generator-0.0.7/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1439 2023-04-19 15:24:26.000000 pyproject-generator-0.0.7/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-19 15:24:26.000000 pyproject-generator-0.0.7/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-04-29 20:44:28.595706 pyproject-generator-0.0.7/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 20:44:28.576781 pyproject-generator-0.0.7/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 20:44:28.582136 pyproject-generator-0.0.7/src/pyproject/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-19 15:24:27.000000 pyproject-generator-0.0.7/src/pyproject/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-29 20:44:17.000000 pyproject-generator-0.0.7/src/pyproject/__version__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2714 2023-04-29 20:40:26.000000 pyproject-generator-0.0.7/src/pyproject/cli.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 20:44:28.584067 pyproject-generator-0.0.7/src/pyproject/config/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.0.7/src/pyproject/config/config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:07.000000 pyproject-generator-0.0.7/src/pyproject/config/default_config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)     8217 2023-04-29 20:43:01.000000 pyproject-generator-0.0.7/src/pyproject/project_builder.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 20:44:28.588838 pyproject-generator-0.0.7/src/pyproject/templates/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.0.7/src/pyproject/templates/gitignore.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.0.7/src/pyproject/templates/pyproject.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.0.7/src/pyproject/templates/readme.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      578 2023-04-14 17:03:04.000000 pyproject-generator-0.0.7/src/pyproject/templates/setup.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.0.7/src/pyproject/templates/tests.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.0.7/src/pyproject/templates/tox.template
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 20:44:28.592894 pyproject-generator-0.0.7/src/pyproject_generator.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-29 20:44:28.000000 pyproject-generator-0.0.7/src/pyproject_generator.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)      766 2023-04-29 20:44:28.000000 pyproject-generator-0.0.7/src/pyproject_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-29 20:44:28.000000 pyproject-generator-0.0.7/src/pyproject_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-29 20:44:28.000000 pyproject-generator-0.0.7/src/pyproject_generator.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-04-29 20:44:28.000000 pyproject-generator-0.0.7/src/pyproject_generator.egg-info/requires.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-29 20:44:28.000000 pyproject-generator-0.0.7/src/pyproject_generator.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 20:44:28.593621 pyproject-generator-0.0.7/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.0.7/tests/test_pyproject.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 21:03:23.894517 pyproject-generator-0.0.8/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-29 21:03:23.894679 pyproject-generator-0.0.8/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1439 2023-04-19 15:24:26.000000 pyproject-generator-0.0.8/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-19 15:24:26.000000 pyproject-generator-0.0.8/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-04-29 21:03:23.895766 pyproject-generator-0.0.8/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 21:03:23.869879 pyproject-generator-0.0.8/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 21:03:23.875511 pyproject-generator-0.0.8/src/pyproject/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-19 15:24:27.000000 pyproject-generator-0.0.8/src/pyproject/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-29 21:03:04.000000 pyproject-generator-0.0.8/src/pyproject/__version__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2714 2023-04-29 20:40:26.000000 pyproject-generator-0.0.8/src/pyproject/cli.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 21:03:23.877802 pyproject-generator-0.0.8/src/pyproject/config/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.0.8/src/pyproject/config/config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:07.000000 pyproject-generator-0.0.8/src/pyproject/config/default_config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     8205 2023-04-29 21:01:17.000000 pyproject-generator-0.0.8/src/pyproject/project_builder.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 21:03:23.885381 pyproject-generator-0.0.8/src/pyproject/templates/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.0.8/src/pyproject/templates/gitignore.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.0.8/src/pyproject/templates/pyproject.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.0.8/src/pyproject/templates/readme.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      578 2023-04-14 17:03:04.000000 pyproject-generator-0.0.8/src/pyproject/templates/setup.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.0.8/src/pyproject/templates/tests.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.0.8/src/pyproject/templates/tox.template
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 21:03:23.893024 pyproject-generator-0.0.8/src/pyproject_generator.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-29 21:03:23.000000 pyproject-generator-0.0.8/src/pyproject_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      766 2023-04-29 21:03:23.000000 pyproject-generator-0.0.8/src/pyproject_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-29 21:03:23.000000 pyproject-generator-0.0.8/src/pyproject_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-29 21:03:23.000000 pyproject-generator-0.0.8/src/pyproject_generator.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-04-29 21:03:23.000000 pyproject-generator-0.0.8/src/pyproject_generator.egg-info/requires.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-29 21:03:23.000000 pyproject-generator-0.0.8/src/pyproject_generator.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 21:03:23.894188 pyproject-generator-0.0.8/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.0.8/tests/test_pyproject.py
```

### Comparing `pyproject-generator-0.0.7/PKG-INFO` & `pyproject-generator-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.0.7
+Version: 0.0.8
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.0.7/README.md` & `pyproject-generator-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.7/setup.cfg` & `pyproject-generator-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.7/src/pyproject/cli.py` & `pyproject-generator-0.0.8/src/pyproject/cli.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.7/src/pyproject/project_builder.py` & `pyproject-generator-0.0.8/src/pyproject/project_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,17 +207,16 @@
                 config["set_dependencies"], sep=","
             )
 
         for k in ("remove_dependencies", "add_dependencies"):
             config[k] = self._parse_arg_to_set(config[k], sep=",")
 
         config["dependencies"] = (
-            config["dependencies"]
-            | config["add_dependencies"] - config["remove_dependencies"]
-        )
+            config["dependencies"] | config["add_dependencies"]
+        ) - config["remove_dependencies"]
 
         merged_config = {}
         for k, v in saved_config.items():
             if config[k] is None:
                 merged_config[k] = v
             else:
                 merged_config[k] = config[k]
```

### Comparing `pyproject-generator-0.0.7/src/pyproject/templates/gitignore.template` & `pyproject-generator-0.0.8/src/pyproject/templates/gitignore.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.7/src/pyproject/templates/setup.template` & `pyproject-generator-0.0.8/src/pyproject/templates/setup.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.7/src/pyproject/templates/tests.template` & `pyproject-generator-0.0.8/src/pyproject/templates/tests.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.7/src/pyproject_generator.egg-info/PKG-INFO` & `pyproject-generator-0.0.8/src/pyproject_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.0.7
+Version: 0.0.8
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.0.7/src/pyproject_generator.egg-info/SOURCES.txt` & `pyproject-generator-0.0.8/src/pyproject_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*


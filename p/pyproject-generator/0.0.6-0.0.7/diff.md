# Comparing `tmp/pyproject-generator-0.0.6.tar.gz` & `tmp/pyproject-generator-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-generator-0.0.6.tar", last modified: Fri Apr 28 19:30:56 2023, max compression
+gzip compressed data, was "pyproject-generator-0.0.7.tar", last modified: Sat Apr 29 20:44:28 2023, max compression
```

## Comparing `pyproject-generator-0.0.6.tar` & `pyproject-generator-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:30:56.416182 pyproject-generator-0.0.6/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-28 19:30:56.416361 pyproject-generator-0.0.6/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1439 2023-04-19 15:24:26.000000 pyproject-generator-0.0.6/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-19 15:24:26.000000 pyproject-generator-0.0.6/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      834 2023-04-28 19:30:56.417212 pyproject-generator-0.0.6/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:30:56.394662 pyproject-generator-0.0.6/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:30:56.399744 pyproject-generator-0.0.6/src/pyproject/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-19 15:24:27.000000 pyproject-generator-0.0.6/src/pyproject/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-28 19:30:35.000000 pyproject-generator-0.0.6/src/pyproject/__version__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2570 2023-04-28 19:13:46.000000 pyproject-generator-0.0.6/src/pyproject/cli.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:30:56.402617 pyproject-generator-0.0.6/src/pyproject/config/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.0.6/src/pyproject/config/config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:07.000000 pyproject-generator-0.0.6/src/pyproject/config/default_config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)     7502 2023-04-28 19:30:05.000000 pyproject-generator-0.0.6/src/pyproject/project_builder.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:30:56.411728 pyproject-generator-0.0.6/src/pyproject/templates/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.0.6/src/pyproject/templates/gitignore.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.0.6/src/pyproject/templates/pyproject.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.0.6/src/pyproject/templates/readme.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      578 2023-04-14 17:03:04.000000 pyproject-generator-0.0.6/src/pyproject/templates/setup.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.0.6/src/pyproject/templates/tests.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.0.6/src/pyproject/templates/tox.template
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:30:56.415347 pyproject-generator-0.0.6/src/pyproject_generator.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-28 19:30:56.000000 pyproject-generator-0.0.6/src/pyproject_generator.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)      720 2023-04-28 19:30:56.000000 pyproject-generator-0.0.6/src/pyproject_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-28 19:30:56.000000 pyproject-generator-0.0.6/src/pyproject_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-28 19:30:56.000000 pyproject-generator-0.0.6/src/pyproject_generator.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-28 19:30:56.000000 pyproject-generator-0.0.6/src/pyproject_generator.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:30:56.415897 pyproject-generator-0.0.6/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.0.6/tests/test_pyproject.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 20:44:28.594156 pyproject-generator-0.0.7/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-29 20:44:28.594668 pyproject-generator-0.0.7/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1439 2023-04-19 15:24:26.000000 pyproject-generator-0.0.7/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-19 15:24:26.000000 pyproject-generator-0.0.7/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-04-29 20:44:28.595706 pyproject-generator-0.0.7/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 20:44:28.576781 pyproject-generator-0.0.7/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 20:44:28.582136 pyproject-generator-0.0.7/src/pyproject/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-19 15:24:27.000000 pyproject-generator-0.0.7/src/pyproject/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-29 20:44:17.000000 pyproject-generator-0.0.7/src/pyproject/__version__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2714 2023-04-29 20:40:26.000000 pyproject-generator-0.0.7/src/pyproject/cli.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 20:44:28.584067 pyproject-generator-0.0.7/src/pyproject/config/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.0.7/src/pyproject/config/config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:07.000000 pyproject-generator-0.0.7/src/pyproject/config/default_config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     8217 2023-04-29 20:43:01.000000 pyproject-generator-0.0.7/src/pyproject/project_builder.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 20:44:28.588838 pyproject-generator-0.0.7/src/pyproject/templates/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.0.7/src/pyproject/templates/gitignore.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.0.7/src/pyproject/templates/pyproject.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.0.7/src/pyproject/templates/readme.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      578 2023-04-14 17:03:04.000000 pyproject-generator-0.0.7/src/pyproject/templates/setup.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.0.7/src/pyproject/templates/tests.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.0.7/src/pyproject/templates/tox.template
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 20:44:28.592894 pyproject-generator-0.0.7/src/pyproject_generator.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-29 20:44:28.000000 pyproject-generator-0.0.7/src/pyproject_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      766 2023-04-29 20:44:28.000000 pyproject-generator-0.0.7/src/pyproject_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-29 20:44:28.000000 pyproject-generator-0.0.7/src/pyproject_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-29 20:44:28.000000 pyproject-generator-0.0.7/src/pyproject_generator.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-04-29 20:44:28.000000 pyproject-generator-0.0.7/src/pyproject_generator.egg-info/requires.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-29 20:44:28.000000 pyproject-generator-0.0.7/src/pyproject_generator.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-29 20:44:28.593621 pyproject-generator-0.0.7/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.0.7/tests/test_pyproject.py
```

### Comparing `pyproject-generator-0.0.6/PKG-INFO` & `pyproject-generator-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.0.6
+Version: 0.0.7
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.0.6/README.md` & `pyproject-generator-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.6/setup.cfg` & `pyproject-generator-0.0.7/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
+install_requires = 
+	platformdirs
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 pyproject = 
 	py.typed
```

### Comparing `pyproject-generator-0.0.6/src/pyproject/cli.py` & `pyproject-generator-0.0.7/src/pyproject/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,17 @@
     parser.add_argument(
         "--remove_dependencies",
         type=str,
         help=(
             "Remove dependencies to always download. Pass in a comma delimited string."
         ),
     )
+    parser.add_argument(
+        "--show", required=False, action="store_true", help="Show the current config"
+    )
 
     parser.add_argument(
         "-v",
         "--version",
         action="version",
         version="%(prog)s {version}".format(version=__version__),
         help="Displays package version",
@@ -71,14 +74,15 @@
         "github_url": args.github_url,
         "author": args.author,
         "email": args.email,
         "set_dependencies": args.set_dependencies,
         "add_dependencies": args.add_dependencies,
         "remove_dependencies": args.remove_dependencies,
         "reset_config": args.reset_config,
+        "show": args.show,
     }
 
     builder = ProjectBuilder(config=config)
     builder.dispatch(action=args.action, project_name=args.project_name)
 
 
 if __name__ == "__main__":
```

### Comparing `pyproject-generator-0.0.6/src/pyproject/project_builder.py` & `pyproject-generator-0.0.7/src/pyproject/project_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # Imports
 
 import os
 import json
 from pathlib import Path
+import pprint
 import re
 import shutil
 import subprocess
 import string
 from types import SimpleNamespace
 from typing import Literal, Optional, Union
 import venv
 
+import platformdirs
+
 Action = Literal["init", "upload", "config"]
 PathLike = Union[Path, str]
 
 BASE_PATH = Path(__file__).resolve().parents[0]
 TEMPLATE_PATH = BASE_PATH / "templates"
-CONFIG_PATH = BASE_PATH / "config"
+USER_CONFIG_PATH = platformdirs.user_config_dir(
+    appname="pyproject-generator", appauthor="cangyuanli"
+)
 
 
 class Env(venv.EnvBuilder):
     def __init__(self, *args, **kwargs) -> None:
         self.context = self.get_context()
         super().__init__(*args, **kwargs)
 
@@ -59,32 +64,44 @@
         return subprocess.run(command, check=True, **kwargs)
 
 
 class ProjectBuilder:
     def __init__(
         self,
         template_path: PathLike = TEMPLATE_PATH,
-        config_path: PathLike = CONFIG_PATH,
+        user_config_dir: PathLike = USER_CONFIG_PATH,
         config: Optional[dict[str, str]] = None,
     ) -> None:
         self.proj_path = Path().cwd()
 
         self._template_path = Path(template_path)
-        self._config_path = Path(config_path)
+
+        self._user_config_dir = Path(user_config_dir)
+        self._create_config_dir()
         self._config = self._set_config(config)
 
     @staticmethod
     def _validate_project_name(project_name: str) -> None:
         regex = "^([A-Z0-9]|[A-Z0-9][A-Z0-9._-]*[A-Z0-9])$"
         if not bool(re.match(regex, project_name, re.IGNORECASE)):
             raise ValueError(
                 "A valid project name may only contain ASCII letters, numbers, ., -,"
                 " and/or _, and they must begin and end with a letter or number."
             )
 
+    def _create_config_dir(self) -> None:
+        self._user_config_dir.mkdir(exist_ok=True)
+        if not (self._user_config_dir / "config.json").exists():
+            shutil.copy(
+                BASE_PATH / "config/default_config.json",
+                self._user_config_dir / "config.json",
+            )
+
+        return None
+
     def _fill_in_templates(self, project_name: str) -> dict[str, str]:
         config = self._config
         d = {
             "PACKAGE": project_name,
             "PYPI_USERNAME": config["pypi_username"],
             "PYPI_PASSWORD": config["pypi_password"],
             "GITHUB_URL": config["github_url"],
@@ -154,15 +171,20 @@
             venv_builder.run_bin(["pip", "install", dep])
 
         # Create requirements_dev file
         reqs = venv_builder.run_bin(["pip", "freeze"], capture_output=True)
         (proj_path / "requirements_dev.txt").write_bytes(reqs.stdout)
 
     def _parse_config_file(self, filename: PathLike) -> dict:
-        with open(self._config_path / filename) as f:
+        if filename == "default_config.json":
+            path = BASE_PATH / "config/default_config.json"
+        else:
+            path = self._user_config_dir / filename
+
+        with open(path) as f:
             config: dict = json.load(f)
 
         return config
 
     @staticmethod
     def _parse_arg_to_set(string: Optional[str], sep: str) -> set[str]:
         if string is None:
@@ -196,20 +218,23 @@
         merged_config = {}
         for k, v in saved_config.items():
             if config[k] is None:
                 merged_config[k] = v
             else:
                 merged_config[k] = config[k]
 
+        if config["show"]:
+            pprint.pprint(merged_config)
+
         return merged_config
 
     def config(self):
         config = self._config
         config["dependencies"] = list(config["dependencies"])
-        with open(self._config_path / "config.json", "w") as f:
+        with open(self._user_config_dir / "config.json", "w") as f:
             json.dump(config, f, indent=4)
 
     def upload(self):
         username = self._config["pypi_username"]
         password = self._config["pypi_password"]
 
         env = Env()
```

### Comparing `pyproject-generator-0.0.6/src/pyproject/templates/gitignore.template` & `pyproject-generator-0.0.7/src/pyproject/templates/gitignore.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.6/src/pyproject/templates/setup.template` & `pyproject-generator-0.0.7/src/pyproject/templates/setup.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.6/src/pyproject/templates/tests.template` & `pyproject-generator-0.0.7/src/pyproject/templates/tests.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.6/src/pyproject_generator.egg-info/PKG-INFO` & `pyproject-generator-0.0.7/src/pyproject_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.0.6
+Version: 0.0.7
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.0.6/src/pyproject_generator.egg-info/SOURCES.txt` & `pyproject-generator-0.0.7/src/pyproject_generator.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,9 +13,10 @@
 src/pyproject/templates/setup.template
 src/pyproject/templates/tests.template
 src/pyproject/templates/tox.template
 src/pyproject_generator.egg-info/PKG-INFO
 src/pyproject_generator.egg-info/SOURCES.txt
 src/pyproject_generator.egg-info/dependency_links.txt
 src/pyproject_generator.egg-info/entry_points.txt
+src/pyproject_generator.egg-info/requires.txt
 src/pyproject_generator.egg-info/top_level.txt
 tests/test_pyproject.py
```


# Comparing `tmp/devcontainer_manager-1.3.1.tar.gz` & `tmp/devcontainer_manager-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devcontainer_manager-1.3.1.tar", last modified: Sun Apr  9 12:59:38 2023, max compression
+gzip compressed data, was "devcontainer_manager-1.3.2.tar", last modified: Sat Apr 29 12:56:29 2023, max compression
```

## Comparing `devcontainer_manager-1.3.1.tar` & `devcontainer_manager-1.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:59:38.320182 devcontainer_manager-1.3.1/
--rw-rw-r--   0 root         (0) root         (0)     1061 2022-01-06 15:44:11.000000 devcontainer_manager-1.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      108 2023-04-09 12:27:48.000000 devcontainer_manager-1.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6285 2023-04-09 12:59:38.320182 devcontainer_manager-1.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5996 2023-04-09 12:55:25.000000 devcontainer_manager-1.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:59:38.320182 devcontainer_manager-1.3.1/devcontainer_manager/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-09 12:54:42.000000 devcontainer_manager-1.3.1/devcontainer_manager/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/devcontainer_manager/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-04-09 12:25:48.000000 devcontainer_manager-1.3.1/devcontainer_manager/alias.py
--rw-r--r--   0 root         (0) root         (0)     3872 2023-04-09 12:14:41.000000 devcontainer_manager-1.3.1/devcontainer_manager/base_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:59:38.320182 devcontainer_manager-1.3.1/devcontainer_manager/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/devcontainer_manager/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1896 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/devcontainer_manager/cli/alias.py
--rw-r--r--   0 root         (0) root         (0)     4303 2023-04-09 12:51:56.000000 devcontainer_manager-1.3.1/devcontainer_manager/cli/cli.py
--rw-r--r--   0 root         (0) root         (0)     8497 2023-04-09 12:52:29.000000 devcontainer_manager-1.3.1/devcontainer_manager/config.py
--rw-r--r--   0 root         (0) root         (0)      336 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/devcontainer_manager/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1673 2022-12-11 13:13:18.000000 devcontainer_manager-1.3.1/devcontainer_manager/global_config.py
--rw-r--r--   0 root         (0) root         (0)      412 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/devcontainer_manager/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:59:38.316182 devcontainer_manager-1.3.1/devcontainer_manager/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:59:38.316182 devcontainer_manager-1.3.1/devcontainer_manager/templates/{{ cookiecutter.project_path }}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:59:38.320182 devcontainer_manager-1.3.1/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/
--rw-rw-r--   0 root         (0) root         (0)      233 2022-01-07 00:28:25.000000 devcontainer_manager-1.3.1/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/build.sh
--rw-r--r--   0 root         (0) root         (0)      240 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1662 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.json
--rw-r--r--   0 root         (0) root         (0)     1834 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/devcontainer_manager/types.py
--rw-r--r--   0 root         (0) root         (0)     1203 2022-11-13 22:15:55.000000 devcontainer_manager-1.3.1/devcontainer_manager/util.py
--rw-r--r--   0 root         (0) root         (0)     2691 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/devcontainer_manager/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:59:38.320182 devcontainer_manager-1.3.1/devcontainer_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6285 2023-04-09 12:59:38.000000 devcontainer_manager-1.3.1/devcontainer_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1061 2023-04-09 12:59:38.000000 devcontainer_manager-1.3.1/devcontainer_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 12:59:38.000000 devcontainer_manager-1.3.1/devcontainer_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-09 12:59:38.000000 devcontainer_manager-1.3.1/devcontainer_manager.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      121 2023-04-09 12:59:38.000000 devcontainer_manager-1.3.1/devcontainer_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-09 12:59:38.000000 devcontainer_manager-1.3.1/devcontainer_manager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      408 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 12:59:38.320182 devcontainer_manager-1.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      991 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 12:56:29.194977 devcontainer_manager-1.3.2/
+-rw-rw-r--   0 root         (0) root         (0)     1061 2022-01-06 15:44:11.000000 devcontainer_manager-1.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      108 2023-04-09 12:27:48.000000 devcontainer_manager-1.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6285 2023-04-29 12:56:29.194977 devcontainer_manager-1.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5996 2023-04-09 12:55:25.000000 devcontainer_manager-1.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 12:56:29.190977 devcontainer_manager-1.3.2/devcontainer_manager/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-29 12:55:34.000000 devcontainer_manager-1.3.2/devcontainer_manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/devcontainer_manager/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-04-09 12:25:48.000000 devcontainer_manager-1.3.2/devcontainer_manager/alias.py
+-rw-r--r--   0 root         (0) root         (0)     3872 2023-04-09 12:14:41.000000 devcontainer_manager-1.3.2/devcontainer_manager/base_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 12:56:29.190977 devcontainer_manager-1.3.2/devcontainer_manager/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/devcontainer_manager/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2023-04-29 12:53:32.000000 devcontainer_manager-1.3.2/devcontainer_manager/cli/alias.py
+-rw-r--r--   0 root         (0) root         (0)     4369 2023-04-29 12:44:30.000000 devcontainer_manager-1.3.2/devcontainer_manager/cli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     8497 2023-04-09 12:52:29.000000 devcontainer_manager-1.3.2/devcontainer_manager/config.py
+-rw-r--r--   0 root         (0) root         (0)      336 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/devcontainer_manager/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2022-12-11 13:13:18.000000 devcontainer_manager-1.3.2/devcontainer_manager/global_config.py
+-rw-r--r--   0 root         (0) root         (0)      412 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/devcontainer_manager/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 12:56:29.190977 devcontainer_manager-1.3.2/devcontainer_manager/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 12:56:29.190977 devcontainer_manager-1.3.2/devcontainer_manager/templates/{{ cookiecutter.project_path }}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 12:56:29.190977 devcontainer_manager-1.3.2/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/
+-rw-rw-r--   0 root         (0) root         (0)      233 2022-01-07 00:28:25.000000 devcontainer_manager-1.3.2/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/build.sh
+-rw-r--r--   0 root         (0) root         (0)      240 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1662 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.json
+-rw-r--r--   0 root         (0) root         (0)     1834 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/devcontainer_manager/types.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2022-11-13 22:15:55.000000 devcontainer_manager-1.3.2/devcontainer_manager/util.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/devcontainer_manager/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 12:56:29.190977 devcontainer_manager-1.3.2/devcontainer_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6285 2023-04-29 12:56:29.000000 devcontainer_manager-1.3.2/devcontainer_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-04-29 12:56:29.000000 devcontainer_manager-1.3.2/devcontainer_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 12:56:29.000000 devcontainer_manager-1.3.2/devcontainer_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-29 12:56:29.000000 devcontainer_manager-1.3.2/devcontainer_manager.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-04-29 12:56:29.000000 devcontainer_manager-1.3.2/devcontainer_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-29 12:56:29.000000 devcontainer_manager-1.3.2/devcontainer_manager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 12:56:29.194977 devcontainer_manager-1.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      991 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/setup.py
```

### Comparing `devcontainer_manager-1.3.1/LICENSE` & `devcontainer_manager-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.1/PKG-INFO` & `devcontainer_manager-1.3.2/devcontainer_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: devcontainer_manager
-Version: 1.3.1
+Name: devcontainer-manager
+Version: 1.3.2
 Summary: UNKNOWN
 Home-page: https://github.com/gnox/devcontainer-manager
 Author: gnox
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `devcontainer_manager-1.3.1/README.md` & `devcontainer_manager-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.1/devcontainer_manager/alias.py` & `devcontainer_manager-1.3.2/devcontainer_manager/alias.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.1/devcontainer_manager/base_config.py` & `devcontainer_manager-1.3.2/devcontainer_manager/base_config.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.1/devcontainer_manager/cli/alias.py` & `devcontainer_manager-1.3.2/devcontainer_manager/cli/alias.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,33 +4,36 @@
 import typer
 
 from ..global_config import GlobalConfig
 
 app = typer.Typer()
 
 
-def complete_aliases(ctx: typer.Context, args: List[str], incomplete: str):
-    global_config = GlobalConfig.load()
-    param_aliases = ctx.params.get("alias") or []
-    for alias, path in global_config.load_alias_config().aliases.items():
-        if alias.startswith(incomplete) and alias not in param_aliases:
-            yield (alias, path)
+def complete_aliases(param_name: str = "alias"):
+    def _complete(ctx: typer.Context, args: List[str], incomplete: str):
+        global_config = GlobalConfig.load()
+        param_aliases = ctx.params.get(param_name) or []
+        for alias, path in global_config.load_alias_config().aliases.items():
+            if alias.startswith(incomplete) and alias not in param_aliases:
+                yield (alias, path.as_posix())
+
+    return _complete
 
 
 @app.command()
 def add(alias: str = typer.Argument(...), config_path: str = typer.Argument(...)):
     path = Path(config_path)
     alias_config = GlobalConfig.load().load_alias_config()
     alias_config.aliases[alias] = path.resolve().as_posix()
     alias_config.write_yaml()
 
 
 @app.command()
 def remove(
-    alias: List[str] = typer.Argument(..., shell_complete=complete_aliases),
+    alias: List[str] = typer.Argument(..., autocompletion=complete_aliases("alias")),
 ):
     alias_config = GlobalConfig.load().load_alias_config()
 
     for alias_remove in alias:
         if alias_remove in alias_config.aliases:
             alias_config.aliases.pop(alias_remove)
             alias_config.write_yaml()
```

### Comparing `devcontainer_manager-1.3.1/devcontainer_manager/cli/cli.py` & `devcontainer_manager-1.3.2/devcontainer_manager/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 
 app = typer.Typer()
 app.add_typer(alias.app, name="alias")
 
 
 @app.command()
 def generate(
-    templates: Optional[List[str]] = typer.Argument(None),
+    templates: Optional[List[str]] = typer.Argument(
+        None, autocompletion=alias.complete_aliases("templates")
+    ),
     build: bool = typer.Option(False, "--build", "-b"),
     print_config: bool = typer.Option(False, "--print-config", "--print", "-p"),
 ):
     global_config = GlobalConfig.load(create_if_not_exist=True)
     alias_config = global_config.load_alias_config()
     from_override = not templates
```

### Comparing `devcontainer_manager-1.3.1/devcontainer_manager/config.py` & `devcontainer_manager-1.3.2/devcontainer_manager/config.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.1/devcontainer_manager/global_config.py` & `devcontainer_manager-1.3.2/devcontainer_manager/global_config.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.1/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.json` & `devcontainer_manager-1.3.2/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.1/devcontainer_manager/types.py` & `devcontainer_manager-1.3.2/devcontainer_manager/types.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.1/devcontainer_manager/util.py` & `devcontainer_manager-1.3.2/devcontainer_manager/util.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.1/devcontainer_manager/yaml.py` & `devcontainer_manager-1.3.2/devcontainer_manager/yaml.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.1/devcontainer_manager.egg-info/PKG-INFO` & `devcontainer_manager-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: devcontainer-manager
-Version: 1.3.1
+Name: devcontainer_manager
+Version: 1.3.2
 Summary: UNKNOWN
 Home-page: https://github.com/gnox/devcontainer-manager
 Author: gnox
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `devcontainer_manager-1.3.1/devcontainer_manager.egg-info/SOURCES.txt` & `devcontainer_manager-1.3.2/devcontainer_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.1/setup.py` & `devcontainer_manager-1.3.2/setup.py`

 * *Files identical despite different names*


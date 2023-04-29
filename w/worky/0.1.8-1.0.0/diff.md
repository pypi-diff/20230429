# Comparing `tmp/worky-0.1.8.tar.gz` & `tmp/worky-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worky-0.1.8.tar", max compression
+gzip compressed data, was "worky-1.0.0.tar", max compression
```

## Comparing `worky-0.1.8.tar` & `worky-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    34523 2023-02-16 01:31:29.674033 worky-0.1.8/LICENSE
--rw-r--r--   0        0        0     5026 2023-04-28 13:27:16.829310 worky-0.1.8/README.md
--rw-r--r--   0        0        0      838 2023-04-28 13:26:52.286016 worky-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      119 2023-04-27 14:39:59.061967 worky-0.1.8/worky/__init__.py
--rw-r--r--   0        0        0      121 2023-04-27 14:33:11.629893 worky-0.1.8/worky/__main__.py
--rw-r--r--   0        0        0     3618 2023-04-27 13:11:21.488772 worky-0.1.8/worky/main.py
--rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-0.1.8/worky/models/__init__.py
--rw-r--r--   0        0        0     1759 2023-04-27 14:40:49.885173 worky-0.1.8/worky/models/config_model.py
--rw-r--r--   0        0        0      120 2023-04-27 10:00:41.124836 worky-0.1.8/worky/models/log_level.py
--rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-0.1.8/worky/utils/__init__.py
--rw-r--r--   0        0        0     1242 2023-04-27 12:32:08.612359 worky-0.1.8/worky/utils/logger.py
--rw-r--r--   0        0        0      156 2023-04-27 10:26:48.078234 worky-0.1.8/worky/utils/util.py
--rw-r--r--   0        0        0     5818 1970-01-01 00:00:00.000000 worky-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-02-16 01:31:29.674033 worky-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5367 2023-04-29 17:08:00.469544 worky-1.0.0/README.md
+-rw-r--r--   0        0        0      838 2023-04-29 17:08:59.307270 worky-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-04-27 14:39:59.061967 worky-1.0.0/worky/__init__.py
+-rw-r--r--   0        0        0      121 2023-04-27 14:33:11.629893 worky-1.0.0/worky/__main__.py
+-rw-r--r--   0        0        0     3957 2023-04-29 17:12:04.408256 worky-1.0.0/worky/main.py
+-rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-1.0.0/worky/models/__init__.py
+-rw-r--r--   0        0        0     1759 2023-04-27 14:40:49.885173 worky-1.0.0/worky/models/config_model.py
+-rw-r--r--   0        0        0      120 2023-04-27 10:00:41.124836 worky-1.0.0/worky/models/log_level.py
+-rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-1.0.0/worky/utils/__init__.py
+-rw-r--r--   0        0        0     1242 2023-04-27 12:32:08.612359 worky-1.0.0/worky/utils/logger.py
+-rw-r--r--   0        0        0      156 2023-04-27 10:26:48.078234 worky-1.0.0/worky/utils/util.py
+-rw-r--r--   0        0        0     6159 1970-01-01 00:00:00.000000 worky-1.0.0/PKG-INFO
```

### Comparing `worky-0.1.8/LICENSE` & `worky-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `worky-0.1.8/README.md` & `worky-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,19 +24,22 @@
 ```shell
 yay -S worky
 ```
 
 ## Configuration
 If you prefer a practical way to understand how to worky configuration works, you can take a look at the [examples directory](https://github.com/ZappaBoy/worky/tree/main/examples).
 
-### Worky configuration file - `.worky.toml`
-Worky automatically looks for a `.worky.toml` file in the current directory where is called.
-If it finds one, it will use it to load the workspace, alternatively, you need to specify a configuration file using the `-c` flag followed by the path of the config file.
-If you prefer, you can create a subdirectory named as your project (`project_name`) under the `~/.config/worky/`. Here you can put your `config.toml` file and worky will automatically look for it when you run `worky project_name`.
-For example, if you have a project named `my_project` you can create a `~/.config/worky/my_project/config.toml` file and use `worky my_project` to load the project workspace.
+### Worky configuration file
+There are multiple ways to configure worky:
+ 1. Worky automatically looks for a `.worky.toml` file in the current directory where is called.
+ 2. You can create a `~/.config/worky/{{project_name}}.toml` file and worky will automatically look for it when you run `worky project_name`.
+    For example, if you have a project named `my_project` you can create a `~/.config/worky/my_project/config.toml` file and use `worky my_project` to load the project workspace.
+ 3. You can create a subdirectory named as your project (`project_name`) under the `~/.config/worky/`. Here you can put your `config.toml` file and worky will look for it when you run `worky project_name`.
+    For example, if you have a project named `my_project` you can create a `~/.config/worky/my_project/config.toml` file and use `worky my_project` to load the project workspace.
+ 4. You can specify a configuration file using the `-c` flag followed by the path of the config file (see `worky --help` for more details).
 
 ### Variables
 Variables can be defined in the `[variables]` section of the configuration file. The variable's value is the command to be executed.
 The variables can be used in all the config file except for the steps name.
 The value of the variables used in the step name defines the command that will be executed. See the [steps section](#steps) for more details.
 
 ### Steps
@@ -69,15 +72,15 @@
 You can crate two different steps using variables with the same value. Moreover, this helps to keep the configuration file clean and readable.
 
 ## Usage
 After installing and configured worky, you can use it to load your project workspace simply by running:
 ```shell
 worky  # If you have a .worky.toml file in the current directory
 # or
-worky {{project_name}}  # If you have a config file in ~/.config/worky/{{project_name}}/config.toml
+worky {{project_name}}  # If you have a config file in ~/.config/worky/{{project_name}}/config.toml or ~/.config/worky/{{project_name}}.toml
 # or
 worky -c {{path_to_config_file}}  # Defining a custom config file
 ```
 
 ## For developers
 Install dependencies:
 ```shell
```

### Comparing `worky-0.1.8/pyproject.toml` & `worky-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "worky"
-version = "0.1.8"
+version = "1.0.0"
 description = "Worky is a tool that helps to define and load project workspaces."
 authors = ["ZappaBoy <federico.zappone@justanother.cloud>"]
 maintainers = ["ZappaBoy <federico.zappone@justanother.cloud>"]
 readme = "README.md"
 packages = [{ include = "worky" }]
 homepage = "https://github.com/ZappaBoy/worky"
 repository = "https://github.com/ZappaBoy/worky"
```

### Comparing `worky-0.1.8/worky/main.py` & `worky-1.0.0/worky/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import argparse
 import os.path
 import subprocess
 import sys
 from typing import List
 
+import toml
+
 from worky.models.config_model import Config
 from worky.utils.logger import Logger
 from worky.utils.util import file_type
 
+VERSION = toml.load("pyproject.toml")["tool"]["poetry"]["version"]
 DEFAULT_CONFIG_DIR = os.path.expanduser('~/.config/worky')
 DEFAULT_CONFIG_FILE_NAME = 'config.toml'
 
 
 class Worky:
     config: Config = None
     flags: List[str] = []
@@ -25,14 +28,16 @@
         if args.quiet:
             self.logger.set_log_level(0)
         else:
             self.logger.set_log_level(args.verbose)
         config_file_path = args.config
         if config_file_path is None and args.name is not None:
             config_file_path = os.path.join(DEFAULT_CONFIG_DIR, args.name, DEFAULT_CONFIG_FILE_NAME)
+            if not os.path.exists(config_file_path):
+                config_file_path = os.path.join(DEFAULT_CONFIG_DIR, f'{args.name}.toml')
         if config_file_path is None or not os.path.exists(config_file_path):
             self.logger.error(f'Config file not found: {config_file_path}')
             sys.exit(1)
 
         self.load_config(config_file_path)
         self.flags = args.flags
         self.dry_run = args.dry_run
@@ -51,14 +56,15 @@
                             help='Print the output of the commands without running them')
         parser.add_argument('-v', '--verbose', action='count', default=0,
                             help='Increase verbosity (can be repeated)')
         parser.add_argument('-q', '--quiet', action=argparse.BooleanOptionalAction, default=False, required=False,
                             help='Do not print any output/log')
         parser.add_argument('name', nargs='?', type=str, default=None,
                             help=f'Define the Worky project name stored in {DEFAULT_CONFIG_DIR}')
+        parser.add_argument('--version', action='version', version=f'%(prog)s {VERSION}')
         return parser.parse_args(args)
 
     def load_config(self, config_path: str):
         self.logger.info(f'Loading config from {config_path}')
         self.config = Config(config_path)
 
     def run_steps(self):
@@ -76,13 +82,13 @@
             args = ' '.join(step_args)
             command = f'{step_command} {args}'
             if self.dry_run:
                 dry_run_output += f'{command}\n'
             else:
                 self.run_command(command)
         if self.dry_run:
-            # Print without logger to be sure to print it every time
+            # Print without logger to be sure to print it every time. This ignores quiet option
             print(dry_run_output)
 
     @staticmethod
     def run_command(command: str):
         subprocess.Popen(command, shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
```

### Comparing `worky-0.1.8/worky/models/config_model.py` & `worky-1.0.0/worky/models/config_model.py`

 * *Files identical despite different names*

### Comparing `worky-0.1.8/worky/utils/logger.py` & `worky-1.0.0/worky/utils/logger.py`

 * *Files identical despite different names*

### Comparing `worky-0.1.8/PKG-INFO` & `worky-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worky
-Version: 0.1.8
+Version: 1.0.0
 Summary: Worky is a tool that helps to define and load project workspaces.
 Home-page: https://github.com/ZappaBoy/worky
 Keywords: worky,productivity,workspace,initializer
 Author: ZappaBoy
 Author-email: federico.zappone@justanother.cloud
 Maintainer: ZappaBoy
 Maintainer-email: federico.zappone@justanother.cloud
@@ -44,19 +44,22 @@
 ```shell
 yay -S worky
 ```
 
 ## Configuration
 If you prefer a practical way to understand how to worky configuration works, you can take a look at the [examples directory](https://github.com/ZappaBoy/worky/tree/main/examples).
 
-### Worky configuration file - `.worky.toml`
-Worky automatically looks for a `.worky.toml` file in the current directory where is called.
-If it finds one, it will use it to load the workspace, alternatively, you need to specify a configuration file using the `-c` flag followed by the path of the config file.
-If you prefer, you can create a subdirectory named as your project (`project_name`) under the `~/.config/worky/`. Here you can put your `config.toml` file and worky will automatically look for it when you run `worky project_name`.
-For example, if you have a project named `my_project` you can create a `~/.config/worky/my_project/config.toml` file and use `worky my_project` to load the project workspace.
+### Worky configuration file
+There are multiple ways to configure worky:
+ 1. Worky automatically looks for a `.worky.toml` file in the current directory where is called.
+ 2. You can create a `~/.config/worky/{{project_name}}.toml` file and worky will automatically look for it when you run `worky project_name`.
+    For example, if you have a project named `my_project` you can create a `~/.config/worky/my_project/config.toml` file and use `worky my_project` to load the project workspace.
+ 3. You can create a subdirectory named as your project (`project_name`) under the `~/.config/worky/`. Here you can put your `config.toml` file and worky will look for it when you run `worky project_name`.
+    For example, if you have a project named `my_project` you can create a `~/.config/worky/my_project/config.toml` file and use `worky my_project` to load the project workspace.
+ 4. You can specify a configuration file using the `-c` flag followed by the path of the config file (see `worky --help` for more details).
 
 ### Variables
 Variables can be defined in the `[variables]` section of the configuration file. The variable's value is the command to be executed.
 The variables can be used in all the config file except for the steps name.
 The value of the variables used in the step name defines the command that will be executed. See the [steps section](#steps) for more details.
 
 ### Steps
@@ -89,15 +92,15 @@
 You can crate two different steps using variables with the same value. Moreover, this helps to keep the configuration file clean and readable.
 
 ## Usage
 After installing and configured worky, you can use it to load your project workspace simply by running:
 ```shell
 worky  # If you have a .worky.toml file in the current directory
 # or
-worky {{project_name}}  # If you have a config file in ~/.config/worky/{{project_name}}/config.toml
+worky {{project_name}}  # If you have a config file in ~/.config/worky/{{project_name}}/config.toml or ~/.config/worky/{{project_name}}.toml
 # or
 worky -c {{path_to_config_file}}  # Defining a custom config file
 ```
 
 ## For developers
 Install dependencies:
 ```shell
```


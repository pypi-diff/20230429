# Comparing `tmp/nua-0.5.16.tar.gz` & `tmp/nua-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua-0.5.16.tar", max compression
+gzip compressed data, was "nua-0.5.8.tar", max compression
```

## Comparing `nua-0.5.16.tar` & `nua-0.5.8.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1360 2023-04-29 10:19:10.759617 nua-0.5.16/pyproject.toml
--rw-r--r--   0        0        0     1945 2023-04-29 10:12:42.488342 nua-0.5.16/readme.md
--rw-r--r--   0        0        0        0 2023-01-02 15:45:01.827907 nua-0.5.16/src/nua_cli/__init__.py
--rw-r--r--   0        0        0     2029 2023-04-17 10:11:29.772670 nua-0.5.16/src/nua_cli/client.py
--rw-r--r--   0        0        0        0 2023-02-08 20:21:55.685155 nua-0.5.16/src/nua_cli/commands/__init__.py
--rw-r--r--   0        0        0     1122 2023-04-26 08:44:27.762943 nua-0.5.16/src/nua_cli/commands/_common.py
--rw-r--r--   0        0        0     1010 2023-04-17 10:06:21.226164 nua-0.5.16/src/nua_cli/commands/apps.py
--rw-r--r--   0        0        0      464 2023-04-17 10:06:36.592612 nua-0.5.16/src/nua_cli/commands/backup.py
--rw-r--r--   0        0        0     1522 2023-04-26 08:44:27.763193 nua-0.5.16/src/nua_cli/commands/build.py
--rw-r--r--   0        0        0      963 2023-04-17 18:21:32.441064 nua-0.5.16/src/nua_cli/commands/config.py
--rw-r--r--   0        0        0     1118 2023-04-26 08:44:27.763360 nua-0.5.16/src/nua_cli/commands/deploy.py
--rw-r--r--   0        0        0     1490 2023-04-17 18:21:32.441043 nua-0.5.16/src/nua_cli/commands/env.py
--rw-r--r--   0        0        0      490 2023-04-17 10:09:42.111936 nua-0.5.16/src/nua_cli/commands/help.py
--rw-r--r--   0        0        0     1760 2023-04-26 08:44:27.763585 nua-0.5.16/src/nua_cli/commands/lifecycle.py
--rw-r--r--   0        0        0      823 2023-04-17 10:10:22.613380 nua-0.5.16/src/nua_cli/commands/logs.py
--rw-r--r--   0        0        0      172 2023-04-17 10:10:35.298837 nua-0.5.16/src/nua_cli/commands/main.py
--rw-r--r--   0        0        0     2520 2023-04-17 18:21:32.441152 nua-0.5.16/src/nua_cli/commands/server.py
--rw-r--r--   0        0        0     1345 2023-04-21 16:06:50.165113 nua-0.5.16/src/nua_cli/common.py
--rw-r--r--   0        0        0     1561 2023-04-29 10:06:56.611354 nua-0.5.16/src/nua_cli/main.py
--rw-r--r--   0        0        0      217 2023-04-29 10:07:13.520071 nua-0.5.16/src/nua_cli/version.py
--rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 nua-0.5.16/PKG-INFO
+-rw-r--r--   0        0        0     1318 2023-04-13 09:53:05.626200 nua-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     1994 2023-04-12 10:06:30.438962 nua-0.5.8/readme.md
+-rw-r--r--   0        0        0        0 2023-01-02 15:45:01.827907 nua-0.5.8/src/nua_cli/__init__.py
+-rw-r--r--   0        0        0     6506 2023-04-13 06:22:42.919805 nua-0.5.8/src/nua_cli/base.py
+-rw-r--r--   0        0        0     2032 2023-04-12 14:30:30.888082 nua-0.5.8/src/nua_cli/client.py
+-rw-r--r--   0        0        0      313 2023-04-11 21:17:25.332899 nua-0.5.8/src/nua_cli/colors.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:21:55.685155 nua-0.5.8/src/nua_cli/commands/__init__.py
+-rw-r--r--   0        0        0     1024 2023-04-12 12:47:44.478176 nua-0.5.8/src/nua_cli/commands/apps.py
+-rw-r--r--   0        0        0      478 2023-04-12 10:07:34.002570 nua-0.5.8/src/nua_cli/commands/backup.py
+-rw-r--r--   0        0        0      849 2023-04-11 21:17:25.332143 nua-0.5.8/src/nua_cli/commands/build.py
+-rw-r--r--   0        0        0      960 2023-04-13 07:58:37.131820 nua-0.5.8/src/nua_cli/commands/config.py
+-rw-r--r--   0        0        0     1476 2023-04-13 08:14:53.074209 nua-0.5.8/src/nua_cli/commands/env.py
+-rw-r--r--   0        0        0      496 2023-04-11 21:17:25.334547 nua-0.5.8/src/nua_cli/commands/help.py
+-rw-r--r--   0        0        0     1805 2023-04-12 12:48:11.107863 nua-0.5.8/src/nua_cli/commands/lifecycle.py
+-rw-r--r--   0        0        0      821 2023-04-13 07:58:37.131453 nua-0.5.8/src/nua_cli/commands/logs.py
+-rw-r--r--   0        0        0      171 2023-04-11 21:17:25.335842 nua-0.5.8/src/nua_cli/commands/main.py
+-rw-r--r--   0        0        0     2463 2023-04-12 12:33:13.257321 nua-0.5.8/src/nua_cli/commands/server.py
+-rw-r--r--   0        0        0     1345 2023-04-11 21:17:25.337231 nua-0.5.8/src/nua_cli/common.py
+-rw-r--r--   0        0        0      168 2023-04-11 21:17:25.337653 nua-0.5.8/src/nua_cli/exceptions.py
+-rw-r--r--   0        0        0     1363 2023-04-12 08:38:41.344743 nua-0.5.8/src/nua_cli/main.py
+-rw-r--r--   0        0        0      103 2023-01-06 22:10:31.942417 nua-0.5.8/src/nua_cli/version.py
+-rw-r--r--   0        0        0     2468 1970-01-01 00:00:00.000000 nua-0.5.8/PKG-INFO
```

### Comparing `nua-0.5.16/pyproject.toml` & `nua-0.5.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [tool.poetry]
 name = "nua"
-version = "0.5.16"
-description = "Command line interface for the Nua self-hosted PaaS (Platform as a Service)"
+version = "0.5.8"
+description = ""
 authors = ["Stefane Fermigier <sf@abilian.com>"]
 readme = "readme.md"
 packages = [
   { include = "nua_cli", from = "src" }
 ]
 
 [tool.poetry.scripts]
-nua = "nua_cli.main:main"
+nua = "nua_cli.main:cli"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
+
 tomli = "^2.0.1"
 fabric = "^3.0.0"
+# Temp: use snoop in prod code
 snoop = "*"
+
+# typer = "^0.7.0"
 termcolor = "^2.2.0"
-cleez = "^0.1.7"
 
 [tool.poetry.group.dev.dependencies]
 abilian-devtools = "*"
 devtools = "*"
 types-setuptools = "*"
 
 # To please poetry
```

### Comparing `nua-0.5.16/readme.md` & `nua-0.5.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,83 +1,93 @@
+Metadata-Version: 2.1
+Name: nua
+Version: 0.5.8
+Summary: 
+Author: Stefane Fermigier
+Author-email: sf@abilian.com
+Requires-Python: >=3.10,<3.12
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fabric (>=3.0.0,<4.0.0)
+Requires-Dist: snoop
+Requires-Dist: termcolor (>=2.2.0,<3.0.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Description-Content-Type: text/markdown
+
 # nua-cli: CLI for NUA (for users)
 
 Command-line interface for Nua.
 
-[Nua](https://nua.rocks/) is an open source, self-hosted cloud platform project (a PaaS - platform as a service).
-
 Used by developers and devops people to deploy and manage applications.
 
 ## Installation
 
-### From PyPI
-
-On PyPI the package is called just `nua` (not `nua-cli`) as it is the main interface for Nua users.
-
-```bash
-pipx install nua
-nua
-```
+Nua-cli will be released soon on PyPI.
 
-### From source
+In the meantime, you can install it from the source repository:
 
-When developing nua-cli, you can install it from the source repository:
 ```bash
 pipx install --force "git+https://github.com/abilian/nua.git#subdirectory=nua-cli"
 ```
 
-Or, in editable mode, from your local clone:
+Alternatively, if you're hacking on nua-cli, you can install it in editable mode from your local clone:
+
 ```bash
 pipx install --force -e path/to/nua/nua-cli
 ```
 
 ## Usage
 
 ```bash
 nua --help
 # or
 nua [command] [options]
 ```
 
-### Main commands and subcommands
+## Main commands and subcommands
 
-Here's the list of commands and subcommands provided by nua-cli (some of them are not yet implemented):
+Here's the list of commands we should support, eventually (TBC):
 
 ```
 Available commands:
-  apps     List applications.
-  backup   Backup a deployed application.
-  build    Build app but don't deploy it.
-  deploy   Deploy app.
-  destroy  Destroy an application.
-  help     Show help.
-  logs     Show application logs.
-  restart  Restart an application.
-  restore  Restore backup data of a deployed application.
-  start    Start an application.
-  stop     Stop an application.
-  update   Update an application.
+  apps             List applications.
+  backup           Backup a deployed application.
+  config           Show/edit application config.
+  destroy          Destroy an application.
+  help             Show help.
+  logs             Show application logs.
+  restart          Restart an application.
+  restore          Restore backup data of a deployed application.
+  server           Manage the Nua server.
+  start            Start an application.
+  stop             Stop an application.
+  update           Update an application.
 
  config
   config show      Show application config.
 
- env
-  env set          Show application env variables.
-  env show         Show application env variables.
-
  server
-  server cleanup   Cleanup server (remove inactive docker images and containers).
   server logs      Show server logs.
   server ps        List all server processes.
   server settings  Show server settings.
   server status    Show Nua status.
   server uptime    Show server uptime.
 ```
 
 
-<!-- TODO: add more specific examples -->
+## Generic options
 
+- `--help` - Show help
+- `--version` - Show version number
 
-## Development
+## Examples (TBC)
 
-### Dependency graph
+```bash
+nua deploy --help
+nua deploy --app-id appid --domain fqdn
+nua deploy --app-id appid --domain fqdn --env SOMEVAR=value
+nua deploy --app-id appid --domain fqdn --env SOMEVAR=value --env-file .env
+nua deploy --app-id appid --domain fqdn --env SOMEVAR=value --env-file .env --config config-path
+nua deploy --app-id hedgedoc-1.9.6-10 --domain hdoc.example.com --env NODE_ENV=production
+```
 
-![Dependency graph](./doc/dependency-graph.png)
```

### Comparing `nua-0.5.16/src/nua_cli/client.py` & `nua-0.5.8/src/nua_cli/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import os
 import sys
 from io import StringIO
 
-from cleez.colors import red
 from fabric import Connection
 
+from nua_cli.colors import red
+
 # Hardcoded for now
 NUA_CMD = "./env/bin/nua-orchestrator"
 
 
 class Client:
     connection: Connection
```

### Comparing `nua-0.5.16/src/nua_cli/commands/apps.py` & `nua-0.5.8/src/nua_cli/commands/apps.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from cleez import Command
-from cleez.colors import green, red, yellow
-
-from ..client import get_client
+from nua_cli.base import Command
+from nua_cli.client import get_client
+from nua_cli.colors import green, red, yellow
 
 client = get_client()
 
 
 class AppsCommand(Command):
     """List applications."""
```

### Comparing `nua-0.5.16/src/nua_cli/commands/config.py` & `nua-0.5.8/src/nua_cli/commands/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,17 @@
 from pprint import pp
 
-from cleez import Command, CommandError
-from cleez.command import Argument
-
-from ..client import get_client
-from ..common import get_current_app_id
+from nua_cli.base import Argument, Command
+from nua_cli.client import get_client
+from nua_cli.common import get_current_app_id
+from nua_cli.exceptions import CommandError
 
 client = get_client()
 
 
-class ConfigCommand(Command):
-    """Show/edit application config."""
-
-    name = "config"
-    hide_from_help = True
-
-    def run(self):
-        self.cli.print_help()
-
-
 class ShowCommand(Command):
     """Show application config."""
 
     name = "config show"
 
     arguments = [
         Argument("app_id", nargs="?", help="Id of the application."),
@@ -38,7 +27,16 @@
 
         for instance in result:
             if instance["app_id"] == app_id:
                 pp(instance)
                 break
         else:
             raise CommandError(f"App {app_id} not found")
+
+
+class ConfigCommand(Command):
+    """Show/edit application config."""
+
+    name = "config"
+
+    def run(self):
+        self.cli.print_help()
```

### Comparing `nua-0.5.16/src/nua_cli/commands/env.py` & `nua-0.5.8/src/nua_cli/commands/env.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,15 @@
-from cleez.colors import bold, red
-from cleez.command import Argument, Command
-
-from ..client import get_client
-from ..common import get_current_app_id
+from nua_cli.base import Argument, Command
+from nua_cli.client import get_client
+from nua_cli.colors import bold, red
+from nua_cli.common import get_current_app_id
 
 client = get_client()
 
 
-class EnvCommand(Command):
-    """Manage an app's env variables."""
-
-    name = "env"
-    hide_from_help = True
-
-    def run(self):
-        self.cli.print_help()
-
-
 class EnvShowCommand(Command):
     """Show application env variables."""
 
     name = "env show"
 
     arguments = [
         Argument("app_id", nargs="?", help="Application ID"),
@@ -52,7 +41,16 @@
 class EnvSetCommand(Command):
     """Show application env variables."""
 
     name = "env set"
 
     def run(self, app_id: str = ""):
         print(red("Not implemented yet"))
+
+
+class EnvCommand(Command):
+    """Manage an app's env variables."""
+
+    name = "env"
+
+    def run(self):
+        self.cli.print_help()
```

### Comparing `nua-0.5.16/src/nua_cli/commands/lifecycle.py` & `nua-0.5.8/src/nua_cli/commands/lifecycle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from cleez.colors import red
-from cleez.command import Argument, Command
-
-from ..client import get_client
-from ._common import ORCH_PATH
+from nua_cli.base import Argument, Command
+from nua_cli.client import get_client
+from nua_cli.colors import red
 
 client = get_client()
 
+# Hardcoded for now
+ORCH_PATH = "/home/nua/env/bin/nua-orchestrator"
+
 
 class StartCommand(Command):
     """Start an application."""
 
     name = "start"
 
     arguments = [
```

### Comparing `nua-0.5.16/src/nua_cli/commands/logs.py` & `nua-0.5.8/src/nua_cli/commands/logs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from cleez.command import Argument, Command
-
+from nua_cli.base import Argument, Command
 from nua_cli.client import get_client
 from nua_cli.common import get_current_app_id
 
 client = get_client()
 
 
 class LogsCommand(Command):
```

### Comparing `nua-0.5.16/src/nua_cli/commands/server.py` & `nua-0.5.8/src/nua_cli/commands/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,17 @@
 from operator import itemgetter
 from pprint import pp
 
-from cleez import BadArgumentError
-from cleez.command import Argument, Command
-
-from ..client import get_client
+from nua_cli.base import Argument, Command
+from nua_cli.client import get_client
+from nua_cli.exceptions import BadArgument
 
 client = get_client()
 
 
-class ServerCommand(Command):
-    """Manage the Nua server."""
-
-    name = "server"
-    hide_from_help = True
-
-    def run(self):
-        self.cli.print_help()
-
-
 class LogsCommand(Command):
     """Show server logs."""
 
     name = "server logs"
 
     arguments = [
         Argument("service", help="Service to show logs for"),
@@ -37,17 +26,15 @@
                 print("Showing Nua logs [TODO]")
             case "letsencrypt":
                 result = client.ssh("cat log/letsencrypt/letsencrypt.log")
                 print(result.stdout)
             case "nginx":
                 print("Showing Nginx logs [TODO]")
             case _:
-                raise BadArgumentError(
-                    "Service must be one of: nua, letsencrypt, nginx"
-                )
+                raise BadArgument("Service must be one of: nua, letsencrypt, nginx")
 
 
 class StatusCommand(Command):
     """Show Nua status."""
 
     name = "server status"
 
@@ -104,7 +91,16 @@
 
     # TODO: ask for confirmation
 
     def run(self):
         result = client.ssh("docker system prune -af")
         result = client.ssh("docker volume prune -f")
         print(result.stdout)
+
+
+class ServerCommand(Command):
+    """Manage the Nua server."""
+
+    name = "server"
+
+    def run(self):
+        self.cli.print_help()
```

### Comparing `nua-0.5.16/src/nua_cli/common.py` & `nua-0.5.8/src/nua_cli/common.py`

 * *Files identical despite different names*


# Comparing `tmp/nua_build-0.5.14.tar.gz` & `tmp/nua_build-0.5.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua_build-0.5.14.tar", max compression
+gzip compressed data, was "nua_build-0.5.15.tar", max compression
```

## Comparing `nua_build-0.5.14.tar` & `nua_build-0.5.15.tar`

### file list

```diff
@@ -1,20 +1,44 @@
--rw-r--r--   0        0        0     3241 2023-04-24 21:25:56.860904 nua_build-0.5.14/README.md
--rw-r--r--   0        0        0     1784 2023-04-26 06:46:51.584593 nua_build-0.5.14/pyproject.toml
--rw-r--r--   0        0        0      208 2022-11-17 17:42:00.898773 nua_build-0.5.14/src/nua/build/__init__.py
--rw-r--r--   0        0        0       86 2023-01-06 12:47:38.576197 nua_build-0.5.14/src/nua/build/__main__.py
--rw-r--r--   0        0        0     2864 2023-04-08 16:30:34.934589 nua_build-0.5.14/src/nua/build/archive_search.py
--rw-r--r--   0        0        0      323 2023-04-16 17:02:10.325031 nua_build-0.5.14/src/nua/build/builders/__init__.py
--rw-r--r--   0        0        0     3166 2023-04-26 06:41:08.602266 nua_build-0.5.14/src/nua/build/builders/base.py
--rw-r--r--   0        0        0     7447 2023-04-26 06:41:08.602485 nua_build-0.5.14/src/nua/build/builders/docker.py
--rw-r--r--   0        0        0     2580 2023-04-26 06:41:08.602708 nua_build-0.5.14/src/nua/build/builders/factory.py
--rw-r--r--   0        0        0     2465 2023-04-26 06:41:08.602900 nua_build-0.5.14/src/nua/build/builders/wrap.py
--rw-r--r--   0        0        0      178 2022-12-20 18:49:45.395907 nua_build-0.5.14/src/nua/build/config.py
--rw-r--r--   0        0        0        0 2022-12-20 18:49:45.396072 nua_build-0.5.14/src/nua/build/default_conf/__init__.py
--rw-r--r--   0        0        0       65 2022-12-20 18:49:45.396131 nua_build-0.5.14/src/nua/build/default_conf/config.toml
--rw-r--r--   0        0        0      151 2023-01-19 17:57:22.672446 nua_build-0.5.14/src/nua/build/defaults/Dockerfile
--rw-r--r--   0        0        0       76 2022-12-03 19:23:00.336307 nua_build-0.5.14/src/nua/build/defaults/__init__.py
--rw-r--r--   0        0        0     2497 2023-04-26 06:41:08.603124 nua_build-0.5.14/src/nua/build/main.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.899795 nua_build-0.5.14/src/nua/build/scripts/__init__.py
--rw-r--r--   0        0        0     1750 2023-04-08 16:32:16.237367 nua_build-0.5.14/src/nua/build/scripts/test_replace_domain.py
--rw-r--r--   0        0        0       81 2022-11-17 17:42:00.900100 nua_build-0.5.14/src/nua/build/version.py
--rw-r--r--   0        0        0     4002 1970-01-01 00:00:00.000000 nua_build-0.5.14/PKG-INFO
+-rw-r--r--   0        0        0     3080 2023-04-29 09:12:48.076818 nua_build-0.5.15/README.md
+-rw-r--r--   0        0        0     1857 2023-04-29 09:31:08.191522 nua_build-0.5.15/pyproject.toml
+-rw-r--r--   0        0        0      208 2022-11-17 17:42:00.898773 nua_build-0.5.15/src/nua/build/__init__.py
+-rw-r--r--   0        0        0       86 2023-01-06 12:47:38.576197 nua_build-0.5.15/src/nua/build/__main__.py
+-rw-r--r--   0        0        0      485 2023-04-29 09:12:48.079484 nua_build-0.5.15/src/nua/build/autobuild/README.md
+-rw-r--r--   0        0        0      100 2023-04-29 09:12:48.079556 nua_build-0.5.15/src/nua/build/autobuild/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-29 09:12:48.079645 nua_build-0.5.15/src/nua/build/autobuild/builders/Dockerfile_nua_builder_node14
+-rw-r--r--   0        0        0      209 2023-04-29 09:12:48.079697 nua_build-0.5.15/src/nua/build/autobuild/builders/Dockerfile_nua_builder_node16
+-rw-r--r--   0        0        0      208 2023-04-29 09:12:48.079753 nua_build-0.5.15/src/nua/build/autobuild/builders/Dockerfile_nua_builder_ruby27
+-rw-r--r--   0        0        0      208 2023-04-29 09:12:48.079810 nua_build-0.5.15/src/nua/build/autobuild/builders/Dockerfile_nua_builder_ruby272
+-rw-r--r--   0        0        0      208 2023-04-29 09:12:48.079860 nua_build-0.5.15/src/nua/build/autobuild/builders/Dockerfile_nua_builder_ruby31
+-rw-r--r--   0        0        0      208 2023-04-29 09:12:48.079910 nua_build-0.5.15/src/nua/build/autobuild/builders/Dockerfile_nua_builder_ruby32
+-rw-r--r--   0        0        0        0 2023-04-29 09:12:48.079931 nua_build-0.5.15/src/nua/build/autobuild/builders/__init__.py
+-rw-r--r--   0        0        0      309 2023-04-29 09:12:48.079992 nua_build-0.5.15/src/nua/build/autobuild/builders/node14.json
+-rw-r--r--   0        0        0      309 2023-04-29 09:12:48.080044 nua_build-0.5.15/src/nua/build/autobuild/builders/node16.json
+-rw-r--r--   0        0        0      245 2023-04-29 09:12:48.080095 nua_build-0.5.15/src/nua/build/autobuild/builders/ruby27.json
+-rw-r--r--   0        0        0      225 2023-04-29 09:12:48.080148 nua_build-0.5.15/src/nua/build/autobuild/builders/ruby272.json
+-rw-r--r--   0        0        0      245 2023-04-29 09:12:48.080205 nua_build-0.5.15/src/nua/build/autobuild/builders/ruby31.json
+-rw-r--r--   0        0        0      245 2023-04-29 09:12:48.080254 nua_build-0.5.15/src/nua/build/autobuild/builders/ruby32.json
+-rw-r--r--   0        0        0      340 2023-04-29 09:12:48.080328 nua_build-0.5.15/src/nua/build/autobuild/constants.py
+-rw-r--r--   0        0        0    63409 2023-04-29 09:12:48.080646 nua_build-0.5.15/src/nua/build/autobuild/dependency-graph.png
+-rw-r--r--   0        0        0      225 2023-04-29 09:12:48.080742 nua_build-0.5.15/src/nua/build/autobuild/dockerfiles/Dockerfile_nua_builder_slim
+-rw-r--r--   0        0        0     1556 2023-04-29 09:12:48.080800 nua_build-0.5.15/src/nua/build/autobuild/dockerfiles/Dockerfile_nua_python_slim
+-rw-r--r--   0        0        0        0 2023-04-29 09:12:48.080821 nua_build-0.5.15/src/nua/build/autobuild/dockerfiles/__init__.py
+-rw-r--r--   0        0        0     1645 2023-04-29 09:12:48.080915 nua_build-0.5.15/src/nua/build/autobuild/main.py
+-rw-r--r--   0        0        0     6609 2023-04-29 09:12:48.081014 nua_build-0.5.15/src/nua/build/autobuild/nua_image_builder.py
+-rw-r--r--   0        0        0     5234 2023-04-29 09:12:48.081090 nua_build-0.5.15/src/nua/build/autobuild/nua_wheel_builder.py
+-rw-r--r--   0        0        0     3239 2023-04-29 09:12:48.081172 nua_build-0.5.15/src/nua/build/autobuild/register_builders.py
+-rw-r--r--   0        0        0       81 2023-04-29 09:12:48.081225 nua_build-0.5.15/src/nua/build/autobuild/version.py
+-rw-r--r--   0        0        0      323 2023-04-16 17:02:10.325031 nua_build-0.5.15/src/nua/build/builders/__init__.py
+-rw-r--r--   0        0        0     3164 2023-04-29 09:12:48.081480 nua_build-0.5.15/src/nua/build/builders/base.py
+-rw-r--r--   0        0        0     7437 2023-04-29 09:12:48.081745 nua_build-0.5.15/src/nua/build/builders/docker.py
+-rw-r--r--   0        0        0     2679 2023-04-29 09:12:48.081929 nua_build-0.5.15/src/nua/build/builders/factory.py
+-rw-r--r--   0        0        0     2447 2023-04-29 09:12:48.082118 nua_build-0.5.15/src/nua/build/builders/wrap.py
+-rw-r--r--   0        0        0      178 2022-12-20 18:49:45.395907 nua_build-0.5.15/src/nua/build/config.py
+-rw-r--r--   0        0        0        0 2022-12-20 18:49:45.396072 nua_build-0.5.15/src/nua/build/default_conf/__init__.py
+-rw-r--r--   0        0        0       65 2022-12-20 18:49:45.396131 nua_build-0.5.15/src/nua/build/default_conf/config.toml
+-rw-r--r--   0        0        0      151 2023-04-28 05:43:59.664713 nua_build-0.5.15/src/nua/build/defaults/Dockerfile
+-rw-r--r--   0        0        0       76 2022-12-03 19:23:00.336307 nua_build-0.5.15/src/nua/build/defaults/__init__.py
+-rw-r--r--   0        0        0     2631 2023-04-29 09:12:48.082306 nua_build-0.5.15/src/nua/build/main.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.899795 nua_build-0.5.15/src/nua/build/scripts/__init__.py
+-rw-r--r--   0        0        0     1750 2023-04-08 16:32:16.237367 nua_build-0.5.15/src/nua/build/scripts/test_replace_domain.py
+-rw-r--r--   0        0        0       81 2022-11-17 17:42:00.900100 nua_build-0.5.15/src/nua/build/version.py
+-rw-r--r--   0        0        0     3813 1970-01-01 00:00:00.000000 nua_build-0.5.15/PKG-INFO
```

### Comparing `nua_build-0.5.14/README.md` & `nua_build-0.5.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 
 - `nua-lib`: common code for all Nua packages. It provides:
 
     - `shell`: shell shortcuts (mostly wrappers above `subprocess` and `shutil`)
     - `exec`: shortcuts to execute sub commands like `exec_as_root()`, `exec_as_root()`
     - `actions`: higher level commands, related to the installation of packages and dependencies (wrappers above `apt`, `pip`, ...)
 
-- `nua-agent`: agent for Nua apps. It provides:
+- `nua-agent`: agent for building Nua apps. It provides:
 
-    - `nua_config`: library to read the embedded `nua-config` file (introspection),
     - `app_builder`: actual builder of the application inside the Docker image.
 
-- `nua-autobuild`: build Docker images used by Nua. It provides:
+## Dependency graph
 
-    - `nua_image_builder`:  tool to build locally the Nua standard base images if needed
+![Dependency graph](./doc/dependency-graph.png)
```

### Comparing `nua_build-0.5.14/pyproject.toml` & `nua_build-0.5.15/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 [tool.poetry]
 name = "nua-build"
-version = "0.5.14"
+version = "0.5.15"
 description = "Nua build package (currently: build, core build, agent)"
 authors = [
     "Stefane Fermigier <sf@abilian.com>",
     "Jerome Dumonteil <jd@abilian.com>",
 ]
 license = "AGPL"
 readme = "README.md"
 packages = [
   { include = "nua", from = "src" }
 ]
 
 [tool.poetry.scripts]
 nua-build = "nua.build.main:app"
+
+# Do we need this?
+nua-build-base-images = "nua.build.autobuild.main:app"
+
+# FIXME: remove
 nua_test_replace_domain = "nua.build.scripts.test_replace_domain:main"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-nua-lib = "=0.5.14"
-nua-agent = "=0.5.14"
-nua-autobuild = "=0.5.14"
+nua-lib = "=0.5.15"
 tomli = "^2.0.1"
+tomli-w = "^1.0.0"
 snoop = "^0.4.3"
 cleez = "^0.1.8"
-pyyaml = "^6.0"
+typer = {version = "^0.7.0", extras = ["all"]}
 docker = {version = "^6.0.1", extras = ["ssh"]}
 
 [tool.poetry.group.dev.dependencies]
 abilian-devtools = "*"
 nox = "*"
-devtools = "^0.11.0"
 
 types-setuptools = "*"
 types-pyyaml = "*"
 
 # To please poetry
 platformdirs = "<3.0.0"
+devtools = "^0.11.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 # ------------------------------------------------------------------------------
 
@@ -63,15 +67,14 @@
 [tool.deptry]
 exclude = [
     '.nox',
     'tests',
     "noxfile.py"
 ]
 ignore_obsolete = [
-    "nua-autobuild",
     "nua-lib",
     "nua-agent",
 ]
 ignore_missing = [
     "nua",
 ]
 ignore_transitive = [
```

### Comparing `nua_build-0.5.14/src/nua/build/builders/base.py` & `nua_build-0.5.15/src/nua/build/builders/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import abc
 import logging
 import tempfile
 from abc import abstractmethod
 from pathlib import Path
 
 from docker.models.images import Image
-from nua.agent.nua_config import NuaConfig
+from nua.lib.nua_config import NuaConfig
 from nua.lib.panic import info, show, title, vfprint, vprint, warning
 from nua.lib.tool.state import verbosity
 
 from .. import config as build_config
 
 logging.basicConfig(level=logging.INFO)
 CLIENT_TIMEOUT = 600
```

### Comparing `nua_build-0.5.14/src/nua/build/builders/docker.py` & `nua_build-0.5.15/src/nua/build/builders/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 import logging
 from contextlib import suppress
 from importlib import resources as rso
 from pathlib import Path
 from shutil import copy2, copytree
 
 import docker
-from nua.agent.constants import NUA_BUILDER_TAG
-from nua.agent.nua_config import hyphen_get, nua_config_names
-from nua.autobuild.docker_build_utils import (
+from nua.lib.constants import NUA_BUILDER_TAG
+from nua.lib.nua_config import hyphen_get, nua_config_names
+from nua.lib.docker import (
     display_docker_img,
     docker_build_log_error,
     docker_stream_build,
 )
-from nua.autobuild.nua_image_builder import NuaImageBuilder
-from nua.autobuild.register_builders import is_builder
+from nua.build.autobuild.nua_image_builder import NuaImageBuilder
+from nua.build.autobuild.register_builders import is_builder
 from nua.lib.backports import chdir
 from nua.lib.panic import info, vprint
 from nua.lib.shell import rm_fr
 from nua.lib.tool.state import verbosity, verbosity_level
 
 from .. import __version__
 from .base import Builder, BuilderError
```

### Comparing `nua_build-0.5.14/src/nua/build/builders/factory.py` & `nua_build-0.5.15/src/nua/build/builders/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from pathlib import Path
 from pprint import pformat
 from typing import Any
 
-from nua.agent.nua_config import NuaConfig
+from nua.lib.nua_config import NuaConfig
 from nua.lib.panic import info, vprint
 from nua.lib.tool.state import verbosity
 
 from .base import Builder, BuilderError
 from .docker import DockerBuilder
 from .wrap import DockerWrapBuilder
 
 
-def get_builder(config_path: str | Path | None = None, **opts) -> Builder:
-    config = NuaConfig(config_path)
+def get_builder(config_or_path: NuaConfig | str | Path = "", **opts) -> Builder:
+    if isinstance(config_or_path, NuaConfig):
+        config = config_or_path
+    else:
+        config = NuaConfig(config_or_path)
     factory = BuilderFactory(config, opts)
     return factory.get_builder()
 
 
 @dataclass(frozen=True)
 class BuilderFactory:
     """Factory to create a Builder instance."""
```

### Comparing `nua_build-0.5.14/src/nua/build/builders/wrap.py` & `nua_build-0.5.15/src/nua/build/builders/wrap.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Docker "wrap" builder: build a container from an existing dockerfile.
 """
 from __future__ import annotations
 
 import logging
 
 import docker
-from nua.autobuild.docker_build_utils import (
+from nua.lib.docker import (
     display_docker_img,
     docker_build_log_error,
     docker_stream_build,
 )
 from nua.lib.backports import chdir
 from nua.lib.panic import info
 from nua.lib.shell import rm_fr
```

### Comparing `nua_build-0.5.14/src/nua/build/main.py` & `nua_build-0.5.15/src/nua/build/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,41 +5,41 @@
 - build locally or wrap docker image
 
 Note: **currently use "nua-build ..." for command line**.
 See later if move this to "nua ...".
 """
 import argparse
 import sys
-import time
 import traceback
+from time import perf_counter
 
 import snoop
-from cleez.actions import VERSION
-
+from cleez.actions import VERSION, COUNT, STORE_TRUE
+from nua.lib.nua_config import NuaConfigError, NuaConfig
+from nua.lib.elapsed import elapsed
 from nua.lib.panic import Abort
 from nua.lib.tool.state import set_color, set_verbosity
-from nua.agent.nua_config import NuaConfigError
 
 from . import __version__
 from .builders import BuilderError, get_builder
 
 snoop.install()
 
 
 def main():
-    t0 = time.time()
+    t0 = perf_counter()
 
     parser = argparse.ArgumentParser()
 
     # Generic / classic options
     parser.add_argument(
         "-v",
         "--verbose",
         default=0,
-        action="count",
+        action=COUNT,
         help="Show more informations, until -vvv.",
     )
     parser.add_argument(
         "--color",
         default=True,
         action=argparse.BooleanOptionalAction,
         help="Enable (default) / disable colorized messages.",
@@ -50,17 +50,17 @@
         action=VERSION,
         version=f"nua-build version: {__version__}",
         help="Show nua-build version and exit.",
     )
 
     # Specific options / arguments
     parser.add_argument(
-        "config_file", help="Path to the package dir or 'nua-config' file."
+        "config_file", nargs="?", default=".", help="Path to the package dir or 'nua-config' file."
     )
-    parser.add_argument("-t", "--time", action="store_true", help="Print timing info")
+    parser.add_argument("-t", "--time", action=STORE_TRUE, help="Print timing info")
     parser.add_argument(
         "-s",
         "--save",
         default=True,
         action=argparse.BooleanOptionalAction,
         help="Save image locally after the build (defaults to True).",
     )
@@ -71,30 +71,32 @@
     set_color(args.color)
 
     opts = {
         "save_image": args.save,
     }
 
     try:
-        builder = get_builder(args.config_file or ".", **opts)
+        config = NuaConfig(args.config_file or ".")
     except NuaConfigError as e:
         # FIXME: not for production
         traceback.print_exc(file=sys.stderr)
         raise Abort(e.args[0])
 
+    builder = get_builder(config, **opts)
+
     try:
         builder.run()
     except BuilderError as e:
         # FIXME: not for production
         traceback.print_exc(file=sys.stderr)
         raise Abort from e
 
     if args.time or args.verbose >= 1:
-        t1 = time.time()
-        print(f"Build time (clock): {t1 - t0:.2f} seconds")
+        t1 = perf_counter()
+        print(f"Build time (clock): {elapsed(t1-t0)}")
 
 
 # Backwards compatibility
 app = main
 
 if __name__ == "__main__":
     main()
```

### Comparing `nua_build-0.5.14/src/nua/build/scripts/test_replace_domain.py` & `nua_build-0.5.15/src/nua/build/scripts/test_replace_domain.py`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.14/PKG-INFO` & `nua_build-0.5.15/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: nua-build
-Version: 0.5.14
+Version: 0.5.15
 Summary: Nua build package (currently: build, core build, agent)
 License: AGPL
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cleez (>=0.1.8,<0.2.0)
 Requires-Dist: docker[ssh] (>=6.0.1,<7.0.0)
-Requires-Dist: nua-agent (==0.5.14)
-Requires-Dist: nua-autobuild (==0.5.14)
-Requires-Dist: nua-lib (==0.5.14)
-Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: nua-lib (==0.5.15)
 Requires-Dist: snoop (>=0.4.3,<0.5.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
+Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # Nua-build
 
 Build system for Nua packages.
 
 [Nua](https://nua.rocks/) is an open source, self-hosted cloud platform project (a PaaS - platform as a service).
@@ -83,16 +82,15 @@
 
 - `nua-lib`: common code for all Nua packages. It provides:
 
     - `shell`: shell shortcuts (mostly wrappers above `subprocess` and `shutil`)
     - `exec`: shortcuts to execute sub commands like `exec_as_root()`, `exec_as_root()`
     - `actions`: higher level commands, related to the installation of packages and dependencies (wrappers above `apt`, `pip`, ...)
 
-- `nua-agent`: agent for Nua apps. It provides:
+- `nua-agent`: agent for building Nua apps. It provides:
 
-    - `nua_config`: library to read the embedded `nua-config` file (introspection),
     - `app_builder`: actual builder of the application inside the Docker image.
 
-- `nua-autobuild`: build Docker images used by Nua. It provides:
+## Dependency graph
 
-    - `nua_image_builder`:  tool to build locally the Nua standard base images if needed
+![Dependency graph](./doc/dependency-graph.png)
```


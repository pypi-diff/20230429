# Comparing `tmp/nua_agent-0.5.14.tar.gz` & `tmp/nua_agent-0.5.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua_agent-0.5.14.tar", max compression
+gzip compressed data, was "nua_agent-0.5.15.tar", max compression
```

## Comparing `nua_agent-0.5.14.tar` & `nua_agent-0.5.15.tar`

### file list

```diff
@@ -1,25 +1,17 @@
--rw-r--r--   0        0        0      793 2023-04-24 21:25:56.856175 nua_agent-0.5.14/README.md
--rw-r--r--   0        0        0     1436 2023-04-26 06:46:41.656673 nua_agent-0.5.14/pyproject.toml
--rw-r--r--   0        0        0      330 2023-04-06 11:40:42.165489 nua_agent-0.5.14/src/nua/agent/__init__.py
--rw-r--r--   0        0        0     1699 2023-04-24 21:25:56.857554 nua_agent-0.5.14/src/nua/agent/auto_install.py
--rw-r--r--   0        0        0      346 2023-02-28 08:14:12.790866 nua_agent-0.5.14/src/nua/agent/constants.py
--rw-r--r--   0        0        0        0 2023-02-06 17:21:30.492413 nua_agent-0.5.14/src/nua/agent/db/__init__.py
--rw-r--r--   0        0        0     1437 2023-02-06 17:21:30.492736 nua_agent-0.5.14/src/nua/agent/db/db_manager.py
--rw-r--r--   0        0        0     6233 2023-02-13 14:04:49.212138 nua_agent-0.5.14/src/nua/agent/db/mariadb_manager.py
--rw-r--r--   0        0        0     8651 2023-04-14 13:29:17.685138 nua_agent-0.5.14/src/nua/agent/db/postgres_manager.py
--rw-r--r--   0        0        0     2203 2023-02-15 19:18:03.537136 nua_agent-0.5.14/src/nua/agent/db/sqlite_manager.py
--rw-r--r--   0        0        0        0 2023-02-06 17:21:30.493328 nua_agent-0.5.14/src/nua/agent/deps/__init__.py
--rw-r--r--   0        0        0       75 2023-02-06 17:21:30.493417 nua_agent-0.5.14/src/nua/agent/deps/meta_packages.json
--rw-r--r--   0        0        0        0 2023-04-24 21:25:56.857636 nua_agent-0.5.14/src/nua/agent/detectors/__init__.py
--rw-r--r--   0        0        0     1114 2023-04-24 21:25:56.857882 nua_agent-0.5.14/src/nua/agent/detectors/base_detector.py
--rw-r--r--   0        0        0      950 2023-04-24 21:25:56.857950 nua_agent-0.5.14/src/nua/agent/detectors/nodejs_yarn.py
--rw-r--r--   0        0        0      646 2023-04-24 21:25:56.858041 nua_agent-0.5.14/src/nua/agent/detectors/python_source.py
--rw-r--r--   0        0        0      567 2023-04-24 21:25:56.858137 nua_agent-0.5.14/src/nua/agent/detectors/python_wheels.py
--rw-r--r--   0        0        0      497 2023-03-03 15:29:31.726769 nua_agent-0.5.14/src/nua/agent/meta_packages.py
--rw-r--r--   0        0        0    13027 2023-04-24 21:25:56.858265 nua_agent-0.5.14/src/nua/agent/nua_config.py
--rw-r--r--   0        0        0      544 2023-04-04 16:08:31.312095 nua_agent-0.5.14/src/nua/agent/nua_tag.py
--rw-r--r--   0        0        0        0 2023-02-06 17:21:30.493877 nua_agent-0.5.14/src/nua/agent/scripts/__init__.py
--rw-r--r--   0        0        0    11212 2023-04-24 21:25:56.858401 nua_agent-0.5.14/src/nua/agent/scripts/app_builder.py
--rw-r--r--   0        0        0     1583 2023-04-08 16:31:17.756437 nua_agent-0.5.14/src/nua/agent/templates.py
--rw-r--r--   0        0        0       81 2023-02-06 17:21:30.494088 nua_agent-0.5.14/src/nua/agent/version.py
--rw-r--r--   0        0        0     1363 1970-01-01 00:00:00.000000 nua_agent-0.5.14/PKG-INFO
+-rw-r--r--   0        0        0      756 2023-04-29 09:12:48.072338 nua_agent-0.5.15/README.md
+-rw-r--r--   0        0        0     1401 2023-04-29 09:31:01.359106 nua_agent-0.5.15/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-04-06 11:40:42.165489 nua_agent-0.5.15/src/nua/agent/__init__.py
+-rw-r--r--   0        0        0     1699 2023-04-26 08:44:27.752477 nua_agent-0.5.15/src/nua/agent/auto_install.py
+-rw-r--r--   0        0        0        0 2023-02-06 17:21:30.493328 nua_agent-0.5.15/src/nua/agent/deps/__init__.py
+-rw-r--r--   0        0        0       75 2023-02-06 17:21:30.493417 nua_agent-0.5.15/src/nua/agent/deps/meta_packages.json
+-rw-r--r--   0        0        0        0 2023-04-26 08:44:27.752548 nua_agent-0.5.15/src/nua/agent/detectors/__init__.py
+-rw-r--r--   0        0        0     1114 2023-04-26 08:44:27.752783 nua_agent-0.5.15/src/nua/agent/detectors/base_detector.py
+-rw-r--r--   0        0        0      950 2023-04-26 08:44:27.752858 nua_agent-0.5.15/src/nua/agent/detectors/nodejs_yarn.py
+-rw-r--r--   0        0        0      646 2023-04-26 08:44:27.752923 nua_agent-0.5.15/src/nua/agent/detectors/python_source.py
+-rw-r--r--   0        0        0      567 2023-04-26 08:44:27.752987 nua_agent-0.5.15/src/nua/agent/detectors/python_wheels.py
+-rw-r--r--   0        0        0      497 2023-03-03 15:29:31.726769 nua_agent-0.5.15/src/nua/agent/meta_packages.py
+-rw-r--r--   0        0        0        0 2023-02-06 17:21:30.493877 nua_agent-0.5.15/src/nua/agent/scripts/__init__.py
+-rw-r--r--   0        0        0    11227 2023-04-29 09:12:48.076574 nua_agent-0.5.15/src/nua/agent/scripts/app_builder.py
+-rw-r--r--   0        0        0     1583 2023-04-08 16:31:17.756437 nua_agent-0.5.15/src/nua/agent/templates.py
+-rw-r--r--   0        0        0       81 2023-02-06 17:21:30.494088 nua_agent-0.5.15/src/nua/agent/version.py
+-rw-r--r--   0        0        0     1253 1970-01-01 00:00:00.000000 nua_agent-0.5.15/PKG-INFO
```

### Comparing `nua_agent-0.5.14/pyproject.toml` & `nua_agent-0.5.15/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nua-agent"
-version = "0.5.14"
+version = "0.5.15"
 description = "Nua agent"
 authors = [
     "Stefane Fermigier <sf@abilian.com>",
     "Jerome Dumonteil <jd@abilian.com>",
 ]
 license = "AGPL"
 readme = "README.md"
@@ -12,24 +12,22 @@
     { include = "nua", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 setuptools = "*"
 packaging = "*"
-nua-lib = "=0.5.14"
-tomli = "^2.0.1"
-pyyaml = "^6.0"
+nua-lib = "=0.5.15"
 
 [tool.poetry.group.dev.dependencies]
 abilian-devtools = "*"
 nox = "*"
 types-setuptools = "*"
-types-pyyaml = "*"
 
+# Pinned for now
 platformdirs = "<3.0.0"
 
 [tool.poetry.scripts]
 app_builder = "nua.agent.scripts.app_builder:main"
 
 [build-system]
 requires = [
```

### Comparing `nua_agent-0.5.14/src/nua/agent/auto_install.py` & `nua_agent-0.5.15/src/nua/agent/auto_install.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.14/src/nua/agent/detectors/base_detector.py` & `nua_agent-0.5.15/src/nua/agent/detectors/base_detector.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.14/src/nua/agent/detectors/nodejs_yarn.py` & `nua_agent-0.5.15/src/nua/agent/detectors/nodejs_yarn.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.14/src/nua/agent/detectors/python_source.py` & `nua_agent-0.5.15/src/nua/agent/detectors/python_source.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.14/src/nua/agent/detectors/python_wheels.py` & `nua_agent-0.5.15/src/nua/agent/detectors/python_wheels.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.14/src/nua/agent/scripts/app_builder.py` & `nua_agent-0.5.15/src/nua/agent/scripts/app_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,35 +18,35 @@
     install_meta_packages,
     install_packages,
     install_pip_packages,
     install_source,
     installed_packages,
 )
 from nua.lib.backports import chdir
+from nua.lib.constants import (
+    NUA_APP_PATH,
+    NUA_BUILD_PATH,
+    NUA_METADATA_PATH,
+    NUA_SCRIPTS_PATH,
+)
 from nua.lib.exec import exec_as_nua, exec_as_root
+from nua.lib.nua_config import NuaConfig, hyphen_get
 from nua.lib.panic import Abort, info, show, vprint, warning
 from nua.lib.shell import chmod_r, chown_r, mkdir_p, rm_fr, sh
 from nua.lib.tool.state import (
     set_packages_updated,
     set_verbosity,
     verbosity,
     verbosity_level,
 )
 
 from ..auto_install import detect_and_install
-from ..constants import (
-    NUA_APP_PATH,
-    NUA_BUILD_PATH,
-    NUA_METADATA_PATH,
-    NUA_SCRIPTS_PATH,
-)
 
-# most inferred meta packages will provided by plugins in the future:
+# most inferred meta packages will be provided by plugins in the future:
 from ..meta_packages import meta_packages_requirements
-from ..nua_config import NuaConfig, hyphen_get
 
 logging.basicConfig(level=logging.INFO)
 
 
 class BuilderApp:
     """Class to hold config and other state information during build."""
```

### Comparing `nua_agent-0.5.14/src/nua/agent/templates.py` & `nua_agent-0.5.15/src/nua/agent/templates.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.14/PKG-INFO` & `nua_agent-0.5.15/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: nua-agent
-Version: 0.5.14
+Version: 0.5.15
 Summary: Nua agent
 License: AGPL
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nua-lib (==0.5.14)
+Requires-Dist: nua-lib (==0.5.15)
 Requires-Dist: packaging
-Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: setuptools
-Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Nua Agent
 
 [Nua](https://nua.rocks/) is an open source, self-hosted cloud platform project (a PaaS - platform as a service).
 
 This packaged is used internally. The main entry point is the `nua` command line tool (see: [Nua on PyPI](https://pypi.org/project/nua/) or [nua-cli on GitHub](https://github.com/abilian/nua/tree/main/nua-cli)).
 
-The `nua-agent` package is included in every Nua application image.
+The `nua-agent` package provides the agent that runs inside the Docker image *during the build of the application*.
 
-It will provide the following features (TBC):
+Note: don't depend on `nua-agent` being installed in the Docker image. It is not a runtime dependency.
 
--   Application licycle management
--   Smoke tests and health checks
--   Logging and monitoring
 
 ## Content
 
 `nua-agent` provides:
 
-- `nua_config`: library to read the embedded `nua-config` file (introspection),
-- `app_builder`: actual builder of the application inside the Docker image.
-- `db`: collection of tools to manage databases
+- The `app-builder` script: actual builder of the application inside the Docker image.
+
+
+## Dependency graph
+
+![Dependency graph](./doc/dependency-graph.png)
```


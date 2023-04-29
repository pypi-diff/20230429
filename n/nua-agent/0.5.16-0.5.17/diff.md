# Comparing `tmp/nua_agent-0.5.16.tar.gz` & `tmp/nua_agent-0.5.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua_agent-0.5.16.tar", max compression
+gzip compressed data, was "nua_agent-0.5.17.tar", max compression
```

## Comparing `nua_agent-0.5.16.tar` & `nua_agent-0.5.17.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      756 2023-04-29 09:12:48.072338 nua_agent-0.5.16/README.md
--rw-r--r--   0        0        0     1401 2023-04-29 10:19:14.436051 nua_agent-0.5.16/pyproject.toml
--rw-r--r--   0        0        0      330 2023-04-06 11:40:42.165489 nua_agent-0.5.16/src/nua/agent/__init__.py
--rw-r--r--   0        0        0     1699 2023-04-26 08:44:27.752477 nua_agent-0.5.16/src/nua/agent/auto_install.py
--rw-r--r--   0        0        0        0 2023-02-06 17:21:30.493328 nua_agent-0.5.16/src/nua/agent/deps/__init__.py
--rw-r--r--   0        0        0       75 2023-02-06 17:21:30.493417 nua_agent-0.5.16/src/nua/agent/deps/meta_packages.json
--rw-r--r--   0        0        0        0 2023-04-26 08:44:27.752548 nua_agent-0.5.16/src/nua/agent/detectors/__init__.py
--rw-r--r--   0        0        0     1114 2023-04-26 08:44:27.752783 nua_agent-0.5.16/src/nua/agent/detectors/base_detector.py
--rw-r--r--   0        0        0      950 2023-04-26 08:44:27.752858 nua_agent-0.5.16/src/nua/agent/detectors/nodejs_yarn.py
--rw-r--r--   0        0        0      646 2023-04-26 08:44:27.752923 nua_agent-0.5.16/src/nua/agent/detectors/python_source.py
--rw-r--r--   0        0        0      567 2023-04-26 08:44:27.752987 nua_agent-0.5.16/src/nua/agent/detectors/python_wheels.py
--rw-r--r--   0        0        0      497 2023-03-03 15:29:31.726769 nua_agent-0.5.16/src/nua/agent/meta_packages.py
--rw-r--r--   0        0        0        0 2023-02-06 17:21:30.493877 nua_agent-0.5.16/src/nua/agent/scripts/__init__.py
--rw-r--r--   0        0        0    11227 2023-04-29 09:12:48.076574 nua_agent-0.5.16/src/nua/agent/scripts/app_builder.py
--rw-r--r--   0        0        0     1583 2023-04-08 16:31:17.756437 nua_agent-0.5.16/src/nua/agent/templates.py
--rw-r--r--   0        0        0       81 2023-02-06 17:21:30.494088 nua_agent-0.5.16/src/nua/agent/version.py
--rw-r--r--   0        0        0     1253 1970-01-01 00:00:00.000000 nua_agent-0.5.16/PKG-INFO
+-rw-r--r--   0        0        0      756 2023-04-29 09:12:48.072338 nua_agent-0.5.17/README.md
+-rw-r--r--   0        0        0     1401 2023-04-29 10:37:24.537624 nua_agent-0.5.17/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-04-06 11:40:42.165489 nua_agent-0.5.17/src/nua/agent/__init__.py
+-rw-r--r--   0        0        0     1699 2023-04-26 08:44:27.752477 nua_agent-0.5.17/src/nua/agent/auto_install.py
+-rw-r--r--   0        0        0        0 2023-02-06 17:21:30.493328 nua_agent-0.5.17/src/nua/agent/deps/__init__.py
+-rw-r--r--   0        0        0       75 2023-02-06 17:21:30.493417 nua_agent-0.5.17/src/nua/agent/deps/meta_packages.json
+-rw-r--r--   0        0        0        0 2023-04-26 08:44:27.752548 nua_agent-0.5.17/src/nua/agent/detectors/__init__.py
+-rw-r--r--   0        0        0     1114 2023-04-26 08:44:27.752783 nua_agent-0.5.17/src/nua/agent/detectors/base_detector.py
+-rw-r--r--   0        0        0      950 2023-04-26 08:44:27.752858 nua_agent-0.5.17/src/nua/agent/detectors/nodejs_yarn.py
+-rw-r--r--   0        0        0      646 2023-04-26 08:44:27.752923 nua_agent-0.5.17/src/nua/agent/detectors/python_source.py
+-rw-r--r--   0        0        0      567 2023-04-26 08:44:27.752987 nua_agent-0.5.17/src/nua/agent/detectors/python_wheels.py
+-rw-r--r--   0        0        0      497 2023-03-03 15:29:31.726769 nua_agent-0.5.17/src/nua/agent/meta_packages.py
+-rw-r--r--   0        0        0        0 2023-02-06 17:21:30.493877 nua_agent-0.5.17/src/nua/agent/scripts/__init__.py
+-rw-r--r--   0        0        0    11227 2023-04-29 09:12:48.076574 nua_agent-0.5.17/src/nua/agent/scripts/app_builder.py
+-rw-r--r--   0        0        0     1583 2023-04-08 16:31:17.756437 nua_agent-0.5.17/src/nua/agent/templates.py
+-rw-r--r--   0        0        0       81 2023-02-06 17:21:30.494088 nua_agent-0.5.17/src/nua/agent/version.py
+-rw-r--r--   0        0        0     1253 1970-01-01 00:00:00.000000 nua_agent-0.5.17/PKG-INFO
```

### Comparing `nua_agent-0.5.16/README.md` & `nua_agent-0.5.17/README.md`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.16/pyproject.toml` & `nua_agent-0.5.17/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nua-agent"
-version = "0.5.16"
+version = "0.5.17"
 description = "Nua agent"
 authors = [
     "Stefane Fermigier <sf@abilian.com>",
     "Jerome Dumonteil <jd@abilian.com>",
 ]
 license = "AGPL"
 readme = "README.md"
@@ -12,15 +12,15 @@
     { include = "nua", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 setuptools = "*"
 packaging = "*"
-nua-lib = "=0.5.16"
+nua-lib = "=0.5.17"
 
 [tool.poetry.group.dev.dependencies]
 abilian-devtools = "*"
 nox = "*"
 types-setuptools = "*"
 
 # Pinned for now
```

### Comparing `nua_agent-0.5.16/src/nua/agent/auto_install.py` & `nua_agent-0.5.17/src/nua/agent/auto_install.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.16/src/nua/agent/detectors/base_detector.py` & `nua_agent-0.5.17/src/nua/agent/detectors/base_detector.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.16/src/nua/agent/detectors/nodejs_yarn.py` & `nua_agent-0.5.17/src/nua/agent/detectors/nodejs_yarn.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.16/src/nua/agent/detectors/python_source.py` & `nua_agent-0.5.17/src/nua/agent/detectors/python_source.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.16/src/nua/agent/detectors/python_wheels.py` & `nua_agent-0.5.17/src/nua/agent/detectors/python_wheels.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.16/src/nua/agent/scripts/app_builder.py` & `nua_agent-0.5.17/src/nua/agent/scripts/app_builder.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.16/src/nua/agent/templates.py` & `nua_agent-0.5.17/src/nua/agent/templates.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.16/PKG-INFO` & `nua_agent-0.5.17/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: nua-agent
-Version: 0.5.16
+Version: 0.5.17
 Summary: Nua agent
 License: AGPL
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nua-lib (==0.5.16)
+Requires-Dist: nua-lib (==0.5.17)
 Requires-Dist: packaging
 Requires-Dist: setuptools
 Description-Content-Type: text/markdown
 
 # Nua Agent
 
 [Nua](https://nua.rocks/) is an open source, self-hosted cloud platform project (a PaaS - platform as a service).
```


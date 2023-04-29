# Comparing `tmp/nua_build-0.5.15.tar.gz` & `tmp/nua_build-0.5.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua_build-0.5.15.tar", max compression
+gzip compressed data, was "nua_build-0.5.16.tar", max compression
```

## Comparing `nua_build-0.5.15.tar` & `nua_build-0.5.16.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     3080 2023-04-29 09:12:48.076818 nua_build-0.5.15/README.md
--rw-r--r--   0        0        0     1857 2023-04-29 09:31:08.191522 nua_build-0.5.15/pyproject.toml
--rw-r--r--   0        0        0      208 2022-11-17 17:42:00.898773 nua_build-0.5.15/src/nua/build/__init__.py
--rw-r--r--   0        0        0       86 2023-01-06 12:47:38.576197 nua_build-0.5.15/src/nua/build/__main__.py
--rw-r--r--   0        0        0      485 2023-04-29 09:12:48.079484 nua_build-0.5.15/src/nua/build/autobuild/README.md
--rw-r--r--   0        0        0      100 2023-04-29 09:12:48.079556 nua_build-0.5.15/src/nua/build/autobuild/__init__.py
--rw-r--r--   0        0        0      209 2023-04-29 09:12:48.079645 nua_build-0.5.15/src/nua/build/autobuild/builders/Dockerfile_nua_builder_node14
--rw-r--r--   0        0        0      209 2023-04-29 09:12:48.079697 nua_build-0.5.15/src/nua/build/autobuild/builders/Dockerfile_nua_builder_node16
--rw-r--r--   0        0        0      208 2023-04-29 09:12:48.079753 nua_build-0.5.15/src/nua/build/autobuild/builders/Dockerfile_nua_builder_ruby27
--rw-r--r--   0        0        0      208 2023-04-29 09:12:48.079810 nua_build-0.5.15/src/nua/build/autobuild/builders/Dockerfile_nua_builder_ruby272
--rw-r--r--   0        0        0      208 2023-04-29 09:12:48.079860 nua_build-0.5.15/src/nua/build/autobuild/builders/Dockerfile_nua_builder_ruby31
--rw-r--r--   0        0        0      208 2023-04-29 09:12:48.079910 nua_build-0.5.15/src/nua/build/autobuild/builders/Dockerfile_nua_builder_ruby32
--rw-r--r--   0        0        0        0 2023-04-29 09:12:48.079931 nua_build-0.5.15/src/nua/build/autobuild/builders/__init__.py
--rw-r--r--   0        0        0      309 2023-04-29 09:12:48.079992 nua_build-0.5.15/src/nua/build/autobuild/builders/node14.json
--rw-r--r--   0        0        0      309 2023-04-29 09:12:48.080044 nua_build-0.5.15/src/nua/build/autobuild/builders/node16.json
--rw-r--r--   0        0        0      245 2023-04-29 09:12:48.080095 nua_build-0.5.15/src/nua/build/autobuild/builders/ruby27.json
--rw-r--r--   0        0        0      225 2023-04-29 09:12:48.080148 nua_build-0.5.15/src/nua/build/autobuild/builders/ruby272.json
--rw-r--r--   0        0        0      245 2023-04-29 09:12:48.080205 nua_build-0.5.15/src/nua/build/autobuild/builders/ruby31.json
--rw-r--r--   0        0        0      245 2023-04-29 09:12:48.080254 nua_build-0.5.15/src/nua/build/autobuild/builders/ruby32.json
--rw-r--r--   0        0        0      340 2023-04-29 09:12:48.080328 nua_build-0.5.15/src/nua/build/autobuild/constants.py
--rw-r--r--   0        0        0    63409 2023-04-29 09:12:48.080646 nua_build-0.5.15/src/nua/build/autobuild/dependency-graph.png
--rw-r--r--   0        0        0      225 2023-04-29 09:12:48.080742 nua_build-0.5.15/src/nua/build/autobuild/dockerfiles/Dockerfile_nua_builder_slim
--rw-r--r--   0        0        0     1556 2023-04-29 09:12:48.080800 nua_build-0.5.15/src/nua/build/autobuild/dockerfiles/Dockerfile_nua_python_slim
--rw-r--r--   0        0        0        0 2023-04-29 09:12:48.080821 nua_build-0.5.15/src/nua/build/autobuild/dockerfiles/__init__.py
--rw-r--r--   0        0        0     1645 2023-04-29 09:12:48.080915 nua_build-0.5.15/src/nua/build/autobuild/main.py
--rw-r--r--   0        0        0     6609 2023-04-29 09:12:48.081014 nua_build-0.5.15/src/nua/build/autobuild/nua_image_builder.py
--rw-r--r--   0        0        0     5234 2023-04-29 09:12:48.081090 nua_build-0.5.15/src/nua/build/autobuild/nua_wheel_builder.py
--rw-r--r--   0        0        0     3239 2023-04-29 09:12:48.081172 nua_build-0.5.15/src/nua/build/autobuild/register_builders.py
--rw-r--r--   0        0        0       81 2023-04-29 09:12:48.081225 nua_build-0.5.15/src/nua/build/autobuild/version.py
--rw-r--r--   0        0        0      323 2023-04-16 17:02:10.325031 nua_build-0.5.15/src/nua/build/builders/__init__.py
--rw-r--r--   0        0        0     3164 2023-04-29 09:12:48.081480 nua_build-0.5.15/src/nua/build/builders/base.py
--rw-r--r--   0        0        0     7437 2023-04-29 09:12:48.081745 nua_build-0.5.15/src/nua/build/builders/docker.py
--rw-r--r--   0        0        0     2679 2023-04-29 09:12:48.081929 nua_build-0.5.15/src/nua/build/builders/factory.py
--rw-r--r--   0        0        0     2447 2023-04-29 09:12:48.082118 nua_build-0.5.15/src/nua/build/builders/wrap.py
--rw-r--r--   0        0        0      178 2022-12-20 18:49:45.395907 nua_build-0.5.15/src/nua/build/config.py
--rw-r--r--   0        0        0        0 2022-12-20 18:49:45.396072 nua_build-0.5.15/src/nua/build/default_conf/__init__.py
--rw-r--r--   0        0        0       65 2022-12-20 18:49:45.396131 nua_build-0.5.15/src/nua/build/default_conf/config.toml
--rw-r--r--   0        0        0      151 2023-04-28 05:43:59.664713 nua_build-0.5.15/src/nua/build/defaults/Dockerfile
--rw-r--r--   0        0        0       76 2022-12-03 19:23:00.336307 nua_build-0.5.15/src/nua/build/defaults/__init__.py
--rw-r--r--   0        0        0     2631 2023-04-29 09:12:48.082306 nua_build-0.5.15/src/nua/build/main.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.899795 nua_build-0.5.15/src/nua/build/scripts/__init__.py
--rw-r--r--   0        0        0     1750 2023-04-08 16:32:16.237367 nua_build-0.5.15/src/nua/build/scripts/test_replace_domain.py
--rw-r--r--   0        0        0       81 2022-11-17 17:42:00.900100 nua_build-0.5.15/src/nua/build/version.py
--rw-r--r--   0        0        0     3813 1970-01-01 00:00:00.000000 nua_build-0.5.15/PKG-INFO
+-rw-r--r--   0        0        0     3080 2023-04-29 09:12:48.076818 nua_build-0.5.16/README.md
+-rw-r--r--   0        0        0     1857 2023-04-29 10:19:18.931091 nua_build-0.5.16/pyproject.toml
+-rw-r--r--   0        0        0      208 2022-11-17 17:42:00.898773 nua_build-0.5.16/src/nua/build/__init__.py
+-rw-r--r--   0        0        0       86 2023-01-06 12:47:38.576197 nua_build-0.5.16/src/nua/build/__main__.py
+-rw-r--r--   0        0        0      485 2023-04-29 09:12:48.079484 nua_build-0.5.16/src/nua/build/autobuild/README.md
+-rw-r--r--   0        0        0      100 2023-04-29 09:12:48.079556 nua_build-0.5.16/src/nua/build/autobuild/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-29 09:12:48.079645 nua_build-0.5.16/src/nua/build/autobuild/builders/Dockerfile_nua_builder_node14
+-rw-r--r--   0        0        0      209 2023-04-29 09:12:48.079697 nua_build-0.5.16/src/nua/build/autobuild/builders/Dockerfile_nua_builder_node16
+-rw-r--r--   0        0        0      208 2023-04-29 09:12:48.079753 nua_build-0.5.16/src/nua/build/autobuild/builders/Dockerfile_nua_builder_ruby27
+-rw-r--r--   0        0        0      208 2023-04-29 09:12:48.079810 nua_build-0.5.16/src/nua/build/autobuild/builders/Dockerfile_nua_builder_ruby272
+-rw-r--r--   0        0        0      208 2023-04-29 09:12:48.079860 nua_build-0.5.16/src/nua/build/autobuild/builders/Dockerfile_nua_builder_ruby31
+-rw-r--r--   0        0        0      208 2023-04-29 09:12:48.079910 nua_build-0.5.16/src/nua/build/autobuild/builders/Dockerfile_nua_builder_ruby32
+-rw-r--r--   0        0        0        0 2023-04-29 09:12:48.079931 nua_build-0.5.16/src/nua/build/autobuild/builders/__init__.py
+-rw-r--r--   0        0        0      309 2023-04-29 09:12:48.079992 nua_build-0.5.16/src/nua/build/autobuild/builders/node14.json
+-rw-r--r--   0        0        0      309 2023-04-29 09:12:48.080044 nua_build-0.5.16/src/nua/build/autobuild/builders/node16.json
+-rw-r--r--   0        0        0      245 2023-04-29 09:12:48.080095 nua_build-0.5.16/src/nua/build/autobuild/builders/ruby27.json
+-rw-r--r--   0        0        0      225 2023-04-29 09:12:48.080148 nua_build-0.5.16/src/nua/build/autobuild/builders/ruby272.json
+-rw-r--r--   0        0        0      245 2023-04-29 09:12:48.080205 nua_build-0.5.16/src/nua/build/autobuild/builders/ruby31.json
+-rw-r--r--   0        0        0      245 2023-04-29 09:12:48.080254 nua_build-0.5.16/src/nua/build/autobuild/builders/ruby32.json
+-rw-r--r--   0        0        0      340 2023-04-29 09:12:48.080328 nua_build-0.5.16/src/nua/build/autobuild/constants.py
+-rw-r--r--   0        0        0    63409 2023-04-29 09:12:48.080646 nua_build-0.5.16/src/nua/build/autobuild/dependency-graph.png
+-rw-r--r--   0        0        0      225 2023-04-29 09:12:48.080742 nua_build-0.5.16/src/nua/build/autobuild/dockerfiles/Dockerfile_nua_builder_slim
+-rw-r--r--   0        0        0     1556 2023-04-29 09:12:48.080800 nua_build-0.5.16/src/nua/build/autobuild/dockerfiles/Dockerfile_nua_python_slim
+-rw-r--r--   0        0        0        0 2023-04-29 09:12:48.080821 nua_build-0.5.16/src/nua/build/autobuild/dockerfiles/__init__.py
+-rw-r--r--   0        0        0     1645 2023-04-29 09:12:48.080915 nua_build-0.5.16/src/nua/build/autobuild/main.py
+-rw-r--r--   0        0        0     6609 2023-04-29 09:12:48.081014 nua_build-0.5.16/src/nua/build/autobuild/nua_image_builder.py
+-rw-r--r--   0        0        0     5234 2023-04-29 09:12:48.081090 nua_build-0.5.16/src/nua/build/autobuild/nua_wheel_builder.py
+-rw-r--r--   0        0        0     3239 2023-04-29 09:12:48.081172 nua_build-0.5.16/src/nua/build/autobuild/register_builders.py
+-rw-r--r--   0        0        0       81 2023-04-29 09:12:48.081225 nua_build-0.5.16/src/nua/build/autobuild/version.py
+-rw-r--r--   0        0        0      323 2023-04-16 17:02:10.325031 nua_build-0.5.16/src/nua/build/builders/__init__.py
+-rw-r--r--   0        0        0     3164 2023-04-29 09:12:48.081480 nua_build-0.5.16/src/nua/build/builders/base.py
+-rw-r--r--   0        0        0     7437 2023-04-29 09:12:48.081745 nua_build-0.5.16/src/nua/build/builders/docker.py
+-rw-r--r--   0        0        0     2679 2023-04-29 09:12:48.081929 nua_build-0.5.16/src/nua/build/builders/factory.py
+-rw-r--r--   0        0        0     2447 2023-04-29 09:12:48.082118 nua_build-0.5.16/src/nua/build/builders/wrap.py
+-rw-r--r--   0        0        0      178 2022-12-20 18:49:45.395907 nua_build-0.5.16/src/nua/build/config.py
+-rw-r--r--   0        0        0        0 2022-12-20 18:49:45.396072 nua_build-0.5.16/src/nua/build/default_conf/__init__.py
+-rw-r--r--   0        0        0       65 2022-12-20 18:49:45.396131 nua_build-0.5.16/src/nua/build/default_conf/config.toml
+-rw-r--r--   0        0        0      151 2023-04-28 05:43:59.664713 nua_build-0.5.16/src/nua/build/defaults/Dockerfile
+-rw-r--r--   0        0        0       76 2022-12-03 19:23:00.336307 nua_build-0.5.16/src/nua/build/defaults/__init__.py
+-rw-r--r--   0        0        0     2631 2023-04-29 09:12:48.082306 nua_build-0.5.16/src/nua/build/main.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.899795 nua_build-0.5.16/src/nua/build/scripts/__init__.py
+-rw-r--r--   0        0        0     1750 2023-04-08 16:32:16.237367 nua_build-0.5.16/src/nua/build/scripts/test_replace_domain.py
+-rw-r--r--   0        0        0       81 2022-11-17 17:42:00.900100 nua_build-0.5.16/src/nua/build/version.py
+-rw-r--r--   0        0        0     3813 1970-01-01 00:00:00.000000 nua_build-0.5.16/PKG-INFO
```

### Comparing `nua_build-0.5.15/README.md` & `nua_build-0.5.16/README.md`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.15/pyproject.toml` & `nua_build-0.5.16/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nua-build"
-version = "0.5.15"
+version = "0.5.16"
 description = "Nua build package (currently: build, core build, agent)"
 authors = [
     "Stefane Fermigier <sf@abilian.com>",
     "Jerome Dumonteil <jd@abilian.com>",
 ]
 license = "AGPL"
 readme = "README.md"
@@ -19,15 +19,15 @@
 nua-build-base-images = "nua.build.autobuild.main:app"
 
 # FIXME: remove
 nua_test_replace_domain = "nua.build.scripts.test_replace_domain:main"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-nua-lib = "=0.5.15"
+nua-lib = "=0.5.16"
 tomli = "^2.0.1"
 tomli-w = "^1.0.0"
 snoop = "^0.4.3"
 cleez = "^0.1.8"
 typer = {version = "^0.7.0", extras = ["all"]}
 docker = {version = "^6.0.1", extras = ["ssh"]}
```

### Comparing `nua_build-0.5.15/src/nua/build/autobuild/dependency-graph.png` & `nua_build-0.5.16/src/nua/build/autobuild/dependency-graph.png`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.15/src/nua/build/autobuild/dockerfiles/Dockerfile_nua_python_slim` & `nua_build-0.5.16/src/nua/build/autobuild/dockerfiles/Dockerfile_nua_python_slim`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.15/src/nua/build/autobuild/main.py` & `nua_build-0.5.16/src/nua/build/autobuild/main.py`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.15/src/nua/build/autobuild/nua_image_builder.py` & `nua_build-0.5.16/src/nua/build/autobuild/nua_image_builder.py`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.15/src/nua/build/autobuild/nua_wheel_builder.py` & `nua_build-0.5.16/src/nua/build/autobuild/nua_wheel_builder.py`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.15/src/nua/build/autobuild/register_builders.py` & `nua_build-0.5.16/src/nua/build/autobuild/register_builders.py`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.15/src/nua/build/builders/base.py` & `nua_build-0.5.16/src/nua/build/builders/base.py`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.15/src/nua/build/builders/docker.py` & `nua_build-0.5.16/src/nua/build/builders/docker.py`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.15/src/nua/build/builders/factory.py` & `nua_build-0.5.16/src/nua/build/builders/factory.py`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.15/src/nua/build/builders/wrap.py` & `nua_build-0.5.16/src/nua/build/builders/wrap.py`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.15/src/nua/build/main.py` & `nua_build-0.5.16/src/nua/build/main.py`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.15/src/nua/build/scripts/test_replace_domain.py` & `nua_build-0.5.16/src/nua/build/scripts/test_replace_domain.py`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.15/PKG-INFO` & `nua_build-0.5.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nua-build
-Version: 0.5.15
+Version: 0.5.16
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
-Requires-Dist: nua-lib (==0.5.15)
+Requires-Dist: nua-lib (==0.5.16)
 Requires-Dist: snoop (>=0.4.3,<0.5.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # Nua-build
```


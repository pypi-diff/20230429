# Comparing `tmp/poetry_docker_plugin-0.4.0.tar.gz` & `tmp/poetry_docker_plugin-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_docker_plugin-0.4.0.tar", max compression
+gzip compressed data, was "poetry_docker_plugin-0.5.0.tar", max compression
```

## Comparing `poetry_docker_plugin-0.4.0.tar` & `poetry_docker_plugin-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1090 2022-10-09 20:19:34.073974 poetry_docker_plugin-0.4.0/LICENSE
--rw-r--r--   0        0        0     2798 2023-01-13 13:59:16.314260 poetry_docker_plugin-0.4.0/README.md
--rw-r--r--   0        0        0      367 2023-01-13 13:04:47.288196 poetry_docker_plugin-0.4.0/poetry_docker_plugin/__init__.py
--rw-r--r--   0        0        0     8388 2023-02-03 17:03:18.026335 poetry_docker_plugin-0.4.0/poetry_docker_plugin/docker_builder.py
--rw-r--r--   0        0        0     8372 2023-02-03 17:28:35.103129 poetry_docker_plugin-0.4.0/poetry_docker_plugin/plugin.py
--rw-r--r--   0        0        0     3099 2023-02-03 17:35:34.441292 poetry_docker_plugin-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3774 1970-01-01 00:00:00.000000 poetry_docker_plugin-0.4.0/setup.py
--rw-r--r--   0        0        0     4728 1970-01-01 00:00:00.000000 poetry_docker_plugin-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2022-10-09 20:19:34.073974 poetry_docker_plugin-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4165 2023-04-29 09:08:59.685183 poetry_docker_plugin-0.5.0/README.md
+-rw-r--r--   0        0        0      367 2023-01-13 13:04:47.288196 poetry_docker_plugin-0.5.0/poetry_docker_plugin/__init__.py
+-rw-r--r--   0        0        0    12116 2023-04-29 10:59:26.405292 poetry_docker_plugin-0.5.0/poetry_docker_plugin/docker_builder.py
+-rw-r--r--   0        0        0    13365 2023-04-29 10:49:16.141420 poetry_docker_plugin-0.5.0/poetry_docker_plugin/plugin.py
+-rw-r--r--   0        0        0     4186 2023-04-29 11:53:45.916789 poetry_docker_plugin-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6138 1970-01-01 00:00:00.000000 poetry_docker_plugin-0.5.0/PKG-INFO
```

### Comparing `poetry_docker_plugin-0.4.0/LICENSE` & `poetry_docker_plugin-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_docker_plugin-0.4.0/README.md` & `poetry_docker_plugin-0.5.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ![PyPI](https://img.shields.io/pypi/v/poetry-docker-plugin?color=gree&label=pypi%20package)
 [![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org)
 
 A [Poetry](https://python-poetry.org) plugin for configuring and building docker images directly from python projects.
 
 ## Installation
 
-In order to install the plugin you need to have installed a poetry version `>1.0` and type:
+In order to install the plugin you need to have installed a poetry version `>=1.2.0` and type:
 
 ```bash
 poetry self add poetry-docker-plugin
 ```
 
 ## Simple Example
 
@@ -33,25 +33,19 @@
 run_service = "app.service:start"
 ```
 
 your project also declares a poetry script that starts a service. Then, by adding the following minimal docker configuration in your `pyproject.toml` you can build your docker image:
 
 ```toml
 [tool.docker]
-copy = [
-    { source = "example_project-1.0.0.tar.gz", target = "/app/example_project.tar.gz" },
-]
-flow = [
-    { run = "pip install /app/example_project.tar.gz" },
-]
 expose = [8000]
 cmd = ["run_service"]
 ```
 
-Note that there is no docker [FROM](https://docs.docker.com/engine/reference/builder/#from)  command, and thus `poetry-docker-plugin` automatically figures out the python version and use `python:3.11` as the base image. Moreover, since we have not defined a name for the image, it derives one, using the first author name and the project name. Thus, by running the command `poetry docker`, poetry builds a docker image ready to run your service in port 8000.
+Note that there is no docker [FROM](https://docs.docker.com/engine/reference/builder/#from)  command, and thus `poetry-docker-plugin` automatically figures out the python version and use `python:3.11` as the base image. Moreover, since we have not defined a name for the image, it derives one, using the first author name and the project name. Thus, by running the command `poetry docker`, poetry builds a docker image ready to run your service in port `8000`. Under the hood, `poetry-docker-plugin` automatically packages the project, copy the distribution into the docker container and installs all dependencies.
  
 ## Docker Configuration Skeleton
 
 The configuration below outlines all supported commands:
 
 ```toml
 [tool.docker]
@@ -78,10 +72,52 @@
 
 then, as soon as you are done configuring, type:
 
 ```bash
 poetry docker
 ```
 
+## Multiple Docker Images
+
+In many projects, we would like to build more than one docker images from our project. For instance, Machine Learning engineers often need to build one image for the training procedure and one for service deployed in production after the training has been completed. To that end, `poetry-docker-plugin` supports multi-docker image configurations. 
+
+Consider again the following simple example:
+
+```toml
+[tool.poetry]
+name = "example_project"
+version = "1.0.0"
+description = "An example poetry project."
+authors = ["Evangelos"]
+
+[tool.poetry.dependencies]
+python = "3.11"
+
+[tool.poetry.scripts]
+run_service = "app.service:start"
+run_trainer = "trainer:start"
+```
+
+Note that the project now declares two poetry scripts, one that starts a service, and another one that runs some kind of training job. Then, we can define two docker configurations, one for each script, as follows:
+
+```toml
+[tool.docker.service]
+expose = [8000]
+cmd = ["run_service"]
+
+[tool.docker.trainer]
+cmd = ["run_trainer"]
+```
+
+By running `poetry docker`, the `poetry-docker-plugin` will detect both configurations and build two separate images, one for the service and one for the trainer.
+
+## Command-Line Options:
+
+The `docker` command provided by the `poetry-docker-plugin` has a couple of useful options. You can read about them by typing:
+
+```bash
+poetry docker --help
+```
+
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `poetry_docker_plugin-0.4.0/pyproject.toml` & `poetry_docker_plugin-0.5.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-docker-plugin"
-version = "0.4.0"
+version = "0.5.0"
 description = "A poetry plugin for configure and build docker images."
 authors = ["Evangelos Michelioudakis <vagmcs@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["poetry", "packaging", "docker"]
 repository = "https://github.com/vagmcs/poetry-docker-plugin"
 documentation = "https://github.com/vagmcs/poetry-docker-plugin"
@@ -33,22 +33,24 @@
 
 packages = [
     { include = "poetry_docker_plugin" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-poetry = "^1.1.0"
+poetry = "^1.2.0"
+gitpython = "^3.1.31"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.10.0"
-mypy = "^0.982"
+black = "^23.3.0"
+mypy = "^1.2.0"
 pytest = "^7.1.3"
-flake8 = "^3.9.2"
+ruff = "^0.0.263"
 isort = "^5.10.1"
+commitizen = "^3.1.1"
 
 # enforce types for safety using mypy
 [tool.mypy]
 python_version = 3.9
 exclude = ['.venv', 'dist']
 
 pretty = true
@@ -98,13 +100,60 @@
 known_typing = ["typing", "types", "typing_extensions", "mypy", "mypy_extensions"]
 import_heading_future="Futures"
 import_heading_stdlib="Standard Library"
 import_heading_typing="Types"
 import_heading_thirdparty="Dependencies"
 import_heading_firstparty="Project"
 
+[tool.ruff]
+line-length = 120
+target-version = "py39"
+
+# Exclude a variety of commonly ignored directories
+exclude = [
+    ".generated",
+    ".hypothesis",
+    ".eggs",
+    ".git",
+    ".mypy_cache",
+    ".nox",
+    ".ruff_cache",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    ".pytest_cache",
+    "build",
+    "dist",
+    "venv",
+    "*.pyi"
+]
+
 [tool.poetry.plugins."poetry.application.plugin"]
 docker = "poetry_docker_plugin.plugin:DockerPlugin"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.commitizen]
+name = "cz_customize"
+version = "0.2.0"
+tag_format = "v$version"
+
+[tool.commitizen.customize]
+change_type_order = ["BREAKING CHANGE", "feat", "build", "fix", "perf", "refactor", "style"]
+commit_parser = "^(?P<change_type>feature|feat|bug fix|bug|fix|perf|build|ci|docs|refactor):\\s(?P<message>.*)?"
+changelog_pattern = "^(feature|feat|bugfix|bug|fix|perf|build|ci|docs|refactor|perf)?(!)?"
+
+[tool.commitizen.customize.change_type_map]
+"feat" = "Features"
+"feature" = "Features"
+"bug fix" = "Fixes"
+"bugfix" = "Fixes"
+"bug" = "Fixes"
+"fix" = "Fixes"
+"ci" = "CI"
+"build" = "Build"
+"docs" = "Documentation"
+"refactor" = "Refactor"
+"perf" = "Performance"
+"style" = "Code style"
```


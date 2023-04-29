# Comparing `tmp/hyfi_template-0.1.9.tar.gz` & `tmp/hyfi_template-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi_template-0.1.9.tar", max compression
+gzip compressed data, was "hyfi_template-0.2.0.tar", max compression
```

## Comparing `hyfi_template-0.1.9.tar` & `hyfi_template-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0     1071 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/LICENSE
--rw-r--r--   0        0        0     6988 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/README.md
--rw-r--r--   0        0        0     3076 2023-04-21 11:36:41.769603 hyfi_template-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      181 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/__cli__.py
--rw-r--r--   0        0        0      882 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/__init__.py
--rw-r--r--   0        0        0       22 2023-04-21 11:36:41.713602 hyfi_template-0.1.9/src/hyfi_template/_version.py
--rw-r--r--   0        0        0        0 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/conf/project/__init__.yaml
--rw-r--r--   0        0        0       83 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/conf/task/__init__.yaml
--rw-r--r--   0        0        0      224 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/project.toml
--rw-r--r--   0        0        0        0 2023-04-21 11:36:11.853217 hyfi_template-0.1.9/src/hyfi_template/py.typed
--rw-r--r--   0        0        0     7634 1970-01-01 00:00:00.000000 hyfi_template-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-29 10:18:02.224290 hyfi_template-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2001 2023-04-29 10:18:02.224290 hyfi_template-0.2.0/README.md
+-rw-r--r--   0        0        0     2964 2023-04-29 10:18:26.744812 hyfi_template-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      181 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/__cli__.py
+-rw-r--r--   0        0        0      894 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-29 10:18:26.692811 hyfi_template-0.2.0/src/hyfi_template/_version.py
+-rw-r--r--   0        0        0        0 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/__init__.py
+-rw-r--r--   0        0        0      255 2023-04-29 10:18:26.692811 hyfi_template-0.2.0/src/hyfi_template/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/task/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/py.typed
+-rw-r--r--   0        0        0     2674 1970-01-01 00:00:00.000000 hyfi_template-0.2.0/PKG-INFO
```

### Comparing `hyfi_template-0.1.9/LICENSE` & `hyfi_template-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.9/pyproject.toml` & `hyfi_template-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 [tool.poetry]
 name = "hyfi-template"
-version = "0.1.9"
+version = "0.2.0"
 description = "A GitHub Template Repository for HyFI-based Projects"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi-template.entelecheia.ai"
+repository = "https://github.com/entelecheia/hyfi-template"
 readme = "README.md"
 packages = [{ include = "hyfi_template", from = "src" }]
 
 [tool.poetry.scripts]
 hyfi_template = 'hyfi_template.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = {extras = ["all"], version = "^0.2.6"}
-toml = "^0.10.2"
+hyfi = "^0.2.20"
+
+[tool.poetry.group.dev]
+optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
-setuptools-scm = "^7.1.0"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 flake8-pyproject = "^1.2.2"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
-ipykernel = "^6.22.0"
+
+[tool.poe]
+include = ".tasks.toml"
 
 [tool.black]
 exclude = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
 [tool.isort]
 profile = "black"
 skip = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
@@ -72,34 +76,29 @@
 addopts = "-p no:cacheprovider" # deactivating pytest caching.
 
 [tool.coverage.report]
 exclude_lines = ['if __name__ == "__main__":']
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.1"
 tag_format = "v$version"
 
-[tool.setuptools_scm]
-write_to_template = '__version__ = "{version}"'
-tag_regex = '^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$'
-
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/hyfi_template/_version.py:__version__"
+version_pattern = 'src/hyfi_template/conf/about/__init__.yaml:version: "{version}"'
 version_source = "tag"
 commit_version_number = true # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
-pre_commit_command = "make scm-version"
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
 build_command = "poetry build --no-cache"
 hvcs = "github" # hosting version control system, gitlab is also supported
 
 [build-system]
-requires = ["poetry-core>=1.0.0", "setuptools>=45", "setuptools_scm[toml]>=6.2"]
-build-backend = 'setuptools.build_meta'
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `hyfi_template-0.1.9/src/hyfi_template/conf/dotenv/__init__.yaml` & `hyfi_template-0.2.0/src/hyfi_template/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.9/src/hyfi_template/conf/hydra/help/help.yaml` & `hyfi_template-0.2.0/src/hyfi_template/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.9/src/hyfi_template/conf/mode/__init__.yaml` & `hyfi_template-0.2.0/src/hyfi_template/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.9/src/hyfi_template/conf/path/__default__.yaml` & `hyfi_template-0.2.0/src/hyfi_template/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.1.9/src/hyfi_template/conf/path/__init__.yaml` & `hyfi_template-0.2.0/src/hyfi_template/conf/path/__init__.yaml`

 * *Files identical despite different names*


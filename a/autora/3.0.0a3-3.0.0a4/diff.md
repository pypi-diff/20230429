# Comparing `tmp/autora-3.0.0a3.tar.gz` & `tmp/autora-3.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-3.0.0a3.tar", last modified: Fri Apr 28 22:14:29 2023, max compression
+gzip compressed data, was "autora-3.0.0a4.tar", last modified: Fri Apr 28 22:50:41 2023, max compression
```

## Comparing `autora-3.0.0a3.tar` & `autora-3.0.0a4.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.151320 autora-3.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-28 22:14:09.000000 autora-3.0.0a3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.139320 autora-3.0.0a3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 22:14:09.000000 autora-3.0.0a3/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-28 22:14:09.000000 autora-3.0.0a3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.143320 autora-3.0.0a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-28 22:14:09.000000 autora-3.0.0a3/.github/workflows/publish-documentation-gh-pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-28 22:14:09.000000 autora-3.0.0a3/.github/workflows/publish-package-anaconda-org.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-28 22:14:09.000000 autora-3.0.0a3/.github/workflows/publish-package-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 22:14:09.000000 autora-3.0.0a3/.github/workflows/test-conda-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-28 22:14:09.000000 autora-3.0.0a3/.github/workflows/test-poetry-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-28 22:14:09.000000 autora-3.0.0a3/.github/workflows/test-pre-commit-hooks.yml
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-28 22:14:09.000000 autora-3.0.0a3/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-28 22:14:09.000000 autora-3.0.0a3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.143320 autora-3.0.0a3/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-28 22:14:09.000000 autora-3.0.0a3/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-28 22:14:09.000000 autora-3.0.0a3/.idea/autora.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.143320 autora-3.0.0a3/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 22:14:09.000000 autora-3.0.0a3/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-28 22:14:09.000000 autora-3.0.0a3/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.143320 autora-3.0.0a3/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-28 22:14:09.000000 autora-3.0.0a3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-28 22:14:09.000000 autora-3.0.0a3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-28 22:14:09.000000 autora-3.0.0a3/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-28 22:14:09.000000 autora-3.0.0a3/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-28 22:14:09.000000 autora-3.0.0a3/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-28 22:14:09.000000 autora-3.0.0a3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.143320 autora-3.0.0a3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:09.000000 autora-3.0.0a3/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-28 22:14:09.000000 autora-3.0.0a3/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 22:14:09.000000 autora-3.0.0a3/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-28 22:14:09.000000 autora-3.0.0a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-04-28 22:14:29.147320 autora-3.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19356 2023-04-28 22:14:09.000000 autora-3.0.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.139320 autora-3.0.0a3/conda/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.143320 autora-3.0.0a3/conda/autora/
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-28 22:14:09.000000 autora-3.0.0a3/conda/autora/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 22:14:09.000000 autora-3.0.0a3/conda/autora/run_test.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.143320 autora-3.0.0a3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.143320 autora-3.0.0a3/docs/experiment-runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:09.000000 autora-3.0.0a3/docs/experiment-runner/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.143320 autora-3.0.0a3/docs/experimentalists/
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-28 22:14:09.000000 autora-3.0.0a3/docs/experimentalists/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.147320 autora-3.0.0a3/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    31814 2023-04-28 22:14:09.000000 autora-3.0.0a3/docs/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   389908 2023-04-28 22:14:09.000000 autora-3.0.0a3/docs/img/overview.png
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-28 22:14:09.000000 autora-3.0.0a3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.147320 autora-3.0.0a3/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-28 22:14:09.000000 autora-3.0.0a3/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.147320 autora-3.0.0a3/docs/theorist/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-28 22:14:09.000000 autora-3.0.0a3/docs/theorist/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.147320 autora-3.0.0a3/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-28 22:14:09.000000 autora-3.0.0a3/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-28 22:14:09.000000 autora-3.0.0a3/mkdocs/gen_ref_pages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.147320 autora-3.0.0a3/mkdocs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-28 22:14:09.000000 autora-3.0.0a3/mkdocs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-28 22:14:09.000000 autora-3.0.0a3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-28 22:14:09.000000 autora-3.0.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:14:29.151320 autora-3.0.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.147320 autora-3.0.0a3/src/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-28 22:14:09.000000 autora-3.0.0a3/src/.keep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:14:29.147320 autora-3.0.0a3/src/autora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-04-28 22:14:29.000000 autora-3.0.0a3/src/autora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-28 22:14:29.000000 autora-3.0.0a3/src/autora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:14:29.000000 autora-3.0.0a3/src/autora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-28 22:14:29.000000 autora-3.0.0a3/src/autora.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:14:29.000000 autora-3.0.0a3/src/autora.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.186652 autora-3.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-28 22:50:29.000000 autora-3.0.0a4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.182652 autora-3.0.0a4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 22:50:29.000000 autora-3.0.0a4/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-28 22:50:29.000000 autora-3.0.0a4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.182652 autora-3.0.0a4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-28 22:50:29.000000 autora-3.0.0a4/.github/workflows/publish-documentation-gh-pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-28 22:50:29.000000 autora-3.0.0a4/.github/workflows/publish-package-anaconda-org.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-28 22:50:29.000000 autora-3.0.0a4/.github/workflows/publish-package-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 22:50:29.000000 autora-3.0.0a4/.github/workflows/test-conda-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-28 22:50:29.000000 autora-3.0.0a4/.github/workflows/test-poetry-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-28 22:50:29.000000 autora-3.0.0a4/.github/workflows/test-pre-commit-hooks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-28 22:50:29.000000 autora-3.0.0a4/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-28 22:50:29.000000 autora-3.0.0a4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.182652 autora-3.0.0a4/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-28 22:50:29.000000 autora-3.0.0a4/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-28 22:50:29.000000 autora-3.0.0a4/.idea/autora.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.182652 autora-3.0.0a4/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 22:50:29.000000 autora-3.0.0a4/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-28 22:50:29.000000 autora-3.0.0a4/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.182652 autora-3.0.0a4/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-28 22:50:29.000000 autora-3.0.0a4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-28 22:50:29.000000 autora-3.0.0a4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-28 22:50:29.000000 autora-3.0.0a4/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-28 22:50:29.000000 autora-3.0.0a4/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-28 22:50:29.000000 autora-3.0.0a4/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-28 22:50:29.000000 autora-3.0.0a4/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.182652 autora-3.0.0a4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:29.000000 autora-3.0.0a4/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-28 22:50:29.000000 autora-3.0.0a4/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 22:50:29.000000 autora-3.0.0a4/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-28 22:50:29.000000 autora-3.0.0a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    21370 2023-04-28 22:50:41.186652 autora-3.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19356 2023-04-28 22:50:29.000000 autora-3.0.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.178652 autora-3.0.0a4/conda/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.182652 autora-3.0.0a4/conda/autora/
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-28 22:50:29.000000 autora-3.0.0a4/conda/autora/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 22:50:29.000000 autora-3.0.0a4/conda/autora/run_test.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.182652 autora-3.0.0a4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.182652 autora-3.0.0a4/docs/experiment-runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:29.000000 autora-3.0.0a4/docs/experiment-runner/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.182652 autora-3.0.0a4/docs/experimentalists/
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-28 22:50:29.000000 autora-3.0.0a4/docs/experimentalists/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.182652 autora-3.0.0a4/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    31814 2023-04-28 22:50:29.000000 autora-3.0.0a4/docs/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   389908 2023-04-28 22:50:29.000000 autora-3.0.0a4/docs/img/overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-28 22:50:29.000000 autora-3.0.0a4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.182652 autora-3.0.0a4/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-28 22:50:29.000000 autora-3.0.0a4/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.182652 autora-3.0.0a4/docs/theorist/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-28 22:50:29.000000 autora-3.0.0a4/docs/theorist/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.182652 autora-3.0.0a4/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-28 22:50:29.000000 autora-3.0.0a4/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-28 22:50:29.000000 autora-3.0.0a4/mkdocs/gen_ref_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.182652 autora-3.0.0a4/mkdocs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-28 22:50:29.000000 autora-3.0.0a4/mkdocs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-28 22:50:29.000000 autora-3.0.0a4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-28 22:50:29.000000 autora-3.0.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:50:41.186652 autora-3.0.0a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.186652 autora-3.0.0a4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-28 22:50:29.000000 autora-3.0.0a4/src/.keep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:50:41.186652 autora-3.0.0a4/src/autora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21370 2023-04-28 22:50:41.000000 autora-3.0.0a4/src/autora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-28 22:50:41.000000 autora-3.0.0a4/src/autora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:50:41.000000 autora-3.0.0a4/src/autora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-28 22:50:41.000000 autora-3.0.0a4/src/autora.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:50:41.000000 autora-3.0.0a4/src/autora.egg-info/top_level.txt
```

### Comparing `autora-3.0.0a3/.github/pull_request_template.md` & `autora-3.0.0a4/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/.github/workflows/publish-documentation-gh-pages.yml` & `autora-3.0.0a4/.github/workflows/publish-documentation-gh-pages.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/.github/workflows/publish-package-anaconda-org.yml` & `autora-3.0.0a4/.github/workflows/publish-package-anaconda-org.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/.github/workflows/publish-package-pypi.yml` & `autora-3.0.0a4/.github/workflows/publish-package-pypi.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/.github/workflows/test-conda-build.yml` & `autora-3.0.0a4/.github/workflows/test-conda-build.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/.github/workflows/test-pre-commit-hooks.yml` & `autora-3.0.0a4/.github/workflows/test-pre-commit-hooks.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/.github/workflows/test-pytest.yml` & `autora-3.0.0a4/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/.gitignore` & `autora-3.0.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/.idea/autora.iml` & `autora-3.0.0a4/.idea/autora.iml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/.idea/inspectionProfiles/Project_Default.xml` & `autora-3.0.0a4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/.idea/modules.xml` & `autora-3.0.0a4/.idea/modules.xml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/.pre-commit-config.yaml` & `autora-3.0.0a4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/LICENSE.md` & `autora-3.0.0a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/PKG-INFO` & `autora-3.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora
-Version: 3.0.0a3
+Version: 3.0.0a4
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process.
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 License: Copyright 2021, Brown University, Providence, RI.
         
                                 All Rights Reserved
         
         Permission to use, copy, modify, and distribute this software and
@@ -26,14 +26,15 @@
 Project-URL: homepage, https://www.empiricalresearch.ai/
 Project-URL: repository, https://github.com/AutoResearch/autora
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: all
 Provides-Extra: all-theorists
+Provides-Extra: theorist-darts
 Provides-Extra: all-experimentalists
 Provides-Extra: all-experiment-runners
 Provides-Extra: synthetic-experiments
 License-File: LICENSE.md
 
 # Automated Research Assistant
 Automated Research Assistant (AutoRA) is an open source AI-based system for automating each aspect of empirical research in the behavioral sciences, from the construction of a scientific hypothesis to conducting novel experiments. The documentation is here: [https://autoresearch.github.io/autora/](https://autoresearch.github.io/autora/)
```

### Comparing `autora-3.0.0a3/README.md` & `autora-3.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/conda/autora/meta.yaml` & `autora-3.0.0a4/conda/autora/meta.yaml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/docs/experimentalists/overview.md` & `autora-3.0.0a4/docs/experimentalists/overview.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/docs/img/logo.png` & `autora-3.0.0a4/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/docs/img/overview.png` & `autora-3.0.0a4/docs/img/overview.png`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/docs/index.md` & `autora-3.0.0a4/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/docs/theorist/overview.md` & `autora-3.0.0a4/docs/theorist/overview.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/mkdocs/base.yml` & `autora-3.0.0a4/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/mkdocs/gen_ref_pages.py` & `autora-3.0.0a4/mkdocs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/mkdocs.yml` & `autora-3.0.0a4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a3/pyproject.toml` & `autora-3.0.0a4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -23,25 +23,29 @@
   "autora[all-theorists]",
   "autora[all-experimentalists]",
   "autora[all-experiment-runners]",
   "autora[synthetic-experiments]",
 ]
 
 all-theorists = [
+  "autora[theorist-darts]",
+]
+theorist-darts = [
   "autora-theorist-darts",
 ]
 all-experimentalists = [
 ]
 all-experiment-runners = [
 ]
 synthetic-experiments = [
   "autora-synthetic-data"
 ]
 
 
+
 [project.urls]
 homepage = "https://www.empiricalresearch.ai/"
 repository = "https://github.com/AutoResearch/autora"
 documentation = "https://autoresearch.github.io/autora/"
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
```

### Comparing `autora-3.0.0a3/src/autora.egg-info/PKG-INFO` & `autora-3.0.0a4/src/autora.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora
-Version: 3.0.0a3
+Version: 3.0.0a4
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process.
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 License: Copyright 2021, Brown University, Providence, RI.
         
                                 All Rights Reserved
         
         Permission to use, copy, modify, and distribute this software and
@@ -26,14 +26,15 @@
 Project-URL: homepage, https://www.empiricalresearch.ai/
 Project-URL: repository, https://github.com/AutoResearch/autora
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: all
 Provides-Extra: all-theorists
+Provides-Extra: theorist-darts
 Provides-Extra: all-experimentalists
 Provides-Extra: all-experiment-runners
 Provides-Extra: synthetic-experiments
 License-File: LICENSE.md
 
 # Automated Research Assistant
 Automated Research Assistant (AutoRA) is an open source AI-based system for automating each aspect of empirical research in the behavioral sciences, from the construction of a scientific hypothesis to conducting novel experiments. The documentation is here: [https://autoresearch.github.io/autora/](https://autoresearch.github.io/autora/)
```

### Comparing `autora-3.0.0a3/src/autora.egg-info/SOURCES.txt` & `autora-3.0.0a4/src/autora.egg-info/SOURCES.txt`

 * *Files identical despite different names*


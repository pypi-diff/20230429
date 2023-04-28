# Comparing `tmp/autora-workflow-0.1.0.tar.gz` & `tmp/autora-workflow-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-workflow-0.1.0.tar", last modified: Thu Apr 27 23:27:06 2023, max compression
+gzip compressed data, was "autora-workflow-0.2.0.tar", last modified: Fri Apr 28 22:15:15 2023, max compression
```

## Comparing `autora-workflow-0.1.0.tar` & `autora-workflow-0.2.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.372820 autora-workflow-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.356819 autora-workflow-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.360819 autora-workflow-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.360819 autora-workflow-0.1.0/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.idea/autora-workflow.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.360819 autora-workflow-0.1.0/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.360819 autora-workflow-0.1.0/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.idea/other.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.360819 autora-workflow-0.1.0/.idea/runConfigurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.idea/runConfigurations/pytest_in_tests.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.360819 autora-workflow-0.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-27 23:27:06.372820 autora-workflow-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.360819 autora-workflow-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    17281 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/accessing-state-dependent-properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/basic-usage.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.356819 autora-workflow-0.1.0/docs/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.356819 autora-workflow-0.1.0/docs/cli/controller/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.360819 autora-workflow-0.1.0/docs/cli/controller/basic-usage/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/basic-usage/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/basic-usage/controller.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.360819 autora-workflow-0.1.0/docs/cli/controller/custom-function/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/custom-function/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/custom-function/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/custom-function/controller.yml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/custom-function/func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.364820 autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc/controller.yml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.364820 autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc/history/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc/history/00000000-METADATA.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc/history/00000001-PARAMS.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.364820 autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc-slurm/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc-slurm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc-slurm/controller.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc-slurm/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc-slurm/flow.cylc
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc-slurm/global.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.364820 autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc-slurm/history/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc-slurm/history/00000000-METADATA.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc-slurm/history/00000001-PARAMS.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.356819 autora-workflow-0.1.0/docs/cli/theorist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.368820 autora-workflow-0.1.0/docs/cli/theorist/basic-usage/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/theorist/basic-usage/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/theorist/basic-usage/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/theorist/basic-usage/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/theorist/basic-usage/parameters.yml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/theorist/basic-usage/regressor.yml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/cli/theorist/basic-usage/variables.yml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-27 23:26:52.000000 autora-workflow-0.1.0/docs/passing-static-parameters.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    32994 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/docs/using-alternative-planners-and-executors.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.368820 autora-workflow-0.1.0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/mkdocs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 23:27:06.372820 autora-workflow-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.356819 autora-workflow-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.356819 autora-workflow-0.1.0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.368820 autora-workflow-0.1.0/src/autora/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    23806 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/src/autora/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/src/autora/workflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/src/autora/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/src/autora/workflow/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/src/autora/workflow/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)    13894 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/src/autora/workflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/src/autora/workflow/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    20247 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/src/autora/workflow/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/src/autora/workflow/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.368820 autora-workflow-0.1.0/src/autora/workflow/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/src/autora/workflow/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/src/autora/workflow/serializer/yaml_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.372820 autora-workflow-0.1.0/src/autora/workflow/state/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/src/autora/workflow/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24565 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/src/autora/workflow/state/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/src/autora/workflow/state/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/src/autora/workflow/state/snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.372820 autora-workflow-0.1.0/src/autora_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-27 23:27:06.000000 autora-workflow-0.1.0/src/autora_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-27 23:27:06.000000 autora-workflow-0.1.0/src/autora_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:27:06.000000 autora-workflow-0.1.0/src/autora_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-27 23:27:06.000000 autora-workflow-0.1.0/src/autora_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 23:27:06.000000 autora-workflow-0.1.0/src/autora_workflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:27:06.372820 autora-workflow-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-04-27 23:26:53.000000 autora-workflow-0.1.0/tests/test_controller_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.791377 autora-workflow-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.771377 autora-workflow-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.779377 autora-workflow-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.783377 autora-workflow-0.2.0/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/autora-workflow.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.783377 autora-workflow-0.2.0/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.783377 autora-workflow-0.2.0/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/other.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.783377 autora-workflow-0.2.0/.idea/runConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/runConfigurations/pytest_in_tests.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.783377 autora-workflow-0.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-28 22:15:15.791377 autora-workflow-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.783377 autora-workflow-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/accessing-state-dependent-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22297 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/basic-usage.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.775377 autora-workflow-0.2.0/docs/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.775377 autora-workflow-0.2.0/docs/cli/controller/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.783377 autora-workflow-0.2.0/docs/cli/controller/basic-usage/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/basic-usage/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/basic-usage/controller.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.783377 autora-workflow-0.2.0/docs/cli/controller/custom-function/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function/controller.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function/func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.787377 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/controller.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.787377 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/history/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/history/00000000-METADATA.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/history/00000001-PARAMS.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.787377 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/controller.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/flow.cylc
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/global.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.787377 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/history/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/history/00000000-METADATA.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/history/00000001-PARAMS.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.775377 autora-workflow-0.2.0/docs/cli/theorist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.787377 autora-workflow-0.2.0/docs/cli/theorist/basic-usage/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/theorist/basic-usage/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/theorist/basic-usage/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/theorist/basic-usage/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/theorist/basic-usage/parameters.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/theorist/basic-usage/regressor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/theorist/basic-usage/variables.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/passing-static-parameters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31206 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/using-alternative-planners-and-executors.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.787377 autora-workflow-0.2.0/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/mkdocs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:15:15.791377 autora-workflow-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.779377 autora-workflow-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.779377 autora-workflow-0.2.0/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.791377 autora-workflow-0.2.0/src/autora/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    23734 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.791377 autora-workflow-0.2.0/src/autora/workflow/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/serializer/yaml_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.791377 autora-workflow-0.2.0/src/autora/workflow/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24555 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/state/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/state/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/state/snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.791377 autora-workflow-0.2.0/src/autora_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-28 22:15:15.000000 autora-workflow-0.2.0/src/autora_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-28 22:15:15.000000 autora-workflow-0.2.0/src/autora_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:15:15.000000 autora-workflow-0.2.0/src/autora_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 22:15:15.000000 autora-workflow-0.2.0/src/autora_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 22:15:15.000000 autora-workflow-0.2.0/src/autora_workflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.791377 autora-workflow-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/tests/test_controller_plots.py
```

### Comparing `autora-workflow-0.1.0/.github/workflows/python-publish.yml` & `autora-workflow-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/.gitignore` & `autora-workflow-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/.idea/autora-workflow.iml` & `autora-workflow-0.2.0/.idea/autora-workflow.iml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/.idea/inspectionProfiles/Project_Default.xml` & `autora-workflow-0.2.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/.idea/runConfigurations/pytest_in_tests.xml` & `autora-workflow-0.2.0/.idea/runConfigurations/pytest_in_tests.xml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/.pre-commit-config.yaml` & `autora-workflow-0.2.0/.pre-commit-config.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 repos:
-  - repo: https://github.com/ambv/black
-    rev: 22.12.0
-    hooks:
-      - id: black
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
-        args:
-        - "--profile=black"
-        - "--filter-files"
-        - "--project=autora"
+  - repo: https://github.com/ambv/black
+    rev: 23.3.0
+    hooks:
+      - id: black
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         args:
         - "--max-line-length=100"
-        - "--extend-ignore=E203"
         - "--per-file-ignores=__init__.py:F401"
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v0.991"
+    rev: "v1.2.0"
     hooks:
       - id: mypy
         additional_dependencies: [types-requests,types-PyYAML]
         language_version: python3.8
 default_language_version:
   python: python3
```

### Comparing `autora-workflow-0.1.0/LICENSE.md` & `autora-workflow-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/PKG-INFO` & `autora-workflow-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-workflow
-Version: 0.1.0
+Version: 0.2.0
 Summary: Workflow tools for the Autonomous Research Assistant (AutoRA) package.
 Author-email: John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
 Project-URL: homepage, https://www.empiricalresearch.ai/
 Project-URL: repository, https://github.com/AutoResearch/autora-workflow
 Project-URL: documentation, https://hollandjg.github.io/autora-workflow/
 Description-Content-Type: text/markdown
```

### Comparing `autora-workflow-0.1.0/docs/accessing-state-dependent-properties.ipynb` & `autora-workflow-0.2.0/docs/accessing-state-dependent-properties.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986598557692308%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'to the current best model or the observed data. These "*

 * *            'data update each cycle, and\\n\'), (17, \'- `"%models[-1]%"`: the last fitted '*

 * *            'theorist\\n\'), (18, \'- `"%models%"`: all the fitted theorists\\n\')], delete: [18, '*

 * *            "17, 4]}}, 1: {'metadata': {'ExecuteTime': {'start_time': "*

 * *            "'2023-04-28T16:00:29.742026Z', 'end_time': '2023-04-28T16:00:30.440209Z'}}}, 2: "*

 * *            "{'metadata': {'ExecuteTime': {'start_tim […]*

```diff
@@ -6,42 +6,42 @@
                 "collapsed": false
             },
             "source": [
                 "# Accessing \"State-dependent Properties\"\n",
                 "\n",
                 "Some experimentalists, experiment runners and theorists require access to the values\n",
                 "created during the cycle execution, e.g. experimentalists which require access\n",
-                "to the current best theory or the observed data. These data update each cycle, and\n",
+                "to the current best model or the observed data. These data update each cycle, and\n",
                 "so cannot easily be set using simple `params`.\n",
                 "\n",
                 "For this case, it is possible to use \"state-dependent properties\" in the `params`\n",
                 "dictionary. These are the following strings, which will be replaced during execution by\n",
                 "their respective current values:\n",
                 "\n",
                 "- `\"%observations.ivs[-1]%\"`: the last observed independent variables\n",
                 "- `\"%observations.dvs[-1]%\"`: the last observed dependent variables\n",
                 "- `\"%observations.ivs%\"`: all the observed independent variables,\n",
                 "concatenated into a single array\n",
                 "- `\"%observations.dvs%\"`: all the observed dependent variables,\n",
                 "concatenated into a single array\n",
-                "- `\"%theories[-1]%\"`: the last fitted theorist\n",
-                "- `\"%theories%\"`: all the fitted theorists\n",
+                "- `\"%models[-1]%\"`: the last fitted theorist\n",
+                "- `\"%models%\"`: all the fitted theorists\n",
                 "\n",
                 "In the following example, we use the `\"observations.ivs\"` cycle property for an\n",
                 "experimentalist which excludes those conditions which have\n",
                 "already been seen."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:19:32.016846Z",
-                    "start_time": "2023-04-27T18:18:41.353526Z"
+                    "end_time": "2023-04-28T16:00:30.440209Z",
+                    "start_time": "2023-04-28T16:00:29.742026Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from autora.experimentalist.pipeline import make_pipeline\n",
@@ -54,16 +54,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:19:32.022389Z",
-                    "start_time": "2023-04-27T18:19:32.020700Z"
+                    "end_time": "2023-04-28T16:00:30.444929Z",
+                    "start_time": "2023-04-28T16:00:30.443462Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "def ground_truth(x):\n",
                 "    return x + 1\n",
@@ -123,16 +123,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:19:32.035430Z",
-                    "start_time": "2023-04-27T18:19:32.027349Z"
+                    "end_time": "2023-04-28T16:00:30.456532Z",
+                    "start_time": "2023-04-28T16:00:30.451649Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>x</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>0</th>\n      <td>2</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
@@ -157,16 +157,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:19:32.078698Z",
-                    "start_time": "2023-04-27T18:19:32.039653Z"
+                    "end_time": "2023-04-28T16:00:30.484920Z",
+                    "start_time": "2023-04-28T16:00:30.460205Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>x</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>0</th>\n      <td>1</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
@@ -202,19 +202,19 @@
                     "ename": "ValueError",
                     "evalue": "a cannot be empty unless no samples are taken",
                     "output_type": "error",
                     "traceback": [
                         "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
                         "\u001b[0;31mValueError\u001b[0m                                Traceback (most recent call last)",
                         "Cell \u001b[0;32mIn[5], line 1\u001b[0m\n\u001b[0;32m----> 1\u001b[0m \u001b[43mcycle_with_state_dep_properties\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mrun\u001b[49m\u001b[43m(\u001b[49m\u001b[43m)\u001b[49m  \u001b[38;5;66;03m# doctest: +ELLIPSIS\u001b[39;00m\n",
-                        "File \u001b[0;32m~/Developer/autora-workflow/src/autora/workflow/cycle.py:83\u001b[0m, in \u001b[0;36mCycle.run\u001b[0;34m(self, num_cycles)\u001b[0m\n\u001b[1;32m     81\u001b[0m \u001b[38;5;28;01mdef\u001b[39;00m \u001b[38;5;21mrun\u001b[39m(\u001b[38;5;28mself\u001b[39m, num_cycles: \u001b[38;5;28mint\u001b[39m \u001b[38;5;241m=\u001b[39m \u001b[38;5;241m1\u001b[39m):\n\u001b[1;32m     82\u001b[0m \u001b[38;5;250m    \u001b[39m\u001b[38;5;124;03m\"\"\"Execute the next step in the cycle.\"\"\"\u001b[39;00m\n\u001b[0;32m---> 83\u001b[0m     \u001b[38;5;28;43msuper\u001b[39;49m\u001b[43m(\u001b[49m\u001b[43m)\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mrun\u001b[49m\u001b[43m(\u001b[49m\u001b[43mnum_steps\u001b[49m\u001b[38;5;241;43m=\u001b[39;49m\u001b[43mnum_cycles\u001b[49m\u001b[43m)\u001b[49m\n\u001b[1;32m     84\u001b[0m     \u001b[38;5;28;01mreturn\u001b[39;00m \u001b[38;5;28mself\u001b[39m\n",
+                        "File \u001b[0;32m~/Developer/autora-workflow/src/autora/workflow/cycle.py:82\u001b[0m, in \u001b[0;36mCycle.run\u001b[0;34m(self, num_cycles)\u001b[0m\n\u001b[1;32m     80\u001b[0m \u001b[38;5;28;01mdef\u001b[39;00m \u001b[38;5;21mrun\u001b[39m(\u001b[38;5;28mself\u001b[39m, num_cycles: \u001b[38;5;28mint\u001b[39m \u001b[38;5;241m=\u001b[39m \u001b[38;5;241m1\u001b[39m):\n\u001b[1;32m     81\u001b[0m \u001b[38;5;250m    \u001b[39m\u001b[38;5;124;03m\"\"\"Execute the next step in the cycle.\"\"\"\u001b[39;00m\n\u001b[0;32m---> 82\u001b[0m     \u001b[38;5;28;43msuper\u001b[39;49m\u001b[43m(\u001b[49m\u001b[43m)\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mrun\u001b[49m\u001b[43m(\u001b[49m\u001b[43mnum_steps\u001b[49m\u001b[38;5;241;43m=\u001b[39;49m\u001b[43mnum_cycles\u001b[49m\u001b[43m)\u001b[49m\n\u001b[1;32m     83\u001b[0m     \u001b[38;5;28;01mreturn\u001b[39;00m \u001b[38;5;28mself\u001b[39m\n",
                         "File \u001b[0;32m~/Developer/autora-workflow/src/autora/workflow/base.py:59\u001b[0m, in \u001b[0;36mBaseController.run\u001b[0;34m(self, num_steps)\u001b[0m\n\u001b[1;32m     57\u001b[0m \u001b[38;5;250m\u001b[39m\u001b[38;5;124;03m\"\"\"Execute the next step in the cycle.\"\"\"\u001b[39;00m\n\u001b[1;32m     58\u001b[0m \u001b[38;5;28;01mfor\u001b[39;00m i \u001b[38;5;129;01min\u001b[39;00m \u001b[38;5;28mrange\u001b[39m(num_steps):\n\u001b[0;32m---> 59\u001b[0m     \u001b[38;5;28mnext\u001b[39m(\u001b[38;5;28mself\u001b[39m)\n\u001b[1;32m     60\u001b[0m \u001b[38;5;28;01mreturn\u001b[39;00m \u001b[38;5;28mself\u001b[39m\n",
-                        "File \u001b[0;32m~/Developer/autora-workflow/src/autora/workflow/base.py:72\u001b[0m, in \u001b[0;36mBaseController.__next__\u001b[0;34m(self)\u001b[0m\n\u001b[1;32m     69\u001b[0m next_params \u001b[38;5;241m=\u001b[39m \u001b[38;5;28mself\u001b[39m\u001b[38;5;241m.\u001b[39mstate\u001b[38;5;241m.\u001b[39mparams\u001b[38;5;241m.\u001b[39mget(next_function_name, {})\n\u001b[1;32m     71\u001b[0m \u001b[38;5;66;03m# Execute\u001b[39;00m\n\u001b[0;32m---> 72\u001b[0m result \u001b[38;5;241m=\u001b[39m \u001b[43mnext_function\u001b[49m\u001b[43m(\u001b[49m\u001b[38;5;28;43mself\u001b[39;49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mstate\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[43mparams\u001b[49m\u001b[38;5;241;43m=\u001b[39;49m\u001b[43mnext_params\u001b[49m\u001b[43m)\u001b[49m\n\u001b[1;32m     74\u001b[0m \u001b[38;5;66;03m# Update\u001b[39;00m\n\u001b[1;32m     75\u001b[0m \u001b[38;5;28mself\u001b[39m\u001b[38;5;241m.\u001b[39mstate \u001b[38;5;241m=\u001b[39m result\n",
-                        "File \u001b[0;32m~/Developer/autora-workflow/src/autora/workflow/executor.py:129\u001b[0m, in \u001b[0;36mfull_cycle_wrapper\u001b[0;34m(state, experimentalist_pipeline, experiment_runner_callable, theorist_estimator, params)\u001b[0m\n\u001b[1;32m    127\u001b[0m \u001b[38;5;250m\u001b[39m\u001b[38;5;124;03m\"\"\"Interface for running the full AER cycle.\"\"\"\u001b[39;00m\n\u001b[1;32m    128\u001b[0m experimentalist_params \u001b[38;5;241m=\u001b[39m params\u001b[38;5;241m.\u001b[39mget(\u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mexperimentalist\u001b[39m\u001b[38;5;124m\"\u001b[39m, {})\n\u001b[0;32m--> 129\u001b[0m experimentalist_result \u001b[38;5;241m=\u001b[39m \u001b[43mexperimentalist_wrapper\u001b[49m\u001b[43m(\u001b[49m\n\u001b[1;32m    130\u001b[0m \u001b[43m    \u001b[49m\u001b[43mstate\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[43mexperimentalist_pipeline\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[43mexperimentalist_params\u001b[49m\n\u001b[1;32m    131\u001b[0m \u001b[43m\u001b[49m\u001b[43m)\u001b[49m\n\u001b[1;32m    132\u001b[0m experiment_runner_params \u001b[38;5;241m=\u001b[39m params\u001b[38;5;241m.\u001b[39mget(\u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mexperiment_runner\u001b[39m\u001b[38;5;124m\"\u001b[39m, {})\n\u001b[1;32m    133\u001b[0m experiment_runner_result \u001b[38;5;241m=\u001b[39m experiment_runner_wrapper(\n\u001b[1;32m    134\u001b[0m     experimentalist_result, experiment_runner_callable, experiment_runner_params\n\u001b[1;32m    135\u001b[0m )\n",
-                        "File \u001b[0;32m~/Developer/autora-workflow/src/autora/workflow/executor.py:31\u001b[0m, in \u001b[0;36mexperimentalist_wrapper\u001b[0;34m(state, pipeline, params)\u001b[0m\n\u001b[1;32m     29\u001b[0m \u001b[38;5;250m\u001b[39m\u001b[38;5;124;03m\"\"\"Interface for running the experimentalist pipeline.\"\"\"\u001b[39;00m\n\u001b[1;32m     30\u001b[0m params_ \u001b[38;5;241m=\u001b[39m resolve_state_params(params, state)\n\u001b[0;32m---> 31\u001b[0m new_conditions \u001b[38;5;241m=\u001b[39m \u001b[43mpipeline\u001b[49m\u001b[43m(\u001b[49m\u001b[38;5;241;43m*\u001b[39;49m\u001b[38;5;241;43m*\u001b[39;49m\u001b[43mparams_\u001b[49m\u001b[43m)\u001b[49m\n\u001b[1;32m     33\u001b[0m \u001b[38;5;28;01mif\u001b[39;00m \u001b[38;5;28misinstance\u001b[39m(new_conditions, pd\u001b[38;5;241m.\u001b[39mDataFrame):\n\u001b[1;32m     34\u001b[0m     new_conditions_array \u001b[38;5;241m=\u001b[39m new_conditions\n",
+                        "File \u001b[0;32m~/Developer/autora-workflow/src/autora/workflow/base.py:71\u001b[0m, in \u001b[0;36mBaseController.__next__\u001b[0;34m(self)\u001b[0m\n\u001b[1;32m     68\u001b[0m next_params \u001b[38;5;241m=\u001b[39m \u001b[38;5;28mself\u001b[39m\u001b[38;5;241m.\u001b[39mstate\u001b[38;5;241m.\u001b[39mparams\u001b[38;5;241m.\u001b[39mget(next_function_name, {})\n\u001b[1;32m     70\u001b[0m \u001b[38;5;66;03m# Execute\u001b[39;00m\n\u001b[0;32m---> 71\u001b[0m result \u001b[38;5;241m=\u001b[39m \u001b[43mnext_function\u001b[49m\u001b[43m(\u001b[49m\u001b[38;5;28;43mself\u001b[39;49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mstate\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[43mparams\u001b[49m\u001b[38;5;241;43m=\u001b[39;49m\u001b[43mnext_params\u001b[49m\u001b[43m)\u001b[49m\n\u001b[1;32m     73\u001b[0m \u001b[38;5;66;03m# Update\u001b[39;00m\n\u001b[1;32m     74\u001b[0m \u001b[38;5;28mself\u001b[39m\u001b[38;5;241m.\u001b[39mstate \u001b[38;5;241m=\u001b[39m result\n",
+                        "File \u001b[0;32m~/Developer/autora-workflow/src/autora/workflow/executor.py:128\u001b[0m, in \u001b[0;36mfull_cycle_wrapper\u001b[0;34m(state, experimentalist_pipeline, experiment_runner_callable, theorist_estimator, params)\u001b[0m\n\u001b[1;32m    126\u001b[0m \u001b[38;5;250m\u001b[39m\u001b[38;5;124;03m\"\"\"Interface for running the full AER cycle.\"\"\"\u001b[39;00m\n\u001b[1;32m    127\u001b[0m experimentalist_params \u001b[38;5;241m=\u001b[39m params\u001b[38;5;241m.\u001b[39mget(\u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mexperimentalist\u001b[39m\u001b[38;5;124m\"\u001b[39m, {})\n\u001b[0;32m--> 128\u001b[0m experimentalist_result \u001b[38;5;241m=\u001b[39m \u001b[43mexperimentalist_wrapper\u001b[49m\u001b[43m(\u001b[49m\n\u001b[1;32m    129\u001b[0m \u001b[43m    \u001b[49m\u001b[43mstate\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[43mexperimentalist_pipeline\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[43mexperimentalist_params\u001b[49m\n\u001b[1;32m    130\u001b[0m \u001b[43m\u001b[49m\u001b[43m)\u001b[49m\n\u001b[1;32m    131\u001b[0m experiment_runner_params \u001b[38;5;241m=\u001b[39m params\u001b[38;5;241m.\u001b[39mget(\u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mexperiment_runner\u001b[39m\u001b[38;5;124m\"\u001b[39m, {})\n\u001b[1;32m    132\u001b[0m experiment_runner_result \u001b[38;5;241m=\u001b[39m experiment_runner_wrapper(\n\u001b[1;32m    133\u001b[0m     experimentalist_result, experiment_runner_callable, experiment_runner_params\n\u001b[1;32m    134\u001b[0m )\n",
+                        "File \u001b[0;32m~/Developer/autora-workflow/src/autora/workflow/executor.py:30\u001b[0m, in \u001b[0;36mexperimentalist_wrapper\u001b[0;34m(state, pipeline, params)\u001b[0m\n\u001b[1;32m     28\u001b[0m \u001b[38;5;250m\u001b[39m\u001b[38;5;124;03m\"\"\"Interface for running the experimentalist pipeline.\"\"\"\u001b[39;00m\n\u001b[1;32m     29\u001b[0m params_ \u001b[38;5;241m=\u001b[39m resolve_state_params(params, state)\n\u001b[0;32m---> 30\u001b[0m new_conditions \u001b[38;5;241m=\u001b[39m \u001b[43mpipeline\u001b[49m\u001b[43m(\u001b[49m\u001b[38;5;241;43m*\u001b[39;49m\u001b[38;5;241;43m*\u001b[39;49m\u001b[43mparams_\u001b[49m\u001b[43m)\u001b[49m\n\u001b[1;32m     32\u001b[0m \u001b[38;5;28;01mif\u001b[39;00m \u001b[38;5;28misinstance\u001b[39m(new_conditions, pd\u001b[38;5;241m.\u001b[39mDataFrame):\n\u001b[1;32m     33\u001b[0m     new_conditions_array \u001b[38;5;241m=\u001b[39m new_conditions\n",
                         "File \u001b[0;32m~/Developer/autora-core/src/autora/experimentalist/pipeline.py:171\u001b[0m, in \u001b[0;36mPipeline.__call__\u001b[0;34m(self, ex, **params)\u001b[0m\n\u001b[1;32m    169\u001b[0m     \u001b[38;5;28;01massert\u001b[39;00m \u001b[38;5;28misinstance\u001b[39m(pipe, Pipe)\n\u001b[1;32m    170\u001b[0m     all_params_for_pipe \u001b[38;5;241m=\u001b[39m merged_params\u001b[38;5;241m.\u001b[39mget(name, \u001b[38;5;28mdict\u001b[39m())\n\u001b[0;32m--> 171\u001b[0m     results\u001b[38;5;241m.\u001b[39mappend(\u001b[43mpipe\u001b[49m\u001b[43m(\u001b[49m\u001b[43mresults\u001b[49m\u001b[43m[\u001b[49m\u001b[38;5;241;43m-\u001b[39;49m\u001b[38;5;241;43m1\u001b[39;49m\u001b[43m]\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[38;5;241;43m*\u001b[39;49m\u001b[38;5;241;43m*\u001b[39;49m\u001b[43mall_params_for_pipe\u001b[49m\u001b[43m)\u001b[49m)\n\u001b[1;32m    173\u001b[0m \u001b[38;5;28;01mreturn\u001b[39;00m results[\u001b[38;5;241m-\u001b[39m\u001b[38;5;241m1\u001b[39m]\n",
                         "Cell \u001b[0;32mIn[2], line 9\u001b[0m, in \u001b[0;36mcustom_random_sampler\u001b[0;34m(conditions, n)\u001b[0m\n\u001b[1;32m      8\u001b[0m \u001b[38;5;28;01mdef\u001b[39;00m \u001b[38;5;21mcustom_random_sampler\u001b[39m(conditions, n):\n\u001b[0;32m----> 9\u001b[0m     sampled_conditions \u001b[38;5;241m=\u001b[39m \u001b[43mrandom_sampler_rng\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mchoice\u001b[49m\u001b[43m(\u001b[49m\u001b[43mconditions\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[43msize\u001b[49m\u001b[38;5;241;43m=\u001b[39;49m\u001b[43mn\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[43mreplace\u001b[49m\u001b[38;5;241;43m=\u001b[39;49m\u001b[38;5;28;43;01mFalse\u001b[39;49;00m\u001b[43m)\u001b[49m\n\u001b[1;32m     10\u001b[0m     \u001b[38;5;28;01mreturn\u001b[39;00m sampled_conditions\n",
                         "File \u001b[0;32m_generator.pyx:729\u001b[0m, in \u001b[0;36mnumpy.random._generator.Generator.choice\u001b[0;34m()\u001b[0m\n",
                         "\u001b[0;31mValueError\u001b[0m: a cannot be empty unless no samples are taken"
                     ]
                 }
             ],
@@ -223,16 +223,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:20:17.726364Z",
-                    "start_time": "2023-04-27T18:20:17.720389Z"
+                    "end_time": "2023-04-28T16:00:58.158434Z",
+                    "start_time": "2023-04-28T16:00:58.149168Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>x</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>0</th>\n      <td>2</td>\n    </tr>\n    <tr>\n      <th>1</th>\n      <td>6</td>\n    </tr>\n    <tr>\n      <th>2</th>\n      <td>5</td>\n    </tr>\n    <tr>\n      <th>3</th>\n      <td>7</td>\n    </tr>\n    <tr>\n      <th>4</th>\n      <td>3</td>\n    </tr>\n    <tr>\n      <th>5</th>\n      <td>4</td>\n    </tr>\n    <tr>\n      <th>6</th>\n      <td>9</td>\n    </tr>\n    <tr>\n      <th>7</th>\n      <td>0</td>\n    </tr>\n    <tr>\n      <th>8</th>\n      <td>8</td>\n    </tr>\n    <tr>\n      <th>9</th>\n      <td>1</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
```

### Comparing `autora-workflow-0.1.0/docs/basic-usage.ipynb` & `autora-workflow-0.2.0/docs/basic-usage.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9942298418209876%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'Aim: Use the Controller to recover a simple ground "*

 * *            "truth model from noisy data.')], delete: [2]}}, 1: {'metadata': {'ExecuteTime': "*

 * *            "{'start_time': '2023-04-28T16:00:28.742319Z', 'end_time': "*

 * *            "'2023-04-28T16:00:29.593823Z'}}}, 2: {'metadata': {'ExecuteTime': {'start_time': "*

 * *            "'2023-04-28T16:00:29.594123Z', 'end_time': '2023-04-28T16:00:29.595804Z'}}}, 4: "*

 * *            "{'metadata': {'ExecuteTime': {'start_time':  […]*

```diff
@@ -4,24 +4,24 @@
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
                 "# Basic Usage\n",
                 "\n",
-                "Aim: Use the Controller to recover a simple ground truth theory from noisy data."
+                "Aim: Use the Controller to recover a simple ground truth model from noisy data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.360541Z",
-                    "start_time": "2023-04-27T18:57:33.362276Z"
+                    "end_time": "2023-04-28T16:00:29.593823Z",
+                    "start_time": "2023-04-28T16:00:28.742319Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from autora.experimentalist.pipeline import make_pipeline\n",
@@ -33,16 +33,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.363376Z",
-                    "start_time": "2023-04-27T18:57:34.361158Z"
+                    "end_time": "2023-04-28T16:00:29.595804Z",
+                    "start_time": "2023-04-28T16:00:29.594123Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "def ground_truth(x):\n",
                 "    return x + 1"
@@ -58,16 +58,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.366884Z",
-                    "start_time": "2023-04-27T18:57:34.364465Z"
+                    "end_time": "2023-04-28T16:00:29.599669Z",
+                    "start_time": "2023-04-28T16:00:29.596722Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "metadata_0 = VariableCollection(\n",
                 "   independent_variables=[Variable(name=\"x1\", allowed_values=range(11))],\n",
@@ -86,16 +86,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.369981Z",
-                    "start_time": "2023-04-27T18:57:34.367394Z"
+                    "end_time": "2023-04-28T16:00:29.602835Z",
+                    "start_time": "2023-04-28T16:00:29.600797Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "example_experimentalist = make_pipeline(\n",
                 "    [metadata_0.independent_variables[0].allowed_values])"
@@ -111,16 +111,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.377470Z",
-                    "start_time": "2023-04-27T18:57:34.373873Z"
+                    "end_time": "2023-04-28T16:00:29.607989Z",
+                    "start_time": "2023-04-28T16:00:29.605654Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "array([2.04339546])"
@@ -142,70 +142,70 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "The theorist \"tries\" to work out the best theory. We use a trivial scikit-learn regressor."
+                "The theorist \"tries\" to work out the best model. We use a trivial scikit-learn regressor."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.379489Z",
-                    "start_time": "2023-04-27T18:57:34.376879Z"
+                    "end_time": "2023-04-28T16:00:29.610805Z",
+                    "start_time": "2023-04-28T16:00:29.608494Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "example_theorist = LinearRegression()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "    We initialize the Controller with the metadata describing the domain of the theory,\n",
+                "    We initialize the Controller with the metadata describing the domain of the model,\n",
                 "    the theorist, experimentalist and experiment runner,\n",
                 "    as well as a monitor which will let us know which cycle we're currently on."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.389200Z",
-                    "start_time": "2023-04-27T18:57:34.380758Z"
+                    "end_time": "2023-04-28T16:00:29.620255Z",
+                    "start_time": "2023-04-28T16:00:29.615491Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "<autora.workflow.cycle.Cycle at 0x17cd8b410>"
+                        "text/plain": "<autora.workflow.cycle.Cycle at 0x14d254910>"
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "cycle = Cycle(\n",
                 "    metadata=metadata_0,\n",
                 "    theorist=example_theorist,\n",
                 "    experimentalist=example_experimentalist,\n",
                 "    experiment_runner=example_synthetic_experiment_runner,\n",
-                "    monitor=lambda state: print(f\"Generated {len(state.theories)} theories\"),\n",
+                "    monitor=lambda state: print(f\"Generated {len(state.models)} models\"),\n",
                 ")\n",
                 "cycle # doctest: +ELLIPSIS"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -216,27 +216,27 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.389887Z",
-                    "start_time": "2023-04-27T18:57:34.384943Z"
+                    "end_time": "2023-04-28T16:00:29.625412Z",
+                    "start_time": "2023-04-28T16:00:29.618752Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Generated 1 theories\n",
-                        "Generated 2 theories\n",
-                        "Generated 3 theories\n"
+                        "Generated 1 models\n",
+                        "Generated 2 models\n",
+                        "Generated 3 models\n"
                     ]
                 }
             ],
             "source": [
                 "_ = cycle.run(num_cycles=3)"
             ]
         },
@@ -251,16 +251,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.394835Z",
-                    "start_time": "2023-04-27T18:57:34.391258Z"
+                    "end_time": "2023-04-28T16:00:29.627948Z",
+                    "start_time": "2023-04-28T16:00:29.624167Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "array([ 0,  1,  2,  3,  4,  5,  6,  7,  8,  9, 10])"
@@ -284,16 +284,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.398947Z",
-                    "start_time": "2023-04-27T18:57:34.395044Z"
+                    "end_time": "2023-04-28T16:00:29.631975Z",
+                    "start_time": "2023-04-28T16:00:29.629640Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "array([[ 0.        ,  0.92675345],\n       [ 1.        ,  1.89519928],\n       [ 2.        ,  3.08746571],\n       [ 3.        ,  3.93023943],\n       [ 4.        ,  4.95429102],\n       [ 5.        ,  6.04763988],\n       [ 6.        ,  7.20770574],\n       [ 7.        ,  7.85681519],\n       [ 8.        ,  9.05735823],\n       [ 9.        , 10.18713406],\n       [10.        , 10.88517906]])"
@@ -317,16 +317,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.402482Z",
-                    "start_time": "2023-04-27T18:57:34.399606Z"
+                    "end_time": "2023-04-28T16:00:29.635291Z",
+                    "start_time": "2023-04-28T16:00:29.633048Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "array([[ 0.        ,  1.08559827],\n       [10.        , 11.08179553]])"
@@ -342,24 +342,24 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "The best fit theory after the first cycle is:"
+                "The best fit model after the first cycle is:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.406845Z",
-                    "start_time": "2023-04-27T18:57:34.403505Z"
+                    "end_time": "2023-04-28T16:00:29.638810Z",
+                    "start_time": "2023-04-28T16:00:29.636568Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": "<style>#sk-container-id-1 {color: black;background-color: white;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 div.sk-toggleable {background-color: white;}#sk-container-id-1 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-1 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-1 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-1 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-1 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-1 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-1 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-1 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-1 div.sk-item {position: relative;z-index: 1;}#sk-container-id-1 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-1 div.sk-item::before, #sk-container-id-1 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-1 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-1 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-1 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-1 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-1 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-1 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-1 div.sk-label-container {text-align: center;}#sk-container-id-1 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-1 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-1\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>LinearRegression()</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-1\" type=\"checkbox\" checked><label for=\"sk-estimator-id-1\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">LinearRegression</label><div class=\"sk-toggleable__content\"><pre>LinearRegression()</pre></div></div></div></div></div>",
@@ -367,24 +367,24 @@
                     },
                     "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "cycle.data.theories[0]"
+                "cycle.data.models[0]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.424584Z",
-                    "start_time": "2023-04-27T18:57:34.407871Z"
+                    "end_time": "2023-04-28T16:00:29.651434Z",
+                    "start_time": "2023-04-28T16:00:29.640123Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "'y = 1.0089 x + 0.9589'"
@@ -395,162 +395,162 @@
                 }
             ],
             "source": [
                 "def report_linear_fit(m: LinearRegression,  precision=4):\n",
                 "    s = f\"y = {np.round(m.coef_[0].item(), precision)} x \" \\\n",
                 "        f\"+ {np.round(m.intercept_.item(), 4)}\"\n",
                 "    return s\n",
-                "report_linear_fit(cycle.data.theories[0])"
+                "report_linear_fit(cycle.data.models[0])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "The best fit theory after all the cycles, including all the data, is:"
+                "The best fit model after all the cycles, including all the data, is:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.425078Z",
-                    "start_time": "2023-04-27T18:57:34.413258Z"
+                    "end_time": "2023-04-28T16:00:29.651704Z",
+                    "start_time": "2023-04-28T16:00:29.642827Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "'y = 0.9989 x + 1.0292'"
                     },
                     "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "report_linear_fit(cycle.data.theories[-1])"
+                "report_linear_fit(cycle.data.models[-1])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "This is close to the ground truth theory of x -> (x + 1)\n",
+                "This is close to the ground truth model of x -> (x + 1)\n",
                 "We can also run the cycle with more control over the execution flow:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.425203Z",
-                    "start_time": "2023-04-27T18:57:34.416286Z"
+                    "end_time": "2023-04-28T16:00:29.651855Z",
+                    "start_time": "2023-04-28T16:00:29.644832Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Generated 4 theories\n"
+                        "Generated 4 models\n"
                     ]
                 }
             ],
             "source": [
                 "_ = next(cycle)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.425333Z",
-                    "start_time": "2023-04-27T18:57:34.420974Z"
+                    "end_time": "2023-04-28T16:00:29.651938Z",
+                    "start_time": "2023-04-28T16:00:29.648413Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Generated 5 theories\n"
+                        "Generated 5 models\n"
                     ]
                 }
             ],
             "source": [
                 "_ = next(cycle)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 17,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.427955Z",
-                    "start_time": "2023-04-27T18:57:34.424978Z"
+                    "end_time": "2023-04-28T16:00:29.657114Z",
+                    "start_time": "2023-04-28T16:00:29.652804Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Generated 6 theories\n"
+                        "Generated 6 models\n"
                     ]
                 }
             ],
             "source": [
                 "_ = next(cycle)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
                 "We can continue to run the cycle as long as we like,\n",
-                "with a simple arbitrary stopping condition like the number of theories generated:"
+                "with a simple arbitrary stopping condition like the number of models generated:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 18,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.434476Z",
-                    "start_time": "2023-04-27T18:57:34.430631Z"
+                    "end_time": "2023-04-28T16:00:29.661188Z",
+                    "start_time": "2023-04-28T16:00:29.658078Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Generated 7 theories\n",
-                        "Generated 8 theories\n",
-                        "Generated 9 theories\n"
+                        "Generated 7 models\n",
+                        "Generated 8 models\n",
+                        "Generated 9 models\n"
                     ]
                 }
             ],
             "source": [
-                "_ = list(takewhile(lambda c: len(c.data.theories) < 9, cycle))"
+                "_ = list(takewhile(lambda c: len(c.data.models) < 9, cycle))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
@@ -559,34 +559,34 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 19,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.439525Z",
-                    "start_time": "2023-04-27T18:57:34.435076Z"
+                    "end_time": "2023-04-28T16:00:29.666266Z",
+                    "start_time": "2023-04-28T16:00:29.663336Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Generated 10 theories\n",
-                        "Generated 11 theories\n"
+                        "Generated 10 models\n",
+                        "Generated 11 models\n"
                     ]
                 }
             ],
             "source": [
                 "_ = list(\n",
                 "        takewhile(\n",
-                "            lambda c: np.abs(c.data.theories[-1].coef_.item() -\n",
-                "                           c.data.theories[-2].coef_.item()) > 1e-3,\n",
+                "            lambda c: np.abs(c.data.models[-1].coef_.item() -\n",
+                "                           c.data.models[-2].coef_.item()) > 1e-3,\n",
                 "            cycle\n",
                 "        )\n",
                 "    )\n"
             ]
         },
         {
             "cell_type": "markdown",
@@ -598,124 +598,124 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 20,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:34.492278Z",
-                    "start_time": "2023-04-27T18:57:34.439730Z"
+                    "end_time": "2023-04-28T16:00:29.711974Z",
+                    "start_time": "2023-04-28T16:00:29.667061Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Generated 12 theories\n",
-                        "Generated 13 theories\n",
-                        "Generated 14 theories\n",
-                        "Generated 15 theories\n",
-                        "Generated 16 theories\n",
-                        "Generated 17 theories\n",
-                        "Generated 18 theories\n",
-                        "Generated 19 theories\n",
-                        "Generated 20 theories\n",
-                        "Generated 21 theories\n",
-                        "Generated 22 theories\n",
-                        "Generated 23 theories\n",
-                        "Generated 24 theories\n",
-                        "Generated 25 theories\n",
-                        "Generated 26 theories\n",
-                        "Generated 27 theories\n",
-                        "Generated 28 theories\n",
-                        "Generated 29 theories\n",
-                        "Generated 30 theories\n",
-                        "Generated 31 theories\n",
-                        "Generated 32 theories\n",
-                        "Generated 33 theories\n",
-                        "Generated 34 theories\n",
-                        "Generated 35 theories\n",
-                        "Generated 36 theories\n",
-                        "Generated 37 theories\n",
-                        "Generated 38 theories\n",
-                        "Generated 39 theories\n",
-                        "Generated 40 theories\n",
-                        "Generated 41 theories\n",
-                        "Generated 42 theories\n",
-                        "Generated 43 theories\n",
-                        "Generated 44 theories\n",
-                        "Generated 45 theories\n",
-                        "Generated 46 theories\n",
-                        "Generated 47 theories\n",
-                        "Generated 48 theories\n",
-                        "Generated 49 theories\n",
-                        "Generated 50 theories\n",
-                        "Generated 51 theories\n",
-                        "Generated 52 theories\n",
-                        "Generated 53 theories\n",
-                        "Generated 54 theories\n",
-                        "Generated 55 theories\n",
-                        "Generated 56 theories\n",
-                        "Generated 57 theories\n",
-                        "Generated 58 theories\n",
-                        "Generated 59 theories\n",
-                        "Generated 60 theories\n",
-                        "Generated 61 theories\n",
-                        "Generated 62 theories\n",
-                        "Generated 63 theories\n",
-                        "Generated 64 theories\n",
-                        "Generated 65 theories\n",
-                        "Generated 66 theories\n",
-                        "Generated 67 theories\n",
-                        "Generated 68 theories\n",
-                        "Generated 69 theories\n",
-                        "Generated 70 theories\n",
-                        "Generated 71 theories\n",
-                        "Generated 72 theories\n",
-                        "Generated 73 theories\n",
-                        "Generated 74 theories\n",
-                        "Generated 75 theories\n",
-                        "Generated 76 theories\n",
-                        "Generated 77 theories\n",
-                        "Generated 78 theories\n",
-                        "Generated 79 theories\n",
-                        "Generated 80 theories\n",
-                        "Generated 81 theories\n",
-                        "Generated 82 theories\n",
-                        "Generated 83 theories\n",
-                        "Generated 84 theories\n",
-                        "Generated 85 theories\n",
-                        "Generated 86 theories\n",
-                        "Generated 87 theories\n",
-                        "Generated 88 theories\n",
-                        "Generated 89 theories\n",
-                        "Generated 90 theories\n",
-                        "Generated 91 theories\n",
-                        "Generated 92 theories\n",
-                        "Generated 93 theories\n",
-                        "Generated 94 theories\n",
-                        "Generated 95 theories\n",
-                        "Generated 96 theories\n",
-                        "Generated 97 theories\n",
-                        "Generated 98 theories\n",
-                        "Generated 99 theories\n",
-                        "Generated 100 theories\n",
-                        "Generated 101 theories\n",
-                        "Generated 102 theories\n",
-                        "Generated 103 theories\n",
-                        "Generated 104 theories\n",
-                        "Generated 105 theories\n",
-                        "Generated 106 theories\n",
-                        "Generated 107 theories\n",
-                        "Generated 108 theories\n",
-                        "Generated 109 theories\n",
-                        "Generated 110 theories\n",
-                        "Generated 111 theories\n"
+                        "Generated 12 models\n",
+                        "Generated 13 models\n",
+                        "Generated 14 models\n",
+                        "Generated 15 models\n",
+                        "Generated 16 models\n",
+                        "Generated 17 models\n",
+                        "Generated 18 models\n",
+                        "Generated 19 models\n",
+                        "Generated 20 models\n",
+                        "Generated 21 models\n",
+                        "Generated 22 models\n",
+                        "Generated 23 models\n",
+                        "Generated 24 models\n",
+                        "Generated 25 models\n",
+                        "Generated 26 models\n",
+                        "Generated 27 models\n",
+                        "Generated 28 models\n",
+                        "Generated 29 models\n",
+                        "Generated 30 models\n",
+                        "Generated 31 models\n",
+                        "Generated 32 models\n",
+                        "Generated 33 models\n",
+                        "Generated 34 models\n",
+                        "Generated 35 models\n",
+                        "Generated 36 models\n",
+                        "Generated 37 models\n",
+                        "Generated 38 models\n",
+                        "Generated 39 models\n",
+                        "Generated 40 models\n",
+                        "Generated 41 models\n",
+                        "Generated 42 models\n",
+                        "Generated 43 models\n",
+                        "Generated 44 models\n",
+                        "Generated 45 models\n",
+                        "Generated 46 models\n",
+                        "Generated 47 models\n",
+                        "Generated 48 models\n",
+                        "Generated 49 models\n",
+                        "Generated 50 models\n",
+                        "Generated 51 models\n",
+                        "Generated 52 models\n",
+                        "Generated 53 models\n",
+                        "Generated 54 models\n",
+                        "Generated 55 models\n",
+                        "Generated 56 models\n",
+                        "Generated 57 models\n",
+                        "Generated 58 models\n",
+                        "Generated 59 models\n",
+                        "Generated 60 models\n",
+                        "Generated 61 models\n",
+                        "Generated 62 models\n",
+                        "Generated 63 models\n",
+                        "Generated 64 models\n",
+                        "Generated 65 models\n",
+                        "Generated 66 models\n",
+                        "Generated 67 models\n",
+                        "Generated 68 models\n",
+                        "Generated 69 models\n",
+                        "Generated 70 models\n",
+                        "Generated 71 models\n",
+                        "Generated 72 models\n",
+                        "Generated 73 models\n",
+                        "Generated 74 models\n",
+                        "Generated 75 models\n",
+                        "Generated 76 models\n",
+                        "Generated 77 models\n",
+                        "Generated 78 models\n",
+                        "Generated 79 models\n",
+                        "Generated 80 models\n",
+                        "Generated 81 models\n",
+                        "Generated 82 models\n",
+                        "Generated 83 models\n",
+                        "Generated 84 models\n",
+                        "Generated 85 models\n",
+                        "Generated 86 models\n",
+                        "Generated 87 models\n",
+                        "Generated 88 models\n",
+                        "Generated 89 models\n",
+                        "Generated 90 models\n",
+                        "Generated 91 models\n",
+                        "Generated 92 models\n",
+                        "Generated 93 models\n",
+                        "Generated 94 models\n",
+                        "Generated 95 models\n",
+                        "Generated 96 models\n",
+                        "Generated 97 models\n",
+                        "Generated 98 models\n",
+                        "Generated 99 models\n",
+                        "Generated 100 models\n",
+                        "Generated 101 models\n",
+                        "Generated 102 models\n",
+                        "Generated 103 models\n",
+                        "Generated 104 models\n",
+                        "Generated 105 models\n",
+                        "Generated 106 models\n",
+                        "Generated 107 models\n",
+                        "Generated 108 models\n",
+                        "Generated 109 models\n",
+                        "Generated 110 models\n",
+                        "Generated 111 models\n"
                     ]
                 }
             ],
             "source": [
                 "_ = cycle.run(num_cycles=100)\n"
             ]
         }
```

### Comparing `autora-workflow-0.1.0/docs/cli/controller/basic-usage/controller.yml` & `autora-workflow-0.2.0/docs/cli/controller/basic-usage/controller.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/docs/cli/controller/custom-function/controller.yml` & `autora-workflow-0.2.0/docs/cli/controller/custom-function/controller.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc/controller.yml` & `autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/controller.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc/flow.cylc` & `autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/flow.cylc`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc/history/00000000-METADATA.yaml` & `autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/history/00000000-METADATA.yaml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc-slurm/controller.yml` & `autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/controller.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc-slurm/environment.yml` & `autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/environment.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc-slurm/flow.cylc` & `autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/flow.cylc`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/docs/cli/controller/custom-function-with-cylc-slurm/history/00000000-METADATA.yaml` & `autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/history/00000000-METADATA.yaml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/docs/passing-static-parameters.ipynb` & `autora-workflow-0.2.0/docs/passing-static-parameters.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990625%*

 * *Differences: {"'cells'": "{1: {'metadata': {'ExecuteTime': {'start_time': '2023-04-28T16:01:26.923273Z', "*

 * *            "'end_time': '2023-04-28T16:01:27.729662Z'}}}, 3: {'metadata': {'ExecuteTime': "*

 * *            "{'start_time': '2023-04-28T16:01:27.731342Z', 'end_time': "*

 * *            "'2023-04-28T16:01:27.732723Z'}}}, 4: {'metadata': {'ExecuteTime': {'start_time': "*

 * *            "'2023-04-28T16:01:27.733127Z', 'end_time': '2023-04-28T16:01:27.739134Z'}}}, 5: "*

 * *            "{'metadata': {'ExecuteTime': {'start_time': '202 […]*

```diff
@@ -12,16 +12,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:35.494832Z",
-                    "start_time": "2023-04-27T18:57:34.545690Z"
+                    "end_time": "2023-04-28T16:01:27.729662Z",
+                    "start_time": "2023-04-28T16:01:26.923273Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import pandas as pd\n",
@@ -42,16 +42,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:35.501759Z",
-                    "start_time": "2023-04-27T18:57:35.498994Z"
+                    "end_time": "2023-04-28T16:01:27.732723Z",
+                    "start_time": "2023-04-28T16:01:27.731342Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "uniform_random_rng = np.random.default_rng(180)\n",
                 "def uniform_random_sampler(n):\n",
@@ -62,16 +62,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:35.626745Z",
-                    "start_time": "2023-04-27T18:57:35.502567Z"
+                    "end_time": "2023-04-28T16:01:27.739134Z",
+                    "start_time": "2023-04-28T16:01:27.733127Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>x</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>0</th>\n      <td>6.33662</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
@@ -87,16 +87,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:35.627699Z",
-                    "start_time": "2023-04-27T18:57:35.622169Z"
+                    "end_time": "2023-04-28T16:01:27.742899Z",
+                    "start_time": "2023-04-28T16:01:27.741715Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "def ground_truth(x):\n",
                 "    return x + 1\n",
@@ -130,16 +130,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:35.662516Z",
-                    "start_time": "2023-04-27T18:57:35.630208Z"
+                    "end_time": "2023-04-28T16:01:27.764446Z",
+                    "start_time": "2023-04-28T16:01:27.743869Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>x</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>0</th>\n      <td>7.349166</td>\n    </tr>\n    <tr>\n      <th>1</th>\n      <td>6.085965</td>\n    </tr>\n    <tr>\n      <th>2</th>\n      <td>2.285666</td>\n    </tr>\n    <tr>\n      <th>3</th>\n      <td>1.955397</td>\n    </tr>\n    <tr>\n      <th>4</th>\n      <td>5.800231</td>\n    </tr>\n    <tr>\n      <th>5</th>\n      <td>3.270079</td>\n    </tr>\n    <tr>\n      <th>6</th>\n      <td>10.583823</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
@@ -172,16 +172,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:57:35.662983Z",
-                    "start_time": "2023-04-27T18:57:35.636711Z"
+                    "end_time": "2023-04-28T16:01:27.772307Z",
+                    "start_time": "2023-04-28T16:01:27.755746Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>x</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>0</th>\n      <td>9.456660</td>\n    </tr>\n    <tr>\n      <th>1</th>\n      <td>2.217216</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
```

### Comparing `autora-workflow-0.1.0/docs/using-alternative-planners-and-executors.ipynb` & `autora-workflow-0.2.0/docs/using-alternative-planners-and-executors.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9938069599051742%*

 * *Differences: {"'cells'": "{1: {'metadata': {'ExecuteTime': {'start_time': '2023-04-28T16:01:56.933043Z', "*

 * *            "'end_time': '2023-04-28T16:01:57.631186Z'}}}, 2: {'metadata': {'ExecuteTime': "*

 * *            "{'start_time': '2023-04-28T16:01:57.633245Z', 'end_time': "*

 * *            "'2023-04-28T16:01:57.635379Z'}}}, 4: {'outputs': {0: {'text': {insert: [(2, 'MONITOR: "*

 * *            "Generated new ResultKind.MODEL\\n'), (5, 'MONITOR: Generated new "*

 * *            "ResultKind.MODEL\\n')], delete: [5, 2]}}}, 'source': ['_ = […]*

```diff
@@ -19,16 +19,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.672733Z",
-                    "start_time": "2023-04-27T18:59:03.873023Z"
+                    "end_time": "2023-04-28T16:01:57.631186Z",
+                    "start_time": "2023-04-28T16:01:56.933043Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from autora.experimentalist.pipeline import make_pipeline\n",
@@ -39,16 +39,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.677510Z",
-                    "start_time": "2023-04-27T18:59:04.676248Z"
+                    "end_time": "2023-04-28T16:01:57.635379Z",
+                    "start_time": "2023-04-28T16:01:57.633245Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "def ground_truth(x):\n",
                 "    return x + 1\n",
@@ -91,35 +91,35 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.684224Z",
-                    "start_time": "2023-04-27T18:59:04.679741Z"
+                    "end_time": "2023-04-28T16:01:57.641066Z",
+                    "start_time": "2023-04-28T16:01:57.636930Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "MONITOR: Generated new ResultKind.CONDITION\n",
                         "MONITOR: Generated new ResultKind.OBSERVATION\n",
-                        "MONITOR: Generated new ResultKind.THEORY\n",
+                        "MONITOR: Generated new ResultKind.MODEL\n",
                         "MONITOR: Generated new ResultKind.CONDITION\n",
                         "MONITOR: Generated new ResultKind.OBSERVATION\n",
-                        "MONITOR: Generated new ResultKind.THEORY\n"
+                        "MONITOR: Generated new ResultKind.MODEL\n"
                     ]
                 }
             ],
             "source": [
-                "_ = list(takewhile(lambda c: len(c.state.theories) < 2, cycle_with_last_result_planner))"
+                "_ = list(takewhile(lambda c: len(c.state.models) < 2, cycle_with_last_result_planner))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
@@ -128,16 +128,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.686641Z",
-                    "start_time": "2023-04-27T18:59:04.685231Z"
+                    "end_time": "2023-04-28T16:01:57.643810Z",
+                    "start_time": "2023-04-28T16:01:57.642246Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "controller_with_seed_observation = Controller(\n",
                 "    monitor=monitor,\n",
@@ -151,25 +151,25 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.692002Z",
-                    "start_time": "2023-04-27T18:59:04.690949Z"
+                    "end_time": "2023-04-28T16:01:57.648672Z",
+                    "start_time": "2023-04-28T16:01:57.646294Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "MONITOR: Generated new ResultKind.THEORY\n"
+                        "MONITOR: Generated new ResultKind.MODEL\n"
                     ]
                 }
             ],
             "source": [
                 "_ = next(controller_with_seed_observation)"
             ]
         },
@@ -195,16 +195,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.725650Z",
-                    "start_time": "2023-04-27T18:59:04.692415Z"
+                    "end_time": "2023-04-28T16:01:57.650942Z",
+                    "start_time": "2023-04-28T16:01:57.648821Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "from autora.workflow.planner import random_operation_planner\n",
                 "def monitor(state):\n",
@@ -229,16 +229,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.734183Z",
-                    "start_time": "2023-04-27T18:59:04.695749Z"
+                    "end_time": "2023-04-28T16:01:57.682695Z",
+                    "start_time": "2023-04-28T16:01:57.651180Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "from random import seed\n",
                 "seed(42)"
@@ -254,16 +254,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.734306Z",
-                    "start_time": "2023-04-27T18:59:04.697356Z"
+                    "end_time": "2023-04-28T16:01:57.690905Z",
+                    "start_time": "2023-04-28T16:01:57.653429Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "import logging\n",
                 "import sys\n",
@@ -281,16 +281,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.734399Z",
-                    "start_time": "2023-04-27T18:59:04.700573Z"
+                    "end_time": "2023-04-28T16:01:57.691071Z",
+                    "start_time": "2023-04-28T16:01:57.655486Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "def step(controller_):\n",
                 "    try:\n",
@@ -310,16 +310,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.734564Z",
-                    "start_time": "2023-04-27T18:59:04.703002Z"
+                    "end_time": "2023-04-28T16:01:57.691280Z",
+                    "start_time": "2023-04-28T16:01:57.659011Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -342,16 +342,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.734675Z",
-                    "start_time": "2023-04-27T18:59:04.705556Z"
+                    "end_time": "2023-04-28T16:01:57.691357Z",
+                    "start_time": "2023-04-28T16:01:57.661419Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -374,16 +374,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.734752Z",
-                    "start_time": "2023-04-27T18:59:04.708019Z"
+                    "end_time": "2023-04-28T16:01:57.691425Z",
+                    "start_time": "2023-04-28T16:01:57.663622Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -406,16 +406,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.734837Z",
-                    "start_time": "2023-04-27T18:59:04.710179Z"
+                    "end_time": "2023-04-28T16:01:57.691501Z",
+                    "start_time": "2023-04-28T16:01:57.667337Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -439,16 +439,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.734976Z",
-                    "start_time": "2023-04-27T18:59:04.715286Z"
+                    "end_time": "2023-04-28T16:01:57.691583Z",
+                    "start_time": "2023-04-28T16:01:57.669604Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -471,33 +471,33 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.735116Z",
-                    "start_time": "2023-04-27T18:59:04.716882Z"
+                    "end_time": "2023-04-28T16:01:57.691641Z",
+                    "start_time": "2023-04-28T16:01:57.671841Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "MONITOR: Generated new ResultKind.CONDITION\n",
                         "MONITOR: Generated new ResultKind.CONDITION\n",
                         "MONITOR: Generated new ResultKind.CONDITION\n",
-                        "MONITOR: Generated new ResultKind.THEORY\n"
+                        "MONITOR: Generated new ResultKind.MODEL\n"
                     ]
                 }
             ],
             "source": [
-                "_ = list(takewhile(lambda c: len(c.state.theories) < 1, controller_with_random_planner))"
+                "_ = list(takewhile(lambda c: len(c.state.models) < 1, controller_with_random_planner))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
@@ -505,39 +505,39 @@
                 "## Arbitrary Executors and Planners\n",
                 "\n",
                 "In some cases, we need to go beyond adding different orders of planning the three\n",
                 "`experimentalist`, `experiment_runner` and `theorist` and build more complex cycles with\n",
                 "different Executors for different states.\n",
                 "\n",
                 "For instance, there might be a situation where at the start, the main \"active\" experimentalist\n",
-                "can't be run as it needs one or more theories as input.\n",
-                "Once there are at least two theories, then the active experimentalist _can_ be run.\n",
+                "can't be run as it needs one or more models as input.\n",
+                "Once there are at least two models, then the active experimentalist _can_ be run.\n",
                 "One method to handle this is to run a \"seed\" experimentalist until the main experimentalist can\n",
                 "be used.\n",
                 "\n",
                 "In these cases, we need full control over (and have full responsibility for) the planners and\n",
                 "executors.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "The theory we'll try to discover is:"
+                "The model we'll try to discover is:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.735164Z",
-                    "start_time": "2023-04-27T18:59:04.722213Z"
+                    "end_time": "2023-04-28T16:01:57.691699Z",
+                    "start_time": "2023-04-28T16:01:57.675535Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "def ground_truth(x, m=3.5, c=1):\n",
                 "    return m * x + c\n",
@@ -561,42 +561,42 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 17,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.735340Z",
-                    "start_time": "2023-04-27T18:59:04.724514Z"
+                    "end_time": "2023-04-28T16:01:57.700515Z",
+                    "start_time": "2023-04-28T16:01:57.677699Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "from autora.workflow.planner import last_result_kind_planner\n",
                 "from autora.workflow.state import History"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 18,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.735920Z",
-                    "start_time": "2023-04-27T18:59:04.725923Z"
+                    "end_time": "2023-04-28T16:01:57.707520Z",
+                    "start_time": "2023-04-28T16:01:57.679940Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "def seeding_planner(state):\n",
                 "    # We're going to reuse the \"last_result_kind_planner\" planner, and modify its output.\n",
                 "    next_function = last_result_kind_planner(state)\n",
                 "    if next_function == \"experimentalist\":\n",
-                "        if len(state.theories) >= 2:\n",
+                "        if len(state.models) >= 2:\n",
                 "            return \"main_experimentalist\"\n",
                 "        else:\n",
                 "            return \"seed_experimentalist\"\n",
                 "    else:\n",
                 "        return next_function\n"
             ]
         },
@@ -610,16 +610,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 19,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.736176Z",
-                    "start_time": "2023-04-27T18:59:04.730860Z"
+                    "end_time": "2023-04-28T16:01:57.707878Z",
+                    "start_time": "2023-04-28T16:01:57.683044Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "'seed_experimentalist'"
@@ -635,72 +635,72 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "... and we also get the seed experimentalist if the last result was a theory and there are less than two theories:"
+                "... and we also get the seed experimentalist if the last result was a model and there are less than two models:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 20,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.736754Z",
-                    "start_time": "2023-04-27T18:59:04.734243Z"
+                    "end_time": "2023-04-28T16:01:57.708090Z",
+                    "start_time": "2023-04-28T16:01:57.685631Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "'seed_experimentalist'"
                     },
                     "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "seeding_planner(History(theories=['a single theory']))"
+                "seeding_planner(History(models=['a single model']))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "whereas if we have at least two theories to work on, we get the main experimentalist:"
+                "whereas if we have at least two models to work on, we get the main experimentalist:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 21,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.745888Z",
-                    "start_time": "2023-04-27T18:59:04.737219Z"
+                    "end_time": "2023-04-28T16:01:57.708246Z",
+                    "start_time": "2023-04-28T16:01:57.688533Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "'main_experimentalist'"
                     },
                     "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "seeding_planner(History(theories=['a theory', 'another theory']))"
+                "seeding_planner(History(models=['a model', 'another model']))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
@@ -709,16 +709,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 22,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.746073Z",
-                    "start_time": "2023-04-27T18:59:04.740082Z"
+                    "end_time": "2023-04-28T16:01:57.708731Z",
+                    "start_time": "2023-04-28T16:01:57.691768Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "'experiment_runner'"
@@ -742,16 +742,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 23,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.746167Z",
-                    "start_time": "2023-04-27T18:59:04.743120Z"
+                    "end_time": "2023-04-28T16:01:57.708804Z",
+                    "start_time": "2023-04-28T16:01:57.694315Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "'theorist'"
@@ -775,16 +775,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 24,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.863538Z",
-                    "start_time": "2023-04-27T18:59:04.745770Z"
+                    "end_time": "2023-04-28T16:01:57.708840Z",
+                    "start_time": "2023-04-28T16:01:57.696837Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "from autora.experimentalist.pipeline import make_pipeline, Pipeline\n",
                 "from autora.experimentalist.sampler.random_sampler import random_sampler\n",
@@ -801,16 +801,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 25,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-04-27T18:59:04.863802Z",
-                    "start_time": "2023-04-27T18:59:04.751620Z"
+                    "end_time": "2023-04-28T16:01:57.708934Z",
+                    "start_time": "2023-04-28T16:01:57.700468Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "array([ 6.71671672, -0.73073073, -5.05505506,  6.13613614,  0.03003003,\n        4.59459459,  2.79279279,  5.43543544, -1.65165165,  8.0980981 ])"
@@ -847,26 +847,26 @@
                 {
                     "ename": "TypeError",
                     "evalue": "model_disagreement_sampler() missing 1 required positional argument: 'models'",
                     "output_type": "error",
                     "traceback": [
                         "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
                         "\u001b[0;31mTypeError\u001b[0m                                 Traceback (most recent call last)",
-                        "Cell \u001b[0;32mIn[26], line 5\u001b[0m\n\u001b[1;32m      1\u001b[0m \u001b[38;5;28;01mfrom\u001b[39;00m \u001b[38;5;21;01mautora\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01mexperimentalist\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01msampler\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01mmodel_disagreement\u001b[39;00m \u001b[38;5;28;01mimport\u001b[39;00m model_disagreement_sampler\n\u001b[1;32m      2\u001b[0m experimentalist_which_needs_a_theory \u001b[38;5;241m=\u001b[39m Pipeline([\n\u001b[1;32m      3\u001b[0m     (\u001b[38;5;124m'\u001b[39m\u001b[38;5;124mpool\u001b[39m\u001b[38;5;124m'\u001b[39m, np\u001b[38;5;241m.\u001b[39mlinspace(\u001b[38;5;241m*\u001b[39mmetadata_2\u001b[38;5;241m.\u001b[39mindependent_variables[\u001b[38;5;241m0\u001b[39m]\u001b[38;5;241m.\u001b[39mvalue_range, \u001b[38;5;241m1_000\u001b[39m)),\n\u001b[1;32m      4\u001b[0m     (\u001b[38;5;124m'\u001b[39m\u001b[38;5;124msampler\u001b[39m\u001b[38;5;124m'\u001b[39m, partial(model_disagreement_sampler, num_samples\u001b[38;5;241m=\u001b[39m\u001b[38;5;241m5\u001b[39m)),])\n\u001b[0;32m----> 5\u001b[0m \u001b[43mexperimentalist_which_needs_a_theory\u001b[49m\u001b[43m(\u001b[49m\u001b[43m)\u001b[49m\n",
+                        "Cell \u001b[0;32mIn[26], line 5\u001b[0m\n\u001b[1;32m      1\u001b[0m \u001b[38;5;28;01mfrom\u001b[39;00m \u001b[38;5;21;01mautora\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01mexperimentalist\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01msampler\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01mmodel_disagreement\u001b[39;00m \u001b[38;5;28;01mimport\u001b[39;00m model_disagreement_sampler\n\u001b[1;32m      2\u001b[0m experimentalist_which_needs_a_model \u001b[38;5;241m=\u001b[39m Pipeline([\n\u001b[1;32m      3\u001b[0m     (\u001b[38;5;124m'\u001b[39m\u001b[38;5;124mpool\u001b[39m\u001b[38;5;124m'\u001b[39m, np\u001b[38;5;241m.\u001b[39mlinspace(\u001b[38;5;241m*\u001b[39mvariables_2\u001b[38;5;241m.\u001b[39mindependent_variables[\u001b[38;5;241m0\u001b[39m]\u001b[38;5;241m.\u001b[39mvalue_range, \u001b[38;5;241m1_000\u001b[39m)),\n\u001b[1;32m      4\u001b[0m     (\u001b[38;5;124m'\u001b[39m\u001b[38;5;124msampler\u001b[39m\u001b[38;5;124m'\u001b[39m, partial(model_disagreement_sampler, num_samples\u001b[38;5;241m=\u001b[39m\u001b[38;5;241m5\u001b[39m)),])\n\u001b[0;32m----> 5\u001b[0m \u001b[43mexperimentalist_which_needs_a_model\u001b[49m\u001b[43m(\u001b[49m\u001b[43m)\u001b[49m\n",
                         "File \u001b[0;32m~/Developer/autora-core/src/autora/experimentalist/pipeline.py:171\u001b[0m, in \u001b[0;36mPipeline.__call__\u001b[0;34m(self, ex, **params)\u001b[0m\n\u001b[1;32m    169\u001b[0m     \u001b[38;5;28;01massert\u001b[39;00m \u001b[38;5;28misinstance\u001b[39m(pipe, Pipe)\n\u001b[1;32m    170\u001b[0m     all_params_for_pipe \u001b[38;5;241m=\u001b[39m merged_params\u001b[38;5;241m.\u001b[39mget(name, \u001b[38;5;28mdict\u001b[39m())\n\u001b[0;32m--> 171\u001b[0m     results\u001b[38;5;241m.\u001b[39mappend(\u001b[43mpipe\u001b[49m\u001b[43m(\u001b[49m\u001b[43mresults\u001b[49m\u001b[43m[\u001b[49m\u001b[38;5;241;43m-\u001b[39;49m\u001b[38;5;241;43m1\u001b[39;49m\u001b[43m]\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[38;5;241;43m*\u001b[39;49m\u001b[38;5;241;43m*\u001b[39;49m\u001b[43mall_params_for_pipe\u001b[49m\u001b[43m)\u001b[49m)\n\u001b[1;32m    173\u001b[0m \u001b[38;5;28;01mreturn\u001b[39;00m results[\u001b[38;5;241m-\u001b[39m\u001b[38;5;241m1\u001b[39m]\n",
                         "\u001b[0;31mTypeError\u001b[0m: model_disagreement_sampler() missing 1 required positional argument: 'models'"
                     ]
                 }
             ],
             "source": [
                 "from autora.experimentalist.sampler.model_disagreement import model_disagreement_sampler\n",
-                "experimentalist_which_needs_a_theory = Pipeline([\n",
+                "experimentalist_which_needs_a_model = Pipeline([\n",
                 "    ('pool', np.linspace(*metadata_2.independent_variables[0].value_range, 1_000)),\n",
                 "    ('sampler', partial(model_disagreement_sampler, num_samples=5)),])\n",
-                "experimentalist_which_needs_a_theory()"
+                "experimentalist_which_needs_a_model()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
@@ -874,15 +874,15 @@
                 "We'll have to provide the models during the cycle run.\n",
                 "\n",
                 "We need a reasonable theorist for this situation. For this problem, a linear regressor will suffice."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-04-27T18:59:16.580114Z",
                     "start_time": "2023-04-27T18:59:16.569889Z"
                 },
                 "collapsed": false
             },
@@ -898,32 +898,23 @@
             },
             "source": [
                 "Let's test the theorist for the ideal case \u2013 lots of data:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-04-27T18:59:17.816552Z",
                     "start_time": "2023-04-27T18:59:17.807609Z"
                 },
                 "collapsed": false
             },
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": "'m = 3.50, c = 1.04'"
-                    },
-                    "execution_count": 28,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
                 "X = np.linspace(*metadata_2.independent_variables[0].value_range, 1_000).reshape(-1, 1)\n",
                 "tfitted = t.fit(X, experiment_runner(X))\n",
                 "f\"m = {tfitted.coef_[0][0]:.2f}, c = {tfitted.intercept_[0]:.2f}\""
             ]
         },
         {
@@ -935,28 +926,28 @@
                 "This seems to work fine.\n",
                 "\n",
                 "Now we can define the executor component. We'll use a factory method to generate the collection:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-04-27T18:59:18.179154Z",
                     "start_time": "2023-04-27T18:59:18.170109Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "from autora.workflow.executor import make_online_executor_collection\n",
                 "executor_collection = make_online_executor_collection([\n",
                 "    (\"seed_experimentalist\", \"experimentalist\", experimentalist_which_needs_no_data),\n",
-                "    (\"main_experimentalist\", \"experimentalist\", experimentalist_which_needs_a_theory),\n",
+                "    (\"main_experimentalist\", \"experimentalist\", experimentalist_which_needs_a_model),\n",
                 "    (\"theorist\", \"theorist\", LinearRegression()),\n",
                 "    (\"experiment_runner\", \"experiment_runner\", experiment_runner),\n",
                 "])\n"
             ]
         },
         {
             "cell_type": "markdown",
@@ -965,70 +956,61 @@
             },
             "source": [
                 "We need some special parameters to handle the main experimentalist, so we specify those:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-04-27T18:59:18.528215Z",
                     "start_time": "2023-04-27T18:59:18.518548Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
-                "params = {\"main_experimentalist\": {\"sampler\": {\"models\": \"%theories%\"}}}"
+                "params = {\"main_experimentalist\": {\"sampler\": {\"models\": \"%models%\"}}}"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
                 "We now instantiate the controller:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-04-27T18:59:18.930882Z",
                     "start_time": "2023-04-27T18:59:18.926964Z"
                 },
                 "collapsed": false
             },
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": "<autora.workflow.base.BaseController at 0x176e719d0>"
-                    },
-                    "execution_count": 31,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
                 "from autora.workflow.base import BaseController\n",
                 "from autora.workflow.state import History\n",
                 "c = BaseController(\n",
                 "        state=History(metadata=metadata_2, params=params),\n",
                 "        planner=seeding_planner,\n",
                 "        executor_collection=executor_collection\n",
                 ")\n",
                 "c"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-04-27T18:59:19.257785Z",
                     "start_time": "2023-04-27T18:59:19.249578Z"
                 },
                 "collapsed": false
             },
@@ -1047,32 +1029,23 @@
             "source": [
                 "On the first step, we generate a condition sampled randomly across the whole domain (as we\n",
                 "expected):"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 33,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-04-27T18:59:19.747720Z",
                     "start_time": "2023-04-27T18:59:19.737183Z"
                 },
                 "collapsed": false
             },
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": "Result(data=array([ 9.4994995 , -8.17817818, -1.19119119,  8.6986987 ,  7.45745746,\n       -6.93693694,  8.05805806, -1.45145145, -5.97597598,  1.57157157]), kind=ResultKind.CONDITION)"
-                    },
-                    "execution_count": 33,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
                 "next(c).state.history[-1]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -1081,109 +1054,74 @@
             "source": [
                 "After three more steps, we generate a new condition, which again is sampled across the whole domain. Here we iterate\n",
                 "the controller until we've got two sets of conditions:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-04-27T18:59:20.145376Z",
                     "start_time": "2023-04-27T18:59:20.137931Z"
                 },
                 "collapsed": false
             },
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": "Result(data=array([ 1.57157157, -3.93393393, -0.47047047, -4.47447447,  8.43843844,\n        6.17617618, -3.49349349, -8.998999  ,  4.93493493,  2.25225225]), kind=ResultKind.CONDITION)"
-                    },
-                    "execution_count": 34,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
                 "_ = list(takewhile(lambda c: len(c.state.conditions) < 2, c))\n",
                 "c.state.history[-1]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "Once we have two theories:"
+                "Once we have two models:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 35,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-04-27T18:59:21.060733Z",
                     "start_time": "2023-04-27T18:59:21.040079Z"
                 },
                 "collapsed": false
             },
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": "[LinearRegression(), LinearRegression()]"
-                    },
-                    "execution_count": 35,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "_ = list(takewhile(lambda c: len(c.state.theories) < 2, c))\n",
-                "c.state.theories"
+                "_ = list(takewhile(lambda c: len(c.state.models) < 2, c))\n",
+                "c.state.models"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
                 "... when we run the next step, we'll get the main experimentalist. This samples five points from the extreme\n",
-                "parts  of the problem domain where the disagreement between the two theories is the greatest:"
+                "parts  of the problem domain where the disagreement between the two models is the greatest:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 36,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2023-04-27T18:59:23.445789Z",
                     "start_time": "2023-04-27T18:59:23.419106Z"
                 },
                 "collapsed": false
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "WARNING: new_conditions=array([-10.        ,  -9.97997998,  -9.95995996,  -9.93993994,\n",
-                        "        -9.91991992]) is an ndarray, so variable confusion is a possibility\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "text/plain": "Result(data=array([-10.        ,  -9.97997998,  -9.95995996,  -9.93993994,\n        -9.91991992]), kind=ResultKind.CONDITION)"
-                    },
-                    "execution_count": 36,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
                 "next(c).state.history[-1]\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `autora-workflow-0.1.0/mkdocs/base.yml` & `autora-workflow-0.2.0/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/mkdocs/gen_ref_pages.py` & `autora-workflow-0.2.0/mkdocs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/pyproject.toml` & `autora-workflow-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -28,7 +28,10 @@
 documentation = "https://hollandjg.github.io/autora-workflow/"
 
 [build-system]
 requires = ["setuptools", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
+
+[tool.isort]
+profile = "black"
```

### Comparing `autora-workflow-0.1.0/src/autora/workflow/__init__.py` & `autora-workflow-0.2.0/src/autora/workflow/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 """
 
 Functions and classes for running the complete AER cycle.
 
 # Basic Usage
 
-Aim: Use the Controller to recover a simple ground truth theory from noisy data.
+Aim: Use the Controller to recover a simple ground truth model from noisy data.
 
 Examples:
 
     >>> def ground_truth(x):
     ...     return x + 1
 
     The space of allowed x values is the integers between 0 and 10 inclusive,
     and we record the allowed output values as well.
     >>> from autora.variable import VariableCollection, Variable
-    >>> metadata_0 = VariableCollection(
+    >>> variables_0 = VariableCollection(
     ...    independent_variables=[Variable(name="x1", allowed_values=range(11))],
     ...    dependent_variables=[Variable(name="y", value_range=(-20, 20))],
     ...    )
 
     The experimentalist is used to propose experiments.
     Since the space of values is so restricted, we can just sample them all each time.
     >>> from autora.experimentalist.pipeline import make_pipeline
     >>> example_experimentalist = make_pipeline(
-    ...     [metadata_0.independent_variables[0].allowed_values])
+    ...     [variables_0.independent_variables[0].allowed_values])
 
     When we run a synthetic experiment, we get a reproducible noisy result:
     >>> import numpy as np
     >>> def get_example_synthetic_experiment_runner():
     ...     rng = np.random.default_rng(seed=180)
     ...     def runner(x):
     ...         return ground_truth(x) + rng.normal(0, 0.1, x.shape)
     ...     return runner
     >>> example_synthetic_experiment_runner = get_example_synthetic_experiment_runner()
     >>> example_synthetic_experiment_runner(np.array([1]))
     array([2.04339546])
 
-    The theorist "tries" to work out the best theory.
+    The theorist "tries" to work out the best model.
     We use a trivial scikit-learn regressor.
     >>> from sklearn.linear_model import LinearRegression
     >>> example_theorist = LinearRegression()
 
-    We initialize the Controller with the metadata describing the domain of the theory,
+    We initialize the Controller with the variables describing the domain of the model,
     the theorist, experimentalist and experiment runner,
     as well as a monitor which will let us know which cycle we're currently on.
     >>> cycle = Cycle(
-    ...     metadata=metadata_0,
+    ...     variables=variables_0,
     ...     theorist=example_theorist,
     ...     experimentalist=example_experimentalist,
     ...     experiment_runner=example_synthetic_experiment_runner,
-    ...     monitor=lambda state: print(f"Generated {len(state.theories)} theories"),
+    ...     monitor=lambda state: print(f"Generated {len(state.models)} models"),
     ... )
     >>> cycle # doctest: +ELLIPSIS
     <...Cycle object at 0x...>
 
     We can run the cycle by calling the run method:
     >>> cycle.run(num_cycles=3)  # doctest: +ELLIPSIS
-    Generated 1 theories
-    Generated 2 theories
-    Generated 3 theories
+    Generated 1 models
+    Generated 2 models
+    Generated 3 models
     <...Cycle object at 0x...>
 
     We can now interrogate the results. The first set of conditions which went into the
     experiment runner were:
     >>> cycle.data.conditions[0]
     array([ 0,  1,  2,  3,  4,  5,  6,  7,  8,  9, 10])
 
@@ -81,69 +81,69 @@
            [10.        , 10.88517906]])
 
     In the third cycle (index = 2) the first and last values are different again:
     >>> cycle.data.observations[2][[0,-1]]
     array([[ 0.        ,  1.08559827],
            [10.        , 11.08179553]])
 
-    The best fit theory after the first cycle is:
-    >>> cycle.data.theories[0]
+    The best fit model after the first cycle is:
+    >>> cycle.data.models[0]
     LinearRegression()
 
     >>> def report_linear_fit(m: LinearRegression,  precision=4):
     ...     s = f"y = {np.round(m.coef_[0].item(), precision)} x " \\
     ...     f"+ {np.round(m.intercept_.item(), 4)}"
     ...     return s
-    >>> report_linear_fit(cycle.data.theories[0])
+    >>> report_linear_fit(cycle.data.models[0])
     'y = 1.0089 x + 0.9589'
 
-    The best fit theory after all the cycles, including all the data, is:
-    >>> report_linear_fit(cycle.data.theories[-1])
+    The best fit model after all the cycles, including all the data, is:
+    >>> report_linear_fit(cycle.data.models[-1])
     'y = 0.9989 x + 1.0292'
 
-    This is close to the ground truth theory of x -> (x + 1)
+    This is close to the ground truth model of x -> (x + 1)
 
     We can also run the cycle with more control over the execution flow:
     >>> next(cycle) # doctest: +ELLIPSIS
-    Generated 4 theories
+    Generated 4 models
     <...Cycle object at 0x...>
 
     >>> next(cycle) # doctest: +ELLIPSIS
-    Generated 5 theories
+    Generated 5 models
     <...Cycle object at 0x...>
 
     >>> next(cycle) # doctest: +ELLIPSIS
-    Generated 6 theories
+    Generated 6 models
     <...Cycle object at 0x...>
 
     We can continue to run the cycle as long as we like,
-    with a simple arbitrary stopping condition like the number of theories generated:
+    with a simple arbitrary stopping condition like the number of models generated:
     >>> from itertools import takewhile
-    >>> _ = list(takewhile(lambda c: len(c.data.theories) < 9, cycle))
-    Generated 7 theories
-    Generated 8 theories
-    Generated 9 theories
+    >>> _ = list(takewhile(lambda c: len(c.data.models) < 9, cycle))
+    Generated 7 models
+    Generated 8 models
+    Generated 9 models
 
     ... or the precision (here we keep iterating while the difference between the gradients
     of the second-last and last cycle is larger than 1x10^-3).
     >>> _ = list(
     ...         takewhile(
-    ...             lambda c: np.abs(c.data.theories[-1].coef_.item() -
-    ...                            c.data.theories[-2].coef_.item()) > 1e-3,
+    ...             lambda c: np.abs(c.data.models[-1].coef_.item() -
+    ...                            c.data.models[-2].coef_.item()) > 1e-3,
     ...             cycle
     ...         )
     ...     )
-    Generated 10 theories
-    Generated 11 theories
+    Generated 10 models
+    Generated 11 models
 
     ... or continue to run as long as we like:
     >>> _ = cycle.run(num_cycles=100) # doctest: +ELLIPSIS
-    Generated 12 theories
+    Generated 12 models
     ...
-    Generated 111 theories
+    Generated 111 models
 
 # Passing Static Parameters
 
 Aim: pass parameters to the cycle components, when they are needed.
 
 Examples:
 
@@ -151,15 +151,15 @@
     >>> uniform_random_rng = np.random.default_rng(180)
     >>> def uniform_random_sampler(n):
     ...     return uniform_random_rng.uniform(low=0, high=11, size=n)
     >>> example_experimentalist_with_parameters = make_pipeline([uniform_random_sampler])
 
     The cycle can handle that using the `params` keyword:
     >>> cycle_with_parameters = Cycle(
-    ...     metadata=metadata_0,
+    ...     variables=variables_0,
     ...     theorist=example_theorist,
     ...     experimentalist=example_experimentalist_with_parameters,
     ...     experiment_runner=example_synthetic_experiment_runner,
     ...     params={"experimentalist": {"uniform_random_sampler": {"n": 7}}}
     ... )
     >>> _ = cycle_with_parameters.run()
     >>> cycle_with_parameters.data.conditions[-1].flatten()
@@ -173,55 +173,55 @@
     >>> cycle_with_parameters.data.conditions[-1].flatten()
     array([10.5838232 ,  9.45666031])
 
 # Accessing "State-dependent Properties"
 
 Some experimentalists, experiment runners and theorists require access to the values
 created during the cycle execution, e.g. experimentalists which require access
-to the current best theory or the observed data. These data update each cycle, and
+to the current best model or the observed data. These data update each cycle, and
 so cannot easily be set using simple `params`.
 
 For this case, it is possible to use "state-dependent properties" in the `params`
 dictionary. These are the following strings, which will be replaced during execution by
 their respective current values:
 
 - `"%observations.ivs[-1]%"`: the last observed independent variables
 - `"%observations.dvs[-1]%"`: the last observed dependent variables
 - `"%observations.ivs%"`: all the observed independent variables,
 concatenated into a single array
 - `"%observations.dvs%"`: all the observed dependent variables,
 concatenated into a single array
-- `"%theories[-1]%"`: the last fitted theorist
-- `"%theories%"`: all the fitted theorists
+- `"%models[-1]%"`: the last fitted theorist
+- `"%models%"`: all the fitted theorists
 
 Examples:
 
     In the following example, we use the `"observations.ivs"` cycle property for an
     experimentalist which excludes those conditions which have
     already been seen.
 
-    >>> metadata_1 = VariableCollection(
+    >>> variables_1 = VariableCollection(
     ...    independent_variables=[Variable(name="x1", allowed_values=range(10))],
     ...    dependent_variables=[Variable(name="y")],
     ...    )
     >>> random_sampler_rng = np.random.default_rng(seed=180)
     >>> def custom_random_sampler(conditions, n):
     ...     sampled_conditions = random_sampler_rng.choice(conditions, size=n, replace=False)
     ...     return sampled_conditions
     >>> def exclude_conditions(conditions, excluded_conditions):
     ...     remaining_conditions = list(set(conditions) - set(excluded_conditions.flatten()))
     ...     return remaining_conditions
     >>> unobserved_data_experimentalist = make_pipeline([
-    ...     metadata_1.independent_variables[0].allowed_values,
+    ...     variables_1.independent_variables[0].allowed_values,
     ...     exclude_conditions,
     ...     custom_random_sampler
     ...     ]
     ... )
     >>> cycle_with_state_dep_properties = Cycle(
-    ...     metadata=metadata_1,
+    ...     variables=variables_1,
     ...     theorist=example_theorist,
     ...     experimentalist=unobserved_data_experimentalist,
     ...     experiment_runner=example_synthetic_experiment_runner,
     ...     params={
     ...         "experimentalist": {
     ...             "exclude_conditions": {"excluded_conditions": "%observations.ivs%"},
     ...             "custom_random_sampler": {"n": 1}
@@ -283,43 +283,43 @@
     order. It considers the last available result and picks the matching next step. This means
     that seeding is relatively simple.
     >>> from autora.workflow import Controller
     >>> def monitor(state):
     ...     print(f"MONITOR: Generated new {state.history[-1].kind.value}")
     >>> cycle_with_last_result_planner = Controller(
     ...     monitor=monitor,
-    ...     metadata=metadata_0,
+    ...     variables=variables_0,
     ...     theorist=example_theorist,
     ...     experimentalist=example_experimentalist,
     ...     experiment_runner=example_synthetic_experiment_runner,
     ... )
 
     When we run this cycle starting with no data, we generate an experimental condition first:
-    >>> _ = list(takewhile(lambda c: len(c.state.theories) < 2, cycle_with_last_result_planner))
+    >>> _ = list(takewhile(lambda c: len(c.state.models) < 2, cycle_with_last_result_planner))
     MONITOR: Generated new CONDITION
     MONITOR: Generated new OBSERVATION
-    MONITOR: Generated new THEORY
+    MONITOR: Generated new MODEL
     MONITOR: Generated new CONDITION
     MONITOR: Generated new OBSERVATION
-    MONITOR: Generated new THEORY
+    MONITOR: Generated new MODEL
 
     However, if we seed the same cycle with observations, then its first Executor will be the
     theorist:
     >>> controller_with_seed_observation = Controller(
     ...     monitor=monitor,
-    ...     metadata=metadata_0,
+    ...     variables=variables_0,
     ...     theorist=example_theorist,
     ...     experimentalist=example_experimentalist,
     ...     experiment_runner=example_synthetic_experiment_runner,
     ... )
     >>> seed_observation = example_synthetic_experiment_runner(np.linspace(0,5,10))
     >>> controller_with_seed_observation.seed(observations=[seed_observation])
 
     >>> _ = next(controller_with_seed_observation)
-    MONITOR: Generated new THEORY
+    MONITOR: Generated new MODEL
 
 ## Arbitrary Execution Order (Toy Example)
 
 In some cases, we need to change the order of execution of different steps completely. This might be
  useful in cases when different experimentalists or theorists are needed at different times in
  the cycle, e.g. for initial seeding, or if the _order_ of execution is the subject of the
  experiment.
@@ -334,15 +334,15 @@
     different times in the cycle, e.g. for initial seeding.
     >>> from autora.workflow.planner import random_operation_planner
     >>> def monitor(state):
     ...     print(f"MONITOR: Generated new {state.history[-1].kind.value}")
     >>> controller_with_random_planner = Controller(
     ...     planner=random_operation_planner,
     ...     monitor=monitor,
-    ...     metadata=metadata_0,
+    ...     variables=variables_0,
     ...     theorist=example_theorist,
     ...     experimentalist=example_experimentalist,
     ...     experiment_runner=example_synthetic_experiment_runner,
     ... )
 
     The `random_operation_planner` depends on the python random number generator, so we seed
     it first:
@@ -381,75 +381,75 @@
 
     On the fifth step, we generate a first real observation, so that the next time we try to run
     a theorist we are successful:
     >>> step(controller_with_random_planner) # i = 4
     MONITOR: Generated new OBSERVATION
 
     By the ninth iteration, there are observations which the theorist can use, and it succeeds.
-    >>> _ = list(takewhile(lambda c: len(c.state.theories) < 1, controller_with_random_planner))
+    >>> _ = list(takewhile(lambda c: len(c.state.models) < 1, controller_with_random_planner))
     MONITOR: Generated new CONDITION
     MONITOR: Generated new CONDITION
     MONITOR: Generated new CONDITION
-    MONITOR: Generated new THEORY
+    MONITOR: Generated new MODEL
 
 ## Arbitrary Executors and Planners
 
 In some cases, we need to go beyond adding different orders of planning the three
 `experimentalist`, `experiment_runner` and `theorist` and build more complex cycles with
 different Executors for different states.
 
 For instance, there might be a situation where at the start, the main "active" experimentalist
-can't be run as it needs one or more theories as input.
-Once there are at least two theories, then the active experimentalist _can_ be run.
+can't be run as it needs one or more models as input.
+Once there are at least two models, then the active experimentalist _can_ be run.
 One method to handle this is to run a "seed" experimentalist until the main experimentalist can
 be used.
 
 In these cases, we need full control over (and have full responsibility for) the planners and
 executors.
 
 Examples:
-    The theory we'll try to discover is:
+    The model we'll try to discover is:
     >>> def ground_truth(x, m=3.5, c=1):
     ...     return m * x + c
     >>> rng = np.random.default_rng(seed=180)
     >>> def experiment_runner(x):
     ...     return ground_truth(x) + rng.normal(0, 0.1)
-    >>> metadata_2 = VariableCollection(
+    >>> variables_2 = VariableCollection(
     ...    independent_variables=[Variable(name="x1", value_range=(-10, 10))],
     ...    dependent_variables=[Variable(name="y", value_range=(-100, 100))],
     ...    )
 
     We now define a planner which chooses a different experimentalist when supplied with no data
     versus some data.
     >>> from autora.workflow.protocol import ResultKind
     >>> from autora.workflow.planner import last_result_kind_planner
     >>> def seeding_planner(state):
     ...     # We're going to reuse the "last_available_result" planner, and modify its output.
     ...     next_function = last_result_kind_planner(state)
     ...     if next_function == "experimentalist":
-    ...         if len(state.theories) >= 2:
+    ...         if len(state.models) >= 2:
     ...             return "main_experimentalist"
     ...         else:
     ...             return "seed_experimentalist"
     ...     else:
     ...         return next_function
 
     Now we can see what would happen with a particular state. If there are no results,
     then we get the seed experimentalist:
     >>> from autora.workflow.state import History
     >>> seeding_planner(History())
     'seed_experimentalist'
 
-    ... and we also get the seed experimentalist if the last result was a theory and there are less
-    than two theories:
-    >>> seeding_planner(History(theories=['a single theory']))
+    ... and we also get the seed experimentalist if the last result was a model and there are less
+    than two models:
+    >>> seeding_planner(History(models=['a single model']))
     'seed_experimentalist'
 
-    ... whereas if we have at least two theories to work on, we get the main experimentalist:
-    >>> seeding_planner(History(theories=['a theory', 'another theory']))
+    ... whereas if we have at least two models to work on, we get the main experimentalist:
+    >>> seeding_planner(History(models=['a model', 'another model']))
     'main_experimentalist'
 
     If we had a condition last, we choose the experiment runner next:
     >>> seeding_planner(History(conditions=['a condition']))
     'experiment_runner'
 
     If we had an observation last, we choose the theorist next:
@@ -459,64 +459,64 @@
     Now we need to define an executor collection to handle the actual execution steps.
     >>> from autora.experimentalist.pipeline import make_pipeline, Pipeline
     >>> from autora.experimentalist.sampler.random_sampler import random_sampler
     >>> from functools import partial
 
     Wen can run the seed pipeline with no data:
     >>> experimentalist_which_needs_no_data = make_pipeline([
-    ...     np.linspace(*metadata_2.independent_variables[0].value_range, 1_000),
+    ...     np.linspace(*variables_2.independent_variables[0].value_range, 1_000),
     ...     partial(random_sampler, n=10)]
     ... )
     >>> np.array(experimentalist_which_needs_no_data())
     array([ 6.71671672, -0.73073073, -5.05505506,  6.13613614,  0.03003003,
             4.59459459,  2.79279279,  5.43543544, -1.65165165,  8.0980981 ])
 
 
     ... whereas we need some model for this sampler:
     >>> from autora.experimentalist.sampler.model_disagreement import model_disagreement_sampler
-    >>> experimentalist_which_needs_a_theory = Pipeline([
-    ...     ('pool', np.linspace(*metadata_2.independent_variables[0].value_range, 1_000)),
+    >>> experimentalist_which_needs_a_model = Pipeline([
+    ...     ('pool', np.linspace(*variables_2.independent_variables[0].value_range, 1_000)),
     ...     ('sampler', partial(model_disagreement_sampler, num_samples=5)),])
-    >>> experimentalist_which_needs_a_theory()
+    >>> experimentalist_which_needs_a_model()
     Traceback (most recent call last):
     ...
     TypeError: model_disagreement_sampler() missing 1 required positional argument: 'models'
 
     We'll have to provide the models during the cycle run.
 
     We need a reasonable theorist for this situation. For this problem, a linear regressor will
     suffice.
     >>> t = LinearRegression()
 
     Let's test the theorist for the ideal case – lots of data:
-    >>> X = np.linspace(*metadata_2.independent_variables[0].value_range, 1_000).reshape(-1, 1)
+    >>> X = np.linspace(*variables_2.independent_variables[0].value_range, 1_000).reshape(-1, 1)
     >>> tfitted = t.fit(X, experiment_runner(X))
     >>> f"m = {tfitted.coef_[0][0]:.2f}, c = {tfitted.intercept_[0]:.2f}"
     'm = 3.50, c = 1.04'
 
     This seems to work fine.
 
     Now we can define the executor component. We'll use a factory method to generate the
     collection:
     >>> from autora.workflow.executor import make_online_executor_collection
     >>> executor_collection = make_online_executor_collection([
     ...     ("seed_experimentalist", "experimentalist", experimentalist_which_needs_no_data),
-    ...     ("main_experimentalist", "experimentalist", experimentalist_which_needs_a_theory),
+    ...     ("main_experimentalist", "experimentalist", experimentalist_which_needs_a_model),
     ...     ("theorist", "theorist", LinearRegression()),
     ...     ("experiment_runner", "experiment_runner", experiment_runner),
     ... ])
 
     We need some special parameters to handle the main experimentalist, so we specify those:
-    >>> params = {"main_experimentalist": {"sampler": {"models": "%theories%"}}}
+    >>> params = {"main_experimentalist": {"sampler": {"models": "%models%"}}}
 
     We now instantiate the controller:
     >>> from autora.workflow.base import BaseController
     >>> from autora.workflow.state import History
     >>> c = BaseController(
-    ...         state=History(metadata=metadata_2, params=params),
+    ...         state=History(variables=variables_2, params=params),
     ...         planner=seeding_planner,
     ...         executor_collection=executor_collection
     ... )
     >>> c  # doctest: +ELLIPSIS
     <...BaseController object at 0x...>
 
     >>> class PrintHandler(logging.Handler):
@@ -534,21 +534,21 @@
     domain. Here we iterate the controller until we've got two sets of conditions:
     >>> _ = list(takewhile(lambda c: len(c.state.conditions) < 2, c))
     >>> c.state.history[-1]  # doctest: +NORMALIZE_WHITESPACE
     Result(data=array([ 1.57157157, -3.93393393, -0.47047047, -4.47447447,  8.43843844,
                         6.17617618, -3.49349349, -8.998999  ,  4.93493493,  2.25225225]),
            kind=ResultKind.CONDITION)
 
-    Once we have two theories:
-    >>> _ = list(takewhile(lambda c: len(c.state.theories) < 2, c))
-    >>> c.state.theories
+    Once we have two models:
+    >>> _ = list(takewhile(lambda c: len(c.state.models) < 2, c))
+    >>> c.state.models
     [LinearRegression(), LinearRegression()]
 
     ... when we run the next step, we'll get the main experimentalist, which samples five points
-    from the extreme parts of the problem domain where the disagreement between the two theories
+    from the extreme parts of the problem domain where the disagreement between the two models
     is the greatest:
     >>> next(c).state.history[-1]  # doctest: +NORMALIZE_WHITESPACE
     Result(data=array([-10.       ,  -9.97997998,  -9.95995996,  -9.93993994,  -9.91991992]),
            kind=ResultKind.CONDITION)
 
 """
 from .controller import Controller
```

### Comparing `autora-workflow-0.1.0/src/autora/workflow/__main__.py` & `autora-workflow-0.2.0/src/autora/workflow/__main__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/src/autora/workflow/base.py` & `autora-workflow-0.2.0/src/autora/workflow/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     def run(self, num_steps: int = 1):
         """Execute the next step in the cycle."""
         for i in range(num_steps):
             next(self)
         return self
 
     def __next__(self):
-
         # Plan
         next_function_name = self.planner(self.state)
 
         # Map
         next_function = self.executor_collection[next_function_name]
         next_params = self.state.params.get(next_function_name, {})
```

### Comparing `autora-workflow-0.1.0/src/autora/workflow/controller.py` & `autora-workflow-0.2.0/src/autora/workflow/controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """  The cycle controller for AER. """
 from __future__ import annotations
 
 import logging
 import pathlib
 from typing import Callable, Dict, Optional
 
-from sklearn.base import BaseEstimator
-
 from autora.experimentalist.pipeline import Pipeline
 from autora.variable import VariableCollection
+from sklearn.base import BaseEstimator
 
 from .base import BaseController
 from .executor import make_online_executor_collection
 from .planner import last_result_kind_planner
 from .serializer import HistorySerializer
 from .state import History
 
@@ -22,35 +21,35 @@
 class Controller(BaseController[History]):
     """
     Runs an experimentalist, experiment runner, and theorist in order.
 
     Once initialized, the `controller` can be started by calling `next(controller)` or using the
         `controller.run` method. Each iteration runs the next logical step based on the last
         result:
-    – if the last result doesn't exist or is a theory, run the experimentalist and add an
+    – if the last result doesn't exist or is a model, run the experimentalist and add an
         experimental condition as a new result,
     - if the last result is an experimental condition, run the experiment runner and add an
        observation as a new result,
-    - if the last result is an observation, run the theorist and add a theory as a new result.
+    - if the last result is an observation, run the theorist and add a model as a new result.
 
     """
 
     def __init__(
         self,
-        metadata: Optional[VariableCollection] = None,
+        variables: Optional[VariableCollection] = None,
         theorist: Optional[BaseEstimator] = None,
         experimentalist: Optional[Pipeline] = None,
         experiment_runner: Optional[Callable] = None,
         params: Optional[Dict] = None,
         monitor: Optional[Callable[[History], None]] = None,
         planner: Callable[[History], str] = last_result_kind_planner,
     ):
         """
         Args:
-            metadata: a description of the dependent and independent variables
+            variables: a description of the dependent and independent variables
             theorist: a scikit-learn-compatible estimator
             experimentalist: an autora.experimentalist.Pipeline
             experiment_runner: a function to map independent variables onto observed dependent
                 variables
             monitor: a function which gets read-only access to the `data` attribute at the end of
                 each cycle.
             params: a nested dictionary with parameters to be passed to the parts of the cycle.
@@ -60,18 +59,18 @@
             planner: a function which maps from the state to the next ExecutorName. The default
                 is to map from the last result in the state's history to the next logical step.
         """
 
         if params is None:
             params = {}
         state = History(
-            metadata=metadata,
+            variables=variables,
             conditions=[],
             observations=[],
-            theories=[],
+            models=[],
             params=params,
         )
 
         self._experimentalist_pipeline = experimentalist
         self._experiment_runner_callable = experiment_runner
         self._theorist_estimator = theorist
```

### Comparing `autora-workflow-0.1.0/src/autora/workflow/cycle.py` & `autora-workflow-0.2.0/src/autora/workflow/cycle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """  The cycle controller for AER. """
 from __future__ import annotations
 
 import logging
 from typing import Callable, Dict, Optional
 
-from sklearn.base import BaseEstimator
-
 from autora.experimentalist.pipeline import Pipeline
 from autora.variable import VariableCollection
+from sklearn.base import BaseEstimator
 
 from .base import BaseController
 from .executor import make_default_online_executor_collection
 from .planner import full_cycle_planner
 from .state import Snapshot
 
 _logger = logging.getLogger(__name__)
@@ -25,42 +24,42 @@
         `cycle.run` method. Each iteration runs the full AER cycle, starting with the
         experimentalist and ending with the theorist.
 
     """
 
     def __init__(
         self,
-        metadata: VariableCollection,
+        variables: VariableCollection,
         theorist: Optional[BaseEstimator] = None,
         experimentalist: Optional[Pipeline] = None,
         experiment_runner: Optional[Callable] = None,
         params: Optional[Dict] = None,
         monitor: Optional[Callable[[Snapshot], None]] = None,
     ):
         """
         Args:
-            metadata: a description of the dependent and independent variables
+            variables: a description of the dependent and independent variables
             theorist: a scikit-learn-compatible estimator
             experimentalist: an autora.experimentalist.Pipeline
             experiment_runner: a function to map independent variables onto observed dependent
                 variables
             monitor: a function which gets read-only access to the `data` attribute at the end of
                 each cycle.
             params: a nested dictionary with parameters to be passed to the parts of the cycle.
                 E.g. if the experimentalist had a step named "pool" which took an argument "n",
                 which you wanted to set to the value 30, then params would be set to this:
                 `{"experimentalist": {"pool": {"n": 30}}}`
         """
         if params is None:
             params = {}
         state = Snapshot(
-            metadata=metadata,
+            variables=variables,
             conditions=[],
             observations=[],
-            theories=[],
+            models=[],
             params={"full_cycle": params},
         )
         planner = full_cycle_planner
 
         self._experimentalist_pipeline = experimentalist
         self._experiment_runner_callable = experiment_runner
         self._theorist_estimator = theorist
@@ -99,15 +98,15 @@
          'experiment_runner': {... params for experiment_runner ...},
          'theorist': {... params for theorist ...}}
         ```
 
         Examples:
             >>> from autora.workflow.cycle import Cycle
             >>> p = {"some": "params"}
-            >>> c = Cycle(metadata=None, theorist=None, experimentalist=None,
+            >>> c = Cycle(variables=None, theorist=None, experimentalist=None,
             ...                 experiment_runner=None, params=p)
             >>> c.params
             {'some': 'params'}
 
             >>> c.params = {"new": "value"}
             >>> c.params
             {'new': 'value'}
@@ -117,20 +116,20 @@
     @params.setter
     def params(self, value):
         self.state = self.state.update(params={"full_cycle": value})
 
     @property
     def theorist(self):
         """
-        Generates new theories.
+        Generates new models.
 
         Examples:
             >>> from autora.workflow.cycle import Cycle
             >>> from sklearn.linear_model import LinearRegression, PoissonRegressor
-            >>> c = Cycle(metadata=None, theorist=LinearRegression(), experimentalist=None,
+            >>> c = Cycle(variables=None, theorist=LinearRegression(), experimentalist=None,
             ...                 experiment_runner=None)
             >>> c.theorist
             LinearRegression()
 
             >>> c.theorist = PoissonRegressor()
             >>> c.theorist
             PoissonRegressor()
@@ -147,15 +146,15 @@
     def experimentalist(self):
         """
         Generates new experimental conditions.
 
         Examples:
             >>> from autora.workflow.cycle import Cycle
             >>> from autora.experimentalist.pipeline import Pipeline
-            >>> c = Cycle(metadata=None, theorist=None, experiment_runner=None,
+            >>> c = Cycle(variables=None, theorist=None, experiment_runner=None,
             ...                 experimentalist=Pipeline([("pool", [11,12,13])]))
             >>> c.experimentalist
             Pipeline(steps=[('pool', [11, 12, 13])], params={})
 
             >>> c.experimentalist = Pipeline([('pool', [21,22,23])])
             >>> c.experimentalist
             Pipeline(steps=[('pool', [21, 22, 23])], params={})
@@ -172,15 +171,15 @@
     def experiment_runner(self):
         """
         Generates new observations.
 
         Examples:
             >>> from autora.workflow.cycle import Cycle
             >>> def plus_one(x): return x + 1
-            >>> c = Cycle(metadata=None, theorist=None, experimentalist=None,
+            >>> c = Cycle(variables=None, theorist=None, experimentalist=None,
             ...                 experiment_runner=plus_one)
             >>> c.experiment_runner  # doctest: +ELLIPSIS
             <function plus_one at 0x...>
             >>> c.experiment_runner(1)
             2
 
             >>> def plus_two(x): return x + 2
```

### Comparing `autora-workflow-0.1.0/src/autora/workflow/executor.py` & `autora-workflow-0.2.0/src/autora/workflow/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 import pprint
 from functools import partial
 from types import MappingProxyType
 from typing import Callable, Dict, Iterable, Literal, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
-from sklearn.base import BaseEstimator
-
 from autora.experimentalist.pipeline import Pipeline
+from sklearn.base import BaseEstimator
 
 from .protocol import SupportsControllerState
 from .state import resolve_state_params
 
 _logger = logging.getLogger(__name__)
 
 
@@ -75,28 +74,28 @@
 
 
 def theorist_wrapper(
     state: SupportsControllerState, estimator: BaseEstimator, params: Dict
 ) -> SupportsControllerState:
     """Interface for running the theorist estimator given some State."""
     params_ = resolve_state_params(params, state)
-    metadata = state.metadata
+    variables = state.variables
     observations = state.observations
     assert (
         len(observations) >= 1
     ), f"{observations=} needs at least one entry for model fitting"
 
     if isinstance(observations[-1], pd.DataFrame):
         all_observations = pd.concat(observations)
-        iv_names = [iv.name for iv in metadata.independent_variables]
-        dv_names = [dv.name for dv in metadata.dependent_variables]
+        iv_names = [iv.name for iv in variables.independent_variables]
+        dv_names = [dv.name for dv in variables.dependent_variables]
         x, y = all_observations[iv_names], all_observations[dv_names]
     elif isinstance(observations[-1], np.ndarray):
         all_observations = np.row_stack(observations)
-        n_xs = len(metadata.independent_variables)
+        n_xs = len(variables.independent_variables)
         x, y = all_observations[:, :n_xs], all_observations[:, n_xs:]
         if y.shape[1] == 1:
             y = y.ravel()
     else:
         raise NotImplementedError(f"type {observations[-1]=} not supported")
 
     new_theorist = copy.deepcopy(estimator)
@@ -109,15 +108,15 @@
         )
     except AttributeError:
         _logger.debug(
             f"fitted {new_theorist=} "
             f"new_theorist has no __dict__ attribute, so no results are shown"
         )
 
-    new_state = state.update(theories=[new_theorist])
+    new_state = state.update(models=[new_theorist])
     return new_state
 
 
 def full_cycle_wrapper(
     state: SupportsControllerState,
     experimentalist_pipeline: Pipeline,
     experiment_runner_callable: Callable,
```

### Comparing `autora-workflow-0.1.0/src/autora/workflow/planner.py` & `autora-workflow-0.2.0/src/autora/workflow/planner.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     """
     return "full_cycle"
 
 
 def last_result_kind_planner(state: SupportsControllerStateHistory):
     """
-    Chooses the operation based on the last result, e.g. new theory -> run experimentalist.
+    Chooses the operation based on the last result, e.g. new model -> run experimentalist.
 
     Interpretation: The "traditional" autora.workflow – a systematic research assistant.
 
     Examples:
         We initialize a new list to run our planner on:
         >>> from autora.workflow.state import History
         >>> state_ = History()
@@ -40,33 +40,33 @@
         'experiment_runner'
 
         ... or if we last produced observations, then we could now run the theorist:
         >>> state_ = state_.update(observations=["some observation"])
         >>> last_result_kind_planner(state_)
         'theorist'
 
-        ... or if we last produced a theory, then we could now run the experimentalist:
-        >>> state_ = state_.update(theories=["some theory"])
+        ... or if we last produced a model, then we could now run the experimentalist:
+        >>> state_ = state_.update(models=["some model"])
         >>> last_result_kind_planner(state_)
         'experimentalist'
 
     """
 
     filtered_history = state.filter_by(
-        kind={ResultKind.CONDITION, ResultKind.OBSERVATION, ResultKind.THEORY}
+        kind={ResultKind.CONDITION, ResultKind.OBSERVATION, ResultKind.MODEL}
     ).history
 
     try:
         last_result_kind = filtered_history[-1].kind
     except IndexError:
         last_result_kind = None
 
     executor_name = {
         None: "experimentalist",
-        ResultKind.THEORY: "experimentalist",
+        ResultKind.MODEL: "experimentalist",
         ResultKind.CONDITION: "experiment_runner",
         ResultKind.OBSERVATION: "theorist",
     }[last_result_kind]
 
     return executor_name
```

### Comparing `autora-workflow-0.1.0/src/autora/workflow/plotting.py` & `autora-workflow-0.2.0/src/autora/workflow/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,20 +27,21 @@
     Args:
         state: AER Cycle object that has been run
 
     Returns: Tuple of 2 lists of tuples
 
     """
     l_iv = [
-        (i, s.name, s.units) for i, s in enumerate(state.metadata.independent_variables)
+        (i, s.name, s.units)
+        for i, s in enumerate(state.variables.independent_variables)
     ]
     n_iv = len(l_iv)
     l_dv = [
         (i + n_iv, s.name, s.units)
-        for i, s in enumerate(state.metadata.dependent_variables)
+        for i, s in enumerate(state.variables.dependent_variables)
     ]
     return l_iv, l_dv
 
 
 def _observed_to_df(state: SupportsControllerState) -> pd.DataFrame:
     """
     Concatenates observation data of cycles into a single dataframe with a field "cycle" with the
@@ -68,15 +69,15 @@
     Args:
         state: AER Cycle object that has been run
 
     Returns: List of tuples
 
     """
     l_return = []
-    iv_index = range(len(state.metadata.independent_variables))
+    iv_index = range(len(state.variables.independent_variables))
     l_observations = state.observations
     # Get min and max of observation data
     # Min and max by cycle - All IVs
     l_mins = [np.min(s, axis=0) for s in l_observations]  # Arrays by columns
     l_maxs = [np.max(s, axis=0) for s in l_observations]
     # Min and max for all cycles by IVs
     for idx in iv_index:
@@ -126,33 +127,33 @@
 
     for min_max in l_min_max:
         l_space.append(np.linspace(min_max[0], min_max[1], steps))
 
     return np.meshgrid(*l_space)
 
 
-def _theory_predict(
+def _model_predict(
     state: SupportsControllerState, conditions: Sequence, predict_proba: bool = False
 ) -> list:
     """
-    Gets theory predictions over conditions space and saves results of each cycle to a list.
+    Gets model predictions over conditions space and saves results of each cycle to a list.
     Args:
         state: AER Cycle object that has been run
         conditions: Condition space. Should be an array of grouped conditions.
         predict_proba: Use estimator.predict_proba method instead of estimator.predict.
 
     Returns: list
 
     """
     l_predictions = []
-    for i, theory in enumerate(state.theories):
+    for i, model in enumerate(state.models):
         if not predict_proba:
-            l_predictions.append(theory.predict(conditions))
+            l_predictions.append(model.predict(conditions))
         else:
-            l_predictions.append(theory.predict_proba(conditions))
+            l_predictions.append(model.predict_proba(conditions))
 
     return l_predictions
 
 
 def _check_replace_default_kw(default: dict, user: dict) -> dict:
     """
     Combines the key/value pairs of two dictionaries, a default and user dictionary. Unique pairs
@@ -187,41 +188,41 @@
     dv_name: Optional[str] = None,
     steps: int = 50,
     wrap: int = 4,
     query: Optional[Union[List, slice]] = None,
     subplot_kw: dict = {},
     scatter_previous_kw: dict = {},
     scatter_current_kw: dict = {},
-    plot_theory_kw: dict = {},
+    plot_model_kw: dict = {},
 ) -> plt.figure:
     """
     Generates a multi-panel figure with 2D plots showing results of one AER cycle.
 
     Observed data is plotted as a scatter plot with the current cycle colored differently than
-    observed data from previous cycles. The current cycle's theory is plotted as a line over the
+    observed data from previous cycles. The current cycle's model is plotted as a line over the
     range of the observed data.
 
     Args:
         state: AER Cycle object that has been run
         iv_name: Independent variable name. Name should match the name instantiated in the cycle
                     object. Default will select the first.
         dv_name: Single dependent variable name. Name should match the names instantiated in the
                     cycle object. Default will select the first DV.
-        steps: Number of steps to define the condition space to plot the theory.
+        steps: Number of steps to define the condition space to plot the model.
         wrap: Number of panels to appear in a row. Example: 9 panels with wrap=3 results in a
                 3x3 grid.
         query: Query which cycles to plot with either a List of indexes or a slice. The slice must
                 be constructed with the `slice()` function or `np.s_[]` index expression.
         subplot_kw: Dictionary of keywords to pass to matplotlib 'subplot' function
         scatter_previous_kw: Dictionary of keywords to pass to matplotlib 'scatter' function that
                     plots the data points from previous cycles.
         scatter_current_kw: Dictionary of keywords to pass to matplotlib 'scatter' function that
                     plots the data points from the current cycle.
-        plot_theory_kw: Dictionary of keywords to pass to matplotlib 'plot' function that plots the
-                    theory line.
+        plot_model_kw: Dictionary of keywords to pass to matplotlib 'plot' function that plots the
+                    model line.
 
     Returns: matplotlib figure
 
     """
 
     # ---Figure and plot params---
     # Set defaults, check and add user supplied keywords
@@ -239,32 +240,32 @@
     }
     scatter_current_defaults = {
         "color": "tab:orange",
         "s": 2,
         "alpha": 0.6,
         "label": "New Data",
     }
-    line_kw_defaults = {"label": "Theory"}
+    line_kw_defaults = {"label": "Model"}
     # Combine default and user supplied keywords
     d_kw = {}
     for d1, d2, key in zip(
         [
             subplot_kw_defaults,
             scatter_previous_defaults,
             scatter_current_defaults,
             line_kw_defaults,
         ],
-        [subplot_kw, scatter_previous_kw, scatter_current_kw, plot_theory_kw],
-        ["subplot_kw", "scatter_previous_kw", "scatter_current_kw", "plot_theory_kw"],
+        [subplot_kw, scatter_previous_kw, scatter_current_kw, plot_model_kw],
+        ["subplot_kw", "scatter_previous_kw", "scatter_current_kw", "plot_model_kw"],
     ):
         assert isinstance(d1, dict)
         assert isinstance(d2, dict)
         d_kw[key] = _check_replace_default_kw(d1, d2)
 
-    # ---Extract IVs and DV metadata and indexes---
+    # ---Extract IVs and DV variables and indexes---
     ivs, dvs = _get_variable_index(state)
     if iv_name:
         iv = [s for s in ivs if s[1] == iv_name][0]
     else:
         iv = [ivs[0]][0]
     if dv_name:
         dv = [s for s in dvs if s[1] == dv_name][0]
@@ -275,19 +276,19 @@
 
     # Create a dataframe of observed data from cycle
     df_observed = _observed_to_df(state)
 
     # Generate IV space
     condition_space = _generate_condition_space(state, steps=steps)
 
-    # Get theory predictions over space
-    l_predictions = _theory_predict(state, condition_space)
+    # Get model predictions over space
+    l_predictions = _model_predict(state, condition_space)
 
     # Cycle Indexing
-    cycle_idx = list(range(len(state.theories)))
+    cycle_idx = list(range(len(state.models)))
     if query:
         if isinstance(query, list):
             cycle_idx = [cycle_idx[s] for s in query]
         elif isinstance(query, slice):
             cycle_idx = cycle_idx[query]
 
     # Subplot configurations
@@ -317,17 +318,17 @@
             dv_current = np.ma.masked_where(
                 df_observed["cycle"] != i_cycle, df_observed[dv[0]]
             )
             # Plotting scatter
             ax.scatter(x_vals, dv_previous, **d_kw["scatter_previous_kw"])
             ax.scatter(x_vals, dv_current, **d_kw["scatter_current_kw"])
 
-            # ---Plot Theory---
+            # ---Plot Model---
             conditions = condition_space[:, iv[0]]
-            ax.plot(conditions, l_predictions[i_cycle], **d_kw["plot_theory_kw"])
+            ax.plot(conditions, l_predictions[i_cycle], **d_kw["plot_model_kw"])
 
             # Label Panels
             ax.text(
                 0.05, 1, f"Cycle {i_cycle}", ha="left", va="top", transform=ax.transAxes
             )
 
         else:
@@ -335,15 +336,15 @@
 
     # Super Labels
     fig.supxlabel(iv_label, y=0.07)
     fig.supylabel(dv_label)
 
     # Legend
     fig.legend(
-        ["Previous Data", "New Data", "Theory"],
+        ["Previous Data", "New Data", "Model"],
         ncols=3,
         bbox_to_anchor=(0.5, 0),
         loc="lower center",
     )
 
     return fig
 
@@ -360,50 +361,50 @@
     scatter_current_kw: dict = {},
     surface_kw: dict = {},
 ) -> plt.figure:
     """
     Generates a multi-panel figure with 3D plots showing results of one AER cycle.
 
     Observed data is plotted as a scatter plot with the current cycle colored differently than
-    observed data from previous cycles. The current cycle's theory is plotted as a line over the
+    observed data from previous cycles. The current cycle's model is plotted as a line over the
     range of the observed data.
 
     Args:
 
         state: AER Cycle object that has been run
         iv_names: List of up to 2 independent variable names. Names should match the names
                     instantiated in the cycle object. Default will select up to the first two.
         dv_name: Single DV name. Name should match the names instantiated in the cycle object.
                     Default will select the first DV
-        steps: Number of steps to define the condition space to plot the theory.
+        steps: Number of steps to define the condition space to plot the model.
         wrap: Number of panels to appear in a row. Example: 9 panels with wrap=3 results in a
                 3x3 grid.
         view: Tuple of elevation angle and azimuth to change the viewing angle of the plot.
         subplot_kw: Dictionary of keywords to pass to matplotlib 'subplot' function
         scatter_previous_kw: Dictionary of keywords to pass to matplotlib 'scatter' function that
                     plots the data points from previous cycles.
         scatter_current_kw: Dictionary of keywords to pass to matplotlib 'scatter' function that
                     plots the data points from the current cycle.
         surface_kw: Dictionary of keywords to pass to matplotlib 'plot_surface' function that plots
-                    the theory plane.
+                    the model plane.
 
     Returns: matplotlib figure
 
     """
-    n_cycles = len(state.theories)
+    n_cycles = len(state.models)
 
     # ---Figure and plot params---
     # Set defaults, check and add user supplied keywords
     # Default keywords
     subplot_kw_defaults = {
         "subplot_kw": {"projection": "3d"},
     }
     scatter_previous_defaults = {"color": "black", "s": 2, "label": "Previous Data"}
     scatter_current_defaults = {"color": "tab:orange", "s": 2, "label": "New Data"}
-    surface_kw_defaults = {"alpha": 0.5, "label": "Theory"}
+    surface_kw_defaults = {"alpha": 0.5, "label": "Model"}
     # Combine default and user supplied keywords
     d_kw = {}
     for d1, d2, key in zip(
         [
             subplot_kw_defaults,
             scatter_previous_defaults,
             scatter_current_defaults,
@@ -412,15 +413,15 @@
         [subplot_kw, scatter_previous_kw, scatter_current_kw, surface_kw],
         ["subplot_kw", "scatter_previous_kw", "scatter_current_kw", "surface_kw"],
     ):
         assert isinstance(d1, dict)
         assert isinstance(d2, dict)
         d_kw[key] = _check_replace_default_kw(d1, d2)
 
-    # ---Extract IVs and DV metadata and indexes---
+    # ---Extract IVs and DV variables and indexes---
     ivs, dvs = _get_variable_index(state)
     if iv_names:
         iv = [s for s in ivs if s[1] == iv_names]
     else:
         iv = ivs[:2]
     if dv_name:
         dv = [s for s in dvs if s[1] == dv_name][0]
@@ -431,44 +432,43 @@
 
     # Create a dataframe of observed data from cycle
     df_observed = _observed_to_df(state)
 
     # Generate IV Mesh Grid
     x1, x2 = _generate_mesh_grid(state, steps=steps)
 
-    # Get theory predictions over space
-    l_predictions = _theory_predict(state, np.column_stack((x1.ravel(), x2.ravel())))
+    # Get model predictions over space
+    l_predictions = _model_predict(state, np.column_stack((x1.ravel(), x2.ravel())))
 
     # Subplot configurations
     if n_cycles < wrap:
         shape = (1, n_cycles)
     else:
         shape = (int(np.ceil(n_cycles / wrap)), wrap)
 
     fig, axs = plt.subplots(*shape, **d_kw["subplot_kw"])
 
     # Loop by panel
     for i, ax in enumerate(axs.flat):
         if i + 1 <= n_cycles:
-
             # ---Plot observed data---
             # Independent variable values
             l_x = [df_observed.loc[:, s[0]] for s in iv]
             # Dependent values masked by current cycle vs previous data
             dv_previous = np.ma.masked_where(
                 df_observed["cycle"] >= i, df_observed[dv[0]]
             )
             dv_current = np.ma.masked_where(
                 df_observed["cycle"] != i, df_observed[dv[0]]
             )
             # Plotting scatter
             ax.scatter(*l_x, dv_previous, **d_kw["scatter_previous_kw"])
             ax.scatter(*l_x, dv_current, **d_kw["scatter_current_kw"])
 
-            # ---Plot Theory---
+            # ---Plot Model---
             ax.plot_surface(
                 x1, x2, l_predictions[i].reshape(x1.shape), **d_kw["surface_kw"]
             )
             # ---Labels---
             # Title
             ax.set_title(f"Cycle {i}")
 
@@ -511,15 +511,15 @@
         state: AER Cycle object that has been run
         x_vals: Test dataset independent values
         y_true: Test dataset dependent values
 
     Returns:
         List of scores by cycle
     """
-    l_scores = [s.score(x_vals, y_true) for s in state.theories]
+    l_scores = [s.score(x_vals, y_true) for s in state.models]
     return l_scores
 
 
 def cycle_specified_score(
     scorer: Callable,
     state: SupportsControllerState,
     x_vals: np.ndarray,
@@ -536,17 +536,17 @@
         **kwargs: Keyword arguments to send to scoring function
 
     Returns:
 
     """
     # Get predictions
     if "y_pred" in inspect.signature(scorer).parameters.keys():
-        l_y_pred = _theory_predict(state, x_vals, predict_proba=False)
+        l_y_pred = _model_predict(state, x_vals, predict_proba=False)
     elif "y_score" in inspect.signature(scorer).parameters.keys():
-        l_y_pred = _theory_predict(state, x_vals, predict_proba=True)
+        l_y_pred = _model_predict(state, x_vals, predict_proba=True)
 
     # Score each cycle
     l_scores = []
     for y_pred in l_y_pred:
         l_scores.append(scorer(y_true, y_pred, **kwargs))
 
     return l_scores
@@ -562,15 +562,15 @@
     figsize: Tuple[float, float] = rcParams["figure.figsize"],
     ylim: Optional[Tuple[float, float]] = None,
     xlim: Optional[Tuple[float, float]] = None,
     scorer_kw: dict = {},
     plot_kw: dict = {},
 ) -> plt.Figure:
     """
-    Plots scoring metrics of cycle's theories given test data.
+    Plots scoring metrics of cycle's models given test data.
     Args:
         state: AER Cycle object that has been run
         X: Test dataset independent values
         y_true: Test dataset dependent values
         scorer: sklearn scoring function (optional)
         x_label: Label for x-axis
         y_label: Label for y-axis
@@ -588,15 +588,15 @@
     if scorer is None:
         l_scores = cycle_default_score(state, X, y_true)
     else:
         l_scores = cycle_specified_score(scorer, state, X, y_true, **scorer_kw)
 
     # Plotting
     fig, ax = plt.subplots(figsize=figsize)
-    ax.plot(np.arange(len(state.theories)), l_scores, **plot_kw)
+    ax.plot(np.arange(len(state.models)), l_scores, **plot_kw)
 
     # Adjusting axis limits
     if ylim:
         ax.set_ylim(*ylim)
     if xlim:
         ax.set_xlim(*xlim)
```

### Comparing `autora-workflow-0.1.0/src/autora/workflow/protocol.py` & `autora-workflow-0.2.0/src/autora/workflow/protocol.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,51 +8,50 @@
     Sequence,
     Set,
     TypeVar,
     Union,
     runtime_checkable,
 )
 
+from autora.variable import VariableCollection
 from numpy.typing import ArrayLike
 from sklearn.base import BaseEstimator
 
-from autora.variable import VariableCollection
-
 State = TypeVar("State")
 
 
 class ResultKind(str, Enum):
     """
     Kinds of results which can be held in the Result object.
 
     Examples:
         >>> ResultKind.CONDITION is ResultKind.CONDITION
         True
 
-        >>> ResultKind.CONDITION is ResultKind.METADATA
+        >>> ResultKind.CONDITION is ResultKind.VARIABLES
         False
 
         >>> ResultKind.CONDITION == "CONDITION"
         True
 
-        >>> ResultKind.CONDITION == "METADATA"
+        >>> ResultKind.CONDITION == "VARIABLES"
         False
 
         >>> ResultKind.CONDITION in {ResultKind.CONDITION, ResultKind.PARAMS}
         True
 
-        >>> ResultKind.METADATA in {ResultKind.CONDITION, ResultKind.PARAMS}
+        >>> ResultKind.VARIABLES in {ResultKind.CONDITION, ResultKind.PARAMS}
         False
     """
 
     CONDITION = "CONDITION"
     OBSERVATION = "OBSERVATION"
-    THEORY = "THEORY"
+    MODEL = "MODEL"
     PARAMS = "PARAMS"
-    METADATA = "METADATA"
+    VARIABLES = "VARIABLES"
 
     def __repr__(self):
         cls_name = self.__class__.__name__
         return f"{cls_name}.{self.name}"
 
 
 class SupportsDataKind(Protocol):
@@ -61,32 +60,32 @@
     data: Optional[Any]
     kind: Optional[ResultKind]
 
 
 class SupportsControllerStateFields(Protocol):
     """Support representing snapshots of a controller state as mutable fields."""
 
-    metadata: VariableCollection
+    variables: VariableCollection
     params: Dict
     conditions: Sequence[ArrayLike]
     observations: Sequence[ArrayLike]
-    theories: Sequence[BaseEstimator]
+    models: Sequence[BaseEstimator]
 
     def update(self: State, **kwargs) -> State:
         ...
 
 
 class SupportsControllerStateProperties(Protocol):
     """Support representing snapshots of a controller state as immutable properties."""
 
     def update(self: State, **kwargs) -> State:
         ...
 
     @property
-    def metadata(self) -> VariableCollection:
+    def variables(self) -> VariableCollection:
         ...
 
     @property
     def params(self) -> Dict:
         ...
 
     @property
@@ -94,15 +93,15 @@
         ...
 
     @property
     def observations(self) -> Sequence[ArrayLike]:
         ...
 
     @property
-    def theories(self) -> Sequence[BaseEstimator]:
+    def models(self) -> Sequence[BaseEstimator]:
         ...
 
 
 SupportsControllerState = Union[
     SupportsControllerStateFields, SupportsControllerStateProperties
 ]
```

### Comparing `autora-workflow-0.1.0/src/autora/workflow/serializer/__init__.py` & `autora-workflow-0.2.0/src/autora/workflow/serializer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,19 +42,19 @@
         self.path = path
         self._check_path()
 
         self._result_kind_serializer_mapping: Mapping[
             Union[None, ResultKind], _DumpSpec
         ] = {
             None: _DumpSpec("yaml", YAMLSerializer, "w+"),
-            ResultKind.METADATA: _DumpSpec("yaml", YAMLSerializer, "w+"),
+            ResultKind.VARIABLES: _DumpSpec("yaml", YAMLSerializer, "w+"),
             ResultKind.PARAMS: _DumpSpec("yaml", YAMLSerializer, "w+"),
             ResultKind.CONDITION: _DumpSpec("yaml", YAMLSerializer, "w+"),
             ResultKind.OBSERVATION: _DumpSpec("yaml", YAMLSerializer, "w+"),
-            ResultKind.THEORY: _DumpSpec("pickle", pickle, "w+b"),
+            ResultKind.MODEL: _DumpSpec("pickle", pickle, "w+b"),
         }
 
         self._extension_loader_mapping: Mapping[str, _LoadSpec] = {
             ".yaml": _LoadSpec(YAMLSerializer, "r"),
             ".pickle": _LoadSpec(pickle, "rb"),
         }
 
@@ -87,43 +87,43 @@
             ...         print(sorted(os.listdir(d)))
 
             >>> dump_and_list(c)
             []
 
             Each immutable part gets its own file.
             >>> from autora.variable import VariableCollection
-            >>> c = c.update(metadata=[VariableCollection()])
+            >>> c = c.update(variables=[VariableCollection()])
             >>> dump_and_list(c)
-            ['00000000-METADATA.yaml']
+            ['00000000-VARIABLES.yaml']
 
             The next step is to plan the first observations by defining experimental conditions.
-            Thes are appended as a Result with the correct metadata.
+            Thes are appended as a Result with the correct variables.
             >>> import numpy as np
             >>> x = np.linspace(-2, 2, 10).reshape(-1, 1) * np.pi
             >>> c = c.update(conditions=[x])
 
             If we dump and list again, we see that the new data are  included as a new file in
             the same directory.
             >>> dump_and_list(c)
-            ['00000000-METADATA.yaml', '00000001-CONDITION.yaml']
+            ['00000000-VARIABLES.yaml', '00000001-CONDITION.yaml']
 
             Then, once we've gathered real data, we dump these too:
             >>> y = 3. * x + 0.1 * np.sin(x - 0.1) - 2.
             >>> c = c.update(observations=[np.column_stack([x, y])])
             >>> dump_and_list(c)
-            ['00000000-METADATA.yaml', '00000001-CONDITION.yaml', '00000002-OBSERVATION.yaml']
+            ['00000000-VARIABLES.yaml', '00000001-CONDITION.yaml', '00000002-OBSERVATION.yaml']
 
-            We can also include a theory in the dump.
-            The theory is saved as a pickle file by default.
+            We can also include a model in the dump.
+            The model is saved as a pickle file by default.
             >>> from sklearn.linear_model import LinearRegression
             >>> estimator = LinearRegression().fit(x, y)
-            >>> c = c.update(theories=[estimator])
+            >>> c = c.update(models=[estimator])
             >>> dump_and_list(c)  # doctest: +NORMALIZE_WHITESPACE
-            ['00000000-METADATA.yaml', '00000001-CONDITION.yaml', '00000002-OBSERVATION.yaml',
-             '00000003-THEORY.pickle']
+            ['00000000-VARIABLES.yaml', '00000001-CONDITION.yaml', '00000002-OBSERVATION.yaml',
+             '00000003-MODEL.pickle']
 
 
         """
         path = self.path
         self._check_path()
 
         for i, container in enumerate(data_collection.history):
@@ -147,31 +147,31 @@
             >>> from autora.variable import VariableCollection
             >>> import numpy as np
             >>> from autora.workflow.state.history import History
             >>> import tempfile
             >>> x = np.linspace(-2, 2, 10).reshape(-1, 1) * np.pi
             >>> y = 3. * x + 0.1 * np.sin(x - 0.1) - 2.
             >>> estimator = LinearRegression().fit(x, y)
-            >>> c = History(metadata=VariableCollection(), conditions=[x],
-            ...     observations=[np.column_stack([x, y])], theories=[estimator])
+            >>> c = History(variables=VariableCollection(), conditions=[x],
+            ...     observations=[np.column_stack([x, y])], models=[estimator])
 
             Now we can serialize the data using _dumper, and reload the data using _loader:
             >>> with tempfile.TemporaryDirectory() as d:
             ...     s = HistorySerializer(d)
             ...     s.dump(c)
             ...     e = s.load()
 
             We can now compare the dumped object "c" with the reloaded object "e". The data arrays
-            should be equal, and the theories should
+            should be equal, and the models should
             >>> from autora.workflow.protocol import ResultKind
             >>> for e_i, c_i in zip(e.history, c.history):
             ...     assert isinstance(e_i.data, type(c_i.data)) # Types match
             ...     if e_i.kind in (ResultKind.CONDITION, ResultKind.OBSERVATION):
             ...         np.testing.assert_array_equal(e_i.data, c_i.data) # two numpy arrays
-            ...     if e_i.kind == ResultKind.THEORY:
+            ...     if e_i.kind == ResultKind.MODEL:
             ...         np.testing.assert_array_equal(e_i.data.coef_, c_i.data.coef_) # 2 estimators
 
 
             We can also have the function load a subclass of the History object, or something
             else which supports its interface:
             >>> class DerivedHistory(History):
             ...     pass
```

### Comparing `autora-workflow-0.1.0/src/autora/workflow/state/history.py` & `autora-workflow-0.2.0/src/autora/workflow/state/history.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,165 +1,165 @@
 """ Classes for storing and passing a cycle's state as an immutable history. """
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Set, Union
 
+from autora.variable import VariableCollection
 from numpy.typing import ArrayLike
 from sklearn.base import BaseEstimator
 
-from autora.variable import VariableCollection
-
 from ..protocol import ResultKind, SupportsControllerStateHistory, SupportsDataKind
 from .snapshot import Snapshot
 
 
 class History(SupportsControllerStateHistory):
     """
     An immutable object for tracking the state and history of an AER cycle.
     """
 
     def __init__(
         self,
-        metadata: Optional[VariableCollection] = None,
+        variables: Optional[VariableCollection] = None,
         params: Optional[Dict] = None,
         conditions: Optional[List[ArrayLike]] = None,
         observations: Optional[List[ArrayLike]] = None,
-        theories: Optional[List[BaseEstimator]] = None,
+        models: Optional[List[BaseEstimator]] = None,
         history: Optional[Sequence[Result]] = None,
     ):
         """
 
         Args:
-            metadata: a single datum to be marked as "metadata"
+            variables: a single datum to be marked as "variables"
             params: a single datum to be marked as "params"
             conditions: an iterable of data, each to be marked as "conditions"
             observations: an iterable of data, each to be marked as "observations"
-            theories: an iterable of data, each to be marked as "theories"
+            models: an iterable of data, each to be marked as "models"
             history: an iterable of Result objects to be used as the initial history.
 
         Examples:
             Empty input leads to an empty state:
             >>> History()
             History([])
 
             ... or with values for any or all of the parameters:
             >>> from autora.variable import VariableCollection
-            >>> History(metadata=VariableCollection()) # doctest: +ELLIPSIS
-            History([Result(data=VariableCollection(...), kind=ResultKind.METADATA)])
+            >>> History(variables=VariableCollection()) # doctest: +ELLIPSIS
+            History([Result(data=VariableCollection(...), kind=ResultKind.VARIABLES)])
 
             >>> History(params={"some": "params"})
             History([Result(data={'some': 'params'}, kind=ResultKind.PARAMS)])
 
             >>> History(conditions=["a condition"])
             History([Result(data='a condition', kind=ResultKind.CONDITION)])
 
             >>> History(observations=["an observation"])
             History([Result(data='an observation', kind=ResultKind.OBSERVATION)])
 
             >>> from sklearn.linear_model import LinearRegression
-            >>> History(theories=[LinearRegression()])
-            History([Result(data=LinearRegression(), kind=ResultKind.THEORY)])
+            >>> History(models=[LinearRegression()])
+            History([Result(data=LinearRegression(), kind=ResultKind.MODEL)])
 
             Parameters passed to the constructor are included in the history in the following order:
-            `history`, `metadata`, `params`, `conditions`, `observations`, `theories`
-            >>> History(theories=['t1', 't2'], conditions=['c1', 'c2'],
-            ...     observations=['o1', 'o2'], params={'a': 'param'}, metadata=VariableCollection(),
-            ...     history=[Result("from history", ResultKind.METADATA)]
+            `history`, `variables`, `params`, `conditions`, `observations`, `models`
+            >>> History(models=['m1', 'm2'], conditions=['c1', 'c2'],
+            ...     observations=['o1', 'o2'], params={'a': 'param'},
+            ...     variables=VariableCollection(),
+            ...     history=[Result("from history", ResultKind.VARIABLES)]
             ... )  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
-            History([Result(data='from history', kind=ResultKind.METADATA),
-                                    Result(data=VariableCollection(...), kind=ResultKind.METADATA),
+            History([Result(data='from history', kind=ResultKind.VARIABLES),
+                                    Result(data=VariableCollection(...), kind=ResultKind.VARIABLES),
                                     Result(data={'a': 'param'}, kind=ResultKind.PARAMS),
                                     Result(data='c1', kind=ResultKind.CONDITION),
                                     Result(data='c2', kind=ResultKind.CONDITION),
                                     Result(data='o1', kind=ResultKind.OBSERVATION),
                                     Result(data='o2', kind=ResultKind.OBSERVATION),
-                                    Result(data='t1', kind=ResultKind.THEORY),
-                                    Result(data='t2', kind=ResultKind.THEORY)])
+                                    Result(data='m1', kind=ResultKind.MODEL),
+                                    Result(data='m2', kind=ResultKind.MODEL)])
         """
         self._history: List
 
         if history is not None:
             self._history = list(history)
         else:
             self._history = []
 
         self._history += _init_result_list(
-            metadata=metadata,
+            variables=variables,
             params=params,
             conditions=conditions,
             observations=observations,
-            theories=theories,
+            models=models,
         )
 
     def update(
         self,
-        metadata=None,
+        variables=None,
         params=None,
         conditions=None,
         observations=None,
-        theories=None,
+        models=None,
         history=None,
     ):
         """
         Create a new object with updated values.
 
         Examples:
             The initial object is empty:
             >>> h0 = History()
             >>> h0
             History([])
 
-            We can update the metadata using the `.update` method:
+            We can update the variables using the `.update` method:
             >>> from autora.variable import VariableCollection
-            >>> h1 = h0.update(metadata=VariableCollection())
+            >>> h1 = h0.update(variables=VariableCollection())
             >>> h1  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
-            History([Result(data=VariableCollection(...), kind=ResultKind.METADATA)])
+            History([Result(data=VariableCollection(...), kind=ResultKind.VARIABLES)])
 
             ... the original object is unchanged:
             >>> h0
             History([])
 
-            We can update the metadata again:
-            >>> h2 = h1.update(metadata=VariableCollection(["some IV"]))
+            We can update the variables again:
+            >>> h2 = h1.update(variables=VariableCollection(["some IV"]))
             >>> h2._by_kind  # doctest: +ELLIPSIS
-            Snapshot(metadata=VariableCollection(independent_variables=['some IV'],...), ...)
+            Snapshot(variables=VariableCollection(independent_variables=['some IV'],...), ...)
 
-            ... and we see that there is only ever one metadata object returned.
+            ... and we see that there is only ever one variables object returned.
 
-            Params is treated the same way as metadata:
+            Params is treated the same way as variables:
             >>> hp = h0.update(params={'first': 'params'})
             >>> hp
             History([Result(data={'first': 'params'}, kind=ResultKind.PARAMS)])
 
             ... where only the most recent "params" object is returned from the `.params` property.
             >>> hp = hp.update(params={'second': 'params'})
             >>> hp.params
             {'second': 'params'}
 
             ... however, the full history of the params objects remains available, if needed:
             >>> hp  # doctest: +NORMALIZE_WHITESPACE
             History([Result(data={'first': 'params'}, kind=ResultKind.PARAMS),
                                     Result(data={'second': 'params'}, kind=ResultKind.PARAMS)])
 
-            When we update the conditions, observations or theories, a new entry is added to the
+            When we update the conditions, observations or models, a new entry is added to the
             history:
-            >>> h3 = h0.update(theories=["1st theory"])
+            >>> h3 = h0.update(models=["1st model"])
             >>> h3  # doctest: +NORMALIZE_WHITESPACE
-            History([Result(data='1st theory', kind=ResultKind.THEORY)])
+            History([Result(data='1st model', kind=ResultKind.MODEL)])
 
-            ... so we can see the history of all the theories, for instance.
-            >>> h3 = h3.update(theories=["2nd theory"])  # doctest: +NORMALIZE_WHITESPACE
+            ... so we can see the history of all the models, for instance.
+            >>> h3 = h3.update(models=["2nd model"])  # doctest: +NORMALIZE_WHITESPACE
             >>> h3  # doctest: +NORMALIZE_WHITESPACE
-            History([Result(data='1st theory', kind=ResultKind.THEORY),
-                                    Result(data='2nd theory', kind=ResultKind.THEORY)])
+            History([Result(data='1st model', kind=ResultKind.MODEL),
+                                    Result(data='2nd model', kind=ResultKind.MODEL)])
 
-            ... and the full history of theories is available using the `.theories` parameter:
-            >>> h3.theories
-            ['1st theory', '2nd theory']
+            ... and the full history of models is available using the `.models` parameter:
+            >>> h3.models
+            ['1st model', '2nd model']
 
             The same for the observations:
             >>> h4 = h0.update(observations=["1st observation"])
             >>> h4
             History([Result(data='1st observation', kind=ResultKind.OBSERVATION)])
 
             >>> h4.update(observations=["2nd observation"]
@@ -173,100 +173,101 @@
             >>> h5
             History([Result(data='1st condition', kind=ResultKind.CONDITION)])
 
             >>> h5.update(conditions=["2nd condition"])  # doctest: +NORMALIZE_WHITESPACE
             History([Result(data='1st condition', kind=ResultKind.CONDITION),
                                     Result(data='2nd condition', kind=ResultKind.CONDITION)])
 
-            You can also update with multiple conditions, observations and theories:
+            You can also update with multiple conditions, observations and models:
             >>> h0.update(conditions=['c1', 'c2'])  # doctest: +NORMALIZE_WHITESPACE
             History([Result(data='c1', kind=ResultKind.CONDITION),
                                     Result(data='c2', kind=ResultKind.CONDITION)])
 
-            >>> h0.update(theories=['t1', 't2'], metadata={'m': 1}) # doctest: +NORMALIZE_WHITESPACE
-            History([Result(data={'m': 1}, kind=ResultKind.METADATA),
-                                    Result(data='t1', kind=ResultKind.THEORY),
-                                    Result(data='t2', kind=ResultKind.THEORY)])
+            >>> h0.update(models=['m1', 'm2'], variables={'m': 1}
+            ... ) # doctest: +NORMALIZE_WHITESPACE
+            History([Result(data={'m': 1}, kind=ResultKind.VARIABLES),
+                     Result(data='m1', kind=ResultKind.MODEL),
+                     Result(data='m2', kind=ResultKind.MODEL)])
 
-            >>> h0.update(theories=['t1'], observations=['o1'], metadata={'m': 1}
+            >>> h0.update(models=['m1'], observations=['o1'], variables={'m': 1}
             ... )  # doctest: +NORMALIZE_WHITESPACE
-            History([Result(data={'m': 1}, kind=ResultKind.METADATA),
+            History([Result(data={'m': 1}, kind=ResultKind.VARIABLES),
                      Result(data='o1', kind=ResultKind.OBSERVATION),
-                     Result(data='t1', kind=ResultKind.THEORY)])
+                     Result(data='m1', kind=ResultKind.MODEL)])
 
             We can also update with a complete history:
-            >>> History().update(history=[Result(data={'m': 2}, kind=ResultKind.METADATA),
+            >>> History().update(history=[Result(data={'m': 2}, kind=ResultKind.VARIABLES),
             ...                           Result(data='o1', kind=ResultKind.OBSERVATION),
-            ...                           Result(data='t1', kind=ResultKind.THEORY)],
+            ...                           Result(data='m1', kind=ResultKind.MODEL)],
             ...                  conditions=['c1']
             ... )  # doctest: +NORMALIZE_WHITESPACE
-            History([Result(data={'m': 2}, kind=ResultKind.METADATA),
+            History([Result(data={'m': 2}, kind=ResultKind.VARIABLES),
                      Result(data='o1', kind=ResultKind.OBSERVATION),
-                     Result(data='t1', kind=ResultKind.THEORY),
+                     Result(data='m1', kind=ResultKind.MODEL),
                      Result(data='c1', kind=ResultKind.CONDITION)])
 
         """
 
         if history is not None:
             history_extension = history
         else:
             history_extension = []
 
         history_extension += _init_result_list(
-            metadata=metadata,
+            variables=variables,
             params=params,
             conditions=conditions,
             observations=observations,
-            theories=theories,
+            models=models,
         )
         new_full_history = self._history + history_extension
 
         return History(history=new_full_history)
 
     def __repr__(self):
         return f"{type(self).__name__}({self.history})"
 
     @property
     def _by_kind(self):
         return _history_to_kind(self._history)
 
     @property
-    def metadata(self) -> VariableCollection:
+    def variables(self) -> VariableCollection:
         """
 
         Examples:
             The initial object is empty:
             >>> h = History()
 
-            ... and returns an emtpy metadata object
-            >>> h.metadata
+            ... and returns an emtpy variables object
+            >>> h.variables
             VariableCollection(independent_variables=[], dependent_variables=[], covariates=[])
 
-            We can update the metadata using the `.update` method:
+            We can update the variables using the `.update` method:
             >>> from autora.variable import VariableCollection
-            >>> h = h.update(metadata=VariableCollection(independent_variables=['some IV']))
-            >>> h.metadata  # doctest: +ELLIPSIS
+            >>> h = h.update(variables=VariableCollection(independent_variables=['some IV']))
+            >>> h.variables  # doctest: +ELLIPSIS
             VariableCollection(independent_variables=['some IV'], ...)
 
-            We can update the metadata again:
-            >>> h = h.update(metadata=VariableCollection(["some other IV"]))
-            >>> h.metadata  # doctest: +ELLIPSIS
+            We can update the variables again:
+            >>> h = h.update(variables=VariableCollection(["some other IV"]))
+            >>> h.variables  # doctest: +ELLIPSIS
             VariableCollection(independent_variables=['some other IV'], ...)
 
-            ... and we see that there is only ever one metadata object returned."""
-        return self._by_kind.metadata
+            ... and we see that there is only ever one variables object returned."""
+        return self._by_kind.variables
 
     @property
     def params(self) -> Dict:
         """
 
         Returns:
 
         Examples:
-            Params is treated the same way as metadata:
+            Params is treated the same way as variables:
             >>> h = History()
             >>> h = h.update(params={'first': 'params'})
             >>> h.params
             {'first': 'params'}
 
             ... where only the most recent "params" object is returned from the `.params` property.
             >>> h = h.update(params={'second': 'params'})
@@ -282,15 +283,15 @@
 
     @property
     def conditions(self) -> List[ArrayLike]:
         """
         Returns:
 
         Examples:
-            View the sequence of theories with one conditions:
+            View the sequence of models with one conditions:
             >>> h = History(conditions=[(1,2,3,)])
             >>> h.conditions
             [(1, 2, 3)]
 
             ... or more conditions:
             >>> h = h.update(conditions=[(4,5,6),(7,8,9)])  # doctest: +NORMALIZE_WHITESPACE
             >>> h.conditions
@@ -315,56 +316,57 @@
             >>> h.observations  # doctest: +ELLIPSIS
             ['1st observation', '2nd observation']
 
         """
         return self._by_kind.observations
 
     @property
-    def theories(self) -> List[BaseEstimator]:
+    def models(self) -> List[BaseEstimator]:
         """
 
         Returns:
 
         Examples:
-            View the sequence of theories with one theory:
-            >>> s = History(theories=["1st theory"])
-            >>> s.theories  # doctest: +NORMALIZE_WHITESPACE
-            ['1st theory']
-
-            ... or more theories:
-            >>> s = s.update(theories=["2nd theory"])  # doctest: +NORMALIZE_WHITESPACE
-            >>> s.theories
-            ['1st theory', '2nd theory']
+            View the sequence of models with one model:
+            >>> s = History(models=["1st model"])
+            >>> s.models  # doctest: +NORMALIZE_WHITESPACE
+            ['1st model']
+
+            ... or more models:
+            >>> s = s.update(models=["2nd model"])  # doctest: +NORMALIZE_WHITESPACE
+            >>> s.models
+            ['1st model', '2nd model']
 
         """
-        return self._by_kind.theories
+        return self._by_kind.models
 
     @property
     def history(self) -> List[Result]:
         """
 
         Examples:
             We initialze some history:
-            >>> h = History(theories=['t1', 't2'], conditions=['c1', 'c2'],
-            ...     observations=['o1', 'o2'], params={'a': 'param'}, metadata=VariableCollection(),
-            ...     history=[Result("from history", ResultKind.METADATA)])
+            >>> h = History(models=['m1', 'm2'], conditions=['c1', 'c2'],
+            ...     observations=['o1', 'o2'], params={'a': 'param'},
+            ...     variables=VariableCollection(),
+            ...     history=[Result("from history", ResultKind.VARIABLES)])
 
             Parameters passed to the constructor are included in the history in the following order:
-            `history`, `metadata`, `params`, `conditions`, `observations`, `theories`
+            `history`, `variables`, `params`, `conditions`, `observations`, `models`
 
             >>> h.history  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
-            [Result(data='from history', kind=ResultKind.METADATA),
-             Result(data=VariableCollection(...), kind=ResultKind.METADATA),
+            [Result(data='from history', kind=ResultKind.VARIABLES),
+             Result(data=VariableCollection(...), kind=ResultKind.VARIABLES),
              Result(data={'a': 'param'}, kind=ResultKind.PARAMS),
              Result(data='c1', kind=ResultKind.CONDITION),
              Result(data='c2', kind=ResultKind.CONDITION),
              Result(data='o1', kind=ResultKind.OBSERVATION),
              Result(data='o2', kind=ResultKind.OBSERVATION),
-             Result(data='t1', kind=ResultKind.THEORY),
-             Result(data='t2', kind=ResultKind.THEORY)]
+             Result(data='m1', kind=ResultKind.MODEL),
+             Result(data='m2', kind=ResultKind.MODEL)]
 
             If we add a new value, like the params object, the updated value is added to the
             end of the history:
             >>> h = h.update(params={'new': 'param'})
             >>> h.history  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
             [..., Result(data={'new': 'param'}, kind=ResultKind.PARAMS)]
 
@@ -372,62 +374,63 @@
         return self._history
 
     def filter_by(self, kind: Optional[Set[Union[str, ResultKind]]] = None) -> History:
         """
         Return a copy of the object with only data belonging to the specified kinds.
 
         Examples:
-            >>> h = History(theories=['t1', 't2'], conditions=['c1', 'c2'],
-            ...     observations=['o1', 'o2'], params={'a': 'param'}, metadata=VariableCollection(),
-            ...     history=[Result("from history", ResultKind.METADATA)])
-
-            >>> h.filter_by(kind={"THEORY"})   # doctest: +NORMALIZE_WHITESPACE
-            History([Result(data='t1', kind=ResultKind.THEORY),
-                                    Result(data='t2', kind=ResultKind.THEORY)])
+            >>> h = History(models=['m1', 'm2'], conditions=['c1', 'c2'],
+            ...     observations=['o1', 'o2'], params={'a': 'param'},
+            ...    variables=VariableCollection(),
+            ...     history=[Result("from history", ResultKind.VARIABLES)])
+
+            >>> h.filter_by(kind={"MODEL"})   # doctest: +NORMALIZE_WHITESPACE
+            History([Result(data='m1', kind=ResultKind.MODEL),
+                                    Result(data='m2', kind=ResultKind.MODEL)])
 
             >>> h.filter_by(kind={ResultKind.OBSERVATION})  # doctest: +NORMALIZE_WHITESPACE
             History([Result(data='o1', kind=ResultKind.OBSERVATION),
                                     Result(data='o2', kind=ResultKind.OBSERVATION)])
 
             If we don't specify any filter criteria, we get the full history back:
             >>> h.filter_by()   # doctest: +NORMALIZE_WHITESPACE +ELLIPSIS
-            History([Result(data='from history', kind=ResultKind.METADATA),
-                     Result(data=VariableCollection(...), kind=ResultKind.METADATA),
+            History([Result(data='from history', kind=ResultKind.VARIABLES),
+                     Result(data=VariableCollection(...), kind=ResultKind.VARIABLES),
                      Result(data={'a': 'param'}, kind=ResultKind.PARAMS),
                      Result(data='c1', kind=ResultKind.CONDITION),
                      Result(data='c2', kind=ResultKind.CONDITION),
                      Result(data='o1', kind=ResultKind.OBSERVATION),
                      Result(data='o2', kind=ResultKind.OBSERVATION),
-                     Result(data='t1', kind=ResultKind.THEORY),
-                     Result(data='t2', kind=ResultKind.THEORY)])
+                     Result(data='m1', kind=ResultKind.MODEL),
+                     Result(data='m2', kind=ResultKind.MODEL)])
 
         """
         if kind is None:
             return self
         else:
             kind_ = {ResultKind(s) for s in kind}
             filtered_history = _filter_history(self._history, kind_)
             new_object = History(history=filtered_history)
             return new_object
 
 
 @dataclass(frozen=True)
 class Result(SupportsDataKind):
     """
-    Container class for data and metadata.
+    Container class for data and variables.
 
     Examples:
         >>> Result()
         Result(data=None, kind=None)
 
         >>> Result("a")
         Result(data='a', kind=None)
 
-        >>> Result(None, "THEORY")
-        Result(data=None, kind=ResultKind.THEORY)
+        >>> Result(None, "MODEL")
+        Result(data=None, kind=ResultKind.MODEL)
 
         >>> Result(data="b")
         Result(data='b', kind=None)
 
         >>> Result("c", "OBSERVATION")
         Result(data='c', kind=ResultKind.OBSERVATION)
     """
@@ -437,83 +440,83 @@
 
     def __post_init__(self):
         if isinstance(self.kind, str):
             object.__setattr__(self, "kind", ResultKind(self.kind))
 
 
 def _init_result_list(
-    metadata: Optional[VariableCollection] = None,
+    variables: Optional[VariableCollection] = None,
     params: Optional[Dict] = None,
     conditions: Optional[Iterable[ArrayLike]] = None,
     observations: Optional[Iterable[ArrayLike]] = None,
-    theories: Optional[Iterable[BaseEstimator]] = None,
+    models: Optional[Iterable[BaseEstimator]] = None,
 ) -> List[Result]:
     """
     Initialize a list of Result objects
 
     Returns:
 
     Args:
-        metadata: a single datum to be marked as "metadata"
+        variables: a single datum to be marked as "variables"
         params: a single datum to be marked as "params"
         conditions: an iterable of data, each to be marked as "conditions"
         observations: an iterable of data, each to be marked as "observations"
-        theories: an iterable of data, each to be marked as "theories"
+        models: an iterable of data, each to be marked as "models"
 
     Examples:
         Empty input leads to an empty state:
         >>> _init_result_list()
         []
 
         ... or with values for any or all of the parameters:
         >>> from autora.variable import VariableCollection
-        >>> _init_result_list(metadata=VariableCollection()) # doctest: +ELLIPSIS
-        [Result(data=VariableCollection(...), kind=ResultKind.METADATA)]
+        >>> _init_result_list(variables=VariableCollection()) # doctest: +ELLIPSIS
+        [Result(data=VariableCollection(...), kind=ResultKind.VARIABLES)]
 
         >>> _init_result_list(params={"some": "params"})
         [Result(data={'some': 'params'}, kind=ResultKind.PARAMS)]
 
         >>> _init_result_list(conditions=["a condition"])
         [Result(data='a condition', kind=ResultKind.CONDITION)]
 
         >>> _init_result_list(observations=["an observation"])
         [Result(data='an observation', kind=ResultKind.OBSERVATION)]
 
         >>> from sklearn.linear_model import LinearRegression
-        >>> _init_result_list(theories=[LinearRegression()])
-        [Result(data=LinearRegression(), kind=ResultKind.THEORY)]
+        >>> _init_result_list(models=[LinearRegression()])
+        [Result(data=LinearRegression(), kind=ResultKind.MODEL)]
 
-        The input arguments are added to the data in the order `metadata`,
-        `params`, `conditions`, `observations`, `theories`:
-        >>> _init_result_list(metadata=VariableCollection(),
+        The input arguments are added to the data in the order `variables`,
+        `params`, `conditions`, `observations`, `models`:
+        >>> _init_result_list(variables=VariableCollection(),
         ...                  params={"some": "params"},
         ...                  conditions=["a condition"],
         ...                  observations=["an observation", "another observation"],
-        ...                  theories=[LinearRegression()],
+        ...                  models=[LinearRegression()],
         ... ) # doctest: +NORMALIZE_WHITESPACE +ELLIPSIS
-        [Result(data=VariableCollection(...), kind=ResultKind.METADATA),
+        [Result(data=VariableCollection(...), kind=ResultKind.VARIABLES),
          Result(data={'some': 'params'}, kind=ResultKind.PARAMS),
          Result(data='a condition', kind=ResultKind.CONDITION),
          Result(data='an observation', kind=ResultKind.OBSERVATION),
          Result(data='another observation', kind=ResultKind.OBSERVATION),
-         Result(data=LinearRegression(), kind=ResultKind.THEORY)]
+         Result(data=LinearRegression(), kind=ResultKind.MODEL)]
 
     """
     data = []
 
-    if metadata is not None:
-        data.append(Result(metadata, ResultKind.METADATA))
+    if variables is not None:
+        data.append(Result(variables, ResultKind.VARIABLES))
 
     if params is not None:
         data.append(Result(params, ResultKind.PARAMS))
 
     for seq, kind in [
         (conditions, ResultKind.CONDITION),
         (observations, ResultKind.OBSERVATION),
-        (theories, ResultKind.THEORY),
+        (models, ResultKind.MODEL),
     ]:
         if seq is not None:
             for i in seq:
                 data.append(Result(i, kind=kind))
 
     return data
 
@@ -522,16 +525,16 @@
     """
     Convert a sequence of results into a Snapshot instance:
 
     Examples:
         History might be empty
         >>> history_ = []
         >>> _history_to_kind(history_) # doctest: +NORMALIZE_WHITESPACE +ELLIPSIS
-        Snapshot(metadata=VariableCollection(...), params={},
-                        conditions=[], observations=[], theories=[])
+        Snapshot(variables=VariableCollection(...), params={},
+                        conditions=[], observations=[], models=[])
 
         ... or with values for any or all of the parameters:
         >>> history_ = _init_result_list(params={"some": "params"})
         >>> _history_to_kind(history_) # doctest: +NORMALIZE_WHITESPACE +ELLIPSIS
         Snapshot(..., params={'some': 'params'}, ...)
 
         >>> history_ += _init_result_list(conditions=["a condition"])
@@ -543,40 +546,40 @@
 
         >>> history_ += _init_result_list(observations=["an observation"])
         >>> _history_to_kind(history_) # doctest: +NORMALIZE_WHITESPACE +ELLIPSIS
         Snapshot(..., params={'some': 'params'}, conditions=['a condition'],
                         observations=['an observation'], ...)
 
         >>> from sklearn.linear_model import LinearRegression
-        >>> history_ = [Result(LinearRegression(), kind=ResultKind.THEORY)]
+        >>> history_ = [Result(LinearRegression(), kind=ResultKind.MODEL)]
         >>> _history_to_kind(history_) # doctest: +ELLIPSIS
-        Snapshot(..., theories=[LinearRegression()])
+        Snapshot(..., models=[LinearRegression()])
 
         >>> from autora.variable import VariableCollection, IV
-        >>> metadata = VariableCollection(independent_variables=[IV(name="example")])
-        >>> history_ = [Result(metadata, kind=ResultKind.METADATA)]
+        >>> variables = VariableCollection(independent_variables=[IV(name="example")])
+        >>> history_ = [Result(variables, kind=ResultKind.VARIABLES)]
         >>> _history_to_kind(history_) # doctest: +ELLIPSIS
-        Snapshot(metadata=VariableCollection(independent_variables=[IV(name='example', ...
+        Snapshot(variables=VariableCollection(independent_variables=[IV(name='example', ...
 
         >>> history_ = [Result({'some': 'params'}, kind=ResultKind.PARAMS)]
         >>> _history_to_kind(history_) # doctest: +ELLIPSIS
         Snapshot(..., params={'some': 'params'}, ...)
 
     """
     namespace = Snapshot(
-        metadata=_get_last_data_with_default(
-            history, kind={ResultKind.METADATA}, default=VariableCollection()
+        variables=_get_last_data_with_default(
+            history, kind={ResultKind.VARIABLES}, default=VariableCollection()
         ),
         params=_get_last_data_with_default(
             history, kind={ResultKind.PARAMS}, default={}
         ),
         observations=_list_data(
             _filter_history(history, kind={ResultKind.OBSERVATION})
         ),
-        theories=_list_data(_filter_history(history, kind={ResultKind.THEORY})),
+        models=_list_data(_filter_history(history, kind={ResultKind.MODEL})),
         conditions=_list_data(_filter_history(history, kind={ResultKind.CONDITION})),
     )
     return namespace
 
 
 def _list_data(data: Sequence[SupportsDataKind]):
     """
```

### Comparing `autora-workflow-0.1.0/src/autora/workflow/state/param.py` & `autora-workflow-0.2.0/src/autora/workflow/state/param.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from __future__ import annotations
 
 import copy
 import logging
 from typing import Dict, Mapping
 
 import numpy as np
-
 from autora.utils.dictionary import LazyDict
 
 from ..protocol import SupportsControllerState
 
 _logger = logging.getLogger(__name__)
 
 
@@ -18,42 +17,42 @@
     """
     Examples:
         Even with an empty data object, we can initialize the dictionary,
         >>> from autora.workflow.state import Snapshot
         >>> state_dependent_properties = _get_state_dependent_properties(Snapshot())
 
         ... but it will raise an exception if a value isn't yet available when we try to use it
-        >>> state_dependent_properties["%theories[-1]%"] # doctest: +ELLIPSIS
+        >>> state_dependent_properties["%models[-1]%"] # doctest: +ELLIPSIS
         Traceback (most recent call last):
         ...
         IndexError: list index out of range
 
         Nevertheless, we can iterate through its keys no problem:
         >>> [key for key in state_dependent_properties.keys()] # doctest: +NORMALIZE_WHITESPACE
         ['%observations.ivs[-1]%', '%observations.dvs[-1]%', '%observations.ivs%',
-        '%observations.dvs%', '%theories[-1]%', '%theories%']
+        '%observations.dvs%', '%models[-1]%', '%models%']
 
     """
 
-    n_ivs = len(state.metadata.independent_variables)
-    n_dvs = len(state.metadata.dependent_variables)
+    n_ivs = len(state.variables.independent_variables)
+    n_dvs = len(state.variables.dependent_variables)
     state_dependent_property_dict = LazyDict(
         {
             "%observations.ivs[-1]%": lambda: np.array(state.observations[-1])[
                 :, 0:n_ivs
             ],
             "%observations.dvs[-1]%": lambda: np.array(state.observations[-1])[
                 :, n_ivs:
             ],
             "%observations.ivs%": lambda: np.row_stack(
                 [np.empty([0, n_ivs + n_dvs])] + list(state.observations)
             )[:, 0:n_ivs],
             "%observations.dvs%": lambda: np.row_stack(state.observations)[:, n_ivs:],
-            "%theories[-1]%": lambda: state.theories[-1],
-            "%theories%": lambda: state.theories,
+            "%models[-1]%": lambda: state.models[-1],
+            "%models%": lambda: state.models,
         }
     )
     return state_dependent_property_dict
 
 
 def _resolve_properties(params: Dict, state_dependent_properties: Mapping):
     """
@@ -103,16 +102,16 @@
 
 def resolve_state_params(params: Dict, state: SupportsControllerState) -> Dict:
     """
     Returns the `params` attribute of the input, with `cycle properties` resolved.
 
     Examples:
         >>> from autora.workflow.state import History
-        >>> params = {"experimentalist": {"source": "%theories[-1]%"}}
-        >>> s = History(theories=["the first theory", "the second theory"])
+        >>> params = {"experimentalist": {"source": "%models[-1]%"}}
+        >>> s = History(models=["the first model", "the second model"])
         >>> resolve_state_params(params, s)
-        {'experimentalist': {'source': 'the second theory'}}
+        {'experimentalist': {'source': 'the second model'}}
 
     """
     state_dependent_properties = _get_state_dependent_properties(state)
     resolved_params = _resolve_properties(params, state_dependent_properties)
     return resolved_params
```

### Comparing `autora-workflow-0.1.0/src/autora/workflow/state/snapshot.py` & `autora-workflow-0.2.0/src/autora/workflow/state/snapshot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 """ Classes for storing and passing a cycle's state as an immutable snapshot. """
 from dataclasses import dataclass, field
 from typing import Dict, List
 
+from autora.variable import VariableCollection
 from numpy.typing import ArrayLike
 from sklearn.base import BaseEstimator
 
-from autora.variable import VariableCollection
-
 from ..protocol import SupportsControllerStateFields
 
 
 @dataclass(frozen=True)
 class Snapshot(SupportsControllerStateFields):
     """An object passed between and updated by processing steps in the Controller."""
 
     # Single values
-    metadata: VariableCollection = field(default_factory=VariableCollection)
+    variables: VariableCollection = field(default_factory=VariableCollection)
     params: Dict = field(default_factory=dict)
 
     # Sequences
     conditions: List[ArrayLike] = field(default_factory=list)
     observations: List[ArrayLike] = field(default_factory=list)
-    theories: List[BaseEstimator] = field(default_factory=list)
+    models: List[BaseEstimator] = field(default_factory=list)
 
     def update(
         self,
-        metadata=None,
+        variables=None,
         params=None,
         conditions=None,
         observations=None,
-        theories=None,
+        models=None,
     ):
         """
         Create a new object with updated values.
 
         The initial object is empty:
         >>> s0 = Snapshot()
         >>> s0  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
-        Snapshot(metadata=VariableCollection(...), params={}, conditions=[],
-                        observations=[], theories=[])
+        Snapshot(variables=VariableCollection(...), params={}, conditions=[],
+                        observations=[], models=[])
 
         We can update the params using the `.update` method:
         >>> s0.update(params={'first': 'params'})  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
         Snapshot(..., params={'first': 'params'}, ...)
 
         ... but the original object is unchanged:
         >>> s0  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
         Snapshot(..., params={}, ...)
 
         For params, only one object is returned from the respective property:
         >>> s0.update(params={'first': 'params'}).update(params={'second': 'params'}).params
         {'second': 'params'}
 
-        ... and the same applies to metadata:
+        ... and the same applies to variables:
         >>> from autora.variable import VariableCollection, IV
-        >>> (s0.update(metadata=VariableCollection([IV("1st IV")]))
-        ...    .update(metadata=VariableCollection([IV("2nd IV")]))).metadata
+        >>> (s0.update(variables=VariableCollection([IV("1st IV")]))
+        ...    .update(variables=VariableCollection([IV("2nd IV")]))).variables
         VariableCollection(independent_variables=[IV(name='2nd IV',...)], ...)
 
-        When we update the conditions, observations or theories, the respective list is extended:
-        >>> s3 = s0.update(theories=["1st theory"])
+        When we update the conditions, observations or models, the respective list is extended:
+        >>> s3 = s0.update(models=["1st model"])
         >>> s3
-        Snapshot(..., theories=['1st theory'])
+        Snapshot(..., models=['1st model'])
 
-        ... so we can see the history of all the theories, for instance.
-        >>> s3.update(theories=["2nd theory"])
-        Snapshot(..., theories=['1st theory', '2nd theory'])
+        ... so we can see the history of all the models, for instance.
+        >>> s3.update(models=["2nd model"])
+        Snapshot(..., models=['1st model', '2nd model'])
 
         The same applies to observations:
         >>> s4 = s0.update(observations=["1st observation"])
         >>> s4
         Snapshot(..., observations=['1st observation'], ...)
 
         >>> s4.update(observations=["2nd observation"])  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
@@ -80,31 +79,31 @@
         >>> s5 = s0.update(conditions=["1st condition"])
         >>> s5
         Snapshot(..., conditions=['1st condition'], ...)
 
         >>> s5.update(conditions=["2nd condition"])  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
         Snapshot(..., conditions=['1st condition', '2nd condition'], ...)
 
-        You can also update with multiple conditions, observations and theories:
+        You can also update with multiple conditions, observations and models:
         >>> s0.update(conditions=['c1', 'c2'])
         Snapshot(..., conditions=['c1', 'c2'], ...)
 
-        >>> s0.update(theories=['t1', 't2'], metadata={'m': 1})
-        Snapshot(metadata={'m': 1}, ..., theories=['t1', 't2'])
+        >>> s0.update(models=['m1', 'm2'], variables={'m': 1})
+        Snapshot(variables={'m': 1}, ..., models=['m1', 'm2'])
 
-        >>> s0.update(theories=['t1'], observations=['o1'], metadata={'m': 1})
-        Snapshot(metadata={'m': 1}, ..., observations=['o1'], theories=['t1'])
+        >>> s0.update(models=['m1'], observations=['o1'], variables={'m': 1})
+        Snapshot(variables={'m': 1}, ..., observations=['o1'], models=['m1'])
 
 
-        Inputs to theories, observations and conditions must be Lists
+        Inputs to models, observations and conditions must be Lists
         which can be cast to lists:
-        >>> s0.update(theories='t1')  # doctest: +ELLIPSIS
+        >>> s0.update(models='m1')  # doctest: +ELLIPSIS
         Traceback (most recent call last):
         ...
-        AssertionError: 't1' must be a list, e.g. `['t1']`?)
+        AssertionError: 'm1' must be a list, e.g. `['m1']`?)
 
         """
 
         def _coalesce_lists(old, new):
             assert isinstance(
                 old, List
             ), f"{repr(old)} must be a list, e.g. `[{repr(old)}]`?)"
@@ -112,13 +111,13 @@
                 assert isinstance(
                     new, List
                 ), f"{repr(new)} must be a list, e.g. `[{repr(new)}]`?)"
                 return old + list(new)
             else:
                 return old
 
-        metadata_ = metadata or self.metadata
+        variables_ = variables or self.variables
         params_ = params or self.params
         conditions_ = _coalesce_lists(self.conditions, conditions)
         observations_ = _coalesce_lists(self.observations, observations)
-        theories_ = _coalesce_lists(self.theories, theories)
-        return Snapshot(metadata_, params_, conditions_, observations_, theories_)
+        models_ = _coalesce_lists(self.models, models)
+        return Snapshot(variables_, params_, conditions_, observations_, models_)
```

### Comparing `autora-workflow-0.1.0/src/autora_workflow.egg-info/PKG-INFO` & `autora-workflow-0.2.0/src/autora_workflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-workflow
-Version: 0.1.0
+Version: 0.2.0
 Summary: Workflow tools for the Autonomous Research Assistant (AutoRA) package.
 Author-email: John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
 Project-URL: homepage, https://www.empiricalresearch.ai/
 Project-URL: repository, https://github.com/AutoResearch/autora-workflow
 Project-URL: documentation, https://hollandjg.github.io/autora-workflow/
 Description-Content-Type: text/markdown
```

### Comparing `autora-workflow-0.1.0/src/autora_workflow.egg-info/SOURCES.txt` & `autora-workflow-0.2.0/src/autora_workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.1.0/tests/test_controller_plots.py` & `autora-workflow-0.2.0/tests/test_controller_plots.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import random
 
 import numpy as np
 import pytest
-from sklearn.linear_model import LinearRegression
-from sklearn.metrics import r2_score
-
 from autora.experimentalist.pipeline import Pipeline
 from autora.experimentalist.pooler.grid import grid_pool
 from autora.experimentalist.sampler.random_sampler import random_sampler
 from autora.variable import Variable, VariableCollection
+from sklearn.linear_model import LinearRegression
+from sklearn.metrics import r2_score
+
 from autora.workflow import Cycle
 from autora.workflow.plotting import (
     _check_replace_default_kw,
     cycle_default_score,
     cycle_specified_score,
     plot_cycle_score,
     plot_results_panel_2d,
@@ -29,15 +29,15 @@
 
 
 @pytest.fixture
 def state_lr(ground_truth_1x):
     random.seed(1)
 
     # Variable Metadata
-    study_metadata = VariableCollection(
+    study_variables = VariableCollection(
         independent_variables=[
             Variable(name="x1", allowed_values=np.linspace(0, 1, 100))
         ],
         dependent_variables=[Variable(name="y", value_range=(-20, 20))],
     )
 
     # Theorist
@@ -47,15 +47,15 @@
     example_experimentalist = Pipeline(
         [
             ("pool", grid_pool),
             ("sampler", random_sampler),
             ("transform", lambda x: [s[0] for s in x]),
         ],
         params={
-            "pool": {"ivs": study_metadata.independent_variables},
+            "pool": {"ivs": study_variables.independent_variables},
             "sampler": {"n": 5},
         },
     )
 
     # Experiment Runner
     def get_example_synthetic_experiment_runner():
         rng = np.random.default_rng(seed=180)
@@ -65,15 +65,15 @@
 
         return runner
 
     example_synthetic_experiment_runner = get_example_synthetic_experiment_runner()
 
     # Initialize Cycle
     cycle = Cycle(
-        metadata=study_metadata,
+        variables=study_variables,
         theorist=lm,
         experimentalist=example_experimentalist,
         experiment_runner=example_synthetic_experiment_runner,
     )
 
     # Run 10 iterations
     cycle.run(10)
@@ -93,15 +93,15 @@
 def cycle_multi_lr(ground_truth_2x):
     random.seed(1)
 
     # def ground_truth(X):
     #     return X[:, 0] + (0.5 * X[:, 1]) + 1.0
 
     # Variable Metadata
-    study_metadata = VariableCollection(
+    study_variables = VariableCollection(
         independent_variables=[
             Variable(name="x1", allowed_values=np.linspace(0, 1, 10)),
             Variable(name="x2", allowed_values=np.linspace(0, 1, 10)),
         ],
         dependent_variables=[Variable(name="y", value_range=(-20, 20))],
     )
 
@@ -112,15 +112,15 @@
     example_experimentalist = Pipeline(
         [
             ("pool", grid_pool),
             ("sampler", random_sampler),
             ("transform", lambda x: np.array(x)),
         ],
         params={
-            "pool": {"ivs": study_metadata.independent_variables},
+            "pool": {"ivs": study_variables.independent_variables},
             "sampler": {"n": 10},
         },
     )
 
     # Experiment Runner
     def get_example_synthetic_experiment_runner():
         rng = np.random.default_rng(seed=180)
@@ -130,15 +130,15 @@
 
         return runner
 
     example_synthetic_experiment_runner = get_example_synthetic_experiment_runner()
 
     # Initialize Cycle
     cycle = Cycle(
-        metadata=study_metadata,
+        variables=study_variables,
         theorist=lm,
         experimentalist=example_experimentalist,
         experiment_runner=example_synthetic_experiment_runner,
     )
 
     # Run 6 iterations
     cycle.run(6)
@@ -211,15 +211,15 @@
                 [35, 5],
                 [40, 5],
                 [45, 5],
             ]
         ),
     )
 
-    # Test theory line is being plotted
+    # Test model line is being plotted
     for axes in fig.axes[:-2]:
         assert len(axes.lines[0].get_xdata()) == steps
         assert len(axes.lines[0].get_ydata()) == steps
 
 
 def test_3d_plot(state_multi_lr):
     """
@@ -258,15 +258,15 @@
     )
 
 
 def test_score_functions(state_lr, ground_truth_1x):
     """
     Tests the scoring functions cycle_default_score and cycle_specified_score.
     """
-    X_test = state_lr.metadata.independent_variables[0].allowed_values.reshape(-1, 1)
+    X_test = state_lr.variables.independent_variables[0].allowed_values.reshape(-1, 1)
     y_test = ground_truth_1x(X_test)
 
     scores_default = cycle_default_score(state_lr, X_test, y_test)
     scores_specified = cycle_specified_score(r2_score, state_lr, X_test, y_test)
 
     # Check scores are the expected values
     score_values = [
@@ -288,15 +288,15 @@
     assert np.array_equal(scores_default, scores_specified)
 
 
 def test_cycle_score_plot(state_lr, ground_truth_1x):
     """
     Tests plotting functionality of test_cycle_score_plot with a 2D linear regression.
     """
-    X_test = state_lr.metadata.independent_variables[0].allowed_values.reshape(-1, 1)
+    X_test = state_lr.variables.independent_variables[0].allowed_values.reshape(-1, 1)
     y_test = ground_truth_1x(X_test)
     fig = plot_cycle_score(state_lr, X_test, y_test)
 
     # Should have 1 axis
     assert len(fig.axes) == 1
 
     # Test line is plotted correctly
@@ -322,15 +322,15 @@
 
 def test_cycle_score_plot_multi_lr(cycle_multi_lr, ground_truth_2x):
     """
     Tests plotting functionality of test_cycle_score_plot with multiple linear regression cycle.
     """
     cycle_multi_lr.run(6)  # Run additional 6 times, total of 12 cycles
     X_test = np.array(
-        list(grid_pool(cycle_multi_lr.state.metadata.independent_variables))
+        list(grid_pool(cycle_multi_lr.state.variables.independent_variables))
     )
     y_test = ground_truth_2x(X_test)
     fig = plot_cycle_score(cycle_multi_lr.state, X_test, y_test)
 
     # Test line is plotted correctly
     axis = fig.axes[0]
     assert len(axis.lines[0].get_xdata()) == 12
```


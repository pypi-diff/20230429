# Comparing `tmp/autora-3.0.0a0.tar.gz` & `tmp/autora-3.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-3.0.0a0.tar", max compression
+gzip compressed data, was "autora-3.0.0a2.tar", last modified: Thu Apr 27 23:34:22 2023, max compression
```

## Comparing `autora-3.0.0a0.tar` & `autora-3.0.0a2.tar`

### file list

```diff
@@ -1,62 +1,67 @@
--rw-r--r--   0        0        0     1100 2023-04-14 15:50:00.492529 autora-3.0.0a0/LICENSE.md
--rw-r--r--   0        0        0    18722 2023-04-14 15:50:00.492529 autora-3.0.0a0/README.md
--rw-r--r--   0        0        0      173 2023-04-14 15:50:00.492529 autora-3.0.0a0/autora/__init__.py
--rw-r--r--   0        0        0      197 2023-04-14 15:50:00.492529 autora-3.0.0a0/autora/cycle/__init__.py
--rw-r--r--   0        0        0    20784 2023-04-14 15:50:00.492529 autora-3.0.0a0/autora/cycle/plot_utils.py
--rw-r--r--   0        0        0    21619 2023-04-14 15:50:00.492529 autora-3.0.0a0/autora/cycle/simple.py
--rw-r--r--   0        0        0        0 2023-04-14 15:50:00.492529 autora-3.0.0a0/autora/experimentalist/__init__.py
--rw-r--r--   0        0        0     5014 2023-04-14 15:50:00.492529 autora-3.0.0a0/autora/experimentalist/filter.py
--rw-r--r--   0        0        0    18310 2023-04-14 15:50:00.492529 autora-3.0.0a0/autora/experimentalist/pipeline.py
--rw-r--r--   0        0        0       87 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/pooler/__init__.py
--rw-r--r--   0        0        0     1800 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/pooler/general_pool.py
--rw-r--r--   0        0        0    13496 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/pooler/poppernet.py
--rw-r--r--   0        0        0      232 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/sampler/__init__.py
--rw-r--r--   0        0        0     2383 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/sampler/assumption.py
--rw-r--r--   0        0        0     2841 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/sampler/dissimilarity.py
--rw-r--r--   0        0        0     2216 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/sampler/model_disagreement.py
--rw-r--r--   0        0        0     1666 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/sampler/nearest_value.py
--rw-r--r--   0        0        0      497 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/sampler/random.py
--rw-r--r--   0        0        0     2052 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/sampler/uncertainty.py
--rw-r--r--   0        0        0     4586 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/experimentalist/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/skl/__init__.py
--rw-r--r--   0        0        0     6087 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/skl/bms.py
--rw-r--r--   0        0        0    12781 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/skl/bsr.py
--rw-r--r--   0        0        0    31115 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/skl/darts.py
--rw-r--r--   0        0        0     2649 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/synthetic/__init__.py
--rw-r--r--   0        0        0       97 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/synthetic/data/__init__.py
--rw-r--r--   0        0        0     5123 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/synthetic/data/expected_value.py
--rw-r--r--   0        0        0     6631 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/synthetic/data/prospect_theory.py
--rw-r--r--   0        0        0     4587 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/synthetic/data/weber_fechner.py
--rw-r--r--   0        0        0     7338 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/synthetic/inventory.py
--rw-r--r--   0        0        0        0 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/__init__.py
--rw-r--r--   0        0        0      126 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bms/__init__.py
--rw-r--r--   0        0        0      164 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bms/data/named_equations.wiki.parsed__num_operations.dat
--rw-r--r--   0        0        0      130 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bms/data/named_equations.wiki.parsed__operation_type.dat
--rw-r--r--   0        0        0      133 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bms/data/named_equations.wiki.parsed__operation_type_sq.dat
--rw-r--r--   0        0        0     8599 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bms/fit_prior.py
--rw-r--r--   0        0        0    60372 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bms/mcmc.py
--rw-r--r--   0        0        0     5726 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bms/parallel.py
--rw-r--r--   0        0        0     2341 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bms/prior.py
--rwxr-xr-x   0        0        0     2860 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bms/utils.py
--rw-r--r--   0        0        0        0 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bsr/__init__.py
--rw-r--r--   0        0        0    32217 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bsr/funcs.py
--rw-r--r--   0        0        0     1430 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bsr/misc.py
--rw-r--r--   0        0        0     6521 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bsr/node.py
--rw-r--r--   0        0        0     2117 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bsr/operation.py
--rw-r--r--   0        0        0     5114 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/bsr/prior.py
--rw-r--r--   0        0        0      347 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/darts/__init__.py
--rwxr-xr-x   0        0        0    12774 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/darts/architect.py
--rw-r--r--   0        0        0     1791 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/darts/dataset.py
--rw-r--r--   0        0        0     1301 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/darts/fan_out.py
--rwxr-xr-x   0        0        0    30660 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/darts/model_search.py
--rwxr-xr-x   0        0        0    19820 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/darts/operations.py
--rwxr-xr-x   0        0        0    41286 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/darts/plot_utils.py
--rwxr-xr-x   0        0        0    13517 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/darts/utils.py
--rwxr-xr-x   0        0        0     6645 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/theorist/darts/visualize.py
--rw-r--r--   0        0        0       25 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/utils/__init__.py
--rw-r--r--   0        0        0      441 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/utils/dictionary.py
--rw-r--r--   0        0        0     1866 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/variable/__init__.py
--rw-r--r--   0        0        0     2511 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/variable/time.py
--rw-r--r--   0        0        0     8899 2023-04-14 15:50:00.496529 autora-3.0.0a0/autora/variable/tinkerforge.py
--rw-r--r--   0        0        0     1812 2023-04-14 15:52:10.495893 autora-3.0.0a0/pyproject.toml
--rw-r--r--   0        0        0    20200 1970-01-01 00:00:00.000000 autora-3.0.0a0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.132985 autora-3.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-27 23:34:04.000000 autora-3.0.0a2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.120985 autora-3.0.0a2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-27 23:34:04.000000 autora-3.0.0a2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-27 23:34:04.000000 autora-3.0.0a2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.124985 autora-3.0.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-27 23:34:04.000000 autora-3.0.0a2/.github/workflows/publish-documentation-gh-pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-27 23:34:04.000000 autora-3.0.0a2/.github/workflows/publish-package-anaconda-org.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-27 23:34:04.000000 autora-3.0.0a2/.github/workflows/publish-package-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 23:34:04.000000 autora-3.0.0a2/.github/workflows/test-conda-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-27 23:34:04.000000 autora-3.0.0a2/.github/workflows/test-poetry-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-27 23:34:04.000000 autora-3.0.0a2/.github/workflows/test-pre-commit-hooks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-27 23:34:04.000000 autora-3.0.0a2/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-27 23:34:04.000000 autora-3.0.0a2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.128985 autora-3.0.0a2/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-27 23:34:04.000000 autora-3.0.0a2/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-27 23:34:04.000000 autora-3.0.0a2/.idea/autora.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.128985 autora-3.0.0a2/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-27 23:34:04.000000 autora-3.0.0a2/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 23:34:04.000000 autora-3.0.0a2/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.128985 autora-3.0.0a2/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-27 23:34:04.000000 autora-3.0.0a2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-27 23:34:04.000000 autora-3.0.0a2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-27 23:34:04.000000 autora-3.0.0a2/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-27 23:34:04.000000 autora-3.0.0a2/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-27 23:34:04.000000 autora-3.0.0a2/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-27 23:34:04.000000 autora-3.0.0a2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.128985 autora-3.0.0a2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:04.000000 autora-3.0.0a2/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 23:34:04.000000 autora-3.0.0a2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 23:34:04.000000 autora-3.0.0a2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-27 23:34:04.000000 autora-3.0.0a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    21370 2023-04-27 23:34:22.132985 autora-3.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19356 2023-04-27 23:34:04.000000 autora-3.0.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.116985 autora-3.0.0a2/conda/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.128985 autora-3.0.0a2/conda/autora/
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-27 23:34:04.000000 autora-3.0.0a2/conda/autora/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-27 23:34:04.000000 autora-3.0.0a2/conda/autora/run_test.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.128985 autora-3.0.0a2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.128985 autora-3.0.0a2/docs/experiment-runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:04.000000 autora-3.0.0a2/docs/experiment-runner/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.128985 autora-3.0.0a2/docs/experimentalists/
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-27 23:34:04.000000 autora-3.0.0a2/docs/experimentalists/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.128985 autora-3.0.0a2/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    31814 2023-04-27 23:34:04.000000 autora-3.0.0a2/docs/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   389908 2023-04-27 23:34:04.000000 autora-3.0.0a2/docs/img/overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-27 23:34:04.000000 autora-3.0.0a2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.128985 autora-3.0.0a2/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-27 23:34:04.000000 autora-3.0.0a2/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.128985 autora-3.0.0a2/docs/theorist/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-27 23:34:04.000000 autora-3.0.0a2/docs/theorist/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.128985 autora-3.0.0a2/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-27 23:34:04.000000 autora-3.0.0a2/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 23:34:04.000000 autora-3.0.0a2/mkdocs/gen_ref_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.128985 autora-3.0.0a2/mkdocs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-27 23:34:04.000000 autora-3.0.0a2/mkdocs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-27 23:34:04.000000 autora-3.0.0a2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-27 23:34:04.000000 autora-3.0.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 23:34:22.132985 autora-3.0.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.132985 autora-3.0.0a2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-27 23:34:04.000000 autora-3.0.0a2/src/.keep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:34:22.132985 autora-3.0.0a2/src/autora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21370 2023-04-27 23:34:22.000000 autora-3.0.0a2/src/autora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-27 23:34:22.000000 autora-3.0.0a2/src/autora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:34:22.000000 autora-3.0.0a2/src/autora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-27 23:34:22.000000 autora-3.0.0a2/src/autora.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:34:22.000000 autora-3.0.0a2/src/autora.egg-info/top_level.txt
```

### Comparing `autora-3.0.0a0/LICENSE.md` & `autora-3.0.0a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a0/README.md` & `autora-3.0.0a2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -418,7 +418,43 @@
     v1.3.0 and fixes a bugfix number v1.2.4. If necessary, modify the version number you've chosen to be consistent 
     with the content of the release.
   - Select whether this is a pre-release or a new "latest" release. It's a "pre-release" if there's an alpha, 
     beta, or release candidate number in the tag name, otherwise it's a new "latest" release.
   - Click on "Publish release"
 - GitHub actions will run to create and publish the PyPI and Anaconda packages, and publish the documentation. Check in 
   GitHub actions whether they run without errors and fix any errors which occur.
+
+
+# How to Develop
+
+Install this in an environment using your chosen package manager. 
+
+## Using `virtualenv`
+
+Install:
+- python: https://www.python.org/downloads/
+- virtualenv: https://virtualenv.pypa.io/en/latest/installation.html
+
+Create a new virtual environment:
+```shell
+virtualenv venv
+```
+
+Activate it:
+```shell
+source venv/bin/activate
+```
+
+Use `pip install` to install the current project (`"."`) in editable mode (`-e`) with dev-dependencies (`[dev]`):
+```shell
+pip install -e ".[dev]"
+```
+
+Build the package using:
+```shell
+python -m build
+```
+
+Publish the package to PyPI using `twine`:
+```shell
+twine upload dist/* 
+```
```

### Comparing `autora-3.0.0a0/PKG-INFO` & `autora-3.0.0a2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 Metadata-Version: 2.1
 Name: autora
-Version: 3.0.0a0
-Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process. This framework implements tools for autonomously and iteratively generating 1) new theories to describe real-world data, and 2) experiments to invalidate those theories and seed a new cycle of theory-making. The experiments will be run online via crowd-sourcing platforms (MTurk, Prolific).
-Home-page: https://musslick.github.io/AER_website/Research.html
-Author: Sebastian Musslick
-Author-email: sebastian_musslick@brown.edu
-Requires-Python: >=3.8.10,<3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Provides-Extra: tinkerforge
-Requires-Dist: graphviz (>=0.14.1,<0.21.0)
-Requires-Dist: imageio (>=2.9.0,<3.0.0)
-Requires-Dist: matplotlib (>=3.2.1,<4.0.0)
-Requires-Dist: numpy (>=1.22.1)
-Requires-Dist: pandas (>=1.4.2,<3.0.0)
-Requires-Dist: scikit-learn (>=1.1.1,<2.0.0)
-Requires-Dist: scipy (>=1.9.3,<2.0.0)
-Requires-Dist: seaborn (>=0.11.1,<0.13.0)
-Requires-Dist: sympy (>=1.10.1,<2.0.0)
-Requires-Dist: tinkerforge (>=2.1.25,<3.0.0) ; extra == "tinkerforge"
-Requires-Dist: torch (==2.0.0)
-Requires-Dist: tqdm (>=4.64.0,<5.0.0)
-Project-URL: Documentation, https://autoresearch.github.io/autora/
-Project-URL: Repository, https://github.com/AutoResearch/autora
+Version: 3.0.0a2
+Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process.
+Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
+License: Copyright 2021, Brown University, Providence, RI.
+        
+                                All Rights Reserved
+        
+        Permission to use, copy, modify, and distribute this software and
+        its documentation for any purpose other than its incorporation into a
+        commercial product or service is hereby granted without fee, provided
+        that the above copyright notice appear in all copies and that both
+        that copyright notice and this permission notice appear in supporting
+        documentation, and that the name of Brown University not be used in
+        advertising or publicity pertaining to distribution of the software
+        without specific, written prior permission.
+        
+        BROWN UNIVERSITY DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE,
+        INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR ANY
+        PARTICULAR PURPOSE.  IN NO EVENT SHALL BROWN UNIVERSITY BE LIABLE FOR
+        ANY SPECIAL, INDIRECT OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
+        WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
+        ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
+        OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
+Project-URL: homepage, https://www.empiricalresearch.ai/
+Project-URL: repository, https://github.com/AutoResearch/autora
+Project-URL: documentation, https://autoresearch.github.io/autora/
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: all
+Provides-Extra: all-theorists
+Provides-Extra: theorist-darts
+Provides-Extra: all-experimentalists
+Provides-Extra: all-experiment-runners
+Provides-Extra: synthetic-experiments
+License-File: LICENSE.md
 
 # Automated Research Assistant
 Automated Research Assistant (AutoRA) is an open source AI-based system for automating each aspect of empirical research in the behavioral sciences, from the construction of a scientific hypothesis to conducting novel experiments. The documentation is here: [https://autoresearch.github.io/autora/](https://autoresearch.github.io/autora/)
 
 # Getting started
 
 You should be familiar with the command line for your operating system. The topics required are covered in:
@@ -447,7 +457,42 @@
     with the content of the release.
   - Select whether this is a pre-release or a new "latest" release. It's a "pre-release" if there's an alpha, 
     beta, or release candidate number in the tag name, otherwise it's a new "latest" release.
   - Click on "Publish release"
 - GitHub actions will run to create and publish the PyPI and Anaconda packages, and publish the documentation. Check in 
   GitHub actions whether they run without errors and fix any errors which occur.
 
+
+# How to Develop
+
+Install this in an environment using your chosen package manager. 
+
+## Using `virtualenv`
+
+Install:
+- python: https://www.python.org/downloads/
+- virtualenv: https://virtualenv.pypa.io/en/latest/installation.html
+
+Create a new virtual environment:
+```shell
+virtualenv venv
+```
+
+Activate it:
+```shell
+source venv/bin/activate
+```
+
+Use `pip install` to install the current project (`"."`) in editable mode (`-e`) with dev-dependencies (`[dev]`):
+```shell
+pip install -e ".[dev]"
+```
+
+Build the package using:
+```shell
+python -m build
+```
+
+Publish the package to PyPI using `twine`:
+```shell
+twine upload dist/* 
+```
```


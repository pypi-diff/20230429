# Comparing `tmp/bump_deps_index-1.4.0.tar.gz` & `tmp/bump_deps_index-1.4.1.tar.gz`

## Comparing `bump_deps_index-1.4.0.tar` & `bump_deps_index-1.4.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/.readthedocs.yml
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/tox.ini
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/whitelist.txt
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/.github/workflows/check.yml
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/docs/changelog.rst
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/docs/cli.rst
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/docs/conf.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/docs/index.rst
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/docs/py_api.rst
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/src/bump_deps_index/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/src/bump_deps_index/__main__.py
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/src/bump_deps_index/_cli.py
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/src/bump_deps_index/_run.py
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/src/bump_deps_index/_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/src/bump_deps_index/py.typed
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/src/bump_deps_index/version.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/tests/test_cli.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/tests/test_main.py
--rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/tests/test_run.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/tests/test_spec.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/tests/test_version.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/LICENSE
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/README.md
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 bump_deps_index-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/.readthedocs.yml
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/tox.ini
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/whitelist.txt
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/.github/workflows/check.yml
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/docs/changelog.rst
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/docs/cli.rst
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/docs/conf.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/docs/index.rst
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/docs/py_api.rst
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/src/bump_deps_index/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/src/bump_deps_index/__main__.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/src/bump_deps_index/_cli.py
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/src/bump_deps_index/_run.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/src/bump_deps_index/_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/src/bump_deps_index/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/src/bump_deps_index/version.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/tests/test_cli.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/tests/test_main.py
+-rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/tests/test_run.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/tests/test_spec.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/tests/test_version.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/LICENSE
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/README.md
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 bump_deps_index-1.4.1/PKG-INFO
```

### Comparing `bump_deps_index-1.4.0/.pre-commit-config.yaml` & `bump_deps_index-1.4.1/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,65 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: check-ast
       - id: check-builtin-literals
       - id: check-docstring-first
       - id: check-merge-conflict
       - id: check-yaml
       - id: check-toml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.2.2
+    rev: v3.3.2
     hooks:
       - id: pyupgrade
         args: ["--py310-plus"]
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
       - id: black
         args: [--safe]
   - repo: https://github.com/asottile/blacken-docs
-    rev: v1.12.1
+    rev: 1.13.0
     hooks:
       - id: blacken-docs
-        additional_dependencies: [black==22.10]
+        additional_dependencies: [black==23.3]
   - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: rst-backticks
   - repo: https://github.com/tox-dev/tox-ini-fmt
-    rev: "0.5.2"
+    rev: "1.3.0"
     hooks:
       - id: tox-ini-fmt
         args: ["-p", "fix"]
   - repo: https://github.com/PyCQA/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies:
-          - flake8-bugbear==22.10.27
-          - flake8-comprehensions==3.10.1
-          - flake8-pytest-style==1.6
+          - flake8-bugbear==23.3.23
+          - flake8-comprehensions==3.12
+          - flake8-pytest-style==1.7.2
           - flake8-spellcheck==0.28
-          - flake8-unused-arguments==0.0.12
-          - flake8-noqa==1.3
-          - pep8-naming==0.13.2
+          - flake8-unused-arguments==0.0.13
+          - flake8-noqa==1.3.1
+          - pep8-naming==0.13.3
+          - flake8-pyproject==1.2.3
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.4"
+    rev: "v2.7.1"
     hooks:
       - id: prettier
         additional_dependencies:
-          - "prettier@3.0.0-alpha.4"
+          - "prettier@2.7.1"
           - "@prettier/plugin-xml@2.2"
+  - repo: https://github.com/tox-dev/pyproject-fmt
+    rev: "0.11.1"
+    hooks:
+      - id: pyproject-fmt
```

### Comparing `bump_deps_index-1.4.0/tox.ini` & `bump_deps_index-1.4.1/tox.ini`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,77 @@
 [tox]
-envlist =
+requires =
+    tox>=4.2
+env_list =
     fix
+    py312
     py311
     py310
     docs
     type
     readme
-isolated_build = true
 skip_missing_interpreters = true
-minversion = 3.21
 
 [testenv]
 description = run the unit tests with pytest under {basepython}
-setenv =
-    COVERAGE_FILE = {env:COVERAGE_FILE:{toxworkdir}{/}.coverage.{envname}}
+package = wheel
+wheel_build_env = .pkg
 extras =
     test
+set_env =
+    COVERAGE_FILE = {env:COVERAGE_FILE:{toxworkdir}{/}.coverage.{envname}}
 commands =
     pytest {tty:--color=yes} {posargs: \
       --cov {envsitepackagesdir}{/}bump_deps_index --cov {toxinidir}{/}tests --cov-config=pyproject.toml \
       --junitxml {toxworkdir}{/}junit.{envname}.xml  --no-cov-on-fail --cov-report term-missing:skip-covered \
       --cov-report html:{envtmpdir}{/}htmlcov --cov-report xml:{toxworkdir}{/}coverage.{envname}.xml \
       tests}
-package = wheel
-wheel_build_env = .pkg
 
 [testenv:fix]
 description = run static analysis and style check using flake8
-passenv =
-    HOMEPATH
-    PROGRAMDATA
 skip_install = true
 deps =
-    pre-commit>=2.20
+    pre-commit>=3.2.2
+pass_env =
+    HOMEPATH
+    PROGRAMDATA
 commands =
     pre-commit run --all-files --show-diff-on-failure
 
 [testenv:docs]
 extras =
     docs
 commands =
     python -c 'import glob; import subprocess; subprocess.call(["proselint"] + glob.glob("docs/*.rst"))'
     sphinx-build -d "{envtmpdir}/doctree" docs "{toxworkdir}/docs_out" --color -b html {posargs}
     python -c 'import pathlib; print("documentation available under \{0\}".format((pathlib.Path(r"{toxworkdir}") / "docs_out" / "index.html").as_uri()))'
 
 [testenv:type]
 description = run type check on code base
-setenv =
-    {tty:MYPY_FORCE_COLOR = 1}
 deps =
-    mypy==0.991
-    types-PyYaml>=6.0.12.2
+    mypy==1.2
+    types-PyYaml>=6.0.12.9
+set_env =
+    {tty:MYPY_FORCE_COLOR = 1}
 commands =
     mypy --strict src
     mypy --strict tests
 
 [testenv:readme]
 description = check that the long description is valid
 skip_install = true
 deps =
-    build[virtualenv]>=0.9
-    twine>=4.0.1
-changedir = {toxinidir}
+    build[virtualenv]>=0.10
+    twine>=4.0.2
+change_dir = {toxinidir}
 commands =
     python -m build -o {envtmpdir} .
     twine check {envtmpdir}/*
 
 [testenv:dev]
 description = generate a DEV environment
-usedevelop = true
+package = editable
 extras =
     test
 commands =
     python -m pip list --format=columns
     python -c 'import sys; print(sys.executable)'
-
-[flake8]
-max-complexity = 22
-max-line-length = 120
-noqa-require-code = true
-ignore =
-    E203 # whitespace before ':'
-dictionaries = en_US,python,technical,django
```

### Comparing `bump_deps_index-1.4.0/.github/workflows/check.yml` & `bump_deps_index-1.4.1/.github/workflows/check.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 name: check
 on:
   push:
+    tags-ignore: ["**"]
   pull_request:
   schedule:
     - cron: "0 8 * * *"
 
 concurrency:
   group: check-${{ github.ref }}
   cancel-in-progress: true
@@ -13,14 +14,15 @@
   test:
     name: test ${{ matrix.py }} - ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         py:
+          - "3.12.0-alpha.7"
           - "3.11"
           - "3.10"
         os:
           - ubuntu-22.04
 
     steps:
       - name: Setup python for tox
@@ -74,30 +76,7 @@
           python-version: "3.11"
       - name: Install tox
         run: python -m pip install tox
       - name: Setup test suite
         run: tox -vv --notest -e ${{ matrix.tox_env }}
       - name: Run test suite
         run: tox --skip-pkg-install -e ${{ matrix.tox_env }}
-
-  publish:
-    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
-    needs: [test, check]
-    runs-on: ubuntu-latest
-    steps:
-      - name: Setup python to build package
-        uses: actions/setup-python@v4
-        with:
-          python-version: "3.11"
-      - name: Install build
-        run: python -m pip install build
-      - uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-      - name: Build sdist and wheel
-        run: python -m build -s -w . -o dist
-      - name: Publish to PyPi
-        uses: pypa/gh-action-pypi-publish@v1.5.1
-        with:
-          skip_existing: true
-          user: __token__
-          password: ${{ secrets.pypi_password }}
```

### Comparing `bump_deps_index-1.4.0/docs/changelog.rst` & `bump_deps_index-1.4.1/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.0/docs/conf.py` & `bump_deps_index-1.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.0/src/bump_deps_index/_cli.py` & `bump_deps_index-1.4.1/src/bump_deps_index/_cli.py`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.0/src/bump_deps_index/_run.py` & `bump_deps_index-1.4.1/src/bump_deps_index/_run.py`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.0/src/bump_deps_index/_spec.py` & `bump_deps_index-1.4.1/src/bump_deps_index/_spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import json
 from enum import Enum, auto
 from functools import cache
 from io import StringIO
 from threading import Lock
 from urllib.request import urlopen
+from xml.etree.ElementTree import parse
 
-from lxml.html import parse
 from packaging.requirements import Requirement
 from packaging.version import Version
 
 
 class PkgType(Enum):
     PYTHON = auto()
     JS = auto()
```

### Comparing `bump_deps_index-1.4.0/tests/test_cli.py` & `bump_deps_index-1.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.0/tests/test_main.py` & `bump_deps_index-1.4.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.0/tests/test_run.py` & `bump_deps_index-1.4.1/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.0/tests/test_spec.py` & `bump_deps_index-1.4.1/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.0/LICENSE` & `bump_deps_index-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.0/README.md` & `bump_deps_index-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.0/pyproject.toml` & `bump_deps_index-1.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,89 @@
 [build-system]
 build-backend = "hatchling.build"
-requires = ["hatchling>=1.11.1", "hatch-vcs>=0.2"]
+requires = [
+  "hatch-vcs>=0.3",
+  "hatchling>=1.14.1",
+]
 
 [project]
 name = "bump-deps-index"
 description = "Bump your dependencies to latest available from index."
 readme = "README.md"
+keywords = [
+  "bump",
+  "index",
+  "pypi",
+  "version",
+]
 license.file = "LICENSE"
 maintainers = [
   { name = "Bernát Gábor", email = "gaborjbernat@gmail.com" },
 ]
-urls.Documentation = "https://bump-deps-index.readthedocs.io"
-urls.Homepage = "https://github.com/gaborbernat/bump-deps-index"
-urls.Source = "https://github.com/gaborbernat/bump-deps-index"
-urls.Tracker = "https://github.com/gaborbernat/bump-deps-index/issues"
 requires-python = ">=3.10"
-dependencies = [
-  "pyyaml>=6",
-  "packaging>=21.3",
-  "lxml>=4.9.1",
-  'tomli>=2.0.1; python_version < "3.11"',
-]
-optional-dependencies.test = [
-  "pytest>=7.2",
-  "pytest-cov>=4",
-  "pytest-mock>=3.10",
-  "covdefaults>=2.2",
-]
-optional-dependencies.docs = [
-  "furo>=2022.9.29",
-  "proselint>=0.13",
-  "sphinx>=5.3",
-  "sphinx-argparse-cli>=1.10",
-]
-keywords = ["pypi", "version", "index", "bump"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-dynamic = ["version"]
-
+dynamic = [
+  "version",
+]
+dependencies = [
+  "packaging>=23.1",
+  "pyyaml>=6",
+  'tomli>=2.0.1; python_version < "3.11"',
+]
+optional-dependencies.docs = [
+  "furo>=2023.3.27",
+  "proselint>=0.13",
+  "sphinx>=6.2.1",
+  "sphinx-argparse-cli>=1.11",
+]
+optional-dependencies.test = [
+  "covdefaults>=2.3",
+  "pytest>=7.3.1",
+  "pytest-cov>=4",
+  "pytest-mock>=3.10",
+]
+urls.Documentation = "https://bump-deps-index.readthedocs.io"
+urls.Homepage = "https://github.com/gaborbernat/bump-deps-index"
+urls.Source = "https://github.com/gaborbernat/bump-deps-index"
+urls.Tracker = "https://github.com/gaborbernat/bump-deps-index/issues"
 [project.entry-points.console_scripts]
 bump-deps-index = "bump_deps_index.__main__:main"
 
 [tool.hatch]
 build.hooks.vcs.version-file = "src/bump_deps_index/version.py"
 version.source = "vcs"
 
 [tool.black]
 line-length = 120
 
+[tool.isort]
+profile = "black"
+known_first_party = ["bumps_deps_index"]
+
+[tool.flake8]
+max-complexity = 22
+max-line-length = 120
+noqa-require-code = true
+ignore =  [
+  "E203", # whitespace before ':'
+]
+dictionaries = ["en_US", "python", "technical", "django"]
+
 [tool.coverage]
 run.dynamic_context = "test_function"
 run.plugins = ["covdefaults"]
 run.parallel = true
 report.fail_under = 100
 html.show_contexts = true
 html.skip_covered = false
@@ -78,11 +101,7 @@
 show_error_codes = true
 strict = true
 overrides = [
   { module = [
     "lxml.*",
   ], ignore_missing_imports = true },
 ]
-
-[tool.isort]
-profile = "black"
-known_first_party = ["bumps_deps_index"]
```

### Comparing `bump_deps_index-1.4.0/PKG-INFO` & `bump_deps_index-1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-deps-index
-Version: 1.4.0
+Version: 1.4.1
 Summary: Bump your dependencies to latest available from index.
 Project-URL: Documentation, https://bump-deps-index.readthedocs.io
 Project-URL: Homepage, https://github.com/gaborbernat/bump-deps-index
 Project-URL: Source, https://github.com/gaborbernat/bump-deps-index
 Project-URL: Tracker, https://github.com/gaborbernat/bump-deps-index/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>
 License: MIT License
@@ -31,33 +31,34 @@
 License-File: LICENSE
 Keywords: bump,index,pypi,version
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
-Requires-Dist: lxml>=4.9.1
-Requires-Dist: packaging>=21.3
+Requires-Dist: packaging>=23.1
 Requires-Dist: pyyaml>=6
 Requires-Dist: tomli>=2.0.1; python_version < '3.11'
 Provides-Extra: docs
-Requires-Dist: furo>=2022.9.29; extra == 'docs'
+Requires-Dist: furo>=2023.3.27; extra == 'docs'
 Requires-Dist: proselint>=0.13; extra == 'docs'
-Requires-Dist: sphinx-argparse-cli>=1.10; extra == 'docs'
-Requires-Dist: sphinx>=5.3; extra == 'docs'
+Requires-Dist: sphinx-argparse-cli>=1.11; extra == 'docs'
+Requires-Dist: sphinx>=6.2.1; extra == 'docs'
 Provides-Extra: test
-Requires-Dist: covdefaults>=2.2; extra == 'test'
+Requires-Dist: covdefaults>=2.3; extra == 'test'
 Requires-Dist: pytest-cov>=4; extra == 'test'
 Requires-Dist: pytest-mock>=3.10; extra == 'test'
-Requires-Dist: pytest>=7.2; extra == 'test'
+Requires-Dist: pytest>=7.3.1; extra == 'test'
 Description-Content-Type: text/markdown
 
 # bump-deps-index
 
 [![PyPI](https://img.shields.io/pypi/v/bump-deps-index?style=flat-square)](https://pypi.org/project/bump-deps-index/)
 [![Supported Python
 versions](https://img.shields.io/pypi/pyversions/bump-deps-index.svg)](https://pypi.org/project/bump-deps-index/)
```


# Comparing `tmp/pyaud-plugins-0.8.0.tar.gz` & `tmp/pyaud-plugins-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaud-plugins-0.8.0.tar", max compression
+gzip compressed data, was "pyaud-plugins-0.9.0.tar", max compression
```

## Comparing `pyaud-plugins-0.8.0.tar` & `pyaud-plugins-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1073 2022-04-26 13:27:55.694627 pyaud-plugins-0.8.0/LICENSE
--rw-r--r--   0        0        0     3233 2022-08-04 07:02:50.647933 pyaud-plugins-0.8.0/README.rst
--rw-r--r--   0        0        0      157 2022-07-01 10:26:08.182614 pyaud-plugins-0.8.0/pyaud_plugins/__init__.py
--rw-r--r--   0        0        0     2335 2022-08-04 07:03:21.216569 pyaud-plugins-0.8.0/pyaud_plugins/_abc.py
--rw-r--r--   0        0        0     6007 2022-08-04 07:03:21.216569 pyaud-plugins-0.8.0/pyaud_plugins/_environ.py
--rw-r--r--   0        0        0     1894 2022-07-13 02:40:49.159713 pyaud-plugins-0.8.0/pyaud_plugins/_parsers.py
--rw-r--r--   0        0        0      128 2022-04-29 13:19:56.279083 pyaud-plugins-0.8.0/pyaud_plugins/_plugins/__init__.py
--rw-r--r--   0        0        0     3600 2022-08-04 07:03:21.216569 pyaud-plugins-0.8.0/pyaud_plugins/_plugins/action.py
--rw-r--r--   0        0        0     3545 2022-07-13 02:40:49.159713 pyaud-plugins-0.8.0/pyaud_plugins/_plugins/audit.py
--rw-r--r--   0        0        0     5471 2022-08-04 07:03:21.217569 pyaud-plugins-0.8.0/pyaud_plugins/_plugins/deprecate.py
--rw-r--r--   0        0        0     2367 2022-08-04 07:03:21.217569 pyaud-plugins-0.8.0/pyaud_plugins/_plugins/fix.py
--rw-r--r--   0        0        0     2737 2022-08-04 07:03:21.217569 pyaud-plugins-0.8.0/pyaud_plugins/_plugins/fix_file.py
--rw-r--r--   0        0        0      870 2022-04-29 13:19:56.281083 pyaud-plugins-0.8.0/pyaud_plugins/_plugins/parametrize.py
--rw-r--r--   0        0        0     5942 2022-08-04 07:03:21.218569 pyaud-plugins-0.8.0/pyaud_plugins/_plugins/write.py
--rw-r--r--   0        0        0      137 2022-04-29 13:19:56.282083 pyaud-plugins-0.8.0/pyaud_plugins/_utils.py
--rw-r--r--   0        0        0      224 2022-08-04 07:03:47.073262 pyaud-plugins-0.8.0/pyaud_plugins/_version.py
--rw-r--r--   0        0        0     2855 2022-08-04 07:03:47.073262 pyaud-plugins-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4641 2022-08-04 07:19:56.530015 pyaud-plugins-0.8.0/setup.py
--rw-r--r--   0        0        0     4818 2022-08-04 07:19:56.530600 pyaud-plugins-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-04-26 13:27:55.694627 pyaud-plugins-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3233 2022-08-05 03:58:03.008761 pyaud-plugins-0.9.0/README.rst
+-rw-r--r--   0        0        0      157 2022-08-05 00:53:52.074915 pyaud-plugins-0.9.0/pyaud_plugins/__init__.py
+-rw-r--r--   0        0        0     2335 2022-08-04 07:03:21.216569 pyaud-plugins-0.9.0/pyaud_plugins/_abc.py
+-rw-r--r--   0        0        0     5765 2022-08-05 04:19:01.423053 pyaud-plugins-0.9.0/pyaud_plugins/_environ.py
+-rw-r--r--   0        0        0     1072 2022-08-05 04:19:01.423053 pyaud-plugins-0.9.0/pyaud_plugins/_parsers.py
+-rw-r--r--   0        0        0      128 2022-04-29 13:19:56.279083 pyaud-plugins-0.9.0/pyaud_plugins/_plugins/__init__.py
+-rw-r--r--   0        0        0     3523 2022-08-05 04:19:01.423053 pyaud-plugins-0.9.0/pyaud_plugins/_plugins/action.py
+-rw-r--r--   0        0        0     3535 2022-08-05 03:49:21.267296 pyaud-plugins-0.9.0/pyaud_plugins/_plugins/audit.py
+-rw-r--r--   0        0        0     5622 2022-08-05 03:39:35.602780 pyaud-plugins-0.9.0/pyaud_plugins/_plugins/deprecate.py
+-rw-r--r--   0        0        0     2367 2022-08-04 07:03:21.217569 pyaud-plugins-0.9.0/pyaud_plugins/_plugins/fix.py
+-rw-r--r--   0        0        0     2737 2022-08-04 07:03:21.217569 pyaud-plugins-0.9.0/pyaud_plugins/_plugins/fix_file.py
+-rw-r--r--   0        0        0      870 2022-04-29 13:19:56.281083 pyaud-plugins-0.9.0/pyaud_plugins/_plugins/parametrize.py
+-rw-r--r--   0        0        0     5942 2022-08-04 07:03:21.218569 pyaud-plugins-0.9.0/pyaud_plugins/_plugins/write.py
+-rw-r--r--   0        0        0      181 2022-08-05 03:39:35.602780 pyaud-plugins-0.9.0/pyaud_plugins/_utils.py
+-rw-r--r--   0        0        0      224 2022-08-05 04:19:01.424053 pyaud-plugins-0.9.0/pyaud_plugins/_version.py
+-rw-r--r--   0        0        0     2833 2022-08-05 04:19:01.424053 pyaud-plugins-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4617 2022-08-05 04:28:14.319864 pyaud-plugins-0.9.0/setup.py
+-rw-r--r--   0        0        0     4780 2022-08-05 04:28:14.321522 pyaud-plugins-0.9.0/PKG-INFO
```

### Comparing `pyaud-plugins-0.8.0/LICENSE` & `pyaud-plugins-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaud-plugins-0.8.0/README.rst` & `pyaud-plugins-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyaud-plugins-0.8.0/pyaud_plugins/_abc.py` & `pyaud-plugins-0.9.0/pyaud_plugins/_abc.py`

 * *Files identical despite different names*

### Comparing `pyaud-plugins-0.8.0/pyaud_plugins/_environ.py` & `pyaud-plugins-0.9.0/pyaud_plugins/_environ.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,22 +145,14 @@
         """Location of the README.rst."""
         with self.prefixed(self.PREFIX):
             return _Path.cwd() / self.path(
                 "README", default=_Path("README.rst")
             )
 
     @property
-    def README_MD(self) -> _Path:
-        """Location of the README.md."""
-        with self.prefixed(self.PREFIX):
-            return _Path.cwd() / self.path(
-                "README", default=_Path("README.md")
-            )
-
-    @property
     def TESTS(self) -> _Path:
         """Location of tests."""
         with self.prefixed(self.PREFIX):
             return _Path.cwd() / self.path("TESTS", default=_Path("tests"))
 
     @property
     def PACKAGE(self) -> _Path:
```

### Comparing `pyaud-plugins-0.8.0/pyaud_plugins/_plugins/action.py` & `pyaud-plugins-0.9.0/pyaud_plugins/_plugins/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import typing as t
 from pathlib import Path
 
 import pyaud
 
 from pyaud_plugins._abc import SphinxBuild
 from pyaud_plugins._environ import environ as e
-from pyaud_plugins._parsers import LineSwitch, Md2Rst
+from pyaud_plugins._parsers import LineSwitch
 from pyaud_plugins._utils import colors
 
 
 @pyaud.plugins.register()
 class Tests(pyaud.plugins.Action):
     """Run the package unit-tests with ``pytest``."""
 
@@ -84,21 +84,20 @@
     def args(self) -> t.Tuple[str | os.PathLike, ...]:
         return "-M", "html", e.DOCS, e.BUILDDIR, "-W"
 
     def action(self, *args: str, **kwargs: bool) -> int:
         returncode = 0
         pyaud.plugins.get("toc")(*args, **kwargs)
         shutil.rmtree(e.BUILDDIR, ignore_errors=True)
-        with Md2Rst(e.README_MD, temp=True):
-            if e.DOCS_CONF.is_file() and e.README_RST.is_file():
-                with LineSwitch(
-                    e.README_RST,
-                    {0: e.README_RST.stem, 1: len(e.README_RST.stem) * "="},
-                ):
-                    returncode = self.sphinx_build(*args, **kwargs)
+        if e.DOCS_CONF.is_file() and e.README_RST.is_file():
+            with LineSwitch(
+                e.README_RST,
+                {0: e.README_RST.stem, 1: len(e.README_RST.stem) * "="},
+            ):
+                returncode = self.sphinx_build(*args, **kwargs)
 
         return returncode
 
 
 @pyaud.plugins.register()
 class DoctestReadme(pyaud.plugins.Action):
     """Run ``doctest`` on Python code-blocks in README."""
```

### Comparing `pyaud-plugins-0.8.0/pyaud_plugins/_plugins/audit.py` & `pyaud-plugins-0.9.0/pyaud_plugins/_plugins/audit.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,15 @@
         )
 
 
 @pyaud.plugins.register()
 class Typecheck(pyaud.plugins.Audit):
     """Typecheck code with ``mypy``.
 
-    Check that there are no errors between the files and their stub-
-    files.
+    Check there are no errors between the files and their stub-files.
     """
 
     mypy = "mypy"
     cache = True
 
     @property
     def exe(self) -> t.List[str]:
```

### Comparing `pyaud-plugins-0.8.0/pyaud_plugins/_plugins/deprecate.py` & `pyaud-plugins-0.9.0/pyaud_plugins/_plugins/deprecate.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,30 @@
 import shutil
 import typing as t
 from pathlib import Path
 
 import pyaud
 
 from pyaud_plugins._environ import environ as e
-from pyaud_plugins._utils import colors
+from pyaud_plugins._utils import colors, git
+
+HEAD = "HEAD"
+
+
+def branch() -> t.Optional[str]:
+    """Return current Git branch if in Git repository.
+
+    :return: Checked out branch or None if no parent commit or repo.
+    """
+    git.symbolic_ref("--short", HEAD, suppress=True, capture=True)
+    stdout = git.stdout()
+    if stdout:
+        return stdout[-1]
+
+    return None
 
 
 @pyaud.plugins.register()
 class Deploy(pyaud.plugins.Parametrize):
     """Deploy package documentation and test coverage."""
 
     def plugins(self) -> t.List[str]:
@@ -68,74 +83,72 @@
     _pushing_skipped = "Pushing skipped"
     _origin = "origin"
     _gh_pages = "gh-pages"
 
     def deploy_docs(self) -> None:
         """Series of functions for deploying docs."""
         root_html = Path.cwd() / "html"
-        pyaud.git.add(".")
-        pyaud.git.diff_index("--cached", "HEAD", capture=True)
+        git.add(".")
+        git.diff_index("--cached", HEAD, capture=True)
         stashed = False
-        if pyaud.git.stdout():
-            pyaud.git.stash(file=os.devnull)
+        if git.stdout():
+            git.stash(file=os.devnull)
             stashed = True
 
         shutil.move(str(e.DOCS_HTML), root_html)
         shutil.copy(e.README_RST, root_html / e.README_RST.name)
-        pyaud.git.rev_list("--max-parents=0", "HEAD", capture=True)
-        stdout = pyaud.git.stdout()
+        git.rev_list("--max-parents=0", HEAD, capture=True)
+        stdout = git.stdout()
         if stdout:
-            pyaud.git.checkout(stdout[-1])
+            git.checkout(stdout[-1])
 
-        pyaud.git.checkout("--orphan", self._gh_pages)
-        pyaud.git.config("--global", "user.name", e.GH_NAME)
-        pyaud.git.config("--global", "user.email", e.GH_EMAIL)
+        git.checkout("--orphan", self._gh_pages)
+        git.config("--global", "user.name", e.GH_NAME)
+        git.config("--global", "user.email", e.GH_EMAIL)
         shutil.rmtree(e.DOCS)
-        pyaud.git.rm("-rf", Path.cwd(), file=os.devnull)
-        pyaud.git.clean("-fdx", "--exclude=html", file=os.devnull)
+        git.rm("-rf", Path.cwd(), file=os.devnull)
+        git.clean("-fdx", "--exclude=html", file=os.devnull)
         for file in root_html.rglob("*"):
             shutil.move(str(file), Path.cwd() / file.name)
 
         shutil.rmtree(root_html)
-        pyaud.git.add(".")
-        pyaud.git.commit(
+        git.add(".")
+        git.commit(
             "-m",
             '"[ci skip] Publishes updated documentation"',
             file=os.devnull,
         )
-        pyaud.git.remote("rm", self._origin)
-        pyaud.git.remote("add", self._origin, e.GH_REMOTE)
-        pyaud.git.fetch()
-        pyaud.git.stdout()
-        pyaud.git.ls_remote(
-            "--heads", e.GH_REMOTE, self._gh_pages, capture=True
-        )
-        result = pyaud.git.stdout()
+        git.remote("rm", self._origin)
+        git.remote("add", self._origin, e.GH_REMOTE)
+        git.fetch()
+        git.stdout()
+        git.ls_remote("--heads", e.GH_REMOTE, self._gh_pages, capture=True)
+        result = git.stdout()
         remote_exists = None if not result else result[-1]
-        pyaud.git.diff(
+        git.diff(
             self._gh_pages, "origin/gh-pages", suppress=True, capture=True
         )
-        result = pyaud.git.stdout()
+        result = git.stdout()
         remote_diff = None if not result else result[-1]
         if remote_exists is not None and remote_diff is None:
             colors.green.print("No difference between local branch and remote")
             print(self._pushing_skipped)
         else:
             colors.green.print("Pushing updated documentation")
-            pyaud.git.push(self._origin, self._gh_pages, "-f")
+            git.push(self._origin, self._gh_pages, "-f")
             print("Documentation Successfully deployed")
 
-        pyaud.git.checkout("master", file=os.devnull)
+        git.checkout("master", file=os.devnull)
         if stashed:
-            pyaud.git.stash("pop", file=os.devnull)
+            git.stash("pop", file=os.devnull)
 
-        pyaud.git.branch("-D", self._gh_pages, file=os.devnull)
+        git.branch("-D", self._gh_pages, file=os.devnull)
 
     def action(self, *args: str, **kwargs: bool) -> int:
-        if pyaud.branch() == "master":
+        if branch() == "master":
             git_credentials = ["GH_NAME", "GH_EMAIL", "GH_TOKEN"]
             null_vals = [k for k in git_credentials if getattr(e, k) is None]
             if not null_vals:
                 if not e.DOCS_HTML.is_dir():
                     pyaud.plugins.get("docs")(**kwargs)
 
                 self.deploy_docs()
```

### Comparing `pyaud-plugins-0.8.0/pyaud_plugins/_plugins/fix.py` & `pyaud-plugins-0.9.0/pyaud_plugins/_plugins/fix.py`

 * *Files identical despite different names*

### Comparing `pyaud-plugins-0.8.0/pyaud_plugins/_plugins/fix_file.py` & `pyaud-plugins-0.9.0/pyaud_plugins/_plugins/fix_file.py`

 * *Files identical despite different names*

### Comparing `pyaud-plugins-0.8.0/pyaud_plugins/_plugins/parametrize.py` & `pyaud-plugins-0.9.0/pyaud_plugins/_plugins/parametrize.py`

 * *Files identical despite different names*

### Comparing `pyaud-plugins-0.8.0/pyaud_plugins/_plugins/write.py` & `pyaud-plugins-0.9.0/pyaud_plugins/_plugins/write.py`

 * *Files identical despite different names*

### Comparing `pyaud-plugins-0.8.0/pyproject.toml` & `pyaud-plugins-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -48,29 +48,28 @@
     "audit",
     "ci",
     "python",
 ]
 license = "MIT"
 name = "pyaud-plugins"
 readme = "README.rst"
-version = "0.8.0"
+version = "0.9.0"
 
 [tool.poetry.dependencies]
 Sphinx = "^4.3.2"
 appdirs = "^1.4.4"
 black = ">=21.12,<23.0"
 codecov = "^2.1.12"
 constcheck = "^0"
 coverage = "^6.2"
 docformatter = "^1.4"
 environs = "^9.4.0"
 flynt = ">=0.75,<0.77"
+gitspy = "^0"
 isort = "^5.10.1"
-m2r = "^0.2.1"
-mistune = "<=0.8.4"
 mypy = ">=0.930,<0.972"
 object-colors = "^2.0.1"
 pipfile-requirements = "^0.3.0"
 pylint = "^2.12.2"
 pytest = ">=6.2.5,<8.0.0"
 pytest-cov = "^3.0.0"
 python = "^3.8"
@@ -82,15 +81,15 @@
 toml-sort = "^0.20.0"
 vulture = "^2.3"
 docsig = "^0"
 
 [tool.poetry.dev-dependencies]
 bump2version = "^1.0.1"
 ipython = "^8.4.0"
-pyaud = "^3.13.5"
+pyaud = "^4.0.2"
 pytest = ">=6.2.5,<8.0.0"
 pytest-randomly = "^3.12.0"
 pytest-sugar = "^0.9.5"
 pytest-xdist = "^2.5.0"
 restview = "^3.0.0"
 sphinx-toolbox = "^3.1.2"
 tomli-w = "^1.0.0"
```

### Comparing `pyaud-plugins-0.8.0/setup.py` & `pyaud-plugins-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,16 @@
  'codecov>=2.1.12,<3.0.0',
  'constcheck>=0,<1',
  'coverage>=6.2,<7.0',
  'docformatter>=1.4,<2.0',
  'docsig>=0,<1',
  'environs>=9.4.0,<10.0.0',
  'flynt>=0.75,<0.77',
+ 'gitspy>=0,<1',
  'isort>=5.10.1,<6.0.0',
- 'm2r>=0.2.1,<0.3.0',
- 'mistune<=0.8.4',
  'mypy>=0.930,<0.972',
  'object-colors>=2.0.1,<3.0.0',
  'pipfile-requirements>=0.3.0,<0.4.0',
  'pylint>=2.12.2,<3.0.0',
  'pytest-cov>=3.0.0,<4.0.0',
  'pytest>=6.2.5,<8.0.0',
  'python-dotenv>=0.19.2,<0.21.0',
@@ -33,15 +32,15 @@
  'sphinxcontrib-programoutput>=0.17,<0.18',
  'toml-sort>=0.20.0,<0.21.0',
  'toml>=0.10.2,<0.11.0',
  'vulture>=2.3,<3.0']
 
 setup_kwargs = {
     'name': 'pyaud-plugins',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Plugin package for Pyaud',
     'long_description': 'pyaud-plugins\n=============\n.. image:: https://img.shields.io/badge/License-MIT-yellow.svg\n    :target: https://opensource.org/licenses/MIT\n    :alt: License\n.. image:: https://img.shields.io/pypi/v/pyaud-plugins\n    :target: https://img.shields.io/pypi/v/pyaud-plugins\n    :alt: pypi\n.. image:: https://github.com/jshwi/pyaud-plugins/actions/workflows/ci.yml/badge.svg\n    :target: https://github.com/jshwi/pyaud-plugins/actions/workflows/ci.yml\n    :alt: CI\n.. image:: https://github.com/jshwi/pyaud-plugins/actions/workflows/codeql-analysis.yml/badge.svg\n    :target: https://github.com/jshwi/pyaud-plugins/actions/workflows/codeql-analysis.yml\n    :alt: CodeQL\n.. image:: https://codecov.io/gh/jshwi/pyaud-plugins/branch/master/graph/badge.svg\n    :target: https://codecov.io/gh/jshwi/pyaud-plugins\n    :alt: codecov.io\n.. image:: https://readthedocs.org/projects/pyaud-plugins/badge/?version=latest\n    :target: https://pyaud-plugins.readthedocs.io/en/latest/?badge=latest\n    :alt: readthedocs.org\n.. image:: https://img.shields.io/badge/python-3.8-blue.svg\n    :target: https://www.python.org/downloads/release/python-380\n    :alt: python3.8\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n    :alt: black\n\nPlugin package for Pyaud\n------------------------\n\nDependencies\n------------\n\n``pip install pyaud``\n\nInstall\n-------\n\n``pip install pyaud-plugins``\n\nDevelopment\n-----------\n\n``poetry install``\n\nUsage\n-----\n\nSee `pyaud <https://github.com/jshwi/pyaud#pyaud>`_\n\nPlugins\n-------\n\n``pyaud`` will automatically load this package on search for all packages prefixed with `"pyaud_"`\n\nFor writing plugins see `docs <https://jshwi.github.io/pyaud/pyaud.html#pyaud-plugins>`_\n\nThis package contains the following plugins on running `pyaud modules`\n\n.. code-block:: console\n\n    const           -- Check code for repeat use of strings\n    coverage        -- Run package unit-tests with `pytest` and `coverage`\n    deploy          -- Deploy package documentation and test coverage\n    deploy-cov      -- Upload coverage data to `Codecov`\n    deploy-docs     -- Deploy package documentation to `gh-pages`\n    docs            -- Compile package documentation with `Sphinx`\n    doctest         -- Run `doctest` on all code examples\n    doctest-package -- Run `doctest` on package\n    doctest-readme  -- Run `doctest` on Python code-blocks in README\n    files           -- Audit project data files\n    format          -- Audit code with `Black`\n    format-docs     -- Format docstrings with `docformatter`\n    format-str      -- Format f-strings with `flynt`\n    imports         -- Audit imports with `isort`\n    lint            -- Lint code with `pylint`\n    readme          -- Parse, test, and assert RST code-blocks\n    requirements    -- Audit requirements.txt with Pipfile.lock\n    sort-pyproject  -- Sort pyproject.toml file with `toml-sort`\n    test            -- Run all tests\n    tests           -- Run the package unit-tests with `pytest`\n    toc             -- Audit docs/<NAME>.rst toc-file\n    typecheck       -- Typecheck code with `mypy`\n    unused          -- Audit unused code with `vulture`\n    whitelist       -- Check whitelist.py file with `vulture`\n',
     'author': 'jshwi',
     'author_email': 'stephen@jshwisolutions.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `pyaud-plugins-0.8.0/PKG-INFO` & `pyaud-plugins-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaud-plugins
-Version: 0.8.0
+Version: 0.9.0
 Summary: Plugin package for Pyaud
 License: MIT
 Keywords: pyaud,plugins,audit,ci,python
 Author: jshwi
 Author-email: stephen@jshwisolutions.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -18,17 +18,16 @@
 Requires-Dist: codecov (>=2.1.12,<3.0.0)
 Requires-Dist: constcheck (>=0,<1)
 Requires-Dist: coverage (>=6.2,<7.0)
 Requires-Dist: docformatter (>=1.4,<2.0)
 Requires-Dist: docsig (>=0,<1)
 Requires-Dist: environs (>=9.4.0,<10.0.0)
 Requires-Dist: flynt (>=0.75,<0.77)
+Requires-Dist: gitspy (>=0,<1)
 Requires-Dist: isort (>=5.10.1,<6.0.0)
-Requires-Dist: m2r (>=0.2.1,<0.3.0)
-Requires-Dist: mistune (<=0.8.4)
 Requires-Dist: mypy (>=0.930,<0.972)
 Requires-Dist: object-colors (>=2.0.1,<3.0.0)
 Requires-Dist: pipfile-requirements (>=0.3.0,<0.4.0)
 Requires-Dist: pylint (>=2.12.2,<3.0.0)
 Requires-Dist: pytest (>=6.2.5,<8.0.0)
 Requires-Dist: pytest-cov (>=3.0.0,<4.0.0)
 Requires-Dist: python-dotenv (>=0.19.2,<0.21.0)
```


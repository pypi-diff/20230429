# Comparing `tmp/coverage_rich-0.1.0.dev1.tar.gz` & `tmp/coverage_rich-0.2.0.dev0.tar.gz`

## Comparing `coverage_rich-0.1.0.dev1.tar` & `coverage_rich-0.2.0.dev0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/CHANGELOG.md
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/.github/workflows/release.yml
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/coverage_rich/__about__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/coverage_rich/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/coverage_rich/__main__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/coverage_rich/config.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/coverage_rich/console.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/coverage_rich/report.py
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/coverage_rich/standard_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/coverage_rich/cli/__init__.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/coverage_rich/cli/app.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/coverage_rich/cli/common.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/coverage_rich/cli/config.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/coverage_rich/cli/report.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/coverage_rich/cli/tui.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/coverage_rich/tui/app.css
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/coverage_rich/tui/app.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/tests/__init__.py
--rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/tests/test_report.py
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/LICENSE.txt
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/README.md
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 coverage_rich-0.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/CHANGELOG.md
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/__about__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/__main__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/config.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/console.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/report.py
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/standard_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/cli/__init__.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/cli/app.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/cli/common.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/cli/config.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/cli/report.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/cli/tui.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/tui/app.css
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/coverage_rich/tui/app.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/tests/__init__.py
+-rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/tests/test_report.py
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/LICENSE.txt
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/README.md
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 coverage_rich-0.2.0.dev0/PKG-INFO
```

### Comparing `coverage_rich-0.1.0.dev1/coverage_rich/report.py` & `coverage_rich-0.2.0.dev0/coverage_rich/report.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,42 @@
 import json
 import subprocess
+import sys
 
 from rich.console import Console
 from rich.table import Table
 
 from coverage_rich.config import config
+from coverage_rich.console import console
+
+
+def get_coverage_data():
+    try:
+        return json.loads(subprocess.check_output(["coverage", "json", "-o", "-"]))
+
+    except subprocess.CalledProcessError:
+        console.log("No coverage data found.")
+        console.log("Attempting to combine coverage data...")
+
+    try:
+        subprocess.check_output(["coverage", "combine"])
+        return json.loads(subprocess.check_output(["coverage", "json", "-o", "-"]))
+    except subprocess.CalledProcessError:
+        Console().log("No coverage data found.")
+        Console().log()
+        Console().log("You might need to run coverage")
+        Console().log("coverage run my_program.py arg1 arg2")
+        Console().log("coverage run -m pytest")
+        Console().log("more help at https://coverage.readthedocs.io/")
+    sys.exit(1)
 
 
 def report(coverage_data=None):
     if coverage_data is None:
-        coverage_data = json.loads(
-            subprocess.check_output(["coverage", "json", "-o", "-"])
-        )
+        coverage_data = get_coverage_data()
     meta = coverage_data.get("meta", {})
 
     table = Table(title=f"pytest-{meta.get('version')} {meta.get('timestamp')}")
     table.add_column("Name", style="blue")
     table.add_column("Stmts", justify="right", style="green")
     table.add_column("Miss", justify="right", style="red")
     table.add_column("Branch", justify="right", style="green")
```

### Comparing `coverage_rich-0.1.0.dev1/coverage_rich/standard_config.py` & `coverage_rich-0.2.0.dev0/coverage_rich/standard_config.py`

 * *Files identical despite different names*

### Comparing `coverage_rich-0.1.0.dev1/coverage_rich/cli/app.py` & `coverage_rich-0.2.0.dev0/coverage_rich/cli/app.py`

 * *Files identical despite different names*

### Comparing `coverage_rich-0.1.0.dev1/coverage_rich/cli/config.py` & `coverage_rich-0.2.0.dev0/coverage_rich/cli/config.py`

 * *Files identical despite different names*

### Comparing `coverage_rich-0.1.0.dev1/coverage_rich/tui/app.py` & `coverage_rich-0.2.0.dev0/coverage_rich/tui/app.py`

 * *Files identical despite different names*

### Comparing `coverage_rich-0.1.0.dev1/tests/test_report.py` & `coverage_rich-0.2.0.dev0/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `coverage_rich-0.1.0.dev1/.gitignore` & `coverage_rich-0.2.0.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `coverage_rich-0.1.0.dev1/LICENSE.txt` & `coverage_rich-0.2.0.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coverage_rich-0.1.0.dev1/README.md` & `coverage_rich-0.2.0.dev0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+<img src="https://user-images.githubusercontent.com/22648375/218338845-4e0ff4e7-fb04-4d13-9b83-58d1b23d2a87.png" alt="coverage-rich" width="250" align=right>
+
+
 # coverage-rich
 
 [![PyPI - Version](https://img.shields.io/pypi/v/coverage-rich.svg)](https://pypi.org/project/coverage-rich)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/coverage-rich.svg)](https://pypi.org/project/coverage-rich)
 
 -----
```

### Comparing `coverage_rich-0.1.0.dev1/pyproject.toml` & `coverage_rich-0.2.0.dev0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 dependencies = [
   "ipython",
   "mypy",
   "pyflyby",
   "pytest",
   "pytest-cov",
   "pytest-mock",
-  "pytest-rich",
   "ruff",
   "black",
 ]
 [tool.hatch.envs.default.scripts]
 test = "coverage run -m pytest"
 covreport = "coverage-rich report"
 cov = ['test', 'covreport']
@@ -87,13 +86,13 @@
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
 [tool.pytest.ini_options]
-addopts = "-ra -q --rich"
+addopts = "-ra -q"
 asyncio_mode = "auto"
 testpaths = ["tests"]
 
 [tool.coverage_rich]
 fail-under=24
```

### Comparing `coverage_rich-0.1.0.dev1/PKG-INFO` & `coverage_rich-0.2.0.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coverage-rich
-Version: 0.1.0.dev1
+Version: 0.2.0.dev0
 Summary: A rich terminal report for coveragepy.
 Project-URL: Documentation, https://github.com/waylonwalker/coverage-rich#readme
 Project-URL: Issues, https://github.com/waylonwalker/coverage-rich/issues
 Project-URL: Source, https://github.com/waylonwalker/coverage-rich
 Project-URL: Changelog, https://github.com/waylonwalker/coverage-rich
 Author-email: "Waylon S. Walker" <waylon@waylonwalker.com>
 License-Expression: MIT
@@ -22,14 +22,17 @@
 Requires-Dist: anyconfig
 Requires-Dist: coverage
 Requires-Dist: rich
 Requires-Dist: textual
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
+<img src="https://user-images.githubusercontent.com/22648375/218338845-4e0ff4e7-fb04-4d13-9b83-58d1b23d2a87.png" alt="coverage-rich" width="250" align=right>
+
+
 # coverage-rich
 
 [![PyPI - Version](https://img.shields.io/pypi/v/coverage-rich.svg)](https://pypi.org/project/coverage-rich)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/coverage-rich.svg)](https://pypi.org/project/coverage-rich)
 
 -----
```


# Comparing `tmp/tryceratops-1.1.0.tar.gz` & `tmp/tryceratops-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tryceratops-1.1.0.tar", max compression
+gzip compressed data, was "tryceratops-1.2.0.tar", max compression
```

## Comparing `tryceratops-1.1.0.tar` & `tryceratops-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0     1084 2022-04-30 13:27:37.265022 tryceratops-1.1.0/LICENSE
--rw-r--r--   0        0        0     6282 2022-04-30 13:28:41.597475 tryceratops-1.1.0/README.md
--rw-r--r--   0        0        0     1997 2022-04-30 13:28:41.625476 tryceratops-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       75 2022-04-30 13:28:41.597475 tryceratops-1.1.0/src/tryceratops/__init__.py
--rw-r--r--   0        0        0     2202 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/__main__.py
--rw-r--r--   0        0        0     1071 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/analyzers/__init__.py
--rw-r--r--   0        0        0     1596 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/analyzers/base.py
--rw-r--r--   0        0        0     5337 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/analyzers/call.py
--rw-r--r--   0        0        0     2136 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/analyzers/conditional.py
--rw-r--r--   0        0        0     5277 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/analyzers/exception_block.py
--rw-r--r--   0        0        0      342 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/analyzers/exceptions.py
--rw-r--r--   0        0        0     1107 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/analyzers/try_block.py
--rw-r--r--   0        0        0       50 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/files/__init__.py
--rw-r--r--   0        0        0     3602 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/files/discovery.py
--rw-r--r--   0        0        0     1453 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/files/parser.py
--rw-r--r--   0        0        0     3102 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/filters.py
--rw-r--r--   0        0        0      601 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/fixers/__init__.py
--rw-r--r--   0        0        0     2463 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/fixers/base.py
--rw-r--r--   0        0        0     2731 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/fixers/exception_block.py
--rw-r--r--   0        0        0      353 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/fixers/exceptions.py
--rw-r--r--   0        0        0     2121 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/flake_plugin.py
--rw-r--r--   0        0        0     2668 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/interfaces.py
--rw-r--r--   0        0        0      165 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/processors.py
--rw-r--r--   0        0        0     3006 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/runners.py
--rw-r--r--   0        0        0     1065 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/settings.py
--rw-r--r--   0        0        0      627 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/types.py
--rw-r--r--   0        0        0      108 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/violations/__init__.py
--rw-r--r--   0        0        0     1258 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/violations/codes.py
--rw-r--r--   0        0        0     1479 2022-04-30 13:27:37.269022 tryceratops-1.1.0/src/tryceratops/violations/violations.py
--rw-r--r--   0        0        0     7525 2022-04-30 13:28:46.540452 tryceratops-1.1.0/setup.py
--rw-r--r--   0        0        0     7416 2022-04-30 13:28:46.540977 tryceratops-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-29 18:22:03.770300 tryceratops-1.2.0/LICENSE
+-rw-r--r--   0        0        0     6162 2023-04-29 18:22:36.390037 tryceratops-1.2.0/README.md
+-rw-r--r--   0        0        0     2143 2023-04-29 18:22:36.434037 tryceratops-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-04-29 18:22:36.390037 tryceratops-1.2.0/src/tryceratops/__init__.py
+-rw-r--r--   0        0        0     2218 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/__main__.py
+-rw-r--r--   0        0        0     1044 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/analyzers/__init__.py
+-rw-r--r--   0        0        0     1746 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/analyzers/base.py
+-rw-r--r--   0        0        0     5616 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/analyzers/call.py
+-rw-r--r--   0        0        0     2154 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/analyzers/conditional.py
+-rw-r--r--   0        0        0     5309 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/analyzers/exception_block.py
+-rw-r--r--   0        0        0      342 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/analyzers/exceptions.py
+-rw-r--r--   0        0        0     1192 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/analyzers/try_block.py
+-rw-r--r--   0        0        0       50 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/files/__init__.py
+-rw-r--r--   0        0        0     3610 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/files/discovery.py
+-rw-r--r--   0        0        0     1453 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/files/parser.py
+-rw-r--r--   0        0        0     3126 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/filters.py
+-rw-r--r--   0        0        0      601 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/fixers/__init__.py
+-rw-r--r--   0        0        0     2653 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/fixers/base.py
+-rw-r--r--   0        0        0     2747 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/fixers/exception_block.py
+-rw-r--r--   0        0        0      353 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/fixers/exceptions.py
+-rw-r--r--   0        0        0     2121 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/flake_plugin.py
+-rw-r--r--   0        0        0     2715 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/interfaces.py
+-rw-r--r--   0        0        0      165 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/processors.py
+-rw-r--r--   0        0        0     3030 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/runners.py
+-rw-r--r--   0        0        0     1065 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/settings.py
+-rw-r--r--   0        0        0      627 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/types.py
+-rw-r--r--   0        0        0      108 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/violations/__init__.py
+-rw-r--r--   0        0        0     1258 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/violations/codes.py
+-rw-r--r--   0        0        0     1773 2023-04-29 18:22:03.774299 tryceratops-1.2.0/src/tryceratops/violations/violations.py
+-rw-r--r--   0        0        0     7341 1970-01-01 00:00:00.000000 tryceratops-1.2.0/PKG-INFO
```

### Comparing `tryceratops-1.1.0/LICENSE` & `tryceratops-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tryceratops-1.1.0/README.md` & `tryceratops-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
   <a href="https://pypi.org/project/tryceratops/"><img alt="PyPI" src="https://img.shields.io/pypi/v/tryceratops"/></a>
   <img src="https://badgen.net/pypi/python/tryceratops" />
   <a href="https://github.com/relekang/python-semantic-release"><img alt="Semantic Release" src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg"></a>
   <a href="https://github.com/guilatrova/tryceratops/blob/main/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/guilatrova/tryceratops"/></a>
   <a href="https://pepy.tech/project/tryceratops/"><img alt="Downloads" src="https://static.pepy.tech/personalized-badge/tryceratops?period=total&units=international_system&left_color=grey&right_color=blue&left_text=%F0%9F%A6%96%20Downloads"/></a>
   <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
   <a href="https://github.com/guilatrova/tryceratops"><img alt="try/except style: tryceratops" src="https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black" /></a>
-  <a href="https://open.vscode.dev/guilatrova/tryceratops"><img alt="Open in Visual Studio Code" src="https://open.vscode.dev/badges/open-in-vscode.svg"/></a>
   <a href="https://twitter.com/intent/user?screen_name=guilatrova"><img alt="Follow guilatrova" src="https://img.shields.io/twitter/follow/guilatrova?style=social"/></a>
 </p>
 
 Inspired by [this blog post](https://blog.guilatrova.dev/handling-exceptions-in-python-like-a-pro/). I described [the building process of this tool here](https://blog.guilatrova.dev/project-tryceratops/).
 
 > “For those who like dinosaurs 🦖 and clean try/except ✨ blocks.”
 
@@ -44,14 +43,20 @@
 
 ### Installation
 
 ```
 pip install tryceratops
 ```
 
+OR
+
+```
+poetry add -D tryceratops
+```
+
 ### Usage
 
 ```
 tryceratops [filename or dir...]
 ```
 
 You can enable experimental analyzers by running:
@@ -135,15 +140,15 @@
 
 ## Pre-commit
 
 If you wish to use pre-commit, add this:
 
 ```yaml
   - repo: https://github.com/guilatrova/tryceratops
-    rev: v1.1.0
+    rev: v1.2.0
     hooks:
       - id: tryceratops
 ```
 
 ## Show your style
 
 [![try/except style: tryceratops](https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black)](https://github.com/guilatrova/tryceratops)
```

### Comparing `tryceratops-1.1.0/pyproject.toml` & `tryceratops-1.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "tryceratops"
-version = "1.1.0"
-description = "A linter to manage your exception like a PRO!"
+version = "1.2.0"
+description = "Prevent Exception Handling AntiPatterns"
 authors = ["Guilherme Latrova <hello@guilatrova.dev>"]
 license = "MIT"
 keywords = ["lint", "try", "except"]
 readme = "README.md"
 homepage = "https://github.com/guilatrova/tryceratops"
 repository = "https://github.com/guilatrova/tryceratops"
 include = [
@@ -61,22 +61,28 @@
 isort = "^5.8.0"
 pre-commit = "^2.13.0"
 astpretty = "^2.1.0"
 pytest-cov = "^2.12.1"
 python-semantic-release = "^7.16.2"
 mypy = "^0.910"
 types-toml = "^0.1.3"
+flake8-annotations = "^2.9.0"
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
 profile = "black"
 line_length = 100
 extra_standard_library = ["pytest", "toml", "click"]
 
 [tool.mypy]
+python_version = 3.8
+warn_unused_configs = true
+namespace_packages = true
+explicit_package_bases = true
 ignore_missing_imports = true
+exclude = 'tests'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tryceratops-1.1.0/src/tryceratops/__main__.py` & `tryceratops-1.2.0/src/tryceratops/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 def entrypoint(
     dir: Tuple[str],
     experimental: bool,
     ignore: Tuple[str, ...],
     exclude: Tuple[str, ...],
     verbose: bool,
     autofix: bool,
-):
+) -> None:
     pyproj_config = load_config(dir)
     if pyproj_config:
         global_settings = GlobalSettings.create_from_config(pyproj_config)
         global_settings.overwrite_from_cli(experimental, ignore, exclude, autofix)
     else:
         global_settings = GlobalSettings(experimental, ignore, exclude, autofix)
 
@@ -57,14 +57,14 @@
 
     parsed_files = list(discovery.parse_python_files(dir))
     runner.analyze(parsed_files, global_settings)
 
     interface.present_and_exit()
 
 
-def main():
+def main() -> None:
     logging.config.dictConfig(LOGGING_CONFIG)
     entrypoint(prog_name="tryceratops")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `tryceratops-1.1.0/src/tryceratops/analyzers/__init__.py` & `tryceratops-1.2.0/src/tryceratops/analyzers/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Set
+from typing import TYPE_CHECKING, Set, Type, cast
 
 from . import call, conditional, exception_block, try_block
 from .base import BaseAnalyzer
 
 if TYPE_CHECKING:
     from tryceratops.filters import GlobalSettings
 
 
-ANALYZER_CLASSES = {
-    call.CallTooManyAnalyzer,  # type: ignore
-    call.CallRaiseVanillaAnalyzer,  # type: ignore
-    call.CallRaiseLongArgsAnalyzer,  # type: ignore
-    call.CallAvoidCheckingToContinueAnalyzer,  # type: ignore
+ANALYZER_CLASSES: Set[Type[BaseAnalyzer]] = {
+    call.CallTooManyAnalyzer,
+    call.CallRaiseVanillaAnalyzer,
+    call.CallRaiseLongArgsAnalyzer,
+    call.CallAvoidCheckingToContinueAnalyzer,
     conditional.PreferTypeErrorAnalyzer,
     exception_block.ExceptReraiseWithoutCauseAnalyzer,
     exception_block.ExceptVerboseReraiseAnalyzer,
     exception_block.ExceptBroadPassAnalyzer,
     exception_block.LogErrorAnalyzer,
     exception_block.LogObjectAnalyzer,
     try_block.TryConsiderElseAnalyzer,
```

### Comparing `tryceratops-1.1.0/src/tryceratops/analyzers/base.py` & `tryceratops-1.2.0/src/tryceratops/analyzers/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import ast
 from abc import ABC, abstractmethod
-from typing import List, Protocol, Type
+from typing import Any, Callable, List, Protocol, Type
 
 from tryceratops.processors import Processor
 from tryceratops.violations import Violation
 
 from .exceptions import AnalyzerVisitException
 
 
 class BaseAnalyzer(ABC, Processor, ast.NodeVisitor):
     violation_type: Type[Violation] = Violation
 
     def __init__(self):
         self.violations: List[Violation] = []
 
-    def _mark_violation(self, *nodes, **kwargs):
+    def _mark_violation(self, *nodes: ast.AST, **kwargs: Any) -> None:  # noqa: ANN401
         klass = self.violation_type
         for node in nodes:
             violation = klass.build(self.filename, self.violation_code, node, **kwargs)
             self.violations.append(violation)
 
     def check(self, tree: ast.AST, filename: str) -> List[Violation]:
         self.filename = filename
@@ -29,30 +29,30 @@
         return self.violations
 
 
 class StmtBodyProtocol(Protocol):
     body: List[ast.stmt]
 
 
-def visit_error_handler(func):
-    def _func(instance, node: ast.stmt):
+def visit_error_handler(func: Callable[[BaseAnalyzer, Any], Any]):  # noqa: ANN201
+    def _func(instance: Any, node: ast.stmt) -> None:  # noqa: ANN401
         try:
             return func(instance, node)
         except Exception as ex:
             raise AnalyzerVisitException(node) from ex
 
     return _func
 
 
 class BaseRaiseCallableAnalyzer(BaseAnalyzer, ABC):
     @abstractmethod
-    def _check_raise_callable(self, node: ast.Raise, exc: ast.Call, func: ast.Name):
+    def _check_raise_callable(self, node: ast.Raise, exc: ast.Call, func: ast.Name) -> None:
         pass
 
     @visit_error_handler
-    def visit_Raise(self, node: ast.Raise):
+    def visit_Raise(self, node: ast.Raise) -> None:
         if exc := node.exc:
             if isinstance(exc, ast.Call):
                 if isinstance(exc.func, ast.Name):
                     self._check_raise_callable(node, exc, exc.func)
 
         self.generic_visit(node)
```

### Comparing `tryceratops-1.1.0/src/tryceratops/analyzers/call.py` & `tryceratops-1.2.0/src/tryceratops/analyzers/call.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,140 +1,141 @@
-# type: ignore
 import ast
-from typing import Dict, List
+from typing import Dict, List, Union, cast
 
 from tryceratops.violations import Violation, codes
 
 from .base import BaseAnalyzer, BaseRaiseCallableAnalyzer, StmtBodyProtocol, visit_error_handler
 
 
 class CallTooManyAnalyzer(BaseAnalyzer):
     violation_code = codes.TOO_MANY_TRY
 
     @visit_error_handler
-    def visit_FunctionDef(self, node: ast.FunctionDef) -> None:
+    def visit_FunctionDef(self, node: ast.FunctionDef):  # noqa: ANN201
         try_blocks = [stm for stm in ast.iter_child_nodes(node) if isinstance(stm, ast.Try)]
 
         if len(try_blocks) > 1:
             _, *violation_blocks = try_blocks
             self._mark_violation(*violation_blocks)
 
         self.generic_visit(node)
 
 
 class CallRaiseVanillaAnalyzer(BaseRaiseCallableAnalyzer):
     violation_code = codes.RAISE_VANILLA_CLASS
 
-    def _check_raise_callable(self, node: ast.Raise, exc: ast.Call, func: ast.Name):
+    def _check_raise_callable(self, node: ast.Raise, exc: ast.Call, func: ast.Name) -> None:
         if func.id == "Exception":
             self._mark_violation(node)
 
 
 class CallRaiseLongArgsAnalyzer(BaseRaiseCallableAnalyzer):
     violation_code = codes.RAISE_VANILLA_ARGS
 
-    def _check_raise_callable(self, node: ast.Raise, exc: ast.Call, func: ast.Name):
+    def _check_raise_callable(self, node: ast.Raise, exc: ast.Call, func: ast.Name) -> None:
         if len(exc.args):
             first_arg, *_ = exc.args
             is_constant_str = isinstance(first_arg, ast.Constant) and isinstance(
                 first_arg.value, str
             )
 
             WHITESPACE = " "
-            if is_constant_str and WHITESPACE in first_arg.value:
+            if is_constant_str and WHITESPACE in first_arg.value:  # type: ignore
                 self._mark_violation(node)
 
 
 class CallAvoidCheckingToContinueAnalyzer(BaseAnalyzer):
     EXPERIMENTAL = True
     violation_code = codes.CHECK_TO_CONTINUE
 
     def __init__(self):
         self.assignments_from_calls: Dict[str, ast.Assign] = {}
         super().__init__()
 
-    def _scan_assignments(self, node: StmtBodyProtocol):
+    def _scan_assignments(self, node: StmtBodyProtocol) -> None:
         def is_assigned_from_call(node: ast.stmt) -> bool:
             if isinstance(node, ast.Assign):
                 if isinstance(node.value, ast.Call):
                     return True
                 else:
                     if hasattr(node.targets[0], "id"):
-                        self.assignments_from_calls.pop(node.targets[0].id, None)
+                        self.assignments_from_calls.pop(node.targets[0].id, None)  # type: ignore
             return False
 
         raw_assignments = [stm for stm in node.body if is_assigned_from_call(stm)]
         # TODO: What if there's more targets?
         assignments = {
-            raw.targets[0].id: raw for raw in raw_assignments if hasattr(raw.targets[0], "id")
+            raw.targets[0].id: raw  # type: ignore
+            for raw in raw_assignments
+            if hasattr(raw.targets[0], "id")  # type: ignore
         }
         self.assignments_from_calls.update(assignments)
 
-    def _find_violations(self, node: StmtBodyProtocol):
+    def _find_violations(self, node: StmtBodyProtocol) -> None:
         code, rawmsg = codes.CHECK_TO_CONTINUE
 
-        def is_if_returning(node: ast.stmt) -> bool:
+        def is_if_returning(node: Union[ast.stmt, StmtBodyProtocol]) -> bool:
             if isinstance(node, ast.If):
                 for child in node.body:
                     if isinstance(child, ast.Return):
                         return True
             return False
 
         ifs_stmt = [stm for stm in node.body if is_if_returning(stm)]
         if is_if_returning(node):
-            ifs_stmt.append(node)
+            ifs_stmt.append(cast(ast.stmt, node))
 
         for if_stmt in ifs_stmt:
-            test = if_stmt.test
+            test = if_stmt.test  # type: ignore
             if isinstance(test, ast.Name):
                 if assignment := self.assignments_from_calls.get(test.id):
-                    if hasattr(assignment.value.func, "id"):
-                        callable_name = assignment.value.func.id
+                    if hasattr(assignment.value.func, "id"):  # type: ignore
+                        callable_name = assignment.value.func.id  # type: ignore
                         msg = rawmsg.format(callable_name)
                         self.violations.append(
                             Violation(
                                 code,
                                 if_stmt.lineno,
                                 if_stmt.col_offset,
                                 msg,
                                 self.filename,
                                 if_stmt,
                             )
                         )
             elif isinstance(test, ast.UnaryOp):
                 if isinstance(test.operand, ast.Name):
                     if assignment := self.assignments_from_calls.get(test.operand.id):
-                        if hasattr(assignment.value.func, "id"):
-                            callable_name = assignment.value.func.id
+                        if hasattr(assignment.value.func, "id"):  # type: ignore
+                            callable_name = assignment.value.func.id  # type: ignore
                             msg = rawmsg.format(callable_name)
                             self.violations.append(
                                 Violation(
                                     code,
                                     if_stmt.lineno,
                                     if_stmt.col_offset,
                                     msg,
                                     self.filename,
                                     if_stmt,
                                 )
                             )
 
-    def _scan_deeper(self, node: StmtBodyProtocol, may_contain_violations: bool):
+    def _scan_deeper(self, node: StmtBodyProtocol, may_contain_violations: bool) -> None:
         self._scan_assignments(node)
 
         if may_contain_violations:
             self._find_violations(node)
         else:
             if node.body:
                 *_, last_stm = node.body
                 if isinstance(last_stm, ast.Return):
                     may_contain_violations = True
 
         for child in node.body:
             if hasattr(child, "body"):
-                self._scan_deeper(child, may_contain_violations)
+                self._scan_deeper(cast(StmtBodyProtocol, child), may_contain_violations)
 
     def check(self, tree: ast.AST, filename: str) -> List[Violation]:
         self.filename = filename
         self.violations = []
 
         for node in ast.walk(tree):
             if isinstance(node, ast.Module):
```

### Comparing `tryceratops-1.1.0/src/tryceratops/analyzers/conditional.py` & `tryceratops-1.2.0/src/tryceratops/analyzers/conditional.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             if isinstance(node.exc.func, ast.Name):
                 if node.exc.func.id in STANDARD_NON_TYPE_ERROR_IDS:
                     self._mark_violation(node.exc.func)
         elif isinstance(node.exc, ast.Name):
             if node.exc.id in STANDARD_NON_TYPE_ERROR_IDS:
                 self._mark_violation(node.exc)
 
-    def _check_for_raises(self, node):
+    def _check_for_raises(self, node: ast.stmt) -> None:
         for stm in ast.iter_child_nodes(node):
             if isinstance(stm, ast.Raise):
                 self._check_is_raise_other_than_typeerror(stm)
         if isinstance(node, ast.If):
             for stm in node.orelse:
                 self._check_for_raises(stm)
```

### Comparing `tryceratops-1.1.0/src/tryceratops/analyzers/exception_block.py` & `tryceratops-1.2.0/src/tryceratops/analyzers/exception_block.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class ExceptReraiseWithoutCauseAnalyzer(BaseAnalyzer):
     violation_code = codes.RERAISE_NO_CAUSE
     violation_type = RaiseWithoutCauseViolation
 
     @visit_error_handler
     def visit_ExceptHandler(self, node: ast.ExceptHandler) -> None:
-        def is_raise_without_cause(node: ast.AST):
+        def is_raise_without_cause(node: ast.AST) -> bool:
             if isinstance(node, ast.Raise):
                 return isinstance(node.exc, ast.Call) and node.cause is None
             return False
 
         reraises_no_cause = [stm for stm in ast.walk(node) if is_raise_without_cause(stm)]
         self._mark_violation(*reraises_no_cause, exception_name=node.name, except_node=node)
 
@@ -25,15 +25,15 @@
 
 class ExceptVerboseReraiseAnalyzer(BaseAnalyzer):
     violation_code = codes.VERBOSE_RERAISE
     violation_type = VerboseReraiseViolation
 
     @visit_error_handler
     def visit_ExceptHandler(self, node: ast.ExceptHandler) -> None:
-        def is_raise_with_name(stm: ast.AST, name: str):
+        def is_raise_with_name(stm: ast.AST, name: str) -> bool:
             if isinstance(stm, ast.Raise) and isinstance(stm.exc, ast.Name):
                 return stm.exc.id == name
             return False
 
         # If no name is set, then it's impossible to be verbose
         # since you don't have the object
         if node.name:
@@ -118,21 +118,21 @@
     def _has_object_reference(self, node: ast.AST) -> bool:
         if isinstance(node, ast.Name):
             if node.id == self.exception_object_name:
                 return True
 
         return False
 
-    def _check_args(self, log_args: Iterable[ast.AST]):
+    def _check_args(self, log_args: Iterable[ast.AST]) -> None:
         for arg in log_args:
             for node in ast.walk(arg):
                 if self._has_object_reference(node):
                     self._mark_violation(node)
 
-    def _find_violations(self, node: ast.ExceptHandler):
+    def _find_violations(self, node: ast.ExceptHandler) -> None:
         for stm in ast.walk(node):
             if possible_log_wrap := self._maybe_get_possible_log_wrap(stm):
                 possible_log_node = possible_log_wrap.func
 
                 if isinstance(possible_log_node, ast.Attribute):
                     object_method = possible_log_node.attr
```

### Comparing `tryceratops-1.1.0/src/tryceratops/analyzers/try_block.py` & `tryceratops-1.2.0/src/tryceratops/analyzers/try_block.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,16 +10,19 @@
     violation_code = codes.CONSIDER_ELSE
 
     @visit_error_handler
     def visit_Try(self, node: ast.Try) -> None:
         *_, last_child = node.body
         theres_more_children = len(node.body) > 1
 
-        if isinstance(last_child, ast.Return) and theres_more_children:
-            self._mark_violation(last_child)
+        has_except_block = bool(node.handlers)
+
+        if has_except_block:
+            if isinstance(last_child, ast.Return) and theres_more_children:
+                self._mark_violation(last_child)
 
         self.generic_visit(node)
 
 
 class TryShouldntRaiseAnalyzer(BaseAnalyzer):
     violation_code = codes.RAISE_WITHIN_TRY
```

### Comparing `tryceratops-1.1.0/src/tryceratops/files/discovery.py` & `tryceratops-1.2.0/src/tryceratops/files/discovery.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from tryceratops.types import ParsedFileType, PyprojectConfig
 
 from .parser import parse_file
 
 logger = logging.getLogger(__name__)
 
 
-def is_python_file(filename: str):
+def is_python_file(filename: str) -> bool:
     return isfile(filename) and filename.endswith(".py")
 
 
 def find_files(dir: str) -> Generator[str, None, None]:
     files = listdir(dir)
     for entry in files:
         full_path = join(dir, entry)
```

### Comparing `tryceratops-1.1.0/src/tryceratops/files/parser.py` & `tryceratops-1.2.0/src/tryceratops/files/parser.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.1.0/src/tryceratops/filters.py` & `tryceratops-1.2.0/src/tryceratops/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 @dataclass
 class FileFilter:
     """Represents a filter applied to a single file"""
 
     ignore_lines: Iterable[IgnoreViolation]
 
-    def ignores_violation(self, violation: Violation):
+    def ignores_violation(self, violation: Violation) -> bool:
         for line in self.ignore_lines:
             if line.is_ignoring(violation.line, violation.code):
                 return True
 
         return False
 
 
@@ -52,15 +52,15 @@
     """
 
     include_experimental: bool
     ignore_violations: Iterable[str]
     exclude_dirs: Iterable[str]
     autofix: bool = False
 
-    def _self_check(self):
+    def _self_check(self) -> None:
         self.exclude_dirs = [excluded for excluded in self.exclude_dirs if excluded]
 
     def __post_init__(self):
         self._self_check()
 
     @property
     def exclude_experimental(self) -> bool:
@@ -93,15 +93,15 @@
 
     def overwrite_from_cli(
         self,
         include_experimental: bool,
         ignore_violations: Iterable[str],
         exclude_dirs: Iterable[str],
         autofix: bool,
-    ):
+    ) -> None:
         """In case any value is set it overwrites the previous value"""
         if include_experimental:
             self.include_experimental = include_experimental
 
         if ignore_violations:
             self.ignore_violations = ignore_violations
```

### Comparing `tryceratops-1.1.0/src/tryceratops/fixers/__init__.py` & `tryceratops-1.2.0/src/tryceratops/fixers/__init__.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.1.0/src/tryceratops/fixers/base.py` & `tryceratops-1.2.0/src/tryceratops/fixers/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import ABC, abstractmethod
 from collections import defaultdict
-from typing import Dict, Generic, Iterable, List, TypeVar
+from types import TracebackType
+from typing import Dict, Generic, Iterable, List, Optional, Type, TypeVar
 
 from tryceratops.processors import Processor
 from tryceratops.violations import Violation
 
 from .exceptions import FixerFixException
 
 ViolationType = TypeVar("ViolationType", bound=Violation)
@@ -19,20 +20,25 @@
         return self
 
     def read_lines(self) -> Iterable[str]:
         lines = self.file.readlines()
         self.file.seek(0)
         return lines
 
-    def write_fix(self, new_lines: Iterable[str]):
+    def write_fix(self, new_lines: Iterable[str]) -> None:
         self.file.writelines(new_lines)
         self.file.truncate()
         self.file.seek(0)
 
-    def __exit__(self, exc_type, exc_value, exc_traceback):
+    def __exit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> None:
         self.file.close()
 
 
 class BaseFixer(ABC, Processor, Generic[ViolationType]):
     fixes_made = 0
 
     def _filter_violations_in_scope(self, violations: List[Violation]) -> List[Violation]:
@@ -43,15 +49,15 @@
     def _group_violations_by_filename(self, violations: List[Violation]) -> GroupedViolations:
         group: GroupedViolations = defaultdict(list)
         for violation in violations:
             group[violation.filename].append(violation)
 
         return group
 
-    def _process_group(self, filename: str, violations: List[ViolationType]):
+    def _process_group(self, filename: str, violations: List[ViolationType]) -> None:
         with FileFixerHandler(filename) as file:
             for violation in violations:
                 try:
                     file_lines = file.read_lines()
                     resulting_lines = self.perform_fix(file_lines, violation)
                     file.write_fix(resulting_lines)
                 except Exception as ex:
@@ -59,13 +65,13 @@
                 else:
                     self.fixes_made += 1
 
     @abstractmethod
     def perform_fix(self, lines: List[str], violation: ViolationType) -> List[str]:
         pass
 
-    def fix(self, violations: List[Violation]):
+    def fix(self, violations: List[Violation]) -> None:
         relevant_violations = self._filter_violations_in_scope(violations)
         grouped = self._group_violations_by_filename(relevant_violations)
 
         for filename, file_violations in grouped.items():
             self._process_group(filename, file_violations)
```

### Comparing `tryceratops-1.1.0/src/tryceratops/fixers/exception_block.py` & `tryceratops-1.2.0/src/tryceratops/fixers/exception_block.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,27 +25,27 @@
         return all_lines
 
 
 class RaiseWithoutCauseFixer(BaseFixer[RaiseWithoutCauseViolation]):
     violation_code = codes.RERAISE_NO_CAUSE
     exception_name_to_create = "ex"
 
-    def _fix_except_handler(self, all_lines: List[str], offending_node: ast.ExceptHandler):
+    def _fix_except_handler(self, all_lines: List[str], offending_node: ast.ExceptHandler) -> None:
         line_offset = offending_node.lineno - 1
         offending_line = all_lines[line_offset]
 
         new_line = re.sub(
             r"except (.*):", rf"except \1 as {self.exception_name_to_create}:", offending_line
         )
 
         all_lines[line_offset] = new_line
 
     def _fix_raise_no_cause(
         self, all_lines: List[str], violation: RaiseWithoutCauseViolation, exception_name: str
-    ):
+    ) -> None:
         endline = violation.node.end_lineno or violation.line
         is_singleline = violation.line == endline
 
         if is_singleline:
             fix_offset = violation.line - 1
             guilty_line = all_lines[fix_offset]
             new_line = re.sub(r"raise (.*)", rf"raise \1 from {exception_name}", guilty_line)
```

### Comparing `tryceratops-1.1.0/src/tryceratops/flake_plugin.py` & `tryceratops-1.2.0/src/tryceratops/flake_plugin.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.1.0/src/tryceratops/interfaces.py` & `tryceratops-1.2.0/src/tryceratops/interfaces.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 class ExitCodes(IntEnum):
     SUCCESS = 0
     LINT_BROKEN = 1
     UNPROCESSED_FILE = 2
     RUNTIME_ISSUES = 100
 
 
-def present_violation(violation: Violation):
+def present_violation(violation: Violation) -> str:
     codestr = violation.code
     descstr = violation.description
     location = f"{violation.filename}:{violation.line}:{violation.col}"
 
     return f"[[yellow]{codestr}[/yellow]] [red]{descstr}[/red] - {location}"
 
 
 class CliInterface:
     def __init__(self, runner: Runner, discovery: FileDiscovery):
         self.runner = runner
         self.discovery = discovery
 
-    def _present_violations(self):
+    def _present_violations(self) -> None:
         for violation in self.runner.violations:
             print(present_violation(violation))
 
-    def _present_status(self):
+    def _present_status(self) -> None:
         print("Done processing!")
 
         if self.runner.analyzed_files:
             print(f"Processed {self.runner.analyzed_files} files")
 
             if self.runner.violations:
                 print(f"Found {len(self.runner.violations)} violations")
@@ -59,33 +59,33 @@
 
         if self.runner.had_issues:
             print(
                 f"Had {len(self.runner.runtime_errors)} unexpected issues "
                 f"stored in {ERROR_LOG_FILENAME}"
             )
 
-    def _exit(self):
+    def _exit(self) -> None:
         exit_code = ExitCodes.SUCCESS
 
         if self.runner.had_issues:
             exit_code = ExitCodes.RUNTIME_ISSUES
         elif self.discovery.had_issues:
             exit_code = ExitCodes.UNPROCESSED_FILE
         elif self.runner.any_violation:
             exit_code = ExitCodes.LINT_BROKEN
 
         sys.exit(exit_code)
 
-    def _delete_empty_logs(self):
+    def _delete_empty_logs(self) -> None:
         cwd = os.getcwd()
         log_file_path = f"{cwd}/{ERROR_LOG_FILENAME}"
         is_log_empty = os.path.getsize(log_file_path) == 0
 
         if is_log_empty:
             os.remove(log_file_path)
 
-    def present_and_exit(self):
+    def present_and_exit(self) -> None:
         logging.shutdown()
         self._present_violations()
         self._present_status()
         self._delete_empty_logs()
         self._exit()
```

### Comparing `tryceratops-1.1.0/src/tryceratops/runners.py` & `tryceratops-1.2.0/src/tryceratops/runners.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,22 +24,22 @@
     def __init__(self):
         self.runtime_errors: List[RuntimeError] = []
         self.violations: List[Violation] = []
         self.analyzed_files = 0
         self.excluded_files = 0
         self.fixed_violations = 0
 
-    def _clear(self):
+    def _clear(self) -> None:
         self.violations = []
         self.runtime_errors = []
         self.excluded_files = 0
 
     def _run_analyzers(
         self, analyzers: Set[BaseAnalyzer], filename: str, filefilter: FileFilter, tree: ast.AST
-    ):
+    ) -> None:
         for analyzer in analyzers:
             try:
                 found_violations = analyzer.check(tree, filename)
                 valid_violations = [
                     violation
                     for violation in found_violations
                     if not filefilter.ignores_violation(violation)
@@ -48,15 +48,15 @@
                 logger.exception(
                     f"Exception raised when running Analyzer: {type(analyzer)} on {filename}"
                 )
                 self.runtime_errors.append(RuntimeError(filename, type(analyzer), ex))
             else:
                 self.violations += valid_violations
 
-    def _run_fixers(self, fixers: Set[BaseFixer]):
+    def _run_fixers(self, fixers: Set[BaseFixer]) -> None:
         for fixer in fixers:
             try:
                 fixer.fix(self.violations)
             except Exception as ex:
                 logger.exception(f"Exception raised when running Fixer: {type(fixer)}")
                 self.runtime_errors.append(RuntimeError("unknown", type(fixer), ex))
             else:
```

### Comparing `tryceratops-1.1.0/src/tryceratops/settings.py` & `tryceratops-1.2.0/src/tryceratops/settings.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.1.0/src/tryceratops/types.py` & `tryceratops-1.2.0/src/tryceratops/types.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.1.0/src/tryceratops/violations/codes.py` & `tryceratops-1.2.0/src/tryceratops/violations/codes.py`

 * *Files identical despite different names*

### Comparing `tryceratops-1.1.0/setup.py` & `tryceratops-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,471 +1,459 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 655f 6469  etup..package_di
-00000040: 7220 3d20 5c0a 7b27 273a 2027 7372 6327  r = \.{'': 'src'
-00000050: 7d0a 0a70 6163 6b61 6765 7320 3d20 5c0a  }..packages = \.
-00000060: 5b27 7472 7963 6572 6174 6f70 7327 2c0a  ['tryceratops',.
-00000070: 2027 7472 7963 6572 6174 6f70 732e 616e   'tryceratops.an
-00000080: 616c 797a 6572 7327 2c0a 2027 7472 7963  alyzers',. 'tryc
-00000090: 6572 6174 6f70 732e 6669 6c65 7327 2c0a  eratops.files',.
-000000a0: 2027 7472 7963 6572 6174 6f70 732e 6669   'tryceratops.fi
-000000b0: 7865 7273 272c 0a20 2774 7279 6365 7261  xers',. 'trycera
-000000c0: 746f 7073 2e76 696f 6c61 7469 6f6e 7327  tops.violations'
-000000d0: 5d0a 0a70 6163 6b61 6765 5f64 6174 6120  ]..package_data 
-000000e0: 3d20 5c0a 7b27 273a 205b 272a 275d 7d0a  = \.{'': ['*']}.
-000000f0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-00000100: 7320 3d20 5c0a 5b27 636c 6963 6b3e 3d37  s = \.['click>=7
-00000110: 272c 2027 7269 6368 3e3d 3130 2e31 342e  ', 'rich>=10.14.
-00000120: 3027 2c20 2774 6f6d 6c3e 3d30 2e31 302e  0', 'toml>=0.10.
-00000130: 3227 5d0a 0a65 6e74 7279 5f70 6f69 6e74  2']..entry_point
-00000140: 7320 3d20 5c0a 7b27 636f 6e73 6f6c 655f  s = \.{'console_
-00000150: 7363 7269 7074 7327 3a20 5b27 7472 7963  scripts': ['tryc
-00000160: 6572 6174 6f70 7320 3d20 7472 7963 6572  eratops = trycer
-00000170: 6174 6f70 732e 5f5f 6d61 696e 5f5f 3a6d  atops.__main__:m
-00000180: 6169 6e27 5d2c 0a20 2766 6c61 6b65 382e  ain'],. 'flake8.
-00000190: 6578 7465 6e73 696f 6e27 3a20 5b27 5443  extension': ['TC
-000001a0: 203d 2074 7279 6365 7261 746f 7073 2e66   = tryceratops.f
-000001b0: 6c61 6b65 5f70 6c75 6769 6e3a 5472 7963  lake_plugin:Tryc
-000001c0: 6572 6174 6f70 7341 6461 7074 6572 506c  eratopsAdapterPl
-000001d0: 7567 696e 275d 7d0a 0a73 6574 7570 5f6b  ugin']}..setup_k
-000001e0: 7761 7267 7320 3d20 7b0a 2020 2020 276e  wargs = {.    'n
-000001f0: 616d 6527 3a20 2774 7279 6365 7261 746f  ame': 'trycerato
-00000200: 7073 272c 0a20 2020 2027 7665 7273 696f  ps',.    'versio
-00000210: 6e27 3a20 2731 2e31 2e30 272c 0a20 2020  n': '1.1.0',.   
-00000220: 2027 6465 7363 7269 7074 696f 6e27 3a20   'description': 
-00000230: 2741 206c 696e 7465 7220 746f 206d 616e  'A linter to man
-00000240: 6167 6520 796f 7572 2065 7863 6570 7469  age your excepti
-00000250: 6f6e 206c 696b 6520 6120 5052 4f21 272c  on like a PRO!',
-00000260: 0a20 2020 2027 6c6f 6e67 5f64 6573 6372  .    'long_descr
-00000270: 6970 7469 6f6e 273a 2027 3c70 2061 6c69  iption': '<p ali
-00000280: 676e 3d22 6365 6e74 6572 223e 5c6e 2020  gn="center">\n  
-00000290: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-000002a0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-000002b0: 6572 636f 6e74 656e 742e 636f 6d2f 6775  ercontent.com/gu
-000002c0: 696c 6174 726f 7661 2f74 7279 6365 7261  ilatrova/trycera
-000002d0: 746f 7073 2f6d 6169 6e2f 696d 672f 6c6f  tops/main/img/lo
-000002e0: 676f 2e70 6e67 223e 5c6e 3c2f 703e 5c6e  go.png">\n</p>\n
-000002f0: 5c6e 3c68 3220 616c 6967 6e3d 2263 656e  \n<h2 align="cen
-00000300: 7465 7222 3e50 7265 7665 6e74 2045 7863  ter">Prevent Exc
-00000310: 6570 7469 6f6e 2048 616e 646c 696e 6720  eption Handling 
-00000320: 416e 7469 5061 7474 6572 6e73 2069 6e20  AntiPatterns in 
-00000330: 5079 7468 6f6e 3c2f 6832 3e5c 6e5c 6e3c  Python</h2>\n\n<
-00000340: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
-00000350: 3e5c 6e20 203c 6120 6872 6566 3d22 6874  >\n  <a href="ht
-00000360: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000370: 2f67 7569 6c61 7472 6f76 612f 7472 7963  /guilatrova/tryc
-00000380: 6572 6174 6f70 732f 6163 7469 6f6e 7322  eratops/actions"
-00000390: 3e3c 696d 6720 616c 743d 2241 6374 696f  ><img alt="Actio
-000003a0: 6e73 2053 7461 7475 7322 2073 7263 3d22  ns Status" src="
-000003b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000003c0: 6f6d 2f67 7569 6c61 7472 6f76 612f 7472  om/guilatrova/tr
-000003d0: 7963 6572 6174 6f70 732f 776f 726b 666c  yceratops/workfl
-000003e0: 6f77 732f 4349 2f62 6164 6765 2e73 7667  ows/CI/badge.svg
-000003f0: 223e 3c2f 613e 5c6e 2020 3c61 2068 7265  "></a>\n  <a hre
-00000400: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
-00000410: 6f72 672f 7072 6f6a 6563 742f 7472 7963  org/project/tryc
-00000420: 6572 6174 6f70 732f 223e 3c69 6d67 2061  eratops/"><img a
-00000430: 6c74 3d22 5079 5049 2220 7372 633d 2268  lt="PyPI" src="h
-00000440: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000450: 6473 2e69 6f2f 7079 7069 2f76 2f74 7279  ds.io/pypi/v/try
-00000460: 6365 7261 746f 7073 222f 3e3c 2f61 3e5c  ceratops"/></a>\
-00000470: 6e20 203c 696d 6720 7372 633d 2268 7474  n  <img src="htt
-00000480: 7073 3a2f 2f62 6164 6765 6e2e 6e65 742f  ps://badgen.net/
-00000490: 7079 7069 2f70 7974 686f 6e2f 7472 7963  pypi/python/tryc
-000004a0: 6572 6174 6f70 7322 202f 3e5c 6e20 203c  eratops" />\n  <
-000004b0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000004c0: 6769 7468 7562 2e63 6f6d 2f72 656c 656b  github.com/relek
-000004d0: 616e 672f 7079 7468 6f6e 2d73 656d 616e  ang/python-seman
-000004e0: 7469 632d 7265 6c65 6173 6522 3e3c 696d  tic-release"><im
-000004f0: 6720 616c 743d 2253 656d 616e 7469 6320  g alt="Semantic 
-00000500: 5265 6c65 6173 6522 2073 7263 3d22 6874  Release" src="ht
-00000510: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000520: 732e 696f 2f62 6164 6765 2f25 3230 2532  s.io/badge/%20%2
-00000530: 3025 4630 2539 4625 3933 2541 3625 4630  0%F0%9F%93%A6%F0
-00000540: 2539 4625 3941 2538 302d 7365 6d61 6e74  %9F%9A%80-semant
-00000550: 6963 2d2d 7265 6c65 6173 652d 6531 3030  ic--release-e100
-00000560: 3739 2e73 7667 223e 3c2f 613e 5c6e 2020  79.svg"></a>\n  
-00000570: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000580: 2f67 6974 6875 622e 636f 6d2f 6775 696c  /github.com/guil
-00000590: 6174 726f 7661 2f74 7279 6365 7261 746f  atrova/trycerato
-000005a0: 7073 2f62 6c6f 622f 6d61 696e 2f4c 4943  ps/blob/main/LIC
-000005b0: 454e 5345 223e 3c69 6d67 2061 6c74 3d22  ENSE"><img alt="
-000005c0: 4769 7448 7562 2220 7372 633d 2268 7474  GitHub" src="htt
-000005d0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000005e0: 2e69 6f2f 6769 7468 7562 2f6c 6963 656e  .io/github/licen
-000005f0: 7365 2f67 7569 6c61 7472 6f76 612f 7472  se/guilatrova/tr
-00000600: 7963 6572 6174 6f70 7322 2f3e 3c2f 613e  yceratops"/></a>
-00000610: 5c6e 2020 3c61 2068 7265 663d 2268 7474  \n  <a href="htt
-00000620: 7073 3a2f 2f70 6570 792e 7465 6368 2f70  ps://pepy.tech/p
-00000630: 726f 6a65 6374 2f74 7279 6365 7261 746f  roject/trycerato
-00000640: 7073 2f22 3e3c 696d 6720 616c 743d 2244  ps/"><img alt="D
-00000650: 6f77 6e6c 6f61 6473 2220 7372 633d 2268  ownloads" src="h
-00000660: 7474 7073 3a2f 2f73 7461 7469 632e 7065  ttps://static.pe
-00000670: 7079 2e74 6563 682f 7065 7273 6f6e 616c  py.tech/personal
-00000680: 697a 6564 2d62 6164 6765 2f74 7279 6365  ized-badge/tryce
-00000690: 7261 746f 7073 3f70 6572 696f 643d 746f  ratops?period=to
-000006a0: 7461 6c26 756e 6974 733d 696e 7465 726e  tal&units=intern
-000006b0: 6174 696f 6e61 6c5f 7379 7374 656d 266c  ational_system&l
-000006c0: 6566 745f 636f 6c6f 723d 6772 6579 2672  eft_color=grey&r
-000006d0: 6967 6874 5f63 6f6c 6f72 3d62 6c75 6526  ight_color=blue&
-000006e0: 6c65 6674 5f74 6578 743d 2546 3025 3946  left_text=%F0%9F
-000006f0: 2541 3625 3936 2532 3044 6f77 6e6c 6f61  %A6%96%20Downloa
-00000700: 6473 222f 3e3c 2f61 3e5c 6e20 203c 6120  ds"/></a>\n  <a 
-00000710: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00000720: 7468 7562 2e63 6f6d 2f70 7366 2f62 6c61  thub.com/psf/bla
-00000730: 636b 223e 3c69 6d67 2061 6c74 3d22 436f  ck"><img alt="Co
-00000740: 6465 2073 7479 6c65 3a20 626c 6163 6b22  de style: black"
-00000750: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00000760: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000770: 6765 2f63 6f64 6525 3230 7374 796c 652d  ge/code%20style-
-00000780: 626c 6163 6b2d 3030 3030 3030 2e73 7667  black-000000.svg
-00000790: 222f 3e3c 2f61 3e5c 6e20 203c 6120 6872  "/></a>\n  <a hr
-000007a0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-000007b0: 7562 2e63 6f6d 2f67 7569 6c61 7472 6f76  ub.com/guilatrov
-000007c0: 612f 7472 7963 6572 6174 6f70 7322 3e3c  a/tryceratops"><
-000007d0: 696d 6720 616c 743d 2274 7279 2f65 7863  img alt="try/exc
-000007e0: 6570 7420 7374 796c 653a 2074 7279 6365  ept style: tryce
-000007f0: 7261 746f 7073 2220 7372 633d 2268 7474  ratops" src="htt
-00000800: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000810: 2e69 6f2f 6261 6467 652f 7472 7925 3246  .io/badge/try%2F
-00000820: 6578 6365 7074 2532 3073 7479 6c65 2d74  except%20style-t
-00000830: 7279 6365 7261 746f 7073 2532 3025 4630  ryceratops%20%F0
-00000840: 2539 4625 4136 2539 3625 4532 2539 4325  %9F%A6%96%E2%9C%
-00000850: 4138 2d62 6c61 636b 2220 2f3e 3c2f 613e  A8-black" /></a>
-00000860: 5c6e 2020 3c61 2068 7265 663d 2268 7474  \n  <a href="htt
-00000870: 7073 3a2f 2f6f 7065 6e2e 7673 636f 6465  ps://open.vscode
-00000880: 2e64 6576 2f67 7569 6c61 7472 6f76 612f  .dev/guilatrova/
-00000890: 7472 7963 6572 6174 6f70 7322 3e3c 696d  tryceratops"><im
-000008a0: 6720 616c 743d 224f 7065 6e20 696e 2056  g alt="Open in V
-000008b0: 6973 7561 6c20 5374 7564 696f 2043 6f64  isual Studio Cod
-000008c0: 6522 2073 7263 3d22 6874 7470 733a 2f2f  e" src="https://
-000008d0: 6f70 656e 2e76 7363 6f64 652e 6465 762f  open.vscode.dev/
-000008e0: 6261 6467 6573 2f6f 7065 6e2d 696e 2d76  badges/open-in-v
-000008f0: 7363 6f64 652e 7376 6722 2f3e 3c2f 613e  scode.svg"/></a>
-00000900: 5c6e 2020 3c61 2068 7265 663d 2268 7474  \n  <a href="htt
-00000910: 7073 3a2f 2f74 7769 7474 6572 2e63 6f6d  ps://twitter.com
-00000920: 2f69 6e74 656e 742f 7573 6572 3f73 6372  /intent/user?scr
-00000930: 6565 6e5f 6e61 6d65 3d67 7569 6c61 7472  een_name=guilatr
-00000940: 6f76 6122 3e3c 696d 6720 616c 743d 2246  ova"><img alt="F
-00000950: 6f6c 6c6f 7720 6775 696c 6174 726f 7661  ollow guilatrova
-00000960: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-00000970: 6d67 2e73 6869 656c 6473 2e69 6f2f 7477  mg.shields.io/tw
-00000980: 6974 7465 722f 666f 6c6c 6f77 2f67 7569  itter/follow/gui
-00000990: 6c61 7472 6f76 613f 7374 796c 653d 736f  latrova?style=so
-000009a0: 6369 616c 222f 3e3c 2f61 3e5c 6e3c 2f70  cial"/></a>\n</p
-000009b0: 3e5c 6e5c 6e49 6e73 7069 7265 6420 6279  >\n\nInspired by
-000009c0: 205b 7468 6973 2062 6c6f 6720 706f 7374   [this blog post
-000009d0: 5d28 6874 7470 733a 2f2f 626c 6f67 2e67  ](https://blog.g
-000009e0: 7569 6c61 7472 6f76 612e 6465 762f 6861  uilatrova.dev/ha
-000009f0: 6e64 6c69 6e67 2d65 7863 6570 7469 6f6e  ndling-exception
-00000a00: 732d 696e 2d70 7974 686f 6e2d 6c69 6b65  s-in-python-like
-00000a10: 2d61 2d70 726f 2f29 2e20 4920 6465 7363  -a-pro/). I desc
-00000a20: 7269 6265 6420 5b74 6865 2062 7569 6c64  ribed [the build
-00000a30: 696e 6720 7072 6f63 6573 7320 6f66 2074  ing process of t
-00000a40: 6869 7320 746f 6f6c 2068 6572 655d 2868  his tool here](h
-00000a50: 7474 7073 3a2f 2f62 6c6f 672e 6775 696c  ttps://blog.guil
-00000a60: 6174 726f 7661 2e64 6576 2f70 726f 6a65  atrova.dev/proje
-00000a70: 6374 2d74 7279 6365 7261 746f 7073 2f29  ct-tryceratops/)
-00000a80: 2e5c 6e5c 6e3e 20e2 809c 466f 7220 7468  .\n\n> ...For th
-00000a90: 6f73 6520 7768 6f20 6c69 6b65 2064 696e  ose who like din
-00000aa0: 6f73 6175 7273 20f0 9fa6 9620 616e 6420  osaurs .... and 
-00000ab0: 636c 6561 6e20 7472 792f 6578 6365 7074  clean try/except
-00000ac0: 20e2 9ca8 2062 6c6f 636b 732e e280 9d5c   ... blocks....\
-00000ad0: 6e5c 6e2a 2a53 756d 6d61 7279 2a2a 5c6e  n\n**Summary**\n
-00000ae0: 2d20 5b49 6e73 7461 6c6c 6174 696f 6e20  - [Installation 
-00000af0: 616e 6420 7573 6167 655d 2823 696e 7374  and usage](#inst
-00000b00: 616c 6c61 7469 6f6e 2d61 6e64 2d75 7361  allation-and-usa
-00000b10: 6765 295c 6e20 202d 205b 496e 7374 616c  ge)\n  - [Instal
-00000b20: 6c61 7469 6f6e 5d28 2369 6e73 7461 6c6c  lation](#install
-00000b30: 6174 696f 6e29 5c6e 2020 2d20 5b55 7361  ation)\n  - [Usa
-00000b40: 6765 5d28 2375 7361 6765 295c 6e20 202d  ge](#usage)\n  -
-00000b50: 205b 6066 6c61 6b65 3860 2050 6c75 6769   [`flake8` Plugi
-00000b60: 6e5d 2823 666c 616b 6538 2d70 6c75 6769  n](#flake8-plugi
-00000b70: 6e29 5c6e 2d20 5b56 696f 6c61 7469 6f6e  n)\n- [Violation
-00000b80: 735d 2823 7669 6f6c 6174 696f 6e73 295c  s](#violations)\
-00000b90: 6e20 202d 205b 4175 746f 6669 7820 7375  n  - [Autofix su
-00000ba0: 7070 6f72 745d 2823 6175 746f 6669 782d  pport](#autofix-
-00000bb0: 7375 7070 6f72 7429 5c6e 2020 2d20 5b49  support)\n  - [I
-00000bc0: 676e 6f72 696e 6720 7669 6f6c 6174 696f  gnoring violatio
-00000bd0: 6e73 5d28 2369 676e 6f72 696e 672d 7669  ns](#ignoring-vi
-00000be0: 6f6c 6174 696f 6e73 295c 6e20 202d 205b  olations)\n  - [
-00000bf0: 436f 6e66 6967 7572 6174 696f 6e5d 2823  Configuration](#
-00000c00: 636f 6e66 6967 7572 6174 696f 6e29 5c6e  configuration)\n
-00000c10: 2d20 5b50 7265 2d63 6f6d 6d69 745d 2823  - [Pre-commit](#
-00000c20: 7072 652d 636f 6d6d 6974 295c 6e2d 205b  pre-commit)\n- [
-00000c30: 5368 6f77 2079 6f75 7220 7374 796c 655d  Show your style]
-00000c40: 2823 7368 6f77 2d79 6f75 722d 7374 796c  (#show-your-styl
-00000c50: 6529 5c6e 2d20 5b45 7874 7261 2052 6573  e)\n- [Extra Res
-00000c60: 6f75 7263 6573 5d28 2365 7874 7261 2d72  ources](#extra-r
-00000c70: 6573 6f75 7263 6573 295c 6e2d 205b 436f  esources)\n- [Co
-00000c80: 6e74 7269 6275 7469 6e67 5d28 2363 6f6e  ntributing](#con
-00000c90: 7472 6962 7574 696e 6729 5c6e 2d20 5b43  tributing)\n- [C
-00000ca0: 6861 6e67 6520 6c6f 675d 2823 6368 616e  hange log](#chan
-00000cb0: 6765 2d6c 6f67 295c 6e2d 205b 4c69 6365  ge-log)\n- [Lice
-00000cc0: 6e73 655d 2823 6c69 6365 6e73 6529 5c6e  nse](#license)\n
-00000cd0: 2d20 5b43 7265 6469 7473 5d28 2363 7265  - [Credits](#cre
-00000ce0: 6469 7473 295c 6e5c 6e2d 2d2d 5c6e 5c6e  dits)\n\n---\n\n
-00000cf0: 2323 2049 6e73 7461 6c6c 6174 696f 6e20  ## Installation 
-00000d00: 616e 6420 7573 6167 655c 6e5c 6e23 2323  and usage\n\n###
-00000d10: 2049 6e73 7461 6c6c 6174 696f 6e5c 6e5c   Installation\n\
-00000d20: 6e60 6060 5c6e 7069 7020 696e 7374 616c  n```\npip instal
-00000d30: 6c20 7472 7963 6572 6174 6f70 735c 6e60  l tryceratops\n`
-00000d40: 6060 5c6e 5c6e 2323 2320 5573 6167 655c  ``\n\n### Usage\
-00000d50: 6e5c 6e60 6060 5c6e 7472 7963 6572 6174  n\n```\ntrycerat
-00000d60: 6f70 7320 5b66 696c 656e 616d 6520 6f72  ops [filename or
-00000d70: 2064 6972 2e2e 2e5d 5c6e 6060 605c 6e5c   dir...]\n```\n\
-00000d80: 6e59 6f75 2063 616e 2065 6e61 626c 6520  nYou can enable 
-00000d90: 6578 7065 7269 6d65 6e74 616c 2061 6e61  experimental ana
-00000da0: 6c79 7a65 7273 2062 7920 7275 6e6e 696e  lyzers by runnin
-00000db0: 673a 5c6e 5c6e 6060 605c 6e74 7279 6365  g:\n\n```\ntryce
-00000dc0: 7261 746f 7073 202d 2d65 7870 6572 696d  ratops --experim
-00000dd0: 656e 7461 6c20 5b66 696c 656e 616d 6520  ental [filename 
-00000de0: 6f72 2064 6972 2e2e 2e5d 5c6e 6060 605c  or dir...]\n```\
-00000df0: 6e5c 6e59 6f75 2063 616e 2069 676e 6f72  n\nYou can ignor
-00000e00: 6520 7370 6563 6966 6963 2076 696f 6c61  e specific viola
-00000e10: 7469 6f6e 7320 6279 2075 7369 6e67 3a20  tions by using: 
-00000e20: 602d 2d69 676e 6f72 6520 5443 5858 5860  `--ignore TCXXX`
-00000e30: 2072 6570 6561 7465 646c 793a 5c6e 5c6e   repeatedly:\n\n
-00000e40: 6060 605c 6e74 7279 6365 7261 746f 7073  ```\ntryceratops
-00000e50: 202d 2d69 676e 6f72 6520 5443 3230 3120   --ignore TC201 
-00000e60: 2d2d 6967 6e6f 7265 2054 4332 3032 205b  --ignore TC202 [
-00000e70: 6669 6c65 6e61 6d65 206f 7220 6469 722e  filename or dir.
-00000e80: 2e2e 5d5c 6e60 6060 5c6e 5c6e 596f 7520  ..]\n```\n\nYou 
-00000e90: 6361 6e20 6578 636c 7564 6520 6469 7273  can exclude dirs
-00000ea0: 2062 7920 7573 696e 673a 2060 2d2d 6578   by using: `--ex
-00000eb0: 636c 7564 6520 6469 722f 7061 7468 6020  clude dir/path` 
-00000ec0: 7265 7065 6174 6564 6c79 3a5c 6e5c 6e60  repeatedly:\n\n`
-00000ed0: 6060 5c6e 7472 7963 6572 6174 6f70 7320  ``\ntryceratops 
-00000ee0: 2d2d 6578 636c 7564 6520 7465 7374 7320  --exclude tests 
-00000ef0: 2d2d 6578 636c 7564 6520 2e76 656e 7620  --exclude .venv 
-00000f00: 5b66 696c 656e 616d 6520 6f72 2064 6972  [filename or dir
-00000f10: 2e2e 2e5d 5c6e 6060 605c 6e5c 6e59 6f75  ...]\n```\n\nYou
-00000f20: 2063 616e 2061 6c73 6f20 6175 746f 6669   can also autofi
-00000f30: 7820 736f 6d65 2076 696f 6c61 7469 6f6e  x some violation
-00000f40: 733a 5c6e 5c6e 6060 605c 6e74 7279 6365  s:\n\n```\ntryce
-00000f50: 7261 746f 7073 202d 2d61 7574 6f66 6978  ratops --autofix
-00000f60: 205b 6669 6c65 6e61 6d65 206f 7220 6469   [filename or di
-00000f70: 722e 2e2e 5d5c 6e60 6060 5c6e 5c6e 215b  r...]\n```\n\n![
-00000f80: 6578 616d 706c 655d 2868 7474 7073 3a2f  example](https:/
-00000f90: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00000fa0: 6f6e 7465 6e74 2e63 6f6d 2f67 7569 6c61  ontent.com/guila
-00000fb0: 7472 6f76 612f 7472 7963 6572 6174 6f70  trova/tryceratop
-00000fc0: 732f 6d61 696e 2f69 6d67 2f74 7279 6365  s/main/img/tryce
-00000fd0: 7261 746f 7073 2d65 7861 6d70 6c65 332e  ratops-example3.
-00000fe0: 6769 6629 5c6e 5c6e 2323 2320 5b60 666c  gif)\n\n### [`fl
-00000ff0: 616b 6538 605d 2868 7474 7073 3a2f 2f67  ake8`](https://g
-00001000: 6974 6875 622e 636f 6d2f 5079 4351 412f  ithub.com/PyCQA/
-00001010: 666c 616b 6538 2920 506c 7567 696e 5c6e  flake8) Plugin\n
-00001020: 5c6e f09f a696 2054 7279 6365 7261 746f  \n.... Trycerato
-00001030: 7073 2069 7320 616c 736f 2061 2070 6c75  ps is also a plu
-00001040: 6769 6e20 666f 7220 6066 6c61 6b65 3860  gin for `flake8`
-00001050: 2c20 736f 2079 6f75 2063 616e 3a5c 6e5c  , so you can:\n\
-00001060: 6e60 6060 5c6e e29d af20 666c 616b 6538  n```\n... flake8
-00001070: 202d 2d73 656c 6563 7420 5443 2073 7263   --select TC src
-00001080: 2f74 6573 7473 2f73 616d 706c 6573 2f76  /tests/samples/v
-00001090: 696f 6c61 7469 6f6e 732f 6361 6c6c 5f72  iolations/call_r
-000010a0: 6169 7365 5f76 616e 696c 6c61 2e70 795c  aise_vanilla.py\
-000010b0: 6e73 7263 2f74 6573 7473 2f73 616d 706c  nsrc/tests/sampl
-000010c0: 6573 2f76 696f 6c61 7469 6f6e 732f 6361  es/violations/ca
-000010d0: 6c6c 5f72 6169 7365 5f76 616e 696c 6c61  ll_raise_vanilla
-000010e0: 2e70 793a 3133 3a39 3a20 5443 3030 3220  .py:13:9: TC002 
-000010f0: 4372 6561 7465 2079 6f75 7220 6f77 6e20  Create your own 
-00001100: 6578 6365 7074 696f 6e5c 6e73 7263 2f74  exception\nsrc/t
-00001110: 6573 7473 2f73 616d 706c 6573 2f76 696f  ests/samples/vio
-00001120: 6c61 7469 6f6e 732f 6361 6c6c 5f72 6169  lations/call_rai
-00001130: 7365 5f76 616e 696c 6c61 2e70 793a 3133  se_vanilla.py:13
-00001140: 3a39 3a20 5443 3030 3320 4176 6f69 6420  :9: TC003 Avoid 
-00001150: 7370 6563 6966 7969 6e67 206c 6f6e 6720  specifying long 
-00001160: 6d65 7373 6167 6573 206f 7574 7369 6465  messages outside
-00001170: 2074 6865 2065 7863 6570 7469 6f6e 2063   the exception c
-00001180: 6c61 7373 5c6e 7372 632f 7465 7374 732f  lass\nsrc/tests/
-00001190: 7361 6d70 6c65 732f 7669 6f6c 6174 696f  samples/violatio
-000011a0: 6e73 2f63 616c 6c5f 7261 6973 655f 7661  ns/call_raise_va
-000011b0: 6e69 6c6c 612e 7079 3a32 313a 393a 2054  nilla.py:21:9: T
-000011c0: 4332 3031 2053 696d 706c 7920 7573 6520  C201 Simply use 
-000011d0: 5c27 7261 6973 655c 2720 7769 7468 6f75  \'raise\' withou
-000011e0: 7420 7370 6563 6966 7969 6e67 2065 7863  t specifying exc
-000011f0: 6570 7469 6f6e 206f 626a 6563 7420 6167  eption object ag
-00001200: 6169 6e5c 6e60 6060 5c6e 5c6e 2323 2056  ain\n```\n\n## V
-00001210: 696f 6c61 7469 6f6e 735c 6e5c 6e41 6c6c  iolations\n\nAll
-00001220: 2076 696f 6c61 7469 6f6e 7320 616e 6420   violations and 
-00001230: 6974 7320 6465 7363 7269 7074 696f 6e73  its descriptions
-00001240: 2063 616e 2062 6520 666f 756e 6420 696e   can be found in
-00001250: 205b 646f 6373 5d28 6874 7470 733a 2f2f   [docs](https://
-00001260: 6769 7468 7562 2e63 6f6d 2f67 7569 6c61  github.com/guila
-00001270: 7472 6f76 612f 7472 7963 6572 6174 6f70  trova/tryceratop
-00001280: 732f 7472 6565 2f6d 6169 6e2f 646f 6373  s/tree/main/docs
-00001290: 2f76 696f 6c61 7469 6f6e 7329 2e5c 6e5c  /violations).\n\
-000012a0: 6e23 2323 2041 7574 6f66 6978 2073 7570  n### Autofix sup
-000012b0: 706f 7274 5c6e 5c6e 536f 2066 6172 2c20  port\n\nSo far, 
-000012c0: 6175 746f 6669 7820 6f6e 6c79 2073 7570  autofix only sup
-000012d0: 706f 7274 7320 7669 6f6c 6174 696f 6e73  ports violations
-000012e0: 3a20 5b54 4332 3030 5d28 646f 6373 2f76  : [TC200](docs/v
-000012f0: 696f 6c61 7469 6f6e 732f 5443 3230 302e  iolations/TC200.
-00001300: 6d64 292c 205b 5443 3230 315d 2864 6f63  md), [TC201](doc
-00001310: 732f 7669 6f6c 6174 696f 6e73 2f54 4332  s/violations/TC2
-00001320: 3031 2e6d 6429 2c20 616e 6420 5b54 4334  01.md), and [TC4
-00001330: 3030 5d28 646f 6373 2f76 696f 6c61 7469  00](docs/violati
-00001340: 6f6e 732f 5443 3430 302e 6d64 292e 5c6e  ons/TC400.md).\n
-00001350: 5c6e 2323 2320 4967 6e6f 7269 6e67 2076  \n### Ignoring v
-00001360: 696f 6c61 7469 6f6e 735c 6e5c 6e49 6620  iolations\n\nIf 
-00001370: 796f 7520 7761 6e74 2074 6f20 6967 6e6f  you want to igno
-00001380: 7265 2061 2076 696f 6c61 7469 6f6e 2069  re a violation i
-00001390: 6e20 6120 7370 6563 6966 6963 2066 696c  n a specific fil
-000013a0: 652c 2079 6f75 2063 616e 2065 6974 6865  e, you can eithe
-000013b0: 723a 5c6e 5c6e 2d20 4164 6420 6120 636f  r:\n\n- Add a co
-000013c0: 6d6d 656e 7420 7769 7468 2060 6e6f 7161  mment with `noqa
-000013d0: 6020 746f 2074 6865 2074 6f70 206f 6620  ` to the top of 
-000013e0: 7468 6520 6669 6c65 2079 6f75 2077 616e  the file you wan
-000013f0: 7420 746f 2069 676e 6f72 655c 6e2d 2041  t to ignore\n- A
-00001400: 6464 2061 2063 6f6d 6d65 6e74 2077 6974  dd a comment wit
-00001410: 6820 606e 6f71 6160 2074 6f20 7468 6520  h `noqa` to the 
-00001420: 6c69 6e65 2079 6f75 2077 616e 7420 746f  line you want to
-00001430: 2069 676e 6f72 655c 6e2d 2041 6464 2061   ignore\n- Add a
-00001440: 2063 6f6d 6d65 6e74 2077 6974 6820 606e   comment with `n
-00001450: 6f71 613a 2043 4f44 4560 2074 6f20 7468  oqa: CODE` to th
-00001460: 6520 6c69 6e65 2079 6f75 2077 616e 7420  e line you want 
-00001470: 746f 2069 676e 6f72 6520 6120 7370 6563  to ignore a spec
-00001480: 6966 6963 2076 696f 6c61 7469 6f6e 5c6e  ific violation\n
-00001490: 5c6e 4578 616d 706c 653a 5c6e 5c6e 6060  \nExample:\n\n``
-000014a0: 6070 795c 6e64 6566 2076 6572 626f 7365  `py\ndef verbose
-000014b0: 5f72 6572 6169 7365 5f31 2829 3a5c 6e20  _reraise_1():\n 
-000014c0: 2020 2074 7279 3a5c 6e20 2020 2020 2020     try:\n       
-000014d0: 2061 203d 2031 5c6e 2020 2020 6578 6365   a = 1\n    exce
-000014e0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-000014f0: 6578 3a5c 6e20 2020 2020 2020 2072 6169  ex:\n        rai
-00001500: 7365 2065 7820 2023 206e 6f71 613a 2054  se ex  # noqa: T
-00001510: 4332 3032 5c6e 6060 605c 6e5c 6e23 2323  C202\n```\n\n###
-00001520: 2043 6f6e 6669 6775 7261 7469 6f6e 5c6e   Configuration\n
-00001530: 5c6e 596f 7520 6361 6e20 7365 7420 7570  \nYou can set up
-00001540: 2061 2060 7079 7072 6f6a 6563 742e 746f   a `pyproject.to
-00001550: 6d6c 6020 6669 6c65 2074 6f20 7365 7420  ml` file to set 
-00001560: 7275 6c65 732e 5c6e 5468 6973 2069 7320  rules.\nThis is 
-00001570: 7573 6566 756c 2074 6f20 6176 6f69 6420  useful to avoid 
-00001580: 7265 7573 696e 6720 7468 6520 7361 6d65  reusing the same
-00001590: 2043 4c49 2066 6c61 6773 206f 7665 7220   CLI flags over 
-000015a0: 616e 6420 6f76 6572 2061 6761 696e 2061  and over again a
-000015b0: 6e64 2068 656c 7073 2074 6f20 6465 6669  nd helps to defi
-000015c0: 6e65 2074 6865 2073 7472 7563 7475 7265  ne the structure
-000015d0: 206f 6620 796f 7572 2070 726f 6a65 6374   of your project
-000015e0: 2e5c 6e5c 6e45 7861 6d70 6c65 3a5c 6e5c  .\n\nExample:\n\
-000015f0: 6e60 6060 746f 6d6c 5c6e 5b74 6f6f 6c2e  n```toml\n[tool.
-00001600: 7472 7963 6572 6174 6f70 735d 5c6e 6578  tryceratops]\nex
-00001610: 636c 7564 6520 3d20 5b22 7361 6d70 6c65  clude = ["sample
-00001620: 7322 5d5c 6e69 676e 6f72 6520 3d20 5b22  s"]\nignore = ["
-00001630: 5443 3030 3222 2c20 2254 4332 3030 222c  TC002", "TC200",
-00001640: 2022 5443 3330 3022 5d5c 6e65 7870 6572   "TC300"]\nexper
-00001650: 696d 656e 7461 6c20 3d20 7472 7565 5c6e  imental = true\n
-00001660: 6060 605c 6e5c 6e43 4c49 2066 6c61 6773  ```\n\nCLI flags
-00001670: 2061 6c77 6179 7320 6f76 6572 7772 6974   always overwrit
-00001680: 6520 7468 6520 636f 6e66 6967 2066 696c  e the config fil
-00001690: 652e 5c6e 5c6e 2323 2050 7265 2d63 6f6d  e.\n\n## Pre-com
-000016a0: 6d69 745c 6e5c 6e49 6620 796f 7520 7769  mit\n\nIf you wi
-000016b0: 7368 2074 6f20 7573 6520 7072 652d 636f  sh to use pre-co
-000016c0: 6d6d 6974 2c20 6164 6420 7468 6973 3a5c  mmit, add this:\
-000016d0: 6e5c 6e60 6060 7961 6d6c 5c6e 2020 2d20  n\n```yaml\n  - 
-000016e0: 7265 706f 3a20 6874 7470 733a 2f2f 6769  repo: https://gi
-000016f0: 7468 7562 2e63 6f6d 2f67 7569 6c61 7472  thub.com/guilatr
-00001700: 6f76 612f 7472 7963 6572 6174 6f70 735c  ova/tryceratops\
-00001710: 6e20 2020 2072 6576 3a20 7631 2e31 2e30  n    rev: v1.1.0
-00001720: 5c6e 2020 2020 686f 6f6b 733a 5c6e 2020  \n    hooks:\n  
-00001730: 2020 2020 2d20 6964 3a20 7472 7963 6572      - id: trycer
-00001740: 6174 6f70 735c 6e60 6060 5c6e 5c6e 2323  atops\n```\n\n##
-00001750: 2053 686f 7720 796f 7572 2073 7479 6c65   Show your style
-00001760: 5c6e 5c6e 5b21 5b74 7279 2f65 7863 6570  \n\n[![try/excep
-00001770: 7420 7374 796c 653a 2074 7279 6365 7261  t style: trycera
-00001780: 746f 7073 5d28 6874 7470 733a 2f2f 696d  tops](https://im
-00001790: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-000017a0: 6765 2f74 7279 2532 4665 7863 6570 7425  ge/try%2Fexcept%
-000017b0: 3230 7374 796c 652d 7472 7963 6572 6174  20style-trycerat
-000017c0: 6f70 7325 3230 2546 3025 3946 2541 3625  ops%20%F0%9F%A6%
-000017d0: 3936 2545 3225 3943 2541 382d 626c 6163  96%E2%9C%A8-blac
-000017e0: 6b29 5d28 6874 7470 733a 2f2f 6769 7468  k)](https://gith
-000017f0: 7562 2e63 6f6d 2f67 7569 6c61 7472 6f76  ub.com/guilatrov
-00001800: 612f 7472 7963 6572 6174 6f70 7329 5c6e  a/tryceratops)\n
-00001810: 5c6e 4164 6420 7468 6973 2066 616e 6379  \nAdd this fancy
-00001820: 2062 6164 6765 2074 6f20 796f 7572 2070   badge to your p
-00001830: 726f 6a65 6374 5c27 7320 6052 4541 444d  roject\'s `READM
-00001840: 452e 6d64 603a 5c6e 5c6e 6060 606d 645c  E.md`:\n\n```md\
-00001850: 6e5b 215b 7472 792f 6578 6365 7074 2073  n[![try/except s
-00001860: 7479 6c65 3a20 7472 7963 6572 6174 6f70  tyle: tryceratop
-00001870: 735d 2868 7474 7073 3a2f 2f69 6d67 2e73  s](https://img.s
-00001880: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00001890: 7472 7925 3246 6578 6365 7074 2532 3073  try%2Fexcept%20s
-000018a0: 7479 6c65 2d74 7279 6365 7261 746f 7073  tyle-tryceratops
-000018b0: 2532 3025 4630 2539 4625 4136 2539 3625  %20%F0%9F%A6%96%
-000018c0: 4532 2539 4325 4138 2d62 6c61 636b 295d  E2%9C%A8-black)]
-000018d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000018e0: 636f 6d2f 6775 696c 6174 726f 7661 2f74  com/guilatrova/t
-000018f0: 7279 6365 7261 746f 7073 295c 6e60 6060  ryceratops)\n```
-00001900: 5c6e 5c6e 2323 2045 7874 7261 2052 6573  \n\n## Extra Res
-00001910: 6f75 7263 6573 5c6e 5c6e 4966 2079 6f75  ources\n\nIf you
-00001920: 2077 616e 7420 746f 2072 6561 6420 6d6f   want to read mo
-00001930: 7265 2061 626f 7574 3a5c 6e5c 6e2d 205b  re about:\n\n- [
-00001940: 486f 7720 746f 2073 7472 7563 7475 7265  How to structure
-00001950: 2065 7863 6570 7469 6f6e 7320 696e 2050   exceptions in P
-00001960: 7974 686f 6e20 f09f 908d 20f0 9f8f 97ef  ython .... .....
-00001970: b88f 20f0 9f92 a35d 2868 7474 7073 3a2f  .. ....](https:/
-00001980: 2f62 6c6f 672e 6775 696c 6174 726f 7661  /blog.guilatrova
-00001990: 2e64 6576 2f68 6f77 2d74 6f2d 7374 7275  .dev/how-to-stru
-000019a0: 6374 7572 652d 6578 6365 7074 696f 6e2d  cture-exception-
-000019b0: 696e 2d70 7974 686f 6e2d 6c69 6b65 2d61  in-python-like-a
-000019c0: 2d70 726f 2f29 5c6e 2d20 5b48 6f77 2074  -pro/)\n- [How t
-000019d0: 6f20 6c6f 6720 696e 2050 7974 686f 6e20  o log in Python 
-000019e0: f09f 908d f09f 8cb4 5d28 6874 7470 733a  ........](https:
-000019f0: 2f2f 626c 6f67 2e67 7569 6c61 7472 6f76  //blog.guilatrov
-00001a00: 612e 6465 762f 686f 772d 746f 2d6c 6f67  a.dev/how-to-log
-00001a10: 2d69 6e2d 7079 7468 6f6e 2d6c 696b 652d  -in-python-like-
-00001a20: 612d 7072 6f2f 295c 6e2d 205b 426f 6f6b  a-pro/)\n- [Book
-00001a30: 3a20 4566 6665 6374 6976 6520 5079 7468  : Effective Pyth
-00001a40: 6f6e 5d28 6874 7470 733a 2f2f 616d 7a6e  on](https://amzn
-00001a50: 2e74 6f2f 3362 4556 4870 4729 5c6e 5c6e  .to/3bEVHpG)\n\n
-00001a60: 2323 2043 6f6e 7472 6962 7574 696e 675c  ## Contributing\
-00001a70: 6e5c 6e54 6861 6e6b 2079 6f75 2066 6f72  n\nThank you for
-00001a80: 2063 6f6e 7369 6465 7269 6e67 206d 616b   considering mak
-00001a90: 696e 6720 5472 7963 6572 6174 6f70 7320  ing Tryceratops 
-00001aa0: 6265 7474 6572 2066 6f72 2065 7665 7279  better for every
-00001ab0: 6f6e 6521 5c6e 5c6e 5265 6665 7220 746f  one!\n\nRefer to
-00001ac0: 205b 436f 6e74 7269 6275 7469 6e67 2064   [Contributing d
-00001ad0: 6f63 735d 2864 6f63 732f 434f 4e54 5249  ocs](docs/CONTRI
-00001ae0: 4255 5449 4e47 2e6d 6429 2e5c 6e5c 6e23  BUTING.md).\n\n#
-00001af0: 2320 4368 616e 6765 206c 6f67 5c6e 5c6e  # Change log\n\n
-00001b00: 5365 6520 5b43 4841 4e47 454c 4f47 5d28  See [CHANGELOG](
-00001b10: 4348 414e 4745 4c4f 472e 6d64 292e 5c6e  CHANGELOG.md).\n
-00001b20: 5c6e 2323 204c 6963 656e 7365 5c6e 5c6e  \n## License\n\n
-00001b30: 4d49 545c 6e5c 6e23 2320 4372 6564 6974  MIT\n\n## Credit
-00001b40: 735c 6e5c 6e54 6861 6e6b 7320 746f 2047  s\n\nThanks to G
-00001b50: 6f64 2066 6f72 2074 6865 2069 6e73 7069  od for the inspi
-00001b60: 7261 7469 6f6e 20f0 9f99 8c20 e298 81ef  ration .... ....
-00001b70: b88f 20e2 9880 efb8 8f5c 6e5c 6e54 6865  .. ......\n\nThe
-00001b80: 205b 626c 6163 6b5d 2868 7474 7073 3a2f   [black](https:/
-00001b90: 2f67 6974 6875 622e 636f 6d2f 7073 662f  /github.com/psf/
-00001ba0: 626c 6163 6b29 2070 726f 6a65 6374 2066  black) project f
-00001bb0: 6f72 2069 6e73 6967 6874 732e 5c6e 272c  or insights.\n',
-00001bc0: 0a20 2020 2027 6175 7468 6f72 273a 2027  .    'author': '
-00001bd0: 4775 696c 6865 726d 6520 4c61 7472 6f76  Guilherme Latrov
-00001be0: 6127 2c0a 2020 2020 2761 7574 686f 725f  a',.    'author_
-00001bf0: 656d 6169 6c27 3a20 2768 656c 6c6f 4067  email': 'hello@g
-00001c00: 7569 6c61 7472 6f76 612e 6465 7627 2c0a  uilatrova.dev',.
-00001c10: 2020 2020 276d 6169 6e74 6169 6e65 7227      'maintainer'
-00001c20: 3a20 4e6f 6e65 2c0a 2020 2020 276d 6169  : None,.    'mai
-00001c30: 6e74 6169 6e65 725f 656d 6169 6c27 3a20  ntainer_email': 
-00001c40: 4e6f 6e65 2c0a 2020 2020 2775 726c 273a  None,.    'url':
-00001c50: 2027 6874 7470 733a 2f2f 6769 7468 7562   'https://github
-00001c60: 2e63 6f6d 2f67 7569 6c61 7472 6f76 612f  .com/guilatrova/
-00001c70: 7472 7963 6572 6174 6f70 7327 2c0a 2020  tryceratops',.  
-00001c80: 2020 2770 6163 6b61 6765 5f64 6972 273a    'package_dir':
-00001c90: 2070 6163 6b61 6765 5f64 6972 2c0a 2020   package_dir,.  
-00001ca0: 2020 2770 6163 6b61 6765 7327 3a20 7061    'packages': pa
-00001cb0: 636b 6167 6573 2c0a 2020 2020 2770 6163  ckages,.    'pac
-00001cc0: 6b61 6765 5f64 6174 6127 3a20 7061 636b  kage_data': pack
-00001cd0: 6167 655f 6461 7461 2c0a 2020 2020 2769  age_data,.    'i
-00001ce0: 6e73 7461 6c6c 5f72 6571 7569 7265 7327  nstall_requires'
-00001cf0: 3a20 696e 7374 616c 6c5f 7265 7175 6972  : install_requir
-00001d00: 6573 2c0a 2020 2020 2765 6e74 7279 5f70  es,.    'entry_p
-00001d10: 6f69 6e74 7327 3a20 656e 7472 795f 706f  oints': entry_po
-00001d20: 696e 7473 2c0a 2020 2020 2770 7974 686f  ints,.    'pytho
-00001d30: 6e5f 7265 7175 6972 6573 273a 2027 3e3d  n_requires': '>=
-00001d40: 332e 382c 3c34 2e30 272c 0a7d 0a0a 0a73  3.8,<4.0',.}...s
-00001d50: 6574 7570 282a 2a73 6574 7570 5f6b 7761  etup(**setup_kwa
-00001d60: 7267 7329 0a                             rgs).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7472 7963  : 2.1.Name: tryc
+00000020: 6572 6174 6f70 730a 5665 7273 696f 6e3a  eratops.Version:
+00000030: 2031 2e32 2e30 0a53 756d 6d61 7279 3a20   1.2.0.Summary: 
+00000040: 5072 6576 656e 7420 4578 6365 7074 696f  Prevent Exceptio
+00000050: 6e20 4861 6e64 6c69 6e67 2041 6e74 6950  n Handling AntiP
+00000060: 6174 7465 726e 730a 486f 6d65 2d70 6167  atterns.Home-pag
+00000070: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
+00000080: 622e 636f 6d2f 6775 696c 6174 726f 7661  b.com/guilatrova
+00000090: 2f74 7279 6365 7261 746f 7073 0a4c 6963  /tryceratops.Lic
+000000a0: 656e 7365 3a20 4d49 540a 4b65 7977 6f72  ense: MIT.Keywor
+000000b0: 6473 3a20 6c69 6e74 2c74 7279 2c65 7863  ds: lint,try,exc
+000000c0: 6570 740a 4175 7468 6f72 3a20 4775 696c  ept.Author: Guil
+000000d0: 6865 726d 6520 4c61 7472 6f76 610a 4175  herme Latrova.Au
+000000e0: 7468 6f72 2d65 6d61 696c 3a20 6865 6c6c  thor-email: hell
+000000f0: 6f40 6775 696c 6174 726f 7661 2e64 6576  o@guilatrova.dev
+00000100: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
+00000110: 3a20 3e3d 332e 382c 3c34 2e30 0a43 6c61  : >=3.8,<4.0.Cla
+00000120: 7373 6966 6965 723a 2044 6576 656c 6f70  ssifier: Develop
+00000130: 6d65 6e74 2053 7461 7475 7320 3a3a 2034  ment Status :: 4
+00000140: 202d 2042 6574 610a 436c 6173 7369 6669   - Beta.Classifi
+00000150: 6572 3a20 456e 7669 726f 6e6d 656e 7420  er: Environment 
+00000160: 3a3a 2043 6f6e 736f 6c65 0a43 6c61 7373  :: Console.Class
+00000170: 6966 6965 723a 2049 6e74 656e 6465 6420  ifier: Intended 
+00000180: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
+00000190: 6c6f 7065 7273 0a43 6c61 7373 6966 6965  lopers.Classifie
+000001a0: 723a 204c 6963 656e 7365 203a 3a20 4f53  r: License :: OS
+000001b0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
+000001c0: 5420 4c69 6365 6e73 650a 436c 6173 7369  T License.Classi
+000001d0: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
+000001e0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+000001f0: 6570 656e 6465 6e74 0a43 6c61 7373 6966  ependent.Classif
+00000200: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000210: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000220: 686f 6e20 3a3a 2033 0a43 6c61 7373 6966  hon :: 3.Classif
+00000230: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000240: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000250: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
+00000260: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000270: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000280: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
+00000290: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+000002a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002b0: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
+000002c0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000002d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000002e0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000002f0: 3131 0a43 6c61 7373 6966 6965 723a 2054  11.Classifier: T
+00000300: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
+00000310: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
+00000320: 4c69 6272 6172 6965 7320 3a3a 2050 7974  Libraries :: Pyt
+00000330: 686f 6e20 4d6f 6475 6c65 730a 436c 6173  hon Modules.Clas
+00000340: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+00000350: 2053 6f66 7477 6172 6520 4465 7665 6c6f   Software Develo
+00000360: 706d 656e 7420 3a3a 2051 7561 6c69 7479  pment :: Quality
+00000370: 2041 7373 7572 616e 6365 0a52 6571 7569   Assurance.Requi
+00000380: 7265 732d 4469 7374 3a20 636c 6963 6b20  res-Dist: click 
+00000390: 283e 3d37 290a 5265 7175 6972 6573 2d44  (>=7).Requires-D
+000003a0: 6973 743a 2072 6963 6820 283e 3d31 302e  ist: rich (>=10.
+000003b0: 3134 2e30 290a 5265 7175 6972 6573 2d44  14.0).Requires-D
+000003c0: 6973 743a 2074 6f6d 6c20 283e 3d30 2e31  ist: toml (>=0.1
+000003d0: 302e 3229 0a50 726f 6a65 6374 2d55 524c  0.2).Project-URL
+000003e0: 3a20 4368 616e 6765 6c6f 672c 2068 7474  : Changelog, htt
+000003f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000400: 6775 696c 6174 726f 7661 2f74 7279 6365  guilatrova/tryce
+00000410: 7261 746f 7073 2f62 6c6f 622f 6d61 696e  ratops/blob/main
+00000420: 2f43 4841 4e47 454c 4f47 2e6d 640a 5072  /CHANGELOG.md.Pr
+00000430: 6f6a 6563 742d 5552 4c3a 2052 6570 6f73  oject-URL: Repos
+00000440: 6974 6f72 792c 2068 7474 7073 3a2f 2f67  itory, https://g
+00000450: 6974 6875 622e 636f 6d2f 6775 696c 6174  ithub.com/guilat
+00000460: 726f 7661 2f74 7279 6365 7261 746f 7073  rova/tryceratops
+00000470: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
+00000480: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+00000490: 6d61 726b 646f 776e 0a0a 3c70 2061 6c69  markdown..<p ali
+000004a0: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
+000004b0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+000004c0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+000004d0: 7263 6f6e 7465 6e74 2e63 6f6d 2f67 7569  rcontent.com/gui
+000004e0: 6c61 7472 6f76 612f 7472 7963 6572 6174  latrova/trycerat
+000004f0: 6f70 732f 6d61 696e 2f69 6d67 2f6c 6f67  ops/main/img/log
+00000500: 6f2e 706e 6722 3e0a 3c2f 703e 0a0a 3c68  o.png">.</p>..<h
+00000510: 3220 616c 6967 6e3d 2263 656e 7465 7222  2 align="center"
+00000520: 3e50 7265 7665 6e74 2045 7863 6570 7469  >Prevent Excepti
+00000530: 6f6e 2048 616e 646c 696e 6720 416e 7469  on Handling Anti
+00000540: 5061 7474 6572 6e73 2069 6e20 5079 7468  Patterns in Pyth
+00000550: 6f6e 3c2f 6832 3e0a 0a3c 7020 616c 6967  on</h2>..<p alig
+00000560: 6e3d 2263 656e 7465 7222 3e0a 2020 3c61  n="center">.  <a
+00000570: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00000580: 6974 6875 622e 636f 6d2f 6775 696c 6174  ithub.com/guilat
+00000590: 726f 7661 2f74 7279 6365 7261 746f 7073  rova/tryceratops
+000005a0: 2f61 6374 696f 6e73 223e 3c69 6d67 2061  /actions"><img a
+000005b0: 6c74 3d22 4163 7469 6f6e 7320 5374 6174  lt="Actions Stat
+000005c0: 7573 2220 7372 633d 2268 7474 7073 3a2f  us" src="https:/
+000005d0: 2f67 6974 6875 622e 636f 6d2f 6775 696c  /github.com/guil
+000005e0: 6174 726f 7661 2f74 7279 6365 7261 746f  atrova/trycerato
+000005f0: 7073 2f77 6f72 6b66 6c6f 7773 2f43 492f  ps/workflows/CI/
+00000600: 6261 6467 652e 7376 6722 3e3c 2f61 3e0a  badge.svg"></a>.
+00000610: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000620: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000630: 6563 742f 7472 7963 6572 6174 6f70 732f  ect/tryceratops/
+00000640: 223e 3c69 6d67 2061 6c74 3d22 5079 5049  "><img alt="PyPI
+00000650: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
+00000660: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000670: 7069 2f76 2f74 7279 6365 7261 746f 7073  pi/v/tryceratops
+00000680: 222f 3e3c 2f61 3e0a 2020 3c69 6d67 2073  "/></a>.  <img s
+00000690: 7263 3d22 6874 7470 733a 2f2f 6261 6467  rc="https://badg
+000006a0: 656e 2e6e 6574 2f70 7970 692f 7079 7468  en.net/pypi/pyth
+000006b0: 6f6e 2f74 7279 6365 7261 746f 7073 2220  on/tryceratops" 
+000006c0: 2f3e 0a20 203c 6120 6872 6566 3d22 6874  />.  <a href="ht
+000006d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000006e0: 2f72 656c 656b 616e 672f 7079 7468 6f6e  /relekang/python
+000006f0: 2d73 656d 616e 7469 632d 7265 6c65 6173  -semantic-releas
+00000700: 6522 3e3c 696d 6720 616c 743d 2253 656d  e"><img alt="Sem
+00000710: 616e 7469 6320 5265 6c65 6173 6522 2073  antic Release" s
+00000720: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000730: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00000740: 2f25 3230 2532 3025 4630 2539 4625 3933  /%20%20%F0%9F%93
+00000750: 2541 3625 4630 2539 4625 3941 2538 302d  %A6%F0%9F%9A%80-
+00000760: 7365 6d61 6e74 6963 2d2d 7265 6c65 6173  semantic--releas
+00000770: 652d 6531 3030 3739 2e73 7667 223e 3c2f  e-e10079.svg"></
+00000780: 613e 0a20 203c 6120 6872 6566 3d22 6874  a>.  <a href="ht
+00000790: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000007a0: 2f67 7569 6c61 7472 6f76 612f 7472 7963  /guilatrova/tryc
+000007b0: 6572 6174 6f70 732f 626c 6f62 2f6d 6169  eratops/blob/mai
+000007c0: 6e2f 4c49 4345 4e53 4522 3e3c 696d 6720  n/LICENSE"><img 
+000007d0: 616c 743d 2247 6974 4875 6222 2073 7263  alt="GitHub" src
+000007e0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000007f0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00000800: 6c69 6365 6e73 652f 6775 696c 6174 726f  license/guilatro
+00000810: 7661 2f74 7279 6365 7261 746f 7073 222f  va/tryceratops"/
+00000820: 3e3c 2f61 3e0a 2020 3c61 2068 7265 663d  ></a>.  <a href=
+00000830: 2268 7474 7073 3a2f 2f70 6570 792e 7465  "https://pepy.te
+00000840: 6368 2f70 726f 6a65 6374 2f74 7279 6365  ch/project/tryce
+00000850: 7261 746f 7073 2f22 3e3c 696d 6720 616c  ratops/"><img al
+00000860: 743d 2244 6f77 6e6c 6f61 6473 2220 7372  t="Downloads" sr
+00000870: 633d 2268 7474 7073 3a2f 2f73 7461 7469  c="https://stati
+00000880: 632e 7065 7079 2e74 6563 682f 7065 7273  c.pepy.tech/pers
+00000890: 6f6e 616c 697a 6564 2d62 6164 6765 2f74  onalized-badge/t
+000008a0: 7279 6365 7261 746f 7073 3f70 6572 696f  ryceratops?perio
+000008b0: 643d 746f 7461 6c26 756e 6974 733d 696e  d=total&units=in
+000008c0: 7465 726e 6174 696f 6e61 6c5f 7379 7374  ternational_syst
+000008d0: 656d 266c 6566 745f 636f 6c6f 723d 6772  em&left_color=gr
+000008e0: 6579 2672 6967 6874 5f63 6f6c 6f72 3d62  ey&right_color=b
+000008f0: 6c75 6526 6c65 6674 5f74 6578 743d 2546  lue&left_text=%F
+00000900: 3025 3946 2541 3625 3936 2532 3044 6f77  0%9F%A6%96%20Dow
+00000910: 6e6c 6f61 6473 222f 3e3c 2f61 3e0a 2020  nloads"/></a>.  
+00000920: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000930: 2f67 6974 6875 622e 636f 6d2f 7073 662f  /github.com/psf/
+00000940: 626c 6163 6b22 3e3c 696d 6720 616c 743d  black"><img alt=
+00000950: 2243 6f64 6520 7374 796c 653a 2062 6c61  "Code style: bla
+00000960: 636b 2220 7372 633d 2268 7474 7073 3a2f  ck" src="https:/
+00000970: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000980: 6261 6467 652f 636f 6465 2532 3073 7479  badge/code%20sty
+00000990: 6c65 2d62 6c61 636b 2d30 3030 3030 302e  le-black-000000.
+000009a0: 7376 6722 2f3e 3c2f 613e 0a20 203c 6120  svg"/></a>.  <a 
+000009b0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+000009c0: 7468 7562 2e63 6f6d 2f67 7569 6c61 7472  thub.com/guilatr
+000009d0: 6f76 612f 7472 7963 6572 6174 6f70 7322  ova/tryceratops"
+000009e0: 3e3c 696d 6720 616c 743d 2274 7279 2f65  ><img alt="try/e
+000009f0: 7863 6570 7420 7374 796c 653a 2074 7279  xcept style: try
+00000a00: 6365 7261 746f 7073 2220 7372 633d 2268  ceratops" src="h
+00000a10: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000a20: 6473 2e69 6f2f 6261 6467 652f 7472 7925  ds.io/badge/try%
+00000a30: 3246 6578 6365 7074 2532 3073 7479 6c65  2Fexcept%20style
+00000a40: 2d74 7279 6365 7261 746f 7073 2532 3025  -tryceratops%20%
+00000a50: 4630 2539 4625 4136 2539 3625 4532 2539  F0%9F%A6%96%E2%9
+00000a60: 4325 4138 2d62 6c61 636b 2220 2f3e 3c2f  C%A8-black" /></
+00000a70: 613e 0a20 203c 6120 6872 6566 3d22 6874  a>.  <a href="ht
+00000a80: 7470 733a 2f2f 7477 6974 7465 722e 636f  tps://twitter.co
+00000a90: 6d2f 696e 7465 6e74 2f75 7365 723f 7363  m/intent/user?sc
+00000aa0: 7265 656e 5f6e 616d 653d 6775 696c 6174  reen_name=guilat
+00000ab0: 726f 7661 223e 3c69 6d67 2061 6c74 3d22  rova"><img alt="
+00000ac0: 466f 6c6c 6f77 2067 7569 6c61 7472 6f76  Follow guilatrov
+00000ad0: 6122 2073 7263 3d22 6874 7470 733a 2f2f  a" src="https://
+00000ae0: 696d 672e 7368 6965 6c64 732e 696f 2f74  img.shields.io/t
+00000af0: 7769 7474 6572 2f66 6f6c 6c6f 772f 6775  witter/follow/gu
+00000b00: 696c 6174 726f 7661 3f73 7479 6c65 3d73  ilatrova?style=s
+00000b10: 6f63 6961 6c22 2f3e 3c2f 613e 0a3c 2f70  ocial"/></a>.</p
+00000b20: 3e0a 0a49 6e73 7069 7265 6420 6279 205b  >..Inspired by [
+00000b30: 7468 6973 2062 6c6f 6720 706f 7374 5d28  this blog post](
+00000b40: 6874 7470 733a 2f2f 626c 6f67 2e67 7569  https://blog.gui
+00000b50: 6c61 7472 6f76 612e 6465 762f 6861 6e64  latrova.dev/hand
+00000b60: 6c69 6e67 2d65 7863 6570 7469 6f6e 732d  ling-exceptions-
+00000b70: 696e 2d70 7974 686f 6e2d 6c69 6b65 2d61  in-python-like-a
+00000b80: 2d70 726f 2f29 2e20 4920 6465 7363 7269  -pro/). I descri
+00000b90: 6265 6420 5b74 6865 2062 7569 6c64 696e  bed [the buildin
+00000ba0: 6720 7072 6f63 6573 7320 6f66 2074 6869  g process of thi
+00000bb0: 7320 746f 6f6c 2068 6572 655d 2868 7474  s tool here](htt
+00000bc0: 7073 3a2f 2f62 6c6f 672e 6775 696c 6174  ps://blog.guilat
+00000bd0: 726f 7661 2e64 6576 2f70 726f 6a65 6374  rova.dev/project
+00000be0: 2d74 7279 6365 7261 746f 7073 2f29 2e0a  -tryceratops/)..
+00000bf0: 0a3e 20e2 809c 466f 7220 7468 6f73 6520  .> ...For those 
+00000c00: 7768 6f20 6c69 6b65 2064 696e 6f73 6175  who like dinosau
+00000c10: 7273 20f0 9fa6 9620 616e 6420 636c 6561  rs .... and clea
+00000c20: 6e20 7472 792f 6578 6365 7074 20e2 9ca8  n try/except ...
+00000c30: 2062 6c6f 636b 732e e280 9d0a 0a2a 2a53   blocks......**S
+00000c40: 756d 6d61 7279 2a2a 0a2d 205b 496e 7374  ummary**.- [Inst
+00000c50: 616c 6c61 7469 6f6e 2061 6e64 2075 7361  allation and usa
+00000c60: 6765 5d28 2369 6e73 7461 6c6c 6174 696f  ge](#installatio
+00000c70: 6e2d 616e 642d 7573 6167 6529 0a20 202d  n-and-usage).  -
+00000c80: 205b 496e 7374 616c 6c61 7469 6f6e 5d28   [Installation](
+00000c90: 2369 6e73 7461 6c6c 6174 696f 6e29 0a20  #installation). 
+00000ca0: 202d 205b 5573 6167 655d 2823 7573 6167   - [Usage](#usag
+00000cb0: 6529 0a20 202d 205b 6066 6c61 6b65 3860  e).  - [`flake8`
+00000cc0: 2050 6c75 6769 6e5d 2823 666c 616b 6538   Plugin](#flake8
+00000cd0: 2d70 6c75 6769 6e29 0a2d 205b 5669 6f6c  -plugin).- [Viol
+00000ce0: 6174 696f 6e73 5d28 2376 696f 6c61 7469  ations](#violati
+00000cf0: 6f6e 7329 0a20 202d 205b 4175 746f 6669  ons).  - [Autofi
+00000d00: 7820 7375 7070 6f72 745d 2823 6175 746f  x support](#auto
+00000d10: 6669 782d 7375 7070 6f72 7429 0a20 202d  fix-support).  -
+00000d20: 205b 4967 6e6f 7269 6e67 2076 696f 6c61   [Ignoring viola
+00000d30: 7469 6f6e 735d 2823 6967 6e6f 7269 6e67  tions](#ignoring
+00000d40: 2d76 696f 6c61 7469 6f6e 7329 0a20 202d  -violations).  -
+00000d50: 205b 436f 6e66 6967 7572 6174 696f 6e5d   [Configuration]
+00000d60: 2823 636f 6e66 6967 7572 6174 696f 6e29  (#configuration)
+00000d70: 0a2d 205b 5072 652d 636f 6d6d 6974 5d28  .- [Pre-commit](
+00000d80: 2370 7265 2d63 6f6d 6d69 7429 0a2d 205b  #pre-commit).- [
+00000d90: 5368 6f77 2079 6f75 7220 7374 796c 655d  Show your style]
+00000da0: 2823 7368 6f77 2d79 6f75 722d 7374 796c  (#show-your-styl
+00000db0: 6529 0a2d 205b 4578 7472 6120 5265 736f  e).- [Extra Reso
+00000dc0: 7572 6365 735d 2823 6578 7472 612d 7265  urces](#extra-re
+00000dd0: 736f 7572 6365 7329 0a2d 205b 436f 6e74  sources).- [Cont
+00000de0: 7269 6275 7469 6e67 5d28 2363 6f6e 7472  ributing](#contr
+00000df0: 6962 7574 696e 6729 0a2d 205b 4368 616e  ibuting).- [Chan
+00000e00: 6765 206c 6f67 5d28 2363 6861 6e67 652d  ge log](#change-
+00000e10: 6c6f 6729 0a2d 205b 4c69 6365 6e73 655d  log).- [License]
+00000e20: 2823 6c69 6365 6e73 6529 0a2d 205b 4372  (#license).- [Cr
+00000e30: 6564 6974 735d 2823 6372 6564 6974 7329  edits](#credits)
+00000e40: 0a0a 2d2d 2d0a 0a23 2320 496e 7374 616c  ..---..## Instal
+00000e50: 6c61 7469 6f6e 2061 6e64 2075 7361 6765  lation and usage
+00000e60: 0a0a 2323 2320 496e 7374 616c 6c61 7469  ..### Installati
+00000e70: 6f6e 0a0a 6060 600a 7069 7020 696e 7374  on..```.pip inst
+00000e80: 616c 6c20 7472 7963 6572 6174 6f70 730a  all tryceratops.
+00000e90: 6060 600a 0a4f 520a 0a60 6060 0a70 6f65  ```..OR..```.poe
+00000ea0: 7472 7920 6164 6420 2d44 2074 7279 6365  try add -D tryce
+00000eb0: 7261 746f 7073 0a60 6060 0a0a 2323 2320  ratops.```..### 
+00000ec0: 5573 6167 650a 0a60 6060 0a74 7279 6365  Usage..```.tryce
+00000ed0: 7261 746f 7073 205b 6669 6c65 6e61 6d65  ratops [filename
+00000ee0: 206f 7220 6469 722e 2e2e 5d0a 6060 600a   or dir...].```.
+00000ef0: 0a59 6f75 2063 616e 2065 6e61 626c 6520  .You can enable 
+00000f00: 6578 7065 7269 6d65 6e74 616c 2061 6e61  experimental ana
+00000f10: 6c79 7a65 7273 2062 7920 7275 6e6e 696e  lyzers by runnin
+00000f20: 673a 0a0a 6060 600a 7472 7963 6572 6174  g:..```.trycerat
+00000f30: 6f70 7320 2d2d 6578 7065 7269 6d65 6e74  ops --experiment
+00000f40: 616c 205b 6669 6c65 6e61 6d65 206f 7220  al [filename or 
+00000f50: 6469 722e 2e2e 5d0a 6060 600a 0a59 6f75  dir...].```..You
+00000f60: 2063 616e 2069 676e 6f72 6520 7370 6563   can ignore spec
+00000f70: 6966 6963 2076 696f 6c61 7469 6f6e 7320  ific violations 
+00000f80: 6279 2075 7369 6e67 3a20 602d 2d69 676e  by using: `--ign
+00000f90: 6f72 6520 5443 5858 5860 2072 6570 6561  ore TCXXX` repea
+00000fa0: 7465 646c 793a 0a0a 6060 600a 7472 7963  tedly:..```.tryc
+00000fb0: 6572 6174 6f70 7320 2d2d 6967 6e6f 7265  eratops --ignore
+00000fc0: 2054 4332 3031 202d 2d69 676e 6f72 6520   TC201 --ignore 
+00000fd0: 5443 3230 3220 5b66 696c 656e 616d 6520  TC202 [filename 
+00000fe0: 6f72 2064 6972 2e2e 2e5d 0a60 6060 0a0a  or dir...].```..
+00000ff0: 596f 7520 6361 6e20 6578 636c 7564 6520  You can exclude 
+00001000: 6469 7273 2062 7920 7573 696e 673a 2060  dirs by using: `
+00001010: 2d2d 6578 636c 7564 6520 6469 722f 7061  --exclude dir/pa
+00001020: 7468 6020 7265 7065 6174 6564 6c79 3a0a  th` repeatedly:.
+00001030: 0a60 6060 0a74 7279 6365 7261 746f 7073  .```.tryceratops
+00001040: 202d 2d65 7863 6c75 6465 2074 6573 7473   --exclude tests
+00001050: 202d 2d65 7863 6c75 6465 202e 7665 6e76   --exclude .venv
+00001060: 205b 6669 6c65 6e61 6d65 206f 7220 6469   [filename or di
+00001070: 722e 2e2e 5d0a 6060 600a 0a59 6f75 2063  r...].```..You c
+00001080: 616e 2061 6c73 6f20 6175 746f 6669 7820  an also autofix 
+00001090: 736f 6d65 2076 696f 6c61 7469 6f6e 733a  some violations:
+000010a0: 0a0a 6060 600a 7472 7963 6572 6174 6f70  ..```.tryceratop
+000010b0: 7320 2d2d 6175 746f 6669 7820 5b66 696c  s --autofix [fil
+000010c0: 656e 616d 6520 6f72 2064 6972 2e2e 2e5d  ename or dir...]
+000010d0: 0a60 6060 0a0a 215b 6578 616d 706c 655d  .```..![example]
+000010e0: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
+000010f0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00001100: 6f6d 2f67 7569 6c61 7472 6f76 612f 7472  om/guilatrova/tr
+00001110: 7963 6572 6174 6f70 732f 6d61 696e 2f69  yceratops/main/i
+00001120: 6d67 2f74 7279 6365 7261 746f 7073 2d65  mg/tryceratops-e
+00001130: 7861 6d70 6c65 332e 6769 6629 0a0a 2323  xample3.gif)..##
+00001140: 2320 5b60 666c 616b 6538 605d 2868 7474  # [`flake8`](htt
+00001150: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001160: 5079 4351 412f 666c 616b 6538 2920 506c  PyCQA/flake8) Pl
+00001170: 7567 696e 0a0a f09f a696 2054 7279 6365  ugin...... Tryce
+00001180: 7261 746f 7073 2069 7320 616c 736f 2061  ratops is also a
+00001190: 2070 6c75 6769 6e20 666f 7220 6066 6c61   plugin for `fla
+000011a0: 6b65 3860 2c20 736f 2079 6f75 2063 616e  ke8`, so you can
+000011b0: 3a0a 0a60 6060 0ae2 9daf 2066 6c61 6b65  :..```.... flake
+000011c0: 3820 2d2d 7365 6c65 6374 2054 4320 7372  8 --select TC sr
+000011d0: 632f 7465 7374 732f 7361 6d70 6c65 732f  c/tests/samples/
+000011e0: 7669 6f6c 6174 696f 6e73 2f63 616c 6c5f  violations/call_
+000011f0: 7261 6973 655f 7661 6e69 6c6c 612e 7079  raise_vanilla.py
+00001200: 0a73 7263 2f74 6573 7473 2f73 616d 706c  .src/tests/sampl
+00001210: 6573 2f76 696f 6c61 7469 6f6e 732f 6361  es/violations/ca
+00001220: 6c6c 5f72 6169 7365 5f76 616e 696c 6c61  ll_raise_vanilla
+00001230: 2e70 793a 3133 3a39 3a20 5443 3030 3220  .py:13:9: TC002 
+00001240: 4372 6561 7465 2079 6f75 7220 6f77 6e20  Create your own 
+00001250: 6578 6365 7074 696f 6e0a 7372 632f 7465  exception.src/te
+00001260: 7374 732f 7361 6d70 6c65 732f 7669 6f6c  sts/samples/viol
+00001270: 6174 696f 6e73 2f63 616c 6c5f 7261 6973  ations/call_rais
+00001280: 655f 7661 6e69 6c6c 612e 7079 3a31 333a  e_vanilla.py:13:
+00001290: 393a 2054 4330 3033 2041 766f 6964 2073  9: TC003 Avoid s
+000012a0: 7065 6369 6679 696e 6720 6c6f 6e67 206d  pecifying long m
+000012b0: 6573 7361 6765 7320 6f75 7473 6964 6520  essages outside 
+000012c0: 7468 6520 6578 6365 7074 696f 6e20 636c  the exception cl
+000012d0: 6173 730a 7372 632f 7465 7374 732f 7361  ass.src/tests/sa
+000012e0: 6d70 6c65 732f 7669 6f6c 6174 696f 6e73  mples/violations
+000012f0: 2f63 616c 6c5f 7261 6973 655f 7661 6e69  /call_raise_vani
+00001300: 6c6c 612e 7079 3a32 313a 393a 2054 4332  lla.py:21:9: TC2
+00001310: 3031 2053 696d 706c 7920 7573 6520 2772  01 Simply use 'r
+00001320: 6169 7365 2720 7769 7468 6f75 7420 7370  aise' without sp
+00001330: 6563 6966 7969 6e67 2065 7863 6570 7469  ecifying excepti
+00001340: 6f6e 206f 626a 6563 7420 6167 6169 6e0a  on object again.
+00001350: 6060 600a 0a23 2320 5669 6f6c 6174 696f  ```..## Violatio
+00001360: 6e73 0a0a 416c 6c20 7669 6f6c 6174 696f  ns..All violatio
+00001370: 6e73 2061 6e64 2069 7473 2064 6573 6372  ns and its descr
+00001380: 6970 7469 6f6e 7320 6361 6e20 6265 2066  iptions can be f
+00001390: 6f75 6e64 2069 6e20 5b64 6f63 735d 2868  ound in [docs](h
+000013a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000013b0: 6d2f 6775 696c 6174 726f 7661 2f74 7279  m/guilatrova/try
+000013c0: 6365 7261 746f 7073 2f74 7265 652f 6d61  ceratops/tree/ma
+000013d0: 696e 2f64 6f63 732f 7669 6f6c 6174 696f  in/docs/violatio
+000013e0: 6e73 292e 0a0a 2323 2320 4175 746f 6669  ns)...### Autofi
+000013f0: 7820 7375 7070 6f72 740a 0a53 6f20 6661  x support..So fa
+00001400: 722c 2061 7574 6f66 6978 206f 6e6c 7920  r, autofix only 
+00001410: 7375 7070 6f72 7473 2076 696f 6c61 7469  supports violati
+00001420: 6f6e 733a 205b 5443 3230 305d 2864 6f63  ons: [TC200](doc
+00001430: 732f 7669 6f6c 6174 696f 6e73 2f54 4332  s/violations/TC2
+00001440: 3030 2e6d 6429 2c20 5b54 4332 3031 5d28  00.md), [TC201](
+00001450: 646f 6373 2f76 696f 6c61 7469 6f6e 732f  docs/violations/
+00001460: 5443 3230 312e 6d64 292c 2061 6e64 205b  TC201.md), and [
+00001470: 5443 3430 305d 2864 6f63 732f 7669 6f6c  TC400](docs/viol
+00001480: 6174 696f 6e73 2f54 4334 3030 2e6d 6429  ations/TC400.md)
+00001490: 2e0a 0a23 2323 2049 676e 6f72 696e 6720  ...### Ignoring 
+000014a0: 7669 6f6c 6174 696f 6e73 0a0a 4966 2079  violations..If y
+000014b0: 6f75 2077 616e 7420 746f 2069 676e 6f72  ou want to ignor
+000014c0: 6520 6120 7669 6f6c 6174 696f 6e20 696e  e a violation in
+000014d0: 2061 2073 7065 6369 6669 6320 6669 6c65   a specific file
+000014e0: 2c20 796f 7520 6361 6e20 6569 7468 6572  , you can either
+000014f0: 3a0a 0a2d 2041 6464 2061 2063 6f6d 6d65  :..- Add a comme
+00001500: 6e74 2077 6974 6820 606e 6f71 6160 2074  nt with `noqa` t
+00001510: 6f20 7468 6520 746f 7020 6f66 2074 6865  o the top of the
+00001520: 2066 696c 6520 796f 7520 7761 6e74 2074   file you want t
+00001530: 6f20 6967 6e6f 7265 0a2d 2041 6464 2061  o ignore.- Add a
+00001540: 2063 6f6d 6d65 6e74 2077 6974 6820 606e   comment with `n
+00001550: 6f71 6160 2074 6f20 7468 6520 6c69 6e65  oqa` to the line
+00001560: 2079 6f75 2077 616e 7420 746f 2069 676e   you want to ign
+00001570: 6f72 650a 2d20 4164 6420 6120 636f 6d6d  ore.- Add a comm
+00001580: 656e 7420 7769 7468 2060 6e6f 7161 3a20  ent with `noqa: 
+00001590: 434f 4445 6020 746f 2074 6865 206c 696e  CODE` to the lin
+000015a0: 6520 796f 7520 7761 6e74 2074 6f20 6967  e you want to ig
+000015b0: 6e6f 7265 2061 2073 7065 6369 6669 6320  nore a specific 
+000015c0: 7669 6f6c 6174 696f 6e0a 0a45 7861 6d70  violation..Examp
+000015d0: 6c65 3a0a 0a60 6060 7079 0a64 6566 2076  le:..```py.def v
+000015e0: 6572 626f 7365 5f72 6572 6169 7365 5f31  erbose_reraise_1
+000015f0: 2829 3a0a 2020 2020 7472 793a 0a20 2020  ():.    try:.   
+00001600: 2020 2020 2061 203d 2031 0a20 2020 2065       a = 1.    e
+00001610: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+00001620: 6173 2065 783a 0a20 2020 2020 2020 2072  as ex:.        r
+00001630: 6169 7365 2065 7820 2023 206e 6f71 613a  aise ex  # noqa:
+00001640: 2054 4332 3032 0a60 6060 0a0a 2323 2320   TC202.```..### 
+00001650: 436f 6e66 6967 7572 6174 696f 6e0a 0a59  Configuration..Y
+00001660: 6f75 2063 616e 2073 6574 2075 7020 6120  ou can set up a 
+00001670: 6070 7970 726f 6a65 6374 2e74 6f6d 6c60  `pyproject.toml`
+00001680: 2066 696c 6520 746f 2073 6574 2072 756c   file to set rul
+00001690: 6573 2e0a 5468 6973 2069 7320 7573 6566  es..This is usef
+000016a0: 756c 2074 6f20 6176 6f69 6420 7265 7573  ul to avoid reus
+000016b0: 696e 6720 7468 6520 7361 6d65 2043 4c49  ing the same CLI
+000016c0: 2066 6c61 6773 206f 7665 7220 616e 6420   flags over and 
+000016d0: 6f76 6572 2061 6761 696e 2061 6e64 2068  over again and h
+000016e0: 656c 7073 2074 6f20 6465 6669 6e65 2074  elps to define t
+000016f0: 6865 2073 7472 7563 7475 7265 206f 6620  he structure of 
+00001700: 796f 7572 2070 726f 6a65 6374 2e0a 0a45  your project...E
+00001710: 7861 6d70 6c65 3a0a 0a60 6060 746f 6d6c  xample:..```toml
+00001720: 0a5b 746f 6f6c 2e74 7279 6365 7261 746f  .[tool.trycerato
+00001730: 7073 5d0a 6578 636c 7564 6520 3d20 5b22  ps].exclude = ["
+00001740: 7361 6d70 6c65 7322 5d0a 6967 6e6f 7265  samples"].ignore
+00001750: 203d 205b 2254 4330 3032 222c 2022 5443   = ["TC002", "TC
+00001760: 3230 3022 2c20 2254 4333 3030 225d 0a65  200", "TC300"].e
+00001770: 7870 6572 696d 656e 7461 6c20 3d20 7472  xperimental = tr
+00001780: 7565 0a60 6060 0a0a 434c 4920 666c 6167  ue.```..CLI flag
+00001790: 7320 616c 7761 7973 206f 7665 7277 7269  s always overwri
+000017a0: 7465 2074 6865 2063 6f6e 6669 6720 6669  te the config fi
+000017b0: 6c65 2e0a 0a23 2320 5072 652d 636f 6d6d  le...## Pre-comm
+000017c0: 6974 0a0a 4966 2079 6f75 2077 6973 6820  it..If you wish 
+000017d0: 746f 2075 7365 2070 7265 2d63 6f6d 6d69  to use pre-commi
+000017e0: 742c 2061 6464 2074 6869 733a 0a0a 6060  t, add this:..``
+000017f0: 6079 616d 6c0a 2020 2d20 7265 706f 3a20  `yaml.  - repo: 
+00001800: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001810: 6f6d 2f67 7569 6c61 7472 6f76 612f 7472  om/guilatrova/tr
+00001820: 7963 6572 6174 6f70 730a 2020 2020 7265  yceratops.    re
+00001830: 763a 2076 312e 322e 300a 2020 2020 686f  v: v1.2.0.    ho
+00001840: 6f6b 733a 0a20 2020 2020 202d 2069 643a  oks:.      - id:
+00001850: 2074 7279 6365 7261 746f 7073 0a60 6060   tryceratops.```
+00001860: 0a0a 2323 2053 686f 7720 796f 7572 2073  ..## Show your s
+00001870: 7479 6c65 0a0a 5b21 5b74 7279 2f65 7863  tyle..[![try/exc
+00001880: 6570 7420 7374 796c 653a 2074 7279 6365  ept style: tryce
+00001890: 7261 746f 7073 5d28 6874 7470 733a 2f2f  ratops](https://
+000018a0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+000018b0: 6164 6765 2f74 7279 2532 4665 7863 6570  adge/try%2Fexcep
+000018c0: 7425 3230 7374 796c 652d 7472 7963 6572  t%20style-trycer
+000018d0: 6174 6f70 7325 3230 2546 3025 3946 2541  atops%20%F0%9F%A
+000018e0: 3625 3936 2545 3225 3943 2541 382d 626c  6%96%E2%9C%A8-bl
+000018f0: 6163 6b29 5d28 6874 7470 733a 2f2f 6769  ack)](https://gi
+00001900: 7468 7562 2e63 6f6d 2f67 7569 6c61 7472  thub.com/guilatr
+00001910: 6f76 612f 7472 7963 6572 6174 6f70 7329  ova/tryceratops)
+00001920: 0a0a 4164 6420 7468 6973 2066 616e 6379  ..Add this fancy
+00001930: 2062 6164 6765 2074 6f20 796f 7572 2070   badge to your p
+00001940: 726f 6a65 6374 2773 2060 5245 4144 4d45  roject's `README
+00001950: 2e6d 6460 3a0a 0a60 6060 6d64 0a5b 215b  .md`:..```md.[![
+00001960: 7472 792f 6578 6365 7074 2073 7479 6c65  try/except style
+00001970: 3a20 7472 7963 6572 6174 6f70 735d 2868  : tryceratops](h
+00001980: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00001990: 6473 2e69 6f2f 6261 6467 652f 7472 7925  ds.io/badge/try%
+000019a0: 3246 6578 6365 7074 2532 3073 7479 6c65  2Fexcept%20style
+000019b0: 2d74 7279 6365 7261 746f 7073 2532 3025  -tryceratops%20%
+000019c0: 4630 2539 4625 4136 2539 3625 4532 2539  F0%9F%A6%96%E2%9
+000019d0: 4325 4138 2d62 6c61 636b 295d 2868 7474  C%A8-black)](htt
+000019e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000019f0: 6775 696c 6174 726f 7661 2f74 7279 6365  guilatrova/tryce
+00001a00: 7261 746f 7073 290a 6060 600a 0a23 2320  ratops).```..## 
+00001a10: 4578 7472 6120 5265 736f 7572 6365 730a  Extra Resources.
+00001a20: 0a49 6620 796f 7520 7761 6e74 2074 6f20  .If you want to 
+00001a30: 7265 6164 206d 6f72 6520 6162 6f75 743a  read more about:
+00001a40: 0a0a 2d20 5b48 6f77 2074 6f20 7374 7275  ..- [How to stru
+00001a50: 6374 7572 6520 6578 6365 7074 696f 6e73  cture exceptions
+00001a60: 2069 6e20 5079 7468 6f6e 20f0 9f90 8d20   in Python .... 
+00001a70: f09f 8f97 efb8 8f20 f09f 92a3 5d28 6874  ....... ....](ht
+00001a80: 7470 733a 2f2f 626c 6f67 2e67 7569 6c61  tps://blog.guila
+00001a90: 7472 6f76 612e 6465 762f 686f 772d 746f  trova.dev/how-to
+00001aa0: 2d73 7472 7563 7475 7265 2d65 7863 6570  -structure-excep
+00001ab0: 7469 6f6e 2d69 6e2d 7079 7468 6f6e 2d6c  tion-in-python-l
+00001ac0: 696b 652d 612d 7072 6f2f 290a 2d20 5b48  ike-a-pro/).- [H
+00001ad0: 6f77 2074 6f20 6c6f 6720 696e 2050 7974  ow to log in Pyt
+00001ae0: 686f 6e20 f09f 908d f09f 8cb4 5d28 6874  hon ........](ht
+00001af0: 7470 733a 2f2f 626c 6f67 2e67 7569 6c61  tps://blog.guila
+00001b00: 7472 6f76 612e 6465 762f 686f 772d 746f  trova.dev/how-to
+00001b10: 2d6c 6f67 2d69 6e2d 7079 7468 6f6e 2d6c  -log-in-python-l
+00001b20: 696b 652d 612d 7072 6f2f 290a 2d20 5b42  ike-a-pro/).- [B
+00001b30: 6f6f 6b3a 2045 6666 6563 7469 7665 2050  ook: Effective P
+00001b40: 7974 686f 6e5d 2868 7474 7073 3a2f 2f61  ython](https://a
+00001b50: 6d7a 6e2e 746f 2f33 6245 5648 7047 290a  mzn.to/3bEVHpG).
+00001b60: 0a23 2320 436f 6e74 7269 6275 7469 6e67  .## Contributing
+00001b70: 0a0a 5468 616e 6b20 796f 7520 666f 7220  ..Thank you for 
+00001b80: 636f 6e73 6964 6572 696e 6720 6d61 6b69  considering maki
+00001b90: 6e67 2054 7279 6365 7261 746f 7073 2062  ng Tryceratops b
+00001ba0: 6574 7465 7220 666f 7220 6576 6572 796f  etter for everyo
+00001bb0: 6e65 210a 0a52 6566 6572 2074 6f20 5b43  ne!..Refer to [C
+00001bc0: 6f6e 7472 6962 7574 696e 6720 646f 6373  ontributing docs
+00001bd0: 5d28 646f 6373 2f43 4f4e 5452 4942 5554  ](docs/CONTRIBUT
+00001be0: 494e 472e 6d64 292e 0a0a 2323 2043 6861  ING.md)...## Cha
+00001bf0: 6e67 6520 6c6f 670a 0a53 6565 205b 4348  nge log..See [CH
+00001c00: 414e 4745 4c4f 475d 2843 4841 4e47 454c  ANGELOG](CHANGEL
+00001c10: 4f47 2e6d 6429 2e0a 0a23 2320 4c69 6365  OG.md)...## Lice
+00001c20: 6e73 650a 0a4d 4954 0a0a 2323 2043 7265  nse..MIT..## Cre
+00001c30: 6469 7473 0a0a 5468 616e 6b73 2074 6f20  dits..Thanks to 
+00001c40: 476f 6420 666f 7220 7468 6520 696e 7370  God for the insp
+00001c50: 6972 6174 696f 6e20 f09f 998c 20e2 9881  iration .... ...
+00001c60: efb8 8f20 e298 80ef b88f 0a0a 5468 6520  ... ........The 
+00001c70: 5b62 6c61 636b 5d28 6874 7470 733a 2f2f  [black](https://
+00001c80: 6769 7468 7562 2e63 6f6d 2f70 7366 2f62  github.com/psf/b
+00001c90: 6c61 636b 2920 7072 6f6a 6563 7420 666f  lack) project fo
+00001ca0: 7220 696e 7369 6768 7473 2e0a 0a         r insights...
```


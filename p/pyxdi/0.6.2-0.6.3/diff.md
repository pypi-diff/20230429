# Comparing `tmp/pyxdi-0.6.2.tar.gz` & `tmp/pyxdi-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxdi-0.6.2.tar", max compression
+gzip compressed data, was "pyxdi-0.6.3.tar", max compression
```

## Comparing `pyxdi-0.6.2.tar` & `pyxdi-0.6.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 pyxdi-0.6.2/LICENSE
--rw-r--r--   0        0        0     1369 2023-03-01 10:13:50.665451 pyxdi-0.6.2/README.md
--rw-r--r--   0        0        0     1381 2023-04-03 07:18:11.487327 pyxdi-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      246 2023-03-24 15:06:03.633072 pyxdi-0.6.2/pyxdi/__init__.py
--rw-r--r--   0        0        0    29879 2023-04-03 07:18:04.638431 pyxdi-0.6.2/pyxdi/core.py
--rw-r--r--   0        0        0     1589 2023-03-23 19:35:30.931349 pyxdi-0.6.2/pyxdi/decorators.py
--rw-r--r--   0        0        0      218 2023-02-27 20:19:45.206653 pyxdi-0.6.2/pyxdi/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-24 15:06:03.633484 pyxdi-0.6.2/pyxdi/ext/__init__.py
--rw-r--r--   0        0        0     2502 2023-04-03 07:18:04.638926 pyxdi-0.6.2/pyxdi/ext/fastapi.py
--rw-r--r--   0        0        0        0 2023-03-24 15:06:03.633846 pyxdi-0.6.2/pyxdi/ext/starlette/__init__.py
--rw-r--r--   0        0        0      635 2023-03-24 15:06:03.633960 pyxdi-0.6.2/pyxdi/ext/starlette/middleware.py
--rw-r--r--   0        0        0        0 2023-02-14 18:16:50.285713 pyxdi-0.6.2/pyxdi/py.typed
--rw-r--r--   0        0        0      149 2023-03-25 12:38:39.922067 pyxdi-0.6.2/pyxdi/types.py
--rw-r--r--   0        0        0      262 2023-04-03 07:18:04.639410 pyxdi-0.6.2/pyxdi/utils.py
--rw-r--r--   0        0        0     2297 1970-01-01 00:00:00.000000 pyxdi-0.6.2/setup.py
--rw-r--r--   0        0        0     2305 1970-01-01 00:00:00.000000 pyxdi-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 pyxdi-0.6.3/LICENSE
+-rw-r--r--   0        0        0     1352 2023-04-05 18:56:37.235297 pyxdi-0.6.3/README.md
+-rw-r--r--   0        0        0     1380 2023-04-29 18:43:08.409486 pyxdi-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-03-24 15:06:03.633072 pyxdi-0.6.3/pyxdi/__init__.py
+-rw-r--r--   0        0        0    30084 2023-04-29 18:42:44.646420 pyxdi-0.6.3/pyxdi/core.py
+-rw-r--r--   0        0        0     1589 2023-03-23 19:35:30.931349 pyxdi-0.6.3/pyxdi/decorators.py
+-rw-r--r--   0        0        0      218 2023-02-27 20:19:45.206653 pyxdi-0.6.3/pyxdi/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-24 15:06:03.633484 pyxdi-0.6.3/pyxdi/ext/__init__.py
+-rw-r--r--   0        0        0     2502 2023-04-03 07:18:04.638926 pyxdi-0.6.3/pyxdi/ext/fastapi.py
+-rw-r--r--   0        0        0        0 2023-03-24 15:06:03.633846 pyxdi-0.6.3/pyxdi/ext/starlette/__init__.py
+-rw-r--r--   0        0        0      635 2023-03-24 15:06:03.633960 pyxdi-0.6.3/pyxdi/ext/starlette/middleware.py
+-rw-r--r--   0        0        0        0 2023-02-14 18:16:50.285713 pyxdi-0.6.3/pyxdi/py.typed
+-rw-r--r--   0        0        0      149 2023-03-25 12:38:39.922067 pyxdi-0.6.3/pyxdi/types.py
+-rw-r--r--   0        0        0      262 2023-04-03 07:18:04.639410 pyxdi-0.6.3/pyxdi/utils.py
+-rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 pyxdi-0.6.3/PKG-INFO
```

### Comparing `pyxdi-0.6.2/LICENSE` & `pyxdi-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxdi-0.6.2/README.md` & `pyxdi-0.6.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# PyxDI (in development)
+# PyxDI
 
 `PyxDI` is a modern, lightweight and async-friendly Python Dependency Injection library that leverages type annotations ([PEP 484](https://peps.python.org/pep-0484/))
 to effortlessly manage dependencies in your applications.
 
 [![CI](https://github.com/antonrh/pyxdi/actions/workflows/ci.yml/badge.svg)](https://github.com/antonrh/pyxdi/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/antonrh/pyxdi/branch/main/graph/badge.svg?token=67CLD19I0C)](https://codecov.io/gh/antonrh/pyxdi)
 [![Documentation Status](https://readthedocs.org/projects/pyxdi/badge/?version=latest)](https://pyxdi.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `pyxdi-0.6.2/pyproject.toml` & `pyxdi-0.6.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyxdi"
-version = "0.6.2"
+version = "0.6.3"
 description = "Dependency Injection library"
 authors = ["Anton Ruhlov <antonruhlov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/antonrh/pyxdi"
 keywords = ["dependency injection", "dependencies", "di", "async", "asyncio", "application"]
 packages = [
@@ -18,40 +18,44 @@
 mkdocs-material = { version = "^9.0.12", optional = true }
 
 [tool.poetry.extras]
 docs = ["mkdocs", "mkdocs-material"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
-isort = "^5.11.5"
-mypy = "^1.0"
-flake8 = "^3.9.2"
-flake8-tidy-imports = "^4.8.0"
+mypy = "^1.2.0"
+ruff = "^0.0.263"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
-sqlalchemy = "^2.0.3"
-flask = "^2.2.2"
-fastapi = "^0.95.0"
-httpx = "^0.23.3"
+fastapi = "^0.95.1"
+httpx = "^0.24.0"
 
 [tool.black]
 line-length = 88
 target-version = ['py310']
 include = '\.pyi?$'
 
-[tool.isort]
-profile = "black"
-combine_as_imports = true
-known_tests = "tests"
-sections = ["FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "TESTS", "LOCALFOLDER"]
-
 [tool.mypy]
 python_version = "3.10"
 strict = true
 
+[tool.ruff]
+line-length = 88
+select = ["C", "E", "F", "W", "B", "TID252", "T20"]
+ignore = ["B008", "B009", "B010"]
+exclude = [
+    ".git",
+    "__pycache__",
+    ".history"
+]
+
+[tool.ruff.isort]
+combine-as-imports = true
+forced-separate = ["tests"]
+
 [tool.pytest.ini_options]
 addopts = [
     "--strict-config",
     "--strict-markers",
 ]
 xfail_strict = true
 junit_family = "xunit2"
```

### Comparing `pyxdi-0.6.2/pyxdi/core.py` & `pyxdi-0.6.3/pyxdi/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import sys
 import contextlib
 import functools
 import importlib
 import inspect
 import logging
 import pkgutil
 import typing as t
@@ -27,14 +28,16 @@
     ProviderError,
     ScopeMismatch,
     UnknownDependency,
 )
 from .types import InterfaceT, ProviderObj, Scope
 from .utils import get_qualname
 
+SUPPORT_SIGNATURE_EVAL_STR = sys.version_info > (3, 9)
+
 logger = logging.getLogger(__name__)
 
 ALLOWED_SCOPES: t.Dict[Scope, t.List[Scope]] = {
     "singleton": ["singleton"],
     "request": ["request", "singleton"],
     "transient": ["transient", "singleton", "request"],
 }
@@ -206,20 +209,20 @@
         self._providers.pop(interface, None)
         self._unresolved_providers.pop(interface, None)
         self._unresolved_dependencies.pop(interface, None)
 
     def get_provider(self, interface: t.Type[t.Any]) -> Provider:
         try:
             return self._providers[interface]
-        except KeyError:
+        except KeyError as exc:
             raise ProviderError(
                 f"The provider interface for `{get_qualname(interface)}` has not been "
                 "registered. Please ensure that the provider interface is properly "
                 "registered before attempting to use it."
-            )
+            ) from exc
 
     def singleton(
         self, interface: t.Type[InterfaceT], instance: t.Any, *, override: bool = False
     ) -> Provider:
         return self.register_provider(
             interface, lambda: instance, scope="singleton", override=override
         )
@@ -653,15 +656,15 @@
         module: ModuleType,
         *,
         tags: t.Iterable[str],
     ) -> t.Tuple[t.List[ScannedProvider], t.List[ScannedDependency]]:
         scanned_providers: t.List[ScannedProvider] = []
         scanned_dependencies: t.List[ScannedDependency] = []
 
-        for name, member in inspect.getmembers(module):
+        for _, member in inspect.getmembers(module):
             if getattr(member, "__module__", None) != module.__name__ or not callable(
                 member
             ):
                 continue
 
             member_tags = getattr(member, "__pyxdi_tags__", [])
             if tags and (
@@ -744,43 +747,44 @@
             if parameter.kind == parameter.POSITIONAL_ONLY:
                 args.append(instance)
             else:
                 kwargs[parameter.name] = instance
         return args, kwargs
 
     def _get_injectable_params(self, obj: t.Callable[..., t.Any]) -> t.Dict[str, t.Any]:
-        signature = self._get_signature(obj)
-        parameters = signature.parameters
-        params = {}
-        for parameter in parameters.values():
+        injectable_params = {}
+        for parameter in self._get_signature(obj).parameters.values():
+            if not isinstance(parameter.default, DependencyMark):
+                continue
+
             annotation = parameter.annotation
             if annotation is inspect._empty:  # noqa
                 raise AnnotationError(
                     f"Missing `{get_qualname(obj)}` parameter annotation."
                 )
 
-            if not isinstance(parameter.default, DependencyMark):
-                continue
-
             if (
                 not self.has_provider(annotation)
                 and annotation not in self._unresolved_providers
                 and annotation not in self._unresolved_dependencies
             ):
                 self._unresolved_dependencies[annotation] = UnresolvedDependency(
                     parameter_name=parameter.name, obj=obj
                 )
 
-            params[parameter.name] = annotation
-        return params
+            injectable_params[parameter.name] = annotation
+        return injectable_params
 
     def _get_signature(self, obj: t.Callable[..., t.Any]) -> inspect.Signature:
         signature = self._signature_cache.get(obj)
         if signature is None:
-            signature = inspect.signature(obj, eval_str=True)
+            signature_kwargs: t.Dict[str, t.Any] = {}
+            if SUPPORT_SIGNATURE_EVAL_STR:
+                signature_kwargs["eval_str"] = True
+            signature = inspect.signature(obj, **signature_kwargs)
             self._signature_cache[obj] = signature
         return signature
 
 
 class ScopedContext:
     def __init__(self, scope: Scope, root: PyxDI) -> None:
         self._scope = scope
```

### Comparing `pyxdi-0.6.2/pyxdi/decorators.py` & `pyxdi-0.6.3/pyxdi/decorators.py`

 * *Files identical despite different names*

### Comparing `pyxdi-0.6.2/pyxdi/ext/fastapi.py` & `pyxdi-0.6.3/pyxdi/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `pyxdi-0.6.2/pyxdi/ext/starlette/middleware.py` & `pyxdi-0.6.3/pyxdi/ext/starlette/middleware.py`

 * *Files identical despite different names*

### Comparing `pyxdi-0.6.2/PKG-INFO` & `pyxdi-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxdi
-Version: 0.6.2
+Version: 0.6.3
 Summary: Dependency Injection library
 Home-page: https://github.com/antonrh/pyxdi
 License: MIT
 Keywords: dependency injection,dependencies,di,async,asyncio,application
 Author: Anton Ruhlov
 Author-email: antonruhlov@gmail.com
 Requires-Python: >=3.7,<3.12
@@ -13,20 +13,20 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: anyio (>=3.6.2,<4.0.0)
-Requires-Dist: mkdocs (>=1.4.2,<2.0.0); extra == "docs"
-Requires-Dist: mkdocs-material (>=9.0.12,<10.0.0); extra == "docs"
+Requires-Dist: mkdocs (>=1.4.2,<2.0.0) ; extra == "docs"
+Requires-Dist: mkdocs-material (>=9.0.12,<10.0.0) ; extra == "docs"
 Project-URL: Repository, https://github.com/antonrh/pyxdi
 Description-Content-Type: text/markdown
 
-# PyxDI (in development)
+# PyxDI
 
 `PyxDI` is a modern, lightweight and async-friendly Python Dependency Injection library that leverages type annotations ([PEP 484](https://peps.python.org/pep-0484/))
 to effortlessly manage dependencies in your applications.
 
 [![CI](https://github.com/antonrh/pyxdi/actions/workflows/ci.yml/badge.svg)](https://github.com/antonrh/pyxdi/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/antonrh/pyxdi/branch/main/graph/badge.svg?token=67CLD19I0C)](https://codecov.io/gh/antonrh/pyxdi)
 [![Documentation Status](https://readthedocs.org/projects/pyxdi/badge/?version=latest)](https://pyxdi.readthedocs.io/en/latest/?badge=latest)
```


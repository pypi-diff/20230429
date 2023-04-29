# Comparing `tmp/result-0.8.0b1.tar.gz` & `tmp/result-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "result-0.8.0b1.tar", last modified: Mon Mar  7 05:08:29 2022, max compression
+gzip compressed data, was "result-0.9.0.tar", last modified: Sat Dec 10 02:51:46 2022, max compression
```

## Comparing `result-0.8.0b1.tar` & `result-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 francium  (1000) users      (985)        0 2022-03-07 05:08:29.135600 result-0.8.0b1/
--rw-r--r--   0 francium  (1000) users      (985)     1079 2022-03-02 03:55:46.000000 result-0.8.0b1/LICENSE
--rw-r--r--   0 francium  (1000) users      (985)       24 2022-03-02 03:55:46.000000 result-0.8.0b1/MANIFEST.in
--rw-r--r--   0 francium  (1000) users      (985)     9981 2022-03-07 05:08:29.135600 result-0.8.0b1/PKG-INFO
--rw-r--r--   0 francium  (1000) users      (985)     9214 2022-03-02 03:55:46.000000 result-0.8.0b1/README.rst
--rw-r--r--   0 francium  (1000) users      (985)     1155 2022-03-02 03:55:46.000000 result-0.8.0b1/pyproject.toml
--rw-r--r--   0 francium  (1000) users      (985)     1064 2022-03-07 05:08:29.138933 result-0.8.0b1/setup.cfg
--rw-r--r--   0 francium  (1000) users      (985)       38 2022-03-02 03:55:46.000000 result-0.8.0b1/setup.py
-drwxr-xr-x   0 francium  (1000) users      (985)        0 2022-03-07 05:08:29.135600 result-0.8.0b1/src/
-drwxr-xr-x   0 francium  (1000) users      (985)        0 2022-03-07 05:08:29.135600 result-0.8.0b1/src/result/
--rw-r--r--   0 francium  (1000) users      (985)      190 2022-03-07 05:07:39.000000 result-0.8.0b1/src/result/__init__.py
--rw-r--r--   0 francium  (1000) users      (985)        0 2022-03-02 03:55:46.000000 result-0.8.0b1/src/result/py.typed
--rw-r--r--   0 francium  (1000) users      (985)     8543 2022-03-07 05:01:02.000000 result-0.8.0b1/src/result/result.py
-drwxr-xr-x   0 francium  (1000) users      (985)        0 2022-03-07 05:08:29.135600 result-0.8.0b1/src/result.egg-info/
--rw-r--r--   0 francium  (1000) users      (985)     9981 2022-03-07 05:08:28.000000 result-0.8.0b1/src/result.egg-info/PKG-INFO
--rw-r--r--   0 francium  (1000) users      (985)      326 2022-03-07 05:08:29.000000 result-0.8.0b1/src/result.egg-info/SOURCES.txt
--rw-r--r--   0 francium  (1000) users      (985)        1 2022-03-07 05:08:28.000000 result-0.8.0b1/src/result.egg-info/dependency_links.txt
--rw-r--r--   0 francium  (1000) users      (985)       46 2022-03-07 05:08:29.000000 result-0.8.0b1/src/result.egg-info/requires.txt
--rw-r--r--   0 francium  (1000) users      (985)        7 2022-03-07 05:08:29.000000 result-0.8.0b1/src/result.egg-info/top_level.txt
--rw-r--r--   0 francium  (1000) users      (985)        1 2022-03-07 04:36:12.000000 result-0.8.0b1/src/result.egg-info/zip-safe
+drwxr-xr-x   0 francium  (1000) users      (984)        0 2022-12-10 02:51:46.070695 result-0.9.0/
+-rw-r--r--   0 francium  (1000) users      (984)     1079 2022-12-10 02:42:53.000000 result-0.9.0/LICENSE
+-rw-r--r--   0 francium  (1000) users      (984)       24 2022-12-10 02:42:53.000000 result-0.9.0/MANIFEST.in
+-rw-r--r--   0 francium  (1000) users      (984)    10561 2022-12-10 02:51:46.070695 result-0.9.0/PKG-INFO
+-rw-r--r--   0 francium  (1000) users      (984)     9765 2022-12-10 02:42:53.000000 result-0.9.0/README.rst
+-rw-r--r--   0 francium  (1000) users      (984)     1117 2022-12-10 02:42:53.000000 result-0.9.0/pyproject.toml
+-rw-r--r--   0 francium  (1000) users      (984)     1104 2022-12-10 02:51:46.070695 result-0.9.0/setup.cfg
+-rw-r--r--   0 francium  (1000) users      (984)       38 2022-12-10 02:42:53.000000 result-0.9.0/setup.py
+drwxr-xr-x   0 francium  (1000) users      (984)        0 2022-12-10 02:51:46.067362 result-0.9.0/src/
+drwxr-xr-x   0 francium  (1000) users      (984)        0 2022-12-10 02:51:46.067362 result-0.9.0/src/result/
+-rw-r--r--   0 francium  (1000) users      (984)      188 2022-12-10 02:48:49.000000 result-0.9.0/src/result/__init__.py
+-rw-r--r--   0 francium  (1000) users      (984)        0 2022-12-10 02:42:53.000000 result-0.9.0/src/result/py.typed
+-rw-r--r--   0 francium  (1000) users      (984)     9603 2022-12-10 02:42:53.000000 result-0.9.0/src/result/result.py
+drwxr-xr-x   0 francium  (1000) users      (984)        0 2022-12-10 02:51:46.067362 result-0.9.0/src/result.egg-info/
+-rw-r--r--   0 francium  (1000) users      (984)    10561 2022-12-10 02:51:46.000000 result-0.9.0/src/result.egg-info/PKG-INFO
+-rw-r--r--   0 francium  (1000) users      (984)      326 2022-12-10 02:51:46.000000 result-0.9.0/src/result.egg-info/SOURCES.txt
+-rw-r--r--   0 francium  (1000) users      (984)        1 2022-12-10 02:51:46.000000 result-0.9.0/src/result.egg-info/dependency_links.txt
+-rw-r--r--   0 francium  (1000) users      (984)       46 2022-12-10 02:51:46.000000 result-0.9.0/src/result.egg-info/requires.txt
+-rw-r--r--   0 francium  (1000) users      (984)        7 2022-12-10 02:51:46.000000 result-0.9.0/src/result.egg-info/top_level.txt
+-rw-r--r--   0 francium  (1000) users      (984)        1 2022-12-10 02:51:45.000000 result-0.9.0/src/result.egg-info/zip-safe
```

### Comparing `result-0.8.0b1/LICENSE` & `result-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `result-0.8.0b1/PKG-INFO` & `result-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: result
-Version: 0.8.0b1
+Version: 0.9.0
 Summary: A Rust-like result type for Python
 Home-page: https://github.com/rustedpy/result
 Author: Danilo Bargen
 Author-email: mail@dbrgn.ch
 Maintainer: rustedpy github org members (https://github.com/rustedpy)
 License: MIT
 Keywords: rust,result,enum
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 License-File: LICENSE
 
 ======
 Result
 ======
@@ -31,14 +31,33 @@
 .. image:: https://codecov.io/gh/rustedpy/result/branch/master/graph/badge.svg
     :alt: Coverage
     :target: https://codecov.io/gh/rustedpy/result
 
 A simple Result type for Python 3 `inspired by Rust
 <https://doc.rust-lang.org/std/result/>`__, fully type annotated.
 
+Installation
+============
+
+Latest release:
+
+.. sourcecode:: sh
+
+   $ pip install result
+
+
+Latest GitHub ``master`` branch version:
+
+.. sourcecode:: sh
+
+   $ pip install git+https://github.com/rustedpy/result
+
+Summary
+=======
+
 The idea is that a result value can be either ``Ok(value)`` or ``Err(error)``,
 with a way to differentiate between the two. ``Ok`` and ``Err`` are both classes
 encapsulating an arbitrary value. ``Result[T, E]`` is a generic type alias for
 ``typing.Union[Ok[T], Err[E]]``. It will change code like this:
 
 .. sourcecode:: python
 
@@ -253,14 +272,26 @@
     >>> res2.unwrap_or('default')
     'default'
     >>> res1.unwrap_or_else(str.upper)
     'yay'
     >>> res2.unwrap_or_else(str.upper)
     'NAY'
 
+The ``unwrap`` method will raised an ``UnwrapError``. A custom exception can be
+raised by using the ``unwrap_or_raise`` method instead:
+
+.. sourcecode:: python
+
+    >>> res1 = Ok('yay')
+    >>> res2 = Err('nay')
+    >>> res1.unwrap_or_raise(ValueError)
+    'yay'
+    >>> res2.unwrap_or_raise(ValueError)
+    ValueError: nay
+
 Values and errors can be mapped using ``map``, ``map_or``, ``map_or_else`` and
 ``map_err``:
 
 .. sourcecode:: python
 
    >>> Ok(1).map(lambda x: x + 1)
    Ok(2)
@@ -337,9 +368,7 @@
 Otherwise using `one of these workarounds
 <https://github.com/python/mypy/issues/3889#issuecomment-325997911>`_ can help.
 
 License
 =======
 
 MIT License
-
-
```

### Comparing `result-0.8.0b1/README.rst` & `result-0.9.0/src/result.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: result
+Version: 0.9.0
+Summary: A Rust-like result type for Python
+Home-page: https://github.com/rustedpy/result
+Author: Danilo Bargen
+Author-email: mail@dbrgn.ch
+Maintainer: rustedpy github org members (https://github.com/rustedpy)
+License: MIT
+Keywords: rust,result,enum
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.7
+License-File: LICENSE
+
 ======
 Result
 ======
 
 .. image:: https://img.shields.io/github/workflow/status/rustedpy/result/CI/master
     :alt: GitHub Workflow Status (branch)
     :target: https://github.com/rustedpy/result/actions?query=workflow%3ACI+branch%3Amaster
@@ -9,14 +31,33 @@
 .. image:: https://codecov.io/gh/rustedpy/result/branch/master/graph/badge.svg
     :alt: Coverage
     :target: https://codecov.io/gh/rustedpy/result
 
 A simple Result type for Python 3 `inspired by Rust
 <https://doc.rust-lang.org/std/result/>`__, fully type annotated.
 
+Installation
+============
+
+Latest release:
+
+.. sourcecode:: sh
+
+   $ pip install result
+
+
+Latest GitHub ``master`` branch version:
+
+.. sourcecode:: sh
+
+   $ pip install git+https://github.com/rustedpy/result
+
+Summary
+=======
+
 The idea is that a result value can be either ``Ok(value)`` or ``Err(error)``,
 with a way to differentiate between the two. ``Ok`` and ``Err`` are both classes
 encapsulating an arbitrary value. ``Result[T, E]`` is a generic type alias for
 ``typing.Union[Ok[T], Err[E]]``. It will change code like this:
 
 .. sourcecode:: python
 
@@ -231,14 +272,26 @@
     >>> res2.unwrap_or('default')
     'default'
     >>> res1.unwrap_or_else(str.upper)
     'yay'
     >>> res2.unwrap_or_else(str.upper)
     'NAY'
 
+The ``unwrap`` method will raised an ``UnwrapError``. A custom exception can be
+raised by using the ``unwrap_or_raise`` method instead:
+
+.. sourcecode:: python
+
+    >>> res1 = Ok('yay')
+    >>> res2 = Err('nay')
+    >>> res1.unwrap_or_raise(ValueError)
+    'yay'
+    >>> res2.unwrap_or_raise(ValueError)
+    ValueError: nay
+
 Values and errors can be mapped using ``map``, ``map_or``, ``map_or_else`` and
 ``map_err``:
 
 .. sourcecode:: python
 
    >>> Ok(1).map(lambda x: x + 1)
    Ok(2)
```

### Comparing `result-0.8.0b1/pyproject.toml` & `result-0.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.mypy]
-python_version = "3.10"
+python_version = "3.11"
 files = [
   "src",
   "tests",
 ]
 # Exclude files with pattern matching syntax until Mypy supports it;
 # see https://github.com/python/mypy/issues/10201
 exclude = "tests/test_pattern_matching.py"
@@ -20,25 +20,23 @@
 disallow_untyped_defs = true
 ignore_missing_imports = true
 no_implicit_optional = true
 no_implicit_reexport = true
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
-show_none_errors = true
 strict_equality = true
 strict_optional = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [tool.pytest.ini_options]
 addopts = [
-  "--flake8",
   "--tb=short",
   "--cov=result",
   "--cov=tests",
   "--cov-report=term",
   "--cov-report=xml",
 
   # By default, ignore tests that only run on Python 3.10+
```

### Comparing `result-0.8.0b1/setup.cfg` & `result-0.9.0/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 include_package_data = True
 install_requires = 
 	typing_extensions;python_version<'3.10'
 package_dir =
```

### Comparing `result-0.8.0b1/src/result/result.py` & `result-0.9.0/src/result/result.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,21 @@
     Any,
     Callable,
     Generic,
     NoReturn,
     Type,
     TypeVar,
     Union,
-    cast,
     overload,
 )
 
 if sys.version_info[:2] >= (3, 10):
-    from typing import ParamSpec
+    from typing import Final, Literal, ParamSpec, TypeAlias
 else:
-    from typing_extensions import ParamSpec
+    from typing_extensions import Final, Literal, ParamSpec, TypeAlias
 
 
 T = TypeVar("T", covariant=True)  # Success type
 E = TypeVar("E", covariant=True)  # Error type
 U = TypeVar("U")
 F = TypeVar("F")
 P = ParamSpec("P")
@@ -58,18 +57,18 @@
 
     def __ne__(self, other: Any) -> bool:
         return not (self == other)
 
     def __hash__(self) -> int:
         return hash((True, self._value))
 
-    def is_ok(self) -> bool:
+    def is_ok(self) -> Literal[True]:
         return True
 
-    def is_err(self) -> bool:
+    def is_err(self) -> Literal[False]:
         return False
 
     def ok(self) -> T:
         """
         Return the value.
         """
         return self._value
@@ -113,50 +112,65 @@
 
     def unwrap_or(self, _default: U) -> T:
         """
         Return the value.
         """
         return self._value
 
-    def unwrap_or_else(self, op: Callable[[E], T]) -> T:
+    def unwrap_or_else(self, op: object) -> T:
+        """
+        Return the value.
+        """
+        return self._value
+
+    def unwrap_or_raise(self, e: object) -> T:
         """
         Return the value.
         """
         return self._value
 
-    def map(self, op: Callable[[T], U]) -> Result[U, E]:
+    def map(self, op: Callable[[T], U]) -> Ok[U]:
         """
         The contained result is `Ok`, so return `Ok` with original value mapped to
         a new value using the passed in function.
         """
         return Ok(op(self._value))
 
-    def map_or(self, default: U, op: Callable[[T], U]) -> U:
+    def map_or(self, default: object, op: Callable[[T], U]) -> U:
         """
         The contained result is `Ok`, so return the original value mapped to a new
         value using the passed in function.
         """
         return op(self._value)
 
-    def map_or_else(
-        self,
-        default_op: Callable[[], U],
-        op: Callable[[T], U]
-    ) -> U:
+    def map_or_else(self, default_op: object, op: Callable[[T], U]) -> U:
         """
         The contained result is `Ok`, so return original value mapped to
         a new value using the passed in `op` function.
         """
         return op(self._value)
 
-    def map_err(self, op: Callable[[E], F]) -> Result[T, F]:
+    def map_err(self, op: object) -> Ok[T]:
+        """
+        The contained result is `Ok`, so return `Ok` with the original value
+        """
+        return self
+
+    def and_then(self, op: Callable[[T], Result[U, E]]) -> Result[U, E]:
+        """
+        The contained result is `Ok`, so return the result of `op` with the
+        original value passed in
+        """
+        return op(self._value)
+
+    def or_else(self, op: object) -> Ok[T]:
         """
         The contained result is `Ok`, so return `Ok` with the original value
         """
-        return cast(Result[T, F], self)
+        return self
 
 
 class Err(Generic[E]):
     """
     A value that signifies failure and which stores arbitrary data for the error.
     """
 
@@ -174,18 +188,18 @@
 
     def __ne__(self, other: Any) -> bool:
         return not (self == other)
 
     def __hash__(self) -> int:
         return hash((False, self._value))
 
-    def is_ok(self) -> bool:
+    def is_ok(self) -> Literal[False]:
         return False
 
-    def is_err(self) -> bool:
+    def is_err(self) -> Literal[True]:
         return True
 
     def ok(self) -> None:
         """
         Return `None`.
         """
         return None
@@ -236,74 +250,89 @@
     def unwrap_or_else(self, op: Callable[[E], T]) -> T:
         """
         The contained result is ``Err``, so return the result of applying
         ``op`` to the error value.
         """
         return op(self._value)
 
-    def map(self, op: Callable[[T], U]) -> Result[U, E]:
+    def unwrap_or_raise(self, e: Type[TBE]) -> NoReturn:
+        """
+        The contained result is ``Err``, so raise the exception with the value.
+        """
+        raise e(self._value)
+
+    def map(self, op: object) -> Err[E]:
         """
         Return `Err` with the same value
         """
-        return cast(Result[U, E], self)
+        return self
 
-    def map_or(self, default: U, op: Callable[[T], U]) -> U:
+    def map_or(self, default: U, op: object) -> U:
         """
         Return the default value
         """
         return default
 
-    def map_or_else(
-        self,
-        default_op: Callable[[], U],
-        op: Callable[[T], U]
-    ) -> U:
+    def map_or_else(self, default_op: Callable[[], U], op: object) -> U:
         """
         Return the result of the default operation
         """
         return default_op()
 
-    def map_err(self, op: Callable[[E], F]) -> Result[T, F]:
+    def map_err(self, op: Callable[[E], F]) -> Err[F]:
         """
         The contained result is `Err`, so return `Err` with original error mapped to
         a new value using the passed in function.
         """
         return Err(op(self._value))
 
+    def and_then(self, op: object) -> Err[E]:
+        """
+        The contained result is `Err`, so return `Err` with the original value
+        """
+        return self
+
+    def or_else(self, op: Callable[[E], Result[T, F]]) -> Result[T, F]:
+        """
+        The contained result is `Err`, so return the result of `op` with the
+        original value passed in
+        """
+        return op(self._value)
+
 
 # define Result as a generic type alias for use
 # in type annotations
 """
 A simple `Result` type inspired by Rust.
 Not all methods (https://doc.rust-lang.org/std/result/enum.Result.html)
 have been implemented, only the ones that make sense in the Python context.
 """
-Result = Union[Ok[T], Err[E]]
+Result: TypeAlias = Union[Ok[T], Err[E]]
 
 """
 A type to use in `isinstance` checks.
 This is purely for convenience sake, as you could also just write `isinstance(res, (Ok, Err))
 """
-OkErr = (Ok, Err)
+OkErr: Final = (Ok, Err)
 
 
 class UnwrapError(Exception):
     """
     Exception raised from ``.unwrap_<...>`` and ``.expect_<...>`` calls.
 
     The original ``Result`` can be accessed via the ``.result`` attribute, but
     this is not intended for regular use, as type information is lost:
     ``UnwrapError`` doesn't know about both ``T`` and ``E``, since it's raised
     from ``Ok()`` or ``Err()`` which only knows about either ``T`` or ``E``,
     not both.
     """
 
-    _result: Result[Any, Any]
+    _result: Result[object, object]
 
-    def __init__(self, result: Result[Any, Any], message: str) -> None:
+    def __init__(self, result: Result[object, object], message: str) -> None:
         self._result = result
         super().__init__(message)
 
     @property
     def result(self) -> Result[Any, Any]:
         """
         Returns the original result.
```

### Comparing `result-0.8.0b1/src/result.egg-info/PKG-INFO` & `result-0.9.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: result
-Version: 0.8.0b1
-Summary: A Rust-like result type for Python
-Home-page: https://github.com/rustedpy/result
-Author: Danilo Bargen
-Author-email: mail@dbrgn.ch
-Maintainer: rustedpy github org members (https://github.com/rustedpy)
-License: MIT
-Keywords: rust,result,enum
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
-License-File: LICENSE
-
 ======
 Result
 ======
 
 .. image:: https://img.shields.io/github/workflow/status/rustedpy/result/CI/master
     :alt: GitHub Workflow Status (branch)
     :target: https://github.com/rustedpy/result/actions?query=workflow%3ACI+branch%3Amaster
@@ -31,14 +9,33 @@
 .. image:: https://codecov.io/gh/rustedpy/result/branch/master/graph/badge.svg
     :alt: Coverage
     :target: https://codecov.io/gh/rustedpy/result
 
 A simple Result type for Python 3 `inspired by Rust
 <https://doc.rust-lang.org/std/result/>`__, fully type annotated.
 
+Installation
+============
+
+Latest release:
+
+.. sourcecode:: sh
+
+   $ pip install result
+
+
+Latest GitHub ``master`` branch version:
+
+.. sourcecode:: sh
+
+   $ pip install git+https://github.com/rustedpy/result
+
+Summary
+=======
+
 The idea is that a result value can be either ``Ok(value)`` or ``Err(error)``,
 with a way to differentiate between the two. ``Ok`` and ``Err`` are both classes
 encapsulating an arbitrary value. ``Result[T, E]`` is a generic type alias for
 ``typing.Union[Ok[T], Err[E]]``. It will change code like this:
 
 .. sourcecode:: python
 
@@ -253,14 +250,26 @@
     >>> res2.unwrap_or('default')
     'default'
     >>> res1.unwrap_or_else(str.upper)
     'yay'
     >>> res2.unwrap_or_else(str.upper)
     'NAY'
 
+The ``unwrap`` method will raised an ``UnwrapError``. A custom exception can be
+raised by using the ``unwrap_or_raise`` method instead:
+
+.. sourcecode:: python
+
+    >>> res1 = Ok('yay')
+    >>> res2 = Err('nay')
+    >>> res1.unwrap_or_raise(ValueError)
+    'yay'
+    >>> res2.unwrap_or_raise(ValueError)
+    ValueError: nay
+
 Values and errors can be mapped using ``map``, ``map_or``, ``map_or_else`` and
 ``map_err``:
 
 .. sourcecode:: python
 
    >>> Ok(1).map(lambda x: x + 1)
    Ok(2)
@@ -337,9 +346,7 @@
 Otherwise using `one of these workarounds
 <https://github.com/python/mypy/issues/3889#issuecomment-325997911>`_ can help.
 
 License
 =======
 
 MIT License
-
-
```


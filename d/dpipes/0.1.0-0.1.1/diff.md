# Comparing `tmp/dpipes-0.1.0.tar.gz` & `tmp/dpipes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpipes-0.1.0.tar", last modified: Thu Apr 27 03:56:49 2023, max compression
+gzip compressed data, was "dpipes-0.1.1.tar", last modified: Sat Apr 29 04:28:27 2023, max compression
```

## Comparing `dpipes-0.1.0.tar` & `dpipes-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:56:49.791490 dpipes-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-27 03:56:49.791490 dpipes-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 03:56:37.000000 dpipes-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:56:49.791490 dpipes-0.1.0/dpipes/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 03:56:37.000000 dpipes-0.1.0/dpipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-27 03:56:37.000000 dpipes-0.1.0/dpipes/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-27 03:56:37.000000 dpipes-0.1.0/dpipes/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:56:49.791490 dpipes-0.1.0/dpipes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-27 03:56:49.000000 dpipes-0.1.0/dpipes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-27 03:56:49.000000 dpipes-0.1.0/dpipes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 03:56:49.000000 dpipes-0.1.0/dpipes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 03:56:49.000000 dpipes-0.1.0/dpipes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 03:56:49.000000 dpipes-0.1.0/dpipes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-27 03:56:37.000000 dpipes-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 03:56:49.791490 dpipes-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 03:56:49.791490 dpipes-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-27 03:56:37.000000 dpipes-0.1.0/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-27 03:56:37.000000 dpipes-0.1.0/tests/test_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:28:27.024623 dpipes-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-04-29 04:28:27.024623 dpipes-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-29 04:28:15.000000 dpipes-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:28:27.024623 dpipes-0.1.1/dpipes/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-29 04:28:15.000000 dpipes-0.1.1/dpipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-29 04:28:15.000000 dpipes-0.1.1/dpipes/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-29 04:28:15.000000 dpipes-0.1.1/dpipes/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:28:27.024623 dpipes-0.1.1/dpipes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-04-29 04:28:27.000000 dpipes-0.1.1/dpipes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-29 04:28:27.000000 dpipes-0.1.1/dpipes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 04:28:27.000000 dpipes-0.1.1/dpipes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-29 04:28:27.000000 dpipes-0.1.1/dpipes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 04:28:27.000000 dpipes-0.1.1/dpipes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-29 04:28:15.000000 dpipes-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 04:28:27.024623 dpipes-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:28:27.024623 dpipes-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-29 04:28:15.000000 dpipes-0.1.1/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-29 04:28:15.000000 dpipes-0.1.1/tests/test_processor.py
```

### Comparing `dpipes-0.1.0/dpipes/pipeline.py` & `dpipes-0.1.1/dpipes/pipeline.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,102 @@
 import functools
 import typing as T
 
 
 def make_pipeline(
     funcs: T.Sequence[T.Callable],
-    kwargs: T.Optional[T.Sequence[T.Optional[T.Dict[str, T.Any]]]],
+    kwargs: T.Optional[
+        T.Union[T.Dict[str, T.Any], T.Sequence[T.Optional[T.Dict[str, T.Any]]]]
+    ] = None,
 ) -> T.Callable:
     """
     Compose a pipeline from a sequence of functions.
 
     Parameters
     ----------
     funcs: Sequence[Callable]
         A sequence of callable functions.
-    kwargs: Optional[Sequence[Optional[Dict[str, Any]]]]
-        An optional, iterable collection of (optional) kwargs to apply respective functions to.
+    kwargs: Optional[Union[Dict[str, Any], Sequence[Optional[Dict[str, Any]]]
+        An iterable collection of kwargs to apply respective functions to. If a single set of
+        kwargs is passed they will be broadcast across the sequence of functions.
         Use `None` if a respective function does not require additional args.
 
     Returns
     -------
     Callable
         A pipeline composition function.
     """
     if kwargs:
         funcs = make_partials(funcs, kwargs)
     return functools.reduce(lambda f, g: lambda x: g(f(x)), funcs)
 
 
 def make_partials(
-    funcs: T.Sequence[T.Callable], kwargs: T.Sequence[T.Optional[T.Dict[str, T.Any]]]
+    funcs: T.Sequence[T.Callable],
+    kwargs: T.Union[T.Dict[str, T.Any], T.Sequence[T.Optional[T.Dict[str, T.Any]]]],
 ) -> T.Sequence[T.Callable]:
     """
     Create a sequence of partial functions.
 
     Parameters
     ----------
     funcs: Sequence[Callable]
         A sequence of callable functions.
-    kwargs: Sequence[Optional[Dict[str, Any]]]
-        An iterable collection of (optional) kwargs to apply respective functions to. Use `None` if
-        a respective function does not require additional args.
+    kwargs: Union[Dict[str, Any], Sequence[Optional[Dict[str, Any]]
+        An iterable collection of kwargs to apply respective functions to. If a single set of
+        kwargs is passed they will be broadcast across the sequence of functions.
+        Use `None` if a respective function does not require additional args.
 
     Returns
     -------
     Sequence[Callable]
         A sequence of partial functions.
     """
+    if isinstance(kwargs, dict):
+        # broadcast single dict
+        return [functools.partial(f, **kwargs) for f in funcs]
     return [functools.partial(f, **kw) if kw else f for f, kw in zip(funcs, kwargs)]
 
 
 class Pipeline:
     """
     Class to sequentially process an arbitrary number of functions.
     """
 
     def __init__(
         self,
         funcs: T.Sequence[T.Callable],
-        kwargs: T.Optional[T.Sequence[T.Optional[T.Dict[str, T.Any]]]] = None,
+        kwargs: T.Optional[
+            T.Union[T.Dict[str, T.Any], T.Sequence[T.Optional[T.Dict[str, T.Any]]]]
+        ] = None,
     ):
         """
         Instantiate a Pipeline object.
 
         Parameters
         ----------
         funcs: Sequence[Callable]
             A sequence of callable functions.
-        kwargs: Optional[Sequence[Optional[Dict[str, Any]]]]
-            An optional, iterable collection of (optional) kwargs to apply respective functions to.
+        kwargs: Optional[Union[Dict[str, Any], Sequence[Optional[Dict[str, Any]]]
+            An iterable collection of kwargs to apply respective functions to. If a single set of
+            kwargs is passed they will be broadcast across the sequence of functions.
             Use `None` if a respective function does not require additional args.
         """
+        if kwargs:
+            if isinstance(kwargs, T.Sequence):
+                self._check_args(funcs, kwargs)
         self.funcs = funcs
         self.kwargs = kwargs
 
     def __call__(self, x):
         reducer = make_pipeline(self.funcs, self.kwargs)
         return reducer(x)
+
+    @staticmethod
+    def _check_args(funcs, args):
+        if len(funcs) != len(args):
+            raise ValueError(
+                f"""
+                    Length of `kwargs` must match length of `funcs`.
+                    Expected {len(funcs)} collections of kwargs, only got {len(args)}.
+                    """
+            )
```

### Comparing `dpipes-0.1.0/dpipes/processor.py` & `dpipes-0.1.1/dpipes/processor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,23 @@
 import functools
 import typing as T
 
+from dpipes.pipeline import Pipeline, make_partials
 
-class PipeProcessor:
+
+class PipeProcessor(Pipeline):
     """
     Class to sequentially process an arbitrary number of pandas.DataFrame.pipe functions.
     """
 
-    def __init__(
-        self,
-        funcs: T.Sequence[T.Callable],
-        kwargs: T.Optional[
-            T.Union[
-                T.Dict[str, T.Union[str, T.Sequence[str]]],
-                T.Sequence[T.Dict[str, T.Union[str, T.Sequence[str]]]],
-            ]
-        ] = None,
-    ):
-        """
-        Instantiate processor.
-
-        Parameters
-        ----------
-        funcs: Sequence[Callable]
-            An iterable collection of user-defined functions.
-        kwargs: Optional[Union[Dict, Sequence[Dict[str, Union[str, Sequence[str]]]]
-            An iterable collection of kwargs to apply respective functions to. If a single set
-            of kwargs is passed they will be broadcast across the sequence of functions.
-
-        Returns
-        -------
-        pd.DataFrame
-            A processed DataFrame.
-        """
-        if kwargs:
-            # broadcast single dict
-            if isinstance(kwargs, dict):
-                self.funcs = [functools.partial(f, **kwargs) for f in funcs]
-
-            else:
-                self._check_args(funcs, kwargs)
-                self.funcs = [
-                    functools.partial(f, **kw) if kw else f
-                    for f, kw in zip(funcs, kwargs)
-                ]
-        else:
-            self.funcs = funcs
-
     def __call__(self, df):
+        if self.kwargs:
+            self.funcs = make_partials(self.funcs, self.kwargs)
         return functools.reduce(lambda _df, trans: _df.pipe(trans), self.funcs, df)
 
-    @staticmethod
-    def _check_args(funcs, args):
-        if len(funcs) != len(args):
-            raise ValueError(
-                f"""
-                Length of `kwargs` must match length of `funcs`.
-                Expected {len(funcs)} collections of kwargs, only got {len(args)}.
-                """
-            )
-
 
 class ColumnPipeProcessor(PipeProcessor):
     """
     Class to sequentially process an arbitrary number of pandas.DataFrame.pipe functions by column.
     """
 
     def __init__(
```

### Comparing `dpipes-0.1.0/pyproject.toml` & `dpipes-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -13,30 +13,43 @@
     "pre-commit-hooks>=4.4.0",
     "pyright>=1.1.304",
     "nox>=2023.4.22",
 ]
 docs = [
     "mkdocs-material>=9.1.8",
     "mkdocstrings-python>=0.9.0",
+    "mkdocs-table-reader-plugin>=2.0",
 ]
 
 [project]
 name = "dpipes"
-version = "0.1.0"
+version = "0.1.1"
 description = "dPipes - Pythonic Data Pipelines"
 authors = [
     {name = "Chris Santiago", email = "cjsantiago@gatech.edu"},
 ]
 dependencies = [
     "pandas>=1.0.0",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 readme = "README.md"
 license = {text = "MIT"}
 
+
+[project.urls]
+"Sourcecode" = "https://github.com/chris-santiago/dpipes"
+"Documentation" = "https://chris-santiago.github.io/dpipes/"
+
+
+[project.optional-dependencies]
+demo = [
+    "polars>=0.17.9",
+    "openpyxl>=3.1.2",
+    "nltk>=3.8.1",
+]
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [tool.ruff]
 line-length = 100
```

### Comparing `dpipes-0.1.0/tests/test_processor.py` & `dpipes-0.1.1/tests/test_processor.py`

 * *Files identical despite different names*


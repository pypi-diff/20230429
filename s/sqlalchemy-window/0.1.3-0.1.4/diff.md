# Comparing `tmp/sqlalchemy_window-0.1.3.tar.gz` & `tmp/sqlalchemy_window-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sqlalchemy-window/sqlalchemy-window/dist/.tmp-o6lgvj2s/sqlalchemy_window-0.1.3.tar", last modified: Sat Apr 22 09:24:07 2023, max compression
+gzip compressed data, was "/home/runner/work/sqlalchemy-window/sqlalchemy-window/dist/.tmp-d6nho6kx/sqlalchemy_window-0.1.4.tar", last modified: Sat Apr 29 09:21:12 2023, max compression
```

## Comparing `sqlalchemy_window-0.1.3.tar` & `sqlalchemy_window-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-22 09:23:46.000000 sqlalchemy_window-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-22 09:23:46.000000 sqlalchemy_window-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-22 09:23:46.000000 sqlalchemy_window-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-22 09:23:46.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-22 09:23:46.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window/_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-04-22 09:23:46.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window/_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/src/sqlalchemy_window.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:24:07.000000 sqlalchemy_window-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-22 09:23:46.000000 sqlalchemy_window-0.1.3/tests/test_over_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-22 09:23:46.000000 sqlalchemy_window-0.1.3/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-04-22 09:23:46.000000 sqlalchemy_window-0.1.3/tests/test_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:21:12.000000 sqlalchemy_window-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-29 09:20:52.000000 sqlalchemy_window-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-29 09:21:12.000000 sqlalchemy_window-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-29 09:20:52.000000 sqlalchemy_window-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-29 09:20:52.000000 sqlalchemy_window-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 09:21:12.000000 sqlalchemy_window-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:21:12.000000 sqlalchemy_window-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:21:12.000000 sqlalchemy_window-0.1.4/src/sqlalchemy_window/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-29 09:20:52.000000 sqlalchemy_window-0.1.4/src/sqlalchemy_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-29 09:20:52.000000 sqlalchemy_window-0.1.4/src/sqlalchemy_window/_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-04-29 09:20:52.000000 sqlalchemy_window-0.1.4/src/sqlalchemy_window/_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:21:12.000000 sqlalchemy_window-0.1.4/src/sqlalchemy_window.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-29 09:21:12.000000 sqlalchemy_window-0.1.4/src/sqlalchemy_window.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-29 09:21:12.000000 sqlalchemy_window-0.1.4/src/sqlalchemy_window.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 09:21:12.000000 sqlalchemy_window-0.1.4/src/sqlalchemy_window.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 09:21:12.000000 sqlalchemy_window-0.1.4/src/sqlalchemy_window.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-29 09:21:12.000000 sqlalchemy_window-0.1.4/src/sqlalchemy_window.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:21:12.000000 sqlalchemy_window-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-29 09:20:52.000000 sqlalchemy_window-0.1.4/tests/test_over_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-29 09:20:52.000000 sqlalchemy_window-0.1.4/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-04-29 09:20:52.000000 sqlalchemy_window-0.1.4/tests/test_window.py
```

### Comparing `sqlalchemy_window-0.1.3/LICENSE` & `sqlalchemy_window-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_window-0.1.3/PKG-INFO` & `sqlalchemy_window-0.1.4/src/sqlalchemy_window.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sqlalchemy_window
-Version: 0.1.3
+Name: sqlalchemy-window
+Version: 0.1.4
 Summary: A SQLAlchemy plugin to add support for PostgreSQL WINDOW clause
 Author-email: Roman Necheporenko <roman@waterfountain.one>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `sqlalchemy_window-0.1.3/README.md` & `sqlalchemy_window-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_window-0.1.3/pyproject.toml` & `sqlalchemy_window-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sqlalchemy_window-0.1.3/src/sqlalchemy_window/_select.py` & `sqlalchemy_window-0.1.4/src/sqlalchemy_window/_select.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 if typing.TYPE_CHECKING:  # pragma: no cover
     from sqlalchemy.sql._typing import _ColumnsClauseArgument
 
 
 class Select(_Select):
     """Custom `Select` construct with WINDOW clause support."""
 
+    inherit_cache: bool = True
+
     _window_clause: typing.Tuple[Window, ...] = ()
 
     def window(self, *windows: Window) -> "Select":
         """Return a new `Select` object with extended WINDOW clause."""
         assert isinstance(self._window_clause, tuple)
         self._window_clause += windows
         return self
```

### Comparing `sqlalchemy_window-0.1.3/src/sqlalchemy_window/_window.py` & `sqlalchemy_window-0.1.4/src/sqlalchemy_window/_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 class OverWindow(ColumnElement[_FT]):
     """Represent an `OVER` statement for window functions.
 
     Do not construct directly, rather through a
     `sqlalchemy_window.over_window` factory.
     """
 
+    inherit_cache: bool = True
+
     def __init__(self, element: FunctionElement[_FT], window: "Window") -> None:
         self.element = element
         self.window = window
 
     @property
     def type(self):
         return self.element.type
@@ -91,14 +93,16 @@
     Do not use this element directly, rather through a
     `sqlalchemy_window.window` factory.
 
     For more information, see:
     https://www.postgresql.org/docs/current/sql-select.html#SQL-WINDOW
     """
 
+    inherit_cache: bool = True
+
     partition_by: typing.Optional[ClauseList] = None
     order_by: typing.Optional[ClauseList] = None
 
     range_: typing.Optional[_RangeType] = None
     rows: typing.Optional[_RangeType] = None
     groups: typing.Optional[_RangeType] = None
```

### Comparing `sqlalchemy_window-0.1.3/src/sqlalchemy_window.egg-info/PKG-INFO` & `sqlalchemy_window-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sqlalchemy-window
-Version: 0.1.3
+Name: sqlalchemy_window
+Version: 0.1.4
 Summary: A SQLAlchemy plugin to add support for PostgreSQL WINDOW clause
 Author-email: Roman Necheporenko <roman@waterfountain.one>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `sqlalchemy_window-0.1.3/tests/test_over_window.py` & `sqlalchemy_window-0.1.4/tests/test_over_window.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_window-0.1.3/tests/test_select.py` & `sqlalchemy_window-0.1.4/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_window-0.1.3/tests/test_window.py` & `sqlalchemy_window-0.1.4/tests/test_window.py`

 * *Files identical despite different names*


# Comparing `tmp/databind.core-4.2.4.tar.gz` & `tmp/databind.core-4.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databind.core-4.2.4.tar", max compression
+gzip compressed data, was "databind.core-4.2.5.tar", max compression
```

## Comparing `databind.core-4.2.4.tar` & `databind.core-4.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1727 2023-04-12 22:47:04.968499 databind.core-4.2.4/pyproject.toml
--rw-r--r--   0        0        0     1245 2023-03-01 15:01:37.487224 databind.core-4.2.4/readme.md
--rw-r--r--   0        0        0       22 2023-04-12 22:47:04.968499 databind.core-4.2.4/src/databind/core/__init__.py
--rw-r--r--   0        0        0     5558 2023-04-12 21:58:39.471732 databind.core-4.2.4/src/databind/core/context.py
--rw-r--r--   0        0        0     4869 2023-04-12 21:47:28.043974 databind.core-4.2.4/src/databind/core/converter.py
--rw-r--r--   0        0        0     4099 2023-04-12 21:58:39.471732 databind.core-4.2.4/src/databind/core/dataclasses.py
--rw-r--r--   0        0        0     7120 2023-03-01 15:01:37.487224 databind.core-4.2.4/src/databind/core/dataclasses.pyi
--rw-r--r--   0        0        0     3943 2023-03-01 15:01:37.487224 databind.core-4.2.4/src/databind/core/mapper.py
--rw-r--r--   0        0        0        0 2023-03-01 15:01:37.487224 databind.core-4.2.4/src/databind/core/py.typed
--rw-r--r--   0        0        0    15234 2023-04-12 22:46:53.368366 databind.core-4.2.4/src/databind/core/schema.py
--rw-r--r--   0        0        0    26830 2023-04-12 21:58:39.471732 databind.core-4.2.4/src/databind/core/settings.py
--rw-r--r--   0        0        0     8709 2023-03-01 15:01:37.487224 databind.core-4.2.4/src/databind/core/union.py
--rw-r--r--   0        0        0     2955 2023-03-01 15:01:37.487224 databind.core-4.2.4/src/databind/core/utils.py
--rw-r--r--   0        0        0     2186 2023-04-12 22:47:18.282069 databind.core-4.2.4/setup.py
--rw-r--r--   0        0        0     2343 2023-04-12 22:47:18.282426 databind.core-4.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1727 2023-04-29 16:35:15.655751 databind.core-4.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1245 2023-04-29 16:34:38.888783 databind.core-4.2.5/readme.md
+-rw-r--r--   0        0        0       22 2023-04-29 16:35:15.655751 databind.core-4.2.5/src/databind/core/__init__.py
+-rw-r--r--   0        0        0     5481 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/context.py
+-rw-r--r--   0        0        0     6059 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/converter.py
+-rw-r--r--   0        0        0     4099 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/dataclasses.py
+-rw-r--r--   0        0        0     7120 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/dataclasses.pyi
+-rw-r--r--   0        0        0     3943 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/mapper.py
+-rw-r--r--   0        0        0        0 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/py.typed
+-rw-r--r--   0        0        0    15234 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/schema.py
+-rw-r--r--   0        0        0    26830 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/settings.py
+-rw-r--r--   0        0        0     8709 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/union.py
+-rw-r--r--   0        0        0     2955 2023-04-29 16:34:38.888783 databind.core-4.2.5/src/databind/core/utils.py
+-rw-r--r--   0        0        0     2186 2023-04-29 16:35:23.687455 databind.core-4.2.5/setup.py
+-rw-r--r--   0        0        0     2343 2023-04-29 16:35:23.687663 databind.core-4.2.5/PKG-INFO
```

### Comparing `databind.core-4.2.4/pyproject.toml` & `databind.core-4.2.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databind.core"
-version = "4.2.4"
+version = "4.2.5"
 description = "Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{include = "databind/core", from = "src"}]
 
 [tool.poetry.urls]
```

### Comparing `databind.core-4.2.4/readme.md` & `databind.core-4.2.5/readme.md`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.4/src/databind/core/context.py` & `databind.core-4.2.5/src/databind/core/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,27 +64,26 @@
     #: A list of #Setting#s that are to be taken into account by the converter which can potentialy impact
     #: the conversion process.
     settings: "SettingsProvider" = dataclasses.field(repr=False)
 
     #: The key or index under which #value is present in the source material relative to the #parent context.
     #: This is `None` only for the root value in the same source. The value must be #Context.ROOT if the context
     #: has no parent.
-    key: t.Union[int, str, Root, None]
+    key: t.Union[int, str, Root, None, t.Any]
 
     #: The location of the #value in the source material.
     location: Location
 
     #: A function to dispatch the further conversion of a #Context.
     convert_func: t.Callable[["Context"], t.Any] = dataclasses.field(repr=False)
 
     ROOT: t.ClassVar = Root.Value
 
     def __post_init__(self) -> None:
         assert isinstance(self.datatype, TypeHint), self.datatype
-        assert isinstance(self.key, (int, str, Root)) or self.key is None, self.key
         assert self.location is not None
         assert self.parent is not None or self.key == Context.ROOT
 
     def get_setting(self, setting_type: t.Type["T_Setting"]) -> "T_Setting | None":
         """Retrieve a setting by type that for the current context."""
 
         return self.settings.get_setting(self, setting_type)
```

### Comparing `databind.core-4.2.4/src/databind/core/converter.py` & `databind.core-4.2.5/src/databind/core/converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import abc
 import logging
 import typing as t
 from textwrap import indent
 
-from typeapi import type_repr
+from typeapi import ClassTypeHint, type_repr
 
 from databind.core.utils import exception_safe_str
 
 if t.TYPE_CHECKING:
     from databind.core.context import Context
 
 logger = logging.getLogger(__name__)
@@ -137,7 +137,31 @@
         super().__init__(
             origin,
             context,
             f"no {context.direction.name.lower()}r for `{context.datatype}` and payload of type "
             f"`{type_repr(type(context.value))}`",
             errors,
         )
+
+
+class DelegateToClassmethodConverter(Converter):
+    """
+    This converter delegaes to the methods defined by name to perform serialization and deserialization of a type. This
+    converter is usually used in conjunction with settings that override the converteer to be used in a specifc
+    scenario (e.g. such as de/serializing JSON with the #databind.json.settings.JsonConverter setting).
+    """
+
+    def __init__(self, *, serialize: "str | None" = None, deserialize: "str | None" = None) -> None:
+        self._serialize = serialize
+        self._deserialize = deserialize
+
+    def serialize(self, ctx: "Context") -> t.Any:
+        if self._serialize is None or not isinstance(ctx.datatype, ClassTypeHint):
+            raise NotImplementedError
+        method: t.Callable[[t.Any], t.Any] = getattr(ctx.datatype.type, self._serialize)
+        return method(ctx.value)
+
+    def deserialize(self, ctx: "Context") -> t.Any:
+        if self._deserialize is None or not isinstance(ctx.datatype, ClassTypeHint):
+            raise NotImplementedError
+        method: t.Callable[[t.Any], t.Any] = getattr(ctx.datatype.type, self._deserialize)
+        return method(ctx.value)
```

### Comparing `databind.core-4.2.4/src/databind/core/dataclasses.py` & `databind.core-4.2.5/src/databind/core/dataclasses.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.4/src/databind/core/dataclasses.pyi` & `databind.core-4.2.5/src/databind/core/dataclasses.pyi`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.4/src/databind/core/mapper.py` & `databind.core-4.2.5/src/databind/core/mapper.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.4/src/databind/core/schema.py` & `databind.core-4.2.5/src/databind/core/schema.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.4/src/databind/core/settings.py` & `databind.core-4.2.5/src/databind/core/settings.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.4/src/databind/core/union.py` & `databind.core-4.2.5/src/databind/core/union.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.4/src/databind/core/utils.py` & `databind.core-4.2.5/src/databind/core/utils.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.4/setup.py` & `databind.core-4.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'nr-date>=2.0.0,<3.0.0',
  'nr-stream>=1.0.0,<2.0.0',
  'typeapi>=1.4.2,<2.0.0',
  'typing-extensions>=3.10.0']
 
 setup_kwargs = {
     'name': 'databind.core',
-    'version': '4.2.4',
+    'version': '4.2.5',
     'description': 'Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer.',
     'long_description': '# databind.core\n\n`databind.core` provides a jackson-databind inspired framework for data de-/serialization in Python. Unless you\nare looking to implement support for de-/serializing new data formats, the `databind.core` package alone might\nnot be what you are looking for (unless you want to use `databind.core.dataclasses` as a drop-in replacement to\nthe standard library `dataclasses` module, for that check out the section at the bottom).\n\n### Known implementations\n\n* [databind.json](https://pypi.org/project/databind.json)\n\n### Dataclass extension\n\nThe standard library `dataclasses` module does not allow to define non-default arguments after default arguments.\nYou can use `databind.core.dataclasses` as a drop-in replacement to get this feature. It behaves exactly like the\nstandard library, only that non-default arguments may follow default arguments. Such arguments can be passed to\nthe constructor as positional or keyword arguments.\n\n```py\nfrom databind.core import dataclasses\n\n@dataclasses.dataclass\nclass A:\n  value1: int = 42\n\n@dataclasses.dataclass\nclass B(A):\n  value2: str\n\nprint(B(0, \'Hello, World!\'))\nprint(B(value2=\'Answer to the universe\'))\n```\n\n---\n\n<p align="center">Copyright &copy; 2020 &ndash; Niklas Rosenstein</p>\n',
     'author': 'Niklas Rosenstein',
     'author_email': 'rosensteinniklas@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `databind.core-4.2.4/PKG-INFO` & `databind.core-4.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databind.core
-Version: 4.2.4
+Version: 4.2.5
 Summary: Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


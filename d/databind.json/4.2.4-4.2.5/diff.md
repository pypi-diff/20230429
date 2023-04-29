# Comparing `tmp/databind.json-4.2.4.tar.gz` & `tmp/databind.json-4.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databind.json-4.2.4.tar", max compression
+gzip compressed data, was "databind.json-4.2.5.tar", max compression
```

## Comparing `databind.json-4.2.4.tar` & `databind.json-4.2.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1600 2023-04-12 22:47:04.968499 databind.json-4.2.4/pyproject.toml
--rw-r--r--   0        0        0     3339 2023-03-01 15:01:37.487224 databind.json-4.2.4/readme.md
--rw-r--r--   0        0        0     2358 2023-04-12 22:47:04.968499 databind.json-4.2.4/src/databind/json/__init__.py
--rw-r--r--   0        0        0    33037 2023-03-01 15:01:37.487224 databind.json-4.2.4/src/databind/json/converters.py
--rw-r--r--   0        0        0     2706 2023-03-01 15:01:37.487224 databind.json-4.2.4/src/databind/json/module.py
--rw-r--r--   0        0        0        0 2023-03-01 15:01:37.487224 databind.json-4.2.4/src/databind/json/py.typed
--rw-r--r--   0        0        0     1364 2023-03-01 15:01:37.487224 databind.json-4.2.4/src/databind/json/settings.py
--rw-r--r--   0        0        0     4232 2023-04-12 22:47:19.567597 databind.json-4.2.4/setup.py
--rw-r--r--   0        0        0     4368 2023-04-12 22:47:19.568039 databind.json-4.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1600 2023-04-29 16:35:15.655751 databind.json-4.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3339 2023-04-29 16:34:38.892782 databind.json-4.2.5/readme.md
+-rw-r--r--   0        0        0     2358 2023-04-29 16:35:15.655751 databind.json-4.2.5/src/databind/json/__init__.py
+-rw-r--r--   0        0        0    33037 2023-04-29 16:34:38.892782 databind.json-4.2.5/src/databind/json/converters.py
+-rw-r--r--   0        0        0     2706 2023-04-29 16:34:38.892782 databind.json-4.2.5/src/databind/json/module.py
+-rw-r--r--   0        0        0        0 2023-04-29 16:34:38.892782 databind.json-4.2.5/src/databind/json/py.typed
+-rw-r--r--   0        0        0     1773 2023-04-29 16:34:38.892782 databind.json-4.2.5/src/databind/json/settings.py
+-rw-r--r--   0        0        0     4232 2023-04-29 16:35:24.438432 databind.json-4.2.5/setup.py
+-rw-r--r--   0        0        0     4368 2023-04-29 16:35:24.438818 databind.json-4.2.5/PKG-INFO
```

### Comparing `databind.json-4.2.4/pyproject.toml` & `databind.json-4.2.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "databind.json"
-version = "4.2.4"
+version = "4.2.5"
 description = "De-/serialize Python dataclasses to or from JSON payloads. Compatible with Python 3.7 and newer."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{include = "databind/json", from = "src"}]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/NiklasRosenstein/python-databind/issues"
 Documentation = "https://niklasrosenstein.github.io/python-databind/"
 # Homepage = ""
 Repository = "https://github.com/NiklasRosenstein/python-databind"
 
 [tool.poetry.dependencies]
 python = "^3.6.3"
-"databind.core" = "^4.2.4"
+"databind.core" = "^4.2.5"
 nr-date = "^2.0.0"
 typeapi = "^1.4.2"
 typing-extensions = ">=3.10.0"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 flake8 = "*"
```

### Comparing `databind.json-4.2.4/readme.md` & `databind.json-4.2.5/readme.md`

 * *Files identical despite different names*

### Comparing `databind.json-4.2.4/src/databind/json/__init__.py` & `databind.json-4.2.5/src/databind/json/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from databind.core.utils import T
 
 if t.TYPE_CHECKING:
     from databind.core.mapper import ObjectMapper
     from databind.core.settings import Setting, Settings
 
-__version__ = "4.2.4"
+__version__ = "4.2.5"
 
 JsonType = t.Union[
     None,
     bool,
     int,
     float,
     str,
```

### Comparing `databind.json-4.2.4/src/databind/json/converters.py` & `databind.json-4.2.5/src/databind/json/converters.py`

 * *Files identical despite different names*

### Comparing `databind.json-4.2.4/src/databind/json/module.py` & `databind.json-4.2.5/src/databind/json/module.py`

 * *Files identical despite different names*

### Comparing `databind.json-4.2.4/setup.py` & `databind.json-4.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 packages = \
 ['json']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['databind.core>=4.2.4,<5.0.0',
+['databind.core>=4.2.5,<5.0.0',
  'nr-date>=2.0.0,<3.0.0',
  'typeapi>=1.4.2,<2.0.0',
  'typing-extensions>=3.10.0']
 
 setup_kwargs = {
     'name': 'databind.json',
-    'version': '4.2.4',
+    'version': '4.2.5',
     'description': 'De-/serialize Python dataclasses to or from JSON payloads. Compatible with Python 3.7 and newer.',
     'long_description': '# databind.json\n\nThe `databind.json` package implements the de-/serialization to or from JSON payloads using\nthe `databind.core` framework.\n\nCheck out the [Documentation][0] for examples.\n\n[0]: https://niklasrosenstein.github.io/python-databind/\n\n## Built-in converters\n\nThe following tables shows which types can be deserialized from / serialize to Python types with the native\nconverters provided by the `databind.json` module:\n\n| Converter name | Types | Description |\n| -------------- | ----- | ----------- |\n| `AnyConverter` | `typing.Any` | Accept any value (useful for arbitrary JSON). |\n| `CollectionConverter` | `typing.Collection[T]`, excl. `str`, `bytes`, `bytearray`, `memoryview` and `typing.Mapping[K, V]` | Converts between native Python collections and JSON arrays. |\n| `DatetimeConverter` | `datetime.date`, `datetime.datetime`, `datetime.time` | Converts between strings and date/time formats, using ISO 8601 time format by default (can be changed with the `databind.core.settings.DateFormat` setting). |\n| `DecimalConverter` | `decimal.Decimal` | Converts between strings (and ints/floats if strict mode is off, strict mode is on by default) and decimals. The precision can be controlled with the `databind.core.settings.Precision` setting. |\n| `EnumConverter` | `enum.Enum`, `enum.IntEnum` | Convert between strings and Python enumerations. The serialized form of `IntEnum` is the integer value, whereas the serialized form of `Enum` is a string (name of the enumeration value). |\n| `MappingConverter` | `typing.Mapping[K, V]` | Converts between Python dicts and JSON objects. (While in theory `K` can be any type, for JSON `K` always needs to be `str`). |\n| `OptionalConverter` | `typing.Optional[T]` | Handles optional fields in a schema. |\n| `PlainDatatypeConverter` | `bytes`, `str`, `int`, `float`, `bool` | Converts between plain datatypes. In non-strict mode (off by default), numeric types will also accept strings as input for the deserialization. |\n| `SchemaConverter` | `dataclasses.dataclass`, `typing.TypedDict` | Converts between Python dataclasses or typed dictionary and JSON objects. |\n| `UnionConverter` | `typing.Union[...]` | Handles union types. Unions in JSON can be expressed in a multitide of ways, e.g. using a discriminator key and flat, keyed or nested structure or "best match". Check out the examples section of the documentation for more information. |\n| `LiteralConverter` | `typing.Literal[...]` | Accepts or rejects a value based on whether it matches one of the values in the literal type hint. |\n\n\nThe following converters are provided for convenience:\n\n| Converter name | Types | Description |\n| -------------- | ----- | ----------- |\n| `StringifyConverter` | n/a | A helper that allows to easily create de/serializers from a "to string" and "from string" function. |\n\nThe following additional types are natively supported by `databind.json` using `StringifyConverter`:\n\n| Types | Description |\n| ----- | ----------- |\n| `uuid.UUID` | Convert between strings and UUIDs. |\n| `pathlib.Path` | Convert between strings and paths. |\n| `pathlib.PurePath` | Convert between strings and paths. |\n| `nr.date.duration` | Deserialize from ISO 8601 duration strings or the object form, serialize to ISO 8601 strings. |\n\n---\n\n<p align="center">Copyright &copy; 2020 &ndash; Niklas Rosenstein</p>\n',
     'author': 'Niklas Rosenstein',
     'author_email': 'rosensteinniklas@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `databind.json-4.2.4/PKG-INFO` & `databind.json-4.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: databind.json
-Version: 4.2.4
+Version: 4.2.5
 Summary: De-/serialize Python dataclasses to or from JSON payloads. Compatible with Python 3.7 and newer.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: databind.core (>=4.2.4,<5.0.0)
+Requires-Dist: databind.core (>=4.2.5,<5.0.0)
 Requires-Dist: nr-date (>=2.0.0,<3.0.0)
 Requires-Dist: typeapi (>=1.4.2,<2.0.0)
 Requires-Dist: typing-extensions (>=3.10.0)
 Project-URL: Bug Tracker, https://github.com/NiklasRosenstein/python-databind/issues
 Project-URL: Documentation, https://niklasrosenstein.github.io/python-databind/
 Project-URL: Repository, https://github.com/NiklasRosenstein/python-databind
 Description-Content-Type: text/markdown
```


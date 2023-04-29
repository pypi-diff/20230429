# Comparing `tmp/types-chardet-5.0.4.4.tar.gz` & `tmp/types-chardet-5.0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-chardet-5.0.4.4.tar", last modified: Mon Apr 24 12:29:59 2023, max compression
+gzip compressed data, was "types-chardet-5.0.4.5.tar", last modified: Sat Apr 29 15:14:05 2023, max compression
```

## Comparing `types-chardet-5.0.4.4.tar` & `types-chardet-5.0.4.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:29:59.953324 types-chardet-5.0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-24 12:29:57.000000 types-chardet-5.0.4.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 12:29:57.000000 types-chardet-5.0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-24 12:29:59.953324 types-chardet-5.0.4.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:29:59.949324 types-chardet-5.0.4.4/chardet-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-24 12:29:57.000000 types-chardet-5.0.4.4/chardet-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-24 12:29:41.000000 types-chardet-5.0.4.4/chardet-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-24 12:29:41.000000 types-chardet-5.0.4.4/chardet-stubs/enums.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-24 12:29:41.000000 types-chardet-5.0.4.4/chardet-stubs/langbulgarianmodel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-24 12:29:41.000000 types-chardet-5.0.4.4/chardet-stubs/langcyrillicmodel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-24 12:29:41.000000 types-chardet-5.0.4.4/chardet-stubs/langgreekmodel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 12:29:41.000000 types-chardet-5.0.4.4/chardet-stubs/langhebrewmodel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-24 12:29:41.000000 types-chardet-5.0.4.4/chardet-stubs/langhungarianmodel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-24 12:29:41.000000 types-chardet-5.0.4.4/chardet-stubs/langthaimodel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-24 12:29:41.000000 types-chardet-5.0.4.4/chardet-stubs/langturkishmodel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-24 12:29:41.000000 types-chardet-5.0.4.4/chardet-stubs/universaldetector.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 12:29:41.000000 types-chardet-5.0.4.4/chardet-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 12:29:59.953324 types-chardet-5.0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-24 12:29:57.000000 types-chardet-5.0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:29:59.949324 types-chardet-5.0.4.4/types_chardet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-24 12:29:59.000000 types-chardet-5.0.4.4/types_chardet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-24 12:29:59.000000 types-chardet-5.0.4.4/types_chardet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:29:59.000000 types-chardet-5.0.4.4/types_chardet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 12:29:59.000000 types-chardet-5.0.4.4/types_chardet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:05.828437 types-chardet-5.0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-29 15:14:05.000000 types-chardet-5.0.4.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 15:14:05.000000 types-chardet-5.0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-29 15:14:05.828437 types-chardet-5.0.4.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:05.828437 types-chardet-5.0.4.5/chardet-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-29 15:14:05.000000 types-chardet-5.0.4.5/chardet-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/langbulgarianmodel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/langcyrillicmodel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/langgreekmodel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/langhebrewmodel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/langhungarianmodel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/langthaimodel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/langturkishmodel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/universaldetector.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:14:05.832437 types-chardet-5.0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-29 15:14:05.000000 types-chardet-5.0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:05.828437 types-chardet-5.0.4.5/types_chardet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-29 15:14:05.000000 types-chardet-5.0.4.5/types_chardet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-29 15:14:05.000000 types-chardet-5.0.4.5/types_chardet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:14:05.000000 types-chardet-5.0.4.5/types_chardet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-29 15:14:05.000000 types-chardet-5.0.4.5/types_chardet.egg-info/top_level.txt
```

### Comparing `types-chardet-5.0.4.4/CHANGELOG.md` & `types-chardet-5.0.4.5/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+## 5.0.4.5 (2023-04-29)
+
+chardet: UniversalDetector.feed accepts bytearray (#10107)
+
+Technically it accepts any buffer, but the inline type annotations
+now say bytes | bytearray, so let's stick to that.
+
+Part of #9006
+
 ## 5.0.4.4 (2023-04-24)
 
 Simplify `chardet` type imports (#10080)
 
 ## 5.0.4.3 (2023-03-27)
 
 Add defaults for third-party stubs A-D (#9952)
```

### Comparing `types-chardet-5.0.4.4/PKG-INFO` & `types-chardet-5.0.4.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-chardet
-Version: 5.0.4.4
+Version: 5.0.4.5
 Summary: Typing stubs for chardet
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/chardet.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,8 +27,8 @@
 
 *Note:* The `chardet` package includes type annotations or type stubs
 since version 5.1.0. Please uninstall the `types-chardet`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `22ced496450a29ecae2cc4f7d5d163185ca6a75f`.
+This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
```

### Comparing `types-chardet-5.0.4.4/chardet-stubs/__init__.pyi` & `types-chardet-5.0.4.5/chardet-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-chardet-5.0.4.4/chardet-stubs/enums.pyi` & `types-chardet-5.0.4.5/chardet-stubs/enums.pyi`

 * *Files identical despite different names*

### Comparing `types-chardet-5.0.4.4/chardet-stubs/universaldetector.pyi` & `types-chardet-5.0.4.5/chardet-stubs/universaldetector.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -21,9 +21,9 @@
 
     result: _IntermediateResultType
     done: bool
     lang_filter: int
     logger: Logger
     def __init__(self, lang_filter: int = 31) -> None: ...
     def reset(self) -> None: ...
-    def feed(self, byte_str: bytes) -> None: ...
+    def feed(self, byte_str: bytes | bytearray) -> None: ...
     def close(self) -> _FinalResultType: ...
```

### Comparing `types-chardet-5.0.4.4/setup.py` & `types-chardet-5.0.4.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
 *Note:* The `chardet` package includes type annotations or type stubs
 since version 5.1.0. Please uninstall the `types-chardet`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `22ced496450a29ecae2cc4f7d5d163185ca6a75f`.
+This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
 '''.lstrip()
 
 setup(name=name,
-      version="5.0.4.4",
+      version="5.0.4.5",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/chardet.md",
```

### Comparing `types-chardet-5.0.4.4/types_chardet.egg-info/PKG-INFO` & `types-chardet-5.0.4.5/types_chardet.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-chardet
-Version: 5.0.4.4
+Version: 5.0.4.5
 Summary: Typing stubs for chardet
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/chardet.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,8 +27,8 @@
 
 *Note:* The `chardet` package includes type annotations or type stubs
 since version 5.1.0. Please uninstall the `types-chardet`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `22ced496450a29ecae2cc4f7d5d163185ca6a75f`.
+This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
```

### Comparing `types-chardet-5.0.4.4/types_chardet.egg-info/SOURCES.txt` & `types-chardet-5.0.4.5/types_chardet.egg-info/SOURCES.txt`

 * *Files identical despite different names*


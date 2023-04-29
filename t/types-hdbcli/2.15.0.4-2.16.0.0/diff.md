# Comparing `tmp/types-hdbcli-2.15.0.4.tar.gz` & `tmp/types-hdbcli-2.16.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-hdbcli-2.15.0.4.tar", last modified: Mon Apr 24 15:16:02 2023, max compression
+gzip compressed data, was "types-hdbcli-2.16.0.0.tar", last modified: Sat Apr 29 15:14:01 2023, max compression
```

## Comparing `types-hdbcli-2.15.0.4.tar` & `types-hdbcli-2.16.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:16:02.865063 types-hdbcli-2.15.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-24 15:16:01.000000 types-hdbcli-2.15.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 15:16:01.000000 types-hdbcli-2.15.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-24 15:16:02.865063 types-hdbcli-2.15.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:16:02.865063 types-hdbcli-2.15.0.4/hdbcli-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-24 15:16:01.000000 types-hdbcli-2.15.0.4/hdbcli-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 15:15:48.000000 types-hdbcli-2.15.0.4/hdbcli-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-24 15:15:48.000000 types-hdbcli-2.15.0.4/hdbcli-stubs/dbapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-24 15:15:48.000000 types-hdbcli-2.15.0.4/hdbcli-stubs/resultrow.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 15:16:02.865063 types-hdbcli-2.15.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-24 15:16:01.000000 types-hdbcli-2.15.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:16:02.865063 types-hdbcli-2.15.0.4/types_hdbcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-24 15:16:02.000000 types-hdbcli-2.15.0.4/types_hdbcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-24 15:16:02.000000 types-hdbcli-2.15.0.4/types_hdbcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:16:02.000000 types-hdbcli-2.15.0.4/types_hdbcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 15:16:02.000000 types-hdbcli-2.15.0.4/types_hdbcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:01.004080 types-hdbcli-2.16.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-29 15:14:00.000000 types-hdbcli-2.16.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 15:14:00.000000 types-hdbcli-2.16.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-29 15:14:01.004080 types-hdbcli-2.16.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:01.004080 types-hdbcli-2.16.0.0/hdbcli-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-29 15:14:00.000000 types-hdbcli-2.16.0.0/hdbcli-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-29 15:13:39.000000 types-hdbcli-2.16.0.0/hdbcli-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-04-29 15:13:39.000000 types-hdbcli-2.16.0.0/hdbcli-stubs/dbapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-29 15:13:39.000000 types-hdbcli-2.16.0.0/hdbcli-stubs/resultrow.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:14:01.004080 types-hdbcli-2.16.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-29 15:14:00.000000 types-hdbcli-2.16.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:01.004080 types-hdbcli-2.16.0.0/types_hdbcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-29 15:14:00.000000 types-hdbcli-2.16.0.0/types_hdbcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-29 15:14:00.000000 types-hdbcli-2.16.0.0/types_hdbcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:14:00.000000 types-hdbcli-2.16.0.0/types_hdbcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 15:14:00.000000 types-hdbcli-2.16.0.0/types_hdbcli.egg-info/top_level.txt
```

### Comparing `types-hdbcli-2.15.0.4/CHANGELOG.md` & `types-hdbcli-2.16.0.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.16.0.0 (2023-04-29)
+
+Update `hdbcli` to `2.16` and mark as completed (#10101)
+
 ## 2.15.0.4 (2023-04-24)
 
 hdbcli: Fix wrong connection argument name (#10070)
 
 The name should be `user` and not `username`
 
 ## 2.15.0.3 (2023-04-13)
```

### Comparing `types-hdbcli-2.15.0.4/PKG-INFO` & `types-hdbcli-2.16.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-hdbcli
-Version: 2.15.0.4
+Version: 2.16.0.0
 Summary: Typing stubs for hdbcli
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/hdbcli.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `hdbcli`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/hdbcli. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1d9f35369d724954e7fc34970692f5509dd10ac7`.
+This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
```

### Comparing `types-hdbcli-2.15.0.4/hdbcli-stubs/dbapi.pyi` & `types-hdbcli-2.16.0.0/hdbcli-stubs/dbapi.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     def server_processing_time(self) -> int: ...
     def setinputsizes(self, *args: Any, **kwargs: Any) -> None: ...
     def setfetchsize(self, value: int) -> None: ...
     def setquerytimeout(self, value: int) -> None: ...
     def setpacketsize(self, value: int) -> None: ...
     def set_resultset_holdability(self, holdability: int) -> None: ...
     def setoutputsize(self, *args: Any, **kwargs: Any) -> None: ...
+    def setcommandinfo(self, command_info: str, line_number: int) -> None: ...
 
 class Warning(Exception):
     errorcode: int
     errortext: str
 
 class Error(Exception):
     errorcode: int
```

### Comparing `types-hdbcli-2.15.0.4/setup.py` & `types-hdbcli-2.16.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `hdbcli`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/hdbcli. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1d9f35369d724954e7fc34970692f5509dd10ac7`.
+This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.15.0.4",
+      version="2.16.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/hdbcli.md",
```

### Comparing `types-hdbcli-2.15.0.4/types_hdbcli.egg-info/PKG-INFO` & `types-hdbcli-2.16.0.0/types_hdbcli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-hdbcli
-Version: 2.15.0.4
+Version: 2.16.0.0
 Summary: Typing stubs for hdbcli
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/hdbcli.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `hdbcli`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/hdbcli. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1d9f35369d724954e7fc34970692f5509dd10ac7`.
+This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
```


# Comparing `tmp/types-aiofiles-23.1.0.1.tar.gz` & `tmp/types-aiofiles-23.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiofiles-23.1.0.1.tar", last modified: Mon Mar 27 18:22:51 2023, max compression
+gzip compressed data, was "types-aiofiles-23.1.0.2.tar", last modified: Sat Apr 29 15:13:56 2023, max compression
```

## Comparing `types-aiofiles-23.1.0.1.tar` & `types-aiofiles-23.1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:51.634207 types-aiofiles-23.1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-03-27 18:22:51.000000 types-aiofiles-23.1.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:22:51.000000 types-aiofiles-23.1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-27 18:22:51.634207 types-aiofiles-23.1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:51.634207 types-aiofiles-23.1.0.1/aiofiles-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-27 18:22:51.000000 types-aiofiles-23.1.0.1/aiofiles-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-27 18:21:24.000000 types-aiofiles-23.1.0.1/aiofiles-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-03-27 18:21:24.000000 types-aiofiles-23.1.0.1/aiofiles-stubs/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-03-27 18:21:24.000000 types-aiofiles-23.1.0.1/aiofiles-stubs/os.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-03-27 18:21:24.000000 types-aiofiles-23.1.0.1/aiofiles-stubs/ospath.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:51.634207 types-aiofiles-23.1.0.1/aiofiles-stubs/tempfile/
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-03-27 18:21:24.000000 types-aiofiles-23.1.0.1/aiofiles-stubs/tempfile/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-27 18:21:24.000000 types-aiofiles-23.1.0.1/aiofiles-stubs/tempfile/temptypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:51.634207 types-aiofiles-23.1.0.1/aiofiles-stubs/threadpool/
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-03-27 18:21:24.000000 types-aiofiles-23.1.0.1/aiofiles-stubs/threadpool/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-03-27 18:21:24.000000 types-aiofiles-23.1.0.1/aiofiles-stubs/threadpool/binary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-27 18:21:24.000000 types-aiofiles-23.1.0.1/aiofiles-stubs/threadpool/text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-27 18:21:24.000000 types-aiofiles-23.1.0.1/aiofiles-stubs/threadpool/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:22:51.634207 types-aiofiles-23.1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-03-27 18:22:50.000000 types-aiofiles-23.1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:51.634207 types-aiofiles-23.1.0.1/types_aiofiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-27 18:22:51.000000 types-aiofiles-23.1.0.1/types_aiofiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-27 18:22:51.000000 types-aiofiles-23.1.0.1/types_aiofiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:22:51.000000 types-aiofiles-23.1.0.1/types_aiofiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-27 18:22:51.000000 types-aiofiles-23.1.0.1/types_aiofiles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:13:56.327733 types-aiofiles-23.1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-29 15:13:53.000000 types-aiofiles-23.1.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 15:13:53.000000 types-aiofiles-23.1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-29 15:13:56.327733 types-aiofiles-23.1.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:13:56.327733 types-aiofiles-23.1.0.2/aiofiles-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-29 15:13:53.000000 types-aiofiles-23.1.0.2/aiofiles-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-29 15:13:39.000000 types-aiofiles-23.1.0.2/aiofiles-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-29 15:13:39.000000 types-aiofiles-23.1.0.2/aiofiles-stubs/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-29 15:13:39.000000 types-aiofiles-23.1.0.2/aiofiles-stubs/os.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-29 15:13:39.000000 types-aiofiles-23.1.0.2/aiofiles-stubs/ospath.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:13:56.327733 types-aiofiles-23.1.0.2/aiofiles-stubs/tempfile/
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-04-29 15:13:39.000000 types-aiofiles-23.1.0.2/aiofiles-stubs/tempfile/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-29 15:13:39.000000 types-aiofiles-23.1.0.2/aiofiles-stubs/tempfile/temptypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:13:56.327733 types-aiofiles-23.1.0.2/aiofiles-stubs/threadpool/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-29 15:13:39.000000 types-aiofiles-23.1.0.2/aiofiles-stubs/threadpool/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-29 15:13:39.000000 types-aiofiles-23.1.0.2/aiofiles-stubs/threadpool/binary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-29 15:13:39.000000 types-aiofiles-23.1.0.2/aiofiles-stubs/threadpool/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-29 15:13:39.000000 types-aiofiles-23.1.0.2/aiofiles-stubs/threadpool/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:13:56.327733 types-aiofiles-23.1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-29 15:13:53.000000 types-aiofiles-23.1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:13:56.327733 types-aiofiles-23.1.0.2/types_aiofiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-29 15:13:56.000000 types-aiofiles-23.1.0.2/types_aiofiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-29 15:13:56.000000 types-aiofiles-23.1.0.2/types_aiofiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:13:56.000000 types-aiofiles-23.1.0.2/types_aiofiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-29 15:13:56.000000 types-aiofiles-23.1.0.2/types_aiofiles.egg-info/top_level.txt
```

### Comparing `types-aiofiles-23.1.0.1/CHANGELOG.md` & `types-aiofiles-23.1.0.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 23.1.0.2 (2023-04-29)
+
+aiofiles: use ReadableBuffer (#10105)
+
+Part of #9006
+
 ## 23.1.0.1 (2023-03-27)
 
 Add defaults for third-party stubs A-D (#9952)
 
 ## 23.1.0.0 (2023-03-09)
 
 Update `aiofiles` for v23.1.* (#9711)
```

### Comparing `types-aiofiles-23.1.0.1/PKG-INFO` & `types-aiofiles-23.1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiofiles
-Version: 23.1.0.1
+Version: 23.1.0.2
 Summary: Typing stubs for aiofiles
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/aiofiles.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `aiofiles`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/aiofiles. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
```

### Comparing `types-aiofiles-23.1.0.1/aiofiles-stubs/base.pyi` & `types-aiofiles-23.1.0.2/aiofiles-stubs/base.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.1.0.1/aiofiles-stubs/os.pyi` & `types-aiofiles-23.1.0.2/aiofiles-stubs/os.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from _typeshed import FileDescriptorOrPath, GenericPath, StrOrBytesPath
+from _typeshed import FileDescriptorOrPath, GenericPath, ReadableBuffer, StrOrBytesPath
 from asyncio.events import AbstractEventLoop
 from collections.abc import Sequence
 from os import _ScandirIterator, stat_result
 from typing import Any, AnyStr, overload
 
 from aiofiles import ospath
 
@@ -64,14 +64,14 @@
     ) -> int: ...
     @overload
     async def sendfile(
         out_fd: int,
         in_fd: int,
         offset: int,
         count: int,
-        headers: Sequence[bytes] = ...,
-        trailers: Sequence[bytes] = ...,
+        headers: Sequence[ReadableBuffer] = ...,
+        trailers: Sequence[ReadableBuffer] = ...,
         flags: int = ...,
         *,
         loop: AbstractEventLoop | None = ...,
         executor: Any = ...,
     ) -> int: ...  # FreeBSD and Mac OS X only
```

### Comparing `types-aiofiles-23.1.0.1/aiofiles-stubs/ospath.pyi` & `types-aiofiles-23.1.0.2/aiofiles-stubs/ospath.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.1.0.1/aiofiles-stubs/tempfile/__init__.pyi` & `types-aiofiles-23.1.0.2/aiofiles-stubs/tempfile/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.1.0.1/aiofiles-stubs/tempfile/temptypes.pyi` & `types-aiofiles-23.1.0.2/aiofiles-stubs/tempfile/temptypes.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.1.0.1/aiofiles-stubs/threadpool/__init__.pyi` & `types-aiofiles-23.1.0.2/aiofiles-stubs/threadpool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.1.0.1/aiofiles-stubs/threadpool/binary.pyi` & `types-aiofiles-23.1.0.2/aiofiles-stubs/threadpool/binary.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.1.0.1/aiofiles-stubs/threadpool/text.pyi` & `types-aiofiles-23.1.0.2/aiofiles-stubs/threadpool/text.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.1.0.1/setup.py` & `types-aiofiles-23.1.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `aiofiles`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/aiofiles. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
 '''.lstrip()
 
 setup(name=name,
-      version="23.1.0.1",
+      version="23.1.0.2",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/aiofiles.md",
```

### Comparing `types-aiofiles-23.1.0.1/types_aiofiles.egg-info/PKG-INFO` & `types-aiofiles-23.1.0.2/types_aiofiles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiofiles
-Version: 23.1.0.1
+Version: 23.1.0.2
 Summary: Typing stubs for aiofiles
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/aiofiles.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `aiofiles`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/aiofiles. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
```

### Comparing `types-aiofiles-23.1.0.1/types_aiofiles.egg-info/SOURCES.txt` & `types-aiofiles-23.1.0.2/types_aiofiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*


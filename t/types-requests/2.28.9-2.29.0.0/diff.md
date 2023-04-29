# Comparing `tmp/types-requests-2.28.9.tar.gz` & `tmp/types-requests-2.29.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-requests-2.28.9.tar", last modified: Thu Aug 18 21:17:29 2022, max compression
+gzip compressed data, was "types-requests-2.29.0.0.tar", last modified: Sat Apr 29 01:14:12 2023, max compression
```

## Comparing `types-requests-2.28.9.tar` & `types-requests-2.29.0.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 21:17:29.039157 types-requests-2.28.9/
--rw-r--r--   0 runner    (1001) docker     (121)     7878 2022-08-18 21:17:28.000000 types-requests-2.28.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-08-18 21:17:28.000000 types-requests-2.28.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-08-18 21:17:29.039157 types-requests-2.28.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 21:17:29.039157 types-requests-2.28.9/requests-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-08-18 21:17:28.000000 types-requests-2.28.9/requests-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-08-18 21:17:02.000000 types-requests-2.28.9/requests-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-08-18 21:17:02.000000 types-requests-2.28.9/requests-stubs/__version__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2913 2022-08-18 21:17:02.000000 types-requests-2.28.9/requests-stubs/adapters.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4790 2022-08-18 21:17:02.000000 types-requests-2.28.9/requests-stubs/api.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-08-18 21:17:02.000000 types-requests-2.28.9/requests-stubs/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-08-18 21:17:02.000000 types-requests-2.28.9/requests-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-08-18 21:17:02.000000 types-requests-2.28.9/requests-stubs/cookies.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-08-18 21:17:02.000000 types-requests-2.28.9/requests-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-08-18 21:17:02.000000 types-requests-2.28.9/requests-stubs/help.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-08-18 21:17:02.000000 types-requests-2.28.9/requests-stubs/hooks.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4975 2022-08-18 21:17:02.000000 types-requests-2.28.9/requests-stubs/models.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-08-18 21:17:02.000000 types-requests-2.28.9/requests-stubs/packages.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10581 2022-08-18 21:17:02.000000 types-requests-2.28.9/requests-stubs/sessions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-18 21:17:02.000000 types-requests-2.28.9/requests-stubs/status_codes.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-08-18 21:17:02.000000 types-requests-2.28.9/requests-stubs/structures.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2501 2022-08-18 21:17:02.000000 types-requests-2.28.9/requests-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-18 21:17:29.039157 types-requests-2.28.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-08-18 21:17:28.000000 types-requests-2.28.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 21:17:29.039157 types-requests-2.28.9/types_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-08-18 21:17:29.000000 types-requests-2.28.9/types_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-08-18 21:17:29.000000 types-requests-2.28.9/types_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 21:17:29.000000 types-requests-2.28.9/types_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-18 21:17:29.000000 types-requests-2.28.9/types_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-18 21:17:29.000000 types-requests-2.28.9/types_requests.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:14:12.733398 types-requests-2.29.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-04-29 01:14:10.000000 types-requests-2.29.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 01:14:10.000000 types-requests-2.29.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-29 01:14:12.733398 types-requests-2.29.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:14:12.733398 types-requests-2.29.0.0/requests-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-29 01:14:10.000000 types-requests-2.29.0.0/requests-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-29 01:13:54.000000 types-requests-2.29.0.0/requests-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-29 01:13:54.000000 types-requests-2.29.0.0/requests-stubs/__version__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-29 01:13:54.000000 types-requests-2.29.0.0/requests-stubs/adapters.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-29 01:13:54.000000 types-requests-2.29.0.0/requests-stubs/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-29 01:13:54.000000 types-requests-2.29.0.0/requests-stubs/auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-29 01:13:54.000000 types-requests-2.29.0.0/requests-stubs/certs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-29 01:13:54.000000 types-requests-2.29.0.0/requests-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-29 01:13:54.000000 types-requests-2.29.0.0/requests-stubs/cookies.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-29 01:13:54.000000 types-requests-2.29.0.0/requests-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-29 01:13:54.000000 types-requests-2.29.0.0/requests-stubs/help.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-29 01:13:54.000000 types-requests-2.29.0.0/requests-stubs/hooks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-04-29 01:13:54.000000 types-requests-2.29.0.0/requests-stubs/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-29 01:13:54.000000 types-requests-2.29.0.0/requests-stubs/packages.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-04-29 01:13:54.000000 types-requests-2.29.0.0/requests-stubs/sessions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-29 01:13:54.000000 types-requests-2.29.0.0/requests-stubs/status_codes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-29 01:13:54.000000 types-requests-2.29.0.0/requests-stubs/structures.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-29 01:13:54.000000 types-requests-2.29.0.0/requests-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 01:14:12.733398 types-requests-2.29.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-29 01:14:10.000000 types-requests-2.29.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:14:12.733398 types-requests-2.29.0.0/types_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-29 01:14:12.000000 types-requests-2.29.0.0/types_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-29 01:14:12.000000 types-requests-2.29.0.0/types_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 01:14:12.000000 types-requests-2.29.0.0/types_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-29 01:14:12.000000 types-requests-2.29.0.0/types_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-29 01:14:12.000000 types-requests-2.29.0.0/types_requests.egg-info/top_level.txt
```

### Comparing `types-requests-2.28.9/CHANGELOG.md` & `types-requests-2.29.0.0/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,112 @@
+## 2.29.0.0 (2023-04-29)
+
+Update `requests` for v2.29 (#10097)
+
+## 2.28.11.17 (2023-03-28)
+
+Add defaults for third-party stubs Q-T (#9959)
+
+## 2.28.11.16 (2023-03-22)
+
+Add type to requests.models.RequestEncodingMixin.path_url (#9923)
+
+We can see at https://github.com/psf/requests/blob/7f694b79e114c06fac5ec06019cada5a61e5570f/requests/models.py#L104 that this always returns a string.
+
+## 2.28.11.15 (2023-02-26)
+
+Improve many `__(a)exit__` annotations (#9696)
+
+## 2.28.11.14 (2023-02-21)
+
+Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
+
+If you're reading about this commit from an autogenerated changelog entry, this should have no user-visible impact on how the stubs are interpreted by a type checker; it's just an internal change to how typeshed's tests work.
+
+## 2.28.11.13 (2023-02-15)
+
+Use `typing_extensions.Self` instead of `_typeshed.Self` (#9702)
+
+## 2.28.11.12 (2023-02-07)
+
+Improve pyright verification of third-party test cases in CI (#9650)
+
+Co-authored-by: Avasam <samuel.06@hotmail.com>
+
+## 2.28.11.11 (2023-02-07)
+
+Enable flake8-pyi's Y037 (#9686)
+
+## 2.28.11.10 (2023-02-07)
+
+Bump mypy to 1.0 (#9684)
+
+## 2.28.11.9 (2023-02-06)
+
+Use `OSError` instead of `IOError` (#9683)
+
+## 2.28.11.8 (2023-01-18)
+
+Replace `Any` with `Incomplete` in many places (#9558)
+
+## 2.28.11.7 (2022-12-22)
+
+`requests`: set `session.headers` to `MutableMapping` (#9395)
+
+## 2.28.11.6 (2022-12-21)
+
+requests: types for auth username and password (#9389)
+
+## 2.28.11.5 (2022-11-16)
+
+Always use `bool` and `Literal` for Python compat code (#9213)
+
+## 2.28.11.4 (2022-11-09)
+
+Annotate known magic-method return types (#9131)
+
+## 2.28.11.3 (2022-11-08)
+
+Fix and allow classes with missing metaclasses (#9136)
+
+## 2.28.11.2 (2022-10-07)
+
+Mark `requests` stubs as complete (#8858)
+
+Co-authored-by: Kevin Kirsche <kevin.kirsche@one.verizon.com>
+
+## 2.28.11.1 (2022-10-04)
+
+`requests`: Add regression test for #8762 (#8835)
+
+The final mypy_primer report for #8762 was an empty diff. Considering the number of issues we've had with our requests stubs over the last year, it feels like it makes sense to add a test case to make sure that it doesn't regress.
+
+## 2.28.11 (2022-09-22)
+
+`requests`: improve `_Data` type (#8762)
+
+requests: improve _Data type
+
+This allows to pass an Iterable[bytes] for streaming request data.
+
+## 2.28.10 (2022-09-08)
+
+Add infrastructure allowing for test cases for third-party stubs (#8700)
+
+- Move the logic for running mypy on the test cases from `tests/mypy_test.py` to a separate script, `tests/regr_test.py`.
+- Add the necessary logic in order to be able to have test cases for third-party stubs.
+- Move logic common to `tests/mypy_test.py` and `tests/regr_test.py` into `tests/colors.py`, and rename `tests/colors.py` to `tests/utils.py`.
+- Add a new check to `tests/check_consistent.py`, to enforce the use of `# pyright: reportUnnecessaryTypeIgnoreComment=true` comments in third-party test cases. These are essential if we want to have our tests against false-negatives work with pyright.
+- Update the relevant documentation to account for the new test file.
+- Add a new job to the `tests.yml` GitHub workflow, to run the new test in CI.
+- Add a simple proof-of-concept test case for `requests`, as a regression test for #7998.
+
+Co-authored-by: Jelle Zijlstra <jelle.zijlstra@gmail.com>
+Co-authored-by: Sebastian Rittau <srittau@rittau.biz>
+
 ## 2.28.9 (2022-08-18)
 
 Support extras in stubtest_third_party.py (#8467)
 
 ## 2.28.8 (2022-08-05)
 
 `requests.adapters`: use re-exports rather than assignments (#8485)
```

### Comparing `types-requests-2.28.9/PKG-INFO` & `types-requests-2.29.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: types-requests
-Version: 2.28.9
+Version: 2.29.0.0
 Summary: Typing stubs for requests
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
 
 ## Typing stubs for requests
 
-This is a PEP 561 type stub package for the `requests` package.
-It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
-that uses `requests`. The source for this package can be found at
-https://github.com/python/typeshed/tree/master/stubs/requests. All fixes for
+This is a PEP 561 type stub package for the `requests` package. It
+can be used by type-checking tools like
+[mypy](https://github.com/python/mypy/),
+[pyright](https://github.com/microsoft/pyright),
+[pytype](https://github.com/google/pytype/),
+PyCharm, etc. to check code that uses
+`requests`. The source for this package can be found at
+https://github.com/python/typeshed/tree/main/stubs/requests. All fixes for
 types and metadata should be contributed there.
 
-See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `8c51fab4e26981b9e21f9d5c5483a42f4a73ce92`.
-
-
+See https://github.com/python/typeshed/blob/main/README.md for more details.
+This package was generated from typeshed commit `2d84e56d6fc12c08d43b4694703bd9a48a9c2b2f`.
```

### Comparing `types-requests-2.28.9/requests-stubs/__init__.pyi` & `types-requests-2.29.0.0/requests-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.28.9/requests-stubs/adapters.pyi` & `types-requests-2.29.0.0/requests-stubs/adapters.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     ConnectTimeoutError as ConnectTimeoutError,
     MaxRetryError as MaxRetryError,
     ProtocolError as ProtocolError,
     ReadTimeoutError as ReadTimeoutError,
     ResponseError as ResponseError,
 )
 from urllib3.poolmanager import PoolManager as PoolManager, proxy_from_url as proxy_from_url
-from urllib3.response import HTTPResponse as HTTPResponse
 from urllib3.util.retry import Retry as Retry
 
 from .cookies import extract_cookies_to_jar as extract_cookies_to_jar
 from .exceptions import (
     ConnectionError as ConnectionError,
     ConnectTimeout as ConnectTimeout,
     ProxyError as ProxyError,
@@ -38,42 +37,42 @@
 DEFAULT_POOL_TIMEOUT: float | None
 
 class BaseAdapter:
     def __init__(self) -> None: ...
     def send(
         self,
         request: PreparedRequest,
-        stream: bool = ...,
-        timeout: None | float | tuple[float, float] | tuple[float, None] = ...,
-        verify: bool | str = ...,
-        cert: None | bytes | str | tuple[bytes | str, bytes | str] = ...,
-        proxies: Mapping[str, str] | None = ...,
+        stream: bool = False,
+        timeout: None | float | tuple[float, float] | tuple[float, None] = None,
+        verify: bool | str = True,
+        cert: None | bytes | str | tuple[bytes | str, bytes | str] = None,
+        proxies: Mapping[str, str] | None = None,
     ) -> Response: ...
     def close(self) -> None: ...
 
 class HTTPAdapter(BaseAdapter):
     __attrs__: Any
     max_retries: Retry
     config: Any
     proxy_manager: Any
     def __init__(
-        self, pool_connections: int = ..., pool_maxsize: int = ..., max_retries: Retry | int | None = ..., pool_block: bool = ...
+        self, pool_connections: int = 10, pool_maxsize: int = 10, max_retries: Retry | int | None = 0, pool_block: bool = False
     ) -> None: ...
     poolmanager: Any
-    def init_poolmanager(self, connections, maxsize, block=..., **pool_kwargs): ...
+    def init_poolmanager(self, connections, maxsize, block=False, **pool_kwargs): ...
     def proxy_manager_for(self, proxy, **proxy_kwargs): ...
     def cert_verify(self, conn, url, verify, cert): ...
     def build_response(self, req, resp): ...
-    def get_connection(self, url, proxies=...): ...
+    def get_connection(self, url, proxies=None): ...
     def close(self): ...
     def request_url(self, request, proxies): ...
     def add_headers(self, request, **kwargs): ...
     def proxy_headers(self, proxy): ...
     def send(
         self,
         request: PreparedRequest,
-        stream: bool = ...,
-        timeout: None | float | tuple[float, float] | tuple[float, None] = ...,
-        verify: bool | str = ...,
-        cert: None | bytes | str | tuple[bytes | str, bytes | str] = ...,
-        proxies: Mapping[str, str] | None = ...,
+        stream: bool = False,
+        timeout: None | float | tuple[float, float] | tuple[float, None] = None,
+        verify: bool | str = True,
+        cert: None | bytes | str | tuple[bytes | str, bytes | str] = None,
+        proxies: Mapping[str, str] | None = None,
     ) -> Response: ...
```

### Comparing `types-requests-2.28.9/requests-stubs/api.pyi` & `types-requests-2.29.0.0/requests-stubs/api.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from _typeshed import Incomplete
 from collections.abc import Mapping
-from typing import Any
 from typing_extensions import TypeAlias
 
 from .models import Response
 from .sessions import RequestsCookieJar, _Auth, _Cert, _Data, _Files, _HooksInput, _Params, _TextMapping, _Timeout, _Verify
 
 _HeadersMapping: TypeAlias = Mapping[str, str | bytes]
 
@@ -20,33 +20,33 @@
     timeout: _Timeout | None = ...,
     allow_redirects: bool = ...,
     proxies: _TextMapping | None = ...,
     hooks: _HooksInput | None = ...,
     stream: bool | None = ...,
     verify: _Verify | None = ...,
     cert: _Cert | None = ...,
-    json: Any | None = ...,
+    json: Incomplete | None = ...,
 ) -> Response: ...
 def get(
     url: str | bytes,
-    params: _Params | None = ...,
+    params: _Params | None = None,
     *,
     data: _Data | None = ...,
     headers: _HeadersMapping | None = ...,
     cookies: RequestsCookieJar | _TextMapping | None = ...,
     files: _Files | None = ...,
     auth: _Auth | None = ...,
     timeout: _Timeout | None = ...,
     allow_redirects: bool = ...,
     proxies: _TextMapping | None = ...,
     hooks: _HooksInput | None = ...,
     stream: bool | None = ...,
     verify: _Verify | None = ...,
     cert: _Cert | None = ...,
-    json: Any | None = ...,
+    json: Incomplete | None = ...,
 ) -> Response: ...
 def options(
     url: str | bytes,
     *,
     params: _Params | None = ...,
     data: _Data | None = ...,
     headers: _HeadersMapping | None = ...,
@@ -56,15 +56,15 @@
     timeout: _Timeout | None = ...,
     allow_redirects: bool = ...,
     proxies: _TextMapping | None = ...,
     hooks: _HooksInput | None = ...,
     stream: bool | None = ...,
     verify: _Verify | None = ...,
     cert: _Cert | None = ...,
-    json: Any | None = ...,
+    json: Incomplete | None = ...,
 ) -> Response: ...
 def head(
     url: str | bytes,
     *,
     params: _Params | None = ...,
     data: _Data | None = ...,
     headers: _HeadersMapping | None = ...,
@@ -74,20 +74,20 @@
     timeout: _Timeout | None = ...,
     allow_redirects: bool = ...,
     proxies: _TextMapping | None = ...,
     hooks: _HooksInput | None = ...,
     stream: bool | None = ...,
     verify: _Verify | None = ...,
     cert: _Cert | None = ...,
-    json: Any | None = ...,
+    json: Incomplete | None = ...,
 ) -> Response: ...
 def post(
     url: str | bytes,
-    data: _Data | None = ...,
-    json: Any | None = ...,
+    data: _Data | None = None,
+    json: Incomplete | None = None,
     *,
     params: _Params | None = ...,
     headers: _HeadersMapping | None = ...,
     cookies: RequestsCookieJar | _TextMapping | None = ...,
     files: _Files | None = ...,
     auth: _Auth | None = ...,
     timeout: _Timeout | None = ...,
@@ -96,47 +96,47 @@
     hooks: _HooksInput | None = ...,
     stream: bool | None = ...,
     verify: _Verify | None = ...,
     cert: _Cert | None = ...,
 ) -> Response: ...
 def put(
     url: str | bytes,
-    data: _Data | None = ...,
+    data: _Data | None = None,
     *,
     params: _Params | None = ...,
     headers: _HeadersMapping | None = ...,
     cookies: RequestsCookieJar | _TextMapping | None = ...,
     files: _Files | None = ...,
     auth: _Auth | None = ...,
     timeout: _Timeout | None = ...,
     allow_redirects: bool = ...,
     proxies: _TextMapping | None = ...,
     hooks: _HooksInput | None = ...,
     stream: bool | None = ...,
     verify: _Verify | None = ...,
     cert: _Cert | None = ...,
-    json: Any | None = ...,
+    json: Incomplete | None = ...,
 ) -> Response: ...
 def patch(
     url: str | bytes,
-    data: _Data | None = ...,
+    data: _Data | None = None,
     *,
     params: _Params | None = ...,
     headers: _HeadersMapping | None = ...,
     cookies: RequestsCookieJar | _TextMapping | None = ...,
     files: _Files | None = ...,
     auth: _Auth | None = ...,
     timeout: _Timeout | None = ...,
     allow_redirects: bool = ...,
     proxies: _TextMapping | None = ...,
     hooks: _HooksInput | None = ...,
     stream: bool | None = ...,
     verify: _Verify | None = ...,
     cert: _Cert | None = ...,
-    json: Any | None = ...,
+    json: Incomplete | None = ...,
 ) -> Response: ...
 def delete(
     url: str | bytes,
     *,
     params: _Params | None = ...,
     data: _Data | None = ...,
     headers: _HeadersMapping | None = ...,
@@ -146,9 +146,9 @@
     timeout: _Timeout | None = ...,
     allow_redirects: bool = ...,
     proxies: _TextMapping | None = ...,
     hooks: _HooksInput | None = ...,
     stream: bool | None = ...,
     verify: _Verify | None = ...,
     cert: _Cert | None = ...,
-    json: Any | None = ...,
+    json: Incomplete | None = ...,
 ) -> Response: ...
```

### Comparing `types-requests-2.28.9/requests-stubs/auth.pyi` & `types-requests-2.29.0.0/requests-stubs/auth.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 
 def _basic_auth_str(username: bytes | str, password: bytes | str) -> str: ...
 
 class AuthBase:
     def __call__(self, r: models.PreparedRequest) -> models.PreparedRequest: ...
 
 class HTTPBasicAuth(AuthBase):
-    username: Any
-    password: Any
-    def __init__(self, username, password) -> None: ...
+    username: bytes | str
+    password: bytes | str
+    def __init__(self, username: bytes | str, password: bytes | str) -> None: ...
     def __call__(self, r): ...
 
 class HTTPProxyAuth(HTTPBasicAuth):
     def __call__(self, r): ...
 
 class HTTPDigestAuth(AuthBase):
-    username: Any
-    password: Any
+    username: bytes | str
+    password: bytes | str
     last_nonce: Any
     nonce_count: Any
     chal: Any
     pos: Any
     num_401_calls: Any
-    def __init__(self, username, password) -> None: ...
+    def __init__(self, username: bytes | str, password: bytes | str) -> None: ...
     def build_digest_header(self, method, url): ...
     def handle_redirect(self, r, **kwargs): ...
     def handle_401(self, r, **kwargs): ...
     def __call__(self, r): ...
     def init_per_thread_state(self) -> None: ...
```

### Comparing `types-requests-2.28.9/requests-stubs/cookies.pyi` & `types-requests-2.29.0.0/requests-stubs/cookies.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def __init__(self, request) -> None: ...
     def get_type(self): ...
     def get_host(self): ...
     def get_origin_req_host(self): ...
     def get_full_url(self): ...
     def is_unverifiable(self): ...
     def has_header(self, name): ...
-    def get_header(self, name, default=...): ...
+    def get_header(self, name, default=None): ...
     def add_header(self, key, val): ...
     def add_unredirected_header(self, name, value): ...
     def get_new_headers(self): ...
     @property
     def unverifiable(self): ...
     @property
     def origin_req_host(self): ...
@@ -25,36 +25,36 @@
 class MockResponse:
     def __init__(self, headers) -> None: ...
     def info(self): ...
     def getheaders(self, name): ...
 
 def extract_cookies_to_jar(jar, request, response): ...
 def get_cookie_header(jar, request): ...
-def remove_cookie_by_name(cookiejar, name, domain=..., path=...): ...
+def remove_cookie_by_name(cookiejar, name, domain=None, path=None): ...
 
 class CookieConflictError(RuntimeError): ...
 
 class RequestsCookieJar(CookieJar, MutableMapping[Any, Any]):
-    def get(self, name, default=..., domain=..., path=...): ...
+    def get(self, name, default=None, domain=None, path=None): ...
     def set(self, name, value, **kwargs): ...
     def iterkeys(self): ...
     def keys(self): ...
     def itervalues(self): ...
     def values(self): ...
     def iteritems(self): ...
     def items(self): ...
     def list_domains(self): ...
     def list_paths(self): ...
     def multiple_domains(self): ...
-    def get_dict(self, domain=..., path=...): ...
+    def get_dict(self, domain=None, path=None): ...
     def __getitem__(self, name): ...
-    def __setitem__(self, name, value): ...
-    def __delitem__(self, name): ...
+    def __setitem__(self, name, value) -> None: ...
+    def __delitem__(self, name) -> None: ...
     def set_cookie(self, cookie, *args, **kwargs): ...
     def update(self, other): ...
     def copy(self): ...
     def get_policy(self): ...
 
 def create_cookie(name, value, **kwargs): ...
 def morsel_to_cookie(morsel): ...
-def cookiejar_from_dict(cookie_dict, cookiejar=..., overwrite=...): ...
+def cookiejar_from_dict(cookie_dict, cookiejar=None, overwrite=True): ...
 def merge_cookies(cookiejar, cookies): ...
```

### Comparing `types-requests-2.28.9/requests-stubs/exceptions.pyi` & `types-requests-2.29.0.0/requests-stubs/exceptions.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any
 
 from urllib3.exceptions import HTTPError as BaseHTTPError
 
-class RequestException(IOError):
+class RequestException(OSError):
     response: Any
     request: Any
     def __init__(self, *args, **kwargs) -> None: ...
 
 class InvalidJSONError(RequestException): ...
 class JSONDecodeError(InvalidJSONError): ...
 class HTTPError(RequestException): ...
```

### Comparing `types-requests-2.28.9/requests-stubs/help.pyi` & `types-requests-2.29.0.0/requests-stubs/help.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.28.9/requests-stubs/models.pyi` & `types-requests-2.29.0.0/requests-stubs/models.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
-from _typeshed import Self
+from _typeshed import Unused
 from collections.abc import Callable, Iterator
 from json import JSONDecoder
 from typing import Any
+from typing_extensions import Self
 
 from urllib3 import exceptions as urllib3_exceptions, fields, filepost, util
 
 from . import auth, cookies, exceptions, hooks, status_codes, utils
 from .cookies import RequestsCookieJar
 from .structures import CaseInsensitiveDict as CaseInsensitiveDict
 
@@ -43,15 +44,15 @@
 REDIRECT_STATI: Any
 DEFAULT_REDIRECT_LIMIT: Any
 CONTENT_CHUNK_SIZE: Any
 ITER_CHUNK_SIZE: Any
 
 class RequestEncodingMixin:
     @property
-    def path_url(self): ...
+    def path_url(self) -> str: ...
 
 class RequestHooksMixin:
     def register_hook(self, event, hook): ...
     def deregister_hook(self, event, hook): ...
 
 class Request(RequestHooksMixin):
     hooks: Any
@@ -61,35 +62,55 @@
     files: Any
     data: Any
     json: Any
     params: Any
     auth: Any
     cookies: Any
     def __init__(
-        self, method=..., url=..., headers=..., files=..., data=..., params=..., auth=..., cookies=..., hooks=..., json=...
+        self,
+        method=None,
+        url=None,
+        headers=None,
+        files=None,
+        data=None,
+        params=None,
+        auth=None,
+        cookies=None,
+        hooks=None,
+        json=None,
     ) -> None: ...
     def prepare(self) -> PreparedRequest: ...
 
 class PreparedRequest(RequestEncodingMixin, RequestHooksMixin):
     method: str | None
     url: str | None
     headers: CaseInsensitiveDict[str]
     body: bytes | str | None
     hooks: Any
     def __init__(self) -> None: ...
     def prepare(
-        self, method=..., url=..., headers=..., files=..., data=..., params=..., auth=..., cookies=..., hooks=..., json=...
+        self,
+        method=None,
+        url=None,
+        headers=None,
+        files=None,
+        data=None,
+        params=None,
+        auth=None,
+        cookies=None,
+        hooks=None,
+        json=None,
     ) -> None: ...
     def copy(self) -> PreparedRequest: ...
     def prepare_method(self, method) -> None: ...
     def prepare_url(self, url, params) -> None: ...
     def prepare_headers(self, headers) -> None: ...
-    def prepare_body(self, data, files, json=...) -> None: ...
+    def prepare_body(self, data, files, json=None) -> None: ...
     def prepare_content_length(self, body) -> None: ...
-    def prepare_auth(self, auth, url=...) -> None: ...
+    def prepare_auth(self, auth, url="") -> None: ...
     def prepare_cookies(self, cookies) -> None: ...
     def prepare_hooks(self, hooks) -> None: ...
 
 class Response:
     __attrs__: Any
     _content: bytes | None  # undocumented
     status_code: int
@@ -102,29 +123,29 @@
     cookies: RequestsCookieJar
     elapsed: datetime.timedelta
     request: PreparedRequest
     def __init__(self) -> None: ...
     def __bool__(self) -> bool: ...
     def __nonzero__(self) -> bool: ...
     def __iter__(self) -> Iterator[bytes]: ...
-    def __enter__(self: Self) -> Self: ...
-    def __exit__(self, *args: object) -> None: ...
+    def __enter__(self) -> Self: ...
+    def __exit__(self, *args: Unused) -> None: ...
     @property
     def next(self) -> PreparedRequest | None: ...
     @property
     def ok(self) -> bool: ...
     @property
     def is_redirect(self) -> bool: ...
     @property
     def is_permanent_redirect(self) -> bool: ...
     @property
     def apparent_encoding(self) -> str: ...
-    def iter_content(self, chunk_size: int | None = ..., decode_unicode: bool = ...) -> Iterator[Any]: ...
+    def iter_content(self, chunk_size: int | None = 1, decode_unicode: bool = False) -> Iterator[Any]: ...
     def iter_lines(
-        self, chunk_size: int | None = ..., decode_unicode: bool = ..., delimiter: str | bytes | None = ...
+        self, chunk_size: int | None = 512, decode_unicode: bool = False, delimiter: str | bytes | None = None
     ) -> Iterator[Any]: ...
     @property
     def content(self) -> bytes: ...
     @property
     def text(self) -> str: ...
     def json(
         self,
```

### Comparing `types-requests-2.28.9/requests-stubs/sessions.pyi` & `types-requests-2.29.0.0/requests-stubs/sessions.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from _typeshed import Self, SupportsItems, SupportsRead
+from _typeshed import Incomplete, SupportsItems, SupportsRead, Unused
 from collections.abc import Callable, Iterable, Mapping, MutableMapping
-from typing import IO, Any, Union
-from typing_extensions import TypeAlias, TypedDict
+from typing import Any
+from typing_extensions import Self, TypeAlias, TypedDict
 
 from urllib3._collections import RecentlyUsedContainer
 
 from . import adapters, auth as _auth, compat, cookies, exceptions, hooks, models, status_codes, utils
 from .models import Response
 from .structures import CaseInsensitiveDict as CaseInsensitiveDict
 
@@ -36,22 +36,53 @@
 codes = status_codes.codes
 REDIRECT_STATI = models.REDIRECT_STATI
 
 def merge_setting(request_setting, session_setting, dict_class=...): ...
 def merge_hooks(request_hooks, session_hooks, dict_class=...): ...
 
 class SessionRedirectMixin:
-    def resolve_redirects(self, resp, req, stream=..., timeout=..., verify=..., cert=..., proxies=...): ...
+    def resolve_redirects(
+        self,
+        resp,
+        req,
+        stream: bool = False,
+        timeout: Incomplete | None = None,
+        verify: bool = True,
+        cert: Incomplete | None = None,
+        proxies: Incomplete | None = None,
+        yield_requests: bool = False,
+        **adapter_kwargs,
+    ): ...
     def rebuild_auth(self, prepared_request, response): ...
     def rebuild_proxies(self, prepared_request, proxies): ...
     def should_strip_auth(self, old_url, new_url): ...
+    def rebuild_method(self, prepared_request: PreparedRequest, response: Response) -> None: ...
+    def get_redirect_target(self, resp: Response) -> str | None: ...
 
-_Data: TypeAlias = str | bytes | Mapping[str, Any] | Iterable[tuple[str, str | None]] | IO[Any]
-_Auth: TypeAlias = Union[tuple[str, str], _auth.AuthBase, Callable[[PreparedRequest], PreparedRequest]]
-_Cert: TypeAlias = Union[str, tuple[str, str]]
+_Data: TypeAlias = (
+    # used in requests.models.PreparedRequest.prepare_body
+    #
+    # case: is_stream
+    # see requests.adapters.HTTPAdapter.send
+    # will be sent directly to http.HTTPConnection.send(...) (through urllib3)
+    Iterable[bytes]
+    # case: not is_stream
+    # will be modified before being sent to urllib3.HTTPConnectionPool.urlopen(body=...)
+    # see requests.models.RequestEncodingMixin._encode_params
+    # see requests.models.RequestEncodingMixin._encode_files
+    # note that keys&values are converted from Any to str by urllib.parse.urlencode
+    | str
+    | bytes
+    | SupportsRead[str | bytes]
+    | list[tuple[Any, Any]]
+    | tuple[tuple[Any, Any], ...]
+    | Mapping[Any, Any]
+)
+_Auth: TypeAlias = tuple[str, str] | _auth.AuthBase | Callable[[PreparedRequest], PreparedRequest]
+_Cert: TypeAlias = str | tuple[str, str]
 # Files is passed to requests.utils.to_key_val_list()
 _FileName: TypeAlias = str | None
 _FileContent: TypeAlias = SupportsRead[str | bytes] | str | bytes
 _FileContentType: TypeAlias = str
 _FileCustomHeaders: TypeAlias = Mapping[str, str]
 _FileSpecTuple2: TypeAlias = tuple[_FileName, _FileContent]
 _FileSpecTuple3: TypeAlias = tuple[_FileName, _FileContent, _FileContentType]
@@ -59,34 +90,37 @@
 _FileSpec: TypeAlias = _FileContent | _FileSpecTuple2 | _FileSpecTuple3 | _FileSpecTuple4
 _Files: TypeAlias = Mapping[str, _FileSpec] | Iterable[tuple[str, _FileSpec]]
 _Hook: TypeAlias = Callable[[Response], Any]
 _HooksInput: TypeAlias = Mapping[str, Iterable[_Hook] | _Hook]
 
 _ParamsMappingKeyType: TypeAlias = str | bytes | int | float
 _ParamsMappingValueType: TypeAlias = str | bytes | int | float | Iterable[str | bytes | int | float] | None
-_Params: TypeAlias = Union[
-    SupportsItems[_ParamsMappingKeyType, _ParamsMappingValueType],
-    tuple[_ParamsMappingKeyType, _ParamsMappingValueType],
-    Iterable[tuple[_ParamsMappingKeyType, _ParamsMappingValueType]],
-    str | bytes,
-]
+_Params: TypeAlias = (
+    SupportsItems[_ParamsMappingKeyType, _ParamsMappingValueType]
+    | tuple[_ParamsMappingKeyType, _ParamsMappingValueType]
+    | Iterable[tuple[_ParamsMappingKeyType, _ParamsMappingValueType]]
+    | str
+    | bytes
+)
 _TextMapping: TypeAlias = MutableMapping[str, str]
 _HeadersUpdateMapping: TypeAlias = Mapping[str, str | bytes | None]
-_Timeout: TypeAlias = Union[float, tuple[float, float], tuple[float, None]]
+_Timeout: TypeAlias = float | tuple[float, float] | tuple[float, None]
 _Verify: TypeAlias = bool | str
 
 class _Settings(TypedDict):
     verify: _Verify | None
     proxies: _TextMapping
     stream: bool
     cert: _Cert | None
 
 class Session(SessionRedirectMixin):
     __attrs__: Any
-    headers: CaseInsensitiveDict[str | bytes]
+    # See https://github.com/psf/requests/issues/5020#issuecomment-989082461:
+    # requests sets this as a CaseInsensitiveDict, but users may set it to any MutableMapping
+    headers: MutableMapping[str, str | bytes]
     auth: _Auth | None
     proxies: _TextMapping
     # Don't complain if:
     #   - value is assumed to be a list (which it is by default)
     #   - a _Hook is assigned directly, without wrapping it in a list (also works)
     hooks: dict[str, list[_Hook] | Any]
     params: _Params
@@ -95,35 +129,35 @@
     cert: _Cert | None
     max_redirects: int
     trust_env: bool
     cookies: RequestsCookieJar
     adapters: MutableMapping[Any, Any]
     redirect_cache: RecentlyUsedContainer[Any, Any]
     def __init__(self) -> None: ...
-    def __enter__(self: Self) -> Self: ...
-    def __exit__(self, *args) -> None: ...
+    def __enter__(self) -> Self: ...
+    def __exit__(self, *args: Unused) -> None: ...
     def prepare_request(self, request: Request) -> PreparedRequest: ...
     def request(
         self,
         method: str | bytes,
         url: str | bytes,
-        params: _Params | None = ...,
-        data: _Data | None = ...,
-        headers: _HeadersUpdateMapping | None = ...,
-        cookies: None | RequestsCookieJar | _TextMapping = ...,
-        files: _Files | None = ...,
-        auth: _Auth | None = ...,
-        timeout: _Timeout | None = ...,
-        allow_redirects: bool = ...,
-        proxies: _TextMapping | None = ...,
-        hooks: _HooksInput | None = ...,
-        stream: bool | None = ...,
-        verify: _Verify | None = ...,
-        cert: _Cert | None = ...,
-        json: Any | None = ...,
+        params: _Params | None = None,
+        data: _Data | None = None,
+        headers: _HeadersUpdateMapping | None = None,
+        cookies: None | RequestsCookieJar | _TextMapping = None,
+        files: _Files | None = None,
+        auth: _Auth | None = None,
+        timeout: _Timeout | None = None,
+        allow_redirects: bool = True,
+        proxies: _TextMapping | None = None,
+        hooks: _HooksInput | None = None,
+        stream: bool | None = None,
+        verify: _Verify | None = None,
+        cert: _Cert | None = None,
+        json: Incomplete | None = None,
     ) -> Response: ...
     def get(
         self,
         url: str | bytes,
         *,
         params: _Params | None = ...,
         data: _Data | None = ...,
@@ -134,15 +168,15 @@
         timeout: _Timeout | None = ...,
         allow_redirects: bool = ...,
         proxies: _TextMapping | None = ...,
         hooks: _HooksInput | None = ...,
         stream: bool | None = ...,
         verify: _Verify | None = ...,
         cert: _Cert | None = ...,
-        json: Any | None = ...,
+        json: Incomplete | None = ...,
     ) -> Response: ...
     def options(
         self,
         url: str | bytes,
         *,
         params: _Params | None = ...,
         data: _Data | None = ...,
@@ -153,15 +187,15 @@
         timeout: _Timeout | None = ...,
         allow_redirects: bool = ...,
         proxies: _TextMapping | None = ...,
         hooks: _HooksInput | None = ...,
         stream: bool | None = ...,
         verify: _Verify | None = ...,
         cert: _Cert | None = ...,
-        json: Any | None = ...,
+        json: Incomplete | None = ...,
     ) -> Response: ...
     def head(
         self,
         url: str | bytes,
         *,
         params: _Params | None = ...,
         data: _Data | None = ...,
@@ -172,21 +206,21 @@
         timeout: _Timeout | None = ...,
         allow_redirects: bool = ...,
         proxies: _TextMapping | None = ...,
         hooks: _HooksInput | None = ...,
         stream: bool | None = ...,
         verify: _Verify | None = ...,
         cert: _Cert | None = ...,
-        json: Any | None = ...,
+        json: Incomplete | None = ...,
     ) -> Response: ...
     def post(
         self,
         url: str | bytes,
-        data: _Data | None = ...,
-        json: Any | None = ...,
+        data: _Data | None = None,
+        json: Incomplete | None = None,
         *,
         params: _Params | None = ...,
         headers: _HeadersUpdateMapping | None = ...,
         cookies: RequestsCookieJar | _TextMapping | None = ...,
         files: _Files | None = ...,
         auth: _Auth | None = ...,
         timeout: _Timeout | None = ...,
@@ -196,48 +230,48 @@
         stream: bool | None = ...,
         verify: _Verify | None = ...,
         cert: _Cert | None = ...,
     ) -> Response: ...
     def put(
         self,
         url: str | bytes,
-        data: _Data | None = ...,
+        data: _Data | None = None,
         *,
         params: _Params | None = ...,
         headers: _HeadersUpdateMapping | None = ...,
         cookies: RequestsCookieJar | _TextMapping | None = ...,
         files: _Files | None = ...,
         auth: _Auth | None = ...,
         timeout: _Timeout | None = ...,
         allow_redirects: bool = ...,
         proxies: _TextMapping | None = ...,
         hooks: _HooksInput | None = ...,
         stream: bool | None = ...,
         verify: _Verify | None = ...,
         cert: _Cert | None = ...,
-        json: Any | None = ...,
+        json: Incomplete | None = ...,
     ) -> Response: ...
     def patch(
         self,
         url: str | bytes,
-        data: _Data | None = ...,
+        data: _Data | None = None,
         *,
         params: _Params | None = ...,
         headers: _HeadersUpdateMapping | None = ...,
         cookies: RequestsCookieJar | _TextMapping | None = ...,
         files: _Files | None = ...,
         auth: _Auth | None = ...,
         timeout: _Timeout | None = ...,
         allow_redirects: bool = ...,
         proxies: _TextMapping | None = ...,
         hooks: _HooksInput | None = ...,
         stream: bool | None = ...,
         verify: _Verify | None = ...,
         cert: _Cert | None = ...,
-        json: Any | None = ...,
+        json: Incomplete | None = ...,
     ) -> Response: ...
     def delete(
         self,
         url: str | bytes,
         *,
         params: _Params | None = ...,
         data: _Data | None = ...,
@@ -248,15 +282,15 @@
         timeout: _Timeout | None = ...,
         allow_redirects: bool = ...,
         proxies: _TextMapping | None = ...,
         hooks: _HooksInput | None = ...,
         stream: bool | None = ...,
         verify: _Verify | None = ...,
         cert: _Cert | None = ...,
-        json: Any | None = ...,
+        json: Incomplete | None = ...,
     ) -> Response: ...
     def send(
         self,
         request: PreparedRequest,
         *,
         stream: bool | None = ...,
         verify: _Verify | None = ...,
```

### Comparing `types-requests-2.28.9/requests-stubs/structures.pyi` & `types-requests-2.29.0.0/requests-stubs/structures.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from collections.abc import Iterable, Iterator, Mapping, MutableMapping
-from typing import Any, Generic, TypeVar
+from typing import Any, Generic, TypeVar, overload
 
+_D = TypeVar("_D")
 _VT = TypeVar("_VT")
 
 class CaseInsensitiveDict(MutableMapping[str, _VT], Generic[_VT]):
-    def __init__(self, data: Mapping[str, _VT] | Iterable[tuple[str, _VT]] | None = ..., **kwargs: _VT) -> None: ...
+    def __init__(self, data: Mapping[str, _VT] | Iterable[tuple[str, _VT]] | None = None, **kwargs: _VT) -> None: ...
     def lower_items(self) -> Iterator[tuple[str, _VT]]: ...
     def __setitem__(self, key: str, value: _VT) -> None: ...
     def __getitem__(self, key: str) -> _VT: ...
     def __delitem__(self, key: str) -> None: ...
     def __iter__(self) -> Iterator[str]: ...
     def __len__(self) -> int: ...
     def copy(self) -> CaseInsensitiveDict[_VT]: ...
 
 class LookupDict(dict[str, _VT]):
     name: Any
-    def __init__(self, name: Any = ...) -> None: ...
+    def __init__(self, name: Any = None) -> None: ...
     def __getitem__(self, key: str) -> _VT | None: ...  # type: ignore[override]
-    def __getattr__(self, attr: str) -> _VT: ...
     def __setattr__(self, __attr: str, __value: _VT) -> None: ...
+    @overload
+    def get(self, key: str, default: None = None) -> _VT | None: ...
+    @overload
+    def get(self, key: str, default: _D | _VT) -> _D | _VT: ...
```

### Comparing `types-requests-2.28.9/requests-stubs/utils.pyi` & `types-requests-2.29.0.0/requests-stubs/utils.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,40 @@
+import sys
+from _typeshed import StrOrBytesPath
 from collections.abc import Generator, Iterable, Mapping
-from contextlib import AbstractContextManager
+from contextlib import _GeneratorContextManager
+from io import BufferedWriter
 from typing import Any, AnyStr
 from typing_extensions import TypeAlias
 
 from . import compat, cookies, exceptions, structures
-from .models import PreparedRequest
+from .models import PreparedRequest, Request
 
 _Uri: TypeAlias = str | bytes
 OrderedDict = compat.OrderedDict
 cookiejar_from_dict = cookies.cookiejar_from_dict
 CaseInsensitiveDict = structures.CaseInsensitiveDict
 InvalidURL = exceptions.InvalidURL
 
 NETRC_FILES: tuple[str, str]
 DEFAULT_CA_BUNDLE_PATH: Any
 DEFAULT_PORTS: dict[str, int]
 DEFAULT_ACCEPT_ENCODING: str
 
 def dict_to_sequence(d): ...
 def super_len(o): ...
-def get_netrc_auth(url: _Uri, raise_errors: bool = ...) -> tuple[str, str] | None: ...
+def get_netrc_auth(url: _Uri, raise_errors: bool = False) -> tuple[str, str] | None: ...
 def guess_filename(obj): ...
 def extract_zipped_paths(path): ...
+def atomic_open(filename: StrOrBytesPath) -> _GeneratorContextManager[BufferedWriter]: ...
 def from_key_val_list(value): ...
 def to_key_val_list(value): ...
 def parse_list_header(value): ...
 def parse_dict_header(value): ...
-def unquote_header_value(value, is_filename: bool = ...): ...
+def unquote_header_value(value, is_filename: bool = False): ...
 def dict_from_cookiejar(cj): ...
 def add_dict_to_cookiejar(cj, cookie_dict): ...
 def get_encodings_from_content(content): ...
 def get_encoding_from_headers(headers): ...
 def stream_decode_response_unicode(iterator, r): ...
 def iter_slices(string: str, slice_length: int | None) -> Generator[str, None, None]: ...
 def get_unicode_from_response(r): ...
@@ -39,21 +43,26 @@
 
 def unquote_unreserved(uri: str) -> str: ...
 def requote_uri(uri: str) -> str: ...
 def address_in_network(ip: str, net: str) -> bool: ...
 def dotted_netmask(mask: int) -> str: ...
 def is_ipv4_address(string_ip: str) -> bool: ...
 def is_valid_cidr(string_network: str) -> bool: ...
-def set_environ(env_name: str, value: None) -> AbstractContextManager[None]: ...
+def set_environ(env_name: str, value: None) -> _GeneratorContextManager[None]: ...
 def should_bypass_proxies(url: _Uri, no_proxy: Iterable[str] | None) -> bool: ...
-def get_environ_proxies(url: _Uri, no_proxy: Iterable[str] | None = ...) -> dict[Any, Any]: ...
+def get_environ_proxies(url: _Uri, no_proxy: Iterable[str] | None = None) -> dict[Any, Any]: ...
 def select_proxy(url: _Uri, proxies: Mapping[Any, Any] | None): ...
-def default_user_agent(name: str = ...) -> str: ...
+def resolve_proxies(request: Request | PreparedRequest, proxies: Mapping[str, str] | None, trust_env: bool = True): ...
+def default_user_agent(name: str = "python-requests") -> str: ...
 def default_headers() -> CaseInsensitiveDict[str]: ...
 def parse_header_links(value: str) -> list[dict[str, str]]: ...
 def guess_json_utf(data): ...
 def prepend_scheme_if_needed(url, new_scheme): ...
 def get_auth_from_url(url: _Uri) -> tuple[str, str]: ...
-def to_native_string(string, encoding=...): ...
+def to_native_string(string, encoding="ascii"): ...
 def urldefragauth(url: _Uri): ...
 def rewind_body(prepared_request: PreparedRequest) -> None: ...
 def check_header_validity(header: tuple[AnyStr, AnyStr]) -> None: ...
+
+if sys.platform == "win32":
+    def proxy_bypass_registry(host: str) -> bool: ...
+    def proxy_bypass(host: str) -> bool: ...
```

### Comparing `types-requests-2.28.9/setup.py` & `types-requests-2.29.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 from setuptools import setup
 
 name = "types-requests"
 description = "Typing stubs for requests"
 long_description = '''
 ## Typing stubs for requests
 
-This is a PEP 561 type stub package for the `requests` package.
-It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
-that uses `requests`. The source for this package can be found at
-https://github.com/python/typeshed/tree/master/stubs/requests. All fixes for
+This is a PEP 561 type stub package for the `requests` package. It
+can be used by type-checking tools like
+[mypy](https://github.com/python/mypy/),
+[pyright](https://github.com/microsoft/pyright),
+[pytype](https://github.com/google/pytype/),
+PyCharm, etc. to check code that uses
+`requests`. The source for this package can be found at
+https://github.com/python/typeshed/tree/main/stubs/requests. All fixes for
 types and metadata should be contributed there.
 
-See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `8c51fab4e26981b9e21f9d5c5483a42f4a73ce92`.
+See https://github.com/python/typeshed/blob/main/README.md for more details.
+This package was generated from typeshed commit `2d84e56d6fc12c08d43b4694703bd9a48a9c2b2f`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.28.9",
+      version="2.29.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['types-urllib3<1.27'],
       packages=['requests-stubs'],
-      package_data={'requests-stubs': ['__init__.pyi', '__version__.pyi', 'adapters.pyi', 'api.pyi', 'auth.pyi', 'compat.pyi', 'cookies.pyi', 'exceptions.pyi', 'help.pyi', 'hooks.pyi', 'models.pyi', 'packages.pyi', 'sessions.pyi', 'status_codes.pyi', 'structures.pyi', 'utils.pyi', 'METADATA.toml']},
+      package_data={'requests-stubs': ['__init__.pyi', '__version__.pyi', 'adapters.pyi', 'api.pyi', 'auth.pyi', 'certs.pyi', 'compat.pyi', 'cookies.pyi', 'exceptions.pyi', 'help.pyi', 'hooks.pyi', 'models.pyi', 'packages.pyi', 'sessions.pyi', 'status_codes.pyi', 'structures.pyi', 'utils.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-requests-2.28.9/types_requests.egg-info/PKG-INFO` & `types-requests-2.29.0.0/types_requests.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: types-requests
-Version: 2.28.9
+Version: 2.29.0.0
 Summary: Typing stubs for requests
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
 
 ## Typing stubs for requests
 
-This is a PEP 561 type stub package for the `requests` package.
-It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
-that uses `requests`. The source for this package can be found at
-https://github.com/python/typeshed/tree/master/stubs/requests. All fixes for
+This is a PEP 561 type stub package for the `requests` package. It
+can be used by type-checking tools like
+[mypy](https://github.com/python/mypy/),
+[pyright](https://github.com/microsoft/pyright),
+[pytype](https://github.com/google/pytype/),
+PyCharm, etc. to check code that uses
+`requests`. The source for this package can be found at
+https://github.com/python/typeshed/tree/main/stubs/requests. All fixes for
 types and metadata should be contributed there.
 
-See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `8c51fab4e26981b9e21f9d5c5483a42f4a73ce92`.
-
-
+See https://github.com/python/typeshed/blob/main/README.md for more details.
+This package was generated from typeshed commit `2d84e56d6fc12c08d43b4694703bd9a48a9c2b2f`.
```

### Comparing `types-requests-2.28.9/types_requests.egg-info/SOURCES.txt` & `types-requests-2.29.0.0/types_requests.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 requests-stubs/METADATA.toml
 requests-stubs/__init__.pyi
 requests-stubs/__version__.pyi
 requests-stubs/adapters.pyi
 requests-stubs/api.pyi
 requests-stubs/auth.pyi
+requests-stubs/certs.pyi
 requests-stubs/compat.pyi
 requests-stubs/cookies.pyi
 requests-stubs/exceptions.pyi
 requests-stubs/help.pyi
 requests-stubs/hooks.pyi
 requests-stubs/models.pyi
 requests-stubs/packages.pyi
```


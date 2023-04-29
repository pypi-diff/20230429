# Comparing `tmp/asgi_context-0.1.1.tar.gz` & `tmp/asgi_context-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgi_context-0.1.1.tar", last modified: Wed Apr 26 16:57:58 2023, max compression
+gzip compressed data, was "asgi_context-0.2.0.tar", last modified: Sat Apr 29 14:15:42 2023, max compression
```

## Comparing `asgi_context-0.1.1.tar` & `asgi_context-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0     1072 2023-04-26 16:57:32.809662 asgi_context-0.1.1/LICENSE
--rw-r--r--   0        0        0     1778 2023-04-26 16:57:32.813662 asgi_context-0.1.1/README.md
--rw-r--r--   0        0        0     4168 2023-04-26 16:57:32.813662 asgi_context-0.1.1/asgi_context/__init__.py
--rw-r--r--   0        0        0      253 2023-04-26 16:57:32.813662 asgi_context-0.1.1/pdm_build.py
--rw-r--r--   0        0        0     1793 2023-04-26 16:57:58.442051 asgi_context-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3782 2023-04-26 16:57:32.813662 asgi_context-0.1.1/tests/test_asgi_context.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 asgi_context-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-29 14:15:22.134448 asgi_context-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2872 2023-04-29 14:15:22.134448 asgi_context-0.2.0/README.md
+-rw-r--r--   0        0        0      356 2023-04-29 14:15:22.134448 asgi_context-0.2.0/asgi_context/__init__.py
+-rw-r--r--   0        0        0     1587 2023-04-29 14:15:22.134448 asgi_context-0.2.0/asgi_context/context.py
+-rw-r--r--   0        0        0     4195 2023-04-29 14:15:22.134448 asgi_context-0.2.0/asgi_context/headers_extrator.py
+-rw-r--r--   0        0        0      338 2023-04-29 14:15:22.134448 asgi_context-0.2.0/asgi_context/protocol.py
+-rw-r--r--   0        0        0      480 2023-04-29 14:15:22.134448 asgi_context-0.2.0/pdm_build.py
+-rw-r--r--   0        0        0     1824 2023-04-29 14:15:42.006631 asgi_context-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4360 2023-04-29 14:15:22.134448 asgi_context-0.2.0/tests/test_asgi_context.py
+-rw-r--r--   0        0        0     3166 1970-01-01 00:00:00.000000 asgi_context-0.2.0/PKG-INFO
```

### Comparing `asgi_context-0.1.1/LICENSE` & `asgi_context-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asgi_context-0.1.1/pyproject.toml` & `asgi_context-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -74,20 +74,22 @@
 line-length = 120
 unfixable = [
     "B",
 ]
 
 [project]
 name = "asgi_context"
-version = "0.1.1"
+version = "0.2.0"
 description = "Simple request context for ASGI compatible applications"
 authors = [
     { name = "Marcin Paliwoda", email = "paliwoda.marcin@zoho.com" },
 ]
-dependencies = []
+dependencies = [
+    "mypy-extensions>=1.0.0",
+]
 requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [build-system]
```

### Comparing `asgi_context-0.1.1/tests/test_asgi_context.py` & `asgi_context-0.2.0/tests/test_asgi_context.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import uuid
+from http import HTTPStatus
 
 import pytest
 from fastapi import FastAPI
 from fastapi.testclient import TestClient as FastAPITestClient
 from starlite import Starlite, get
 from starlite.testing import TestClient as StarliteTestClient
 
 from asgi_context import (
     ContextMiddleware,
     HeadersExtractorMiddlewareFactory,
-    HeaderValidationException,
     RequestContextException,
+    ValidationConfig,
     http_request_context,
 )
 
 
 class TestFastAPI:
     def test_fastapi_correct_setup(self):
         tracing_middleware = HeadersExtractorMiddlewareFactory.build("Tracing", header_names=["X-Trace-ID"])
@@ -52,30 +53,42 @@
             try:
                 uuid.UUID(value)
                 return True
             except ValueError:
                 return False
 
         tracing_middleware = HeadersExtractorMiddlewareFactory.build(
-            "Tracing", header_names=["X-Trace-ID"], validators={"X-Trace-ID": uuid_validator}
+            "Tracing",
+            header_names=["X-Trace-ID"],
+            validation_config=ValidationConfig(
+                err_on_missing=HTTPStatus.UNPROCESSABLE_ENTITY,
+                err_on_invalid=HTTPStatus.BAD_REQUEST,
+                validators={"X-Trace-ID": uuid_validator},
+            ),
         )
 
         app = FastAPI()
         app.add_middleware(tracing_middleware)
         app.add_middleware(ContextMiddleware)
 
         @app.get("/")
         async def index():
             return {"X-Trace-ID": http_request_context["X-Trace-ID"]}
 
         with FastAPITestClient(app) as client:
-            client.get("/", headers={"X-Trace-ID": "00703a09-a666-411e-940d-768489c69302"})
+            ok_response = client.get("/", headers={"X-Trace-ID": "00703a09-a666-411e-940d-768489c69302"})
+            assert ok_response.status_code == 200
 
-            with pytest.raises(HeaderValidationException):
-                client.get("/", headers={"X-Trace-ID": "hello"})
+            bad_response = client.get("/", headers={"X-Trace-ID": "hello"})
+            assert bad_response.status_code == 400
+            assert bad_response.json() == {"error": "Invalid value for header: X-Trace-ID"}
+
+            bad_response = client.get("/", headers={})
+            assert bad_response.status_code == 422
+            assert bad_response.json() == {"error": "Missing header: X-Trace-ID"}
 
 
 class TestStarlite:
     def test_starlite_correct_setup(self):
         @get("/")
         async def index() -> dict[str, str]:
             return {"X-Trace-ID": http_request_context["X-Trace-ID"]}
```

### Comparing `asgi_context-0.1.1/PKG-INFO` & `asgi_context-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: asgi-context
-Version: 0.1.1
-Summary: Simple request context for ASGI compatible applications
-Author-Email: Marcin Paliwoda <paliwoda.marcin@zoho.com>
-License: MIT
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # ASGI Context
 
 Zero dependency middleware for storing HTTP request data in scoped context.
 By default the library exposes the middleware for creating the context and
 header extrator builder which can be used e.g. for storing tracing headers.
 
 ## Installation
@@ -24,73 +15,102 @@
 or you can use pre-built sdist and wheels from `Releases` page.
 
 ## Example usage
 
 ### FastAPI
 
 ```python
+from http import HTTPStatus
+
 from fastapi import FastAPI
 
 from asgi_context import (
     http_requst_context,
     ContextMiddleware,
     HeadersExtractorMiddlewareFactory,
+    ValidationConfig,
 )
 
 app = FastAPI()
 
 def example_headers_validator(header_value: str) -> bool:
     return "example" in value
 
-example_headers_extractor_middleware = HeadersExtractorMiddlewareFactory.build(
-    base_name="example",
-    header_names=("X-Example",)
-    validators={
-        "X-Example": example_headers_validator,
-    }
+# will return 400 when missing specified headers or headers don't pass validation
+example_headers_extractor_with_validation = HeadersExtractorMiddlewareFactory.build(
+    base_name="example_with_validation",
+    header_names=("X-Example",),
+    validation_config=ValidationConfig(
+        err_on_missing=HTTPStatus.BAD_REQUEST,
+        err_on_invalid=HTTPStatus.BAD_REQUEST,
+        validators={
+            "X-Example": example_headers_validator,
+        },
+    ),
+)
+
+example_headers_extractor_without_validation = HeadersExtractorMiddlewareFactory.build(
+    base_name="example_without_validation",
+    header_names=("X-Not-Validated-Example",)
 )
 
-app.add_middleware(example_headers_extractor_middleware)
+app.add_middleware(example_headers_extractor_with_validation)
+app.add_middleware(example_headers_extractor_without_validation)
 app.add_middleware(ContextMiddleware)
 
 @app.get("/")
 def index():
     return http_request_context["X-Example"]
 ```
 
 ### Starlite
 
 ```python
+from http import HTTPStatus
+
 from starlite import Starlite, get
 
 from asgi_context import (
     http_requst_context,
     ContextMiddleware,
     HeadersExtractorMiddlewareFactory,
+    ValidationConfig,
 )
 
 def example_headers_validator(header_value: str) -> bool:
     return "example" in value
 
 
-example_headers_extractor_middleware = HeadersExtractorMiddlewareFactory.build(
+# will return 400 when missing specified headers or headers don't pass validation
+example_headers_extractor_with_validation = HeadersExtractorMiddlewareFactory.build(
     base_name="example",
     header_names=("X-Example",)
-    validators={
-        "X-Example": example_headers_validator,
-    }
+    validation_config=ValidationConfig(
+        err_on_missing=HTTPStatus.BAD_REQUEST,
+        err_on_invalid=HTTPStatus.BAD_REQUEST,
+        validators={
+            "X-Example": example_headers_validator,
+        },
+    ),
+)
+
+
+example_headers_extractor_without_validation = HeadersExtractorMiddlewareFactory.build(
+    base_name="example_without_validation",
+    header_names=("X-Not-Validated-Example",)
 )
 
 
 @get("/")
 def index() -> str:
     return http_request_context["X-Example"]
 
 
 app = Starlite(
     route_handlers=[index],
     middleware=[
         ContextMiddleware,
-        example_headers_extractor_middleware
+        example_headers_extractor_with_validation,
+        example_headers_extractor_without_validation,
     ]
 )
 ```
```


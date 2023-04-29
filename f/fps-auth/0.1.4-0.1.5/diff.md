# Comparing `tmp/fps_auth-0.1.4.tar.gz` & `tmp/fps_auth-0.1.5.tar.gz`

## Comparing `fps_auth-0.1.4.tar` & `fps_auth-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_auth-0.1.4/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_auth-0.1.4/fps_auth/__init__.py
--rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 fps_auth-0.1.4/fps_auth/backends.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fps_auth-0.1.4/fps_auth/config.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 fps_auth-0.1.4/fps_auth/db.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 fps_auth-0.1.4/fps_auth/main.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fps_auth-0.1.4/fps_auth/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_auth-0.1.4/fps_auth/py.typed
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 fps_auth-0.1.4/fps_auth/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_auth-0.1.4/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth-0.1.4/COPYING.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_auth-0.1.4/README.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 fps_auth-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fps_auth-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_auth-0.1.5/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_auth-0.1.5/fps_auth/__init__.py
+-rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 fps_auth-0.1.5/fps_auth/backends.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fps_auth-0.1.5/fps_auth/config.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 fps_auth-0.1.5/fps_auth/db.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 fps_auth-0.1.5/fps_auth/main.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fps_auth-0.1.5/fps_auth/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_auth-0.1.5/fps_auth/py.typed
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 fps_auth-0.1.5/fps_auth/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_auth-0.1.5/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth-0.1.5/COPYING.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_auth-0.1.5/README.md
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 fps_auth-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 fps_auth-0.1.5/PKG-INFO
```

### Comparing `fps_auth-0.1.4/fps_auth/backends.py` & `fps_auth-0.1.5/fps_auth/backends.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import uuid
 from dataclasses import dataclass
-from typing import Any, Dict, Generic, List, Optional, Tuple
+from typing import Any, Dict, Generic, List, Optional, Tuple, cast
 
 import httpx
 from fastapi import Depends, HTTPException, Response, WebSocket, status
 from fastapi_users import (
     BaseUserManager,
     FastAPIUsers,
     UUIDIDMixin,
@@ -48,19 +48,19 @@
     class NoAuthScheme:
         def __call__(self):
             return "noauth"
 
     class NoAuthTransport(Transport):
         scheme = NoAuthScheme()  # type: ignore
 
-        async def get_login_response(self, token: str, response: Response):
-            pass
+        async def get_login_response(self, token: str) -> Response:
+            return Response()
 
-        async def get_logout_response(self, response: Response):
-            pass
+        async def get_logout_response(self) -> Response:
+            return Response()
 
         @staticmethod
         def get_openapi_login_responses_success():
             pass
 
         @staticmethod
         def get_openapi_logout_responses_success():
@@ -76,18 +76,19 @@
         async def write_token(self, user: models.UP):
             pass
 
         async def destroy_token(self, token: str, user: models.UP):
             pass
 
     class GitHubTransport(CookieTransport):
-        async def get_login_response(self, token: str, response: Response):
-            await super().get_login_response(token, response)
+        async def get_login_response(self, token: str) -> Response:
+            response = await super().get_login_response(token)
             response.status_code = status.HTTP_302_FOUND
             response.headers["Location"] = "/lab"
+            return response
 
     def get_noauth_strategy() -> NoAuthStrategy:
         return NoAuthStrategy()
 
     def get_jwt_strategy() -> JWTStrategy:
         return JWTStrategy(secret=db.secret, lifetime_seconds=None)
 
@@ -186,27 +187,37 @@
                             user = None
                             break
             else:
                 # "noauth" or "token" authentication
                 if frontend_config.collaborative:
                     if not user and auth_config.mode == "noauth":
                         user = await create_guest(user_manager)
-                        await cookie_authentication.login(get_jwt_strategy(), user, response)
+                        token = await get_jwt_strategy().write_token(user)
+                        cookie_transport = cast(CookieTransport, cookie_authentication.transport)
+                        cookie_transport._set_login_cookie(response, token)
 
                     elif not user and auth_config.mode == "token":
                         global_user = await user_manager.get_by_email(auth_config.global_email)
                         if global_user and global_user.username == token:
                             user = await create_guest(user_manager)
-                            await cookie_authentication.login(get_jwt_strategy(), user, response)
+                            token = await get_jwt_strategy().write_token(user)
+                            cookie_transport = cast(
+                                CookieTransport, cookie_authentication.transport
+                            )
+                            cookie_transport._set_login_cookie(response, token)
                 else:
                     if auth_config.mode == "token":
                         global_user = await user_manager.get_by_email(auth_config.global_email)
                         if global_user and global_user.username == token:
                             user = global_user
-                            await cookie_authentication.login(get_jwt_strategy(), user, response)
+                            token = await get_jwt_strategy().write_token(user)
+                            cookie_transport = cast(
+                                CookieTransport, cookie_authentication.transport
+                            )
+                            cookie_transport._set_login_cookie(response, token)
 
             if user:
                 return user
 
             elif auth_config.login_url:
                 raise RedirectException(auth_config.login_url)
```

### Comparing `fps_auth-0.1.4/fps_auth/config.py` & `fps_auth-0.1.5/fps_auth/config.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.4/fps_auth/db.py` & `fps_auth-0.1.5/fps_auth/db.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.4/fps_auth/main.py` & `fps_auth-0.1.5/fps_auth/main.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.4/fps_auth/routes.py` & `fps_auth-0.1.5/fps_auth/routes.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.4/.gitignore` & `fps_auth-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.4/COPYING.md` & `fps_auth-0.1.5/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.4/pyproject.toml` & `fps_auth-0.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "fps_auth"
 description = "An FPS plugin for the authentication API"
 keywords = ["jupyter", "server", "fastapi", "plugins"]
 dynamic = ["version"]
 requires-python = ">=3.8"
 dependencies = [
     "aiosqlite",
-    "fastapi-users[sqlalchemy,oauth] >=10.1.4,<11",
+    "fastapi-users[sqlalchemy,oauth] >=11,<12",
     "sqlalchemy >=1,<2",
     "jupyverse-api >=0.1.2,<1",
 ]
 
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
```


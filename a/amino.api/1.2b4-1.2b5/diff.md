# Comparing `tmp/amino.api-1.2b4.tar.gz` & `tmp/amino.api-1.2b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.api-1.2b4.tar", last modified: Sat Apr 29 15:37:46 2023, max compression
+gzip compressed data, was "amino.api-1.2b5.tar", last modified: Sat Apr 29 17:32:17 2023, max compression
```

## Comparing `amino.api-1.2b4.tar` & `amino.api-1.2b5.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 15:37:46.404132 amino.api-1.2b4/
--rw-rw-rw-   0        0        0      773 2023-04-29 15:37:46.404132 amino.api-1.2b4/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-22 10:17:55.000000 amino.api-1.2b4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 15:37:46.359136 amino.api-1.2b4/amino/
--rw-rw-rw-   0        0        0      883 2023-04-29 15:37:12.000000 amino.api-1.2b4/amino/__init__.py
--rw-rw-rw-   0        0        0    36475 2023-04-28 13:47:41.000000 amino.api-1.2b4/amino/client.py
--rw-rw-rw-   0        0        0    18444 2023-04-29 14:43:07.000000 amino.api-1.2b4/amino/full_client.py
--rw-rw-rw-   0        0        0    10956 2023-04-28 22:02:14.000000 amino.api-1.2b4/amino/local_client.py
--rw-rw-rw-   0        0        0    11535 2023-04-21 23:43:16.000000 amino.api-1.2b4/amino/socket.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:37:46.403125 amino.api-1.2b4/amino/utils/
--rw-rw-rw-   0        0        0        0 2023-04-21 21:48:51.000000 amino.api-1.2b4/amino/utils/__init__.py
--rw-rw-rw-   0        0        0     1099 2023-04-28 13:22:02.000000 amino.api-1.2b4/amino/utils/exceptions.py
--rw-rw-rw-   0        0        0     7429 2023-04-22 10:56:39.000000 amino.api-1.2b4/amino/utils/helpers.py
--rw-rw-rw-   0        0        0    14652 2023-04-29 15:04:24.000000 amino.api-1.2b4/amino/utils/objects.py
--rw-rw-rw-   0        0        0     2270 2023-04-22 10:51:46.000000 amino.api-1.2b4/amino/utils/requester.py
--rw-rw-rw-   0        0        0     3660 2023-04-26 13:04:41.000000 amino.api-1.2b4/amino/utils/snippetTools.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:37:46.385142 amino.api-1.2b4/amino.api.egg-info/
--rw-rw-rw-   0        0        0      773 2023-04-29 15:37:44.000000 amino.api-1.2b4/amino.api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-04-29 15:37:45.000000 amino.api-1.2b4/amino.api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 15:37:44.000000 amino.api-1.2b4/amino.api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-29 15:37:44.000000 amino.api-1.2b4/amino.api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-29 15:37:44.000000 amino.api-1.2b4/amino.api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 15:37:46.406130 amino.api-1.2b4/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-04-29 15:37:22.000000 amino.api-1.2b4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:32:17.968560 amino.api-1.2b5/
+-rw-rw-rw-   0        0        0      773 2023-04-29 17:32:17.968560 amino.api-1.2b5/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-04-22 10:17:55.000000 amino.api-1.2b5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 17:32:17.945092 amino.api-1.2b5/amino/
+-rw-rw-rw-   0        0        0      922 2023-04-29 17:31:29.000000 amino.api-1.2b5/amino/__init__.py
+-rw-rw-rw-   0        0        0       50 2023-04-21 21:48:51.000000 amino.api-1.2b5/amino/async_client.py
+-rw-rw-rw-   0        0        0       56 2023-04-21 21:48:51.000000 amino.api-1.2b5/amino/async_full_client.py
+-rw-rw-rw-   0        0        0       59 2023-04-21 21:48:51.000000 amino.api-1.2b5/amino/async_local_client.py
+-rw-rw-rw-   0        0        0       50 2023-04-21 21:48:51.000000 amino.api-1.2b5/amino/async_socket.py
+-rw-rw-rw-   0        0        0    36475 2023-04-28 13:47:41.000000 amino.api-1.2b5/amino/client.py
+-rw-rw-rw-   0        0        0    18444 2023-04-29 14:43:07.000000 amino.api-1.2b5/amino/full_client.py
+-rw-rw-rw-   0        0        0    10956 2023-04-28 22:02:14.000000 amino.api-1.2b5/amino/local_client.py
+-rw-rw-rw-   0        0        0    11535 2023-04-21 23:43:16.000000 amino.api-1.2b5/amino/socket.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:32:17.967560 amino.api-1.2b5/amino/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-21 21:48:51.000000 amino.api-1.2b5/amino/utils/__init__.py
+-rw-rw-rw-   0        0        0     1099 2023-04-28 13:22:02.000000 amino.api-1.2b5/amino/utils/exceptions.py
+-rw-rw-rw-   0        0        0     7429 2023-04-22 10:56:39.000000 amino.api-1.2b5/amino/utils/helpers.py
+-rw-rw-rw-   0        0        0    14652 2023-04-29 15:04:24.000000 amino.api-1.2b5/amino/utils/objects.py
+-rw-rw-rw-   0        0        0     2270 2023-04-22 10:51:46.000000 amino.api-1.2b5/amino/utils/requester.py
+-rw-rw-rw-   0        0        0     3660 2023-04-26 13:04:41.000000 amino.api-1.2b5/amino/utils/snippetTools.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:32:17.958558 amino.api-1.2b5/amino.api.egg-info/
+-rw-rw-rw-   0        0        0      773 2023-04-29 17:32:17.000000 amino.api-1.2b5/amino.api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2023-04-29 17:32:17.000000 amino.api-1.2b5/amino.api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 17:32:17.000000 amino.api-1.2b5/amino.api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-29 17:32:17.000000 amino.api-1.2b5/amino.api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-29 17:32:17.000000 amino.api-1.2b5/amino.api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 17:32:17.970560 amino.api-1.2b5/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-04-29 17:31:45.000000 amino.api-1.2b5/setup.py
```

### Comparing `amino.api-1.2b4/PKG-INFO` & `amino.api-1.2b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.api
-Version: 1.2b4
+Version: 1.2b5
 Summary: Library for creating amino bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/amino.api
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip
 Description: <h1 align="center">Amino.API</h1>
```

### Comparing `amino.api-1.2b4/amino/__init__.py` & `amino.api-1.2b5/amino/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 
 
 from .utils import helpers, exceptions, objects, requester
 from .client import Client
 from .local_client import LocalClient
 from .full_client import FullClient
 
-from .asynclib.client import AsyncClient
-from .asynclib.local_client import AsyncLocalClient
-from .asynclib.socket import AsyncSocket
+from .async_client import AsyncClient
+from .async_local_client import AsyncLocalClient
+from .async_socket import AsyncSocket
+from .async_full_client import AsyncFullClient
 
 from os import system as s
 from json import loads
 from requests import get
 
 __title__ = 'amino.api'
 __author__ = 'Xsarz'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Xsarz'
-__version__ = '1.2b4'
+__version__ = '1.2b5'
 __newest__ = loads(get("https://pypi.org/pypi/amino.api/json").text)["info"]["version"]
 
 
 
 if __version__ != __newest__:
 	s('cls || clear')
 	print(f'\033[38;5;214m{__title__} made by {__author__}\nPlease update the library. Your version: {__version__}  A new version:{__newest__}\033[0m')
```

### Comparing `amino.api-1.2b4/amino/client.py` & `amino.api-1.2b5/amino/client.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b4/amino/full_client.py` & `amino.api-1.2b5/amino/full_client.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b4/amino/local_client.py` & `amino.api-1.2b5/amino/local_client.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b4/amino/socket.py` & `amino.api-1.2b5/amino/socket.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b4/amino/utils/exceptions.py` & `amino.api-1.2b5/amino/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b4/amino/utils/helpers.py` & `amino.api-1.2b5/amino/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b4/amino/utils/objects.py` & `amino.api-1.2b5/amino/utils/objects.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b4/amino/utils/requester.py` & `amino.api-1.2b5/amino/utils/requester.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b4/amino/utils/snippetTools.py` & `amino.api-1.2b5/amino/utils/snippetTools.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b4/amino.api.egg-info/PKG-INFO` & `amino.api-1.2b5/amino.api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.api
-Version: 1.2b4
+Version: 1.2b5
 Summary: Library for creating amino bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/amino.api
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip
 Description: <h1 align="center">Amino.API</h1>
```

### Comparing `amino.api-1.2b4/setup.py` & `amino.api-1.2b5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 info = {
 	"name": "amino.api",
-	"version": "1.2b4",
+	"version": "1.2b5",
 	"github_page": "https://github.com/xXxCLOTIxXx/amino.api",
 	"download_link": "https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip",
 	"license": "MIT",
 	"author": "Xsarz",
 	"author_email": "xsarzy@gmail.com",
 	"description": "Library for creating amino bots and scripts.",
 	"long_description": None,
```


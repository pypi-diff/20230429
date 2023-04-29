# Comparing `tmp/pyoscar_emr-0.9.0.tar.gz` & `tmp/pyoscar_emr-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoscar_emr-0.9.0.tar", max compression
+gzip compressed data, was "pyoscar_emr-0.9.1.tar", max compression
```

## Comparing `pyoscar_emr-0.9.0.tar` & `pyoscar_emr-0.9.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-04-27 18:31:38.067485 pyoscar_emr-0.9.0/LICENSE
--rw-r--r--   0        0        0      193 2023-04-27 18:32:41.748181 pyoscar_emr-0.9.0/README.md
--rw-r--r--   0        0        0      331 2023-04-19 03:35:10.246610 pyoscar_emr-0.9.0/pyoscar_emr/__init__.py
--rw-r--r--   0        0        0     2050 2023-04-19 03:35:19.937225 pyoscar_emr-0.9.0/pyoscar_emr/appointment.py
--rw-r--r--   0        0        0     1311 2023-04-19 03:35:17.453180 pyoscar_emr-0.9.0/pyoscar_emr/appointment_status.py
--rw-r--r--   0        0        0     2652 2023-04-19 03:35:22.570531 pyoscar_emr-0.9.0/pyoscar_emr/demographic.py
--rw-r--r--   0        0        0     2497 2023-04-19 03:35:25.414929 pyoscar_emr-0.9.0/pyoscar_emr/endpoints.py
--rw-r--r--   0        0        0      259 2023-04-27 18:22:39.524253 pyoscar_emr-0.9.0/pyoscar_emr/exceptions.py
--rw-r--r--   0        0        0     1081 2023-04-19 03:35:45.949559 pyoscar_emr-0.9.0/pyoscar_emr/ontario_health_card.py
--rw-r--r--   0        0        0    16042 2023-04-27 18:09:12.134337 pyoscar_emr-0.9.0/pyoscar_emr/oscar.py
--rw-r--r--   0        0        0      191 2023-04-19 03:36:01.949472 pyoscar_emr-0.9.0/pyoscar_emr/response_type.py
--rw-r--r--   0        0        0     7949 2023-04-27 18:10:49.311346 pyoscar_emr-0.9.0/pyoscar_emr/util/get_oauth_creds.py
--rw-r--r--   0        0        0      653 2023-04-27 18:25:59.845671 pyoscar_emr-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 pyoscar_emr-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-27 18:31:38.067485 pyoscar_emr-0.9.1/LICENSE
+-rw-r--r--   0        0        0      193 2023-04-27 18:32:41.748181 pyoscar_emr-0.9.1/README.md
+-rw-r--r--   0        0        0      331 2023-04-19 03:35:10.246610 pyoscar_emr-0.9.1/pyoscar_emr/__init__.py
+-rw-r--r--   0        0        0     2050 2023-04-19 03:35:19.937225 pyoscar_emr-0.9.1/pyoscar_emr/appointment.py
+-rw-r--r--   0        0        0     1311 2023-04-19 03:35:17.453180 pyoscar_emr-0.9.1/pyoscar_emr/appointment_status.py
+-rw-r--r--   0        0        0     2652 2023-04-19 03:35:22.570531 pyoscar_emr-0.9.1/pyoscar_emr/demographic.py
+-rw-r--r--   0        0        0     2497 2023-04-19 03:35:25.414929 pyoscar_emr-0.9.1/pyoscar_emr/endpoints.py
+-rw-r--r--   0        0        0      259 2023-04-27 18:22:39.524253 pyoscar_emr-0.9.1/pyoscar_emr/exceptions.py
+-rw-r--r--   0        0        0     1081 2023-04-19 03:35:45.949559 pyoscar_emr-0.9.1/pyoscar_emr/ontario_health_card.py
+-rw-r--r--   0        0        0    16062 2023-04-29 16:49:48.960440 pyoscar_emr-0.9.1/pyoscar_emr/oscar.py
+-rw-r--r--   0        0        0      191 2023-04-19 03:36:01.949472 pyoscar_emr-0.9.1/pyoscar_emr/response_type.py
+-rw-r--r--   0        0        0     7949 2023-04-27 18:10:49.311346 pyoscar_emr-0.9.1/pyoscar_emr/util/get_oauth_creds.py
+-rw-r--r--   0        0        0      653 2023-04-29 16:55:56.374399 pyoscar_emr-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 pyoscar_emr-0.9.1/PKG-INFO
```

### Comparing `pyoscar_emr-0.9.0/LICENSE` & `pyoscar_emr-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoscar_emr-0.9.0/pyoscar_emr/appointment.py` & `pyoscar_emr-0.9.1/pyoscar_emr/appointment.py`

 * *Files identical despite different names*

### Comparing `pyoscar_emr-0.9.0/pyoscar_emr/appointment_status.py` & `pyoscar_emr-0.9.1/pyoscar_emr/appointment_status.py`

 * *Files identical despite different names*

### Comparing `pyoscar_emr-0.9.0/pyoscar_emr/demographic.py` & `pyoscar_emr-0.9.1/pyoscar_emr/demographic.py`

 * *Files identical despite different names*

### Comparing `pyoscar_emr-0.9.0/pyoscar_emr/endpoints.py` & `pyoscar_emr-0.9.1/pyoscar_emr/endpoints.py`

 * *Files identical despite different names*

### Comparing `pyoscar_emr-0.9.0/pyoscar_emr/ontario_health_card.py` & `pyoscar_emr-0.9.1/pyoscar_emr/ontario_health_card.py`

 * *Files identical despite different names*

### Comparing `pyoscar_emr-0.9.0/pyoscar_emr/oscar.py` & `pyoscar_emr-0.9.1/pyoscar_emr/oscar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import aiohttp
 import json
 
-from playwright.async_api import Playwright
+from playwright.async_api import Playwright, BrowserType
 from playwright_stealth import stealth_async
 
 import oauthlib.oauth1
 from datetime import datetime
 import logging
 from xml.etree import ElementTree
 import re
@@ -98,26 +98,29 @@
         )
 
         self._statuses = await self.get_appointment_statuses()
 
         return self
 
     async def activate_webscraping(
-        self, username: str, password: str, pin: str, playwright_context: Playwright
+        self,
+        username: str,
+        password: str,
+        pin: str,
+        browser_type: BrowserType,
+        headless: bool = True,
     ) -> None:
         """
         Set up web scraping and enable functions that require it (ex. checking if health card is valid).
         Please note that the playwright context should always be alive.
         Raises OscarAPIInvalidCredentials if the credentials were invalid.
         """
 
-        self.playwright_context = playwright_context
-
         # Log into OSCAR
-        self.playwright_browser = await playwright_context.chromium.launch()
+        self.playwright_browser = await browser_type.launch(headless=headless)
         page = await self.playwright_browser.new_page()
         await stealth_async(page)
         await page.goto(self._endpoint_webscraping.login.url)
 
         # Interact with login form
         await page.get_by_placeholder("Username:").fill(username)
         await page.get_by_placeholder("Password:").fill(password)
```

### Comparing `pyoscar_emr-0.9.0/pyoscar_emr/util/get_oauth_creds.py` & `pyoscar_emr-0.9.1/pyoscar_emr/util/get_oauth_creds.py`

 * *Files identical despite different names*

### Comparing `pyoscar_emr-0.9.0/pyproject.toml` & `pyoscar_emr-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyoscar_emr"
-version = "0.9.0"
+version = "0.9.1"
 description = "Python wrapper for the OSCAR EMR API"
 authors = ["Aritro <29025984+AritroSaha10@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = {extras = ["speedups"], version = "^3.8.4"}
```

### Comparing `pyoscar_emr-0.9.0/PKG-INFO` & `pyoscar_emr-0.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoscar-emr
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python wrapper for the OSCAR EMR API
 Author: Aritro
 Author-email: 29025984+AritroSaha10@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp[speedups] (>=3.8.4,<4.0.0)
```


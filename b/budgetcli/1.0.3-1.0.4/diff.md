# Comparing `tmp/budgetcli-1.0.3.tar.gz` & `tmp/budgetcli-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budgetcli-1.0.3.tar", last modified: Thu Apr 27 19:26:17 2023, max compression
+gzip compressed data, was "budgetcli-1.0.4.tar", last modified: Sat Apr 29 18:41:58 2023, max compression
```

## Comparing `budgetcli-1.0.3.tar` & `budgetcli-1.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:26:17.646772 budgetcli-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-27 19:25:52.000000 budgetcli-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-27 19:26:17.646772 budgetcli-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-27 19:25:52.000000 budgetcli-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-27 19:25:52.000000 budgetcli-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-27 19:26:17.646772 budgetcli-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:26:17.642773 budgetcli-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:26:17.646772 budgetcli-1.0.3/src/budgetcli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:26:17.646772 budgetcli-1.0.3/src/budgetcli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/cli/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:26:17.646772 budgetcli-1.0.3/src/budgetcli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-27 19:25:52.000000 budgetcli-1.0.3/src/budgetcli/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:26:17.646772 budgetcli-1.0.3/src/budgetcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-27 19:26:17.000000 budgetcli-1.0.3/src/budgetcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-27 19:26:17.000000 budgetcli-1.0.3/src/budgetcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:26:17.000000 budgetcli-1.0.3/src/budgetcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-27 19:26:17.000000 budgetcli-1.0.3/src/budgetcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-27 19:26:17.000000 budgetcli-1.0.3/src/budgetcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 19:26:17.000000 budgetcli-1.0.3/src/budgetcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:41:58.841636 budgetcli-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-29 18:41:36.000000 budgetcli-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-29 18:41:58.841636 budgetcli-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-29 18:41:36.000000 budgetcli-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-29 18:41:36.000000 budgetcli-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-29 18:41:58.841636 budgetcli-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:41:58.837636 budgetcli-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:41:58.837636 budgetcli-1.0.4/src/budgetcli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:41:58.841636 budgetcli-1.0.4/src/budgetcli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/cli/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:41:58.841636 budgetcli-1.0.4/src/budgetcli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-29 18:41:36.000000 budgetcli-1.0.4/src/budgetcli/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:41:58.841636 budgetcli-1.0.4/src/budgetcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-29 18:41:58.000000 budgetcli-1.0.4/src/budgetcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-29 18:41:58.000000 budgetcli-1.0.4/src/budgetcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:41:58.000000 budgetcli-1.0.4/src/budgetcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-29 18:41:58.000000 budgetcli-1.0.4/src/budgetcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-29 18:41:58.000000 budgetcli-1.0.4/src/budgetcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 18:41:58.000000 budgetcli-1.0.4/src/budgetcli.egg-info/top_level.txt
```

### Comparing `budgetcli-1.0.3/LICENSE` & `budgetcli-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.3/PKG-INFO` & `budgetcli-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budgetcli
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple async budgeting app to manage expenses and budgets in google spreadsheets
 Author: Code Rustle
 Author-email: coderustle@gmail.com
 License: MIT
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `budgetcli-1.0.3/README.md` & `budgetcli-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.3/setup.cfg` & `budgetcli-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = budgetcli
-version = 1.0.3
+version = 1.0.4
 author = Code Rustle
 author_email = coderustle@gmail.com
 description = A simple async budgeting app to manage expenses and budgets in google spreadsheets
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_file = LICENSE
```

### Comparing `budgetcli-1.0.3/src/budgetcli/auth.py` & `budgetcli-1.0.4/src/budgetcli/auth.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.3/src/budgetcli/cli/add.py` & `budgetcli-1.0.4/src/budgetcli/cli/add.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.3/src/budgetcli/cli/config.py` & `budgetcli-1.0.4/src/budgetcli/cli/config.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.3/src/budgetcli/cli/display.py` & `budgetcli-1.0.4/src/budgetcli/cli/display.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.3/src/budgetcli/commands.py` & `budgetcli-1.0.4/src/budgetcli/commands.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.3/src/budgetcli/data_manager.py` & `budgetcli-1.0.4/src/budgetcli/data_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from rich.pretty import pprint
 
 import httpx
 from google.oauth2.credentials import Credentials
 
 from .auth import load_user_token
 from .settings import API_URL, GVI_URL
-from .utils.config import get_config
+from .utils.config import get_config, update_config
 
 T = TypeVar("T", bound="AbstractDataManager")
 
 SPREADSHEET_ID = get_config("spreadsheet_id")
 
 
 class AbstractDataManager(ABC, Generic[T]):
@@ -49,17 +49,17 @@
             result = response.json()
             return result.get("values", [])
         except httpx.HTTPStatusError as err:
             req_url = err.request.url
             status = err.response.status_code
             pprint(f"Error calling {req_url}, http status: {status}")
 
-    async def _query(self, query: str) -> list[dict[str, list]] | None:
+    async def _query(self, query: str, sheet_index: int) -> list[dict[str, list]] | None:
         """A method to use Goolge Visualization API"""
-        params = f"gid={1}&tq={query}&tqx=out:json"
+        params = f"gid={sheet_index}&tq={query}&tqx=out:json"
         url = f"{self.gvi_url}?{params}"
         response = await self.session.get(url)
         try:
             response.raise_for_status()
             to_replace = "/*O_o*/\ngoogle.visualization.Query.setResponse("
             clean_data = response.text.replace(to_replace, "")[:-2]
             json_data = json.loads(clean_data)
@@ -93,55 +93,89 @@
                     return True
         except httpx.HTTPStatusError as err:
             req_url = err.request.url
             status = err.response.status_code
             pprint(f"Error calling {req_url}, http status: {status}")
         return False
 
-    async def create_sheet(self, title: str) -> bool:
+    async def get_sheet_index(self, title: str) -> int:
+        """Get google sheet index position"""
+        params = "fields=sheets"
+        url = f"{self.base_url}?{params}"
+        response = await self.session.get(url)
+        try:
+            response.raise_for_status()
+            data = response.json()
+            sheets = data.get("sheets")
+            for sheet in sheets:
+                if sheet["properties"]["title"] == title:
+                    sheet_index = sheet["properties"]["index"]
+                    return sheet_index
+        except httpx.HTTPStatusError as err:
+            req_url = err.request.url
+            status = err.response.status_code
+            pprint(f"Error calling {req_url}, http status: {status}")
+        return -1
+
+    async def create_sheet(self, title: str) -> dict[str, str] | None:
         """Create sheet with the given title"""
         url = f"{self.base_url}/:batchUpdate"
         body = {"requests": [{"addSheet": {"properties": {"title": title}}}]}
         response = await self.session.post(url, json=body)
         try:
             response.raise_for_status()
-            return True
+            data = response.json()
+            replies = data.get('replies', []) 
+            sheet = replies[0].get("addSheet")
+            properties = sheet.get("properties")
+            return properties
         except httpx.HTTPStatusError as err:
             req_url = err.request.url
             status = err.response.status_code
             pprint(f"Error calling {req_url}, http status: {status}")
-        return False
 
 
 class TransactionDataManager(AbstractDataManager):
     SHEET_NAME = "TRANSACTIONS!"
     FIRST_COLUMN = "A"
     LAST_COLUMN = "E"
     TRANSACTIONS_RANGE = f"{SHEET_NAME}{FIRST_COLUMN}1:{LAST_COLUMN}"
 
     async def init_sheet(self):
         """Create TRANSACTIONS sheet if not exists"""
-        check_task = asyncio.create_task(self.sheet_exists("TRANSACTIONS"))
-        create_task = asyncio.create_task(self.create_sheet("TRANSACTIONS"))
+        check = self.sheet_exists("TRANSACTIONS")
+        index = self.get_sheet_index("TRANSACTIONS")
         try:
-            sheet = await asyncio.wait_for(check_task, timeout=5)
-            if not sheet:
-                await asyncio.wait_for(create_task, timeout=5)
+            exists = await asyncio.wait_for(check, timeout=5)
+            if exists:
+                index = await asyncio.wait_for(index, timeout=5)
+                update_config("transactions_sheet_index", str(index))
+            else:
+                create = self.create_sheet("TRANSACTIONS")
+                properties = await asyncio.wait_for(create, timeout=5)
+                if properties:
+                    index =  properties.get("index")
+                    update_config("transactions_sheet_index", str(index))
         except asyncio.TimeoutError:
             print("Timeout error")
 
     async def get_transactions_for_month(
-        self, month: int
+        self, month: int 
     ) -> list[list[str]] | None:
         """Query the transactions for current month"""
         month = month - 1  # month query starts from 0 to 11
         query = f"select A,B,C,D,E where month(A)={month}"
         transactions = []
-        rows = await self._query(query)
-        pprint(rows, expand_all=True)
+        sheet_index = get_config("transactions_sheet_index")
+        rows = None
+        if sheet_index:
+            index = int(sheet_index)
+            rows = await self._query(query, index)
+        else:
+            rows = await self._query(query, 0)
         if rows:
             for row in rows:
                 transaction = []
                 for cel in row.get("c", []):
                     if "Date(" in str(cel.get("v")):
                         date = cel.get("f")
                         transaction.append(date)
```

### Comparing `budgetcli-1.0.3/src/budgetcli/main.py` & `budgetcli-1.0.4/src/budgetcli/main.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.3/src/budgetcli/models.py` & `budgetcli-1.0.4/src/budgetcli/models.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.3/src/budgetcli/settings.py` & `budgetcli-1.0.4/src/budgetcli/settings.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.3/src/budgetcli/utils/config.py` & `budgetcli-1.0.4/src/budgetcli/utils/config.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.3/src/budgetcli/utils/dates.py` & `budgetcli-1.0.4/src/budgetcli/utils/dates.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.3/src/budgetcli/utils/display.py` & `budgetcli-1.0.4/src/budgetcli/utils/display.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.0.3/src/budgetcli.egg-info/PKG-INFO` & `budgetcli-1.0.4/src/budgetcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budgetcli
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple async budgeting app to manage expenses and budgets in google spreadsheets
 Author: Code Rustle
 Author-email: coderustle@gmail.com
 License: MIT
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `budgetcli-1.0.3/src/budgetcli.egg-info/SOURCES.txt` & `budgetcli-1.0.4/src/budgetcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*


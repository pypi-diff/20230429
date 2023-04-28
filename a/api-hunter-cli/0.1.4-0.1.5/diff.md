# Comparing `tmp/api_hunter_cli-0.1.4.tar.gz` & `tmp/api_hunter_cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_hunter_cli-0.1.4.tar", last modified: Fri Apr 28 22:56:29 2023, max compression
+gzip compressed data, was "api_hunter_cli-0.1.5.tar", last modified: Fri Apr 28 23:03:43 2023, max compression
```

## Comparing `api_hunter_cli-0.1.4.tar` & `api_hunter_cli-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 22:56:29.986945 api_hunter_cli-0.1.4/
--rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 22:56:29.986945 api_hunter_cli-0.1.4/PKG-INFO
--rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 02:35:29.000000 api_hunter_cli-0.1.4/README.md
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 22:56:29.986945 api_hunter_cli-0.1.4/api_hunter_cli/
--rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 21:41:33.000000 api_hunter_cli-0.1.4/api_hunter_cli/__init__.py
--rw-rw-r--   0 charly    (1000) charly    (1000)     4239 2023-04-28 04:53:55.000000 api_hunter_cli-0.1.4/api_hunter_cli/main.py
--rw-rw-r--   0 charly    (1000) charly    (1000)      649 2023-04-28 22:53:47.000000 api_hunter_cli-0.1.4/api_hunter_cli/post_install.py
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 22:56:29.986945 api_hunter_cli-0.1.4/api_hunter_cli.egg-info/
--rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 22:56:29.000000 api_hunter_cli-0.1.4/api_hunter_cli.egg-info/PKG-INFO
--rw-rw-r--   0 charly    (1000) charly    (1000)      329 2023-04-28 22:56:29.000000 api_hunter_cli-0.1.4/api_hunter_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)        1 2023-04-28 22:56:29.000000 api_hunter_cli-0.1.4/api_hunter_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)      130 2023-04-28 22:56:29.000000 api_hunter_cli-0.1.4/api_hunter_cli.egg-info/entry_points.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 22:56:29.000000 api_hunter_cli-0.1.4/api_hunter_cli.egg-info/requires.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       15 2023-04-28 22:56:29.000000 api_hunter_cli-0.1.4/api_hunter_cli.egg-info/top_level.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 22:56:29.986945 api_hunter_cli-0.1.4/setup.cfg
--rw-rw-r--   0 charly    (1000) charly    (1000)     1412 2023-04-28 22:56:26.000000 api_hunter_cli-0.1.4/setup.py
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 23:03:43.462778 api_hunter_cli-0.1.5/
+-rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 23:03:43.462778 api_hunter_cli-0.1.5/PKG-INFO
+-rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 02:35:29.000000 api_hunter_cli-0.1.5/README.md
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 23:03:43.462778 api_hunter_cli-0.1.5/api_hunter_cli/
+-rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 21:41:33.000000 api_hunter_cli-0.1.5/api_hunter_cli/__init__.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)     4332 2023-04-28 23:03:00.000000 api_hunter_cli-0.1.5/api_hunter_cli/main.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)      649 2023-04-28 22:53:47.000000 api_hunter_cli-0.1.5/api_hunter_cli/post_install.py
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 23:03:43.462778 api_hunter_cli-0.1.5/api_hunter_cli.egg-info/
+-rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 23:03:43.000000 api_hunter_cli-0.1.5/api_hunter_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 charly    (1000) charly    (1000)      329 2023-04-28 23:03:43.000000 api_hunter_cli-0.1.5/api_hunter_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)        1 2023-04-28 23:03:43.000000 api_hunter_cli-0.1.5/api_hunter_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)      129 2023-04-28 23:03:43.000000 api_hunter_cli-0.1.5/api_hunter_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 23:03:43.000000 api_hunter_cli-0.1.5/api_hunter_cli.egg-info/requires.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       15 2023-04-28 23:03:43.000000 api_hunter_cli-0.1.5/api_hunter_cli.egg-info/top_level.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 23:03:43.462778 api_hunter_cli-0.1.5/setup.cfg
+-rw-rw-r--   0 charly    (1000) charly    (1000)     1411 2023-04-28 23:03:41.000000 api_hunter_cli-0.1.5/setup.py
```

### Comparing `api_hunter_cli-0.1.4/PKG-INFO` & `api_hunter_cli-0.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api_hunter_cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: CLI tool for finding hidden apis in a certain url.
 Home-page: https://github.com/engcarlosperezmolero/
 Author: Charly Molero
 Author-email: perez.moleroc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `api_hunter_cli-0.1.4/api_hunter_cli/main.py` & `api_hunter_cli-0.1.5/api_hunter_cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 import os
 from playwright.sync_api import sync_playwright
 from playwright._impl._api_types import Error as PlaywrightClientTypeError
 from playwright.sync_api._generated import Playwright as SyncPlaywright
 from playwright.sync_api._generated import Response as PlaywrightClientResponse
 
 
+app = typer.Typer()
+
 def return_json_response(response: PlaywrightClientResponse, errors_counters: dict, json_responses: list,
                          json_request_urls: list) -> None:
     try:
         formatted_response = {"url": response.url, "json_response": response.json()}
         json_responses.append(formatted_response)
         json_request_urls.append(response.url)
 
@@ -57,15 +59,16 @@
                 json.dump(json_responses, f)
 
             with open(f'{file_name}_urls.txt', 'w') as f:
                 f.write('\n'.join(json_request_urls))
     return json_responses, json_request_urls, errors_counters
 
 
-def main(url_to_analyze: str, verbose_response: bool = False):
+@app.command()
+def main(url_to_analyze: str, verbose_response: bool = typer.Option(False, help="Show additional error information.")):
     questions = [
         inquirer.Text('file_name', message="Write a name for the file to save the responses of hidden apis (if any)",
                       validate=lambda _, x: re.match(r'^[a-zA-Z0-9_]{1,40}$', x),
                       )
     ]
     file_information: dict = inquirer.prompt(questions)
     file_name = file_information.get('file_name')
```

### Comparing `api_hunter_cli-0.1.4/api_hunter_cli/post_install.py` & `api_hunter_cli-0.1.5/api_hunter_cli/post_install.py`

 * *Files identical despite different names*

### Comparing `api_hunter_cli-0.1.4/api_hunter_cli.egg-info/PKG-INFO` & `api_hunter_cli-0.1.5/api_hunter_cli.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-hunter-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: CLI tool for finding hidden apis in a certain url.
 Home-page: https://github.com/engcarlosperezmolero/
 Author: Charly Molero
 Author-email: perez.moleroc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `api_hunter_cli-0.1.4/setup.py` & `api_hunter_cli-0.1.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,29 +7,29 @@
     def run(self):
         install.run(self)
         self.spawn([sys.executable, "post_install.py"])
 
 
 setup(
     name="api_hunter_cli",
-    version="0.1.4",
+    version="0.1.5",
     description="CLI tool for finding hidden apis in a certain url.",
     author="Charly Molero",
     author_email="perez.moleroc@gmail.com",
     url="https://github.com/engcarlosperezmolero/",
     packages=find_packages(),
     install_requires=[
         "playwright",
         "typer[all]",
         "yaspin",
         "inquirer",
     ],
     entry_points={
         "console_scripts": [
-            "apihunter=api_hunter_cli.main:main",
+            "apihunter=api_hunter_cli.main:app",
             "api-hunter-cli-post-install=api_hunter_cli.post_install:install_chromium",
         ],
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```


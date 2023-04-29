# Comparing `tmp/api_hunter_cli-0.2.0.tar.gz` & `tmp/api_hunter_cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_hunter_cli-0.2.0.tar", last modified: Sat Apr 29 16:14:17 2023, max compression
+gzip compressed data, was "api_hunter_cli-0.2.1.tar", last modified: Sat Apr 29 16:58:11 2023, max compression
```

## Comparing `api_hunter_cli-0.2.0.tar` & `api_hunter_cli-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-29 16:14:17.987537 api_hunter_cli-0.2.0/
--rw-rw-r--   0 charly    (1000) charly    (1000)      745 2023-04-29 16:14:17.987537 api_hunter_cli-0.2.0/PKG-INFO
--rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 02:35:29.000000 api_hunter_cli-0.2.0/README.md
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-29 16:14:17.987537 api_hunter_cli-0.2.0/api_hunter_cli/
--rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 21:41:33.000000 api_hunter_cli-0.2.0/api_hunter_cli/__init__.py
--rw-rw-r--   0 charly    (1000) charly    (1000)     3486 2023-04-29 16:13:48.000000 api_hunter_cli-0.2.0/api_hunter_cli/main.py
--rw-rw-r--   0 charly    (1000) charly    (1000)     3724 2023-04-29 16:02:02.000000 api_hunter_cli-0.2.0/api_hunter_cli/playwright_custom.py
--rw-rw-r--   0 charly    (1000) charly    (1000)      649 2023-04-28 22:53:47.000000 api_hunter_cli-0.2.0/api_hunter_cli/post_install.py
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-29 16:14:17.987537 api_hunter_cli-0.2.0/api_hunter_cli.egg-info/
--rw-rw-r--   0 charly    (1000) charly    (1000)      745 2023-04-29 16:14:17.000000 api_hunter_cli-0.2.0/api_hunter_cli.egg-info/PKG-INFO
--rw-rw-r--   0 charly    (1000) charly    (1000)      365 2023-04-29 16:14:17.000000 api_hunter_cli-0.2.0/api_hunter_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)        1 2023-04-29 16:14:17.000000 api_hunter_cli-0.2.0/api_hunter_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)      129 2023-04-29 16:14:17.000000 api_hunter_cli-0.2.0/api_hunter_cli.egg-info/entry_points.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-29 16:14:17.000000 api_hunter_cli-0.2.0/api_hunter_cli.egg-info/requires.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       15 2023-04-29 16:14:17.000000 api_hunter_cli-0.2.0/api_hunter_cli.egg-info/top_level.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-29 16:14:17.987537 api_hunter_cli-0.2.0/setup.cfg
--rw-rw-r--   0 charly    (1000) charly    (1000)     1178 2023-04-29 16:14:09.000000 api_hunter_cli-0.2.0/setup.py
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-29 16:58:11.381924 api_hunter_cli-0.2.1/
+-rw-rw-r--   0 charly    (1000) charly    (1000)     1070 2023-04-29 16:47:37.000000 api_hunter_cli-0.2.1/LICENSE
+-rw-rw-r--   0 charly    (1000) charly    (1000)      767 2023-04-29 16:58:11.381924 api_hunter_cli-0.2.1/PKG-INFO
+-rw-rw-r--   0 charly    (1000) charly    (1000)     1911 2023-04-29 16:44:38.000000 api_hunter_cli-0.2.1/README.md
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-29 16:58:11.381924 api_hunter_cli-0.2.1/api_hunter_cli/
+-rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 21:41:33.000000 api_hunter_cli-0.2.1/api_hunter_cli/__init__.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)     3488 2023-04-29 16:17:13.000000 api_hunter_cli-0.2.1/api_hunter_cli/main.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)     3724 2023-04-29 16:02:02.000000 api_hunter_cli-0.2.1/api_hunter_cli/playwright_custom.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)      649 2023-04-28 22:53:47.000000 api_hunter_cli-0.2.1/api_hunter_cli/post_install.py
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-29 16:58:11.381924 api_hunter_cli-0.2.1/api_hunter_cli.egg-info/
+-rw-rw-r--   0 charly    (1000) charly    (1000)      767 2023-04-29 16:58:11.000000 api_hunter_cli-0.2.1/api_hunter_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 charly    (1000) charly    (1000)      373 2023-04-29 16:58:11.000000 api_hunter_cli-0.2.1/api_hunter_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)        1 2023-04-29 16:58:11.000000 api_hunter_cli-0.2.1/api_hunter_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)      129 2023-04-29 16:58:11.000000 api_hunter_cli-0.2.1/api_hunter_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-29 16:58:11.000000 api_hunter_cli-0.2.1/api_hunter_cli.egg-info/requires.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       15 2023-04-29 16:58:11.000000 api_hunter_cli-0.2.1/api_hunter_cli.egg-info/top_level.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-29 16:58:11.381924 api_hunter_cli-0.2.1/setup.cfg
+-rw-rw-r--   0 charly    (1000) charly    (1000)     1178 2023-04-29 16:19:30.000000 api_hunter_cli-0.2.1/setup.py
```

### Comparing `api_hunter_cli-0.2.0/api_hunter_cli/main.py` & `api_hunter_cli-0.2.1/api_hunter_cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,18 +47,18 @@
                 for error, count in errors_counters.items():
                     table.add_row(str(error), str(count))
                 console.print(Panel.fit(table, title="Additional info", title_align="left", padding=1))
 
     else:
         file_name = str(typer.prompt("Write a name for the file to save the responses of hidden apis (if any): ",
                                  default="results"))
-        rich_print(f"\nSearching for possible [yellow]hidden apis[/yellow] in [blue]{url_to_analyze}[/blue]...")
+        rich_print(f"\nSearching for possible [yellow]hidden apis[/yellow] in [blue]{url_to_analyze}[/blue] ...")
         json_responses, json_request_urls, errors_counters = main_execution(url_to_analyze, file_name)
         if json_responses:
-            rich_print(f"\nFor {url_to_analyze}, {len(json_responses)} possible hidden apis have been found."
+            rich_print(f"\nFor {url_to_analyze} , {len(json_responses)} possible hidden apis have been found."
                   f"\n\nYou can find your responses at: [green]{os.getcwd()}/{file_name}_responses.json[/green]"
                   f"\nand the requested hidden apis at: [green]{os.getcwd()}/{file_name}_urls.txt[/green]")
 
         else:
             rich_print(f"\n[bold red]No hidden apis have been found.[/bold red]")
 
         if verbose_response:
```

### Comparing `api_hunter_cli-0.2.0/api_hunter_cli/playwright_custom.py` & `api_hunter_cli-0.2.1/api_hunter_cli/playwright_custom.py`

 * *Files identical despite different names*

### Comparing `api_hunter_cli-0.2.0/api_hunter_cli/post_install.py` & `api_hunter_cli-0.2.1/api_hunter_cli/post_install.py`

 * *Files identical despite different names*

### Comparing `api_hunter_cli-0.2.0/api_hunter_cli.egg-info/PKG-INFO` & `api_hunter_cli-0.2.1/api_hunter_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-hunter-cli
-Version: 0.2.0
+Version: 0.2.1
 Summary: CLI tool for finding hidden apis in a certain url.
 Home-page: https://github.com/engcarlosperezmolero/api_hunter_cli
 Author: Charly Molero
 Author-email: perez.moleroc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,7 +12,8 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
+License-File: LICENSE
```

### Comparing `api_hunter_cli-0.2.0/setup.py` & `api_hunter_cli-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="api_hunter_cli",
-    version="0.2.0",
+    version="0.2.1",
     description="CLI tool for finding hidden apis in a certain url.",
     author="Charly Molero",
     author_email="perez.moleroc@gmail.com",
     url="https://github.com/engcarlosperezmolero/api_hunter_cli",
     packages=find_packages(),
     install_requires=[
         "playwright",
```


# Comparing `tmp/api_hunter_cli-0.1.5.tar.gz` & `tmp/api_hunter_cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_hunter_cli-0.1.5.tar", last modified: Fri Apr 28 23:03:43 2023, max compression
+gzip compressed data, was "api_hunter_cli-0.1.6.tar", last modified: Fri Apr 28 23:22:28 2023, max compression
```

## Comparing `api_hunter_cli-0.1.5.tar` & `api_hunter_cli-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 23:03:43.462778 api_hunter_cli-0.1.5/
--rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 23:03:43.462778 api_hunter_cli-0.1.5/PKG-INFO
--rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 02:35:29.000000 api_hunter_cli-0.1.5/README.md
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 23:03:43.462778 api_hunter_cli-0.1.5/api_hunter_cli/
--rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 21:41:33.000000 api_hunter_cli-0.1.5/api_hunter_cli/__init__.py
--rw-rw-r--   0 charly    (1000) charly    (1000)     4332 2023-04-28 23:03:00.000000 api_hunter_cli-0.1.5/api_hunter_cli/main.py
--rw-rw-r--   0 charly    (1000) charly    (1000)      649 2023-04-28 22:53:47.000000 api_hunter_cli-0.1.5/api_hunter_cli/post_install.py
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 23:03:43.462778 api_hunter_cli-0.1.5/api_hunter_cli.egg-info/
--rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 23:03:43.000000 api_hunter_cli-0.1.5/api_hunter_cli.egg-info/PKG-INFO
--rw-rw-r--   0 charly    (1000) charly    (1000)      329 2023-04-28 23:03:43.000000 api_hunter_cli-0.1.5/api_hunter_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)        1 2023-04-28 23:03:43.000000 api_hunter_cli-0.1.5/api_hunter_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)      129 2023-04-28 23:03:43.000000 api_hunter_cli-0.1.5/api_hunter_cli.egg-info/entry_points.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 23:03:43.000000 api_hunter_cli-0.1.5/api_hunter_cli.egg-info/requires.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       15 2023-04-28 23:03:43.000000 api_hunter_cli-0.1.5/api_hunter_cli.egg-info/top_level.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 23:03:43.462778 api_hunter_cli-0.1.5/setup.cfg
--rw-rw-r--   0 charly    (1000) charly    (1000)     1411 2023-04-28 23:03:41.000000 api_hunter_cli-0.1.5/setup.py
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 23:22:28.276446 api_hunter_cli-0.1.6/
+-rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 23:22:28.276446 api_hunter_cli-0.1.6/PKG-INFO
+-rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 02:35:29.000000 api_hunter_cli-0.1.6/README.md
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 23:22:28.276446 api_hunter_cli-0.1.6/api_hunter_cli/
+-rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 21:41:33.000000 api_hunter_cli-0.1.6/api_hunter_cli/__init__.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)     5427 2023-04-28 23:22:25.000000 api_hunter_cli-0.1.6/api_hunter_cli/main.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)      649 2023-04-28 22:53:47.000000 api_hunter_cli-0.1.6/api_hunter_cli/post_install.py
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 23:22:28.276446 api_hunter_cli-0.1.6/api_hunter_cli.egg-info/
+-rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 23:22:28.000000 api_hunter_cli-0.1.6/api_hunter_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 charly    (1000) charly    (1000)      329 2023-04-28 23:22:28.000000 api_hunter_cli-0.1.6/api_hunter_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)        1 2023-04-28 23:22:28.000000 api_hunter_cli-0.1.6/api_hunter_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)      129 2023-04-28 23:22:28.000000 api_hunter_cli-0.1.6/api_hunter_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 23:22:28.000000 api_hunter_cli-0.1.6/api_hunter_cli.egg-info/requires.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       15 2023-04-28 23:22:28.000000 api_hunter_cli-0.1.6/api_hunter_cli.egg-info/top_level.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 23:22:28.276446 api_hunter_cli-0.1.6/setup.cfg
+-rw-rw-r--   0 charly    (1000) charly    (1000)     1411 2023-04-28 23:22:25.000000 api_hunter_cli-0.1.6/setup.py
```

### Comparing `api_hunter_cli-0.1.5/PKG-INFO` & `api_hunter_cli-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api_hunter_cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: CLI tool for finding hidden apis in a certain url.
 Home-page: https://github.com/engcarlosperezmolero/
 Author: Charly Molero
 Author-email: perez.moleroc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `api_hunter_cli-0.1.5/api_hunter_cli/main.py` & `api_hunter_cli-0.1.6/api_hunter_cli/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import typer
-from rich import print
+from rich import print as rich_print
 from rich.console import Console
 from rich.table import Table
 from rich.panel import Panel
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 import inquirer
 import json
@@ -60,42 +60,60 @@
 
             with open(f'{file_name}_urls.txt', 'w') as f:
                 f.write('\n'.join(json_request_urls))
     return json_responses, json_request_urls, errors_counters
 
 
 @app.command()
-def main(url_to_analyze: str, verbose_response: bool = typer.Option(False, help="Show additional error information.")):
-    questions = [
-        inquirer.Text('file_name', message="Write a name for the file to save the responses of hidden apis (if any)",
-                      validate=lambda _, x: re.match(r'^[a-zA-Z0-9_]{1,40}$', x),
-                      )
-    ]
-    file_information: dict = inquirer.prompt(questions)
-    file_name = file_information.get('file_name')
-
-    with yaspin(spinner=Spinners.bouncingBar, text=f"Searching for possible hidden apis in {url_to_analyze}...",
-                color="yellow") as spinner:
+def main(url_to_analyze: str, verbose_response: bool = typer.Option(False, help="Show additional error information."),
+         style: bool = typer.Option(True, help="Prints results without styling (Good for running in notebooks with !)")):
+    if style:
+        questions = [
+            inquirer.Text('file_name', message="Write a name for the file to save the responses of hidden apis (if any)",
+                          validate=lambda _, x: re.match(r'^[a-zA-Z0-9_]{1,40}$', x),
+                          )
+        ]
+        file_information: dict = inquirer.prompt(questions)
+        file_name = file_information.get('file_name')
+
+        with yaspin(spinner=Spinners.bouncingBar, text=f"Searching for possible hidden apis in {url_to_analyze}...",
+                    color="yellow") as spinner:
+            json_responses, json_request_urls, errors_counters = main_execution(url_to_analyze, file_name)
+            rich_print("\n")
+            if json_responses:
+                rich_print(Panel.fit(f"For [link={url_to_analyze}]{url_to_analyze}[/link],"
+                                f" [bold green]{len(json_responses)}[/bold green] possible hidden apis have been found."
+                              f"\n\nYou can find your responses at:   [green]{os.getcwd()}/{file_name}_responses.json[/green]"
+                                f"\nand the requested hidden apis at: [green]{os.getcwd()}/{file_name}_urls.txt[/green]",
+                                title="Results", title_align="left", padding=1))
+            else:
+                rich_print(Panel.fit(f"[bold red]No hidden apis have been found.[/bold red]",
+                                title="Result", title_align="left", padding=1))
+
+            if verbose_response:
+                rich_print("\n")
+                console = Console()
+                table = Table("Error", "Count")
+                for error, count in errors_counters.items():
+                    table.add_row(str(error), str(count))
+                console.print(Panel.fit(table, title="Additional info", title_align="left", padding=1))
+
+    else:
+        file_name = input("Write a name for the file to save the responses of hidden apis (if any): ")
+        print(f"\nSearching for possible hidden apis in {url_to_analyze}...")
         json_responses, json_request_urls, errors_counters = main_execution(url_to_analyze, file_name)
-        print("\n")
         if json_responses:
-            print(Panel.fit(f"For [link={url_to_analyze}]{url_to_analyze}[/link],"
-                            f" [bold green]{len(json_responses)}[/bold green] possible hidden apis have been found."
-                          f"\n\nYou can find your responses at:   [green]{os.getcwd()}/{file_name}_responses.json[/green]"
-                            f"\nand the requested hidden apis at: [green]{os.getcwd()}/{file_name}_urls.txt[/green]",
-                            title="Results", title_align="left", padding=1))
+            print(f"For {url_to_analyze}, {len(json_responses)} possible hidden apis have been found."
+                  f"\n\nYou can find your responses at: {os.getcwd()}/{file_name}_responses.json"
+                  f"\nand the requested hidden apis at: {os.getcwd()}/{file_name}_urls.txt")
+
         else:
-            print(Panel.fit(f"[bold red]No hidden apis have been found.[/bold red]",
-                            title="Result", title_align="left", padding=1))
-            return 1
+            print(f"No hidden apis have been found.")
 
         if verbose_response:
             print("\n")
-            console = Console()
-            table = Table("Error", "Count")
             for error, count in errors_counters.items():
-                table.add_row(str(error), str(count))
-            console.print(Panel.fit(table, title="Additional info", title_align="left", padding=1))
+                print(f"{error}: {count}")
 
 
 if __name__ == "__main__":
     typer.run(main)
```

### Comparing `api_hunter_cli-0.1.5/api_hunter_cli/post_install.py` & `api_hunter_cli-0.1.6/api_hunter_cli/post_install.py`

 * *Files identical despite different names*

### Comparing `api_hunter_cli-0.1.5/api_hunter_cli.egg-info/PKG-INFO` & `api_hunter_cli-0.1.6/api_hunter_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-hunter-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: CLI tool for finding hidden apis in a certain url.
 Home-page: https://github.com/engcarlosperezmolero/
 Author: Charly Molero
 Author-email: perez.moleroc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `api_hunter_cli-0.1.5/setup.py` & `api_hunter_cli-0.1.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def run(self):
         install.run(self)
         self.spawn([sys.executable, "post_install.py"])
 
 
 setup(
     name="api_hunter_cli",
-    version="0.1.5",
+    version="0.1.6",
     description="CLI tool for finding hidden apis in a certain url.",
     author="Charly Molero",
     author_email="perez.moleroc@gmail.com",
     url="https://github.com/engcarlosperezmolero/",
     packages=find_packages(),
     install_requires=[
         "playwright",
```


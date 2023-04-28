# Comparing `tmp/api_hunter_cli-0.1.6.tar.gz` & `tmp/api_hunter_cli-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_hunter_cli-0.1.6.tar", last modified: Fri Apr 28 23:22:28 2023, max compression
+gzip compressed data, was "api_hunter_cli-0.1.7.tar", last modified: Fri Apr 28 23:29:16 2023, max compression
```

## Comparing `api_hunter_cli-0.1.6.tar` & `api_hunter_cli-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 23:22:28.276446 api_hunter_cli-0.1.6/
--rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 23:22:28.276446 api_hunter_cli-0.1.6/PKG-INFO
--rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 02:35:29.000000 api_hunter_cli-0.1.6/README.md
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 23:22:28.276446 api_hunter_cli-0.1.6/api_hunter_cli/
--rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 21:41:33.000000 api_hunter_cli-0.1.6/api_hunter_cli/__init__.py
--rw-rw-r--   0 charly    (1000) charly    (1000)     5427 2023-04-28 23:22:25.000000 api_hunter_cli-0.1.6/api_hunter_cli/main.py
--rw-rw-r--   0 charly    (1000) charly    (1000)      649 2023-04-28 22:53:47.000000 api_hunter_cli-0.1.6/api_hunter_cli/post_install.py
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 23:22:28.276446 api_hunter_cli-0.1.6/api_hunter_cli.egg-info/
--rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 23:22:28.000000 api_hunter_cli-0.1.6/api_hunter_cli.egg-info/PKG-INFO
--rw-rw-r--   0 charly    (1000) charly    (1000)      329 2023-04-28 23:22:28.000000 api_hunter_cli-0.1.6/api_hunter_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)        1 2023-04-28 23:22:28.000000 api_hunter_cli-0.1.6/api_hunter_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)      129 2023-04-28 23:22:28.000000 api_hunter_cli-0.1.6/api_hunter_cli.egg-info/entry_points.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 23:22:28.000000 api_hunter_cli-0.1.6/api_hunter_cli.egg-info/requires.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       15 2023-04-28 23:22:28.000000 api_hunter_cli-0.1.6/api_hunter_cli.egg-info/top_level.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 23:22:28.276446 api_hunter_cli-0.1.6/setup.cfg
--rw-rw-r--   0 charly    (1000) charly    (1000)     1411 2023-04-28 23:22:25.000000 api_hunter_cli-0.1.6/setup.py
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 23:29:16.526376 api_hunter_cli-0.1.7/
+-rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 23:29:16.526376 api_hunter_cli-0.1.7/PKG-INFO
+-rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 02:35:29.000000 api_hunter_cli-0.1.7/README.md
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 23:29:16.526376 api_hunter_cli-0.1.7/api_hunter_cli/
+-rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 21:41:33.000000 api_hunter_cli-0.1.7/api_hunter_cli/__init__.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)     5495 2023-04-28 23:29:09.000000 api_hunter_cli-0.1.7/api_hunter_cli/main.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)      649 2023-04-28 22:53:47.000000 api_hunter_cli-0.1.7/api_hunter_cli/post_install.py
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-28 23:29:16.526376 api_hunter_cli-0.1.7/api_hunter_cli.egg-info/
+-rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-28 23:29:16.000000 api_hunter_cli-0.1.7/api_hunter_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 charly    (1000) charly    (1000)      329 2023-04-28 23:29:16.000000 api_hunter_cli-0.1.7/api_hunter_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)        1 2023-04-28 23:29:16.000000 api_hunter_cli-0.1.7/api_hunter_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)      129 2023-04-28 23:29:16.000000 api_hunter_cli-0.1.7/api_hunter_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 23:29:16.000000 api_hunter_cli-0.1.7/api_hunter_cli.egg-info/requires.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       15 2023-04-28 23:29:16.000000 api_hunter_cli-0.1.7/api_hunter_cli.egg-info/top_level.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-28 23:29:16.530376 api_hunter_cli-0.1.7/setup.cfg
+-rw-rw-r--   0 charly    (1000) charly    (1000)     1411 2023-04-28 23:29:09.000000 api_hunter_cli-0.1.7/setup.py
```

### Comparing `api_hunter_cli-0.1.6/PKG-INFO` & `api_hunter_cli-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api_hunter_cli
-Version: 0.1.6
+Version: 0.1.7
 Summary: CLI tool for finding hidden apis in a certain url.
 Home-page: https://github.com/engcarlosperezmolero/
 Author: Charly Molero
 Author-email: perez.moleroc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `api_hunter_cli-0.1.6/api_hunter_cli/main.py` & `api_hunter_cli-0.1.7/api_hunter_cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,24 +94,25 @@
                 console = Console()
                 table = Table("Error", "Count")
                 for error, count in errors_counters.items():
                     table.add_row(str(error), str(count))
                 console.print(Panel.fit(table, title="Additional info", title_align="left", padding=1))
 
     else:
-        file_name = input("Write a name for the file to save the responses of hidden apis (if any): ")
+        file_name = str(typer.prompt("Write a name for the file to save the responses of hidden apis (if any): ",
+                                 default="results"))
         print(f"\nSearching for possible hidden apis in {url_to_analyze}...")
         json_responses, json_request_urls, errors_counters = main_execution(url_to_analyze, file_name)
         if json_responses:
-            print(f"For {url_to_analyze}, {len(json_responses)} possible hidden apis have been found."
+            print(f"\nFor {url_to_analyze}, {len(json_responses)} possible hidden apis have been found."
                   f"\n\nYou can find your responses at: {os.getcwd()}/{file_name}_responses.json"
                   f"\nand the requested hidden apis at: {os.getcwd()}/{file_name}_urls.txt")
 
         else:
-            print(f"No hidden apis have been found.")
+            print(f"\nNo hidden apis have been found.")
 
         if verbose_response:
             print("\n")
             for error, count in errors_counters.items():
                 print(f"{error}: {count}")
```

### Comparing `api_hunter_cli-0.1.6/api_hunter_cli/post_install.py` & `api_hunter_cli-0.1.7/api_hunter_cli/post_install.py`

 * *Files identical despite different names*

### Comparing `api_hunter_cli-0.1.6/api_hunter_cli.egg-info/PKG-INFO` & `api_hunter_cli-0.1.7/api_hunter_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-hunter-cli
-Version: 0.1.6
+Version: 0.1.7
 Summary: CLI tool for finding hidden apis in a certain url.
 Home-page: https://github.com/engcarlosperezmolero/
 Author: Charly Molero
 Author-email: perez.moleroc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `api_hunter_cli-0.1.6/setup.py` & `api_hunter_cli-0.1.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def run(self):
         install.run(self)
         self.spawn([sys.executable, "post_install.py"])
 
 
 setup(
     name="api_hunter_cli",
-    version="0.1.6",
+    version="0.1.7",
     description="CLI tool for finding hidden apis in a certain url.",
     author="Charly Molero",
     author_email="perez.moleroc@gmail.com",
     url="https://github.com/engcarlosperezmolero/",
     packages=find_packages(),
     install_requires=[
         "playwright",
```


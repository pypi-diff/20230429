# Comparing `tmp/api_hunter_cli-0.1.8.tar.gz` & `tmp/api_hunter_cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_hunter_cli-0.1.8.tar", last modified: Sat Apr 29 16:03:28 2023, max compression
+gzip compressed data, was "api_hunter_cli-0.1.9.tar", last modified: Sat Apr 29 16:09:44 2023, max compression
```

## Comparing `api_hunter_cli-0.1.8.tar` & `api_hunter_cli-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-29 16:03:28.163875 api_hunter_cli-0.1.8/
--rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-29 16:03:28.163875 api_hunter_cli-0.1.8/PKG-INFO
--rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 02:35:29.000000 api_hunter_cli-0.1.8/README.md
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-29 16:03:28.163875 api_hunter_cli-0.1.8/api_hunter_cli/
--rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 21:41:33.000000 api_hunter_cli-0.1.8/api_hunter_cli/__init__.py
--rw-rw-r--   0 charly    (1000) charly    (1000)     3472 2023-04-29 16:02:23.000000 api_hunter_cli-0.1.8/api_hunter_cli/main.py
--rw-rw-r--   0 charly    (1000) charly    (1000)     3724 2023-04-29 16:02:02.000000 api_hunter_cli-0.1.8/api_hunter_cli/playwright_custom.py
--rw-rw-r--   0 charly    (1000) charly    (1000)      649 2023-04-28 22:53:47.000000 api_hunter_cli-0.1.8/api_hunter_cli/post_install.py
-drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-29 16:03:28.163875 api_hunter_cli-0.1.8/api_hunter_cli.egg-info/
--rw-rw-r--   0 charly    (1000) charly    (1000)      731 2023-04-29 16:03:28.000000 api_hunter_cli-0.1.8/api_hunter_cli.egg-info/PKG-INFO
--rw-rw-r--   0 charly    (1000) charly    (1000)      365 2023-04-29 16:03:28.000000 api_hunter_cli-0.1.8/api_hunter_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)        1 2023-04-29 16:03:28.000000 api_hunter_cli-0.1.8/api_hunter_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)      129 2023-04-29 16:03:28.000000 api_hunter_cli-0.1.8/api_hunter_cli.egg-info/entry_points.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-29 16:03:28.000000 api_hunter_cli-0.1.8/api_hunter_cli.egg-info/requires.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       15 2023-04-29 16:03:28.000000 api_hunter_cli-0.1.8/api_hunter_cli.egg-info/top_level.txt
--rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-29 16:03:28.163875 api_hunter_cli-0.1.8/setup.cfg
--rw-rw-r--   0 charly    (1000) charly    (1000)     1411 2023-04-29 16:03:09.000000 api_hunter_cli-0.1.8/setup.py
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-29 16:09:44.267587 api_hunter_cli-0.1.9/
+-rw-rw-r--   0 charly    (1000) charly    (1000)      745 2023-04-29 16:09:44.267587 api_hunter_cli-0.1.9/PKG-INFO
+-rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 02:35:29.000000 api_hunter_cli-0.1.9/README.md
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-29 16:09:44.267587 api_hunter_cli-0.1.9/api_hunter_cli/
+-rw-rw-r--   0 charly    (1000) charly    (1000)        0 2023-04-28 21:41:33.000000 api_hunter_cli-0.1.9/api_hunter_cli/__init__.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)     3487 2023-04-29 16:09:00.000000 api_hunter_cli-0.1.9/api_hunter_cli/main.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)     3724 2023-04-29 16:02:02.000000 api_hunter_cli-0.1.9/api_hunter_cli/playwright_custom.py
+-rw-rw-r--   0 charly    (1000) charly    (1000)      649 2023-04-28 22:53:47.000000 api_hunter_cli-0.1.9/api_hunter_cli/post_install.py
+drwxrwxr-x   0 charly    (1000) charly    (1000)        0 2023-04-29 16:09:44.267587 api_hunter_cli-0.1.9/api_hunter_cli.egg-info/
+-rw-rw-r--   0 charly    (1000) charly    (1000)      745 2023-04-29 16:09:44.000000 api_hunter_cli-0.1.9/api_hunter_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 charly    (1000) charly    (1000)      365 2023-04-29 16:09:44.000000 api_hunter_cli-0.1.9/api_hunter_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)        1 2023-04-29 16:09:44.000000 api_hunter_cli-0.1.9/api_hunter_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)      129 2023-04-29 16:09:44.000000 api_hunter_cli-0.1.9/api_hunter_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-29 16:09:44.000000 api_hunter_cli-0.1.9/api_hunter_cli.egg-info/requires.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       15 2023-04-29 16:09:44.000000 api_hunter_cli-0.1.9/api_hunter_cli.egg-info/top_level.txt
+-rw-rw-r--   0 charly    (1000) charly    (1000)       38 2023-04-29 16:09:44.267587 api_hunter_cli-0.1.9/setup.cfg
+-rw-rw-r--   0 charly    (1000) charly    (1000)     1178 2023-04-29 16:09:41.000000 api_hunter_cli-0.1.9/setup.py
```

### Comparing `api_hunter_cli-0.1.8/PKG-INFO` & `api_hunter_cli-0.1.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: api_hunter_cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: CLI tool for finding hidden apis in a certain url.
-Home-page: https://github.com/engcarlosperezmolero/
+Home-page: https://github.com/engcarlosperezmolero/api_hunter_cli
 Author: Charly Molero
 Author-email: perez.moleroc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `api_hunter_cli-0.1.8/api_hunter_cli/main.py` & `api_hunter_cli-0.1.9/api_hunter_cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from rich.table import Table
 from rich.panel import Panel
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 import inquirer
 import re
 import os
-from playwright_custom import main_execution
+from api_hunter_cli.playwright_custom import main_execution
 
 
 app = typer.Typer()
 
 
 @app.command()
 def main(url_to_analyze: str, verbose_response: bool = typer.Option(False, help="Show additional error information."),
```

### Comparing `api_hunter_cli-0.1.8/api_hunter_cli/playwright_custom.py` & `api_hunter_cli-0.1.9/api_hunter_cli/playwright_custom.py`

 * *Files identical despite different names*

### Comparing `api_hunter_cli-0.1.8/api_hunter_cli/post_install.py` & `api_hunter_cli-0.1.9/api_hunter_cli/post_install.py`

 * *Files identical despite different names*

### Comparing `api_hunter_cli-0.1.8/api_hunter_cli.egg-info/PKG-INFO` & `api_hunter_cli-0.1.9/api_hunter_cli.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: api-hunter-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: CLI tool for finding hidden apis in a certain url.
-Home-page: https://github.com/engcarlosperezmolero/
+Home-page: https://github.com/engcarlosperezmolero/api_hunter_cli
 Author: Charly Molero
 Author-email: perez.moleroc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `api_hunter_cli-0.1.8/setup.py` & `api_hunter_cli-0.1.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,17 @@
 from setuptools import setup, find_packages
-from setuptools.command.install import install
-import sys
-
-
-class PostInstallCommand(install):
-    def run(self):
-        install.run(self)
-        self.spawn([sys.executable, "post_install.py"])
 
 
 setup(
     name="api_hunter_cli",
-    version="0.1.8",
+    version="0.1.9",
     description="CLI tool for finding hidden apis in a certain url.",
     author="Charly Molero",
     author_email="perez.moleroc@gmail.com",
-    url="https://github.com/engcarlosperezmolero/",
+    url="https://github.com/engcarlosperezmolero/api_hunter_cli",
     packages=find_packages(),
     install_requires=[
         "playwright",
         "typer[all]",
         "yaspin",
         "inquirer",
     ],
@@ -38,9 +30,8 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     python_requires=">=3.7",
-    cmdclass={"post_install": PostInstallCommand},
 )
```


# Comparing `tmp/flet-web-template-0.1.0.tar.gz` & `tmp/flet-web-template-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet-web-template-0.1.0.tar", last modified: Sat Apr 29 15:32:34 2023, max compression
+gzip compressed data, was "flet-web-template-0.1.1.tar", last modified: Sat Apr 29 15:49:02 2023, max compression
```

## Comparing `flet-web-template-0.1.0.tar` & `flet-web-template-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 15:32:34.473455 flet-web-template-0.1.0/
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 flet-web-template-0.1.0/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      531 2023-04-29 15:32:34.473253 flet-web-template-0.1.0/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-26 21:15:23.000000 flet-web-template-0.1.0/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 15:32:34.468988 flet-web-template-0.1.0/command/
--rw-r--r--   0 ahmad      (501) staff       (20)     9184 2023-04-29 15:21:59.000000 flet-web-template-0.1.0/command/cli.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 15:32:34.470795 flet-web-template-0.1.0/flet_template/
--rw-r--r--   0 ahmad      (501) staff       (20)      178 2023-04-29 14:22:03.000000 flet-web-template-0.1.0/flet_template/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2587 2023-04-29 14:05:59.000000 flet-web-template-0.1.0/flet_template/base.py
--rw-r--r--   0 ahmad      (501) staff       (20)      441 2023-04-29 14:18:26.000000 flet-web-template-0.1.0/flet_template/main.py
--rw-r--r--   0 ahmad      (501) staff       (20)      162 2023-04-29 14:06:34.000000 flet-web-template-0.1.0/flet_template/route_base.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3662 2023-04-29 14:04:15.000000 flet-web-template-0.1.0/flet_template/script.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 15:32:34.472761 flet-web-template-0.1.0/flet_web_template.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      531 2023-04-29 15:32:34.000000 flet-web-template-0.1.0/flet_web_template.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      424 2023-04-29 15:32:34.000000 flet-web-template-0.1.0/flet_web_template.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-04-29 15:32:34.000000 flet-web-template-0.1.0/flet_web_template.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       71 2023-04-29 15:32:34.000000 flet-web-template-0.1.0/flet_web_template.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       25 2023-04-29 15:32:34.000000 flet-web-template-0.1.0/flet_web_template.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       22 2023-04-29 15:32:34.000000 flet-web-template-0.1.0/flet_web_template.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-04-29 15:32:34.473512 flet-web-template-0.1.0/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)      792 2023-04-29 15:30:30.000000 flet-web-template-0.1.0/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 15:32:34.472986 flet-web-template-0.1.0/test/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-27 13:33:55.000000 flet-web-template-0.1.0/test/test.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 15:49:02.962995 flet-web-template-0.1.1/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 flet-web-template-0.1.1/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      531 2023-04-29 15:49:02.962806 flet-web-template-0.1.1/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-26 21:15:23.000000 flet-web-template-0.1.1/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 15:49:02.959883 flet-web-template-0.1.1/command/
+-rw-r--r--   0 ahmad      (501) staff       (20)     9226 2023-04-29 15:48:41.000000 flet-web-template-0.1.1/command/cli.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 15:49:02.960725 flet-web-template-0.1.1/flet_template/
+-rw-r--r--   0 ahmad      (501) staff       (20)      178 2023-04-29 14:22:03.000000 flet-web-template-0.1.1/flet_template/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2587 2023-04-29 14:05:59.000000 flet-web-template-0.1.1/flet_template/base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      441 2023-04-29 14:18:26.000000 flet-web-template-0.1.1/flet_template/main.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      162 2023-04-29 14:06:34.000000 flet-web-template-0.1.1/flet_template/route_base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3662 2023-04-29 14:04:15.000000 flet-web-template-0.1.1/flet_template/script.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 15:49:02.962222 flet-web-template-0.1.1/flet_web_template.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      531 2023-04-29 15:49:02.000000 flet-web-template-0.1.1/flet_web_template.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      424 2023-04-29 15:49:02.000000 flet-web-template-0.1.1/flet_web_template.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-04-29 15:49:02.000000 flet-web-template-0.1.1/flet_web_template.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       71 2023-04-29 15:49:02.000000 flet-web-template-0.1.1/flet_web_template.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       41 2023-04-29 15:49:02.000000 flet-web-template-0.1.1/flet_web_template.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       22 2023-04-29 15:49:02.000000 flet-web-template-0.1.1/flet_web_template.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-04-29 15:49:02.963053 flet-web-template-0.1.1/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)      812 2023-04-29 15:48:47.000000 flet-web-template-0.1.1/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-29 15:49:02.962562 flet-web-template-0.1.1/test/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-27 13:33:55.000000 flet-web-template-0.1.1/test/test.py
```

### Comparing `flet-web-template-0.1.0/LICENSE` & `flet-web-template-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flet-web-template-0.1.0/PKG-INFO` & `flet-web-template-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-web-template
-Version: 0.1.0
+Version: 0.1.1
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/flet_boilerplate
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 License: UNKNOWN
 Keywords: python web templates,web application,development
 Platform: UNKNOWN
```

### Comparing `flet-web-template-0.1.0/command/cli.py` & `flet-web-template-0.1.1/command/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
 import os
 
 
-main_thread = """import flet as ft
-from script import run_template_script
+main_thread = """'''import flet as ft
+from script import run_template_script'''
 
 
 def main(page: ft.Page):
     returned_modules, theme_template = run_template_script()
     page.padding = 10
     page.bgcolor = theme_template["bgcolor"]
 
@@ -104,16 +104,16 @@
     e.page.views.clear()
 %s '''
     
 """
 
 script_thread = """import os, importlib.util
 import yaml
-from base import base_page
-from route_base import route_page
+'''from base import base_page'''
+'''from route_base import route_page'''
 import flet as ft
 import pickle5 as pickle
 
 
 class RouteButton(ft.ElevatedButton):
     def __str__(self, route):
         return f"ft.Text(size=14, weight='bold', spans=[ft.TextSpan('{route}', on_click=lambda e: router(e, '/{route}'))])"
@@ -248,18 +248,18 @@
     for file_name in file_list:
         file_path = os.path.join("templates", file_name)
         open(file_path, "a").close()
 
         # If it's the __init__.py file, write the import statements
         if file_name == "__init__.py":
             with open(file_path, "w") as f:
-                f.write("from templates.base import base_page\n")
-                f.write("from templates.main import main\n")
-                f.write("from templates.script import run_template_script\n")
-                f.write("from templates.route_base import route_page\n")
+                f.write("'''from templates.base import base_page'''\n")
+                f.write("'''from templates.main import main'''\n")
+                f.write("'''from templates.script import run_template_script'''\n")
+                f.write("'''from templates.route_base import route_page'''\n")
 
         # If it's the main.py file, write the main statements
         if file_name == "main.py":
             with open(file_path, "w") as f:
                 f.write(main_thread)
 
         # If it's the base.py file, write the main statements
```

### Comparing `flet-web-template-0.1.0/flet_template/base.py` & `flet-web-template-0.1.1/flet_template/base.py`

 * *Files identical despite different names*

### Comparing `flet-web-template-0.1.0/flet_template/script.py` & `flet-web-template-0.1.1/flet_template/script.py`

 * *Files identical despite different names*

### Comparing `flet-web-template-0.1.0/flet_web_template.egg-info/PKG-INFO` & `flet-web-template-0.1.1/flet_web_template.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-web-template
-Version: 0.1.0
+Version: 0.1.1
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/flet_boilerplate
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 License: UNKNOWN
 Keywords: python web templates,web application,development
 Platform: UNKNOWN
```

### Comparing `flet-web-template-0.1.0/setup.py` & `flet-web-template-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 setup(
     name="flet-web-template",
-    version="0.1.0",
+    version="0.1.1",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Flet Library",
     long_description="",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/flet_boilerplate",
     packages=["flet_template", "command"],
-    install_requires=["click==8.1.3", "flet==0.5.2"],
+    install_requires=["click==8.1.3", "flet==0.5.2", " pickle5==0.0.12"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": ["flet_material_init=flet_template.command.cli:init"],
```


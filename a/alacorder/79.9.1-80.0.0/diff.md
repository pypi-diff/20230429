# Comparing `tmp/alacorder-79.9.1.tar.gz` & `tmp/alacorder-80.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-79.9.1.tar", max compression
+gzip compressed data, was "alacorder-80.0.0.tar", max compression
```

## Comparing `alacorder-79.9.1.tar` & `alacorder-80.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.9.1/LICENSE
--rw-r--r--   0        0        0     6664 2023-04-28 23:25:48.704872 alacorder-79.9.1/README.md
--rw-r--r--   0        0        0      697 2023-04-28 23:25:58.581585 alacorder-79.9.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-04-28 21:53:41.054817 alacorder-79.9.1/src/alacorder/.DS_Store
--rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-79.9.1/src/alacorder/__init__.py
--rw-r--r--   0        0        0   190643 2023-04-28 23:29:52.946345 alacorder-79.9.1/src/alacorder/__main__.py
--rw-r--r--   0        0        0   190643 2023-04-28 23:29:40.604436 alacorder-79.9.1/src/alacorder/alac.py
--rw-r--r--   0        0        0     7593 1970-01-01 00:00:00.000000 alacorder-79.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.0.0/LICENSE
+-rw-r--r--   0        0        0     6664 2023-04-28 23:25:48.704872 alacorder-80.0.0/README.md
+-rw-r--r--   0        0        0      697 2023-04-29 00:42:05.913149 alacorder-80.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-04-28 21:53:41.054817 alacorder-80.0.0/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-80.0.0/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   190596 2023-04-29 00:41:32.764564 alacorder-80.0.0/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   190596 2023-04-29 00:41:28.483775 alacorder-80.0.0/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7593 1970-01-01 00:00:00.000000 alacorder-80.0.0/PKG-INFO
```

### Comparing `alacorder-79.9.1/LICENSE` & `alacorder-80.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-79.9.1/README.md` & `alacorder-80.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-79.9.1/pyproject.toml` & `alacorder-80.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "79.9.1"
+version = "80.0.0"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-79.9.1/src/alacorder/.DS_Store` & `alacorder-80.0.0/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-79.9.1/src/alacorder/__init__.py` & `alacorder-80.0.0/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-79.9.1/src/alacorder/__main__.py` & `alacorder-80.0.0/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
  Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
  
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "79.9.1"
+version = "80.0.0"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3544,15 +3544,15 @@
                 bind_return_key=True,
             )
         ],
     ]  # "TB"
     about_layout = [
         [
             sg.Text(
-                f""" ┌─┐┌─┐┬─┐┌┬┐┬ ┬┌┬┐┌─┐┬ ┬┌┐┌┌┬┐┌─┐┬┌┐┌\n ├─┘├─┤├┬┘ │ └┬┘││││ ││ ││││ │ ├─┤││││\n ┴  ┴ ┴┴└─ ┴  ┴ ┴ ┴└─┘└─┘┘└┘ ┴ ┴ ┴┴┘└┘\n {version}""",
+                f"""╔═╗╔╗╔╔═╗╦ ╦╔═╗╔═╗╦  ╔═╗╔═╗╔═╗\n╚═╗║║║║ ║║║║╠═╝╠═╣║  ╠═╣║  ║╣ \n╚═╝╝╚╝╚═╝╚╩╝╩  ╩ ╩╩═╝╩ ╩╚═╝╚═╝\nversion {version}""",
                 font=ASCII_FONT,
                 pad=(5, 5),
             )
         ],
         [
             sg.Text(
                 "Alacorder retrieves and processes\nAlacourt case detail PDFs into\ndata tables and archives.",
```

### Comparing `alacorder-79.9.1/src/alacorder/alac.py` & `alacorder-80.0.0/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
  Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
  
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "79.9.1"
+version = "80.0.0"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3544,15 +3544,15 @@
                 bind_return_key=True,
             )
         ],
     ]  # "TB"
     about_layout = [
         [
             sg.Text(
-                f""" ┌─┐┌─┐┬─┐┌┬┐┬ ┬┌┬┐┌─┐┬ ┬┌┐┌┌┬┐┌─┐┬┌┐┌\n ├─┘├─┤├┬┘ │ └┬┘││││ ││ ││││ │ ├─┤││││\n ┴  ┴ ┴┴└─ ┴  ┴ ┴ ┴└─┘└─┘┘└┘ ┴ ┴ ┴┴┘└┘\n {version}""",
+                f"""╔═╗╔╗╔╔═╗╦ ╦╔═╗╔═╗╦  ╔═╗╔═╗╔═╗\n╚═╗║║║║ ║║║║╠═╝╠═╣║  ╠═╣║  ║╣ \n╚═╝╝╚╝╚═╝╚╩╝╩  ╩ ╩╩═╝╩ ╩╚═╝╚═╝\nversion {version}""",
                 font=ASCII_FONT,
                 pad=(5, 5),
             )
         ],
         [
             sg.Text(
                 "Alacorder retrieves and processes\nAlacourt case detail PDFs into\ndata tables and archives.",
```

### Comparing `alacorder-79.9.1/PKG-INFO` & `alacorder-80.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 79.9.1
+Version: 80.0.0
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


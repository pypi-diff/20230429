# Comparing `tmp/alacorder-79.9.0.tar.gz` & `tmp/alacorder-79.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-79.9.0.tar", max compression
+gzip compressed data, was "alacorder-79.9.1.tar", max compression
```

## Comparing `alacorder-79.9.0.tar` & `alacorder-79.9.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.9.0/LICENSE
--rw-r--r--   0        0        0     9801 2023-04-27 23:24:11.886024 alacorder-79.9.0/README.md
--rw-r--r--   0        0        0      697 2023-04-28 21:55:02.900566 alacorder-79.9.0/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-04-28 21:53:41.054817 alacorder-79.9.0/src/alacorder/.DS_Store
--rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-79.9.0/src/alacorder/__init__.py
--rw-r--r--   0        0        0   190051 2023-04-28 21:52:54.246441 alacorder-79.9.0/src/alacorder/__main__.py
--rw-r--r--   0        0        0   190051 2023-04-28 21:52:41.293491 alacorder-79.9.0/src/alacorder/alac.py
--rw-r--r--   0        0        0    10730 1970-01-01 00:00:00.000000 alacorder-79.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.9.1/LICENSE
+-rw-r--r--   0        0        0     6664 2023-04-28 23:25:48.704872 alacorder-79.9.1/README.md
+-rw-r--r--   0        0        0      697 2023-04-28 23:25:58.581585 alacorder-79.9.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-04-28 21:53:41.054817 alacorder-79.9.1/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-79.9.1/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   190643 2023-04-28 23:29:52.946345 alacorder-79.9.1/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   190643 2023-04-28 23:29:40.604436 alacorder-79.9.1/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7593 1970-01-01 00:00:00.000000 alacorder-79.9.1/PKG-INFO
```

### Comparing `alacorder-79.9.0/LICENSE` & `alacorder-79.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-79.9.0/pyproject.toml` & `alacorder-79.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "79.9.0"
+version = "79.9.1"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-79.9.0/src/alacorder/.DS_Store` & `alacorder-79.9.1/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-79.9.0/src/alacorder/__init__.py` & `alacorder-79.9.1/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-79.9.0/src/alacorder/__main__.py` & `alacorder-79.9.1/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 """
 ALACORDER --------------------
 ╔═╗╔╗╔╔═╗╦ ╦╔═╗╔═╗╦  ╔═╗╔═╗╔═╗
 ╚═╗║║║║ ║║║║╠═╝╠═╣║  ╠═╣║  ║╣ 
 ╚═╝╝╚╝╚═╝╚╩╝╩  ╩ ╩╩═╝╩ ╩╚═╝╚═╝
 (c) 2023 Sam Robson ----------
 
- Dependencies: 
-    python 3.9 - 3.11
-    brotli 1.0.9
-    click 8.1.3
-    polars 0.17.6
-    PyMuPDF 1.21.1
-    PySimpleGUI 4.60.4
-    selenium 4.8.3
-    tqdm 4.65.0
-    xlsx2csv 0.8.1
-    XlsxWriter 3.0.9
+ Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
+ 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "79.9.0"
+version = "79.9.1"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -321,28 +312,31 @@
     return out
 
 
 def vrr_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
-    print("Combining cases by AIS / Unique ID to create voting rights summary...", cf=cf)
+    print(
+        "Combining cases by AIS / Unique ID to create voting rights summary...", cf=cf
+    )
     vr = vrr_summary_from_pairs(cf["INPUTS"], cf["PAIRS"])
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
             vr, sheet_names=["VRR"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
         )
         print("Completed table export.", cf=cf)
     if cf["LOG"]:
         print("Created table successfully.")
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("VRR-COMPLETE", True)
     return vr
 
+
 def charges_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
     print("Combining cases by AIS / Unique ID to create charges summary...", cf=cf)
     ch = charges_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
     if not cf["NO_WRITE"]:
@@ -4023,15 +4017,15 @@
     is_flag=True,
     help="Do not print logs to console",
 )
 @click.option(
     "--no-write", default=False, is_flag=True, help="Do not export to output path"
 )
 @click.option(
-    "--debug",  default=False, is_flag=True, help="Print debug logs to console"
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
 def cli_table(
     input_path, output_path, count, table, overwrite, no_write, no_log, no_prompt, debug
 ):
@@ -4068,14 +4062,15 @@
         debug=debug,
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf)
     return o
 
+
 @main.command(name="multi", help="Export all data tables to .xls/.xlsx")
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
     prompt="Input Path",
@@ -4219,16 +4214,24 @@
         overwrite (bool): Overwrite existing files at output path
         no_write (bool): Do not export to output path
         no_log(bool): Do not print logs to console
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console
     """
     log = not no_log
-    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
-        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    if os.path.splitext(output_path)[1] not in (
+        ".xls",
+        ".xlsx",
+        ".csv",
+        ".json",
+        ".parquet",
+    ):
+        error(
+            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
+        )
     cf = set(
         input_path,
         output_path,
         count=count,
         table="cases",
         overwrite=overwrite,
         no_write=no_write,
@@ -4250,16 +4253,20 @@
     type=click.Path(),
     prompt="Input Path",
     show_choices=False,
 )
 @click.option(
     "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
 )
-@click.option("--filing", "-f", is_flag=True, default=False, help="Only export filing charges")
-@click.option("--disposition", is_flag=True, default=False, help="Only export disposition charges")
+@click.option(
+    "--filing", "-f", is_flag=True, default=False, help="Only export filing charges"
+)
+@click.option(
+    "--disposition", is_flag=True, default=False, help="Only export disposition charges"
+)
 @click.option(
     "--count",
     "-c",
     default=0,
     help="Total cases to pull from input",
     show_default=False,
 )
@@ -4290,15 +4297,24 @@
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
 def cli_charges(
-    input_path, output_path, filing, disposition, count, overwrite, no_write, no_log, no_prompt, debug
+    input_path,
+    output_path,
+    filing,
+    disposition,
+    count,
+    overwrite,
+    no_write,
+    no_log,
+    no_prompt,
+    debug,
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
         output_path (str): Path to table output
@@ -4308,16 +4324,24 @@
         overwrite (bool): Overwrite existing files at output path
         no_write (bool): Do not export to output path
         no_log(bool): Do not print logs to console
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console
     """
     log = not no_log
-    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
-        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    if os.path.splitext(output_path)[1] not in (
+        ".xls",
+        ".xlsx",
+        ".csv",
+        ".json",
+        ".parquet",
+    ):
+        error(
+            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
+        )
     table = "charges" if not filing and not disposition else ""
     table = "filing" if filing else table
     table = "disposition" if disposition else table
     cf = set(
         input_path,
         output_path,
         count=count,
@@ -4329,14 +4353,15 @@
         debug=debug,
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf)
     return o
 
+
 @main.command(name="fees", help="Create and export fees table")
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
     prompt="Input Path",
@@ -4395,16 +4420,24 @@
         overwrite (bool): Overwrite existing files at output path
         no_write (bool): Do not export to output path
         no_log(bool): Do not print logs to console
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console
     """
     log = not no_log
-    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
-        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    if os.path.splitext(output_path)[1] not in (
+        ".xls",
+        ".xlsx",
+        ".csv",
+        ".json",
+        ".parquet",
+    ):
+        error(
+            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
+        )
     cf = set(
         input_path,
         output_path,
         count=count,
         table="fees",
         overwrite=overwrite,
         no_write=no_write,
@@ -4413,14 +4446,15 @@
         debug=debug,
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf)
     return o
 
+
 @main.command(name="settings", help="Create and export settings table")
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
     prompt="Input Path",
@@ -4479,16 +4513,24 @@
         overwrite (bool): Overwrite existing files at output path
         no_write (bool): Do not export to output path
         no_log(bool): Do not print logs to console
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console
     """
     log = not no_log
-    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
-        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    if os.path.splitext(output_path)[1] not in (
+        ".xls",
+        ".xlsx",
+        ".csv",
+        ".json",
+        ".parquet",
+    ):
+        error(
+            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
+        )
     cf = set(
         input_path,
         output_path,
         count=count,
         table="settings",
         overwrite=overwrite,
         no_write=no_write,
@@ -4497,14 +4539,15 @@
         debug=debug,
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf)
     return o
 
+
 @main.command(name="witnesses", help="Create and export witnesses table")
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
     prompt="Input Path",
@@ -4563,16 +4606,24 @@
         overwrite (bool): Overwrite existing files at output path
         no_write (bool): Do not export to output path
         no_log(bool): Do not print logs to console
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console
     """
     log = not no_log
-    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
-        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    if os.path.splitext(output_path)[1] not in (
+        ".xls",
+        ".xlsx",
+        ".csv",
+        ".json",
+        ".parquet",
+    ):
+        error(
+            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
+        )
     cf = set(
         input_path,
         output_path,
         count=count,
         table="witnesses",
         overwrite=overwrite,
         no_write=no_write,
@@ -4581,15 +4632,18 @@
         debug=debug,
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf)
     return o
 
-@main.command(name="case-action-summary", help="Create and export case action summaries")
+
+@main.command(
+    name="case-action-summary", help="Create and export case action summaries"
+)
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
     prompt="Input Path",
     show_choices=False,
@@ -4647,16 +4701,24 @@
         overwrite (bool): Overwrite existing files at output path
         no_write (bool): Do not export to output path
         no_log(bool): Do not print logs to console
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console
     """
     log = not no_log
-    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
-        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    if os.path.splitext(output_path)[1] not in (
+        ".xls",
+        ".xlsx",
+        ".csv",
+        ".json",
+        ".parquet",
+    ):
+        error(
+            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
+        )
     cf = set(
         input_path,
         output_path,
         count=count,
         table="case-action-summary",
         overwrite=overwrite,
         no_write=no_write,
@@ -4732,16 +4794,24 @@
         overwrite (bool): Overwrite existing files at output path
         no_write (bool): Do not export to output path
         no_log(bool): Do not print logs to console
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console
     """
     log = not no_log
-    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
-        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    if os.path.splitext(output_path)[1] not in (
+        ".xls",
+        ".xlsx",
+        ".csv",
+        ".json",
+        ".parquet",
+    ):
+        error(
+            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
+        )
     cf = set(
         input_path,
         output_path,
         count=count,
         table="images",
         overwrite=overwrite,
         no_write=no_write,
@@ -4750,14 +4820,15 @@
         debug=debug,
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf)
     return o
 
+
 @main.command(name="attorneys", help="Create and export attorneys table")
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
     prompt="Input Path",
@@ -4816,16 +4887,24 @@
         overwrite (bool): Overwrite existing files at output path
         no_write (bool): Do not export to output path
         no_log(bool): Do not print logs to console
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console
     """
     log = not no_log
-    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
-        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    if os.path.splitext(output_path)[1] not in (
+        ".xls",
+        ".xlsx",
+        ".csv",
+        ".json",
+        ".parquet",
+    ):
+        error(
+            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
+        )
     cf = set(
         input_path,
         output_path,
         count=count,
         table="attorneys",
         overwrite=overwrite,
         no_write=no_write,
@@ -4834,14 +4913,15 @@
         debug=debug,
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf)
     return o
 
+
 @main.command(name="archive", help="Create full text archive from case PDFs")
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
     prompt="PDF directory or archive input",
```

### Comparing `alacorder-79.9.0/src/alacorder/alac.py` & `alacorder-79.9.1/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 """
 ALACORDER --------------------
 ╔═╗╔╗╔╔═╗╦ ╦╔═╗╔═╗╦  ╔═╗╔═╗╔═╗
 ╚═╗║║║║ ║║║║╠═╝╠═╣║  ╠═╣║  ║╣ 
 ╚═╝╝╚╝╚═╝╚╩╝╩  ╩ ╩╩═╝╩ ╩╚═╝╚═╝
 (c) 2023 Sam Robson ----------
 
- Dependencies: 
-    python 3.9 - 3.11
-    brotli 1.0.9
-    click 8.1.3
-    polars 0.17.6
-    PyMuPDF 1.21.1
-    PySimpleGUI 4.60.4
-    selenium 4.8.3
-    tqdm 4.65.0
-    xlsx2csv 0.8.1
-    XlsxWriter 3.0.9
+ Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
+ 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "79.9.0"
+version = "79.9.1"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -321,28 +312,31 @@
     return out
 
 
 def vrr_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
-    print("Combining cases by AIS / Unique ID to create voting rights summary...", cf=cf)
+    print(
+        "Combining cases by AIS / Unique ID to create voting rights summary...", cf=cf
+    )
     vr = vrr_summary_from_pairs(cf["INPUTS"], cf["PAIRS"])
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
             vr, sheet_names=["VRR"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
         )
         print("Completed table export.", cf=cf)
     if cf["LOG"]:
         print("Created table successfully.")
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("VRR-COMPLETE", True)
     return vr
 
+
 def charges_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
     print("Combining cases by AIS / Unique ID to create charges summary...", cf=cf)
     ch = charges_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
     if not cf["NO_WRITE"]:
@@ -4023,15 +4017,15 @@
     is_flag=True,
     help="Do not print logs to console",
 )
 @click.option(
     "--no-write", default=False, is_flag=True, help="Do not export to output path"
 )
 @click.option(
-    "--debug",  default=False, is_flag=True, help="Print debug logs to console"
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
 def cli_table(
     input_path, output_path, count, table, overwrite, no_write, no_log, no_prompt, debug
 ):
@@ -4068,14 +4062,15 @@
         debug=debug,
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf)
     return o
 
+
 @main.command(name="multi", help="Export all data tables to .xls/.xlsx")
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
     prompt="Input Path",
@@ -4219,16 +4214,24 @@
         overwrite (bool): Overwrite existing files at output path
         no_write (bool): Do not export to output path
         no_log(bool): Do not print logs to console
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console
     """
     log = not no_log
-    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
-        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    if os.path.splitext(output_path)[1] not in (
+        ".xls",
+        ".xlsx",
+        ".csv",
+        ".json",
+        ".parquet",
+    ):
+        error(
+            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
+        )
     cf = set(
         input_path,
         output_path,
         count=count,
         table="cases",
         overwrite=overwrite,
         no_write=no_write,
@@ -4250,16 +4253,20 @@
     type=click.Path(),
     prompt="Input Path",
     show_choices=False,
 )
 @click.option(
     "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
 )
-@click.option("--filing", "-f", is_flag=True, default=False, help="Only export filing charges")
-@click.option("--disposition", is_flag=True, default=False, help="Only export disposition charges")
+@click.option(
+    "--filing", "-f", is_flag=True, default=False, help="Only export filing charges"
+)
+@click.option(
+    "--disposition", is_flag=True, default=False, help="Only export disposition charges"
+)
 @click.option(
     "--count",
     "-c",
     default=0,
     help="Total cases to pull from input",
     show_default=False,
 )
@@ -4290,15 +4297,24 @@
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
 def cli_charges(
-    input_path, output_path, filing, disposition, count, overwrite, no_write, no_log, no_prompt, debug
+    input_path,
+    output_path,
+    filing,
+    disposition,
+    count,
+    overwrite,
+    no_write,
+    no_log,
+    no_prompt,
+    debug,
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
         output_path (str): Path to table output
@@ -4308,16 +4324,24 @@
         overwrite (bool): Overwrite existing files at output path
         no_write (bool): Do not export to output path
         no_log(bool): Do not print logs to console
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console
     """
     log = not no_log
-    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
-        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    if os.path.splitext(output_path)[1] not in (
+        ".xls",
+        ".xlsx",
+        ".csv",
+        ".json",
+        ".parquet",
+    ):
+        error(
+            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
+        )
     table = "charges" if not filing and not disposition else ""
     table = "filing" if filing else table
     table = "disposition" if disposition else table
     cf = set(
         input_path,
         output_path,
         count=count,
@@ -4329,14 +4353,15 @@
         debug=debug,
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf)
     return o
 
+
 @main.command(name="fees", help="Create and export fees table")
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
     prompt="Input Path",
@@ -4395,16 +4420,24 @@
         overwrite (bool): Overwrite existing files at output path
         no_write (bool): Do not export to output path
         no_log(bool): Do not print logs to console
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console
     """
     log = not no_log
-    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
-        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    if os.path.splitext(output_path)[1] not in (
+        ".xls",
+        ".xlsx",
+        ".csv",
+        ".json",
+        ".parquet",
+    ):
+        error(
+            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
+        )
     cf = set(
         input_path,
         output_path,
         count=count,
         table="fees",
         overwrite=overwrite,
         no_write=no_write,
@@ -4413,14 +4446,15 @@
         debug=debug,
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf)
     return o
 
+
 @main.command(name="settings", help="Create and export settings table")
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
     prompt="Input Path",
@@ -4479,16 +4513,24 @@
         overwrite (bool): Overwrite existing files at output path
         no_write (bool): Do not export to output path
         no_log(bool): Do not print logs to console
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console
     """
     log = not no_log
-    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
-        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    if os.path.splitext(output_path)[1] not in (
+        ".xls",
+        ".xlsx",
+        ".csv",
+        ".json",
+        ".parquet",
+    ):
+        error(
+            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
+        )
     cf = set(
         input_path,
         output_path,
         count=count,
         table="settings",
         overwrite=overwrite,
         no_write=no_write,
@@ -4497,14 +4539,15 @@
         debug=debug,
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf)
     return o
 
+
 @main.command(name="witnesses", help="Create and export witnesses table")
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
     prompt="Input Path",
@@ -4563,16 +4606,24 @@
         overwrite (bool): Overwrite existing files at output path
         no_write (bool): Do not export to output path
         no_log(bool): Do not print logs to console
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console
     """
     log = not no_log
-    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
-        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    if os.path.splitext(output_path)[1] not in (
+        ".xls",
+        ".xlsx",
+        ".csv",
+        ".json",
+        ".parquet",
+    ):
+        error(
+            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
+        )
     cf = set(
         input_path,
         output_path,
         count=count,
         table="witnesses",
         overwrite=overwrite,
         no_write=no_write,
@@ -4581,15 +4632,18 @@
         debug=debug,
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf)
     return o
 
-@main.command(name="case-action-summary", help="Create and export case action summaries")
+
+@main.command(
+    name="case-action-summary", help="Create and export case action summaries"
+)
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
     prompt="Input Path",
     show_choices=False,
@@ -4647,16 +4701,24 @@
         overwrite (bool): Overwrite existing files at output path
         no_write (bool): Do not export to output path
         no_log(bool): Do not print logs to console
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console
     """
     log = not no_log
-    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
-        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    if os.path.splitext(output_path)[1] not in (
+        ".xls",
+        ".xlsx",
+        ".csv",
+        ".json",
+        ".parquet",
+    ):
+        error(
+            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
+        )
     cf = set(
         input_path,
         output_path,
         count=count,
         table="case-action-summary",
         overwrite=overwrite,
         no_write=no_write,
@@ -4732,16 +4794,24 @@
         overwrite (bool): Overwrite existing files at output path
         no_write (bool): Do not export to output path
         no_log(bool): Do not print logs to console
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console
     """
     log = not no_log
-    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
-        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    if os.path.splitext(output_path)[1] not in (
+        ".xls",
+        ".xlsx",
+        ".csv",
+        ".json",
+        ".parquet",
+    ):
+        error(
+            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
+        )
     cf = set(
         input_path,
         output_path,
         count=count,
         table="images",
         overwrite=overwrite,
         no_write=no_write,
@@ -4750,14 +4820,15 @@
         debug=debug,
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf)
     return o
 
+
 @main.command(name="attorneys", help="Create and export attorneys table")
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
     prompt="Input Path",
@@ -4816,16 +4887,24 @@
         overwrite (bool): Overwrite existing files at output path
         no_write (bool): Do not export to output path
         no_log(bool): Do not print logs to console
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console
     """
     log = not no_log
-    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
-        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    if os.path.splitext(output_path)[1] not in (
+        ".xls",
+        ".xlsx",
+        ".csv",
+        ".json",
+        ".parquet",
+    ):
+        error(
+            "File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export."
+        )
     cf = set(
         input_path,
         output_path,
         count=count,
         table="attorneys",
         overwrite=overwrite,
         no_write=no_write,
@@ -4834,14 +4913,15 @@
         debug=debug,
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf)
     return o
 
+
 @main.command(name="archive", help="Create full text archive from case PDFs")
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
     prompt="PDF directory or archive input",
```


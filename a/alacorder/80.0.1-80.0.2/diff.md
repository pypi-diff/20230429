# Comparing `tmp/alacorder-80.0.1.tar.gz` & `tmp/alacorder-80.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.0.1.tar", max compression
+gzip compressed data, was "alacorder-80.0.2.tar", max compression
```

## Comparing `alacorder-80.0.1.tar` & `alacorder-80.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.0.1/LICENSE
--rw-r--r--   0        0        0     6750 2023-04-29 03:07:07.203418 alacorder-80.0.1/README.md
--rw-r--r--   0        0        0      697 2023-04-29 03:05:43.347566 alacorder-80.0.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-04-28 21:53:41.054817 alacorder-80.0.1/src/alacorder/.DS_Store
--rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-80.0.1/src/alacorder/__init__.py
--rw-r--r--   0        0        0   190596 2023-04-29 00:41:32.764564 alacorder-80.0.1/src/alacorder/__main__.py
--rw-r--r--   0        0        0   195064 2023-04-29 03:05:30.842169 alacorder-80.0.1/src/alacorder/alac.py
--rw-r--r--   0        0        0     7679 1970-01-01 00:00:00.000000 alacorder-80.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.0.2/LICENSE
+-rw-r--r--   0        0        0     6750 2023-04-29 03:07:07.203418 alacorder-80.0.2/README.md
+-rw-r--r--   0        0        0      697 2023-04-29 04:20:16.087769 alacorder-80.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-04-29 04:20:01.169511 alacorder-80.0.2/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-80.0.2/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   196670 2023-04-29 04:19:32.129885 alacorder-80.0.2/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   196670 2023-04-29 04:19:13.963251 alacorder-80.0.2/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7679 1970-01-01 00:00:00.000000 alacorder-80.0.2/PKG-INFO
```

### Comparing `alacorder-80.0.1/LICENSE` & `alacorder-80.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.1/README.md` & `alacorder-80.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.1/pyproject.toml` & `alacorder-80.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.0.1"
+version = "80.0.2"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.0.1/src/alacorder/.DS_Store` & `alacorder-80.0.2/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.1/src/alacorder/__init__.py` & `alacorder-80.0.2/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.1/src/alacorder/__main__.py` & `alacorder-80.0.2/src/alacorder/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,31 @@
 
  Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
  
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.0.0"
+version = "80.0.2"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.chrome.options import Options
 
+
 #   #   #   #               LOGS                 #   #   #   #
 
+
 pl.Config.set_tbl_rows(20)
 pl.Config.set_fmt_str_lengths(100)
 pl.Config.set_tbl_width_chars(90)
 pl.Config.set_tbl_formatting("NOTHING")
 pl.Config.set_tbl_hide_column_data_types(True)
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
@@ -129,14 +131,16 @@
     df = read(cf)
     plog("Extracting case info...", cf=cf)
     ca, ac, af = split_cases(df, debug=cf["DEBUG"])
     print("Parsing charges...", cf=cf)
     ch = split_charges(ac, debug=cf["DEBUG"])
     print("Parsing fees...", cf=cf)
     fs = split_fees(af, debug=cf["DEBUG"])
+    print("Parsing financial history...", cf=cf)
+    fh = explode_split_financial_history(df, debug=cf['DEBUG'])
     print("Parsing settings...", cf=cf)
     settings = explode_settings(df)
     print("Parsing case action summaries...", cf=cf)
     cas = explode_case_action_summary(df)
     print("Parsing witnesses...", cf=cf)
     wit = explode_witnesses(df)
     print("Parsing attorneys...", cf=cf)
@@ -243,14 +247,29 @@
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["witnesses"], cf=cf)
         print("Completed table export.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
+def financial_history(cf):
+    """
+    Collect witnesses tables using configuration object `cf`.
+    """
+    q = read(cf)
+    print("Parsing financial history...", cf=cf)
+    out = explode_split_financial_history(q)
+    if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
+        write(out, sheet_names=["financial-history"], cf=cf)
+        print("Completed table export.", cf=cf)
+    if cf["WINDOW"]:
+        cf["WINDOW"].write_event_value("COMPLETE-TB", True)
+    return out
+
 
 def cas(cf):
     """
     Collect case action summaries using configuration object `cf`.
     """
     print("Parsing case action summaries...", cf=cf)
     q = read(cf["QUEUE"])
@@ -608,27 +627,29 @@
         and archive == False
         and fetch == False
         and table
         not in (
             "cases",
             "charges",
             "fees",
+            "financial-history",
+            "history",
             "disposition",
             "disposition-charges",
             "filing",
             "filing-charges",
             "attorneys",
             "settings",
             "images",
             "case-action-summary",
             "witnesses",
         )
     ):
         error(
-            "Single table export choice required! (cases, charges, fees, disposition, filing, settings, attorneys, images, case-action-summary, witnesses)",
+            "Single table export choice required! (cases, charges, fees, financial-history, disposition, filing, settings, attorneys, images, case-action-summary, witnesses)",
             cf={"WINDOW": window, "FORCE": force},
         )
 
     if archive and append and existing_output and not no_write:  # raise append failure
         try:
             old_archive = read(outputs)
         except:
@@ -975,14 +996,17 @@
         return ca
     elif (
         cf["TABLE"].lower() in ("fees", "feesheet", "fines")
         and cf["SUPPORT_SINGLETABLE"]
     ):
         fs = fees(cf)
         return fs
+    elif cf["TABLE"].lower() in ("financial-history", "history"):
+        fh = financial_history(cf)
+        return fh
     elif cf["TABLE"].lower() in ("witnesses", "witness") and cf["SUPPORT_SINGLETABLE"]:
         out = witnesses(cf)
         return out
     elif (
         cf["TABLE"].lower()
         in (
             "case-action-summary",
@@ -1077,14 +1101,50 @@
     out = pl.concat([inarc, outarc])
 
     if window:
         window.write_event_value("COMPLETE-AA", True)
     write(out, path=outpath, overwrite=True)
     return out
 
+def getCaseNumber(text):
+    try:
+        return (
+            re.search(r"Case Number: (\d\d-\w+) County:", str(text)).group(1)[0:2]
+            + "-"
+            + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
+        )
+    except:
+        return ""
+
+def rename_pdfs(cf):
+    if isinstance(cf, dict):
+        q = cf['QUEUE']
+    elif isinstance(cf, pl.dataframe.frame.DataFrame):
+        if "Path" in cf.columns:
+            q = cf.select("Path").to_series().to_list()
+            cf = {'LOG': False}
+    else:
+        q = cf
+        cf = {'LOG': False}
+    if cf['LOG']:
+        for path in tqdm(q):
+            text = extract_text(path)
+            try:
+                cnum = re.search(r"Case Number: (\d\d-\w+) County:", str(text)).group(1)[0:2] + "-" + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
+            except:
+                cnum = os.path.split(path)[1]
+            newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
+            os.rename(path, newpath)
+    else:
+        for path in q:
+            text = extract_text(path)
+            cnum = re.search(r"Case Number: (\d\d-\w+) County:", str(text)).group(1)[0:2] + "-" + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
+            newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
+            os.rename(path, newpath)
+
 
 def make_pairs_template(df, debug=False):
     if isinstance(df, str):
         df = read(df)
     names = df.with_columns(
         [
             pl.concat_str(
@@ -2110,14 +2170,30 @@
         "TBNV1",
         "TBNV2",
         "DriverLicenseNo",
         "StateID",
     )
     return cases, all_charges, all_fees
 
+def explode_split_financial_history(df, debug=False):
+    fh = df.with_columns([
+        pl.col("AllPagesText").str.extract_all(r'(\d\d/\d\d/\d\d\d\d)\s(RECEIPT|CREDIT)\s(\$\d+\.\d\d)\s(\w\d\d\d)\s(\d\d\d)\s(\w)\s(....)\s(\d{8})\s(\d{7})\s(\w{3})').alias("FinancialHistory")
+        ])
+    fh = fh.explode("FinancialHistory")
+    fh = fh.with_columns([
+        pl.col("FinancialHistory").str.extract(r'(\d\d/\d\d/\d\d\d\d)').alias("TransactionDate"),
+        pl.col("FinancialHistory").str.extract(r'(RECEIPT|CREDIT)').alias("Description"),
+        pl.col("FinancialHistory").str.extract(r'(\$\d+\.\d\d)').str.replace(r'\$','').str.strip().cast(pl.Float64, strict=False).alias("Amount"),
+        pl.col("FinancialHistory").str.extract(r'\s(\w\d\d\d)\s').alias("FromParty"),
+        pl.col("FinancialHistory").str.extract(r'\s(\d\d\d)\s').alias("ToParty"),
+        pl.col("FinancialHistory").str.extract(r'\s(\w)\s').alias("AdminFee"),
+        pl.col("FinancialHistory").str.extract(r'\s([A-Z]{3})\s').alias("Operator"),
+        ])
+    fh = fh.fill_null('')
+    return fh
 
 def split_charges(df, debug=False):
     dlog(df.columns, df.shape, "^ split_charges input param", cf=debug)
     charges = df.with_columns(
         [
             pl.col("Name"),
             pl.col("CaseNumber"),
@@ -3522,14 +3598,17 @@
             sg.Radio("Case Action Summary", "TABLE", key="TB-CAS", default=False),
             sg.Radio("Witnesses", "TABLE", key="TB-WITNESSES", default=False),
             sg.Radio("Images", "TABLE", key="TB-IMAGES", default=False),
         ],
         [
             sg.Radio("Attorneys", "TABLE", key="TB-ATTORNEYS", default=False),
             sg.Radio("Settings", "TABLE", key="TB-SETTINGS", default=False),
+            sg.Radio("Financial History", "TABLE", key="TB-HISTORY", default=False),
+        ],
+        [
             sg.Radio("Disposition", "TABLE", key="TB-DISPOSITION", default=False),
             sg.Radio("Filing", "TABLE", key="TB-FILING", default=False),
         ],
         [
             sg.Text("Max cases: "),
             sg.Input(key="TB-COUNT", default_text="0", size=[5, 1]),
             sg.Checkbox("Allow Overwrite", key="TB-OVERWRITE", default=True),
@@ -3689,14 +3768,15 @@
             table = "case-action-summary" if window["TB-CAS"].get() else table
             table = "witnesses" if window["TB-WITNESSES"].get() else table
             table = "images" if window["TB-IMAGES"].get() else table
             table = "attorneys" if window["TB-ATTORNEYS"].get() else table
             table = "settings" if window["TB-SETTINGS"].get() else table
             table = "disposition" if window["TB-DISPOSITION"].get() else table
             table = "filing" if window["TB-FILING"].get() else table
+            table = "financial-history" if window["TB-HISTORY"].get() else table
             if (
                 window["TB-INPUTPATH"].get() == ""
                 or window["TB-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
             else:
                 cf = set(
@@ -4540,14 +4620,106 @@
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf)
     return o
 
 
+@main.command(name="financial-history", help="Create and export financial history table")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_finhist(
+    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write `cases` table to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
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
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table="financial-history",
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = init(cf)
+    return o
+
 @main.command(name="witnesses", help="Create and export witnesses table")
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
     prompt="Input Path",
@@ -5002,14 +5174,20 @@
         debug=debug,
     )
     if debug:
         click.echo(cf)
     o = archive(cf)
     return o
 
+@main.command(name="rename", help="Rename cases in input directory to case numbers")
+@click.option("--input-path", "-in", "input_path", required=True, type=click.Path(), prompt="PDF directory")
+def cli_rename(input_path):
+    c = cf(input_path, log=True)
+    rename_pdfs(c)
+
 
 @main.command(
     name="pair",
     help="Create blank AIS / unique pairing template",
 )
 @click.option(
     "--input-path",
```

### Comparing `alacorder-80.0.1/src/alacorder/alac.py` & `alacorder-80.0.2/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,29 +7,31 @@
 
  Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
  
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.0.1"
+version = "80.0.2"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.chrome.options import Options
 
+
 #   #   #   #               LOGS                 #   #   #   #
 
+
 pl.Config.set_tbl_rows(20)
 pl.Config.set_fmt_str_lengths(100)
 pl.Config.set_tbl_width_chars(90)
 pl.Config.set_tbl_formatting("NOTHING")
 pl.Config.set_tbl_hide_column_data_types(True)
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
@@ -1099,14 +1101,50 @@
     out = pl.concat([inarc, outarc])
 
     if window:
         window.write_event_value("COMPLETE-AA", True)
     write(out, path=outpath, overwrite=True)
     return out
 
+def getCaseNumber(text):
+    try:
+        return (
+            re.search(r"Case Number: (\d\d-\w+) County:", str(text)).group(1)[0:2]
+            + "-"
+            + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
+        )
+    except:
+        return ""
+
+def rename_pdfs(cf):
+    if isinstance(cf, dict):
+        q = cf['QUEUE']
+    elif isinstance(cf, pl.dataframe.frame.DataFrame):
+        if "Path" in cf.columns:
+            q = cf.select("Path").to_series().to_list()
+            cf = {'LOG': False}
+    else:
+        q = cf
+        cf = {'LOG': False}
+    if cf['LOG']:
+        for path in tqdm(q):
+            text = extract_text(path)
+            try:
+                cnum = re.search(r"Case Number: (\d\d-\w+) County:", str(text)).group(1)[0:2] + "-" + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
+            except:
+                cnum = os.path.split(path)[1]
+            newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
+            os.rename(path, newpath)
+    else:
+        for path in q:
+            text = extract_text(path)
+            cnum = re.search(r"Case Number: (\d\d-\w+) County:", str(text)).group(1)[0:2] + "-" + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
+            newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
+            os.rename(path, newpath)
+
 
 def make_pairs_template(df, debug=False):
     if isinstance(df, str):
         df = read(df)
     names = df.with_columns(
         [
             pl.concat_str(
@@ -5136,14 +5174,20 @@
         debug=debug,
     )
     if debug:
         click.echo(cf)
     o = archive(cf)
     return o
 
+@main.command(name="rename", help="Rename cases in input directory to case numbers")
+@click.option("--input-path", "-in", "input_path", required=True, type=click.Path(), prompt="PDF directory")
+def cli_rename(input_path):
+    c = cf(input_path, log=True)
+    rename_pdfs(c)
+
 
 @main.command(
     name="pair",
     help="Create blank AIS / unique pairing template",
 )
 @click.option(
     "--input-path",
```

### Comparing `alacorder-80.0.1/PKG-INFO` & `alacorder-80.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.0.1
+Version: 80.0.2
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


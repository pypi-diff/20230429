# Comparing `tmp/alacorder-80.0.2.tar.gz` & `tmp/alacorder-80.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.0.2.tar", max compression
+gzip compressed data, was "alacorder-80.0.3.tar", max compression
```

## Comparing `alacorder-80.0.2.tar` & `alacorder-80.0.3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.0.2/LICENSE
--rw-r--r--   0        0        0     6750 2023-04-29 03:07:07.203418 alacorder-80.0.2/README.md
--rw-r--r--   0        0        0      697 2023-04-29 04:20:16.087769 alacorder-80.0.2/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-04-29 04:20:01.169511 alacorder-80.0.2/src/alacorder/.DS_Store
--rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-80.0.2/src/alacorder/__init__.py
--rw-r--r--   0        0        0   196670 2023-04-29 04:19:32.129885 alacorder-80.0.2/src/alacorder/__main__.py
--rw-r--r--   0        0        0   196670 2023-04-29 04:19:13.963251 alacorder-80.0.2/src/alacorder/alac.py
--rw-r--r--   0        0        0     7679 1970-01-01 00:00:00.000000 alacorder-80.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.0.3/LICENSE
+-rw-r--r--   0        0        0     6750 2023-04-29 03:07:07.203418 alacorder-80.0.3/README.md
+-rw-r--r--   0        0        0      697 2023-04-29 14:45:03.069647 alacorder-80.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-80.0.3/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   196842 2023-04-29 14:44:32.156574 alacorder-80.0.3/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   196842 2023-04-29 14:44:22.792925 alacorder-80.0.3/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7679 1970-01-01 00:00:00.000000 alacorder-80.0.3/PKG-INFO
```

### Comparing `alacorder-80.0.2/LICENSE` & `alacorder-80.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.2/README.md` & `alacorder-80.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.2/pyproject.toml` & `alacorder-80.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.0.2"
+version = "80.0.3"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.0.2/src/alacorder/__init__.py` & `alacorder-80.0.3/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.2/src/alacorder/__main__.py` & `alacorder-80.0.3/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
  Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
  
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.0.2"
+version = "80.0.3"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -151,20 +151,21 @@
     ch_filing = ch.filter(pl.col("Filing") == True).select(
         pl.exclude("CourtAction", "CourtActionDate")
     )
     ch_disposition = ch.filter(pl.col("Filing") == False)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
-            [ca, ch_filing, ch_disposition, fs, settings, cas, wit, att, img],
+            [ca, ch_filing, ch_disposition, fs, fh, settings, cas, wit, att, img],
             sheet_names=[
                 "cases",
                 "filing-charges",
                 "disposition-charges",
                 "fees",
+                "financial-history",
                 "settings",
                 "case-action-summary",
                 "witnesses",
                 "attorneys",
                 "images",
             ],
             cf=cf,
@@ -173,14 +174,15 @@
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     out = {
         "cases": ca,
         "charges": ch,
         "filing-charges": ch_filing,
         "disposition-charges": ch_disposition,
         "fees": fs,
+        "financial-history": fh, 
         "settings": settings,
         "case-action-summary": cas,
         "witnesses": wit,
         "attorneys": att,
         "images": img,
     }
     return out
@@ -755,19 +757,22 @@
 def read(cf):
     """
     Read `cf` input PDF directory or case text archive into memory.
     """
     if isinstance(cf, pl.dataframe.frame.DataFrame):  # df input
         df = cf
         if "AllPagesTextNoNewLine" not in df.columns and "AllPagesText" in df.columns:
-            df = df.with_columns(
-                pl.col("AllPagesText")
-                .str.replace_all(r"\n", " ")
-                .alias("AllPagesTextNoNewLine")
-            )
+            try:
+                df = df.with_columns(
+                    pl.col("AllPagesText")
+                    .str.replace_all(r"\n", " ")
+                    .alias("AllPagesTextNoNewLine")
+                )
+            except:
+                pass
             return df
         else:
             return df
     elif isinstance(cf, list):  # [paths] input
         queue = cf
         aptxt = []
         for pp in queue:
@@ -872,15 +877,15 @@
             with open(cf) as f:
                 text = f.read()
             return text
         elif ext == ".pdf":
             text = extract_text(cf)
             return text
     else:
-        return None
+        error("Could not read input.")
 
 
 def write(outputs, sheet_names=[], cf=None, path=None, overwrite=False):
     """Write `outputs` to output path at `cf['OUTPUT_PATH']` or `path`.
 
     Args:
         outputs ([DataFrame]): DataFrame(s) to write to output
```

### Comparing `alacorder-80.0.2/src/alacorder/alac.py` & `alacorder-80.0.3/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
  Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
  
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.0.2"
+version = "80.0.3"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -151,20 +151,21 @@
     ch_filing = ch.filter(pl.col("Filing") == True).select(
         pl.exclude("CourtAction", "CourtActionDate")
     )
     ch_disposition = ch.filter(pl.col("Filing") == False)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
-            [ca, ch_filing, ch_disposition, fs, settings, cas, wit, att, img],
+            [ca, ch_filing, ch_disposition, fs, fh, settings, cas, wit, att, img],
             sheet_names=[
                 "cases",
                 "filing-charges",
                 "disposition-charges",
                 "fees",
+                "financial-history",
                 "settings",
                 "case-action-summary",
                 "witnesses",
                 "attorneys",
                 "images",
             ],
             cf=cf,
@@ -173,14 +174,15 @@
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     out = {
         "cases": ca,
         "charges": ch,
         "filing-charges": ch_filing,
         "disposition-charges": ch_disposition,
         "fees": fs,
+        "financial-history": fh, 
         "settings": settings,
         "case-action-summary": cas,
         "witnesses": wit,
         "attorneys": att,
         "images": img,
     }
     return out
@@ -755,19 +757,22 @@
 def read(cf):
     """
     Read `cf` input PDF directory or case text archive into memory.
     """
     if isinstance(cf, pl.dataframe.frame.DataFrame):  # df input
         df = cf
         if "AllPagesTextNoNewLine" not in df.columns and "AllPagesText" in df.columns:
-            df = df.with_columns(
-                pl.col("AllPagesText")
-                .str.replace_all(r"\n", " ")
-                .alias("AllPagesTextNoNewLine")
-            )
+            try:
+                df = df.with_columns(
+                    pl.col("AllPagesText")
+                    .str.replace_all(r"\n", " ")
+                    .alias("AllPagesTextNoNewLine")
+                )
+            except:
+                pass
             return df
         else:
             return df
     elif isinstance(cf, list):  # [paths] input
         queue = cf
         aptxt = []
         for pp in queue:
@@ -872,15 +877,15 @@
             with open(cf) as f:
                 text = f.read()
             return text
         elif ext == ".pdf":
             text = extract_text(cf)
             return text
     else:
-        return None
+        error("Could not read input.")
 
 
 def write(outputs, sheet_names=[], cf=None, path=None, overwrite=False):
     """Write `outputs` to output path at `cf['OUTPUT_PATH']` or `path`.
 
     Args:
         outputs ([DataFrame]): DataFrame(s) to write to output
```

### Comparing `alacorder-80.0.2/PKG-INFO` & `alacorder-80.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.0.2
+Version: 80.0.3
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


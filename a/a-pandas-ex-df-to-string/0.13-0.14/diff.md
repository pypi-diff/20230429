# Comparing `tmp/a_pandas_ex_df_to_string-0.13.tar.gz` & `tmp/a_pandas_ex_df_to_string-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a_pandas_ex_df_to_string-0.13.tar", last modified: Thu Apr 27 23:28:38 2023, max compression
+gzip compressed data, was "a_pandas_ex_df_to_string-0.14.tar", last modified: Fri Apr 28 22:58:39 2023, max compression
```

## Comparing `a_pandas_ex_df_to_string-0.13.tar` & `a_pandas_ex_df_to_string-0.14.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 23:28:38.812415 a_pandas_ex_df_to_string-0.13/
--rw-rw-rw-   0        0        0     1148 2023-04-27 23:28:31.000000 a_pandas_ex_df_to_string-0.13/LICENSE.rst
--rw-rw-rw-   0        0        0      185 2023-04-27 23:28:31.000000 a_pandas_ex_df_to_string-0.13/MANIFEST.in
--rw-rw-rw-   0        0        0     2993 2023-04-27 23:28:38.812415 a_pandas_ex_df_to_string-0.13/PKG-INFO
--rw-rw-rw-   0        0        0     2304 2023-04-15 00:18:30.000000 a_pandas_ex_df_to_string-0.13/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 23:28:38.808707 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/
--rw-rw-rw-   0        0        0     1069 2023-04-15 00:18:30.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/LICENSE
--rw-rw-rw-   0        0        0     2304 2023-04-15 00:18:30.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/README.MD
--rw-rw-rw-   0        0        0     2130 2023-04-27 23:27:05.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/__init__.py
--rw-rw-rw-   0        0        0        6 2023-04-27 23:28:37.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/requirements.txt
--rw-rw-rw-   0        0        0     1746 2023-04-27 23:28:37.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-27 23:28:38.811418 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string.egg-info/
--rw-rw-rw-   0        0        0     2993 2023-04-27 23:28:38.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      479 2023-04-27 23:28:38.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 23:28:38.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 23:28:38.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-04-27 23:28:38.000000 a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-04-27 23:28:38.813413 a_pandas_ex_df_to_string-0.13/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-04-27 23:28:37.000000 a_pandas_ex_df_to_string-0.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 22:58:39.876293 a_pandas_ex_df_to_string-0.14/
+-rw-rw-rw-   0        0        0     1148 2023-04-28 22:58:32.000000 a_pandas_ex_df_to_string-0.14/LICENSE.rst
+-rw-rw-rw-   0        0        0      185 2023-04-28 22:58:30.000000 a_pandas_ex_df_to_string-0.14/MANIFEST.in
+-rw-rw-rw-   0        0        0     2993 2023-04-28 22:58:39.876293 a_pandas_ex_df_to_string-0.14/PKG-INFO
+-rw-rw-rw-   0        0        0     2304 2023-04-27 23:30:25.000000 a_pandas_ex_df_to_string-0.14/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 22:58:39.871306 a_pandas_ex_df_to_string-0.14/a_pandas_ex_df_to_string/
+-rw-rw-rw-   0        0        0     1069 2023-04-27 23:30:25.000000 a_pandas_ex_df_to_string-0.14/a_pandas_ex_df_to_string/LICENSE
+-rw-rw-rw-   0        0        0     2304 2023-04-27 23:30:25.000000 a_pandas_ex_df_to_string-0.14/a_pandas_ex_df_to_string/README.MD
+-rw-rw-rw-   0        0        0     2184 2023-04-28 21:56:18.000000 a_pandas_ex_df_to_string-0.14/a_pandas_ex_df_to_string/__init__.py
+-rw-rw-rw-   0        0        0        6 2023-04-28 22:58:38.000000 a_pandas_ex_df_to_string-0.14/a_pandas_ex_df_to_string/requirements.txt
+-rw-rw-rw-   0        0        0     1746 2023-04-28 22:58:38.000000 a_pandas_ex_df_to_string-0.14/a_pandas_ex_df_to_string/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-28 22:58:39.876293 a_pandas_ex_df_to_string-0.14/a_pandas_ex_df_to_string.egg-info/
+-rw-rw-rw-   0        0        0     2993 2023-04-28 22:58:39.000000 a_pandas_ex_df_to_string-0.14/a_pandas_ex_df_to_string.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2023-04-28 22:58:39.000000 a_pandas_ex_df_to_string-0.14/a_pandas_ex_df_to_string.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 22:58:39.000000 a_pandas_ex_df_to_string-0.14/a_pandas_ex_df_to_string.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-28 22:58:39.000000 a_pandas_ex_df_to_string-0.14/a_pandas_ex_df_to_string.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-04-28 22:58:39.000000 a_pandas_ex_df_to_string-0.14/a_pandas_ex_df_to_string.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-04-28 22:58:39.877290 a_pandas_ex_df_to_string-0.14/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-04-28 22:58:38.000000 a_pandas_ex_df_to_string-0.14/setup.py
```

### Comparing `a_pandas_ex_df_to_string-0.13/LICENSE.rst` & `a_pandas_ex_df_to_string-0.14/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_df_to_string-0.13/PKG-INFO` & `a_pandas_ex_df_to_string-0.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a_pandas_ex_df_to_string
-Version: 0.13
+Version: 0.14
 Summary: Just a function to convert everything in Pandas DataFrames / Series to string
 Home-page: https://github.com/hansalemaos/a_pandas_ex_df_to_string
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: pandas,numpy,dataframe,series
 Classifier: Development Status :: 4 - Beta
```

### Comparing `a_pandas_ex_df_to_string-0.13/README.md` & `a_pandas_ex_df_to_string-0.14/README.md`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/LICENSE` & `a_pandas_ex_df_to_string-0.14/a_pandas_ex_df_to_string/LICENSE`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/README.MD` & `a_pandas_ex_df_to_string-0.14/a_pandas_ex_df_to_string/README.MD`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/__init__.py` & `a_pandas_ex_df_to_string-0.14/a_pandas_ex_df_to_string/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Union
 
 import pandas as pd
 from pandas.core.base import PandasObject
 
-def _conv_col(column):
+def _conv_col(column,errors='ignore'):
     try:
         return column.astype("string")
     except Exception:
         try:
-            return column.apply(lambda x: x.decode('utf-8', 'replace') if not isinstance(x, str) else str(x)).astype(
+            return column.apply(lambda x: x.decode('utf-8', errors) if not isinstance(x, str) else str(x)).astype(
             "string")
         except Exception:
-            return column.apply(lambda x: x.decode('utf-8', 'replace')).astype(
+            return column.apply(lambda x: x.decode('utf-8', errors)).astype(
             "string")
 
-def ds_to_string(df: Union[pd.DataFrame, pd.Series]) -> Union[pd.Series, pd.DataFrame]:
+def ds_to_string(df: Union[pd.DataFrame, pd.Series],errors='ignore') -> Union[pd.Series, pd.DataFrame]:
     """
     Example:
     from random import choice
     csvtests = [
     "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_long.csv",
     "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_no2.csv",
     "https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_no2_long.csv",
@@ -42,21 +42,21 @@
     if isinstance(df, pd.DataFrame):
         for col in df2.columns:
             if not df2[col].dtype == "string":
                 try:
                     df2[col] = df2[col].fillna(nastring)
                 except Exception:
                     pass
-                df2[col] = _conv_col(df2[col])
+                df2[col] = _conv_col(df2[col],errors=errors)
     else:
         try:
             df2 = df2.fillna(nastring)
         except Exception:
             pass
-        df2 = _conv_col(df2)
+        df2 = _conv_col(df2,errors=errors)
     df2 = df2.fillna(nastring).copy()
     return df2
 
 
 def pd_add_to_string():
     PandasObject.ds_to_string = ds_to_string
```

### Comparing `a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string/thirdparty.json` & `a_pandas_ex_df_to_string-0.14/a_pandas_ex_df_to_string/thirdparty.json`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_df_to_string-0.13/a_pandas_ex_df_to_string.egg-info/PKG-INFO` & `a_pandas_ex_df_to_string-0.14/a_pandas_ex_df_to_string.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a-pandas-ex-df-to-string
-Version: 0.13
+Version: 0.14
 Summary: Just a function to convert everything in Pandas DataFrames / Series to string
 Home-page: https://github.com/hansalemaos/a_pandas_ex_df_to_string
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: pandas,numpy,dataframe,series
 Classifier: Development Status :: 4 - Beta
```

### Comparing `a_pandas_ex_df_to_string-0.13/setup.py` & `a_pandas_ex_df_to_string-0.14/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.13'''
+VERSION = '''0.14'''
 DESCRIPTION = '''Just a function to convert everything in Pandas DataFrames / Series to string'''
 
 # Setting up
 setup(
     name="a_pandas_ex_df_to_string",
     version=VERSION,
     license='MIT',
```


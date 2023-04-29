# Comparing `tmp/plotguy-1.0.5.tar.gz` & `tmp/plotguy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotguy-1.0.5.tar", last modified: Wed Apr 19 08:47:57 2023, max compression
+gzip compressed data, was "plotguy-1.0.6.tar", last modified: Sat Apr 29 03:04:05 2023, max compression
```

## Comparing `plotguy-1.0.5.tar` & `plotguy-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-19 08:47:57.602859 plotguy-1.0.5/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-04-19 08:47:57.602313 plotguy-1.0.5/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.0.5/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-19 08:47:57.600389 plotguy-1.0.5/plotguy/
--rw-r--r--   0 cmw        (501) staff       (20)    25758 2023-04-19 08:44:51.000000 plotguy-1.0.5/plotguy/__init__.py
--rw-r--r--   0 cmw        (501) staff       (20)    16762 2023-02-28 03:04:57.000000 plotguy-1.0.5/plotguy/aggregate.py
--rw-r--r--   0 cmw        (501) staff       (20)    63231 2023-04-18 03:28:10.000000 plotguy-1.0.5/plotguy/components.py
--rw-r--r--   0 cmw        (501) staff       (20)    37694 2023-04-18 03:32:08.000000 plotguy-1.0.5/plotguy/equity_curves.py
--rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.0.5/plotguy/signals.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-19 08:47:57.601734 plotguy-1.0.5/plotguy.egg-info/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-04-19 08:47:57.000000 plotguy-1.0.5/plotguy.egg-info/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)      279 2023-04-19 08:47:57.000000 plotguy-1.0.5/plotguy.egg-info/SOURCES.txt
--rw-r--r--   0 cmw        (501) staff       (20)        1 2023-04-19 08:47:57.000000 plotguy-1.0.5/plotguy.egg-info/dependency_links.txt
--rw-r--r--   0 cmw        (501) staff       (20)      124 2023-04-19 08:47:57.000000 plotguy-1.0.5/plotguy.egg-info/requires.txt
--rw-r--r--   0 cmw        (501) staff       (20)        8 2023-04-19 08:47:57.000000 plotguy-1.0.5/plotguy.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-04-19 08:47:57.603075 plotguy-1.0.5/setup.cfg
--rw-r--r--   0 cmw        (501) staff       (20)      814 2023-04-19 08:45:56.000000 plotguy-1.0.5/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-29 03:04:05.431820 plotguy-1.0.6/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-04-29 03:04:05.431668 plotguy-1.0.6/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.0.6/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-29 03:04:05.430703 plotguy-1.0.6/plotguy/
+-rw-r--r--   0 cmw        (501) staff       (20)    25461 2023-04-29 03:02:55.000000 plotguy-1.0.6/plotguy/__init__.py
+-rw-r--r--   0 cmw        (501) staff       (20)    16762 2023-02-28 03:04:57.000000 plotguy-1.0.6/plotguy/aggregate.py
+-rw-r--r--   0 cmw        (501) staff       (20)    63231 2023-04-18 03:28:10.000000 plotguy-1.0.6/plotguy/components.py
+-rw-r--r--   0 cmw        (501) staff       (20)    37694 2023-04-18 03:32:08.000000 plotguy-1.0.6/plotguy/equity_curves.py
+-rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.0.6/plotguy/signals.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-29 03:04:05.431481 plotguy-1.0.6/plotguy.egg-info/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-04-29 03:04:05.000000 plotguy-1.0.6/plotguy.egg-info/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)      279 2023-04-29 03:04:05.000000 plotguy-1.0.6/plotguy.egg-info/SOURCES.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        1 2023-04-29 03:04:05.000000 plotguy-1.0.6/plotguy.egg-info/dependency_links.txt
+-rw-r--r--   0 cmw        (501) staff       (20)      124 2023-04-29 03:04:05.000000 plotguy-1.0.6/plotguy.egg-info/requires.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        8 2023-04-29 03:04:05.000000 plotguy-1.0.6/plotguy.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-04-29 03:04:05.431871 plotguy-1.0.6/setup.cfg
+-rw-r--r--   0 cmw        (501) staff       (20)      814 2023-04-29 03:03:27.000000 plotguy-1.0.6/setup.py
```

### Comparing `plotguy-1.0.5/plotguy/__init__.py` & `plotguy-1.0.6/plotguy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import itertools
 import multiprocessing as mp
 import zlib
 import requests
 from bs4 import BeautifulSoup
 import pandas as pd
 import numpy as np
+# import polars as pl
 
 from .equity_curves import *
 from .signals import *
 from .aggregate import *
 
 def multi_process(function, parameters, number_of_core=8):
     pool = mp.Pool(processes=number_of_core)
@@ -45,14 +46,15 @@
     return save_name
 
 
 def path_reference_code(save_name):
     reference_code = str(zlib.crc32(bytes(save_name, 'UTF-8')))[:6]
     return reference_code
 
+
 def generate_filepath(para_combination, folder=''):
 
     file_format = para_combination['file_format']
 
     if not file_format == 'parquet':
         file_format = 'csv'
 
@@ -62,25 +64,35 @@
     save_name = reference_code + '_' + save_name[:-1]     # position -1 to avoid '&' at the end
 
     output_folder = para_combination['output_folder']
     filepath = os.path.join(folder,output_folder, f'{save_name}.{file_format}')
 
     return filepath
 
-# def read_data(path):
-
-
 
 def mp_cal_performance(tuple_data):
     para_combination = tuple_data[0]
     manager_list = tuple_data[1]
 
     result = cal_performance(para_combination)
-    index = para_combination['reference_index']
-    manager_list.append((index,result))
+
+    # new
+    para_df_dict = {}
+
+    para_df_dict['reference_code'] = path_reference_code(filename_only(para_combination))
+    para_df_dict['reference_index'] = para_combination['reference_index']
+
+    keys_to_keep = para_combination['para_dict'].keys()
+    para_df_dict.update({k: v for k, v in para_combination.items() if k in keys_to_keep})
+    para_df_dict.update(result)
+    manager_list.append(para_df_dict)
+
+
+def reference_code_apply(row):
+    return path_reference_code(filename_only(reference_code_apply.all_para_combination[row.reference_index]))
 
 
 def generate_backtest_result(all_para_combination, number_of_core=8, risk_free_rate='geometric_mean'):
     ## Get / Calculate risk free rate
     start_date = all_para_combination[0]['start_date']
     end_date = all_para_combination[0]['end_date']
 
@@ -96,52 +108,26 @@
             risk_free_rate = 2  # if network error, set rate to 2 %
             print('Network error. Risk free rate: {:.2f} %'.format(risk_free_rate))
     else:
         print('Risk free rate: {:.2f} %'.format(risk_free_rate))
 
     print('Backtest result is loading. Please wait patiently.')
 
-
     manager_list = mp.Manager().list()# To save the result with index number
 
     cal_performance_list = []
     for para_combination in all_para_combination:
         para_combination['risk_free_rate'] = risk_free_rate
         cal_performance_list.append((para_combination, manager_list))
 
     pool = mp.Pool(processes=number_of_core)
     pool.map(mp_cal_performance, cal_performance_list)
     pool.close()
 
-    df_backtest_result = pd.DataFrame()
-    df_backtest_result['reference_code'] = np.NaN
-    df_backtest_result['reference_index'] = np.NaN
-    para_keys = all_para_combination[0]['para_dict'].keys()
-    for key in para_keys:
-        df_backtest_result[key] = np.NaN
-    for key in manager_list[0][1].keys():
-        df_backtest_result[key] = np.NaN
-
-    for mp_data in manager_list:
-        reference_index = mp_data[0]
-        result_dict = mp_data[1]
-        para_combination = all_para_combination[reference_index]
-        save_name = filename_only(para_combination)
-        reference_code = path_reference_code(save_name)
-        df_backtest_result.at[reference_index, 'reference_code'] = reference_code
-        df_backtest_result.at[reference_index, 'reference_index'] = reference_index
-        for key in para_keys:
-            df_backtest_result.at[reference_index, key] = para_combination[key]
-        for key in result_dict:
-            df_backtest_result.at[reference_index, key] = result_dict[key]
-
-    # print(df_backtest_result)
-    df_backtest_result['reference_index'] = df_backtest_result['reference_index'].astype(int)
-    df_backtest_result.to_csv('backtest_result.csv')
-
+    pd.DataFrame(list(manager_list)).to_csv('backtest_result.csv')
 
 
 def plot_signal_analysis(py_filename, output_folder, start_date, end_date, para_dict, signal_settings):
 
     app = signals.Signals(py_filename, output_folder, start_date, end_date, para_dict, generate_filepath, signal_settings)
 
     return app
@@ -292,16 +278,22 @@
     code = para_combination['code']
     lot_size = lot_size_dict[code]
 
     intraday = para_combination['intraday']
     freq = para_combination['freq']
     file_format = para_combination['file_format']
     sec_profile = para_combination['sec_profile']
-    margin_req = sec_profile['margin_req']
-    multiplier = sec_profile['multiplier']
+
+
+    if sectype == 'FUT':
+        margin_req = sec_profile['margin_req']
+        multiplier = sec_profile['multiplier']
+    elif sectype == 'STK':
+        multiplier = 1
+
 
     # Read backtest data
     save_path = generate_filepath(para_combination=para_combination,folder=folder)
     if file_format == 'parquet':
         df_backtest = pd.read_parquet(save_path) # Daraframe that may not be daily
         ### parquet specific, All backtest force to treart as summary, # ie filter action only
         # df_backtest = df_backtest.loc[df_backtest['action'] != ''].copy()
@@ -477,14 +469,15 @@
 
     return df_daily
 
 
 
 
 def cal_performance(para_combination):
+
     start_date = para_combination['start_date']
     end_date = para_combination['end_date']
 
     risk_free_rate = para_combination['risk_free_rate']
 
     intraday = para_combination['intraday']
     summary_mode = para_combination['summary_mode']
@@ -503,14 +496,22 @@
         df_backtest['date'] = pd.to_datetime(df_backtest['date'], format='%Y-%m-%d')
         df_backtest = df_backtest.loc[(df_backtest['date'] >= start_date) & (df_backtest['date'] <= end_date)]
         df_backtest = df_backtest.reset_index(drop=True)  # Reset Index
         df_daily = df_backtest.copy()
 
     df = df_daily.copy()
 
+
+
+    # end_time = time.time()
+    # elapsed_time = end_time - start_time
+    # print("Resample: {:.2f} seconds".format(elapsed_time))
+
+
+
     # Deter if equity_value unchange = no tade
     equity_value_column = df['equity_value'].to_numpy()
     no_trade = (equity_value_column[0] == equity_value_column).all()
 
     result_dict = {}
 
     # Determine years at the beginning
@@ -629,14 +630,20 @@
             else: # no trade
                 result_dict[f'{year}_return'] = '-----'
 
             first_equity_value = last_equity_value
 
 
 
+    # end_time = time.time()
+    # elapsed_time = end_time - start_time
+    # print("No Trade: {:.2f} seconds".format(elapsed_time))
+
+
+
     result_dict['risk_free_rate'] = risk_free_rate
 
     # BaH Performance
     bah_net_return, holding_period_day, bah_return, \
     bah_annualized_return, bah_annualized_std, bah_annualized_sr = calculate_sharp_ratio(df, 'close',
                                                                                          risk_free_rate)
     initial_capital = df.loc[df.index[0], 'equity_value']
```

### Comparing `plotguy-1.0.5/plotguy/aggregate.py` & `plotguy-1.0.6/plotguy/aggregate.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.0.5/plotguy/components.py` & `plotguy-1.0.6/plotguy/components.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.0.5/plotguy/equity_curves.py` & `plotguy-1.0.6/plotguy/equity_curves.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.0.5/plotguy/signals.py` & `plotguy-1.0.6/plotguy/signals.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.0.5/setup.py` & `plotguy-1.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plotguy",
-    version="1.0.5",
+    version="1.0.6",
     author="Plotguy Team",
     author_email="plotguy.info@gmail.com",
     description="Plotguy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[         
         'pandas>=1.5.2',
```


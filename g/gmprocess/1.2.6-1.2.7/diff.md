# Comparing `tmp/gmprocess-1.2.6.tar.gz` & `tmp/gmprocess-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmprocess-1.2.6.tar", last modified: Sat Mar 18 15:16:39 2023, max compression
+gzip compressed data, was "gmprocess-1.2.7.tar", last modified: Fri Apr 28 22:48:13 2023, max compression
```

## Comparing `gmprocess-1.2.6.tar` & `gmprocess-1.2.7.tar`

### file list

```diff
@@ -1,288 +1,289 @@
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.304593 gmprocess-1.2.6/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1660 2023-03-18 15:15:05.000000 gmprocess-1.2.6/LICENSE.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      114 2023-03-18 15:15:05.000000 gmprocess-1.2.6/MANIFEST.in
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     4167 2023-03-18 15:16:39.304593 gmprocess-1.2.6/PKG-INFO
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1582 2023-03-18 15:15:05.000000 gmprocess-1.2.6/README.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2376 2023-03-18 15:15:05.000000 gmprocess-1.2.6/pyproject.toml
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2023-03-18 15:16:39.304593 gmprocess-1.2.6/setup.cfg
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      175 2023-03-18 15:15:05.000000 gmprocess-1.2.6/setup.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.236593 gmprocess-1.2.6/src/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.244593 gmprocess-1.2.6/src/gmprocess/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/__init__.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.248593 gmprocess-1.2.6/src/gmprocess/apps/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/apps/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14621 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/apps/gmrecords.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.248593 gmprocess-1.2.6/src/gmprocess/bin/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/bin/__init__.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8142 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/bin/cwb_gather.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     5144 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/bin/gmconvert.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8917 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/bin/gminfo.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      152 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/bin/gmrecords.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     5104 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/bin/gmworkspace.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     2002 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/bin/list_metrics.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.248593 gmprocess-1.2.6/src/gmprocess/core/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/core/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    19155 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/core/stationstream.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    51521 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/core/stationtrace.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5481 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/core/streamarray.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    31952 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/core/streamcollection.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.252593 gmprocess-1.2.6/src/gmprocess/data/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      616 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/data/CESMD_NGA_ids.csv
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    41885 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/data/GDMSstations.json
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/data/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    19096 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/data/config_production.yml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    25699 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/data/config_test.yml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    39424 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/data/cosmos_table10.xls
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    32768 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/data/cosmos_table4.xls
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.240593 gmprocess-1.2.6/src/gmprocess/data/demo/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.240593 gmprocess-1.2.6/src/gmprocess/data/demo/ci38457511/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.256593 gmprocess-1.2.6/src/gmprocess/data/demo/ci38457511/raw/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   989427 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/data/demo/ci38457511/raw/CICCC.RAW
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   896593 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/data/demo/ci38457511/raw/CICLC.v1
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   994737 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/data/demo/ci38457511/raw/CITOW2.RAW
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    55506 2023-03-18 15:15:05.000000 gmprocess-1.2.6/src/gmprocess/data/fdsn_codes.csv
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.256593 gmprocess-1.2.6/src/gmprocess/data/lme/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999) 11719610 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/lme/SA_rotd50.0_2020.03.31.csv
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      427 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/modules.yml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   737944 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nga_w2_selected.csv
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.268593 gmprocess-1.2.6/src/gmprocess/data/nn_clipping/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      409 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_clipping/bias_1.csv
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       26 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_clipping/bias_output.csv
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       26 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_clipping/masterF.txt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2032 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_clipping/weight_1.csv
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      408 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_clipping/weight_output.csv
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.240593 gmprocess-1.2.6/src/gmprocess/data/nn_qa/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.268593 gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8152 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/M.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      304 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/bias_1.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      406 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/bias_2.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)       43 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/bias_output.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     5251 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/final_training.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)       35 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/masterF.txt
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    11468 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/model_3.txt
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    12981 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/model_5.txt
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      767 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/mu_sigma.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     6135 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/weight_1.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     6041 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/weight_2.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      791 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/weight_output.csv
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.272593 gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8171 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/M.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      293 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/bias_1.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      316 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/bias_2.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)       42 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/bias_output.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     3569 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/final_training.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)       35 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/masterF.txt
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    10524 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/model_0.txt
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      770 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/mu_sigma.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     6037 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/weight_1.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     4418 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/weight_2.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      596 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/weight_output.csv
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2233 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/picker.yml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11182 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/station_coordinates.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    79189 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/data/usgs_ids_nga_and_srcmod_cross_reference.xlsx
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.272593 gmprocess-1.2.6/src/gmprocess/io/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/__init__.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.276593 gmprocess-1.2.6/src/gmprocess/io/asdf/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/asdf/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2255 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/asdf/core.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    62330 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/asdf/stream_workspace.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2514 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/asdf/utils.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.276593 gmprocess-1.2.6/src/gmprocess/io/bhrc/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/bhrc/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7790 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/bhrc/core.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.276593 gmprocess-1.2.6/src/gmprocess/io/cosmos/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/cosmos/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13189 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/cosmos/cesmd_fetcher.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    17913 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/cosmos/cesmd_search.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    28891 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/cosmos/core.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    31504 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/cosmos/cosmos_writer.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4117 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/cosmos/data_structures.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.276593 gmprocess-1.2.6/src/gmprocess/io/cwb/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/cwb/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9341 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/cwb/core.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.276593 gmprocess-1.2.6/src/gmprocess/io/dmg/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/dmg/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    32782 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/dmg/core.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.276593 gmprocess-1.2.6/src/gmprocess/io/esm/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/esm/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6486 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/esm/core.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4086 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/fetcher.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.276593 gmprocess-1.2.6/src/gmprocess/io/geonet/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/geonet/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13209 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/geonet/core.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4736 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/global_fetcher.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.280593 gmprocess-1.2.6/src/gmprocess/io/knet/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/knet/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6831 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/knet/core.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    15155 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/knet/knet_fetcher.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2014 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/nga.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.280593 gmprocess-1.2.6/src/gmprocess/io/nsmn/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/nsmn/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6209 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/nsmn/core.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.280593 gmprocess-1.2.6/src/gmprocess/io/obspy/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/obspy/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9206 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/obspy/core.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    12214 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/obspy/fdsn_fetcher.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5571 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/read.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2594 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/read_directory.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.280593 gmprocess-1.2.6/src/gmprocess/io/renadic/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/renadic/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9248 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/renadic/core.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9896 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/report.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2046 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/seedname.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.280593 gmprocess-1.2.6/src/gmprocess/io/smc/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/smc/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    18236 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/smc/core.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8478 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/stream.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.280593 gmprocess-1.2.6/src/gmprocess/io/unam/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/unam/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    12482 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/unam/core.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.280593 gmprocess-1.2.6/src/gmprocess/io/usc/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/usc/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    17339 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/usc/core.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5748 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/io/utils.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.280593 gmprocess-1.2.6/src/gmprocess/metrics/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/__init__.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.284593 gmprocess-1.2.6/src/gmprocess/metrics/combination/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/combination/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1466 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/combination/arithmetic_mean.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2579 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/combination/combination.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1512 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/combination/geometric_mean.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      888 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/combination/greater_of_two_horizontals.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      743 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/combination/null_combination.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1572 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/combination/quadratic_mean.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      129 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/exception.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      691 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/gather.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.284593 gmprocess-1.2.6/src/gmprocess/metrics/imc/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imc/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1253 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imc/arithmetic_mean.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1162 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imc/channels.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1249 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imc/geometric_mean.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1114 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imc/gmrotd.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1243 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imc/greater_of_two_horizontals.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1550 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imc/imc.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1405 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imc/quadratic_mean.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1201 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imc/radial_transverse.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1300 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imc/rotd.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.288593 gmprocess-1.2.6/src/gmprocess/metrics/imt/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imt/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1128 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imt/arias.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1320 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imt/duration.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1041 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imt/fas.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1375 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imt/imt.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1035 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imt/pga.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1031 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imt/pgv.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      970 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imt/sa.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1340 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/imt/sorted_duration.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    33485 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/metrics_controller.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.288593 gmprocess-1.2.6/src/gmprocess/metrics/reduction/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/reduction/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2911 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/reduction/arias.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2737 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/reduction/duration.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2947 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/reduction/max.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1752 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/reduction/null_reduction.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3074 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/reduction/percentile.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1233 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/reduction/reduction.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3458 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/reduction/smooth_select.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2892 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/reduction/sorted_duration.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.288593 gmprocess-1.2.6/src/gmprocess/metrics/rotation/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/rotation/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1207 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/rotation/gmrotd.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      605 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/rotation/null_rotation.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3573 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/rotation/radial_transverse.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7993 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/rotation/rotation.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1461 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/rotation/rotd.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    31152 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/station_summary.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.292593 gmprocess-1.2.6/src/gmprocess/metrics/transform/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/transform/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2744 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/transform/differentiate.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3594 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/transform/fft.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2038 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/transform/integrate.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1008 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/transform/null_transform.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6571 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/transform/oscillator.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2486 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/metrics/transform/transform.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.296593 gmprocess-1.2.6/src/gmprocess/subcommands/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      284 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/arg_dicts.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3579 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/assemble.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4368 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/autoprocess.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3688 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/autoshakemap.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7512 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/base.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4687 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/clean.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5372 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/compute_station_metrics.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5265 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/compute_waveform_metrics.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5189 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/config.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1312 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/download.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4911 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/export_failure_tables.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2280 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/export_gmpacket.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6554 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/export_metric_tables.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2749 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/export_provenance_tables.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2919 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/export_shakemap.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4449 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/generate_regression_plot.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5226 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/generate_report.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2761 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/generate_station_maps.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2365 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/import_data.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1485 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/init.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1406 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/lazy_loader.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5002 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/process_waveforms.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1960 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/processing_steps.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    15355 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/subcommands/projects.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.300593 gmprocess-1.2.6/src/gmprocess/utils/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      746 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/args.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3404 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/assemble_utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7007 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/base_utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10273 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/config.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3316 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/constants.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6652 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/download_utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7242 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/event.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11690 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/export_gmpacket_utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13378 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/export_shakemap_utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3302 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/logging.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      375 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/misc.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      783 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/models.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    25313 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/plot.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2301 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/prompt.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    12750 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/report_utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      567 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/rupture_utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6174 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/tables.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2011 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/utils/test_utils.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.304593 gmprocess-1.2.6/src/gmprocess/waveform_processing/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4479 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/adjust_highpass.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3127 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/adjust_highpass_ridder.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1793 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/baseline_correction.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.304593 gmprocess-1.2.6/src/gmprocess/waveform_processing/clipping/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2412 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/clipping/clip_detection.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7409 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/clipping/clipping_ann.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2345 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/clipping/clipping_check.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    15086 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/clipping/histogram.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3540 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/clipping/jerk.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2987 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/clipping/max_amp.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3222 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/clipping/ping.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4401 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/clipping/std_dev.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10608 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/corner_frequencies.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2322 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/detrend.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3449 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/fft.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4220 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/filtering.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8479 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/instrument_response.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1101 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/integrate.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    30822 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/nn_quality_assurance.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    26308 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/phase.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7176 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/pretesting.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     6545 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/processing.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1235 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/processing_step.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1072 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/resample.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3373 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/sanity_checks.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10011 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/snr.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    20415 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/spectrum.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1561 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/taper.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    19092 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/windows.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2027 2023-03-18 15:15:06.000000 gmprocess-1.2.6/src/gmprocess/waveform_processing/zero_crossings.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-03-18 15:16:39.244593 gmprocess-1.2.6/src/gmprocess.egg-info/
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     4167 2023-03-18 15:16:39.000000 gmprocess-1.2.6/src/gmprocess.egg-info/PKG-INFO
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     9759 2023-03-18 15:16:39.000000 gmprocess-1.2.6/src/gmprocess.egg-info/SOURCES.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2023-03-18 15:16:39.000000 gmprocess-1.2.6/src/gmprocess.egg-info/dependency_links.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)      270 2023-03-18 15:16:39.000000 gmprocess-1.2.6/src/gmprocess.egg-info/entry_points.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)      735 2023-03-18 15:16:39.000000 gmprocess-1.2.6/src/gmprocess.egg-info/requires.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       10 2023-03-18 15:16:39.000000 gmprocess-1.2.6/src/gmprocess.egg-info/top_level.txt
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.063561 gmprocess-1.2.7/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1660 2023-04-28 22:46:27.000000 gmprocess-1.2.7/LICENSE.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      114 2023-04-28 22:46:27.000000 gmprocess-1.2.7/MANIFEST.in
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     4167 2023-04-28 22:48:13.059561 gmprocess-1.2.7/PKG-INFO
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1582 2023-04-28 22:46:27.000000 gmprocess-1.2.7/README.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2452 2023-04-28 22:46:27.000000 gmprocess-1.2.7/pyproject.toml
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2023-04-28 22:48:13.063561 gmprocess-1.2.7/setup.cfg
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      175 2023-04-28 22:46:27.000000 gmprocess-1.2.7/setup.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:12.995561 gmprocess-1.2.7/src/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.003561 gmprocess-1.2.7/src/gmprocess/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/__init__.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.003561 gmprocess-1.2.7/src/gmprocess/apps/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/apps/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14621 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/apps/gmrecords.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.003561 gmprocess-1.2.7/src/gmprocess/bin/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/bin/__init__.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8142 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/bin/cwb_gather.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5432 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/bin/fix_inventory.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     5144 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/bin/gmconvert.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8792 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/bin/gminfo.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      152 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/bin/gmrecords.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     5104 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/bin/gmworkspace.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     2002 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/bin/list_metrics.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.007561 gmprocess-1.2.7/src/gmprocess/core/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/core/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    19040 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/core/stationstream.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    51521 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/core/stationtrace.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5481 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/core/streamarray.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    31952 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/core/streamcollection.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.011561 gmprocess-1.2.7/src/gmprocess/data/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      616 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/CESMD_NGA_ids.csv
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    41885 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/GDMSstations.json
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/data/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    19115 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/config_production.yml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    25718 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/config_test.yml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    39424 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/cosmos_table10.xls
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    32768 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/cosmos_table4.xls
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:12.995561 gmprocess-1.2.7/src/gmprocess/data/demo/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:12.995561 gmprocess-1.2.7/src/gmprocess/data/demo/ci38457511/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.011561 gmprocess-1.2.7/src/gmprocess/data/demo/ci38457511/raw/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   989427 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/demo/ci38457511/raw/CICCC.RAW
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   896593 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/demo/ci38457511/raw/CICLC.v1
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   994737 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/demo/ci38457511/raw/CITOW2.RAW
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    55506 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/fdsn_codes.csv
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.011561 gmprocess-1.2.7/src/gmprocess/data/lme/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999) 11719610 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/lme/SA_rotd50.0_2020.03.31.csv
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      427 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/modules.yml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   737944 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nga_w2_selected.csv
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.023561 gmprocess-1.2.7/src/gmprocess/data/nn_clipping/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      409 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_clipping/bias_1.csv
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       26 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_clipping/bias_output.csv
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       26 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_clipping/masterF.txt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2032 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_clipping/weight_1.csv
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      408 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_clipping/weight_output.csv
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:12.999561 gmprocess-1.2.7/src/gmprocess/data/nn_qa/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.027561 gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8152 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/M.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      304 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/bias_1.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      406 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/bias_2.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)       43 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/bias_output.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     5251 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/final_training.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)       35 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/masterF.txt
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    11468 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/model_3.txt
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    12981 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/model_5.txt
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      767 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/mu_sigma.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     6135 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/weight_1.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     6041 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/weight_2.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      791 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/weight_output.csv
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.027561 gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8171 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/M.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      293 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/bias_1.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      316 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/bias_2.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)       42 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/bias_output.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     3569 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/final_training.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)       35 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/masterF.txt
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    10524 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/model_0.txt
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      770 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/mu_sigma.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     6037 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/weight_1.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     4418 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/weight_2.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      596 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/weight_output.csv
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2233 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/picker.yml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11182 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/station_coordinates.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    79189 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/data/usgs_ids_nga_and_srcmod_cross_reference.xlsx
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.031561 gmprocess-1.2.7/src/gmprocess/io/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/io/__init__.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.031561 gmprocess-1.2.7/src/gmprocess/io/asdf/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/io/asdf/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2255 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/asdf/core.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    65765 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/asdf/stream_workspace.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2514 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/asdf/utils.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.031561 gmprocess-1.2.7/src/gmprocess/io/bhrc/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/io/bhrc/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7790 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/bhrc/core.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.031561 gmprocess-1.2.7/src/gmprocess/io/cosmos/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/io/cosmos/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13189 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/cosmos/cesmd_fetcher.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    17913 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/cosmos/cesmd_search.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    28891 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/cosmos/core.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    31504 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/cosmos/cosmos_writer.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4117 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/cosmos/data_structures.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.035561 gmprocess-1.2.7/src/gmprocess/io/cwb/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/io/cwb/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9341 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/cwb/core.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.035561 gmprocess-1.2.7/src/gmprocess/io/dmg/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/io/dmg/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    32782 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/dmg/core.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.035561 gmprocess-1.2.7/src/gmprocess/io/esm/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/io/esm/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6486 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/esm/core.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4086 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/fetcher.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.035561 gmprocess-1.2.7/src/gmprocess/io/geonet/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/io/geonet/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13209 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/geonet/core.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4736 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/global_fetcher.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.035561 gmprocess-1.2.7/src/gmprocess/io/knet/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/io/knet/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6831 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/knet/core.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    15155 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/knet/knet_fetcher.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2014 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/nga.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.035561 gmprocess-1.2.7/src/gmprocess/io/nsmn/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/io/nsmn/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6209 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/nsmn/core.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.035561 gmprocess-1.2.7/src/gmprocess/io/obspy/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/io/obspy/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9206 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/obspy/core.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    12214 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/obspy/fdsn_fetcher.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5571 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/read.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2594 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/read_directory.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.035561 gmprocess-1.2.7/src/gmprocess/io/renadic/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/io/renadic/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9248 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/renadic/core.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9896 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/report.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2046 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/seedname.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.035561 gmprocess-1.2.7/src/gmprocess/io/smc/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/io/smc/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    18236 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/smc/core.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8478 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/stream.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.035561 gmprocess-1.2.7/src/gmprocess/io/unam/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/io/unam/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    12482 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/unam/core.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.039561 gmprocess-1.2.7/src/gmprocess/io/usc/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/io/usc/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    17339 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/usc/core.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5748 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/io/utils.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.039561 gmprocess-1.2.7/src/gmprocess/metrics/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/metrics/__init__.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.039561 gmprocess-1.2.7/src/gmprocess/metrics/combination/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/metrics/combination/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1466 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/combination/arithmetic_mean.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2579 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/combination/combination.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1512 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/combination/geometric_mean.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      888 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/combination/greater_of_two_horizontals.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      743 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/combination/null_combination.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1572 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/combination/quadratic_mean.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      129 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/exception.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      691 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/gather.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.043561 gmprocess-1.2.7/src/gmprocess/metrics/imc/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/metrics/imc/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1253 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/imc/arithmetic_mean.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1162 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/imc/channels.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1249 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/imc/geometric_mean.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1114 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/imc/gmrotd.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1243 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/imc/greater_of_two_horizontals.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1550 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/imc/imc.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1405 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/imc/quadratic_mean.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1201 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/imc/radial_transverse.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1300 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/imc/rotd.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.043561 gmprocess-1.2.7/src/gmprocess/metrics/imt/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/metrics/imt/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1128 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/imt/arias.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1320 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/imt/duration.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1041 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/imt/fas.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1375 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/imt/imt.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1035 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/imt/pga.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1031 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/imt/pgv.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      970 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/imt/sa.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1340 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/imt/sorted_duration.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    33485 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/metrics_controller.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.043561 gmprocess-1.2.7/src/gmprocess/metrics/reduction/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/metrics/reduction/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2911 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/reduction/arias.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2737 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/reduction/duration.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2947 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/reduction/max.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1752 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/reduction/null_reduction.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3074 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/reduction/percentile.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1233 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/reduction/reduction.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3458 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/reduction/smooth_select.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2892 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/reduction/sorted_duration.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.047561 gmprocess-1.2.7/src/gmprocess/metrics/rotation/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/metrics/rotation/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1207 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/rotation/gmrotd.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      605 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/rotation/null_rotation.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3573 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/rotation/radial_transverse.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7993 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/rotation/rotation.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1461 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/rotation/rotd.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    31152 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/station_summary.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.047561 gmprocess-1.2.7/src/gmprocess/metrics/transform/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/metrics/transform/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2744 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/transform/differentiate.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3594 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/transform/fft.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2038 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/transform/integrate.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1008 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/transform/null_transform.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6571 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/transform/oscillator.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2486 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/metrics/transform/transform.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.051561 gmprocess-1.2.7/src/gmprocess/subcommands/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/subcommands/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      284 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/arg_dicts.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3579 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/assemble.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4368 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/autoprocess.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3688 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/autoshakemap.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7512 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/base.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4687 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/clean.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5372 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/compute_station_metrics.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5265 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/compute_waveform_metrics.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5189 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/config.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1312 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/download.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4911 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/export_failure_tables.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2273 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/export_gmpacket.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6554 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/export_metric_tables.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2749 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/export_provenance_tables.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2919 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/export_shakemap.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4545 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/generate_regression_plot.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5226 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/generate_report.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2761 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/generate_station_maps.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2365 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/import_data.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1485 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/init.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1406 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/lazy_loader.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5002 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/process_waveforms.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1960 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/processing_steps.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    16160 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/subcommands/projects.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.055561 gmprocess-1.2.7/src/gmprocess/utils/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/utils/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      746 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/utils/args.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3404 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/utils/assemble_utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7007 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/utils/base_utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10235 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/utils/config.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3317 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/utils/constants.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6652 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/utils/download_utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7242 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/utils/event.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11772 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/utils/export_gmpacket_utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13378 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/utils/export_shakemap_utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3302 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/utils/logging.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      375 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/utils/misc.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      783 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/utils/models.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    25391 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/utils/plot.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2301 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/utils/prompt.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    12750 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/utils/report_utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      567 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/utils/rupture_utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6174 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/utils/tables.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2011 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/utils/test_utils.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.059561 gmprocess-1.2.7/src/gmprocess/waveform_processing/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:46:28.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4479 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/adjust_highpass.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3127 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/adjust_highpass_ridder.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1793 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/baseline_correction.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.059561 gmprocess-1.2.7/src/gmprocess/waveform_processing/clipping/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2412 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/clipping/clip_detection.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7409 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/clipping/clipping_ann.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2345 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/clipping/clipping_check.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    15086 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/clipping/histogram.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3540 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/clipping/jerk.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2987 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/clipping/max_amp.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3222 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/clipping/ping.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4401 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/clipping/std_dev.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10608 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/corner_frequencies.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2322 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/detrend.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3449 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/fft.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4220 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/filtering.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8479 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/instrument_response.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1101 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/integrate.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    30822 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/nn_quality_assurance.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    26308 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/phase.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7176 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/pretesting.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     6545 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/processing.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1235 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/processing_step.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1072 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/resample.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3373 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/sanity_checks.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10011 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/snr.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    20415 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/spectrum.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1561 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/taper.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    19499 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/windows.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2027 2023-04-28 22:46:27.000000 gmprocess-1.2.7/src/gmprocess/waveform_processing/zero_crossings.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-04-28 22:48:13.003561 gmprocess-1.2.7/src/gmprocess.egg-info/
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     4167 2023-04-28 22:48:12.000000 gmprocess-1.2.7/src/gmprocess.egg-info/PKG-INFO
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     9794 2023-04-28 22:48:12.000000 gmprocess-1.2.7/src/gmprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2023-04-28 22:48:12.000000 gmprocess-1.2.7/src/gmprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      319 2023-04-28 22:48:12.000000 gmprocess-1.2.7/src/gmprocess.egg-info/entry_points.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      753 2023-04-28 22:48:12.000000 gmprocess-1.2.7/src/gmprocess.egg-info/requires.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       10 2023-04-28 22:48:12.000000 gmprocess-1.2.7/src/gmprocess.egg-info/top_level.txt
```

### Comparing `gmprocess-1.2.6/LICENSE.md` & `gmprocess-1.2.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/PKG-INFO` & `gmprocess-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmprocess
-Version: 1.2.6
+Version: 1.2.7
 Summary: USGS Automated Ground Motion Processing Software
 Author-email: Eric Thompson <emthompsone@usgs.gov>, Mike Hearne <mhearne@usgs.gov>, Brad Aagaard <baagaard@usgs.gov>, Bruce Worden <cbworden@contractor.usgs.gov>, John Rekoske <jrekoske@ucsd.edu>, Heather Hunsinger <hhunsinger@usgs.gov>, Gabe Ferragut <gferragut@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United States
         because it contains materials that originally came from the United States Geological Survey,
```

### Comparing `gmprocess-1.2.6/README.md` & `gmprocess-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/pyproject.toml` & `gmprocess-1.2.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     "pyasdf>=0.7",
     "requests>=2.23",
     "ruamel.yaml>=0.17.16",
     "schema>=0.7",
     "scipy>=1.7",
     "setuptools-scm>=6.3.2",
     "statsmodels>=0.12.2",
+    "usgs-strec>=2.2.6",
     "xlrd>=2.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "build>=0.7.0",
     "black>=21",
@@ -82,14 +83,15 @@
 [project.scripts]
 gmconvert = "gmprocess.bin.gmconvert:main"
 gminfo = "gmprocess.bin.gminfo:main"
 gmrecords = "gmprocess.bin.gmrecords:main"
 gmworkspace = "gmprocess.bin.gmworkspace:main"
 list_metrics = "gmprocess.bin.list_metrics:main"
 cwb_gather = "gmprocess.bin.cwb_gather:main"
+fix_inventory = "gmprocess.bin.fix_inventory:main"
 
 [build-system]
 requires = [
   "setuptools>=42",
   "wheel",
   "setuptools_scm[toml]>=3.4",
   "numpy",
```

### Comparing `gmprocess-1.2.6/src/gmprocess/apps/gmrecords.py` & `gmprocess-1.2.7/src/gmprocess/apps/gmrecords.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/bin/cwb_gather.py` & `gmprocess-1.2.7/src/gmprocess/bin/cwb_gather.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/bin/gmconvert.py` & `gmprocess-1.2.7/src/gmprocess/bin/gmconvert.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/bin/gminfo.py` & `gmprocess-1.2.7/src/gmprocess/bin/gminfo.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,16 +33,14 @@
     "Station",
     "Channel",
     "Sampling Rate (Hz)",
     "Latitude",
     "Longitude",
 ]
 
-ERROR_COLUMNS = ["Filename", "Error"]
-
 REV_PROCESS_LEVELS = {
     "raw counts": "V0",
     "uncorrected physical units": "V1",
     "corrected physical units": "V2",
     "derived time series": "V3",
 }
 
@@ -67,33 +65,34 @@
         row["Longitude"] = trace.stats.coordinates["longitude"]
         rows.append(row.copy())
     df = pd.DataFrame(rows)
     return df
 
 
 def render_concise(files, save=False):
-    errors = pd.DataFrame(columns=ERROR_COLUMNS)
     df = pd.DataFrame(columns=COLUMNS, index=None)
     folders = []
+    error_rows = []
     for path in files:
         fpath = path.parent
         if fpath not in folders:
             sys.stderr.write(f"Parsing files from subfolder {fpath}...\n")
             folders.append(fpath)
         try:
             streams = readmod.read_data(str(path))
             for stream in streams:
                 tdf = get_dataframe(path, stream)
                 df = pd.concat([df, tdf], axis=0)
         except BaseException as e:
-            row = pd.Series(index=ERROR_COLUMNS)
+            row = {}
             row["Filename"] = str(path)
             row["Error"] = str(e)
-            errors = errors.append(row, ignore_index=True)
+            error_rows.append(row)
             continue
+    errors = pd.DataFrame(error_rows)
 
     # organize dataframe by network, station, and channel
     df = df.sort_values(["Network", "Station", "Channel"])
     if not save:
         print(df.to_string(index=False))
 
     return (df, errors)
@@ -110,15 +109,15 @@
         df = None
 
     return (df, errors)
 
 
 def render_verbose(files):
     config = confmod.get_config()
-    errors = pd.DataFrame(columns=ERROR_COLUMNS)
+    error_rows = []
     for fname in files:
         try:
             fmt = readmod._get_format(fname, config)
             stream = readmod.read_data(fname, config)[0]
             stats = stream[0].stats
             tpl = (
                 stats["coordinates"]["latitude"],
@@ -151,19 +150,20 @@
                 channel["Peak Value"] = trace.max()
                 print()
                 chstr = pd.Series(channel).to_string()
                 parts = ["\t" + line for line in chstr.split("\n")]
                 chstr = "\n".join(parts)
                 print(chstr)
         except BaseException as e:
-            row = pd.Series(index=ERROR_COLUMNS)
+            row = {}
             row["Filename"] = str(fname)
             row["Error"] = str(e)
-            errors = errors.append(row, ignore_index=True)
+            error_rows.append(row)
             continue
+    errors = pd.DataFrame(error_rows)
     return errors
 
 
 def main():
     description = """Display summary information about a file, multiple files,
     or directories of files containing strong motion data in the supported
     formats.
```

### Comparing `gmprocess-1.2.6/src/gmprocess/bin/gmworkspace.py` & `gmprocess-1.2.7/src/gmprocess/bin/gmworkspace.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/bin/list_metrics.py` & `gmprocess-1.2.7/src/gmprocess/bin/list_metrics.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/core/stationstream.py` & `gmprocess-1.2.7/src/gmprocess/core/stationstream.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # stdlib imports
-import json
 import logging
 
 # third party imports
 import numpy as np
 from obspy.core.stream import Stream
 from obspy.core.utcdatetime import UTCDateTime
 from obspy.core.inventory import (
@@ -27,19 +26,14 @@
 
 UNITS = {"acc": "cm/s/s", "vel": "cm/s"}
 REVERSE_UNITS = {"cm/s/s": "acc", "cm/s": "vel"}
 
 # Number of samples for Landzos interpolation.
 N_LANCZOS = 20
 
-# if we find places for these in the standard metadata,
-# remove them from this list. Anything here will
-# be extracted from the stats standard dictionary,
-# combined with the format_specific dictionary,
-# serialized to json and stored in the station description.
 UNUSED_STANDARD_PARAMS = [
     "instrument_period",
     "instrument_damping",
     "process_time",
     "process_level",
     "structure_type",
     "corner_frequency",
@@ -408,43 +402,48 @@
         )
         channels = []
         for trace in self:
             logging.debug(f"trace: {trace}")
             channel = _channel_from_stats(trace.stats)
             channels.append(channel)
 
-        subdict = {}
-        for k in UNUSED_STANDARD_PARAMS:
-            if k in self[0].stats.standard:
-                subdict[k] = self[0].stats.standard[k]
-
-        format_specific = {}
-        if "format_specific" in self[0].stats:
-            format_specific = dict(self[0].stats.format_specific)
-
-        big_dict = {"standard": subdict, "format_specific": format_specific}
-        jsonstr = json.dumps(big_dict)
         sta = Station(
             # This is the station code according to the SEED standard.
             code=self[0].stats.station,
             latitude=self[0].stats.coordinates.latitude,
             elevation=self[0].stats.coordinates.elevation,
             longitude=self[0].stats.coordinates.longitude,
             channels=channels,
             site=Site(name=self[0].stats.standard.station_name),
-            description=jsonstr,
             creation_date=UTCDateTime(1970, 1, 1),  # this is bogus
             total_number_of_channels=len(self),
         )
 
         net.stations.append(sta)
         inv.networks.append(net)
 
         return inv
 
+    def getSupplementalStats(self):
+        """Return dictionary supplemental stream information.
+
+        This was created to include information that is not captured in StationXML
+        or in obspy's trace stats object.
+        """
+        subdict = {}
+        for k in UNUSED_STANDARD_PARAMS:
+            if k in self[0].stats.standard:
+                subdict[k] = self[0].stats.standard[k]
+
+        format_specific = {}
+        if "format_specific" in self[0].stats:
+            format_specific = dict(self[0].stats.format_specific)
+
+        return {"standard": subdict, "format_specific": format_specific}
+
     def check_stream(self):
         """Check StationStream for being flagged as failed.
 
         The logic of this method is controlled by the "any_trace_failures" config
         parameter in the "check_stream" section:
             - If "any_trace_failures" is True, then the stream is treated as failed if
               ANY of the constituent traces failed.
```

### Comparing `gmprocess-1.2.6/src/gmprocess/core/stationtrace.py` & `gmprocess-1.2.7/src/gmprocess/core/stationtrace.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/core/streamarray.py` & `gmprocess-1.2.7/src/gmprocess/core/streamarray.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/core/streamcollection.py` & `gmprocess-1.2.7/src/gmprocess/core/streamcollection.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/CESMD_NGA_ids.csv` & `gmprocess-1.2.7/src/gmprocess/data/CESMD_NGA_ids.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/GDMSstations.json` & `gmprocess-1.2.7/src/gmprocess/data/GDMSstations.json`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/config_production.yml` & `gmprocess-1.2.7/src/gmprocess/data/config_production.yml`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 #    |____________________|_/  \  /\    /    \/\____|
 #    |                    |     \/  \  /            |
 #    |                    |          \/             |
 #
 #    record_start       split              signal_end
 
 windows:
-
+    no_noise: False
     signal_end:
         # Options for setting the end of the signal window. Options are set with the key
         # "method":
         #    - "velocity": Set the end of the signal can be set using a phase velocity;
         #      this option makes use of the keys "vmin" and "floor".
         #    - "model": Set the end of the signal window using a shaking duration model;
         #      this options makes use of the keys "model" and "epsilon"
```

### Comparing `gmprocess-1.2.6/src/gmprocess/data/config_test.yml` & `gmprocess-1.2.7/src/gmprocess/data/config_test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 #    |____________________|_/  \  /\    /    \/\____|
 #    |                    |     \/  \  /            |
 #    |                    |          \/             |
 #
 #    record_start       split              signal_end
 
 windows:
-
+    no_noise: False
     signal_end:
         # Options for setting the end of the signal window. Options are set with the key
         # "method":
         #    - "velocity": Set the end of the signal can be set using a phase velocity;
         #      this option makes use of the keys "vmin" and "floor".
         #    - "model": Set the end of the signal window using a shaking duration model;
         #      this options makes use of the keys "model" and "epsilon"
```

### Comparing `gmprocess-1.2.6/src/gmprocess/data/cosmos_table10.xls` & `gmprocess-1.2.7/src/gmprocess/data/cosmos_table10.xls`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/cosmos_table4.xls` & `gmprocess-1.2.7/src/gmprocess/data/cosmos_table4.xls`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/demo/ci38457511/raw/CICCC.RAW` & `gmprocess-1.2.7/src/gmprocess/data/demo/ci38457511/raw/CICCC.RAW`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/demo/ci38457511/raw/CICLC.v1` & `gmprocess-1.2.7/src/gmprocess/data/demo/ci38457511/raw/CICLC.v1`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/demo/ci38457511/raw/CITOW2.RAW` & `gmprocess-1.2.7/src/gmprocess/data/demo/ci38457511/raw/CITOW2.RAW`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/fdsn_codes.csv` & `gmprocess-1.2.7/src/gmprocess/data/fdsn_codes.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/lme/SA_rotd50.0_2020.03.31.csv` & `gmprocess-1.2.7/src/gmprocess/data/lme/SA_rotd50.0_2020.03.31.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/nga_w2_selected.csv` & `gmprocess-1.2.7/src/gmprocess/data/nga_w2_selected.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/nn_clipping/weight_1.csv` & `gmprocess-1.2.7/src/gmprocess/data/nn_clipping/weight_1.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/M.csv` & `gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/M.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/final_training.csv` & `gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/final_training.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/model_3.txt` & `gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/model_3.txt`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/model_5.txt` & `gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/model_5.txt`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/mu_sigma.csv` & `gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/mu_sigma.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/weight_1.csv` & `gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/weight_1.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/weight_2.csv` & `gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/weight_2.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/nn_qa/Cant/weight_output.csv` & `gmprocess-1.2.7/src/gmprocess/data/nn_qa/Cant/weight_output.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/M.csv` & `gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/M.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/final_training.csv` & `gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/final_training.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/model_0.txt` & `gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/model_0.txt`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/mu_sigma.csv` & `gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/mu_sigma.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/weight_1.csv` & `gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/weight_1.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/weight_2.csv` & `gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/weight_2.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/nn_qa/CantWell/weight_output.csv` & `gmprocess-1.2.7/src/gmprocess/data/nn_qa/CantWell/weight_output.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/picker.yml` & `gmprocess-1.2.7/src/gmprocess/data/picker.yml`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/station_coordinates.xlsx` & `gmprocess-1.2.7/src/gmprocess/data/station_coordinates.xlsx`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/data/usgs_ids_nga_and_srcmod_cross_reference.xlsx` & `gmprocess-1.2.7/src/gmprocess/data/usgs_ids_nga_and_srcmod_cross_reference.xlsx`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/asdf/core.py` & `gmprocess-1.2.7/src/gmprocess/io/asdf/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/asdf/stream_workspace.py` & `gmprocess-1.2.7/src/gmprocess/io/asdf/stream_workspace.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 # stdlib imports
+import copy
 import json
+import logging
 import re
-import copy
 import warnings
-import logging
 from pathlib import Path
 
+import numpy as np
+import pandas as pd
+import prov.model
+
 # third party imports
 import pyasdf
-import prov.model
-import numpy as np
 import scipy.interpolate as spint
-from obspy.core.utcdatetime import UTCDateTime
-import pandas as pd
-from h5py.h5py_warnings import H5pyDeprecationWarning
-from ruamel.yaml import YAML
 from esi_utils_rupture.factory import get_rupture
 from esi_utils_rupture.origin import Origin
+from gmprocess.core.stationstream import StationStream
 
 # local imports
 from gmprocess.core.stationtrace import (
-    StationTrace,
-    TIMEFMT_MS,
     NS_SEIS,
+    TIMEFMT_MS,
+    StationTrace,
     _get_person_agent,
     _get_software_agent,
 )
-from gmprocess.core.stationstream import StationStream
-from gmprocess.core.streamcollection import StreamCollection
 from gmprocess.core.streamarray import StreamArray
-from gmprocess.metrics.station_summary import StationSummary, XML_UNITS
+from gmprocess.core.streamcollection import StreamCollection
+from gmprocess.metrics.station_summary import XML_UNITS, StationSummary
+from gmprocess.utils import constants
+from gmprocess.utils.config import get_config, update_dict
 from gmprocess.utils.event import ScalarEvent
 from gmprocess.utils.tables import _get_table_row
-from gmprocess.utils.config import get_config
-from gmprocess.utils.config import update_dict
-from gmprocess.utils import constants
+from h5py.h5py_warnings import H5pyDeprecationWarning
+from obspy.core.utcdatetime import UTCDateTime
+from ruamel.yaml import YAML
+from strec.subtype import SubductionSelector
 
 TIMEPAT = "[0-9]{4}-[0-9]{2}-[0-9]{2}T"
 EVENT_TABLE_COLUMNS = [
     "id",
     "time",
     "latitude",
     "longitude",
@@ -271,16 +272,46 @@
 
     def addEvent(self, event):
         """Add event object to file.
 
         Args:
             event (Event): Obspy event object.
         """
+        self.insert_strec(event)
         self.dataset.add_quakeml(event)
 
+    def insert_strec(self, event):
+        selector = SubductionSelector()
+        tensor_params = None
+        if hasattr(event, "id"):
+            _, _, _, _, tensor_params = selector.getOnlineTensor(event.id)
+        strec_params = selector.getSubductionType(
+            event.latitude,
+            event.longitude,
+            event.depth_km,
+            event.magnitude,
+            eventid=event.id,
+            tensor_params=tensor_params,
+        ).to_dict()
+        strec_params_str = _stringify_dict(strec_params)
+        dtype = "StrecParameters"
+        strec_path = f"STREC/{event.id}"
+        logging.info(f"Inserting strec info for {event.id}")
+        self.insert_aux(json.dumps(strec_params_str), dtype, strec_path, True)
+
+    def get_strec(self, event):
+        eventid = event.id.replace("smi:local/", "")
+        aux_data = self.dataset.auxiliary_data
+        if "StrecParameters" not in aux_data:
+            return None
+        bytelist = aux_data["StrecParameters"]["STREC"][eventid].data[:].tolist()
+        jsonstr = "".join([chr(b) for b in bytelist])
+        jdict = json.loads(jsonstr)
+        return jdict
+
     def addConfig(self, config=None, force=False):
         """Add config to an ASDF dataset and workspace attribute.
 
         Args:
             config (dict):
                 Configuration options.
             force (bool):
@@ -313,16 +344,27 @@
     def setConfig(self):
         """Get config from ASDF dataset and set as a workspace attribute."""
         group_name = "config/config"
         data_exists = group_name in self.dataset._auxiliary_data_group
         if not data_exists:
             logging.error("No config found in auxiliary data.")
         bytelist = self.dataset._auxiliary_data_group[group_name][()].tolist()
+
+        # Load config from the workshapce file
         conf_str = "".join([chr(b) for b in bytelist])
-        self.config = json.loads(conf_str)
+        custom_config = json.loads(conf_str)
+
+        # Get the default config
+        default_config_file = constants.DATA_DIR / constants.CONFIG_FILE_PRODUCTION
+        with open(default_config_file, "r", encoding="utf-8") as f:
+            yaml = YAML()
+            yaml.preserve_quotes = True
+            default_config = yaml.load(f)
+        update_dict(default_config, custom_config)
+        self.config = default_config
 
     def addGmprocessVersion(self, version):
         """Add gmprocess version to an ASDF file."""
         self.insert_aux(version, data_name="gmprocess_version", path="version")
 
     def getGmprocessVersion(self):
         """Get gmprocess version from ASDF file."""
@@ -410,41 +452,50 @@
                 provdocs = stream.getProvenanceDocuments(
                     base_prov=base_prov, gmprocess_version=gmprocess_version
                 )
                 for provdoc, trace in zip(provdocs, stream):
                     provname = format_nslct(trace.stats, tag)
                     self.dataset.add_provenance_document(provdoc, name=provname)
 
+            # get the path for the stream for storing aux data
+            if config["read"]["use_streamcollection"]:
+                chancode = stream.get_inst()
+            else:
+                chancode = stream[0].stats.channel
+            stream_path = "/".join(
+                [
+                    format_netsta(stream[0].stats),
+                    format_nslit(stream[0].stats, chancode, tag),
+                ]
+            )
+
+            # add supplemental stats, e.g., "standard" and "format_specific"
+            sup_stats = stream.getSupplementalStats()
+            sup_stats_str = _stringify_dict(sup_stats)
+            self.insert_aux(
+                json.dumps(sup_stats_str), "StreamSupplementalStats", stream_path
+            )
+
             # add processing parameters from streams
-            jdict = {}
+            proc_params = {}
             for key in stream.getStreamParamKeys():
                 value = stream.getStreamParam(key)
-                jdict[key] = value
+                proc_params[key] = value
 
-            if len(jdict):
-                # NOTE: We would store this dictionary just as
-                # the parameters dictionary, but HDF cannot handle
-                # nested dictionaries.
-                # Also, this seems like a lot of effort
-                # just to store a string in HDF, but other
+            if len(proc_params):
+                # NOTE: We would store this dictionary just as the parameters
+                # dictionary, but HDF cannot handle nested dictionaries. Also, this
+                # seems like a lot of effort just to store a string in HDF, but other
                 # approaches failed. Suggestions are welcome.
-                jdict = _stringify_dict(jdict)
+                proc_params_str = _stringify_dict(proc_params)
                 dtype = "StreamProcessingParameters"
-                if config["read"]["use_streamcollection"]:
-                    chancode = stream.get_inst()
-                else:
-                    chancode = stream[0].stats.channel
-                parampath = "/".join(
-                    [
-                        format_netsta(stream[0].stats),
-                        format_nslit(stream[0].stats, chancode, tag),
-                    ]
-                )
 
-                self.insert_aux(json.dumps(jdict), dtype, parampath, overwrite)
+                self.insert_aux(
+                    json.dumps(proc_params_str), dtype, stream_path, overwrite
+                )
 
             # add processing parameters from traces
             for trace in stream:
                 procname = "/".join(
                     [
                         format_netsta(trace.stats),
                         format_nslct(trace.stats, tag),
@@ -544,20 +595,17 @@
                     yaml.preserve_quotes = True
                     default_config = yaml.load(f)
                 update_dict(self.config, default_config)
             else:
                 config = get_config()
 
         trace_auxholder = []
-        stream_auxholder = []
         auxdata = self.dataset.auxiliary_data
         if "TraceProcessingParameters" in auxdata:
             trace_auxholder = auxdata.TraceProcessingParameters
-        if "StreamProcessingParameters" in auxdata:
-            stream_auxholder = auxdata.StreamProcessingParameters
         streams = []
 
         if stations is None:
             stations = self.getStations()
         if labels is None:
             labels = self.getLabels()
         else:
@@ -606,52 +654,52 @@
                     # get the provenance information
                     provname = format_nslct(trace.stats, tag)
                     if provname in self.dataset.provenance.list():
                         provdoc = self.dataset.provenance[provname]
                         trace.setProvenanceDocument(provdoc)
 
                     # get the trace processing parameters
-                    top = format_netsta(trace.stats)
+                    net_sta = format_netsta(trace.stats)
                     trace_path = format_nslct(trace.stats, tag)
-                    if top in trace_auxholder:
-                        root_auxholder = trace_auxholder[top]
+                    if net_sta in trace_auxholder:
+                        root_auxholder = trace_auxholder[net_sta]
                         if trace_path in root_auxholder:
                             bytelist = root_auxholder[trace_path].data[:].tolist()
                             jsonstr = "".join([chr(b) for b in bytelist])
                             jdict = json.loads(jsonstr)
                             for key, value in jdict.items():
                                 trace.setParameter(key, value)
 
                     # get the trace spectra arrays from auxiliary,
                     # repack into stationtrace object
                     spectra = {}
 
                     if "Cache" in auxdata:
                         for aux in auxdata["Cache"].list():
                             auxarray = auxdata["Cache"][aux]
-                            if top not in auxarray.list():
+                            if net_sta not in auxarray.list():
                                 continue
-                            auxarray_top = auxarray[top]
-                            if trace_path in auxarray_top:
+                            auxarray_net_sta = auxarray[net_sta]
+                            if trace_path in auxarray_net_sta:
                                 specparts = camel_case_split(aux)
                                 array_name = specparts[-1].lower()
                                 specname = "_".join(specparts[:-1]).lower()
-                                specarray = auxarray_top[trace_path].data[()]
+                                specarray = auxarray_net_sta[trace_path].data[()]
                                 if specname in spectra:
                                     spectra[specname][array_name] = specarray
                                 else:
                                     spectra[specname] = {array_name: specarray}
                         for key, value in spectra.items():
                             trace.setCached(key, value)
 
                     # get review information if it is present:
                     if "review" in auxdata:
-                        if top in auxdata.review:
-                            if trace_path in auxdata.review[top]:
-                                tr_review = auxdata.review[top][trace_path]
+                        if net_sta in auxdata.review:
+                            if trace_path in auxdata.review[net_sta]:
+                                tr_review = auxdata.review[net_sta][trace_path]
                                 review_dict = {}
                                 if "accepted" in tr_review:
                                     tr_acc = tr_review.accepted
                                     review_dict["accepted"] = bool(tr_acc.data[0])
                                     if "timestamp" in tr_acc.parameters:
                                         review_dict["time"] = tr_acc.parameters[
                                             "timestamp"
@@ -672,25 +720,37 @@
                                             "lowpass"
                                         ] = fc_dict["lowpass"].data[0]
                                 trace.setParameter("review", review_dict)
 
                     stream = StationStream(traces=[trace], config=config)
                     stream.tag = tag
 
-                    # get the stream processing parameters
+                    # deal with stream-level data
                     stream_path = format_nslit(trace.stats, stream.get_inst(), tag)
-                    if top in stream_auxholder:
-                        top_auxholder = stream_auxholder[top]
-                        if stream_path in top_auxholder:
-                            auxarray = top_auxholder[stream_path]
-                            bytelist = auxarray.data[:].tolist()
-                            jsonstr = "".join([chr(b) for b in bytelist])
-                            jdict = json.loads(jsonstr)
-                            for key, value in jdict.items():
-                                stream.setStreamParam(key, value)
+
+                    # get the stream processing parameters
+                    proc_dict = self._get_aux_dict(
+                        "StreamProcessingParameters", net_sta, stream_path
+                    )
+                    if proc_dict:
+                        for key, value in proc_dict.items():
+                            stream.setStreamParam(key, value)
+
+                    # get the supplemental stream parameters
+                    supp_dict = self._get_aux_dict(
+                        "StreamSupplementalStats", net_sta, stream_path
+                    )
+                    if supp_dict:
+                        supp_keys = ["standard", "format_specific"]
+                        for supp_key in supp_keys:
+                            for key1, value1 in supp_dict.items():
+                                if key1 == supp_key:
+                                    for key2, value2 in value1.items():
+                                        for tr in stream:
+                                            tr.stats[supp_key][key2] = value2
 
                     streams.append(stream)
 
         # Note: no need to handle duplicates when retrieving stations from the
         # workspace file because it must have been handled before putting them
         # into the workspace file.
 
@@ -700,14 +760,42 @@
             "use_streamcollection"
         ]:
             streams = StreamCollection(streams, handle_duplicates=False, config=config)
         else:
             streams = StreamArray(streams, config=config)
         return streams
 
+    def _get_aux_dict(self, aux_name, net_sta, stream_path):
+        """Convenience function to get a diction stored in aux data
+
+        Args:
+            aux_name (str):
+                Name of data in aux data.
+            net_sta (str):
+                <net code>.<sta code>.
+            stream_path (str):
+                <net code>.<sta code>.<loc code>.<chan code>_<event id>_<label>
+
+        Returns:
+            dict if found, otherwise None.
+        """
+        aux_data = self.dataset.auxiliary_data
+        if aux_name in aux_data:
+            stream_auxholder = aux_data[aux_name][net_sta]
+            if stream_path in stream_auxholder:
+                auxarray = stream_auxholder[stream_path]
+                bytelist = auxarray.data[:].tolist()
+                jsonstr = "".join([chr(b) for b in bytelist])
+                if len(jsonstr):
+                    return json.loads(jsonstr)
+                else:
+                    return None
+        else:
+            return None
+
     def getStations(self):
         """Get list of station codes within the file.
 
         Returns:
             list: List of station codes contained in workspace.
         """
         stations = self.dataset.waveforms.list()
@@ -722,16 +810,15 @@
             data_name (str):
                 What this data should be called in the ASDF file.
             path (str):
                 The aux path where this data should be stored.
             overwrite (bool):
                 Should the data be overwritten if it already exists?
         """
-        # this seems like a lot of effort
-        # just to store a string in HDF, but other
+        # this seems like a lot of effort just to store a string in HDF, but other
         # approaches failed. Suggestions are welcome.
 
         group_name = f"{data_name}/{path}"
         data_exists = group_name in self.dataset._auxiliary_data_group
         if overwrite and data_exists:
             del self.dataset._auxiliary_data_group[group_name]
 
@@ -1262,26 +1349,26 @@
         else:
             stream_tag = streams[0].tag
 
         if hasattr(streams[0], "use_array") and streams[0].use_array:
             chancode = streams[0][0].stats.channel
         else:
             chancode = streams[0].get_inst()
-        top = format_netsta(streams[0][0].stats)
+        net_sta = format_netsta(streams[0][0].stats)
 
         metricpath = format_nslit(streams[0][0].stats, chancode, stream_tag)
 
-        if top in auxholder:
-            tauxholder = auxholder[top]
-            if metricpath not in tauxholder:
+        if net_sta in auxholder:
+            net_sta_auxholder = auxholder[net_sta]
+            if metricpath not in net_sta_auxholder:
                 fmt = "Stream metrics path (%s) not in WaveFormMetrics auxiliary_data."
                 logging.warning(fmt % metricpath)
                 return None
 
-            bytelist = tauxholder[metricpath].data[:].tolist()
+            bytelist = net_sta_auxholder[metricpath].data[:].tolist()
             xml_stream = "".join([chr(b) for b in bytelist])
             xml_stream = xml_stream.encode("utf-8")
         else:
             return
 
         # ----------------------------------------------------------- #
         # Station Metrics
@@ -1292,24 +1379,24 @@
 
         if hasattr(streams[0], "use_array") and streams[0].use_array:
             chancode = streams[0][0].stats.channel
         else:
             chancode = streams[0].get_inst()
         station_path = format_nslit(streams[0][0].stats, chancode, eventid)
 
-        if top in auxholder:
-            tauxholder = auxholder[top]
-            if station_path not in tauxholder:
+        if net_sta in auxholder:
+            net_sta_auxholder = auxholder[net_sta]
+            if station_path not in net_sta_auxholder:
                 logging.warning(
                     "Stream path (%s) not in StationMetrics auxiliary_data."
                     % station_path
                 )
                 return
 
-            bytelist = tauxholder[station_path].data[:].tolist()
+            bytelist = net_sta_auxholder[station_path].data[:].tolist()
             xml_station = "".join([chr(b) for b in bytelist])
             xml_station = xml_station.encode("utf-8")
         else:
             return
 
         summary = StationSummary.from_xml(xml_stream, xml_station)
         return summary
```

### Comparing `gmprocess-1.2.6/src/gmprocess/io/asdf/utils.py` & `gmprocess-1.2.7/src/gmprocess/io/asdf/utils.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/bhrc/core.py` & `gmprocess-1.2.7/src/gmprocess/io/bhrc/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/cosmos/cesmd_fetcher.py` & `gmprocess-1.2.7/src/gmprocess/io/cosmos/cesmd_fetcher.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/cosmos/cesmd_search.py` & `gmprocess-1.2.7/src/gmprocess/io/cosmos/cesmd_search.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/cosmos/core.py` & `gmprocess-1.2.7/src/gmprocess/io/cosmos/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/cosmos/cosmos_writer.py` & `gmprocess-1.2.7/src/gmprocess/io/cosmos/cosmos_writer.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/cosmos/data_structures.py` & `gmprocess-1.2.7/src/gmprocess/io/cosmos/data_structures.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/cwb/core.py` & `gmprocess-1.2.7/src/gmprocess/io/cwb/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/dmg/core.py` & `gmprocess-1.2.7/src/gmprocess/io/dmg/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/esm/core.py` & `gmprocess-1.2.7/src/gmprocess/io/esm/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/fetcher.py` & `gmprocess-1.2.7/src/gmprocess/io/fetcher.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/geonet/core.py` & `gmprocess-1.2.7/src/gmprocess/io/geonet/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/global_fetcher.py` & `gmprocess-1.2.7/src/gmprocess/io/global_fetcher.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/knet/core.py` & `gmprocess-1.2.7/src/gmprocess/io/knet/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/knet/knet_fetcher.py` & `gmprocess-1.2.7/src/gmprocess/io/knet/knet_fetcher.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/nga.py` & `gmprocess-1.2.7/src/gmprocess/io/nga.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/nsmn/core.py` & `gmprocess-1.2.7/src/gmprocess/io/nsmn/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/obspy/core.py` & `gmprocess-1.2.7/src/gmprocess/io/obspy/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/obspy/fdsn_fetcher.py` & `gmprocess-1.2.7/src/gmprocess/io/obspy/fdsn_fetcher.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/read.py` & `gmprocess-1.2.7/src/gmprocess/io/read.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/read_directory.py` & `gmprocess-1.2.7/src/gmprocess/io/read_directory.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/renadic/core.py` & `gmprocess-1.2.7/src/gmprocess/io/renadic/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/report.py` & `gmprocess-1.2.7/src/gmprocess/io/report.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/seedname.py` & `gmprocess-1.2.7/src/gmprocess/io/seedname.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/smc/core.py` & `gmprocess-1.2.7/src/gmprocess/io/smc/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/stream.py` & `gmprocess-1.2.7/src/gmprocess/io/stream.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/unam/core.py` & `gmprocess-1.2.7/src/gmprocess/io/unam/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/usc/core.py` & `gmprocess-1.2.7/src/gmprocess/io/usc/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/io/utils.py` & `gmprocess-1.2.7/src/gmprocess/io/utils.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/combination/arithmetic_mean.py` & `gmprocess-1.2.7/src/gmprocess/metrics/combination/arithmetic_mean.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/combination/combination.py` & `gmprocess-1.2.7/src/gmprocess/metrics/combination/combination.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/combination/geometric_mean.py` & `gmprocess-1.2.7/src/gmprocess/metrics/combination/geometric_mean.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/combination/greater_of_two_horizontals.py` & `gmprocess-1.2.7/src/gmprocess/metrics/combination/greater_of_two_horizontals.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/combination/null_combination.py` & `gmprocess-1.2.7/src/gmprocess/metrics/combination/null_combination.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/combination/quadratic_mean.py` & `gmprocess-1.2.7/src/gmprocess/metrics/combination/quadratic_mean.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/gather.py` & `gmprocess-1.2.7/src/gmprocess/metrics/gather.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/imc/arithmetic_mean.py` & `gmprocess-1.2.7/src/gmprocess/metrics/imc/arithmetic_mean.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/imc/channels.py` & `gmprocess-1.2.7/src/gmprocess/metrics/imc/channels.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/imc/geometric_mean.py` & `gmprocess-1.2.7/src/gmprocess/metrics/imc/geometric_mean.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/imc/gmrotd.py` & `gmprocess-1.2.7/src/gmprocess/metrics/imc/gmrotd.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/imc/greater_of_two_horizontals.py` & `gmprocess-1.2.7/src/gmprocess/metrics/imc/greater_of_two_horizontals.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/imc/imc.py` & `gmprocess-1.2.7/src/gmprocess/metrics/imc/imc.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/imc/quadratic_mean.py` & `gmprocess-1.2.7/src/gmprocess/metrics/imc/quadratic_mean.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/imc/radial_transverse.py` & `gmprocess-1.2.7/src/gmprocess/metrics/imc/radial_transverse.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/imc/rotd.py` & `gmprocess-1.2.7/src/gmprocess/metrics/imc/rotd.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/imt/arias.py` & `gmprocess-1.2.7/src/gmprocess/metrics/imt/arias.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/imt/duration.py` & `gmprocess-1.2.7/src/gmprocess/metrics/imt/duration.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/imt/fas.py` & `gmprocess-1.2.7/src/gmprocess/metrics/imt/fas.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/imt/imt.py` & `gmprocess-1.2.7/src/gmprocess/metrics/imt/imt.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/imt/pga.py` & `gmprocess-1.2.7/src/gmprocess/metrics/imt/pga.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/imt/pgv.py` & `gmprocess-1.2.7/src/gmprocess/metrics/imt/pgv.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/imt/sa.py` & `gmprocess-1.2.7/src/gmprocess/metrics/imt/sa.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/imt/sorted_duration.py` & `gmprocess-1.2.7/src/gmprocess/metrics/imt/sorted_duration.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/metrics_controller.py` & `gmprocess-1.2.7/src/gmprocess/metrics/metrics_controller.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/reduction/arias.py` & `gmprocess-1.2.7/src/gmprocess/metrics/reduction/arias.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/reduction/duration.py` & `gmprocess-1.2.7/src/gmprocess/metrics/reduction/duration.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/reduction/max.py` & `gmprocess-1.2.7/src/gmprocess/metrics/reduction/max.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/reduction/null_reduction.py` & `gmprocess-1.2.7/src/gmprocess/metrics/reduction/null_reduction.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/reduction/percentile.py` & `gmprocess-1.2.7/src/gmprocess/metrics/reduction/percentile.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/reduction/reduction.py` & `gmprocess-1.2.7/src/gmprocess/metrics/reduction/reduction.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/reduction/smooth_select.py` & `gmprocess-1.2.7/src/gmprocess/metrics/reduction/smooth_select.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/reduction/sorted_duration.py` & `gmprocess-1.2.7/src/gmprocess/metrics/reduction/sorted_duration.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/rotation/gmrotd.py` & `gmprocess-1.2.7/src/gmprocess/metrics/rotation/gmrotd.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/rotation/null_rotation.py` & `gmprocess-1.2.7/src/gmprocess/metrics/rotation/null_rotation.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/rotation/radial_transverse.py` & `gmprocess-1.2.7/src/gmprocess/metrics/rotation/radial_transverse.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/rotation/rotation.py` & `gmprocess-1.2.7/src/gmprocess/metrics/rotation/rotation.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/rotation/rotd.py` & `gmprocess-1.2.7/src/gmprocess/metrics/rotation/rotd.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/station_summary.py` & `gmprocess-1.2.7/src/gmprocess/metrics/station_summary.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/transform/differentiate.py` & `gmprocess-1.2.7/src/gmprocess/metrics/transform/differentiate.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/transform/fft.py` & `gmprocess-1.2.7/src/gmprocess/metrics/transform/fft.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/transform/integrate.py` & `gmprocess-1.2.7/src/gmprocess/metrics/transform/integrate.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/transform/null_transform.py` & `gmprocess-1.2.7/src/gmprocess/metrics/transform/null_transform.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/transform/oscillator.py` & `gmprocess-1.2.7/src/gmprocess/metrics/transform/oscillator.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/metrics/transform/transform.py` & `gmprocess-1.2.7/src/gmprocess/metrics/transform/transform.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/assemble.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/assemble.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/autoprocess.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/autoprocess.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/autoshakemap.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/autoshakemap.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/base.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/clean.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/clean.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/compute_station_metrics.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/compute_station_metrics.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/compute_waveform_metrics.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/compute_waveform_metrics.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/config.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/config.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/download.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/download.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/export_failure_tables.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/export_failure_tables.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/export_gmpacket.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/export_gmpacket.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,13 +54,12 @@
             packet_writer = gmp_utils.GroundMotionPacketWriter(
                 event_dir, workname, label="default"
             )
             files, nevents, nstreams, ntraces = packet_writer.write()
             logging.info(
                 f"Processed {nevents} events - {nstreams} streams and {ntraces} traces."
             )
-            jsonfile = files[0]
-
-            if jsonfile is not None:
+            if len(files):
+                jsonfile = files[0]
                 self.append_file("shakemap", jsonfile)
 
         self._summarize_files_created()
```

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/export_metric_tables.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/export_metric_tables.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/export_provenance_tables.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/export_provenance_tables.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/export_shakemap.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/export_shakemap.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/generate_regression_plot.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/generate_regression_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,19 @@
         imc_table_ext = list(self.gmrecords.data_path.glob("*_README*"))[0].suffix
 
         imc_tables = {}
         for imckey in imc_table_names:
             if "fit_spectra_parameters" not in imc_tables:
                 table_name = self.gmrecords.data_path / f"{imckey}{imc_table_ext}"
                 if imc_table_ext == ".csv":
-                    imc_tables[imckey] = pd.read_csv(table_name)
+                    if table_name.exists():
+                        imc_tables[imckey] = pd.read_csv(table_name)
                 else:
-                    imc_tables[imckey] = pd.read_excel(table_name)
+                    if table_name.exists():
+                        imc_tables[imckey] = pd.read_excel(table_name)
 
         event_files = list(self.gmrecords.data_path.glob("*_events.*"))
         if len(event_files) == 1:
             event_file = event_files[0]
         elif len(event_files) == 0:
             msg = (
                 "No event file found. Cannot build regression plot. "
```

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/generate_report.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/generate_report.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/generate_station_maps.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/generate_station_maps.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/import_data.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/import_data.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/init.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/init.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/lazy_loader.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/process_waveforms.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/process_waveforms.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/processing_steps.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/processing_steps.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/subcommands/projects.py` & `gmprocess-1.2.7/src/gmprocess/subcommands/projects.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
+import logging
 import os
-import sys
+import pathlib
 import platform
-import logging
 import shutil
-
+import sys
 from pathlib import Path
+
+from esi_utils_io.cmd import get_command_output
 from gmprocess.subcommands.lazy_loader import LazyLoader
 
 ryaml = LazyLoader("yaml", globals(), "ruamel.yaml")
 base = LazyLoader("base", globals(), "gmprocess.subcommands.base")
 constants = LazyLoader("constants", globals(), "gmprocess.utils.constants")
 prompt = LazyLoader("prompt", globals(), "gmprocess.utils.prompt")
 configobj = LazyLoader("configobj", globals(), "configobj")
 
 
 CURRENT_MARKERS = {True: "**Current Project**", False: ""}
+STREC_CONFIG = pathlib.Path.home() / ".strec" / "config.ini"
+NEW_STREC_FOLDER = pathlib.Path.home() / ".gmprocess" / "strec"
 
 
 class ProjectsModule(base.SubcommandModule):
     """
     Manage gmrecords projects.
     """
 
@@ -130,14 +134,18 @@
 
         if not self.config:
             print(f"Could not find project configuration file {self.config_filepath}.")
             return
         if len(self.config["projects"]) == 0:
             print(f"No projects in {self.config_filepath}.")
 
+        # check to see if user already has strec installed
+        if not STREC_CONFIG.exists():
+            self.configure_strec()
+
         if args.list:
             self.list_projects()
         elif args.switch:
             self.switch_project(args.switch)
         elif args.delete:
             self.delete_project(args.delete)
         elif args.rename:
@@ -148,14 +156,26 @@
             self._set_path(proj_name, conf_path, "conf_path")
         elif args.set_data:
             proj_name, data_path = args.set_data
             self._set_path(proj_name, data_path, "data_path")
         else:
             raise NotImplementedError("Subcommand projects option not implemented.")
 
+    def configure_strec(self):
+        cmd = f"strec_cfg update --datafolder {NEW_STREC_FOLDER} --slab --gcmt"
+        res, stdout, stderr = get_command_output(cmd)
+        if not res:
+            logging.CRITICAL(
+                f"Failed to configure STREC code with command {cmd}. Output:"
+            )
+            logging.CRITICAL(f"\n'{stdout}'")
+            logging.CRITICAL(f"\n'{stderr}'")
+        else:
+            logging.info(f"Successfully installed STREC with {cmd}.")
+
     def list_projects(self):
         projects = self.config["projects"]
         for name in projects.keys():
             project = Project.from_config(self.config, name)
             print("\n" + str(project) + "\n")
 
     def switch_project(self, target):
```

### Comparing `gmprocess-1.2.6/src/gmprocess/utils/args.py` & `gmprocess-1.2.7/src/gmprocess/utils/args.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/utils/assemble_utils.py` & `gmprocess-1.2.7/src/gmprocess/utils/assemble_utils.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/utils/base_utils.py` & `gmprocess-1.2.7/src/gmprocess/utils/base_utils.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/utils/config.py` & `gmprocess-1.2.7/src/gmprocess/utils/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
 import os
-from pathlib import Path
 
 from gmprocess.utils import constants
 from ruamel.yaml import YAML
 from ruamel.yaml.error import YAMLError
 from schema import Optional, Or, Schema
 
 CONF_SCHEMA = Schema(
@@ -87,14 +86,15 @@
             "resample_rate": float,
             "sac_conversion_factor": float,
             "sac_source": str,
             "use_streamcollection": bool,
             "exclude_patterns": list,
         },
         "windows": {
+            "no_noise": bool,
             "signal_end": {
                 "method": Or("model", "velocity", "magnitude", "none"),
                 "vmin": float,
                 "floor": float,
                 "model": str,
                 "epsilon": float,
             },
@@ -270,16 +270,15 @@
         dictionary:
             Configuration parameters.
     Raises:
         IndexError:
             If input section name is not found.
     """
     # Read in default config from the repository
-    data_dir = Path(__file__).parent / ".." / "data"
-    default_config_file = data_dir / constants.CONFIG_FILE_PRODUCTION
+    default_config_file = constants.DATA_DIR / constants.CONFIG_FILE_PRODUCTION
     if not default_config_file.exists():
         fmt = "Missing config file: %s."
         raise OSError(fmt % default_config_file)
     else:
         with open(default_config_file, "r", encoding="utf-8") as f:
             yaml = YAML()
             yaml.preserve_quotes = True
```

### Comparing `gmprocess-1.2.6/src/gmprocess/utils/constants.py` & `gmprocess-1.2.7/src/gmprocess/utils/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-import scipy.constants as sp
 import pathlib
 
+import scipy.constants as sp
+
 DATA_DIR = (pathlib.Path(__file__).parent / ".." / "data").resolve()
 TEST_DATA_DIR = (pathlib.Path(".").parent / "tests" / "data").resolve()
 
 PROJ_CONF_DIR = ".gmprocess"
 PROJ_CONF_FILE = "projects.conf"
 PROJECTS_PATH = (pathlib.Path("~").expanduser() / PROJ_CONF_DIR).resolve()
```

### Comparing `gmprocess-1.2.6/src/gmprocess/utils/download_utils.py` & `gmprocess-1.2.7/src/gmprocess/utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/utils/event.py` & `gmprocess-1.2.7/src/gmprocess/utils/event.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/utils/export_gmpacket_utils.py` & `gmprocess-1.2.7/src/gmprocess/utils/export_gmpacket_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,26 +234,27 @@
                 ]
                 gmp_feature_geom = FeatureGeometry(coordinates=[lon, lat, elev])
                 gmp_feature = Feature(
                     geometry=gmp_feature_geom,
                     properties=gmp_feature_props,
                 )
                 gmp_features.append(gmp_feature)
-            gmp_packet = GroundMotionPacket(
-                event=gmp_event,
-                provenance=gmp_provenance,
-                features=gmp_features,
-                version=VERSION,
-            )
-            outfile = pathlib.Path(
-                self._gmpacket_directory, f"{eventid}_groundmotion_packet.json"
-            )
-            gmp_packet.save_to_json(outfile)
-            files.append(outfile)
-            nevents += 1
+            if len(gmp_features):
+                gmp_packet = GroundMotionPacket(
+                    event=gmp_event,
+                    provenance=gmp_provenance,
+                    features=gmp_features,
+                    version=VERSION,
+                )
+                outfile = pathlib.Path(
+                    self._gmpacket_directory, f"{eventid}_groundmotion_packet.json"
+                )
+                gmp_packet.save_to_json(outfile)
+                files.append(outfile)
+                nevents += 1
 
         return (files, nevents, nstreams, ntraces)
 
     def __del__(self):
         self._workspace.close()
```

### Comparing `gmprocess-1.2.6/src/gmprocess/utils/export_shakemap_utils.py` & `gmprocess-1.2.7/src/gmprocess/utils/export_shakemap_utils.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/utils/logging.py` & `gmprocess-1.2.7/src/gmprocess/utils/logging.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/utils/models.py` & `gmprocess-1.2.7/src/gmprocess/utils/models.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/utils/plot.py` & `gmprocess-1.2.7/src/gmprocess/utils/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -420,15 +420,15 @@
         if tr.hasParameter("fit_spectra"):
             fit_spectra_dict = tr.getParameter("fit_spectra")
         else:
             fit_spectra_dict = None
 
         # ---------------------------------------------------------------------
         # Compute model spectra
-        if fit_spectra_dict is not None:
+        if (fit_spectra_dict is not None) and (smooth_signal_dict is not None):
             model_spec = spectrum.model(
                 (fit_spectra_dict["moment"], fit_spectra_dict["stress_drop"]),
                 freq=np.array(smooth_signal_dict["freq"]),
                 dist=fit_spectra_dict["epi_dist"],
                 kappa=fit_spectra_dict["kappa"],
             )
 
@@ -609,15 +609,15 @@
                 smooth_noise_dict["freq"],
                 smooth_noise_dict["spec"] / noise_norm_factor,
                 color="red",
                 alpha=0.8,
                 label="Noise",
             )
 
-        if fit_spectra_dict is not None:
+        if (fit_spectra_dict is not None) and (smooth_signal_dict is not None):
             # Model spec
             ax[j + 3 * ntrace].loglog(
                 smooth_signal_dict["freq"],
                 model_spec / signal_norm_factor,
                 color="black",
                 linestyle="dashed",
             )
```

### Comparing `gmprocess-1.2.6/src/gmprocess/utils/prompt.py` & `gmprocess-1.2.7/src/gmprocess/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/utils/report_utils.py` & `gmprocess-1.2.7/src/gmprocess/utils/report_utils.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/utils/rupture_utils.py` & `gmprocess-1.2.7/src/gmprocess/utils/rupture_utils.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/utils/tables.py` & `gmprocess-1.2.7/src/gmprocess/utils/tables.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/utils/test_utils.py` & `gmprocess-1.2.7/src/gmprocess/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/adjust_highpass.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/adjust_highpass.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/adjust_highpass_ridder.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/adjust_highpass_ridder.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/baseline_correction.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/baseline_correction.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/clipping/clip_detection.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/clipping/clip_detection.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/clipping/clipping_ann.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/clipping/clipping_ann.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/clipping/clipping_check.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/clipping/clipping_check.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/clipping/histogram.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/clipping/histogram.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/clipping/jerk.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/clipping/jerk.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/clipping/max_amp.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/clipping/max_amp.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/clipping/ping.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/clipping/ping.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/clipping/std_dev.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/clipping/std_dev.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/corner_frequencies.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/corner_frequencies.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/detrend.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/detrend.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/fft.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/fft.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/filtering.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/filtering.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/instrument_response.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/instrument_response.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/integrate.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/integrate.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/nn_quality_assurance.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/nn_quality_assurance.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/phase.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/phase.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/pretesting.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/pretesting.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/processing.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/processing.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/processing_step.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/processing_step.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/resample.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/resample.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/sanity_checks.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/snr.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/snr.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/spectrum.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/spectrum.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/taper.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/taper.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/windows.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/windows.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
 M_TO_KM = 1.0 / 1000
 
 
 def duration_from_magnitude(event_magnitude):
     """Compute shaking duration in seconds from earthquake magnitude.
 
-    From Hamid Haddadi, generic ground-motion record duration, (including 30s pre-event window:
-    Duration (minutes) = earthquake magnitude / 2.0 .
+    From Hamid Haddadi, generic ground-motion record duration, (including 30s pre-event
+    window: Duration (minutes) = earthquake magnitude / 2.0 .
 
     Args:
         event_magnitude (float):
             Earthquake magnitude.
     Returns:
         Duration of earthquake shaking in seconds.
     """
@@ -164,14 +164,27 @@
 
     Returns:
         trace with stats dict updated to include a
         stats['processing_parameters']['signal_split'] dictionary.
     """
     if config is None:
         config = get_config()
+
+    # If we are in "no noise" window mode, then set the split time to the start time
+    if config["windows"]["no_noise"]:
+        tsplit = st[0].stats.starttime
+        split_params = {
+            "split_time": tsplit,
+            "method": "no noise window",
+            "picker_type": "none",
+        }
+        for tr in st:
+            tr.setParameter("signal_split", split_params)
+        return st
+
     picker_config = config["pickers"]
 
     loc, mean_snr = pick_travel(st, event, model)
     if loc > 0:
         tsplit = st[0].stats.starttime + loc
         preferred_picker = "travel_time"
     else:
```

### Comparing `gmprocess-1.2.6/src/gmprocess/waveform_processing/zero_crossings.py` & `gmprocess-1.2.7/src/gmprocess/waveform_processing/zero_crossings.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.2.6/src/gmprocess.egg-info/PKG-INFO` & `gmprocess-1.2.7/src/gmprocess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmprocess
-Version: 1.2.6
+Version: 1.2.7
 Summary: USGS Automated Ground Motion Processing Software
 Author-email: Eric Thompson <emthompsone@usgs.gov>, Mike Hearne <mhearne@usgs.gov>, Brad Aagaard <baagaard@usgs.gov>, Bruce Worden <cbworden@contractor.usgs.gov>, John Rekoske <jrekoske@ucsd.edu>, Heather Hunsinger <hhunsinger@usgs.gov>, Gabe Ferragut <gferragut@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United States
         because it contains materials that originally came from the United States Geological Survey,
```

### Comparing `gmprocess-1.2.6/src/gmprocess.egg-info/SOURCES.txt` & `gmprocess-1.2.7/src/gmprocess.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/gmprocess.egg-info/entry_points.txt
 src/gmprocess.egg-info/requires.txt
 src/gmprocess.egg-info/top_level.txt
 src/gmprocess/apps/__init__.py
 src/gmprocess/apps/gmrecords.py
 src/gmprocess/bin/__init__.py
 src/gmprocess/bin/cwb_gather.py
+src/gmprocess/bin/fix_inventory.py
 src/gmprocess/bin/gmconvert.py
 src/gmprocess/bin/gminfo.py
 src/gmprocess/bin/gmrecords.py
 src/gmprocess/bin/gmworkspace.py
 src/gmprocess/bin/list_metrics.py
 src/gmprocess/core/__init__.py
 src/gmprocess/core/stationstream.py
```

### Comparing `gmprocess-1.2.6/src/gmprocess.egg-info/requires.txt` & `gmprocess-1.2.7/src/gmprocess.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 pyasdf>=0.7
 requests>=2.23
 ruamel.yaml>=0.17.16
 schema>=0.7
 scipy>=1.7
 setuptools-scm>=6.3.2
 statsmodels>=0.12.2
+usgs-strec>=2.2.6
 xlrd>=2.0
 
 [build]
 build
 twine
 check-wheel-contents
```


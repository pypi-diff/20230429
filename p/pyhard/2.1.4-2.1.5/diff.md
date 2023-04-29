# Comparing `tmp/pyhard-2.1.4.tar.gz` & `tmp/pyhard-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyhard-2.1.4.tar", last modified: Wed Apr 19 19:00:04 2023, max compression
+gzip compressed data, was "pyhard-2.1.5.tar", last modified: Sat Apr 29 17:11:45 2023, max compression
```

## Comparing `pyhard-2.1.4.tar` & `pyhard-2.1.5.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-04-19 18:59:55.000000 pyhard-2.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10752 2023-04-19 19:00:04.000000 pyhard-2.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8692 2023-04-19 18:59:55.000000 pyhard-2.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard/
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    34484 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/app.py
--rw-rw-rw-   0 root         (0) root         (0)    19119 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/base.py
--rw-rw-rw-   0 root         (0) root         (0)    12128 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/classification.py
--rw-rw-rw-   0 root         (0) root         (0)    20574 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard/conf/
--rw-rw-rw-   0 root         (0) root         (0)     5199 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/conf/config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    12210 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard/data/2normals/
--rw-rw-rw-   0 root         (0) root         (0)    39390 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/2normals/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    39209 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/2normals/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   242683 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/2normals/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   168248 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/2normals/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)   328455 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/2normals/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard/data/2normalsSd030/
--rw-rw-rw-   0 root         (0) root         (0)    39624 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/2normalsSd030/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    38990 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/2normalsSd030/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   130100 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/2normalsSd030/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)    94130 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/2normalsSd030/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)   284473 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/2normalsSd030/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard/data/2normalsSd045/
--rw-rw-rw-   0 root         (0) root         (0)    39780 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/2normalsSd045/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    39157 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/2normalsSd045/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   178828 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/2normalsSd045/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   131886 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/2normalsSd045/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)   318453 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/2normalsSd045/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard/data/circle/
--rw-rw-rw-   0 root         (0) root         (0)    39346 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/circle/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    40231 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/circle/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   226405 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/circle/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   145447 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/circle/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)   320526 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/circle/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard/data/easy/
--rw-rw-rw-   0 root         (0) root         (0)    40190 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/easy/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    40952 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/easy/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   147238 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/easy/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)    54473 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/easy/feature_raw_color.csv
--rw-rw-rw-   0 root         (0) root         (0)   282881 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/easy/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard/data/easy2/
--rw-rw-rw-   0 root         (0) root         (0)    39957 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/easy2/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    40817 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/easy2/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   285261 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/easy2/metadata.csv
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/easy2/projection_matrix.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard/data/iris/
--rw-rw-rw-   0 root         (0) root         (0)     5787 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/iris/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)     3877 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/iris/data.csv
--rw-rw-rw-   0 root         (0) root         (0)    42802 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/iris/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard/data/mix/
--rw-rw-rw-   0 root         (0) root         (0)    39716 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/mix/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    40903 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/mix/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   193499 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/mix/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   144369 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/mix/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)   296920 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/mix/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard/data/overlap/
--rw-rw-rw-   0 root         (0) root         (0)    39233 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/overlap/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    39752 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/overlap/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   321095 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/overlap/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard/data/separate/
--rw-rw-rw-   0 root         (0) root         (0)    39995 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/separate/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    42167 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/separate/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   177556 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/separate/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   113525 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/separate/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)   287283 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/separate/metadata.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard/data/wine/
--rw-rw-rw-   0 root         (0) root         (0)    29361 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/algorithm_bin.csv
--rw-rw-rw-   0 root         (0) root         (0)   226327 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/algorithm_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   218520 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/algorithm_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)    10101 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/beta_easy.csv
--rw-rw-rw-   0 root         (0) root         (0)    69563 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)   100951 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   163688 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/feature_process.csv
--rw-rw-rw-   0 root         (0) root         (0)   163380 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/feature_raw.csv
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/footprint_bagging_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1634 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/footprint_bagging_good.csv
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/footprint_gradient_boosting_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1726 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/footprint_gradient_boosting_good.csv
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/footprint_instance_easiness_good.csv
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/footprint_logistic_regression_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1696 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/footprint_logistic_regression_good.csv
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/footprint_mlp_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1663 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/footprint_mlp_good.csv
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/footprint_performance.csv
--rw-rw-rw-   0 root         (0) root         (0)     2760 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/footprint_random_forest_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1903 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/footprint_random_forest_good.csv
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/footprint_svc_linear_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1434 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/footprint_svc_linear_good.csv
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/footprint_svc_rbf_best.csv
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/footprint_svc_rbf_good.csv
--rw-rw-rw-   0 root         (0) root         (0)    10103 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/good_algos.csv
--rw-rw-rw-   0 root         (0) root         (0)    37458 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/ih.csv
--rw-rw-rw-   0 root         (0) root         (0)   317680 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/metadata.csv
--rw-rw-rw-   0 root         (0) root         (0)   522841 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/metadata_full.csv
--rw-rw-rw-   0 root         (0) root         (0)    10105 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/portfolio.csv
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/wine/projection_matrix.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard/data/xor/
--rw-rw-rw-   0 root         (0) root         (0)    40143 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/xor/coordinates.csv
--rw-rw-rw-   0 root         (0) root         (0)    40214 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/xor/data.csv
--rw-rw-rw-   0 root         (0) root         (0)   272866 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/xor/metadata.csv
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/data/xor/projection_matrix.csv
--rw-rw-rw-   0 root         (0) root         (0)     7659 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/feature_selection.py
--rw-rw-rw-   0 root         (0) root         (0)    10144 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/hpo.py
--rw-rw-rw-   0 root         (0) root         (0)    10847 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/integrator.py
--rw-rw-rw-   0 root         (0) root         (0)    43069 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/measures.py
--rw-rw-rw-   0 root         (0) root         (0)     3787 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard/midia/
--rw-rw-rw-   0 root         (0) root         (0)   157445 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/midia/blobs.svg
--rw-rw-rw-   0 root         (0) root         (0)    11042 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/regression.py
--rw-rw-rw-   0 root         (0) root         (0)     4123 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/structures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard/thirdparty/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/thirdparty/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    10787 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/thirdparty/entropy_estimators.py
--rw-rw-rw-   0 root         (0) root         (0)     4948 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/thirdparty/rank_aggregation.py
--rw-rw-rw-   0 root         (0) root         (0)    21966 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/thirdparty/skfeature.py
--rw-rw-rw-   0 root         (0) root         (0)     5221 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2359 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/validator.py
--rw-rw-rw-   0 root         (0) root         (0)    38600 2023-04-19 18:59:55.000000 pyhard-2.1.4/pyhard/visualization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10752 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3654 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      338 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-19 19:00:04.000000 pyhard-2.1.4/pyhard.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-19 19:00:04.000000 pyhard-2.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1794 2023-04-19 18:59:55.000000 pyhard-2.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.456764 pyhard-2.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-04-29 17:11:33.000000 pyhard-2.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9423 2023-04-29 17:11:45.456764 pyhard-2.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8692 2023-04-29 17:11:33.000000 pyhard-2.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.417760 pyhard-2.1.5/pyhard/
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    37751 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/app.py
+-rw-rw-rw-   0 root         (0) root         (0)    19119 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    12128 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)    20574 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.419760 pyhard-2.1.5/pyhard/conf/
+-rw-rw-rw-   0 root         (0) root         (0)     5199 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/conf/config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    12210 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.409759 pyhard-2.1.5/pyhard/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.422761 pyhard-2.1.5/pyhard/data/2normals/
+-rw-rw-rw-   0 root         (0) root         (0)    39390 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normals/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    39209 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normals/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   242683 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normals/feature_process.csv
+-rw-rw-rw-   0 root         (0) root         (0)   168248 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normals/feature_raw.csv
+-rw-rw-rw-   0 root         (0) root         (0)   328455 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normals/metadata.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.424761 pyhard-2.1.5/pyhard/data/2normalsSd030/
+-rw-rw-rw-   0 root         (0) root         (0)    39624 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd030/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    38990 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd030/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   130100 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd030/feature_process.csv
+-rw-rw-rw-   0 root         (0) root         (0)    94130 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd030/feature_raw.csv
+-rw-rw-rw-   0 root         (0) root         (0)   284473 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd030/metadata.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.426761 pyhard-2.1.5/pyhard/data/2normalsSd045/
+-rw-rw-rw-   0 root         (0) root         (0)    39780 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd045/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    39157 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd045/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   178828 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd045/feature_process.csv
+-rw-rw-rw-   0 root         (0) root         (0)   131886 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd045/feature_raw.csv
+-rw-rw-rw-   0 root         (0) root         (0)   318453 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/2normalsSd045/metadata.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.429761 pyhard-2.1.5/pyhard/data/circle/
+-rw-rw-rw-   0 root         (0) root         (0)    39346 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/circle/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    40231 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/circle/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   226405 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/circle/feature_process.csv
+-rw-rw-rw-   0 root         (0) root         (0)   145447 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/circle/feature_raw.csv
+-rw-rw-rw-   0 root         (0) root         (0)   320526 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/circle/metadata.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.431762 pyhard-2.1.5/pyhard/data/easy/
+-rw-rw-rw-   0 root         (0) root         (0)    40190 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/easy/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    40952 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/easy/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   147238 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/easy/feature_process.csv
+-rw-rw-rw-   0 root         (0) root         (0)    54473 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/easy/feature_raw_color.csv
+-rw-rw-rw-   0 root         (0) root         (0)   282881 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/easy/metadata.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.433762 pyhard-2.1.5/pyhard/data/easy2/
+-rw-rw-rw-   0 root         (0) root         (0)    39957 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/easy2/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    40817 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/easy2/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   285261 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/easy2/metadata.csv
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/easy2/projection_matrix.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.434762 pyhard-2.1.5/pyhard/data/iris/
+-rw-rw-rw-   0 root         (0) root         (0)     5787 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/iris/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3877 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/iris/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)    42802 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/iris/metadata.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.436762 pyhard-2.1.5/pyhard/data/mix/
+-rw-rw-rw-   0 root         (0) root         (0)    39716 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/mix/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    40903 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/mix/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   193499 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/mix/feature_process.csv
+-rw-rw-rw-   0 root         (0) root         (0)   144369 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/mix/feature_raw.csv
+-rw-rw-rw-   0 root         (0) root         (0)   296920 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/mix/metadata.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.438762 pyhard-2.1.5/pyhard/data/overlap/
+-rw-rw-rw-   0 root         (0) root         (0)    39233 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/overlap/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    39752 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/overlap/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   321095 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/overlap/metadata.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.440762 pyhard-2.1.5/pyhard/data/separate/
+-rw-rw-rw-   0 root         (0) root         (0)    39995 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/separate/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    42167 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/separate/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   177556 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/separate/feature_process.csv
+-rw-rw-rw-   0 root         (0) root         (0)   113525 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/separate/feature_raw.csv
+-rw-rw-rw-   0 root         (0) root         (0)   287283 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/separate/metadata.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.453764 pyhard-2.1.5/pyhard/data/wine/
+-rw-rw-rw-   0 root         (0) root         (0)    29361 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/algorithm_bin.csv
+-rw-rw-rw-   0 root         (0) root         (0)   226327 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/algorithm_process.csv
+-rw-rw-rw-   0 root         (0) root         (0)   218520 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/algorithm_raw.csv
+-rw-rw-rw-   0 root         (0) root         (0)    10101 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/beta_easy.csv
+-rw-rw-rw-   0 root         (0) root         (0)    69563 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)   100951 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   163688 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/feature_process.csv
+-rw-rw-rw-   0 root         (0) root         (0)   163380 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/feature_raw.csv
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_bagging_best.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1634 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_bagging_good.csv
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_gradient_boosting_best.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_gradient_boosting_good.csv
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_instance_easiness_good.csv
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_logistic_regression_best.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1696 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_logistic_regression_good.csv
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_mlp_best.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1663 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_mlp_good.csv
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_performance.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_random_forest_best.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_random_forest_good.csv
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_svc_linear_best.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1434 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_svc_linear_good.csv
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_svc_rbf_best.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/footprint_svc_rbf_good.csv
+-rw-rw-rw-   0 root         (0) root         (0)    10103 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/good_algos.csv
+-rw-rw-rw-   0 root         (0) root         (0)    37458 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/ih.csv
+-rw-rw-rw-   0 root         (0) root         (0)   317680 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/metadata.csv
+-rw-rw-rw-   0 root         (0) root         (0)   522841 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/metadata_full.csv
+-rw-rw-rw-   0 root         (0) root         (0)    10105 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/portfolio.csv
+-rw-rw-rw-   0 root         (0) root         (0)      231 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/wine/projection_matrix.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.454764 pyhard-2.1.5/pyhard/data/xor/
+-rw-rw-rw-   0 root         (0) root         (0)    40143 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/xor/coordinates.csv
+-rw-rw-rw-   0 root         (0) root         (0)    40214 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/xor/data.csv
+-rw-rw-rw-   0 root         (0) root         (0)   272866 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/xor/metadata.csv
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/data/xor/projection_matrix.csv
+-rw-rw-rw-   0 root         (0) root         (0)     7659 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/feature_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)    10144 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/hpo.py
+-rw-rw-rw-   0 root         (0) root         (0)    10847 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/integrator.py
+-rw-rw-rw-   0 root         (0) root         (0)    43069 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/measures.py
+-rw-rw-rw-   0 root         (0) root         (0)     3787 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.455764 pyhard-2.1.5/pyhard/midia/
+-rw-rw-rw-   0 root         (0) root         (0)   157445 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/midia/blobs.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11042 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/regression.py
+-rw-rw-rw-   0 root         (0) root         (0)     4123 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/structures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.456764 pyhard-2.1.5/pyhard/thirdparty/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/thirdparty/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10787 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/thirdparty/entropy_estimators.py
+-rw-rw-rw-   0 root         (0) root         (0)     4948 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/thirdparty/rank_aggregation.py
+-rw-rw-rw-   0 root         (0) root         (0)    21966 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/thirdparty/skfeature.py
+-rw-rw-rw-   0 root         (0) root         (0)     5221 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2359 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/validator.py
+-rw-rw-rw-   0 root         (0) root         (0)    38600 2023-04-29 17:11:33.000000 pyhard-2.1.5/pyhard/visualization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 17:11:45.419760 pyhard-2.1.5/pyhard.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9423 2023-04-29 17:11:45.000000 pyhard-2.1.5/pyhard.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3654 2023-04-29 17:11:45.000000 pyhard-2.1.5/pyhard.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 17:11:45.000000 pyhard-2.1.5/pyhard.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-04-29 17:11:45.000000 pyhard-2.1.5/pyhard.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      338 2023-04-29 17:11:45.000000 pyhard-2.1.5/pyhard.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-29 17:11:45.000000 pyhard-2.1.5/pyhard.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-29 17:11:45.457764 pyhard-2.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2023-04-29 17:11:33.000000 pyhard-2.1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyhard-2.1.4/LICENSE` & `pyhard-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/PKG-INFO` & `pyhard-2.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,185 +1,185 @@
 Metadata-Version: 2.1
 Name: pyhard
-Version: 2.1.4
+Version: 2.1.5
 Summary: Analyze, explore and visualize instance hardness within datasets
 Home-page: https://gitlab.com/ita-ml/pyhard
+Download-URL: https://gitlab.com/ita-ml/pyhard/-/archive/v2.1.5/pyhard-v2.1.5.tar.gz
 Author: Pedro Paiva
 Author-email: paiva@ita.br
 License: MIT
-Download-URL: https://gitlab.com/ita-ml/pyhard/-/archive/v2.1.4/pyhard-v2.1.4.tar.gz
-Description: <!--
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/ita-ml%2Finstance-hardness/binder?filepath=notebooks%2F)
-        [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-        [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://en.wikipedia.org/wiki/MIT_License)
-        -->
-        
-        # PyHard
-        
-        Instance Hardness analysis in Python, with a two-fold objective: insights on data quality issues; 
-        and better understanding of the weaknesses and strengths of different algorithms.
-        
-        * Documentation: https://ita-ml.gitlab.io/pyhard/
-        * Source code: https://gitlab.com/ita-ml/pyhard
-        * Bug reports: https://gitlab.com/ita-ml/pyhard/-/issues
-        
-        ## Getting Started
-        
-        PyHard employes a methodology known as [_Instance Space Analysis_](https://github.com/andremun/InstanceSpace) (ISA) to analyse performance at the instance level rather than at dataset level. The result is an alternative for visualizing algorithm performance for each instance within a dataset, by relating predictive performance to estimated instance hardness measures extracted from the data. This analysis reveals regions of strengths and weaknesses of predictors (aka _footprints_), and highlights individual instances within a  dataset that warrant further investigation, either due to their unique properties or potential data quality issues.
-        
-        
-        ### Installation
-        Although the original ISA toolkit has been written in Matlab, we provide a lighter version in Python, with less tools, but enough for the instance hardness analysis purposes. You may find the implementation in the separate package [PyISpace](https://gitlab.com/ita-ml/pyispace). Notwithstanding, the choice of the ISA engine is left up to the user, which can be set in the configuration file. Below, we present the standard installation, and also the the additional steps to configure the Matlab engine (optional).
-        
-        _For users_
-        
-        ```
-        pip install pyhard
-        ```
-        
-        _For developers_
-        
-        Alternatively, if you are a developer and want to contribute, the following installation is better suited for testing new features:
-        ```
-        git clone https://gitlab.com/ita-ml/pyhard.git
-        cd pyhard
-        pip install -e .
-        ```
-        
-        #### Anaconda environment
-        
-        We **strongly recommend** using a separate Python environment. We provide an env file [environment.yml](./environment.yml) to create a conda env with all required dependencies:
-        
-        ```
-        conda env create --file environment.yml
-        ```
-        
-        
-        ### Usage
-        
-        First, make sure that the configuration files are placed within the current directory and the settings are the desired ones. To generate those files, run
-        
-        ```
-        pyhard init
-        ```
-        
-        This will create both `config.yaml` and `options.json` in the current directory.
-        
-        The file `config.yaml` is used to configurate steps 1-4 below. Through it, options for file paths, measures, classifiers, feature selection and hyper-parameter optimization can be set. More instructions can be found in the comments within the file.
-        
-        At least the field `datafile` (in section 'general') should be set in `config.yaml`. It specifies the path (absolute or relative) of the input dataset. Leaving the field `rootdir` as `'.'` (default), the output files will be saved in the current folder along with the configuration files (recommended).
-        
-        Once everything is configured, run the analysis:
-        
-        ```
-        pyhard run
-        ```
-        
-        By default, the following steps shall be taken:
-        
-        1. Calculate the _hardness measures_;
-        
-        2. Evaluate classification performance at instance level for each algorithm;
-        
-        3. Select the most relevant hardness measures with respect to the instance classification error;
-        
-        4. Join the outputs of steps 1, 2 and 3 to build the _metadata_ file (`metadata.csv`);
-        
-        5. Run __ISA__ (_Instance Space Analysis_), which generates the _Instance Space_ (IS) representation and the _footprint_ areas;
-        
-        Steps 1 to 4 comprise the metadata construction, and step 5 the ISA itself. To curb any of these two major stages, use the options with command `run`:
-        
-        * `--no-meta`: does not attempt to build the metadata file
-        
-        * `--no-isa`: prevents the Instance Space Analysis
-        
-        Finally, to explore the results, launch the app:  
-        
-        ```
-        pyhard app
-        ```
-        
-        To see all CLI commands, run `pyhard --help`, or `pyhard run --help` to get the options for this command.
-        
-        
-        ### Guidelines for input dataset
-        
-        Please follow the recommendations below:
-        
-        * Only `csv` files are accepted
-        
-        * The dataset should be in the format `(n_instances, n_features)`
-        
-        * It cannot contains NaNs or missing values
-        
-        * **Do not** include any index column. Instances will be indexed in order, starting from **1**
-        
-        * **The last column** should contain the target variable (`y`). Otherwise, the name of the target column must be declared in the field `target_col` (config file)
-        
-        * Categorical features should be handled previously
-        
-        
-        ## Citation
-        
-        If you're using PyHard in your research or application, please cite our [paper](https://link.springer.com/article/10.1007/s10994-022-06205-9):
-        
-        > Paiva, P. Y. A., Moreno, C. C., Smith-Miles, K., Valeriano, M. G., & Lorena, A. C. (2022). Relating instance hardness to classification performance in a dataset: a visual approach. Machine Learning, 111(8), 3085-3123. https://doi.org/10.1007/s10994-022-06205-9
-        
-        ```
-        @article{paiva2022relating,
-              title={Relating instance hardness to classification performance in a dataset: a visual approach},
-              author={Paiva, Pedro Yuri Arbs and Moreno, Camila Castro and Smith-Miles, Kate and Valeriano, Maria Gabriela and Lorena, Ana Carolina},
-              journal={Machine Learning},
-              volume={111},
-              number={8},
-              pages={3085--3123},
-              year={2022},
-              publisher={Springer}
-        }
-        ```
-        
-        
-        ## References
-        
-        _Base_
-        
-        1. Michael R. Smith, Tony Martinez, and Christophe Giraud-Carrier. 2014. __An instance level analysis of data complexity__. Mach. Learn. 95, 2 (May 2014), 225–256.
-        
-        2. Ana C. Lorena, Luís P. F. Garcia, Jens Lehmann, Marcilio C. P. Souto, and Tin Kam Ho. 2019. __How Complex Is Your Classification Problem? A Survey on Measuring Classification Complexity__. ACM Comput. Surv. 52, 5, Article 107 (October 2019), 34 pages.
-        
-        3. Mario A. Muñoz, Laura Villanova, Davaatseren Baatar, and Kate Smith-Miles. 2018. __Instance spaces for machine learning classification__. Mach. Learn. 107, 1 (January   2018), 109–147.
-        
-        _Feature selection_
-        
-        4. Luiz H. Lorena, André C. Carvalho, and Ana C. Lorena. 2015. __Filter Feature Selection for One-Class Classification__. Journal of Intelligent and Robotic Systems 80, 1 (October   2015), 227–243.
-        
-        5. Goldberger, J., Hinton, G., Roweis, S., Salakhutdinov, R. (2005). __Neighbourhood Components Analysis__. Advances in Neural Information Processing Systems. 17, 513-520.
-        
-        6. Yang, W., Wang, K., & Zuo, W. (2012). __Neighborhood component feature selection for high-dimensional data__. J. Comput., 7(1), 161-168.
-        
-        7. Amankwaa-Kyeremeh, B., Greet, C., Zanin, M., Skinner, W. and Asamoah, R. K., (2020), __Selecting key predictor parameters for regression analysis using modified Neighbourhood Component Analysis (NCA) Algorithm__. Proceedings of 6th UMaT Biennial International Mining and Mineral Conference, Tarkwa, Ghana, pp. 320-325.
-        
-        8. Artur J. Ferreira and Mário A. T. Figueiredo. 2012. __Efficient feature selection filters for high-dimensional data__. Pattern Recognition Letters 33, 13 (October, 2012), 1794–1804.
-        
-        9. Jundong Li, Kewei Cheng, Suhang Wang, Fred Morstatter, Robert P. Trevino, Jiliang Tang, and Huan Liu. 2017. __Feature Selection: A Data Perspective__. ACM Comput. Surv. 50, 6, Article 94 (January 2018), 45 pages.
-        
-        10. Shuyang Gao, Greg Ver Steeg, and Aram Galstyan. __Efficient Estimation of Mutual Information for Strongly Dependent Variables__. Available in http://arxiv.org/abs/1411.2003. AISTATS, 2015.
-        
-        _Hyper parameter optimization_
-        
-        11. James Bergstra, Rémi Bardenet, Yoshua Bengio, and Balázs Kégl. 2011. __Algorithms for hyper-parameter optimization__. In Proceedings of the 24th International Conference on Neural Information Processing Systems (NIPS’11). Curran Associates Inc., Red Hook, NY, USA, 2546–2554.
-        
-        12. Jasper Snoek, Hugo Larochelle, and Ryan P. Adams. 2012. __Practical Bayesian optimization of machine learning algorithms__. In Proceedings of the 25th International Conference on Neural Information Processing Systems - Volume 2 (NIPS’12). Curran Associates Inc., Red Hook, NY, USA, 2951–2959.
-          
-        13. J. Bergstra, D. Yamins, and D. D. Cox. 2013. __Making a science of model search: hyperparameter optimization in hundreds of dimensions for vision architectures__. In Proceedings of the 30th International Conference on International Conference on Machine Learning - Volume 28 (ICML’13). JMLR.org, I–115–I–123.
-          
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
+License-File: LICENSE
+
+<!--
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/ita-ml%2Finstance-hardness/binder?filepath=notebooks%2F)
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+[![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://en.wikipedia.org/wiki/MIT_License)
+-->
+
+# PyHard
+
+Instance Hardness analysis in Python, with a two-fold objective: insights on data quality issues; 
+and better understanding of the weaknesses and strengths of different algorithms.
+
+* Documentation: https://ita-ml.gitlab.io/pyhard/
+* Source code: https://gitlab.com/ita-ml/pyhard
+* Bug reports: https://gitlab.com/ita-ml/pyhard/-/issues
+
+## Getting Started
+
+PyHard employes a methodology known as [_Instance Space Analysis_](https://github.com/andremun/InstanceSpace) (ISA) to analyse performance at the instance level rather than at dataset level. The result is an alternative for visualizing algorithm performance for each instance within a dataset, by relating predictive performance to estimated instance hardness measures extracted from the data. This analysis reveals regions of strengths and weaknesses of predictors (aka _footprints_), and highlights individual instances within a  dataset that warrant further investigation, either due to their unique properties or potential data quality issues.
+
+
+### Installation
+Although the original ISA toolkit has been written in Matlab, we provide a lighter version in Python, with less tools, but enough for the instance hardness analysis purposes. You may find the implementation in the separate package [PyISpace](https://gitlab.com/ita-ml/pyispace). Notwithstanding, the choice of the ISA engine is left up to the user, which can be set in the configuration file. Below, we present the standard installation, and also the the additional steps to configure the Matlab engine (optional).
+
+_For users_
+
+```
+pip install pyhard
+```
+
+_For developers_
+
+Alternatively, if you are a developer and want to contribute, the following installation is better suited for testing new features:
+```
+git clone https://gitlab.com/ita-ml/pyhard.git
+cd pyhard
+pip install -e .
+```
+
+#### Anaconda environment
+
+We **strongly recommend** using a separate Python environment. We provide an env file [environment.yml](./environment.yml) to create a conda env with all required dependencies:
+
+```
+conda env create --file environment.yml
+```
+
+
+### Usage
+
+First, make sure that the configuration files are placed within the current directory and the settings are the desired ones. To generate those files, run
+
+```
+pyhard init
+```
+
+This will create both `config.yaml` and `options.json` in the current directory.
+
+The file `config.yaml` is used to configurate steps 1-4 below. Through it, options for file paths, measures, classifiers, feature selection and hyper-parameter optimization can be set. More instructions can be found in the comments within the file.
+
+At least the field `datafile` (in section 'general') should be set in `config.yaml`. It specifies the path (absolute or relative) of the input dataset. Leaving the field `rootdir` as `'.'` (default), the output files will be saved in the current folder along with the configuration files (recommended).
+
+Once everything is configured, run the analysis:
+
+```
+pyhard run
+```
+
+By default, the following steps shall be taken:
+
+1. Calculate the _hardness measures_;
+
+2. Evaluate classification performance at instance level for each algorithm;
+
+3. Select the most relevant hardness measures with respect to the instance classification error;
+
+4. Join the outputs of steps 1, 2 and 3 to build the _metadata_ file (`metadata.csv`);
+
+5. Run __ISA__ (_Instance Space Analysis_), which generates the _Instance Space_ (IS) representation and the _footprint_ areas;
+
+Steps 1 to 4 comprise the metadata construction, and step 5 the ISA itself. To curb any of these two major stages, use the options with command `run`:
+
+* `--no-meta`: does not attempt to build the metadata file
+
+* `--no-isa`: prevents the Instance Space Analysis
+
+Finally, to explore the results, launch the app:  
+
+```
+pyhard app
+```
+
+To see all CLI commands, run `pyhard --help`, or `pyhard run --help` to get the options for this command.
+
+
+### Guidelines for input dataset
+
+Please follow the recommendations below:
+
+* Only `csv` files are accepted
+
+* The dataset should be in the format `(n_instances, n_features)`
+
+* It cannot contains NaNs or missing values
+
+* **Do not** include any index column. Instances will be indexed in order, starting from **1**
+
+* **The last column** should contain the target variable (`y`). Otherwise, the name of the target column must be declared in the field `target_col` (config file)
+
+* Categorical features should be handled previously
+
+
+## Citation
+
+If you're using PyHard in your research or application, please cite our [paper](https://link.springer.com/article/10.1007/s10994-022-06205-9):
+
+> Paiva, P. Y. A., Moreno, C. C., Smith-Miles, K., Valeriano, M. G., & Lorena, A. C. (2022). Relating instance hardness to classification performance in a dataset: a visual approach. Machine Learning, 111(8), 3085-3123. https://doi.org/10.1007/s10994-022-06205-9
+
+```
+@article{paiva2022relating,
+      title={Relating instance hardness to classification performance in a dataset: a visual approach},
+      author={Paiva, Pedro Yuri Arbs and Moreno, Camila Castro and Smith-Miles, Kate and Valeriano, Maria Gabriela and Lorena, Ana Carolina},
+      journal={Machine Learning},
+      volume={111},
+      number={8},
+      pages={3085--3123},
+      year={2022},
+      publisher={Springer}
+}
+```
+
+
+## References
+
+_Base_
+
+1. Michael R. Smith, Tony Martinez, and Christophe Giraud-Carrier. 2014. __An instance level analysis of data complexity__. Mach. Learn. 95, 2 (May 2014), 225–256.
+
+2. Ana C. Lorena, Luís P. F. Garcia, Jens Lehmann, Marcilio C. P. Souto, and Tin Kam Ho. 2019. __How Complex Is Your Classification Problem? A Survey on Measuring Classification Complexity__. ACM Comput. Surv. 52, 5, Article 107 (October 2019), 34 pages.
+
+3. Mario A. Muñoz, Laura Villanova, Davaatseren Baatar, and Kate Smith-Miles. 2018. __Instance spaces for machine learning classification__. Mach. Learn. 107, 1 (January   2018), 109–147.
+
+_Feature selection_
+
+4. Luiz H. Lorena, André C. Carvalho, and Ana C. Lorena. 2015. __Filter Feature Selection for One-Class Classification__. Journal of Intelligent and Robotic Systems 80, 1 (October   2015), 227–243.
+
+5. Goldberger, J., Hinton, G., Roweis, S., Salakhutdinov, R. (2005). __Neighbourhood Components Analysis__. Advances in Neural Information Processing Systems. 17, 513-520.
+
+6. Yang, W., Wang, K., & Zuo, W. (2012). __Neighborhood component feature selection for high-dimensional data__. J. Comput., 7(1), 161-168.
+
+7. Amankwaa-Kyeremeh, B., Greet, C., Zanin, M., Skinner, W. and Asamoah, R. K., (2020), __Selecting key predictor parameters for regression analysis using modified Neighbourhood Component Analysis (NCA) Algorithm__. Proceedings of 6th UMaT Biennial International Mining and Mineral Conference, Tarkwa, Ghana, pp. 320-325.
+
+8. Artur J. Ferreira and Mário A. T. Figueiredo. 2012. __Efficient feature selection filters for high-dimensional data__. Pattern Recognition Letters 33, 13 (October, 2012), 1794–1804.
+
+9. Jundong Li, Kewei Cheng, Suhang Wang, Fred Morstatter, Robert P. Trevino, Jiliang Tang, and Huan Liu. 2017. __Feature Selection: A Data Perspective__. ACM Comput. Surv. 50, 6, Article 94 (January 2018), 45 pages.
+
+10. Shuyang Gao, Greg Ver Steeg, and Aram Galstyan. __Efficient Estimation of Mutual Information for Strongly Dependent Variables__. Available in http://arxiv.org/abs/1411.2003. AISTATS, 2015.
+
+_Hyper parameter optimization_
+
+11. James Bergstra, Rémi Bardenet, Yoshua Bengio, and Balázs Kégl. 2011. __Algorithms for hyper-parameter optimization__. In Proceedings of the 24th International Conference on Neural Information Processing Systems (NIPS’11). Curran Associates Inc., Red Hook, NY, USA, 2546–2554.
+
+12. Jasper Snoek, Hugo Larochelle, and Ryan P. Adams. 2012. __Practical Bayesian optimization of machine learning algorithms__. In Proceedings of the 25th International Conference on Neural Information Processing Systems - Volume 2 (NIPS’12). Curran Associates Inc., Red Hook, NY, USA, 2951–2959.
+  
+13. J. Bergstra, D. Yamins, and D. D. Cox. 2013. __Making a science of model search: hyperparameter optimization in hundreds of dimensions for vision architectures__. In Proceedings of the 30th International Conference on International Conference on Machine Learning - Volume 28 (ICML’13). JMLR.org, I–115–I–123.
+
```

### Comparing `pyhard-2.1.4/README.md` & `pyhard-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/__init__.py` & `pyhard-2.1.5/pyhard/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 from pathlib import Path
 from typing import Union
 
 
-__version__ = "2.1.4"
+__version__ = "2.1.5"
 
 
 def get_seed() -> Union[int, None]:
     seed = os.environ.get("PYHARD_SEED")
     if seed is None:
         return seed
     else:
```

### Comparing `pyhard-2.1.4/pyhard/app.py` & `pyhard-2.1.5/pyhard/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import holoviews as hv
 import numpy as np
 import pandas as pd
 import panel as pn
 import plotly.express as px
 import plotly.io as pio
+import plotly.graph_objects as go
 from bokeh.colors import RGB
 from bokeh.core.enums import MarkerType
 from bokeh.models import HoverTool
 from bokeh.settings import settings
 from holoviews import opts, dim
 from holoviews.streams import PlotReset, SelectionExpr
 from matplotlib import cm
@@ -42,14 +43,19 @@
 transparent = 'rgba(0,0,0,0)'
 footprint_colors = {'good': '#58D68D', 'best': '#9B59B6'}
 
 colorbar_opts = {'background_fill_color': transparent}
 grid_opts = {'grid_line_dash': [6, 4], 'grid_line_alpha': .5}
 control_width = 280
 
+pn.extension('plotly')
+hv.extension('bokeh')
+pn.extension(notifications=True)
+pn.state.notifications.position = 'bottom-left'
+
 
 @dataclass
 class Content:
     name: str = ""
     main: Any = None
     control: Any = None
 
@@ -68,17 +74,14 @@
 
     Args:
         workspace (Workspace): loaded workspace instance
     """
     _tabs_labels = ['Instance Space', 'Footprint Performance', 'Distributions', 'Data Explorer']
 
     def __init__(self, workspace: Workspace):
-        pn.extension('plotly')
-        hv.extension('bokeh')
-
         self.workspace = workspace
         self.bbox = None
         self.cmap = 'coolwarm'
         self.tabs = pn.Tabs(*[(name, None) for name in self._tabs_labels], dynamic=False)
 
         self.all_cols = (
                 workspace.data.columns.to_list() +
@@ -151,21 +154,32 @@
             solid=False
         )
 
         # Data explorer tab widgets
         self.w_var_y = pn.widgets.Select(name='y-axis', options=self.all_cols, value='z_2')
         self.w_var_x = pn.widgets.Select(name='x-axis', options=self.all_cols, value='z_1')
         self.w_var_c = pn.widgets.Select(name='Color', options=self.all_cols, value=self.output_col)
+        self.w_filter = pn.widgets.TextInput(name='Filtering', placeholder='Pandas query like')
+        info_text = "Expressions create new columns;\n" \
+                    "enter one per line (e.g. A=z_1**2).\n\n" \
+                    "Arithmetic operations supported: \n" \
+                    "+, -, *, /, **, % \n" \
+                    "Some functions are also supported: \n" \
+                    "sqrt, log, sin, cos, ...\n" \
+                    "Boolean operations: \n" \
+                    "| (or), & (and), and ~ (not)"
+        self.w_eval = pn.widgets.TextAreaInput(name='Evaluate expression', placeholder=info_text, height=220)
         self.w_var_cm = pn.widgets.RadioButtonGroup(
             name='Color map',
             options=['Continuous', 'Discrete'],
             button_type='default',
             value='Continuous'
         )
         self.w_var_s = pn.widgets.DiscreteSlider(name='Size', options=list(range(1, 16)), value=7)
+        self.explorer_data = None
 
         val = 'instance_easiness' if 'instance_easiness' in df_footprint.index else ''
         self.w_footprint_algo = pn.widgets.Select(options=df_footprint.index.unique(level='algo').to_list(), value=val)
 
         # Download
         self.w_group_data = pn.widgets.CheckButtonGroup(
             name='Data sources',
@@ -593,64 +607,135 @@
             pn.Spacer(),
             self.w_dist_type,
             self.w_dist_var,
             width=control_width
         )
 
     def render_explorer_panel(self):
-        @pn.depends(a=self.tabs.param.active, x=self.w_var_x, y=self.w_var_y, c=self.w_var_c.param.value)
-        def plot_scatter(a, x, y, c):
+        @pn.depends(
+            a=self.tabs.param.active,
+            x=self.w_var_x,
+            y=self.w_var_y,
+            c=self.w_var_c.param.value,
+            filter_expr=self.w_filter.param.value,
+            eval_expr=self.w_eval.param.value
+        )
+        def plot_scatter(a, x, y, c, filter_expr, eval_expr):
             if a != 3:
                 return ""
             mask = self.select_instances()
             output_col = self.output_col
             df_all = self.workspace.data[mask].copy()
             df_all = df_all.join(self.workspace.extended_metadata, how='left')
             df_all = df_all.join(self.workspace.is_coordinates, how='left')
+
+            if eval_expr != "":
+                try:
+                    df_all = df_all.eval(eval_expr)
+                    new_cols = set(df_all.columns) - set(self.all_cols)
+                    self.w_var_c.options = self.all_cols + list(new_cols)
+                except:
+                    self.w_var_c.options = self.all_cols
+                    pn.state.notifications.error('Invalid evaluated expression.', duration=4000)
+            else:
+                self.w_var_c.options = self.all_cols
+            if c not in self.w_var_c.options:
+                c = self.w_var_c.value = self.output_col
+
+            try:
+                idx = df_all.query(filter_expr).index if filter_expr != "" else df_all.index
+                background = ~df_all.index.isin(idx)
+            except:
+                background = ~df_all.index.isin(df_all.index)
+                pn.state.notifications.error('Invalid filtering expression.', duration=4000)
+
             df_all.loc[:, output_col] = df_all[output_col].apply(lambda v: str(v))
             classes = df_all[output_col].unique().tolist()
             classes.sort()
             category_orders = {output_col: classes}
+            range_color = (df_all[c].min(), df_all[c].max())
+            self.explorer_data = df_all[~background].copy()
 
-            fig_plotly = px.scatter(
-                df_all,
+            fig1 = px.scatter(
+                df_all[~background],
+                x=x,
+                y=y,
+                color=c,
+                symbol=self.output_col,
+                size_max=7,
+                opacity=1,
+                # marginal_x="histogram",
+                # marginal_y="histogram",
+                category_orders=category_orders,
+                range_color=range_color
+            )
+            fig2 = px.scatter(
+                df_all[background],
                 x=x,
                 y=y,
                 color=c,
                 symbol=self.output_col,
+                size_max=7,
+                opacity=0.1,
                 # marginal_x="histogram",
                 # marginal_y="histogram",
-                category_orders=category_orders
+                category_orders=category_orders,
+                range_color=range_color
             )
+            fig_plotly = go.Figure(data=fig1.data + fig2.data, layout=fig1.layout)
+
             fig_plotly.update_layout(
                 margin=dict(l=0, r=0, t=20, b=10),
                 paper_bgcolor='rgba(0,0,0,0)',
                 modebar={'bgcolor': 'rgba(255,255,255,0)'},
                 font_family="'Source Sans Pro', verdana, arial",
                 legend_font_size=15,
                 font_size=16,
                 legend=dict(
                     orientation="h",
                     yanchor="bottom",
                     y=1.02,
                     xanchor="left",
                     x=0
-                )
+                ),
+                coloraxis={'colorscale': coolwarm_cmap}
             )
-            fig_plotly.update_traces(marker=dict(size=7))
+            # fig_plotly.update_traces(marker=dict(size=7))
             fig_plotly.layout.autosize = True
             return pn.Column(
                 pn.Spacer(),
                 pn.pane.Plotly(fig_plotly, aspect_ratio=2),
                 sizing_mode="stretch_width"
             )
 
+        def download_data():
+            return BytesIO(self.explorer_data.to_csv().encode())
+
+        button_download = pn.widgets.FileDownload(
+            embed=False,
+            auto=True,
+            callback=download_data,
+            filename='data.csv',
+            label='Save explorer data',
+            button_type='default'
+        )
+
         self.layout.explorer.name = self._tabs_labels[3]
         self.layout.explorer.main = plot_scatter
-        self.layout.explorer.control = pn.Column(self.w_var_x, self.w_var_y, self.w_var_c, width=control_width)
+        self.layout.explorer.control = pn.Column(
+            self.w_var_x,
+            self.w_var_y,
+            self.w_var_c,
+            pn.layout.Divider(sizing_mode='stretch_width'),
+            self.w_filter,
+            self.w_eval,
+            pn.Spacer(height=20),
+            button_download,
+            width=control_width
+        )
 
     def populate_tabs(self):
         """
         Populates the panel tabs.
         """
         self.tabs[0] = (self.layout.space.name, self.layout.space.main)
         self.tabs[1] = (self.layout.performance.name, self.layout.performance.main)
```

### Comparing `pyhard-2.1.4/pyhard/base.py` & `pyhard-2.1.5/pyhard/base.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/classification.py` & `pyhard-2.1.5/pyhard/classification.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/cli.py` & `pyhard-2.1.5/pyhard/cli.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/conf/config.yaml` & `pyhard-2.1.5/pyhard/conf/config.yaml`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/context.py` & `pyhard-2.1.5/pyhard/context.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/2normals/coordinates.csv` & `pyhard-2.1.5/pyhard/data/2normals/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/2normals/data.csv` & `pyhard-2.1.5/pyhard/data/2normals/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/2normals/feature_process.csv` & `pyhard-2.1.5/pyhard/data/2normals/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/2normals/feature_raw.csv` & `pyhard-2.1.5/pyhard/data/2normals/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/2normals/metadata.csv` & `pyhard-2.1.5/pyhard/data/2normals/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/2normalsSd030/coordinates.csv` & `pyhard-2.1.5/pyhard/data/2normalsSd030/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/2normalsSd030/data.csv` & `pyhard-2.1.5/pyhard/data/2normalsSd030/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/2normalsSd030/feature_process.csv` & `pyhard-2.1.5/pyhard/data/2normalsSd030/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/2normalsSd030/feature_raw.csv` & `pyhard-2.1.5/pyhard/data/2normalsSd030/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/2normalsSd030/metadata.csv` & `pyhard-2.1.5/pyhard/data/2normalsSd030/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/2normalsSd045/coordinates.csv` & `pyhard-2.1.5/pyhard/data/2normalsSd045/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/2normalsSd045/data.csv` & `pyhard-2.1.5/pyhard/data/2normalsSd045/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/2normalsSd045/feature_process.csv` & `pyhard-2.1.5/pyhard/data/2normalsSd045/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/2normalsSd045/feature_raw.csv` & `pyhard-2.1.5/pyhard/data/2normalsSd045/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/2normalsSd045/metadata.csv` & `pyhard-2.1.5/pyhard/data/2normalsSd045/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/circle/coordinates.csv` & `pyhard-2.1.5/pyhard/data/circle/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/circle/data.csv` & `pyhard-2.1.5/pyhard/data/circle/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/circle/feature_process.csv` & `pyhard-2.1.5/pyhard/data/circle/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/circle/feature_raw.csv` & `pyhard-2.1.5/pyhard/data/circle/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/circle/metadata.csv` & `pyhard-2.1.5/pyhard/data/circle/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/easy/coordinates.csv` & `pyhard-2.1.5/pyhard/data/easy/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/easy/data.csv` & `pyhard-2.1.5/pyhard/data/easy/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/easy/feature_process.csv` & `pyhard-2.1.5/pyhard/data/easy/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/easy/feature_raw_color.csv` & `pyhard-2.1.5/pyhard/data/easy/feature_raw_color.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/easy/metadata.csv` & `pyhard-2.1.5/pyhard/data/easy/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/easy2/coordinates.csv` & `pyhard-2.1.5/pyhard/data/easy2/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/easy2/data.csv` & `pyhard-2.1.5/pyhard/data/easy2/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/easy2/metadata.csv` & `pyhard-2.1.5/pyhard/data/easy2/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/iris/coordinates.csv` & `pyhard-2.1.5/pyhard/data/iris/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/iris/data.csv` & `pyhard-2.1.5/pyhard/data/iris/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/iris/metadata.csv` & `pyhard-2.1.5/pyhard/data/iris/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/mix/coordinates.csv` & `pyhard-2.1.5/pyhard/data/mix/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/mix/data.csv` & `pyhard-2.1.5/pyhard/data/mix/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/mix/feature_process.csv` & `pyhard-2.1.5/pyhard/data/mix/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/mix/feature_raw.csv` & `pyhard-2.1.5/pyhard/data/mix/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/mix/metadata.csv` & `pyhard-2.1.5/pyhard/data/mix/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/overlap/coordinates.csv` & `pyhard-2.1.5/pyhard/data/overlap/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/overlap/data.csv` & `pyhard-2.1.5/pyhard/data/overlap/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/overlap/metadata.csv` & `pyhard-2.1.5/pyhard/data/overlap/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/separate/coordinates.csv` & `pyhard-2.1.5/pyhard/data/separate/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/separate/data.csv` & `pyhard-2.1.5/pyhard/data/separate/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/separate/feature_process.csv` & `pyhard-2.1.5/pyhard/data/separate/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/separate/feature_raw.csv` & `pyhard-2.1.5/pyhard/data/separate/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/separate/metadata.csv` & `pyhard-2.1.5/pyhard/data/separate/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/algorithm_bin.csv` & `pyhard-2.1.5/pyhard/data/wine/algorithm_bin.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/algorithm_process.csv` & `pyhard-2.1.5/pyhard/data/wine/algorithm_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/algorithm_raw.csv` & `pyhard-2.1.5/pyhard/data/wine/algorithm_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/beta_easy.csv` & `pyhard-2.1.5/pyhard/data/wine/beta_easy.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/coordinates.csv` & `pyhard-2.1.5/pyhard/data/wine/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/data.csv` & `pyhard-2.1.5/pyhard/data/wine/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/feature_process.csv` & `pyhard-2.1.5/pyhard/data/wine/feature_process.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/feature_raw.csv` & `pyhard-2.1.5/pyhard/data/wine/feature_raw.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/footprint_bagging_good.csv` & `pyhard-2.1.5/pyhard/data/wine/footprint_bagging_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/footprint_gradient_boosting_good.csv` & `pyhard-2.1.5/pyhard/data/wine/footprint_gradient_boosting_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/footprint_instance_easiness_good.csv` & `pyhard-2.1.5/pyhard/data/wine/footprint_instance_easiness_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/footprint_logistic_regression_good.csv` & `pyhard-2.1.5/pyhard/data/wine/footprint_logistic_regression_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/footprint_mlp_good.csv` & `pyhard-2.1.5/pyhard/data/wine/footprint_mlp_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/footprint_performance.csv` & `pyhard-2.1.5/pyhard/data/wine/footprint_performance.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/footprint_random_forest_best.csv` & `pyhard-2.1.5/pyhard/data/wine/footprint_random_forest_best.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/footprint_random_forest_good.csv` & `pyhard-2.1.5/pyhard/data/wine/footprint_random_forest_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/footprint_svc_linear_good.csv` & `pyhard-2.1.5/pyhard/data/wine/footprint_svc_linear_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/footprint_svc_rbf_good.csv` & `pyhard-2.1.5/pyhard/data/wine/footprint_svc_rbf_good.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/good_algos.csv` & `pyhard-2.1.5/pyhard/data/wine/good_algos.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/ih.csv` & `pyhard-2.1.5/pyhard/data/wine/ih.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/metadata.csv` & `pyhard-2.1.5/pyhard/data/wine/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/metadata_full.csv` & `pyhard-2.1.5/pyhard/data/wine/metadata_full.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/wine/portfolio.csv` & `pyhard-2.1.5/pyhard/data/wine/portfolio.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/xor/coordinates.csv` & `pyhard-2.1.5/pyhard/data/xor/coordinates.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/xor/data.csv` & `pyhard-2.1.5/pyhard/data/xor/data.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/data/xor/metadata.csv` & `pyhard-2.1.5/pyhard/data/xor/metadata.csv`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/feature_selection.py` & `pyhard-2.1.5/pyhard/feature_selection.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/hpo.py` & `pyhard-2.1.5/pyhard/hpo.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/integrator.py` & `pyhard-2.1.5/pyhard/integrator.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/measures.py` & `pyhard-2.1.5/pyhard/measures.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/metrics.py` & `pyhard-2.1.5/pyhard/metrics.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/midia/blobs.svg` & `pyhard-2.1.5/pyhard/midia/blobs.svg`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/regression.py` & `pyhard-2.1.5/pyhard/regression.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/structures.py` & `pyhard-2.1.5/pyhard/structures.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/thirdparty/entropy_estimators.py` & `pyhard-2.1.5/pyhard/thirdparty/entropy_estimators.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/thirdparty/rank_aggregation.py` & `pyhard-2.1.5/pyhard/thirdparty/rank_aggregation.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/thirdparty/skfeature.py` & `pyhard-2.1.5/pyhard/thirdparty/skfeature.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/utils.py` & `pyhard-2.1.5/pyhard/utils.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/validator.py` & `pyhard-2.1.5/pyhard/validator.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard/visualization.py` & `pyhard-2.1.5/pyhard/visualization.py`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/pyhard.egg-info/PKG-INFO` & `pyhard-2.1.5/pyhard.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,185 +1,185 @@
 Metadata-Version: 2.1
 Name: pyhard
-Version: 2.1.4
+Version: 2.1.5
 Summary: Analyze, explore and visualize instance hardness within datasets
 Home-page: https://gitlab.com/ita-ml/pyhard
+Download-URL: https://gitlab.com/ita-ml/pyhard/-/archive/v2.1.5/pyhard-v2.1.5.tar.gz
 Author: Pedro Paiva
 Author-email: paiva@ita.br
 License: MIT
-Download-URL: https://gitlab.com/ita-ml/pyhard/-/archive/v2.1.4/pyhard-v2.1.4.tar.gz
-Description: <!--
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/ita-ml%2Finstance-hardness/binder?filepath=notebooks%2F)
-        [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-        [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://en.wikipedia.org/wiki/MIT_License)
-        -->
-        
-        # PyHard
-        
-        Instance Hardness analysis in Python, with a two-fold objective: insights on data quality issues; 
-        and better understanding of the weaknesses and strengths of different algorithms.
-        
-        * Documentation: https://ita-ml.gitlab.io/pyhard/
-        * Source code: https://gitlab.com/ita-ml/pyhard
-        * Bug reports: https://gitlab.com/ita-ml/pyhard/-/issues
-        
-        ## Getting Started
-        
-        PyHard employes a methodology known as [_Instance Space Analysis_](https://github.com/andremun/InstanceSpace) (ISA) to analyse performance at the instance level rather than at dataset level. The result is an alternative for visualizing algorithm performance for each instance within a dataset, by relating predictive performance to estimated instance hardness measures extracted from the data. This analysis reveals regions of strengths and weaknesses of predictors (aka _footprints_), and highlights individual instances within a  dataset that warrant further investigation, either due to their unique properties or potential data quality issues.
-        
-        
-        ### Installation
-        Although the original ISA toolkit has been written in Matlab, we provide a lighter version in Python, with less tools, but enough for the instance hardness analysis purposes. You may find the implementation in the separate package [PyISpace](https://gitlab.com/ita-ml/pyispace). Notwithstanding, the choice of the ISA engine is left up to the user, which can be set in the configuration file. Below, we present the standard installation, and also the the additional steps to configure the Matlab engine (optional).
-        
-        _For users_
-        
-        ```
-        pip install pyhard
-        ```
-        
-        _For developers_
-        
-        Alternatively, if you are a developer and want to contribute, the following installation is better suited for testing new features:
-        ```
-        git clone https://gitlab.com/ita-ml/pyhard.git
-        cd pyhard
-        pip install -e .
-        ```
-        
-        #### Anaconda environment
-        
-        We **strongly recommend** using a separate Python environment. We provide an env file [environment.yml](./environment.yml) to create a conda env with all required dependencies:
-        
-        ```
-        conda env create --file environment.yml
-        ```
-        
-        
-        ### Usage
-        
-        First, make sure that the configuration files are placed within the current directory and the settings are the desired ones. To generate those files, run
-        
-        ```
-        pyhard init
-        ```
-        
-        This will create both `config.yaml` and `options.json` in the current directory.
-        
-        The file `config.yaml` is used to configurate steps 1-4 below. Through it, options for file paths, measures, classifiers, feature selection and hyper-parameter optimization can be set. More instructions can be found in the comments within the file.
-        
-        At least the field `datafile` (in section 'general') should be set in `config.yaml`. It specifies the path (absolute or relative) of the input dataset. Leaving the field `rootdir` as `'.'` (default), the output files will be saved in the current folder along with the configuration files (recommended).
-        
-        Once everything is configured, run the analysis:
-        
-        ```
-        pyhard run
-        ```
-        
-        By default, the following steps shall be taken:
-        
-        1. Calculate the _hardness measures_;
-        
-        2. Evaluate classification performance at instance level for each algorithm;
-        
-        3. Select the most relevant hardness measures with respect to the instance classification error;
-        
-        4. Join the outputs of steps 1, 2 and 3 to build the _metadata_ file (`metadata.csv`);
-        
-        5. Run __ISA__ (_Instance Space Analysis_), which generates the _Instance Space_ (IS) representation and the _footprint_ areas;
-        
-        Steps 1 to 4 comprise the metadata construction, and step 5 the ISA itself. To curb any of these two major stages, use the options with command `run`:
-        
-        * `--no-meta`: does not attempt to build the metadata file
-        
-        * `--no-isa`: prevents the Instance Space Analysis
-        
-        Finally, to explore the results, launch the app:  
-        
-        ```
-        pyhard app
-        ```
-        
-        To see all CLI commands, run `pyhard --help`, or `pyhard run --help` to get the options for this command.
-        
-        
-        ### Guidelines for input dataset
-        
-        Please follow the recommendations below:
-        
-        * Only `csv` files are accepted
-        
-        * The dataset should be in the format `(n_instances, n_features)`
-        
-        * It cannot contains NaNs or missing values
-        
-        * **Do not** include any index column. Instances will be indexed in order, starting from **1**
-        
-        * **The last column** should contain the target variable (`y`). Otherwise, the name of the target column must be declared in the field `target_col` (config file)
-        
-        * Categorical features should be handled previously
-        
-        
-        ## Citation
-        
-        If you're using PyHard in your research or application, please cite our [paper](https://link.springer.com/article/10.1007/s10994-022-06205-9):
-        
-        > Paiva, P. Y. A., Moreno, C. C., Smith-Miles, K., Valeriano, M. G., & Lorena, A. C. (2022). Relating instance hardness to classification performance in a dataset: a visual approach. Machine Learning, 111(8), 3085-3123. https://doi.org/10.1007/s10994-022-06205-9
-        
-        ```
-        @article{paiva2022relating,
-              title={Relating instance hardness to classification performance in a dataset: a visual approach},
-              author={Paiva, Pedro Yuri Arbs and Moreno, Camila Castro and Smith-Miles, Kate and Valeriano, Maria Gabriela and Lorena, Ana Carolina},
-              journal={Machine Learning},
-              volume={111},
-              number={8},
-              pages={3085--3123},
-              year={2022},
-              publisher={Springer}
-        }
-        ```
-        
-        
-        ## References
-        
-        _Base_
-        
-        1. Michael R. Smith, Tony Martinez, and Christophe Giraud-Carrier. 2014. __An instance level analysis of data complexity__. Mach. Learn. 95, 2 (May 2014), 225–256.
-        
-        2. Ana C. Lorena, Luís P. F. Garcia, Jens Lehmann, Marcilio C. P. Souto, and Tin Kam Ho. 2019. __How Complex Is Your Classification Problem? A Survey on Measuring Classification Complexity__. ACM Comput. Surv. 52, 5, Article 107 (October 2019), 34 pages.
-        
-        3. Mario A. Muñoz, Laura Villanova, Davaatseren Baatar, and Kate Smith-Miles. 2018. __Instance spaces for machine learning classification__. Mach. Learn. 107, 1 (January   2018), 109–147.
-        
-        _Feature selection_
-        
-        4. Luiz H. Lorena, André C. Carvalho, and Ana C. Lorena. 2015. __Filter Feature Selection for One-Class Classification__. Journal of Intelligent and Robotic Systems 80, 1 (October   2015), 227–243.
-        
-        5. Goldberger, J., Hinton, G., Roweis, S., Salakhutdinov, R. (2005). __Neighbourhood Components Analysis__. Advances in Neural Information Processing Systems. 17, 513-520.
-        
-        6. Yang, W., Wang, K., & Zuo, W. (2012). __Neighborhood component feature selection for high-dimensional data__. J. Comput., 7(1), 161-168.
-        
-        7. Amankwaa-Kyeremeh, B., Greet, C., Zanin, M., Skinner, W. and Asamoah, R. K., (2020), __Selecting key predictor parameters for regression analysis using modified Neighbourhood Component Analysis (NCA) Algorithm__. Proceedings of 6th UMaT Biennial International Mining and Mineral Conference, Tarkwa, Ghana, pp. 320-325.
-        
-        8. Artur J. Ferreira and Mário A. T. Figueiredo. 2012. __Efficient feature selection filters for high-dimensional data__. Pattern Recognition Letters 33, 13 (October, 2012), 1794–1804.
-        
-        9. Jundong Li, Kewei Cheng, Suhang Wang, Fred Morstatter, Robert P. Trevino, Jiliang Tang, and Huan Liu. 2017. __Feature Selection: A Data Perspective__. ACM Comput. Surv. 50, 6, Article 94 (January 2018), 45 pages.
-        
-        10. Shuyang Gao, Greg Ver Steeg, and Aram Galstyan. __Efficient Estimation of Mutual Information for Strongly Dependent Variables__. Available in http://arxiv.org/abs/1411.2003. AISTATS, 2015.
-        
-        _Hyper parameter optimization_
-        
-        11. James Bergstra, Rémi Bardenet, Yoshua Bengio, and Balázs Kégl. 2011. __Algorithms for hyper-parameter optimization__. In Proceedings of the 24th International Conference on Neural Information Processing Systems (NIPS’11). Curran Associates Inc., Red Hook, NY, USA, 2546–2554.
-        
-        12. Jasper Snoek, Hugo Larochelle, and Ryan P. Adams. 2012. __Practical Bayesian optimization of machine learning algorithms__. In Proceedings of the 25th International Conference on Neural Information Processing Systems - Volume 2 (NIPS’12). Curran Associates Inc., Red Hook, NY, USA, 2951–2959.
-          
-        13. J. Bergstra, D. Yamins, and D. D. Cox. 2013. __Making a science of model search: hyperparameter optimization in hundreds of dimensions for vision architectures__. In Proceedings of the 30th International Conference on International Conference on Machine Learning - Volume 28 (ICML’13). JMLR.org, I–115–I–123.
-          
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
+License-File: LICENSE
+
+<!--
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/ita-ml%2Finstance-hardness/binder?filepath=notebooks%2F)
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+[![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://en.wikipedia.org/wiki/MIT_License)
+-->
+
+# PyHard
+
+Instance Hardness analysis in Python, with a two-fold objective: insights on data quality issues; 
+and better understanding of the weaknesses and strengths of different algorithms.
+
+* Documentation: https://ita-ml.gitlab.io/pyhard/
+* Source code: https://gitlab.com/ita-ml/pyhard
+* Bug reports: https://gitlab.com/ita-ml/pyhard/-/issues
+
+## Getting Started
+
+PyHard employes a methodology known as [_Instance Space Analysis_](https://github.com/andremun/InstanceSpace) (ISA) to analyse performance at the instance level rather than at dataset level. The result is an alternative for visualizing algorithm performance for each instance within a dataset, by relating predictive performance to estimated instance hardness measures extracted from the data. This analysis reveals regions of strengths and weaknesses of predictors (aka _footprints_), and highlights individual instances within a  dataset that warrant further investigation, either due to their unique properties or potential data quality issues.
+
+
+### Installation
+Although the original ISA toolkit has been written in Matlab, we provide a lighter version in Python, with less tools, but enough for the instance hardness analysis purposes. You may find the implementation in the separate package [PyISpace](https://gitlab.com/ita-ml/pyispace). Notwithstanding, the choice of the ISA engine is left up to the user, which can be set in the configuration file. Below, we present the standard installation, and also the the additional steps to configure the Matlab engine (optional).
+
+_For users_
+
+```
+pip install pyhard
+```
+
+_For developers_
+
+Alternatively, if you are a developer and want to contribute, the following installation is better suited for testing new features:
+```
+git clone https://gitlab.com/ita-ml/pyhard.git
+cd pyhard
+pip install -e .
+```
+
+#### Anaconda environment
+
+We **strongly recommend** using a separate Python environment. We provide an env file [environment.yml](./environment.yml) to create a conda env with all required dependencies:
+
+```
+conda env create --file environment.yml
+```
+
+
+### Usage
+
+First, make sure that the configuration files are placed within the current directory and the settings are the desired ones. To generate those files, run
+
+```
+pyhard init
+```
+
+This will create both `config.yaml` and `options.json` in the current directory.
+
+The file `config.yaml` is used to configurate steps 1-4 below. Through it, options for file paths, measures, classifiers, feature selection and hyper-parameter optimization can be set. More instructions can be found in the comments within the file.
+
+At least the field `datafile` (in section 'general') should be set in `config.yaml`. It specifies the path (absolute or relative) of the input dataset. Leaving the field `rootdir` as `'.'` (default), the output files will be saved in the current folder along with the configuration files (recommended).
+
+Once everything is configured, run the analysis:
+
+```
+pyhard run
+```
+
+By default, the following steps shall be taken:
+
+1. Calculate the _hardness measures_;
+
+2. Evaluate classification performance at instance level for each algorithm;
+
+3. Select the most relevant hardness measures with respect to the instance classification error;
+
+4. Join the outputs of steps 1, 2 and 3 to build the _metadata_ file (`metadata.csv`);
+
+5. Run __ISA__ (_Instance Space Analysis_), which generates the _Instance Space_ (IS) representation and the _footprint_ areas;
+
+Steps 1 to 4 comprise the metadata construction, and step 5 the ISA itself. To curb any of these two major stages, use the options with command `run`:
+
+* `--no-meta`: does not attempt to build the metadata file
+
+* `--no-isa`: prevents the Instance Space Analysis
+
+Finally, to explore the results, launch the app:  
+
+```
+pyhard app
+```
+
+To see all CLI commands, run `pyhard --help`, or `pyhard run --help` to get the options for this command.
+
+
+### Guidelines for input dataset
+
+Please follow the recommendations below:
+
+* Only `csv` files are accepted
+
+* The dataset should be in the format `(n_instances, n_features)`
+
+* It cannot contains NaNs or missing values
+
+* **Do not** include any index column. Instances will be indexed in order, starting from **1**
+
+* **The last column** should contain the target variable (`y`). Otherwise, the name of the target column must be declared in the field `target_col` (config file)
+
+* Categorical features should be handled previously
+
+
+## Citation
+
+If you're using PyHard in your research or application, please cite our [paper](https://link.springer.com/article/10.1007/s10994-022-06205-9):
+
+> Paiva, P. Y. A., Moreno, C. C., Smith-Miles, K., Valeriano, M. G., & Lorena, A. C. (2022). Relating instance hardness to classification performance in a dataset: a visual approach. Machine Learning, 111(8), 3085-3123. https://doi.org/10.1007/s10994-022-06205-9
+
+```
+@article{paiva2022relating,
+      title={Relating instance hardness to classification performance in a dataset: a visual approach},
+      author={Paiva, Pedro Yuri Arbs and Moreno, Camila Castro and Smith-Miles, Kate and Valeriano, Maria Gabriela and Lorena, Ana Carolina},
+      journal={Machine Learning},
+      volume={111},
+      number={8},
+      pages={3085--3123},
+      year={2022},
+      publisher={Springer}
+}
+```
+
+
+## References
+
+_Base_
+
+1. Michael R. Smith, Tony Martinez, and Christophe Giraud-Carrier. 2014. __An instance level analysis of data complexity__. Mach. Learn. 95, 2 (May 2014), 225–256.
+
+2. Ana C. Lorena, Luís P. F. Garcia, Jens Lehmann, Marcilio C. P. Souto, and Tin Kam Ho. 2019. __How Complex Is Your Classification Problem? A Survey on Measuring Classification Complexity__. ACM Comput. Surv. 52, 5, Article 107 (October 2019), 34 pages.
+
+3. Mario A. Muñoz, Laura Villanova, Davaatseren Baatar, and Kate Smith-Miles. 2018. __Instance spaces for machine learning classification__. Mach. Learn. 107, 1 (January   2018), 109–147.
+
+_Feature selection_
+
+4. Luiz H. Lorena, André C. Carvalho, and Ana C. Lorena. 2015. __Filter Feature Selection for One-Class Classification__. Journal of Intelligent and Robotic Systems 80, 1 (October   2015), 227–243.
+
+5. Goldberger, J., Hinton, G., Roweis, S., Salakhutdinov, R. (2005). __Neighbourhood Components Analysis__. Advances in Neural Information Processing Systems. 17, 513-520.
+
+6. Yang, W., Wang, K., & Zuo, W. (2012). __Neighborhood component feature selection for high-dimensional data__. J. Comput., 7(1), 161-168.
+
+7. Amankwaa-Kyeremeh, B., Greet, C., Zanin, M., Skinner, W. and Asamoah, R. K., (2020), __Selecting key predictor parameters for regression analysis using modified Neighbourhood Component Analysis (NCA) Algorithm__. Proceedings of 6th UMaT Biennial International Mining and Mineral Conference, Tarkwa, Ghana, pp. 320-325.
+
+8. Artur J. Ferreira and Mário A. T. Figueiredo. 2012. __Efficient feature selection filters for high-dimensional data__. Pattern Recognition Letters 33, 13 (October, 2012), 1794–1804.
+
+9. Jundong Li, Kewei Cheng, Suhang Wang, Fred Morstatter, Robert P. Trevino, Jiliang Tang, and Huan Liu. 2017. __Feature Selection: A Data Perspective__. ACM Comput. Surv. 50, 6, Article 94 (January 2018), 45 pages.
+
+10. Shuyang Gao, Greg Ver Steeg, and Aram Galstyan. __Efficient Estimation of Mutual Information for Strongly Dependent Variables__. Available in http://arxiv.org/abs/1411.2003. AISTATS, 2015.
+
+_Hyper parameter optimization_
+
+11. James Bergstra, Rémi Bardenet, Yoshua Bengio, and Balázs Kégl. 2011. __Algorithms for hyper-parameter optimization__. In Proceedings of the 24th International Conference on Neural Information Processing Systems (NIPS’11). Curran Associates Inc., Red Hook, NY, USA, 2546–2554.
+
+12. Jasper Snoek, Hugo Larochelle, and Ryan P. Adams. 2012. __Practical Bayesian optimization of machine learning algorithms__. In Proceedings of the 25th International Conference on Neural Information Processing Systems - Volume 2 (NIPS’12). Curran Associates Inc., Red Hook, NY, USA, 2951–2959.
+  
+13. J. Bergstra, D. Yamins, and D. D. Cox. 2013. __Making a science of model search: hyperparameter optimization in hundreds of dimensions for vision architectures__. In Proceedings of the 30th International Conference on International Conference on Machine Learning - Volume 28 (ICML’13). JMLR.org, I–115–I–123.
+
```

### Comparing `pyhard-2.1.4/pyhard.egg-info/SOURCES.txt` & `pyhard-2.1.5/pyhard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhard-2.1.4/setup.py` & `pyhard-2.1.5/setup.py`

 * *Files identical despite different names*


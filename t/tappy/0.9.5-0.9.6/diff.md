# Comparing `tmp/tappy-0.9.5.tar.gz` & `tmp/tappy-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tappy-0.9.5.tar", last modified: Thu Jul 14 01:14:51 2022, max compression
+gzip compressed data, was "tappy-0.9.6.tar", last modified: Thu Jul 14 02:21:17 2022, max compression
```

## Comparing `tappy-0.9.5.tar` & `tappy-0.9.6.tar`

### file list

```diff
@@ -1,133 +1,135 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 01:14:51.225630 tappy-0.9.5/
--rw-rw-r--   0 tim       (1000) tim       (1000)      105 2022-06-27 02:03:47.000000 tappy-0.9.5/.deepsource.toml
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 01:14:51.209630 tappy-0.9.5/.github/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 01:14:51.209630 tappy-0.9.5/.github/workflows/
--rw-rw-r--   0 tim       (1000) tim       (1000)     1713 2022-07-11 17:14:29.000000 tappy-0.9.5/.github/workflows/python-package.yml
--rw-rw-r--   0 tim       (1000) tim       (1000)     2402 2022-06-02 19:32:09.000000 tappy-0.9.5/.pre-commit-config.yaml
--rw-rw-r--   0 tim       (1000) tim       (1000)       50 2022-04-05 13:33:48.000000 tappy-0.9.5/AUTHORS.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      745 2022-04-05 13:32:14.000000 tappy-0.9.5/BADGES.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      375 2022-07-04 11:58:32.000000 tappy-0.9.5/CHANGELOG.md
--rw-r--r--   0 tim       (1000) tim       (1000)     3123 2022-07-03 23:02:05.000000 tappy-0.9.5/CONTRIBUTING.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1482 2022-07-03 23:02:18.000000 tappy-0.9.5/LICENSE.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      210 2022-06-27 02:03:47.000000 tappy-0.9.5/MANIFEST.in
--rw-rw-r--   0 tim       (1000) tim       (1000)     4966 2022-07-14 01:14:51.225630 tappy-0.9.5/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     3622 2022-06-06 00:30:11.000000 tappy-0.9.5/README.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)        6 2022-07-04 11:58:32.000000 tappy-0.9.5/VERSION
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 01:14:51.209630 tappy-0.9.5/dist/
--rw-rw-r--   0 tim       (1000) tim       (1000)    33849 2022-04-17 02:20:35.000000 tappy-0.9.5/dist/tappy-0.9.3.tar.gz
--rw-rw-r--   0 tim       (1000) tim       (1000)    33839 2022-04-17 02:58:32.000000 tappy-0.9.5/dist/tappy-0.9.4.tar.gz
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 01:14:51.213630 tappy-0.9.5/docs/
--rw-rw-r--   0 tim       (1000) tim       (1000)     2538 2022-06-12 00:06:46.000000 tappy-0.9.5/docs/CompareTidalFilters.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)    14579 2022-04-05 12:03:23.000000 tappy-0.9.5/docs/Comparison_of_subtraction.png
--rw-rw-r--   0 tim       (1000) tim       (1000)    13684 2022-04-05 12:04:00.000000 tappy-0.9.5/docs/Comparison_of_tidal_filters_large.png
--rw-rw-r--   0 tim       (1000) tim       (1000)    12734 2022-04-05 12:04:28.000000 tappy-0.9.5/docs/Comparison_of_tidal_filters_small.png
--rw-rw-r--   0 tim       (1000) tim       (1000)      462 2022-06-02 19:34:03.000000 tappy-0.9.5/docs/FillMissing.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     1074 2022-06-02 19:34:03.000000 tappy-0.9.5/docs/HarmonicAnalysis.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     5712 2022-04-05 13:36:55.000000 tappy-0.9.5/docs/Makefile
--rw-rw-r--   0 tim       (1000) tim       (1000)    11237 2022-04-05 12:05:55.000000 tappy-0.9.5/docs/Missing.png
--rw-rw-r--   0 tim       (1000) tim       (1000)    16497 2022-06-27 02:03:47.000000 tappy-0.9.5/docs/TappyUsersGuide.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     3233 2022-06-12 00:06:46.000000 tappy-0.9.5/docs/TidalScience.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       55 2022-04-05 15:46:46.000000 tappy-0.9.5/docs/authors.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     9573 2022-06-09 03:45:34.000000 tappy-0.9.5/docs/conf.py
--rw-r--r--   0 tim       (1000) tim       (1000)       60 2022-04-05 15:46:22.000000 tappy-0.9.5/docs/contributing.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      527 2022-06-02 19:34:03.000000 tappy-0.9.5/docs/index.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       79 2022-04-05 15:46:53.000000 tappy-0.9.5/docs/license.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)       27 2022-04-05 15:41:05.000000 tappy-0.9.5/docs/readme.rst
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 01:14:51.213630 tappy-0.9.5/example/
--rwxrwxr-x   0 tim       (1000) tim       (1000)      850 2022-06-27 02:03:47.000000 tappy-0.9.5/example/example.sh
--rw-rw-r--   0 tim       (1000) tim       (1000)     2065 2022-04-01 22:29:05.000000 tappy-0.9.5/example/mayport_florida_8720220_con_noaa.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      954 2022-04-01 22:29:05.000000 tappy-0.9.5/example/mayport_florida_8720220_con_tappy.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)    33481 2022-06-27 02:03:47.000000 tappy-0.9.5/example/mayport_florida_8720220_data.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      634 2022-06-27 02:03:47.000000 tappy-0.9.5/example/mayport_florida_8720220_data_def.txt
--rwxrwxr-x   0 tim       (1000) tim       (1000)      854 2022-06-12 00:06:51.000000 tappy-0.9.5/example/process_grace.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      635 2022-06-27 02:03:47.000000 tappy-0.9.5/example/sparse.def
--rw-rw-r--   0 tim       (1000) tim       (1000)      662 2022-06-27 02:03:47.000000 tappy-0.9.5/example/tidesandcurrents.def
--rw-rw-r--   0 tim       (1000) tim       (1000)     2066 2022-04-01 22:29:05.000000 tappy-0.9.5/example/tridentpier_florida_8721604_con_noaa.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      953 2022-04-01 22:29:05.000000 tappy-0.9.5/example/tridentpier_florida_8721604_con_tappy.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)    14490 2022-04-01 22:29:05.000000 tappy-0.9.5/example/tridentpier_florida_8721604_data.txt.gz
--rw-rw-r--   0 tim       (1000) tim       (1000)      955 2022-06-27 02:03:47.000000 tappy-0.9.5/example/tridentpier_florida_8721604_datetime.txt.def
--rw-r--r--   0 tim       (1000) tim       (1000)      650 2022-07-04 11:58:32.000000 tappy-0.9.5/pyproject.toml
--rw-r--r--   0 tim       (1000) tim       (1000)     1878 2022-07-14 01:14:51.225630 tappy-0.9.5/setup.cfg
--rw-rw-r--   0 tim       (1000) tim       (1000)      698 2022-07-14 01:14:46.000000 tappy-0.9.5/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 01:14:51.209630 tappy-0.9.5/src/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 01:14:51.213630 tappy-0.9.5/src/tappy/
--rwxrwxr-x   0 tim       (1000) tim       (1000)    86416 2022-07-03 23:02:38.000000 tappy-0.9.5/src/tappy/tappy.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 01:14:51.217630 tappy-0.9.5/src/tappy/tappy_lib/
--rw-rw-r--   0 tim       (1000) tim       (1000)      251 2022-07-04 11:57:10.000000 tappy-0.9.5/src/tappy/tappy_lib/__init__.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     2643 2022-06-12 00:06:46.000000 tappy-0.9.5/src/tappy/tappy_lib/filter.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    40408 2022-06-12 00:06:46.000000 tappy-0.9.5/src/tappy/tappy_lib/parameter_database.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)    15295 2022-07-04 00:48:11.000000 tappy-0.9.5/src/tappy/tappy_lib/sparser.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 01:14:51.213630 tappy-0.9.5/src/tappy.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)     4966 2022-07-14 01:14:50.000000 tappy-0.9.5/src/tappy.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     3499 2022-07-14 01:14:51.000000 tappy-0.9.5/src/tappy.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2022-07-14 01:14:50.000000 tappy-0.9.5/src/tappy.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       43 2022-07-14 01:14:50.000000 tappy-0.9.5/src/tappy.egg-info/entry_points.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2022-07-03 18:20:26.000000 tappy-0.9.5/src/tappy.egg-info/not-zip-safe
--rw-rw-r--   0 tim       (1000) tim       (1000)      226 2022-07-14 01:14:50.000000 tappy-0.9.5/src/tappy.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2022-07-14 01:14:50.000000 tappy-0.9.5/src/tappy.egg-info/top_level.txt
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 01:14:51.217630 tappy-0.9.5/tests/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 01:14:51.225630 tappy-0.9.5/tests/output_ts/
--rw-rw-r--   0 tim       (1000) tim       (1000)     2413 2022-04-01 22:29:05.000000 tappy-0.9.5/tests/output_ts/constituents.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31114 2022-07-03 20:09:20.000000 tappy-0.9.5/tests/output_ts/outts_2MN6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31139 2022-07-03 20:09:20.000000 tappy-0.9.5/tests/output_ts/outts_2MS6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31089 2022-07-03 20:09:20.000000 tappy-0.9.5/tests/output_ts/outts_2Q1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30606 2022-07-03 20:09:20.000000 tappy-0.9.5/tests/output_ts/outts_2SM2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31149 2022-07-03 20:09:21.000000 tappy-0.9.5/tests/output_ts/outts_2SM6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31560 2022-07-03 20:09:21.000000 tappy-0.9.5/tests/output_ts/outts_J1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30221 2022-07-03 20:09:21.000000 tappy-0.9.5/tests/output_ts/outts_K1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    29590 2022-07-03 20:09:21.000000 tappy-0.9.5/tests/output_ts/outts_M2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30959 2022-07-03 20:09:21.000000 tappy-0.9.5/tests/output_ts/outts_M3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30698 2022-07-03 20:09:22.000000 tappy-0.9.5/tests/output_ts/outts_M4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31021 2022-07-03 20:09:22.000000 tappy-0.9.5/tests/output_ts/outts_M6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31618 2022-07-03 20:09:22.000000 tappy-0.9.5/tests/output_ts/outts_M8.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30841 2022-07-03 20:09:22.000000 tappy-0.9.5/tests/output_ts/outts_MK3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30806 2022-07-03 20:09:22.000000 tappy-0.9.5/tests/output_ts/outts_MN4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31258 2022-07-03 20:09:23.000000 tappy-0.9.5/tests/output_ts/outts_MO3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30884 2022-07-03 20:09:23.000000 tappy-0.9.5/tests/output_ts/outts_MS4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30446 2022-07-03 20:09:23.000000 tappy-0.9.5/tests/output_ts/outts_MSf.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30050 2022-07-03 20:09:23.000000 tappy-0.9.5/tests/output_ts/outts_N2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30958 2022-07-03 20:09:23.000000 tappy-0.9.5/tests/output_ts/outts_NO1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30493 2022-07-03 20:09:24.000000 tappy-0.9.5/tests/output_ts/outts_O1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31009 2022-07-03 20:09:24.000000 tappy-0.9.5/tests/output_ts/outts_OO1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30878 2022-07-03 20:09:24.000000 tappy-0.9.5/tests/output_ts/outts_Q1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30244 2022-07-03 20:09:24.000000 tappy-0.9.5/tests/output_ts/outts_S2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31326 2022-07-03 20:09:24.000000 tappy-0.9.5/tests/output_ts/outts_S4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31482 2022-07-03 20:09:25.000000 tappy-0.9.5/tests/output_ts/outts_S6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31053 2022-07-03 20:09:25.000000 tappy-0.9.5/tests/output_ts/outts_SK3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30580 2022-07-03 20:09:25.000000 tappy-0.9.5/tests/output_ts/outts_eta2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28802 2022-07-03 20:09:20.000000 tappy-0.9.5/tests/output_ts/outts_ff_2MN6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:20.000000 tappy-0.9.5/tests/output_ts/outts_ff_2MS6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:20.000000 tappy-0.9.5/tests/output_ts/outts_ff_2Q1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:20.000000 tappy-0.9.5/tests/output_ts/outts_ff_2SM2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:21.000000 tappy-0.9.5/tests/output_ts/outts_ff_2SM6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28899 2022-07-03 20:09:21.000000 tappy-0.9.5/tests/output_ts/outts_ff_J1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28900 2022-07-03 20:09:21.000000 tappy-0.9.5/tests/output_ts/outts_ff_K1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:21.000000 tappy-0.9.5/tests/output_ts/outts_ff_M2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28799 2022-07-03 20:09:21.000000 tappy-0.9.5/tests/output_ts/outts_ff_M3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:22.000000 tappy-0.9.5/tests/output_ts/outts_ff_M4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28802 2022-07-03 20:09:22.000000 tappy-0.9.5/tests/output_ts/outts_ff_M6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28799 2022-07-03 20:09:22.000000 tappy-0.9.5/tests/output_ts/outts_ff_M8.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28886 2022-07-03 20:09:22.000000 tappy-0.9.5/tests/output_ts/outts_ff_MK3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:22.000000 tappy-0.9.5/tests/output_ts/outts_ff_MN4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28912 2022-07-03 20:09:23.000000 tappy-0.9.5/tests/output_ts/outts_ff_MO3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:23.000000 tappy-0.9.5/tests/output_ts/outts_ff_MS4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:23.000000 tappy-0.9.5/tests/output_ts/outts_ff_MSf.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:23.000000 tappy-0.9.5/tests/output_ts/outts_ff_N2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28911 2022-07-03 20:09:23.000000 tappy-0.9.5/tests/output_ts/outts_ff_NO1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:24.000000 tappy-0.9.5/tests/output_ts/outts_ff_O1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28904 2022-07-03 20:09:24.000000 tappy-0.9.5/tests/output_ts/outts_ff_OO1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:24.000000 tappy-0.9.5/tests/output_ts/outts_ff_Q1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    17853 2022-07-03 20:09:24.000000 tappy-0.9.5/tests/output_ts/outts_ff_S2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    17853 2022-07-03 20:09:24.000000 tappy-0.9.5/tests/output_ts/outts_ff_S4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    17853 2022-07-03 20:09:25.000000 tappy-0.9.5/tests/output_ts/outts_ff_S6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28900 2022-07-03 20:09:25.000000 tappy-0.9.5/tests/output_ts/outts_ff_SK3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28911 2022-07-03 20:09:25.000000 tappy-0.9.5/tests/output_ts/outts_ff_eta2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28904 2022-07-03 20:09:25.000000 tappy-0.9.5/tests/output_ts/outts_ff_ups1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    21576 2022-04-01 22:29:05.000000 tappy-0.9.5/tests/output_ts/outts_filtered_transform.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    19317 2022-07-03 20:09:25.000000 tappy-0.9.5/tests/output_ts/outts_original.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    21918 2022-04-01 22:29:05.000000 tappy-0.9.5/tests/output_ts/outts_total_prediction.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    29591 2022-07-03 20:09:25.000000 tappy-0.9.5/tests/output_ts/outts_total_tidal_components.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31026 2022-07-03 20:09:25.000000 tappy-0.9.5/tests/output_ts/outts_ups1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)      412 2022-06-27 02:03:47.000000 tappy-0.9.5/tests/predict_def.out
--rw-rw-r--   0 tim       (1000) tim       (1000)      588 2022-06-27 02:03:47.000000 tappy-0.9.5/tests/sparse.def
--rwxrwxr-x   0 tim       (1000) tim       (1000)     3416 2022-07-04 11:57:12.000000 tappy-0.9.5/tests/test_tappy.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.878642 tappy-0.9.6/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      105 2022-06-27 02:03:47.000000 tappy-0.9.6/.deepsource.toml
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.862641 tappy-0.9.6/.github/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.866642 tappy-0.9.6/.github/workflows/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      472 2022-07-04 12:00:17.000000 tappy-0.9.6/.github/workflows/clean-workflow-runs.yml
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1713 2022-07-11 17:14:29.000000 tappy-0.9.6/.github/workflows/python-package.yml
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2402 2022-06-02 19:32:09.000000 tappy-0.9.6/.pre-commit-config.yaml
+-rw-rw-r--   0 tim       (1000) tim       (1000)       50 2022-04-05 13:33:48.000000 tappy-0.9.6/AUTHORS.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      745 2022-04-05 13:32:14.000000 tappy-0.9.6/BADGES.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      456 2022-07-14 02:19:20.000000 tappy-0.9.6/CHANGELOG.md
+-rw-r--r--   0 tim       (1000) tim       (1000)     3123 2022-07-03 23:02:05.000000 tappy-0.9.6/CONTRIBUTING.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1482 2022-07-03 23:02:18.000000 tappy-0.9.6/LICENSE.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      207 2022-07-14 02:17:58.000000 tappy-0.9.6/MANIFEST.in
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4966 2022-07-14 02:21:17.878642 tappy-0.9.6/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3622 2022-06-06 00:30:11.000000 tappy-0.9.6/README.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)        6 2022-07-14 02:19:20.000000 tappy-0.9.6/VERSION
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.866642 tappy-0.9.6/dist/
+-rw-rw-r--   0 tim       (1000) tim       (1000)    33849 2022-04-17 02:20:35.000000 tappy-0.9.6/dist/tappy-0.9.3.tar.gz
+-rw-rw-r--   0 tim       (1000) tim       (1000)    33839 2022-04-17 02:58:32.000000 tappy-0.9.6/dist/tappy-0.9.4.tar.gz
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.866642 tappy-0.9.6/docs/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2538 2022-06-12 00:06:46.000000 tappy-0.9.6/docs/CompareTidalFilters.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)    14579 2022-04-05 12:03:23.000000 tappy-0.9.6/docs/Comparison_of_subtraction.png
+-rw-rw-r--   0 tim       (1000) tim       (1000)    13684 2022-04-05 12:04:00.000000 tappy-0.9.6/docs/Comparison_of_tidal_filters_large.png
+-rw-rw-r--   0 tim       (1000) tim       (1000)    12734 2022-04-05 12:04:28.000000 tappy-0.9.6/docs/Comparison_of_tidal_filters_small.png
+-rw-rw-r--   0 tim       (1000) tim       (1000)      462 2022-06-02 19:34:03.000000 tappy-0.9.6/docs/FillMissing.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1074 2022-06-02 19:34:03.000000 tappy-0.9.6/docs/HarmonicAnalysis.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     5712 2022-04-05 13:36:55.000000 tappy-0.9.6/docs/Makefile
+-rw-rw-r--   0 tim       (1000) tim       (1000)    11237 2022-04-05 12:05:55.000000 tappy-0.9.6/docs/Missing.png
+-rw-rw-r--   0 tim       (1000) tim       (1000)    16497 2022-06-27 02:03:47.000000 tappy-0.9.6/docs/TappyUsersGuide.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3233 2022-06-12 00:06:46.000000 tappy-0.9.6/docs/TidalScience.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       55 2022-04-05 15:46:46.000000 tappy-0.9.6/docs/authors.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     9573 2022-06-09 03:45:34.000000 tappy-0.9.6/docs/conf.py
+-rw-r--r--   0 tim       (1000) tim       (1000)       60 2022-04-05 15:46:22.000000 tappy-0.9.6/docs/contributing.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      527 2022-06-02 19:34:03.000000 tappy-0.9.6/docs/index.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       79 2022-04-05 15:46:53.000000 tappy-0.9.6/docs/license.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)       27 2022-04-05 15:41:05.000000 tappy-0.9.6/docs/readme.rst
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.870642 tappy-0.9.6/example/
+-rwxrwxr-x   0 tim       (1000) tim       (1000)      850 2022-06-27 02:03:47.000000 tappy-0.9.6/example/example.sh
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2065 2022-04-01 22:29:05.000000 tappy-0.9.6/example/mayport_florida_8720220_con_noaa.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      954 2022-04-01 22:29:05.000000 tappy-0.9.6/example/mayport_florida_8720220_con_tappy.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)    33481 2022-06-27 02:03:47.000000 tappy-0.9.6/example/mayport_florida_8720220_data.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      634 2022-06-27 02:03:47.000000 tappy-0.9.6/example/mayport_florida_8720220_data_def.txt
+-rwxrwxr-x   0 tim       (1000) tim       (1000)      854 2022-06-12 00:06:51.000000 tappy-0.9.6/example/process_grace.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      635 2022-06-27 02:03:47.000000 tappy-0.9.6/example/sparse.def
+-rw-rw-r--   0 tim       (1000) tim       (1000)      662 2022-06-27 02:03:47.000000 tappy-0.9.6/example/tidesandcurrents.def
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2066 2022-04-01 22:29:05.000000 tappy-0.9.6/example/tridentpier_florida_8721604_con_noaa.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      953 2022-04-01 22:29:05.000000 tappy-0.9.6/example/tridentpier_florida_8721604_con_tappy.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)    14490 2022-04-01 22:29:05.000000 tappy-0.9.6/example/tridentpier_florida_8721604_data.txt.gz
+-rw-rw-r--   0 tim       (1000) tim       (1000)      955 2022-06-27 02:03:47.000000 tappy-0.9.6/example/tridentpier_florida_8721604_datetime.txt.def
+-rw-r--r--   0 tim       (1000) tim       (1000)      650 2022-07-14 02:19:20.000000 tappy-0.9.6/pyproject.toml
+-rw-r--r--   0 tim       (1000) tim       (1000)     1878 2022-07-14 02:21:17.878642 tappy-0.9.6/setup.cfg
+-rw-rw-r--   0 tim       (1000) tim       (1000)      698 2022-07-14 01:14:46.000000 tappy-0.9.6/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.862641 tappy-0.9.6/src/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.870642 tappy-0.9.6/src/tappy/
+-rw-rw-r--   0 tim       (1000) tim       (1000)        0 2022-07-14 02:12:37.000000 tappy-0.9.6/src/tappy/__init__.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)    86394 2022-07-14 01:21:01.000000 tappy-0.9.6/src/tappy/tappy.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.870642 tappy-0.9.6/src/tappy/tappy_lib/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      251 2022-07-04 11:57:10.000000 tappy-0.9.6/src/tappy/tappy_lib/__init__.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     2643 2022-06-12 00:06:46.000000 tappy-0.9.6/src/tappy/tappy_lib/filter.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    40408 2022-06-12 00:06:46.000000 tappy-0.9.6/src/tappy/tappy_lib/parameter_database.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)    15295 2022-07-04 00:48:11.000000 tappy-0.9.6/src/tappy/tappy_lib/sparser.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.870642 tappy-0.9.6/src/tappy.egg-info/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4966 2022-07-14 02:21:16.000000 tappy-0.9.6/src/tappy.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3563 2022-07-14 02:21:17.000000 tappy-0.9.6/src/tappy.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2022-07-14 02:21:17.000000 tappy-0.9.6/src/tappy.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       43 2022-07-14 02:21:17.000000 tappy-0.9.6/src/tappy.egg-info/entry_points.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2022-07-03 18:20:26.000000 tappy-0.9.6/src/tappy.egg-info/not-zip-safe
+-rw-rw-r--   0 tim       (1000) tim       (1000)      226 2022-07-14 02:21:17.000000 tappy-0.9.6/src/tappy.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        6 2022-07-14 02:21:17.000000 tappy-0.9.6/src/tappy.egg-info/top_level.txt
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.870642 tappy-0.9.6/tests/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.878642 tappy-0.9.6/tests/output_ts/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2413 2022-04-01 22:29:05.000000 tappy-0.9.6/tests/output_ts/constituents.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31114 2022-07-03 20:09:20.000000 tappy-0.9.6/tests/output_ts/outts_2MN6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31139 2022-07-03 20:09:20.000000 tappy-0.9.6/tests/output_ts/outts_2MS6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31089 2022-07-03 20:09:20.000000 tappy-0.9.6/tests/output_ts/outts_2Q1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30606 2022-07-03 20:09:20.000000 tappy-0.9.6/tests/output_ts/outts_2SM2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31149 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_2SM6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31560 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_J1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30221 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_K1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    29590 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_M2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30959 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_M3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30698 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_M4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31021 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_M6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31618 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_M8.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30841 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_MK3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30806 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_MN4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31258 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_MO3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30884 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_MS4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30446 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_MSf.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30050 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_N2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30958 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_NO1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30493 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_O1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31009 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_OO1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30878 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_Q1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30244 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_S2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31326 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_S4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31482 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_S6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31053 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_SK3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30580 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_eta2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28802 2022-07-03 20:09:20.000000 tappy-0.9.6/tests/output_ts/outts_ff_2MN6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:20.000000 tappy-0.9.6/tests/output_ts/outts_ff_2MS6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:20.000000 tappy-0.9.6/tests/output_ts/outts_ff_2Q1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:20.000000 tappy-0.9.6/tests/output_ts/outts_ff_2SM2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_ff_2SM6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28899 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_ff_J1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28900 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_ff_K1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_ff_M2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28799 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_ff_M3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_ff_M4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28802 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_ff_M6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28799 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_ff_M8.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28886 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_ff_MK3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_ff_MN4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28912 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_ff_MO3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_ff_MS4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_ff_MSf.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_ff_N2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28911 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_ff_NO1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_ff_O1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28904 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_ff_OO1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_ff_Q1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    17853 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_ff_S2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    17853 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_ff_S4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    17853 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_ff_S6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28900 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_ff_SK3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28911 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_ff_eta2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28904 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_ff_ups1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    21576 2022-04-01 22:29:05.000000 tappy-0.9.6/tests/output_ts/outts_filtered_transform.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    19317 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_original.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    21918 2022-04-01 22:29:05.000000 tappy-0.9.6/tests/output_ts/outts_total_prediction.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    29591 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_total_tidal_components.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31026 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_ups1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)      412 2022-06-27 02:03:47.000000 tappy-0.9.6/tests/predict_def.out
+-rw-rw-r--   0 tim       (1000) tim       (1000)      588 2022-06-27 02:03:47.000000 tappy-0.9.6/tests/sparse.def
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     3416 2022-07-04 11:57:12.000000 tappy-0.9.6/tests/test_tappy.py
```

### Comparing `tappy-0.9.5/.github/workflows/python-package.yml` & `tappy-0.9.6/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/.pre-commit-config.yaml` & `tappy-0.9.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/BADGES.rst` & `tappy-0.9.6/BADGES.rst`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/CONTRIBUTING.rst` & `tappy-0.9.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/LICENSE.txt` & `tappy-0.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/PKG-INFO` & `tappy-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tappy
-Version: 0.9.5
+Version: 0.9.6
 Summary: Command line script and Python library to analyze tidal constituents.
 Home-page: https://timcera.bitbucket.io/
 Author: Tim Cera, PE
 Author-email: tim@cerazone.net
 License: BSD 3-Clause License
 Project-URL: documentation, https://timcera.bitbucket.io/tappy/docs/index.html#tappy-documentation,
 Project-URL: github, https://github.com/timcera/tappy,
```

### Comparing `tappy-0.9.5/README.rst` & `tappy-0.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/dist/tappy-0.9.3.tar.gz` & `tappy-0.9.6/dist/tappy-0.9.3.tar.gz`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/dist/tappy-0.9.4.tar.gz` & `tappy-0.9.6/dist/tappy-0.9.4.tar.gz`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/docs/CompareTidalFilters.rst` & `tappy-0.9.6/docs/CompareTidalFilters.rst`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/docs/Comparison_of_subtraction.png` & `tappy-0.9.6/docs/Comparison_of_subtraction.png`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/docs/Comparison_of_tidal_filters_large.png` & `tappy-0.9.6/docs/Comparison_of_tidal_filters_large.png`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/docs/Comparison_of_tidal_filters_small.png` & `tappy-0.9.6/docs/Comparison_of_tidal_filters_small.png`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/docs/HarmonicAnalysis.rst` & `tappy-0.9.6/docs/HarmonicAnalysis.rst`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/docs/Makefile` & `tappy-0.9.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/docs/Missing.png` & `tappy-0.9.6/docs/Missing.png`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/docs/TappyUsersGuide.rst` & `tappy-0.9.6/docs/TappyUsersGuide.rst`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/docs/TidalScience.rst` & `tappy-0.9.6/docs/TidalScience.rst`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/docs/conf.py` & `tappy-0.9.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/docs/index.rst` & `tappy-0.9.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/example/example.sh` & `tappy-0.9.6/example/example.sh`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/example/mayport_florida_8720220_con_noaa.txt` & `tappy-0.9.6/example/mayport_florida_8720220_con_noaa.txt`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/example/mayport_florida_8720220_con_tappy.txt` & `tappy-0.9.6/example/mayport_florida_8720220_con_tappy.txt`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/example/mayport_florida_8720220_data.txt` & `tappy-0.9.6/example/mayport_florida_8720220_data.txt`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/example/mayport_florida_8720220_data_def.txt` & `tappy-0.9.6/example/mayport_florida_8720220_data_def.txt`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/example/process_grace.py` & `tappy-0.9.6/example/process_grace.py`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/example/sparse.def` & `tappy-0.9.6/example/sparse.def`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/example/tidesandcurrents.def` & `tappy-0.9.6/example/tidesandcurrents.def`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/example/tridentpier_florida_8721604_con_noaa.txt` & `tappy-0.9.6/example/tridentpier_florida_8721604_con_noaa.txt`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/example/tridentpier_florida_8721604_con_tappy.txt` & `tappy-0.9.6/example/tridentpier_florida_8721604_con_tappy.txt`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/example/tridentpier_florida_8721604_data.txt.gz` & `tappy-0.9.6/example/tridentpier_florida_8721604_data.txt.gz`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/example/tridentpier_florida_8721604_datetime.txt.def` & `tappy-0.9.6/example/tridentpier_florida_8721604_datetime.txt.def`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/pyproject.toml` & `tappy-0.9.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
           ".coverage",
           ".deepsource.toml",
           ".ipynb_checkpoints/*"]
 
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.9.5"
+version = "0.9.6"
 tag_format = "$version"
 version_files = ["VERSION"]
 update_changelog_on_bump = true
 
 
 [build-system]
 requires = [
```

### Comparing `tappy-0.9.5/setup.cfg` & `tappy-0.9.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/setup.py` & `tappy-0.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/src/tappy/tappy.py` & `tappy-0.9.6/src/tappy/tappy.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 from scipy.optimize import leastsq
 
 from tappy.tappy_lib import sparser
 from tappy.tappy_lib.parameter_database import _master_speed_dict, letter_to_factor_map
 
 # ===globals======================
 modname = "tappy"
-__version__ = "0.9.0"
 
 # --option args--
 debug_p = 0
 # opt_b=None  #string arg, default is undefined
 
 # ---other---
 deg2rad = np.pi / 180.0
```

### Comparing `tappy-0.9.5/src/tappy/tappy_lib/filter.py` & `tappy-0.9.6/src/tappy/tappy_lib/filter.py`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/src/tappy/tappy_lib/parameter_database.py` & `tappy-0.9.6/src/tappy/tappy_lib/parameter_database.py`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/src/tappy/tappy_lib/sparser.py` & `tappy-0.9.6/src/tappy/tappy_lib/sparser.py`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/src/tappy.egg-info/PKG-INFO` & `tappy-0.9.6/src/tappy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tappy
-Version: 0.9.5
+Version: 0.9.6
 Summary: Command line script and Python library to analyze tidal constituents.
 Home-page: https://timcera.bitbucket.io/
 Author: Tim Cera, PE
 Author-email: tim@cerazone.net
 License: BSD 3-Clause License
 Project-URL: documentation, https://timcera.bitbucket.io/tappy/docs/index.html#tappy-documentation,
 Project-URL: github, https://github.com/timcera/tappy,
```

### Comparing `tappy-0.9.5/src/tappy.egg-info/SOURCES.txt` & `tappy-0.9.6/src/tappy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
 VERSION
 pyproject.toml
 setup.cfg
 setup.py
+.github/workflows/clean-workflow-runs.yml
 .github/workflows/python-package.yml
 dist/tappy-0.9.3.tar.gz
 dist/tappy-0.9.4.tar.gz
 docs/CompareTidalFilters.rst
 docs/Comparison_of_subtraction.png
 docs/Comparison_of_tidal_filters_large.png
 docs/Comparison_of_tidal_filters_small.png
@@ -38,14 +39,15 @@
 example/process_grace.py
 example/sparse.def
 example/tidesandcurrents.def
 example/tridentpier_florida_8721604_con_noaa.txt
 example/tridentpier_florida_8721604_con_tappy.txt
 example/tridentpier_florida_8721604_data.txt.gz
 example/tridentpier_florida_8721604_datetime.txt.def
+src/tappy/__init__.py
 src/tappy/tappy.py
 src/tappy.egg-info/PKG-INFO
 src/tappy.egg-info/SOURCES.txt
 src/tappy.egg-info/dependency_links.txt
 src/tappy.egg-info/entry_points.txt
 src/tappy.egg-info/not-zip-safe
 src/tappy.egg-info/requires.txt
```

### Comparing `tappy-0.9.5/tests/output_ts/constituents.dat` & `tappy-0.9.6/tests/output_ts/constituents.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_2MN6.dat` & `tappy-0.9.6/tests/output_ts/outts_2MN6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_2MS6.dat` & `tappy-0.9.6/tests/output_ts/outts_2MS6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_2Q1.dat` & `tappy-0.9.6/tests/output_ts/outts_2Q1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_2SM2.dat` & `tappy-0.9.6/tests/output_ts/outts_2SM2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_2SM6.dat` & `tappy-0.9.6/tests/output_ts/outts_2SM6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_J1.dat` & `tappy-0.9.6/tests/output_ts/outts_J1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_K1.dat` & `tappy-0.9.6/tests/output_ts/outts_K1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_M2.dat` & `tappy-0.9.6/tests/output_ts/outts_M2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_M3.dat` & `tappy-0.9.6/tests/output_ts/outts_M3.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_M4.dat` & `tappy-0.9.6/tests/output_ts/outts_M4.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_M6.dat` & `tappy-0.9.6/tests/output_ts/outts_M6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_M8.dat` & `tappy-0.9.6/tests/output_ts/outts_M8.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_MK3.dat` & `tappy-0.9.6/tests/output_ts/outts_MK3.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_MN4.dat` & `tappy-0.9.6/tests/output_ts/outts_MN4.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_MO3.dat` & `tappy-0.9.6/tests/output_ts/outts_MO3.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_MS4.dat` & `tappy-0.9.6/tests/output_ts/outts_MS4.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_MSf.dat` & `tappy-0.9.6/tests/output_ts/outts_MSf.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_N2.dat` & `tappy-0.9.6/tests/output_ts/outts_N2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_NO1.dat` & `tappy-0.9.6/tests/output_ts/outts_NO1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_O1.dat` & `tappy-0.9.6/tests/output_ts/outts_O1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_OO1.dat` & `tappy-0.9.6/tests/output_ts/outts_OO1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_Q1.dat` & `tappy-0.9.6/tests/output_ts/outts_Q1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_S2.dat` & `tappy-0.9.6/tests/output_ts/outts_S2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_S4.dat` & `tappy-0.9.6/tests/output_ts/outts_S4.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_S6.dat` & `tappy-0.9.6/tests/output_ts/outts_S6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_SK3.dat` & `tappy-0.9.6/tests/output_ts/outts_SK3.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_eta2.dat` & `tappy-0.9.6/tests/output_ts/outts_eta2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_2MN6.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_2MN6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_2MS6.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_2MS6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_2Q1.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_2Q1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_2SM2.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_2SM2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_2SM6.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_2SM6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_J1.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_J1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_K1.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_K1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_M2.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_M2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_M3.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_M3.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_M4.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_M4.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_M6.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_M6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_M8.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_M8.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_MK3.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_MK3.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_MN4.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_MN4.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_MO3.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_MO3.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_MS4.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_MS4.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_MSf.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_MSf.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_N2.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_N2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_NO1.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_NO1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_O1.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_O1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_OO1.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_OO1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_Q1.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_Q1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_S2.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_S2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_S4.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_S4.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_S6.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_S6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_SK3.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_SK3.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_eta2.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_eta2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ff_ups1.dat` & `tappy-0.9.6/tests/output_ts/outts_ff_ups1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_filtered_transform.dat` & `tappy-0.9.6/tests/output_ts/outts_filtered_transform.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_original.dat` & `tappy-0.9.6/tests/output_ts/outts_original.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_total_prediction.dat` & `tappy-0.9.6/tests/output_ts/outts_total_prediction.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_total_tidal_components.dat` & `tappy-0.9.6/tests/output_ts/outts_total_tidal_components.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/output_ts/outts_ups1.dat` & `tappy-0.9.6/tests/output_ts/outts_ups1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/sparse.def` & `tappy-0.9.6/tests/sparse.def`

 * *Files identical despite different names*

### Comparing `tappy-0.9.5/tests/test_tappy.py` & `tappy-0.9.6/tests/test_tappy.py`

 * *Files identical despite different names*


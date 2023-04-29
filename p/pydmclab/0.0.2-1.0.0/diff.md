# Comparing `tmp/pydmclab-0.0.2.tar.gz` & `tmp/pydmclab-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydmclab-0.0.2.tar", last modified: Mon Apr  3 22:06:39 2023, max compression
+gzip compressed data, was "pydmclab-1.0.0.tar", last modified: Sat Apr 29 17:44:37 2023, max compression
```

## Comparing `pydmclab-0.0.2.tar` & `pydmclab-1.0.0.tar`

### file list

```diff
@@ -1,78 +1,81 @@
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-03 22:06:39.782416 pydmclab-0.0.2/
--rw-------   0 cbartel    (503) staff       (20)     1071 2023-04-03 21:26:17.000000 pydmclab-0.0.2/LICENSE.txt
--rw-------   0 cbartel    (503) staff       (20)      173 2023-04-03 21:38:56.000000 pydmclab-0.0.2/MANIFEST.in
--rw-r--r--   0 cbartel    (503) staff       (20)      588 2023-04-03 22:06:39.782048 pydmclab-0.0.2/PKG-INFO
--rw-------   0 cbartel    (503) staff       (20)      116 2023-04-03 22:05:54.000000 pydmclab-0.0.2/README.md
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-03 22:06:39.713304 pydmclab-0.0.2/pydmclab/
--rw-------   0 cbartel    (503) staff       (20)      245 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/__init__.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-03 22:06:39.735020 pydmclab-0.0.2/pydmclab/core/
--rw-------   0 cbartel    (503) staff       (20)      398 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/core/README.md
--rw-------   0 cbartel    (503) staff       (20)      176 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/core/__init__.py
--rw-------   0 cbartel    (503) staff       (20)     3895 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/core/comp.py
--rw-r--r--   0 cbartel    (503) staff       (20)    12187 2023-04-03 21:34:13.000000 pydmclab-0.0.2/pydmclab/core/energies.py
--rw-------   0 cbartel    (503) staff       (20)    34041 2023-04-03 21:34:19.000000 pydmclab-0.0.2/pydmclab/core/hulls.py
--rw-------   0 cbartel    (503) staff       (20)    12067 2023-04-03 21:34:25.000000 pydmclab-0.0.2/pydmclab/core/mag.py
--rw-------   0 cbartel    (503) staff       (20)    15189 2023-04-03 21:34:29.000000 pydmclab-0.0.2/pydmclab/core/query.py
--rw-------   0 cbartel    (503) staff       (20)    12279 2023-04-03 21:34:35.000000 pydmclab-0.0.2/pydmclab/core/struc.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-03 22:06:39.745566 pydmclab-0.0.2/pydmclab/data/
--rw-r--r--   0 cbartel    (503) staff       (20)     6148 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/.DS_Store
--rw-------   0 cbartel    (503) staff       (20)      346 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/README.md
--rw-------   0 cbartel    (503) staff       (20)      331 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/__init__.py
--rw-------   0 cbartel    (503) staff       (20)      916 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/configs.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-03 22:06:39.759865 pydmclab-0.0.2/pydmclab/data/data/
--rw-r--r--   0 cbartel    (503) staff       (20)    15963 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/data/221220_dmc-mus.json
--rw-r--r--   0 cbartel    (503) staff       (20)     7720 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/data/230122_dmc-mus.json
--rw-r--r--   0 cbartel    (503) staff       (20)     1233 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/data/_batch_vasp_analysis_configs.yaml
--rw-------   0 cbartel    (503) staff       (20)      405 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/data/_launch_configs.yaml
--rw-------   0 cbartel    (503) staff       (20)     1496 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/data/_partition_configs.yaml
--rw-------   0 cbartel    (503) staff       (20)      573 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/data/_slurm_configs.yaml
--rw-r--r--   0 cbartel    (503) staff       (20)     1414 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/data/_sub_configs.yaml
--rw-------   0 cbartel    (503) staff       (20)     1561 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/data/_vasp_configs.yaml
--rw-------   0 cbartel    (503) staff       (20)     1570 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/data/atomic_masses.json
--rw-r--r--   0 cbartel    (503) staff       (20)     3140 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/data/bartel2019_npj_reference-energies.csv
--rw-r--r--   0 cbartel    (503) staff       (20)     2596 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/data/colors.json
--rw-------   0 cbartel    (503) staff       (20)    40326 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/data/elemental_gibbs_energies_T.json
--rw-r--r--   0 cbartel    (503) staff       (20)     3788 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/data/mus_from_bartel2019_npj.json
--rw-r--r--   0 cbartel    (503) staff       (20)     7719 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/data/mus_from_dmc_no_corrections.json
--rw-------   0 cbartel    (503) staff       (20)     1710 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/data/mus_from_mp_no_corrections.json
--rw-------   0 cbartel    (503) staff       (20)    43287 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/data/ssub.dat
--rw-r--r--   0 cbartel    (503) staff       (20)    45994 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/data/ssub.json
--rw-------   0 cbartel    (503) staff       (20)      246 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/data/features.py
--rw-r--r--   0 cbartel    (503) staff       (20)     2252 2023-04-03 21:35:30.000000 pydmclab-0.0.2/pydmclab/data/plotting_configs.py
--rw-r--r--   0 cbartel    (503) staff       (20)     4026 2023-04-03 21:35:26.000000 pydmclab-0.0.2/pydmclab/data/thermochem.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-03 22:06:39.769490 pydmclab-0.0.2/pydmclab/demos/
--rw-------   0 cbartel    (503) staff       (20)     2990 2023-04-03 21:35:25.000000 pydmclab-0.0.2/pydmclab/demos/demo_comp.py
--rw-------   0 cbartel    (503) staff       (20)    10604 2023-04-03 21:35:25.000000 pydmclab-0.0.2/pydmclab/demos/demo_hulls.py
--rw-------   0 cbartel    (503) staff       (20)     4333 2023-04-03 21:35:45.000000 pydmclab-0.0.2/pydmclab/demos/demo_query.py
--rw-------   0 cbartel    (503) staff       (20)     2494 2023-04-03 21:35:23.000000 pydmclab-0.0.2/pydmclab/demos/demo_struc.py
--rw-------   0 cbartel    (503) staff       (20)    27905 2023-04-03 21:55:04.000000 pydmclab-0.0.2/pydmclab/demos/demo_vasp_template.py
--rw-------   0 cbartel    (503) staff       (20)    28183 2023-04-03 21:54:59.000000 pydmclab-0.0.2/pydmclab/demos/demo_vasp_test-mp-chemsys.py
--rw-------   0 cbartel    (503) staff       (20)    28075 2023-04-03 21:55:19.000000 pydmclab-0.0.2/pydmclab/demos/demo_vasp_test-template.py
--rw-------   0 cbartel    (503) staff       (20)    28376 2023-04-03 21:55:14.000000 pydmclab-0.0.2/pydmclab/demos/demo_vasp_test-transform-strucs.py
--rw-------   0 cbartel    (503) staff       (20)    28254 2023-04-03 21:55:09.000000 pydmclab-0.0.2/pydmclab/demos/demo_vasp_test-typical-dmc.py
--rw-r--r--   0 cbartel    (503) staff       (20)    23914 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/demos/tmp.png
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-03 22:06:39.773662 pydmclab-0.0.2/pydmclab/dev/
--rw-------   0 cbartel    (503) staff       (20)       48 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/dev/__init__.py
--rw-------   0 cbartel    (503) staff       (20)     3091 2023-04-03 21:37:38.000000 pydmclab-0.0.2/pydmclab/dev/entries.py
--rw-------   0 cbartel    (503) staff       (20)      170 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/dev/grand.py
--rw-r--r--   0 cbartel    (503) staff       (20)     3911 2023-04-03 21:36:53.000000 pydmclab-0.0.2/pydmclab/dev/reactions.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-03 22:06:39.779095 pydmclab-0.0.2/pydmclab/hpc/
--rw-------   0 cbartel    (503) staff       (20)      707 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/hpc/README.md
--rw-------   0 cbartel    (503) staff       (20)      156 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/hpc/__init__.py
--rw-r--r--   0 cbartel    (503) staff       (20)    48098 2023-04-03 21:37:02.000000 pydmclab-0.0.2/pydmclab/hpc/analyze.py
--rw-------   0 cbartel    (503) staff       (20)    11935 2023-04-03 21:37:12.000000 pydmclab-0.0.2/pydmclab/hpc/launch.py
--rw-r--r--   0 cbartel    (503) staff       (20)    36673 2023-04-03 21:37:21.000000 pydmclab-0.0.2/pydmclab/hpc/submit.py
--rw-r--r--   0 cbartel    (503) staff       (20)    26676 2023-04-03 21:37:28.000000 pydmclab-0.0.2/pydmclab/hpc/vasp.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-03 22:06:39.781472 pydmclab-0.0.2/pydmclab/utils/
--rw-------   0 cbartel    (503) staff       (20)      271 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/utils/README.md
--rw-r--r--   0 cbartel    (503) staff       (20)      201 2023-04-03 21:26:17.000000 pydmclab-0.0.2/pydmclab/utils/__init__.py
--rw-r--r--   0 cbartel    (503) staff       (20)     4097 2023-04-03 21:38:03.000000 pydmclab-0.0.2/pydmclab/utils/handy.py
--rw-------   0 cbartel    (503) staff       (20)     1659 2023-04-03 21:38:07.000000 pydmclab-0.0.2/pydmclab/utils/plotting.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-03 22:06:39.718650 pydmclab-0.0.2/pydmclab.egg-info/
--rw-r--r--   0 cbartel    (503) staff       (20)      588 2023-04-03 22:06:39.000000 pydmclab-0.0.2/pydmclab.egg-info/PKG-INFO
--rw-r--r--   0 cbartel    (503) staff       (20)     2005 2023-04-03 22:06:39.000000 pydmclab-0.0.2/pydmclab.egg-info/SOURCES.txt
--rw-r--r--   0 cbartel    (503) staff       (20)        1 2023-04-03 22:06:39.000000 pydmclab-0.0.2/pydmclab.egg-info/dependency_links.txt
--rw-r--r--   0 cbartel    (503) staff       (20)       15 2023-04-03 22:06:39.000000 pydmclab-0.0.2/pydmclab.egg-info/requires.txt
--rw-r--r--   0 cbartel    (503) staff       (20)        9 2023-04-03 22:06:39.000000 pydmclab-0.0.2/pydmclab.egg-info/top_level.txt
--rw-r--r--   0 cbartel    (503) staff       (20)       38 2023-04-03 22:06:39.782482 pydmclab-0.0.2/setup.cfg
--rw-r--r--   0 cbartel    (503) staff       (20)     2539 2023-04-03 21:52:12.000000 pydmclab-0.0.2/setup.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.461262 pydmclab-1.0.0/
+-rw-------   0 cbartel    (503) staff       (20)     1071 2023-04-03 21:26:17.000000 pydmclab-1.0.0/LICENSE.txt
+-rw-------   0 cbartel    (503) staff       (20)      173 2023-04-03 21:38:56.000000 pydmclab-1.0.0/MANIFEST.in
+-rw-r--r--   0 cbartel    (503) staff       (20)      642 2023-04-29 17:44:37.461028 pydmclab-1.0.0/PKG-INFO
+-rw-------   0 cbartel    (503) staff       (20)      170 2023-04-05 14:50:32.000000 pydmclab-1.0.0/README.md
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.363164 pydmclab-1.0.0/pydmclab/
+-rw-------   0 cbartel    (503) staff       (20)      245 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/__init__.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.379480 pydmclab-1.0.0/pydmclab/core/
+-rw-------   0 cbartel    (503) staff       (20)      398 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/core/README.md
+-rw-------   0 cbartel    (503) staff       (20)      176 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/core/__init__.py
+-rw-------   0 cbartel    (503) staff       (20)     3895 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/core/comp.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    12187 2023-04-03 21:34:13.000000 pydmclab-1.0.0/pydmclab/core/energies.py
+-rw-------   0 cbartel    (503) staff       (20)    52660 2023-04-29 17:43:03.000000 pydmclab-1.0.0/pydmclab/core/hulls.py
+-rw-------   0 cbartel    (503) staff       (20)    12067 2023-04-03 21:34:25.000000 pydmclab-1.0.0/pydmclab/core/mag.py
+-rw-------   0 cbartel    (503) staff       (20)    15189 2023-04-03 21:34:29.000000 pydmclab-1.0.0/pydmclab/core/query.py
+-rw-------   0 cbartel    (503) staff       (20)    13148 2023-04-10 22:21:48.000000 pydmclab-1.0.0/pydmclab/core/struc.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.394135 pydmclab-1.0.0/pydmclab/data/
+-rw-r--r--   0 cbartel    (503) staff       (20)     6148 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/.DS_Store
+-rw-------   0 cbartel    (503) staff       (20)      346 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/README.md
+-rw-------   0 cbartel    (503) staff       (20)      331 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/__init__.py
+-rw-------   0 cbartel    (503) staff       (20)      916 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/configs.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.437059 pydmclab-1.0.0/pydmclab/data/data/
+-rw-r--r--   0 cbartel    (503) staff       (20)    15963 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/221220_dmc-mus.json
+-rw-r--r--   0 cbartel    (503) staff       (20)     7720 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/230122_dmc-mus.json
+-rw-r--r--   0 cbartel    (503) staff       (20)     1241 2023-04-17 14:02:36.000000 pydmclab-1.0.0/pydmclab/data/data/_batch_vasp_analysis_configs.yaml
+-rw-------   0 cbartel    (503) staff       (20)      437 2023-04-17 14:52:59.000000 pydmclab-1.0.0/pydmclab/data/data/_launch_configs.yaml
+-rw-------   0 cbartel    (503) staff       (20)     1496 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/_partition_configs.yaml
+-rw-------   0 cbartel    (503) staff       (20)      573 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/_slurm_configs.yaml
+-rw-r--r--   0 cbartel    (503) staff       (20)     1414 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/_sub_configs.yaml
+-rw-------   0 cbartel    (503) staff       (20)     1561 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/_vasp_configs.yaml
+-rw-------   0 cbartel    (503) staff       (20)     1570 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/atomic_masses.json
+-rw-r--r--   0 cbartel    (503) staff       (20)     3140 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/bartel2019_npj_reference-energies.csv
+-rw-r--r--   0 cbartel    (503) staff       (20)     2596 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/colors.json
+-rw-------   0 cbartel    (503) staff       (20)    40326 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/elemental_gibbs_energies_T.json
+-rw-r--r--   0 cbartel    (503) staff       (20)     3788 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/mus_from_bartel2019_npj.json
+-rw-r--r--   0 cbartel    (503) staff       (20)     7719 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/mus_from_dmc_no_corrections.json
+-rw-------   0 cbartel    (503) staff       (20)     1710 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/mus_from_mp_no_corrections.json
+-rw-------   0 cbartel    (503) staff       (20)    43287 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/ssub.dat
+-rw-r--r--   0 cbartel    (503) staff       (20)    45994 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/ssub.json
+-rw-------   0 cbartel    (503) staff       (20)      246 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/features.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     2252 2023-04-03 21:35:30.000000 pydmclab-1.0.0/pydmclab/data/plotting_configs.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     4026 2023-04-03 21:35:26.000000 pydmclab-1.0.0/pydmclab/data/thermochem.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.445374 pydmclab-1.0.0/pydmclab/demos/
+-rw-------   0 cbartel    (503) staff       (20)     2990 2023-04-03 21:35:25.000000 pydmclab-1.0.0/pydmclab/demos/demo_comp.py
+-rw-------   0 cbartel    (503) staff       (20)    10887 2023-04-26 22:19:29.000000 pydmclab-1.0.0/pydmclab/demos/demo_hulls.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    32860 2023-04-17 22:09:59.000000 pydmclab-1.0.0/pydmclab/demos/demo_launcher_template.py
+-rw-------   0 cbartel    (503) staff       (20)     4333 2023-04-03 21:35:45.000000 pydmclab-1.0.0/pydmclab/demos/demo_query.py
+-rw-------   0 cbartel    (503) staff       (20)     2494 2023-04-03 21:35:23.000000 pydmclab-1.0.0/pydmclab/demos/demo_struc.py
+-rw-------   0 cbartel    (503) staff       (20)    27730 2023-04-17 14:10:29.000000 pydmclab-1.0.0/pydmclab/demos/demo_vasp_template.py
+-rw-------   0 cbartel    (503) staff       (20)    28183 2023-04-04 14:55:15.000000 pydmclab-1.0.0/pydmclab/demos/demo_vasp_test-mp-chemsys.py
+-rw-------   0 cbartel    (503) staff       (20)    28075 2023-04-03 21:55:19.000000 pydmclab-1.0.0/pydmclab/demos/demo_vasp_test-template.py
+-rw-------   0 cbartel    (503) staff       (20)    28376 2023-04-03 21:55:14.000000 pydmclab-1.0.0/pydmclab/demos/demo_vasp_test-transform-strucs.py
+-rw-------   0 cbartel    (503) staff       (20)    28254 2023-04-03 21:55:09.000000 pydmclab-1.0.0/pydmclab/demos/demo_vasp_test-typical-dmc.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    23914 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/demos/tmp.png
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.449517 pydmclab-1.0.0/pydmclab/dev/
+-rw-r--r--   0 cbartel    (503) staff       (20)      153 2023-04-19 19:26:44.000000 pydmclab-1.0.0/pydmclab/dev/Untitled-2.py
+-rw-------   0 cbartel    (503) staff       (20)       48 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/dev/__init__.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     7018 2023-04-29 17:42:52.000000 pydmclab-1.0.0/pydmclab/dev/echem.py
+-rw-------   0 cbartel    (503) staff       (20)     3091 2023-04-03 21:37:38.000000 pydmclab-1.0.0/pydmclab/dev/entries.py
+-rw-------   0 cbartel    (503) staff       (20)      170 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/dev/grand.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     3911 2023-04-03 21:36:53.000000 pydmclab-1.0.0/pydmclab/dev/reactions.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.455356 pydmclab-1.0.0/pydmclab/hpc/
+-rw-------   0 cbartel    (503) staff       (20)      707 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/hpc/README.md
+-rw-------   0 cbartel    (503) staff       (20)      156 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/hpc/__init__.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    50350 2023-04-17 17:05:40.000000 pydmclab-1.0.0/pydmclab/hpc/analyze.py
+-rw-------   0 cbartel    (503) staff       (20)    13255 2023-04-17 14:57:25.000000 pydmclab-1.0.0/pydmclab/hpc/launch.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    43385 2023-04-17 17:05:40.000000 pydmclab-1.0.0/pydmclab/hpc/submit.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    26676 2023-04-03 21:37:28.000000 pydmclab-1.0.0/pydmclab/hpc/vasp.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.460101 pydmclab-1.0.0/pydmclab/utils/
+-rw-------   0 cbartel    (503) staff       (20)      271 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/utils/README.md
+-rw-r--r--   0 cbartel    (503) staff       (20)      201 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/utils/__init__.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     4097 2023-04-03 21:38:03.000000 pydmclab-1.0.0/pydmclab/utils/handy.py
+-rw-------   0 cbartel    (503) staff       (20)     1659 2023-04-03 21:38:07.000000 pydmclab-1.0.0/pydmclab/utils/plotting.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.366552 pydmclab-1.0.0/pydmclab.egg-info/
+-rw-r--r--   0 cbartel    (503) staff       (20)      642 2023-04-29 17:44:37.000000 pydmclab-1.0.0/pydmclab.egg-info/PKG-INFO
+-rw-r--r--   0 cbartel    (503) staff       (20)     2095 2023-04-29 17:44:37.000000 pydmclab-1.0.0/pydmclab.egg-info/SOURCES.txt
+-rw-r--r--   0 cbartel    (503) staff       (20)        1 2023-04-29 17:44:37.000000 pydmclab-1.0.0/pydmclab.egg-info/dependency_links.txt
+-rw-r--r--   0 cbartel    (503) staff       (20)       15 2023-04-29 17:44:37.000000 pydmclab-1.0.0/pydmclab.egg-info/requires.txt
+-rw-r--r--   0 cbartel    (503) staff       (20)        9 2023-04-29 17:44:37.000000 pydmclab-1.0.0/pydmclab.egg-info/top_level.txt
+-rw-r--r--   0 cbartel    (503) staff       (20)       38 2023-04-29 17:44:37.461324 pydmclab-1.0.0/setup.cfg
+-rw-r--r--   0 cbartel    (503) staff       (20)     2539 2023-04-17 17:59:25.000000 pydmclab-1.0.0/setup.py
```

### Comparing `pydmclab-0.0.2/LICENSE.txt` & `pydmclab-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/PKG-INFO` & `pydmclab-1.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydmclab
-Version: 0.0.2
+Version: 1.0.0
 Summary: Package to facilitate DFT calculations and analysis
 Home-page: https://github.umn.edu/bartel-group/pydmclab
 Author: Chris Bartel
 Author-email: cbartel@umn.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,7 +13,9 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # pydmclab
 
 - common framework to rely upon for typical calculations and analysis done in the Bartel research group
+
+- documentation details can be found [here](docs.md)
```

### Comparing `pydmclab-0.0.2/pydmclab/core/comp.py` & `pydmclab-1.0.0/pydmclab/core/comp.py`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/core/energies.py` & `pydmclab-1.0.0/pydmclab/core/energies.py`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/core/mag.py` & `pydmclab-1.0.0/pydmclab/core/mag.py`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/core/query.py` & `pydmclab-1.0.0/pydmclab/core/query.py`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/core/struc.py` & `pydmclab-1.0.0/pydmclab/core/struc.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,14 +291,39 @@
 
         Returns:
             spacegroup number or symbol with loose or tight tolerance
         """
         sg_info = self.spacegroup_info
         return sg_info[loose_or_tight][number_or_symbol]
 
+    def scale_structure(self, scale_factor, structure=None):
+        """_summary_
+
+        Args:
+            scale_factor (float): fractional scaling of the structure volume
+                - e.g., 1.2 will increase each lattice vector by 20%
+                - e.g., 0.8 will make eaech lattice vector 80% of the initial length
+                - e.g., 1.0 will do nothing
+
+            structure (Structure, optional): structure to scale. Defaults to None.
+                - if None will use self.structure fed to initialization
+
+        Returns:
+            pymatgen structure object
+        """
+        if not structure:
+            structure = self.structure.copy()
+        else:
+            structure = structure.copy()
+        orig_vol = structure.volume
+        new_vol = orig_vol * scale_factor
+        structure.scale_lattice(new_vol)
+
+        return structure
+
 
 class SiteTools(object):
     """
     make it a little easier to get site info from structures
 
     """
```

### Comparing `pydmclab-0.0.2/pydmclab/data/.DS_Store` & `pydmclab-1.0.0/pydmclab/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/data/configs.py` & `pydmclab-1.0.0/pydmclab/data/configs.py`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/data/data/221220_dmc-mus.json` & `pydmclab-1.0.0/pydmclab/data/data/221220_dmc-mus.json`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/data/data/230122_dmc-mus.json` & `pydmclab-1.0.0/pydmclab/data/data/230122_dmc-mus.json`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/data/data/_batch_vasp_analysis_configs.yaml` & `pydmclab-1.0.0/pydmclab/data/data/_batch_vasp_analysis_configs.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 only_static: True # only retrieve data from the static calculations
 one_xc: # if None, retrieve all xcs, else retrieve only the one specified
 check_relax: True # make sure the relax calculation and the static have similar energies
 include_meta: True # include metadata like INCAR, KPOINTS, POTCAR settings
 include_calc_setup: True # include things related to the calculation setup -- standard, mag, final_xc, etc
-include_structure: True # include the relaxed crystal structure as a dict
-include_mag: True # include the relaxed magnetization info as as dict
-include_tdos: True # include the light version of the density of states
-include_pdos: True # include heavy dos
-include_charge: True # include partial chage info
-include_madelung: True # include Madelung energies
-include_tcohp: True # include light COHPCAR data
-include_pcohp: True # include heavy COHPCAR data
+include_structure: False # include the relaxed crystal structure as a dict
+include_mag: False # include the relaxed magnetization info as as dict
+include_tdos: False # include the light version of the density of states
+include_pdos: False # include heavy dos
+include_charge: False # include partial chage info
+include_madelung: False # include Madelung energies
+include_tcohp: False # include light COHPCAR data
+include_pcohp: False # include heavy COHPCAR data
 include_tcoop: False # include light COOPCAR data
 include_pcoop: False # include heavy COOPCAR data
 include_tcobi: False # include light COBICAR data
 include_pcobi: False # include heavy COBICAR data
 create_cif: True # create a .cif file for each CONTCAR
 verbose: True # print stuff as things get analyzed
 n_procs: 1 # how many cores to parallelize the analysis over
```

### Comparing `pydmclab-0.0.2/pydmclab/data/data/_partition_configs.yaml` & `pydmclab-1.0.0/pydmclab/data/data/_partition_configs.yaml`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/data/data/_slurm_configs.yaml` & `pydmclab-1.0.0/pydmclab/data/data/_slurm_configs.yaml`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/data/data/_sub_configs.yaml` & `pydmclab-1.0.0/pydmclab/data/data/_sub_configs.yaml`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/data/data/_vasp_configs.yaml` & `pydmclab-1.0.0/pydmclab/data/data/_vasp_configs.yaml`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/data/data/atomic_masses.json` & `pydmclab-1.0.0/pydmclab/data/data/atomic_masses.json`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/data/data/bartel2019_npj_reference-energies.csv` & `pydmclab-1.0.0/pydmclab/data/data/bartel2019_npj_reference-energies.csv`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/data/data/colors.json` & `pydmclab-1.0.0/pydmclab/data/data/colors.json`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/data/data/elemental_gibbs_energies_T.json` & `pydmclab-1.0.0/pydmclab/data/data/elemental_gibbs_energies_T.json`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/data/data/mus_from_bartel2019_npj.json` & `pydmclab-1.0.0/pydmclab/data/data/mus_from_bartel2019_npj.json`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/data/data/mus_from_dmc_no_corrections.json` & `pydmclab-1.0.0/pydmclab/data/data/mus_from_dmc_no_corrections.json`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/data/data/mus_from_mp_no_corrections.json` & `pydmclab-1.0.0/pydmclab/data/data/mus_from_mp_no_corrections.json`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/data/data/ssub.dat` & `pydmclab-1.0.0/pydmclab/data/data/ssub.dat`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/data/data/ssub.json` & `pydmclab-1.0.0/pydmclab/data/data/ssub.json`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/data/plotting_configs.py` & `pydmclab-1.0.0/pydmclab/data/plotting_configs.py`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/data/thermochem.py` & `pydmclab-1.0.0/pydmclab/data/thermochem.py`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/demos/demo_comp.py` & `pydmclab-1.0.0/pydmclab/demos/demo_comp.py`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/demos/demo_hulls.py` & `pydmclab-1.0.0/pydmclab/demos/demo_hulls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pydmclab.core.comp import CompTools
 from pydmclab.core.query import MPQuery
 from pydmclab.core.hulls import GetHullInputData, AnalyzeHull, ParallelHulls
 from pydmclab.utils.handy import read_json, write_json
-from pydmclab.utils.plotting import set_rc_params, tableau_colors
+from pydmclab.utils.plotting import set_rc_params, get_colors
 from pydmclab.data.thermochem import mus_at_0K, mus_at_T
 
 import matplotlib.pyplot as plt
 
 import os
 import numpy as np
 
@@ -21,53 +21,65 @@
 TO-DO:
     - convert into formal "tests"
 """
 # Chris B's API key for MP query
 API_KEY = "N3KdATtMmcsUL94g"
 
 # chemical system to test on
-CHEMSYS = "Ca-Al-Ti-O-F"
+CHEMSYS = "Ca-Al-Ti-F"
 
 # where to save data
 DATA_DIR = os.path.join("output", "hulls", "data")
 if not os.path.exists(DATA_DIR):
     os.mkdir(DATA_DIR)
 
 # where to save figures
 FIG_DIR = os.path.join("output", "hulls", "figures")
 if not os.path.exists(FIG_DIR):
     os.mkdir(FIG_DIR)
 
 
 def get_mp_data_for_chemsys(
-    chemsys=CHEMSYS,
+    comp=CHEMSYS,
+    properties=None,
+    criteria={},
     only_gs=True,
-    dict_key="cmpd",
-    remake=False,
+    include_structure=True,
+    supercell_structure=False,
+    max_Ehull=0.1,
+    max_sites_per_structure=100,
+    max_strucs_per_cmpd=5,
     data_dir=DATA_DIR,
-    api_key=API_KEY,
+    remake=False,
 ):
     """
     Args:
         chemsys (str): chemical system to query ('-'.join([elements]))
         only_gs (bool): if True, remove non-ground state polymorphs from MP query
             - good practice to do this before doing hull analysis b/c non-gs polymorphs trivially have Ehull=Ehull_gs + dE_polymorph-gs
         dict_key (str): key to use to orient dictionary of MPQuery results
             - 'cmpd' is the default behavior in MPQuery, meaning we get a dictionary that looks like {CHEMICAL_FORMULA : {DATA}}
         remake (bool): if True, re-query MP
 
     Returns:
         gs (dict): dictionary of ground state data from MPQuery for chemsys
     """
-    fjson = os.path.join(data_dir, "query_" + chemsys + ".json")
+    fjson = os.path.join(data_dir, "query_" + comp + ".json")
     if not remake and os.path.exists(fjson):
         return read_json(fjson)
 
-    mpq = MPQuery(api_key)
-    out = mpq.get_data_for_comp(comp=chemsys, only_gs=only_gs, dict_key=dict_key)
+    mpq = MPQuery(API_KEY)
+    d = mpq.get_data_for_comp(comp=comp, only_gs=only_gs)
+
+    out = {}
+    formulas = list(set([d[k]["cmpd"] for k in d]))
+    for formula in formulas:
+        # NOTE: this only works because I know my query only has 1 structure per formula (only_gs = True)
+        gs_key = [k for k in d if d[k]["cmpd"] == formula][0]
+        out[formula] = d[gs_key]
     return write_json(out, fjson)
 
 
 def serial_get_hull_input_data(
     gs, formation_energy_key="Ef_mp", remake=False, data_dir=DATA_DIR, chemsys=CHEMSYS
 ):
     """
@@ -256,18 +268,14 @@
     # if True, re-calculate hull output data
     remake_serial_hullout = True
     # if True, re-calculate hull output data in parallel
     remake_parallel_hullout = True
     # if True, generate figure to check results
     remake_hull_figure_check = True
 
-    # if True, test chemical potential stuff
-
-    remake_mus_figure_check = True
-
     # MP query for CHEMSYS
     gs = get_mp_data_for_chemsys(CHEMSYS, remake=remake_query)
 
     # hull input data for CHEMSYS
     hullin = serial_get_hull_input_data(gs, remake=remake_serial_hullin)
 
     # hull output data for CHEMSYS
@@ -284,10 +292,9 @@
         plot_to_check_success(gs, hullout, p_hullout)
         # %%
 
     return gs, hullin, hullout, p_hullout
 
 
 if __name__ == "__main__":
-
     # MP Query --> hull input data (serial) --> hull output data (serial) --> hull output data (parallel)
-    gs, hullin, hullout, p_hullout = main()
+    gs = main()
```

### Comparing `pydmclab-0.0.2/pydmclab/demos/demo_query.py` & `pydmclab-1.0.0/pydmclab/demos/demo_query.py`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/demos/demo_struc.py` & `pydmclab-1.0.0/pydmclab/demos/demo_struc.py`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/demos/demo_vasp_template.py` & `pydmclab-1.0.0/pydmclab/demos/demo_vasp_test-template.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,50 +166,50 @@
 API_KEY = "N3KdATtMmcsUL94g"
 
 # lets put a tag on all the files we save
 FILE_TAG = CALCS_DIR.split("/")[-2]
 
 # what to query MP for
 ## e.g., 'MnO2', ['MnO2', 'TiO2'], 'Ca-Ti-O, etc
-COMPOSITIONS = None
+COMPOSITIONS = "MnO2"
 
 # how to transform MP structures
 ## e.g., [x/8 for x in range(9)]
 ## NOTE: you need to modify get_strucs to make this work (hard to generalize)
 TRANSFORM_STRUCS = False
 
 # whether or not you want to generate MAGMOMs
 ## True if you're running AFM, else False
-GEN_MAGMOMS = False
+GEN_MAGMOMS = True
 
 # what {standard : [final_xcs]} to calculate
 ## e.g., {'dmc' : ['metagga', 'ggau']} if you want to run METAGGA + GGA+U at DMC standards
-TO_LAUNCH = {}
+TO_LAUNCH = {"dmc": ["metagga", "ggau"]}
 
 # any configurations related to LaunchTools
 ## e.g., {'compare_to_mp' : True, 'n_afm_configs' : 4}
-LAUNCH_CONFIGS = {}
+LAUNCH_CONFIGS = {"compare_to_mp": True, "n_afm_configs": 1}
 
 # any configurations related to SubmitTools
 ## usually no need to change anything but n_procs... n_procs will determine how to parallelize over launch_dirs
 ## NOTE: do not set n_procs = 'all' unless you are running on a compute node (ie not a login node)
 SUB_CONFIGS = {"n_procs": 1}
 
 # any configurations related to Slurm
 ## e.g., {'ntasks' : 16, 'time' : int(24*60)}
-SLURM_CONFIGS = {}
+SLURM_CONFIGS = {"ntasks": 16, "time": int(24 * 60)}
 
 # any configurations related to VASPSetUp
 ## e.g., {'lobster_static' : True, 'relax_incar' : {'ENCUT' : 555}}
-VASP_CONFIGS = {}
+VASP_CONFIGS = {"lobster_static": True, "relax_incar": {"ENCUT": 555}}
 
 # any configurations related to AnalyzeBatch
 ## e.g., {'include_meta' : True, 'include_mag' : True, 'n_procs' : 4}
 ## NOTE: do not set n_procs = 'all' unless you are running on a compute node (ie not a login node)
-ANALYSIS_CONFIGS = {}
+ANALYSIS_CONFIGS = {"include_meta": True, "include_mag": True, "n_procs": 4}
 
 """
 Don't forget to inspect the arguments to:
     get_query
     get_strucs
     get_magmoms
     get_launch_dirs
@@ -304,15 +304,18 @@
     return read_json(fjson)
 
 
 def check_query(query):
     for mpid in query:
         print("\nmpid: %s" % mpid)
         print("\tcmpd: %s" % query[mpid]["cmpd"])
-        print("\tstructure formula: %s" % StrucTools(query[mpid]["structure"]).formula)
+        print(
+            "\tstructure formula: %s"
+            % len(StrucTools(query[mpid]["structure"]).formula)
+        )
 
 
 def get_strucs(
     query,
     transform_strucs,
     max_strucs_per_starting_struc=1,
     ox_states=None,
@@ -670,15 +673,15 @@
 
     data = analyzer.results
 
     write_json(data, fjson)
     return read_json(fjson)
 
 
-def check_results(results, print_structure=False):
+def check_results(results):
 
     keys_to_check = list(results.keys())
 
     converged = 0
     for key in keys_to_check:
         top_level, ID, standard, mag, xc_calc = key.split(".")
         data = results[key]
@@ -699,18 +702,16 @@
                 and (ANALYSIS_CONFIGS["include_mag"])
             ):
                 magnetization = data["magnetization"]
                 an_el = list(magnetization.keys())[0]
                 an_idx = list(magnetization[an_el].keys())[0]
                 that_mag = magnetization[an_el][an_idx]["mag"]
                 print("mag on %s (%s) = %.2f" % (an_el, str(an_idx), that_mag))
-            if (
-                (print_structure)
-                and ("include_structure" not in ANALYSIS_CONFIGS)
-                or (ANALYSIS_CONFIGS["include_structure"])
+            if ("include_structure" not in ANALYSIS_CONFIGS) or (
+                ANALYSIS_CONFIGS["include_structure"]
             ):
                 print(data["structure"])
 
     print("\n\n SUMMARY: %i/%i converged" % (converged, len(keys_to_check)))
 
 
 def main():
```

### Comparing `pydmclab-0.0.2/pydmclab/demos/demo_vasp_test-mp-chemsys.py` & `pydmclab-1.0.0/pydmclab/demos/demo_vasp_test-mp-chemsys.py`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/demos/demo_vasp_test-template.py` & `pydmclab-1.0.0/pydmclab/demos/demo_vasp_test-typical-dmc.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,45 +166,45 @@
 API_KEY = "N3KdATtMmcsUL94g"
 
 # lets put a tag on all the files we save
 FILE_TAG = CALCS_DIR.split("/")[-2]
 
 # what to query MP for
 ## e.g., 'MnO2', ['MnO2', 'TiO2'], 'Ca-Ti-O, etc
-COMPOSITIONS = "MnO2"
+COMPOSITIONS = ["Zn3MoN4", "ZnMoN2"]
 
 # how to transform MP structures
-## e.g., [x/8 for x in range(9)]
+## e.g., [x for x in range(5)] ([0,1,2,3,4])
 ## NOTE: you need to modify get_strucs to make this work (hard to generalize)
 TRANSFORM_STRUCS = False
 
 # whether or not you want to generate MAGMOMs
 ## True if you're running AFM, else False
 GEN_MAGMOMS = True
 
 # what {standard : [final_xcs]} to calculate
 ## e.g., {'dmc' : ['metagga', 'ggau']} if you want to run METAGGA + GGA+U at DMC standards
-TO_LAUNCH = {"dmc": ["metagga", "ggau"]}
+TO_LAUNCH = {"dmc": ["metagga"]}
 
 # any configurations related to LaunchTools
 ## e.g., {'compare_to_mp' : True, 'n_afm_configs' : 4}
-LAUNCH_CONFIGS = {"compare_to_mp": True, "n_afm_configs": 1}
+LAUNCH_CONFIGS = {"compare_to_mp": False, "n_afm_configs": 2}
 
 # any configurations related to SubmitTools
 ## usually no need to change anything but n_procs... n_procs will determine how to parallelize over launch_dirs
 ## NOTE: do not set n_procs = 'all' unless you are running on a compute node (ie not a login node)
 SUB_CONFIGS = {"n_procs": 1}
 
 # any configurations related to Slurm
 ## e.g., {'ntasks' : 16, 'time' : int(24*60)}
 SLURM_CONFIGS = {"ntasks": 16, "time": int(24 * 60)}
 
 # any configurations related to VASPSetUp
 ## e.g., {'lobster_static' : True, 'relax_incar' : {'ENCUT' : 555}}
-VASP_CONFIGS = {"lobster_static": True, "relax_incar": {"ENCUT": 555}}
+VASP_CONFIGS = {"lobster_static": True}
 
 # any configurations related to AnalyzeBatch
 ## e.g., {'include_meta' : True, 'include_mag' : True, 'n_procs' : 4}
 ## NOTE: do not set n_procs = 'all' unless you are running on a compute node (ie not a login node)
 ANALYSIS_CONFIGS = {"include_meta": True, "include_mag": True, "n_procs": 4}
 
 """
@@ -222,15 +222,15 @@
 
 def get_query(
     comp,
     properties=None,
     criteria=None,
     only_gs=True,
     include_structure=True,
-    supercell_structure=False,
+    supercell_structure=[2, 1, 1],
     max_Ehull=0.05,
     max_sites_per_structure=65,
     max_strucs_per_cmpd=4,
     savename="query_%s.json" % FILE_TAG,
     remake=False,
 ):
     """
@@ -313,16 +313,16 @@
             % len(StrucTools(query[mpid]["structure"]).formula)
         )
 
 
 def get_strucs(
     query,
     transform_strucs,
-    max_strucs_per_starting_struc=1,
-    ox_states=None,
+    max_strucs_per_starting_struc=2,
+    ox_states={"Ru": 4, "Ir": 4, "O": -2},
     savename="strucs_%s.json" % FILE_TAG,
     remake=False,
 ):
     """
     Args:
         query (dict) - {mpid : {DATA}}
         transform_strucs (bool or list):
@@ -371,15 +371,17 @@
             for x in transform_strucs:
                 # make a new "formula" that includes are iterator in the transformation
                 key = "_".join([formula, str(x)])
                 structools = StrucTools(
                     structure=initial_structure, ox_states=ox_states
                 )
 
-                species_mapping = None  # *NOTE*: you should customize this for your desired transformation
+                species_mapping = {
+                    "Ru": {"Ru": 1 - x / max(x), "Ir": x / (max(x))}
+                }  # *NOTE*: you should customize this for your desired transformation
 
                 # strucs will have the form {index_identifier : structure}
                 strucs = structools.replace_species(
                     species_mapping=species_mapping,
                     n_strucs=max_strucs_per_starting_struc,
                 )
 
@@ -712,14 +714,17 @@
                 print(data["structure"])
 
     print("\n\n SUMMARY: %i/%i converged" % (converged, len(keys_to_check)))
 
 
 def main():
 
+    if not os.path.exists("sub_launcher.sh"):
+        make_sub_for_launcher()
+
     remake_query = False
     print_query_check = True
 
     remake_strucs = False
     print_strucs_check = True
 
     remake_magmoms = False
```

### Comparing `pydmclab-0.0.2/pydmclab/demos/demo_vasp_test-transform-strucs.py` & `pydmclab-1.0.0/pydmclab/demos/demo_vasp_test-transform-strucs.py`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/demos/demo_vasp_test-typical-dmc.py` & `pydmclab-1.0.0/pydmclab/demos/demo_vasp_template.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,153 +4,19 @@
 
 from pydmclab.utils.handy import read_json, write_json, make_sub_for_launcher
 from pydmclab.core.query import MPQuery
 from pydmclab.core.mag import MagTools
 from pydmclab.core.struc import StrucTools
 from pydmclab.hpc.launch import LaunchTools
 from pydmclab.hpc.submit import SubmitTools
-from pydmclab.hpc.analyze import AnalyzeBatch
+from pydmclab.hpc.analyze import AnalyzeBatch, get_analysis_configs
+from pydmclab.core.energies import ChemPots, FormationEnthalpy
 
 """
-Basic framework
-
-Initial crystal structures
-    a) Sometimes these are entries in Materials Project meeting some criteria:
-        - e.g., certain chemical space, chemical formula, E above hull, etc
-    b) Other times, we might start with an MP structure then perform some transformations to generate new structures
-        - e.g., replace x % of Ru with Ir in Ru_{1-x}Ir_{x}O_2 or extract x Li from Li_{1-x}CoO_2
-            - note: now we are disordering structures, so each chemical formula will have >= 1 enumerated structure
-                - i.e., Ru_0.5Ir_0.5O_2 has > 1 way to configure Ru/Ir on the cation sublattice
-    
-    The first two levels of our caculation directories will correspond to information relating to the crystal structure:
-        - top_level: the chemical formula (or some surrogate for the chemical formula)
-            - e.g., this could be RuO2 in 1(a) or it could be x in 1(b)
-        - unique_ID: some unique identifier for a crystal structure belonging to that "top_level"
-            - e.g., the Materials Project ID for the 1(a) case; or the index of 
-        
-    Each unique initial crytsal structure will be used for all directories below top_level/unique_ID
-    
-    Example tree #1:
-    calculating RuO2 and IrO2 ground-state polymorphs
-    -calcs
-     -RuO2
-      -mp-1234
-     -IrO2
-      -mp-5678
-      
-    Example tree #2:
-    calculating Ru_{2-x}Ir_{x}O4 for x = 0, 1, 2 for 2 ordered structures at each x
-    -calcs
-     -0
-      -0
-      -1
-     -1
-      -0
-      -1
-     -2
-      -0
-      -1
-         
-VASP input settings ("standard")
-
-    Usually we want to compute a group of structures with similar settings so that we can safely compare the resulting energies
-    
-    - right now, we have two standards:
-        - dmc: our group standard (to be evolved collectively)
-            - these are best practice settings for our group
-        - mp: settings to use for strict comparison to Materials Project data
-    - standards define the non-structure VASP input files (INCAR, KPOINTS, POTCAR)
-    
-    This will be the third level of our calculation directory: top_level/unique_ID/standard
-    
-    If we were calculating with dmc and mp standards, a part of the tree might look like:
-    
-    -calcs
-     -RuO2
-      -mp-1234
-       -dmc
-       -mp
-    
-Magnetic configuration (mag)
-
-    We need to define what initial magnetic configuration we want to calculate for each initial structure
-    - nm: non-magnetic (no spins)
-    - fm: ferromagnetic (all spins > 0)
-    - afm_*: antiferromagnetic (spins up and down with sum(spins) = 0)
-        - * is a unique identifier for the ordering of spins
-            - much like partially occupied / disordered structures have multiple ways to configure ions on the lattice,
-                - there are often many ways to configure spins on the lattice while still being AFM (sum(spins) = 0)
-        - if we want to do AFM calculations, we should first generate a "MAGMOM" (AFM ordering) file for each unique structure and save that data
-        - note: if we are computing AFM, we will also compute FM
-        
-    This will be the fourth level of our calculation directory: top_level/unique_ID/standard/mag
-    
-    -calcs
-     -RuO2
-      -mp-1234
-       -dmc
-        -afm_0
-
-        
-Exchange-correlation functional (xc)
-
-Now, we need to decide what flavor of DFT we want to use. Materials Project uses GGA+U. We will often use METAGGA.
-
-For each xc that we use, it's generally a good idea to run calculations in a sequence:
-    - a "loose" calculation that has fast-converging standards but not super accurate
-    - a "relax" calculation that will optimize the crystal structure with stricter standards
-    - a "static" calculation that will give us a better energy/electronic structure at that optimized geometry
-    - for METAGGA calculations, we need to first converge a GGA calculation before we start to optimize the geometry with metagga
-    
-We don't want to have to submit each of these individually to the queue, so we will "pack" them together:
-
-    So, if we're running gga, that means three calculations will get packed together: gga-loose --> gga-relax --> gga-static
-        - if we're running metagga, we'll have 5 calcs: gga-loose --> gga-relax --> gga-static --> metagga-relax --> metagga-static
-        - each packing or chain of jobs will need a submission script (i.e., something that gets submitted to the queue)
-        
-Each one of these "xc-calcs" (e.g., gga-relax) will require a VASP execution, meaning it needs VASP inputs and will generate VASP outputs,
-    so each xc-calc gets its own directory, becoming the 5th level of our calculation directory:
-    
-    top_level/unique_ID/standard/mag/xc-calc
-    
-    -calcs
-     -RuO2
-      -mp-1234
-       -dmc
-        -afm_0
-         -gga-loose
-         -gga-relax
-         -gga-static
-
-"""
-
-"""
-Most of this is taken care of automatically in pydmc
-
-1) Use MPQuery to get crystal structures from Materials Project
-    - write to a dictionary: query.json
-2) [OPTIONAL] Transform those structures to generate new structures using StrucTools
-    - write to a dictionary: strucs.json
-3) [OPTIONAL] Create AFM orderings ("magmoms") for each structure using MagTools(structure).get_afm_magmoms
-    - write to a dictionary: magmoms.json
-4) Create a dictionary of "launch directories" using LaunchTools
-    - customizable with various _launch_configs
-    - launch directories are the directories that hold submission scripts
-        - these launch directories are defined by the top_level, unique_ID, standard, and mag
-    - this will look like: {top_level/unique_ID/standard/mag : 
-                                {'xcs' : [XCs to use for that standard],
-                                'magmom' : [magmoms to use for that structure]}
-    - write to a dictionary: launch_dirs.json
-5) Loop through the launch directories and prepare VASP inputs + submission files and launch each chain of VASP jobs using SubmitTools
-    - customizable with _sub_configs, _vasp_configs, and _slurm_configs
-    - SubmitTools will figure out which jobs can be submitted together and how to order them for submission
-    - It will also prepare each VASP job accordingly
-6) Crawl through the launch directories, and analyze every VASP calculation using AnalyzeBatch
-    - customizable with _analysis_configs
-    - write to a dictionary: results.json
+see [pydmclab docs](https://github.umn.edu/bartel-group/pydmclab/blob/main/docs.md) for help
 """
 
 # where is this file
 SCRIPTS_DIR = os.getcwd()
 
 # where are my calculations going to live
 CALCS_DIR = SCRIPTS_DIR.replace("scripts", "calcs")
@@ -166,50 +32,58 @@
 API_KEY = "N3KdATtMmcsUL94g"
 
 # lets put a tag on all the files we save
 FILE_TAG = CALCS_DIR.split("/")[-2]
 
 # what to query MP for
 ## e.g., 'MnO2', ['MnO2', 'TiO2'], 'Ca-Ti-O, etc
-COMPOSITIONS = ["Zn3MoN4", "ZnMoN2"]
+COMPOSITIONS = None
 
 # how to transform MP structures
-## e.g., [x for x in range(5)] ([0,1,2,3,4])
+## e.g., [x/8 for x in range(9)]
 ## NOTE: you need to modify get_strucs to make this work (hard to generalize)
 TRANSFORM_STRUCS = False
 
 # whether or not you want to generate MAGMOMs
 ## True if you're running AFM, else False
-GEN_MAGMOMS = True
+GEN_MAGMOMS = False
 
 # what {standard : [final_xcs]} to calculate
 ## e.g., {'dmc' : ['metagga', 'ggau']} if you want to run METAGGA + GGA+U at DMC standards
-TO_LAUNCH = {"dmc": ["metagga"]}
+TO_LAUNCH = {}
 
 # any configurations related to LaunchTools
 ## e.g., {'compare_to_mp' : True, 'n_afm_configs' : 4}
-LAUNCH_CONFIGS = {"compare_to_mp": False, "n_afm_configs": 2}
+LAUNCH_CONFIGS = {}
 
 # any configurations related to SubmitTools
 ## usually no need to change anything but n_procs... n_procs will determine how to parallelize over launch_dirs
 ## NOTE: do not set n_procs = 'all' unless you are running on a compute node (ie not a login node)
 SUB_CONFIGS = {"n_procs": 1}
 
 # any configurations related to Slurm
 ## e.g., {'ntasks' : 16, 'time' : int(24*60)}
-SLURM_CONFIGS = {"ntasks": 16, "time": int(24 * 60)}
+SLURM_CONFIGS = {}
 
 # any configurations related to VASPSetUp
 ## e.g., {'lobster_static' : True, 'relax_incar' : {'ENCUT' : 555}}
-VASP_CONFIGS = {"lobster_static": True}
+VASP_CONFIGS = {}
 
 # any configurations related to AnalyzeBatch
 ## e.g., {'include_meta' : True, 'include_mag' : True, 'n_procs' : 4}
 ## NOTE: do not set n_procs = 'all' unless you are running on a compute node (ie not a login node)
-ANALYSIS_CONFIGS = {"include_meta": True, "include_mag": True, "n_procs": 4}
+ANALYSIS_CONFIGS = get_analysis_configs(
+    n_procs=1,
+    analyze_structure=True,
+    analyze_mag=False,
+    analyze_charge=False,
+    analyze_dos=False,
+    analyze_bonding=False,
+    exclude=[],
+)
 
 """
 Don't forget to inspect the arguments to:
     get_query
     get_strucs
     get_magmoms
     get_launch_dirs
@@ -222,15 +96,15 @@
 
 def get_query(
     comp,
     properties=None,
     criteria=None,
     only_gs=True,
     include_structure=True,
-    supercell_structure=[2, 1, 1],
+    supercell_structure=False,
     max_Ehull=0.05,
     max_sites_per_structure=65,
     max_strucs_per_cmpd=4,
     savename="query_%s.json" % FILE_TAG,
     remake=False,
 ):
     """
@@ -304,25 +178,22 @@
     return read_json(fjson)
 
 
 def check_query(query):
     for mpid in query:
         print("\nmpid: %s" % mpid)
         print("\tcmpd: %s" % query[mpid]["cmpd"])
-        print(
-            "\tstructure formula: %s"
-            % len(StrucTools(query[mpid]["structure"]).formula)
-        )
+        print("\tstructure formula: %s" % StrucTools(query[mpid]["structure"]).formula)
 
 
 def get_strucs(
     query,
     transform_strucs,
-    max_strucs_per_starting_struc=2,
-    ox_states={"Ru": 4, "Ir": 4, "O": -2},
+    max_strucs_per_starting_struc=1,
+    ox_states=None,
     savename="strucs_%s.json" % FILE_TAG,
     remake=False,
 ):
     """
     Args:
         query (dict) - {mpid : {DATA}}
         transform_strucs (bool or list):
@@ -371,17 +242,15 @@
             for x in transform_strucs:
                 # make a new "formula" that includes are iterator in the transformation
                 key = "_".join([formula, str(x)])
                 structools = StrucTools(
                     structure=initial_structure, ox_states=ox_states
                 )
 
-                species_mapping = {
-                    "Ru": {"Ru": 1 - x / max(x), "Ir": x / (max(x))}
-                }  # *NOTE*: you should customize this for your desired transformation
+                species_mapping = None  # *NOTE*: you should customize this for your desired transformation
 
                 # strucs will have the form {index_identifier : structure}
                 strucs = structools.replace_species(
                     species_mapping=species_mapping,
                     n_strucs=max_strucs_per_starting_struc,
                 )
 
@@ -681,49 +550,206 @@
 
 def check_results(results):
 
     keys_to_check = list(results.keys())
 
     converged = 0
     for key in keys_to_check:
-        top_level, ID, standard, mag, xc_calc = key.split(".")
+        if "--" in key:
+            delimiter = "--"
+        else:
+            delimiter = "."
+        top_level, ID, standard, mag, xc_calc = key.split(delimiter)
         data = results[key]
         convergence = results[key]["results"]["convergence"]
         print("\n%s" % key)
         print("convergence = %s" % convergence)
         if convergence:
             converged += 1
+            print("\n%s" % key)
             print("E (static) = %.2f" % data["results"]["E_per_at"])
-            continue
-            if ANALYSIS_CONFIGS["include_meta"]:
-                print("E (relax) = %.2f" % data["meta"]["E_relax"])
-                print("EDIFFG = %i" % data["meta"]["incar"]["EDIFFG"])
-                print("1st POTCAR = %s" % data["meta"]["potcar"][0])
-            if (
-                (mag != "nm")
-                and ("include_mag" in ANALYSIS_CONFIGS)
-                and (ANALYSIS_CONFIGS["include_mag"])
-            ):
-                magnetization = data["magnetization"]
-                an_el = list(magnetization.keys())[0]
-                an_idx = list(magnetization[an_el].keys())[0]
-                that_mag = magnetization[an_el][an_idx]["mag"]
-                print("mag on %s (%s) = %.2f" % (an_el, str(an_idx), that_mag))
-            if ("include_structure" not in ANALYSIS_CONFIGS) or (
-                ANALYSIS_CONFIGS["include_structure"]
-            ):
-                print(data["structure"])
 
     print("\n\n SUMMARY: %i/%i converged" % (converged, len(keys_to_check)))
 
 
-def main():
+def get_gs(
+    results, include_structure=False, savename="gs_%s.json" % FILE_TAG, remake=False
+):
+    """
+    Args:
+        results (dict) - {'formula.ID.standard.mag.xc_calc' : {scraped results from VASP calculation}}
+        include_structure (bool) - include the structure or not
+        savename (str) - filename for fjson in DATA_DIR
+        remake (bool) - write (True) or just read (False) fjson
+
+    Returns:
+    {standard (str, the calculation standard) :
+        {xc (str, the exchange-correlation method) :
+            {formula (str) :
+                {'E' : energy of the ground-structure,
+                'key' : formula.ID.standard.mag.xc_calc for the ground-state structure,
+                'structure' : structure of the ground-state structure,
+                'n_started' : how many polymorphs you tried to calculate,
+                'n_converged' : how many polymorphs are converged,
+                'complete' : True if n_converged = n_started (i.e., all structures for this formula at this xc are done)}
+    """
+    fjson = os.path.join(DATA_DIR, savename)
+    if os.path.exists(fjson) and not remake:
+        return read_json(fjson)
+
+    standards = sorted(
+        list(set([results[key]["meta"]["setup"]["standard"] for key in results]))
+    )
+
+    gs = {
+        standard: {
+            xc: {}
+            for xc in sorted(
+                list(
+                    set(
+                        [
+                            results[key]["meta"]["setup"]["xc"]
+                            for key in results
+                            if results[key]["meta"]["setup"]["standard"] == standard
+                        ]
+                    )
+                )
+            )
+        }
+        for standard in standards
+    }
+
+    for standard in gs:
+        for xc in gs[standard]:
+            keys = [
+                k
+                for k in results
+                if results[k]["meta"]["setup"]["standard"] == standard
+                if results[k]["meta"]["setup"]["xc"] == xc
+            ]
+
+            unique_formulas = sorted(
+                list(set([results[key]["results"]["formula"] for key in keys]))
+            )
+            for formula in unique_formulas:
+                gs[standard][xc][formula] = {}
+                formula_keys = [
+                    k for k in keys if results[k]["results"]["formula"] == formula
+                ]
+                converged_keys = [
+                    k for k in formula_keys if results[k]["results"]["convergence"]
+                ]
+                if not converged_keys:
+                    gs_energy, gs_structure, gs_key = None, None, None
+                else:
+                    energies = [
+                        results[k]["results"]["E_per_at"] for k in converged_keys
+                    ]
+                    gs_energy = min(energies)
+                    gs_key = converged_keys[energies.index(gs_energy)]
+                    gs_structure = results[gs_key]["structure"]
+                complete = True if len(formula_keys) == len(converged_keys) else False
+                gs[standard][xc][formula] = {
+                    "E": gs_energy,
+                    "key": gs_key,
+                    "n_started": len(formula_keys),
+                    "n_converged": len(converged_keys),
+                    "complete": complete,
+                }
+                if include_structure:
+                    gs[standard][xc][formula]["structure"] = gs_structure
+
+    write_json(gs, fjson)
+    return read_json(fjson)
+
+
+def check_gs(gs):
+    """
+    checks that this dictionary is generated properly
 
-    if not os.path.exists("sub_launcher.sh"):
-        make_sub_for_launcher()
+    Args:
+        gs (_type_): _description_
+
+    """
+
+    print("\nchecking ground-states")
+    standards = gs.keys()
+    print("standards = ", standards)
+    for standard in standards:
+        print("\nworking on %s standard" % standard)
+        xcs = list(gs[standard].keys())
+        for xc in xcs:
+            print("  xc = %s" % xc)
+            formulas = list(gs[standard][xc].keys())
+            n_formulas = len(formulas)
+            n_formulas_complete = len(
+                [k for k in formulas if gs[standard][xc][k]["complete"]]
+            )
+            print(
+                "%i/%i formulas with all calculations completed"
+                % (n_formulas_complete, n_formulas)
+            )
+
+
+def get_Efs(
+    gs, non_default_functional=None, savename="Efs_%s.json" % FILE_TAG, remake=False
+):
+    """
+    Args:
+        gs (dict) - {formula (str) : {basic stuff for ground-states}}
+        non_default_functional (str or None) - if None, use default functionals
+        savename (str) - filename for fjson in DATA_DIR
+        remake (bool) - write (True) or just read (False) fjson
+
+    Returns:
+    {xc (str, the exchange-correlation method) :}
+        {formula (str) :
+            {'E' : energy of the ground-structure,
+             'key' : formula.ID.standard.mag.xc_calc for the ground-state structure,
+             'structure' : structure of the ground-state structure,
+             'n_started' : how many polymorphs you tried to calculate,
+             'n_converged' : how many polymorphs are converged,
+             'complete' : True if n_converged = n_started (i.e., all structures for this formula at this xc are done),
+             'Ef' : formation enthalpy at 0 K (float)}
+    """
+    fjson = os.path.join(DATA_DIR, savename)
+    if os.path.exists(fjson) and not remake:
+        return read_json(fjson)
+    for standard in gs:
+        for xc in gs[standard]:
+            if not non_default_functional:
+                functional = "r2scan" if xc == "metagga" else "pbe"
+            else:
+                functional = non_default_functional
+            mus = ChemPots(functional=functional, standard=standard).chempots
+            for formula in gs[standard][xc]:
+                E = gs[standard][xc][formula]["E"]
+                if E:
+                    Ef = FormationEnthalpy(formula=formula, E_DFT=E, chempots=mus).Ef
+                else:
+                    Ef = None
+                gs[standard][xc][formula]["Ef"] = Ef
+
+    write_json(gs, fjson)
+    return read_json(fjson)
+
+
+def check_Efs(Efs):
+    print("\nchecking formation enthalpies")
+
+    for standard in Efs:
+        print("\n\nworking on %s standard" % standard)
+        for xc in Efs[standard]:
+            print("\nxc = %s" % xc)
+            for formula in Efs[standard][xc]:
+                print("%s : %s eV/at" % (formula, Efs[standard][xc][formula]["Ef"]))
+    return
+
+
+def main():
 
     remake_query = False
     print_query_check = True
 
     remake_strucs = False
     print_strucs_check = True
 
@@ -735,14 +761,20 @@
 
     remake_subs = True
     ready_to_launch = True
 
     remake_results = True
     print_results_check = True
 
+    remake_gs = True
+    print_gs_check = True
+
+    remake_Efs = True
+    print_Efs_check = True
+
     comp = COMPOSITIONS
     query = get_query(comp=comp, remake=remake_query)
     if print_query_check:
         check_query(query)
 
     transform_strucs = TRANSFORM_STRUCS
     strucs = get_strucs(
@@ -785,12 +817,22 @@
     analysis_configs = ANALYSIS_CONFIGS
     results = get_results(
         launch_dirs=launch_dirs, user_configs=analysis_configs, remake=remake_results
     )
     if print_results_check:
         check_results(results)
 
+    gs = get_gs(results=results, remake=remake_gs)
+
+    if print_gs_check:
+        check_gs(gs)
+
+    Efs = get_Efs(gs=gs, remake=remake_Efs)
+
+    if print_Efs_check:
+        check_Efs(Efs)
+
     return
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pydmclab-0.0.2/pydmclab/demos/tmp.png` & `pydmclab-1.0.0/pydmclab/demos/tmp.png`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/dev/entries.py` & `pydmclab-1.0.0/pydmclab/dev/entries.py`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/dev/reactions.py` & `pydmclab-1.0.0/pydmclab/dev/reactions.py`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/hpc/README.md` & `pydmclab-1.0.0/pydmclab/hpc/README.md`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/hpc/analyze.py` & `pydmclab-1.0.0/pydmclab/hpc/analyze.py`

 * *Files 3% similar despite different names*

```diff
@@ -1203,15 +1203,15 @@
         Args:
             calc_dir (str) : path to a calculation directory where VASP was executed
 
         Returns:
             a string that can be used as a key for a dictionary
                 top_level.unique_ID.standard.mag.xc_calc
         """
-        return ".".join(calc_dir.split("/")[-5:])
+        return "--".join(calc_dir.split("/")[-5:])
 
     def _results_for_calc_dir(self, calc_dir):
         """
         Args:
             calc_dir (str) : path to a calculation directory where VASP was executed
 
         Returns:
@@ -1362,7 +1362,76 @@
             % (len(purged_files), mem_created / 1e9)
         )
     if safety == "on":
         print(
             "You had the safety on\n If it were off, you would have purged %i files, freeing up %.2f GB of memory"
             % (len(purged_files), mem_created / 1e9)
         )
+
+def get_analysis_configs(
+    analyze_calculations_in_parallel=False,
+    analyze_structure=True,
+    analyze_mag=False,
+    analyze_charge=False,
+    analyze_dos=False,
+    analyze_bonding=False,
+    exclude=[],
+):
+    """
+
+    function for modifying analysis configs from the defaults (see *** for defaults)
+
+    Args:
+        analyze_calculations_in_parallel (bool or int): whether to analyze calculation results in parallel or not
+            False: use 1 processor
+            True: use all available processors
+            int: use that many processors
+        analyze_structure (bool, optional): True to include structure in your results
+        analyze_mag (bool, optional): True to include magnetization in your results
+        analyze_charge (bool, optional): True to include bader charge + lobster charges + madelung in your results
+        analyze_dos (bool, optional): True to include pdos, tdos in your results
+        analyze_bonding (bool, optional): True to include tcohp, pcohp, tcoop, pcoop, tcobi, pcobi in your results
+        exclude (list, optional): list of strings to exclude from analysis. Defaults to [].
+            - overwrites other options
+    Returns:
+        dictionary of ANALYSIS_CONFIGS
+            {'include_*' : True or False}
+    """
+
+    analysis_configs = {}
+
+    if not analyze_calculations_in_parallel:
+        n_procs = 1
+    else:
+        if analyze_calculations_in_parallel == True:
+            n_procs = multip.cpu_count() - 1
+        elif analyze_calculations_in_paralle == False:
+            n_procs = 1
+        else:
+            n_procs = analyze_calculations_in_parallel
+
+    analysis_configs["n_procs"] = n_procs
+
+    includes = []
+    if analyze_structure:
+        includes.append("structure")
+
+    if analyze_mag:
+        includes.append("mag")
+
+    if analyze_charge:
+        includes.extend(["charge", "madelung"])
+
+    if analyze_dos:
+        includes.extend(["tdos", "pdos"])
+
+    if analyze_bonding:
+        includes.extend(["tcohp", "pcohp", "tcoop", "pcoop", "tcobi", "pcobi"])
+
+    for include in includes:
+        analysis_configs["include_" + include] = True
+
+    if exclude:
+        for ex in exclude:
+            analysis_configs["include_" + ex] = False
+
+    return analysis_configs
```

### Comparing `pydmclab-0.0.2/pydmclab/hpc/launch.py` & `pydmclab-1.0.0/pydmclab/hpc/launch.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
     def __init__(
         self,
         calcs_dir,
         structure,
         top_level,
         unique_ID,
-        to_launch,
         magmoms=None,
         user_configs={},
         refresh_configs=True,
         launch_configs_yaml=os.path.join(os.getcwd(), "_launch_configs.yaml"),
     ):
         """
         Args:
@@ -57,32 +56,30 @@
                         - I might make top_level = LiCoO2
 
             unique_ID (str): level below top_level
                 - could be a material ID in materials project (for standard geometry relaxations, this makes sense)
                 - could be x in the LiCoO2 example I described previously
                 - it's really up to you, but it must be unique within the top_level directory
 
-            to_launch (dict) :
-                {standard (str) : [list of xcs (str)]}
-                - e.g., if I want to run gga+u and metagga with dmc standards, to_launch = {'dmc' : ['metagga', 'ggau']}
-
             magmoms (dict):
                 - if you are running AFM calculations
                     - {index of configuration index (int) : magmom (list)} generated using MagTools
                     - best practice is to save this as a json in data_dir so you only call MagTools once
                 - if you are not running AFM calculations
                     - can be None or {}
 
             user_configs (dict):
                 - any setting you want to pass that's not default in pydmc/data/data/_launch_configs.yaml
                 - launch_configs:
                     compare_to_mp: False # if True, launch will get everything it needs to generate MP-consistent data
                     n_afm_configs: 0 # how many AFM configurations to run
                     override_mag: False # could be ['nm'] if you only want to run nonmagnetic, won't check for whether structure is mag or not mag, it will just do as you say
-
+                    to_launch:
+                        - what xcs we want to launch for each standard
+                            - e.g., {'dmc' : ['metagga']}
 
             refresh_configs (bool) - if True, will copy pydmc baseline configs to your local directory
                 - this is useful if you've made changes to the configs files in the directory you're working in and want to start over
 
             launch_configs_yaml (os.pathLike) - path to yaml file containing launch configs
                 - there's usually no reason to change this
                 - this holds some default configs for LaunchTools
@@ -115,23 +112,18 @@
         if configs["n_afm_configs"] > 0:
             if MagTools(structure).could_be_afm:
                 if not magmoms:
                     raise ValueError(
                         "You are running afm calculations but provided no magmoms, generate these first, then pass to LaunchTools"
                     )
 
-        # include gga+u calcs w/ mp standards if we're comparing to MP
-        if configs["compare_to_mp"]:
-            to_launch["mp"] = ["ggau"]
-
         # add the required arguments to our configs file
         configs["top_level"] = top_level
         configs["unique_ID"] = unique_ID
         configs["calcs_dir"] = calcs_dir
-        configs["to_launch"] = to_launch
 
         # store our magmoms and structure
         self.magmoms = magmoms
         self.structure = structure
 
         # make a copy of our configs to prevent unwanted changes
         self.configs = configs.copy()
@@ -272,7 +264,55 @@
                                 perturbation
                             )
                             perturbed_structure.to(fmt="poscar", filename=fposcar)
                         else:
                             struc.to(fmt="poscar", filename=fposcar)
 
         return launch_dirs
+
+
+def get_launch_configs(
+    standards=["dmc"],
+    xcs=["metagga"],
+    use_mp_thermo_data=False,
+    n_afm_configs=0,
+    skip_xcs_for_standards={"mp": ["gga", "metagga"]},
+):
+    """
+
+    configs related to launching  chains of calculations
+
+    Args:
+        standards (list, optional): list of standards you'd like to calculate
+        xcs (list, optional): list of xcs you'd like to calculate for each standard
+        use_mp_thermo_data (bool, optional): True if you are going to use formation energies provided in Materials Project for phase stability analysis
+        n_afm_configs (int, optional): number of antiferromagnetic configurations to run for each structure (0 if you don't want to run AFM)
+        skip_xcs_for_standards (dict, optional): dictionary of xcs to skip for a given standard.
+            Defaults to {"mp": ["gga", "metagga"]}.
+                - e.g., we don't want to run GGA or MetaGGA MP calculations because MP uses GGA+U (for now)
+
+    Returns:
+        dictionary of launch configurations
+    """
+
+    launch_configs = {}
+
+    to_launch = {}
+
+    for standard in standards:
+        to_launch[standard] = xcs
+
+    if use_mp_thermo_data:
+        to_launch["mp"] = ["ggau"]
+
+    for standard in skip_xcs_for_standards:
+        for xc in skip_xcs_for_standards[standard]:
+            if xc in to_launch[standard]:
+                to_launch[standard].remove(xc)
+
+    launch_configs["to_launch"] = to_launch
+
+    launch_configs["compare_to_mp"] = use_mp_thermo_data
+
+    launch_configs["n_afm_configs"] = n_afm_configs
+
+    return launch_configs
```

### Comparing `pydmclab-0.0.2/pydmclab/hpc/submit.py` & `pydmclab-1.0.0/pydmclab/hpc/submit.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     load_slurm_configs,
     load_sub_configs,
     load_partition_configs,
 )
 
 from pymatgen.core.structure import Structure
 
+import multiprocessing as multip
 import os
 from shutil import copyfile, rmtree
 import subprocess
 import warnings
 
 HERE = os.path.dirname(os.path.abspath(__file__))
 
@@ -279,27 +280,28 @@
         """
         Returns command used to execute vasp
             e.g., 'srun -n 24 PATH_TO_VASP/vasp_std > vasp.o'
         """
         sub_configs = self.sub_configs.copy()
         vasp_configs = self.vasp_configs.copy()
         vasp_exec = os.path.join(sub_configs["vasp_dir"], sub_configs["vasp"])
-        if sub_configs['mpi_command'] == 'srun':
+        if sub_configs["mpi_command"] == "srun":
             return "\n%s --ntasks=%s --mpi=pmi2 %s > %s\n" % (
                 sub_configs["mpi_command"],
                 str(self.slurm_options["ntasks"]),
                 vasp_exec,
-                vasp_configs["fvaspout"]
+                vasp_configs["fvaspout"],
             )
-        elif sub_configs['mpi_command'] == 'mpirun':
-            return '\n%s -np=%s %s > %s\n' % (
-                sub_configs['mpi_command'],
-                str(self.slurm_options['ntasks']),
+        elif sub_configs["mpi_command"] == "mpirun":
+            return "\n%s -np=%s %s > %s\n" % (
+                sub_configs["mpi_command"],
+                str(self.slurm_options["ntasks"]),
                 vasp_exec,
-                vasp_configs['fvaspout'])
+                vasp_configs["fvaspout"],
+            )
 
     @property
     def lobster_command(self):
         """
         Returns command used to execute lobster
         """
         lobster = "/home/cbartel/shared/bin/lobster/lobster-4.1.0/lobster-4.1.0"
@@ -620,16 +622,16 @@
                     slurm_option = slurm_options[key]
                     if slurm_option:
                         f.write(
                             "%s --%s=%s\n" % (queue_manager, key, str(slurm_option))
                         )
                 f.write("\n\n")
                 f.write("ulimit -s unlimited\n")
-                if sub_configs['mpi_command'] == 'mpirun':
-                    f.write('module load impi/2018/release_multithread\n')
+                if sub_configs["mpi_command"] == "mpirun":
+                    f.write("module load impi/2018/release_multithread\n")
                 # now write what is needed for the chain of VASP calcs + postprocessing
                 print("\n:::: writing sub now - %s ::::" % fsub)
 
                 # use this counter to figure if there are parents for a given calc and who those parents are
                 xc_calc_counter = -1
                 for xc_calc in packing[final_xc]:
                     # loop through the calculations that should be chained together for a given final_xc
@@ -774,14 +776,207 @@
 
             # if we made it this far, launch it
             os.chdir(launch_dir)
             subprocess.call(["sbatch", "sub_%s.sh" % final_xc])
             os.chdir(scripts_dir)
 
 
+def get_sub_configs(
+    submit_calculations_in_parallel=False,
+    start_all_calculations_from_scratch=False,
+    rerun_lobster=False,
+    mpi_command="mpirun",
+    special_packing=False,
+):
+    """
+
+    configs related to preparing submission scripts and submitting VASP calculations
+        - see defaults in ***
+
+
+    Args:
+        submit_calculations_in_parallel (bool or int): whether to prepare submission scripts in parallel or not
+            False: use 1 processor
+            True: use all available processors
+            int: use that many processors
+
+        start_all_calculations_from_scratch (bool): if True, start all calculations over (ie delete all outputs)
+
+        rerun_lobster (bool) : if True, rerun lobster even if it has already been run
+
+        mpi_command (str): the command to use for mpi (eg mpirun, srun, etc)
+
+        special_packing (dict): if you want to change the loose --> relax --> static flow for some functional
+            e.g., {'metagga' : ['loose', 'static']}
+
+    Returns:
+        {config_name : config_value}
+
+    """
+    sub_configs = {}
+
+    if not submit_calculations_in_parallel:
+        n_procs = 1
+    else:
+        if submit_calculations_in_parallel == True:
+            n_procs = multip.cpu_count() - 1
+        elif submit_calculations_in_parallel == False:
+            n_procs = 1
+        else:
+            n_procs = submit_calculations_in_parallel
+
+    sub_configs["n_procs"] = n_procs
+
+    if start_all_calculations_from_scratch:
+        sub_configs["fresh_restart"] = True
+
+    if rerun_lobster:
+        sub_configs["force_postprocess"] = True
+
+    sub_configs["mpi_command"] = mpi_command
+
+    if special_packing:
+        sub_configs["packing"] = {}
+        for xc in special_packing:
+            sub_configs["packing"]["xc"] = special_packing[xc]
+
+    return sub_configs
+
+
+def get_slurm_configs(
+    total_nodes=1,
+    cores_per_node=32,
+    walltime_in_hours=23,
+    partition="msismall",
+    error_file="log.e",
+    output_file="log.o",
+    account="cbartel",
+):
+    """
+
+    how to modify slurm configurations for each VASP job (see *** for defaults)
+
+    Args:
+        total_nodes (int, optional): how many nodes to run each VASP job on
+        cores_per_node (int, optional): how many cores per node to use for each VASP job
+        walltime_in_hours (int, optional): how long to run each VASP job
+        partition (str, optional): what part of the cluster to run each VASP job on
+        error_file (str, optional): where to send each VASP job error
+        output_file (str, optional): where to send each VASP job output
+        account (str, optional): what account to charge for your VASP jobs
+
+    Returns:
+        {slurm config name : slurm config value}
+    """
+    slurm_configs = {}
+
+    slurm_configs["nodes"] = total_nodes
+    slurm_configs["ntasks"] = int(total_nodes * cores_per_node)
+
+    slurm_configs["time"] = int(walltime_in_hours * 60)
+
+    if total_nodes > 1:
+        if "small" in partition:
+            print("WARNING: cant use small partition on > 1 node; switching to large")
+        partition = partition.replace("small", "large")
+        slurm_configs["partition"] = partition
+
+    slurm_configs["error_file"] = error_file
+    slurm_configs["output_file"] = output_file
+    slurm_configs["account"] = account
+
+    if total_nodes > 4:
+        print("WARNING: are you sure you need more than 4 nodes??")
+
+    if (total_nodes > 1) and (cores_per_node < 32):
+        print("WARNING: this seems like a small job. are you sure you need > 1 node??")
+
+    return slurm_configs
+
+
+def get_vasp_configs(
+    run_lobster=False,
+    modify_loose_incar=False,
+    modify_relax_incar=False,
+    modify_static_incar=False,
+    modify_loose_kpoints=False,
+    modify_relax_kpoints=False,
+    modify_static_kpoints=False,
+    modify_loose_potcar=False,
+    modify_relax_potcar=False,
+    modify_static_potcar=False,
+):
+    """
+
+    how to modify VASP calculations from the defaults (see pydmclab.hpc.vasp for defaults)
+
+    Args:
+        run_lobster (bool, optional): True to run LOBSTER
+
+        modify_loose_incar (bool, optional):
+            - dictionary of {incar flag (str) : setting for that flag}
+            - modifies only the "loose" calculations
+        modify_relax_incar (bool, optional):
+            - dictionary of {incar flag (str) : setting for that flag}
+            - modifies only the "relax" calculations
+        modify_static_incar (bool, optional):
+            - dictionary of {incar flag (str) : setting for that flag}
+            - modifies only the "static" calculations
+
+
+        modify_loose_kpoints (bool, optional):
+            - dictionary of non-default K-point setting. see pydmclab.hpc.vasp for format
+            - modifies only the "loose" calculations
+        modify_relax_kpoints (bool, optional):
+            - dictionary of non-default K-point setting. see pydmclab.hpc.vasp for format
+            - modifies only the "relax" calculations
+        modify_static_kpoints (bool, optional):
+            - dictionary of non-default K-point setting. see pydmclab.hpc.vasp for format
+            - modifies only the "static" calculations
+
+
+        modify_loose_potcar (bool, optional):
+            - dictionary of non-default POTCAR in format {element (str) : POTCAR to use (str)}
+            - modifies only the "loose" calculations
+        modify_relax_potcar (bool, optional):
+            - dictionary of non-default POTCAR in format {element (str) : POTCAR to use (str)}
+            - modifies only the "loose" calculations
+        modify_static_potcar (bool, optional):
+            - dictionary of non-default POTCAR in format {element (str) : POTCAR to use (str)}
+            - modifies only the "static" calculations
+
+    Returns:
+        dictionary of VASP_CONFIGS
+    """
+    vasp_configs = {"lobster_static": run_lobster}
+
+    if modify_loose_incar:
+        vasp_configs["loose_incar"] = modify_loose_incar
+    if modify_relax_incar:
+        vasp_configs["relax_incar"] = modify_relax_incar
+    if modify_static_incar:
+        vasp_configs["static_incar"] = modify_static_incar
+
+    if modify_loose_kpoints:
+        vasp_configs["loose_kpoints"] = modify_loose_kpoints
+    if modify_relax_kpoints:
+        vasp_configs["relax_kpoints"] = modify_relax_kpoints
+    if modify_static_kpoints:
+        vasp_configs["static_kpoints"] = modify_static_kpoints
+
+    if modify_loose_potcar:
+        vasp_configs["loose_potcar"] = modify_loose_potcar
+    if modify_relax_potcar:
+        vasp_configs["relax_potcar"] = modify_relax_potcar
+    if modify_static_potcar:
+        vasp_configs["static_potcar"] = modify_static_potcar
+
+    return vasp_configs
+
+
 def main():
 
     return
 
 
 if __name__ == "__main__":
     sub = main()
```

### Comparing `pydmclab-0.0.2/pydmclab/hpc/vasp.py` & `pydmclab-1.0.0/pydmclab/hpc/vasp.py`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/utils/handy.py` & `pydmclab-1.0.0/pydmclab/utils/handy.py`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab/utils/plotting.py` & `pydmclab-1.0.0/pydmclab/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `pydmclab-0.0.2/pydmclab.egg-info/PKG-INFO` & `pydmclab-1.0.0/pydmclab.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydmclab
-Version: 0.0.2
+Version: 1.0.0
 Summary: Package to facilitate DFT calculations and analysis
 Home-page: https://github.umn.edu/bartel-group/pydmclab
 Author: Chris Bartel
 Author-email: cbartel@umn.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,7 +13,9 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # pydmclab
 
 - common framework to rely upon for typical calculations and analysis done in the Bartel research group
+
+- documentation details can be found [here](docs.md)
```

### Comparing `pydmclab-0.0.2/pydmclab.egg-info/SOURCES.txt` & `pydmclab-1.0.0/pydmclab.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -38,23 +38,26 @@
 pydmclab/data/data/mus_from_bartel2019_npj.json
 pydmclab/data/data/mus_from_dmc_no_corrections.json
 pydmclab/data/data/mus_from_mp_no_corrections.json
 pydmclab/data/data/ssub.dat
 pydmclab/data/data/ssub.json
 pydmclab/demos/demo_comp.py
 pydmclab/demos/demo_hulls.py
+pydmclab/demos/demo_launcher_template.py
 pydmclab/demos/demo_query.py
 pydmclab/demos/demo_struc.py
 pydmclab/demos/demo_vasp_template.py
 pydmclab/demos/demo_vasp_test-mp-chemsys.py
 pydmclab/demos/demo_vasp_test-template.py
 pydmclab/demos/demo_vasp_test-transform-strucs.py
 pydmclab/demos/demo_vasp_test-typical-dmc.py
 pydmclab/demos/tmp.png
+pydmclab/dev/Untitled-2.py
 pydmclab/dev/__init__.py
+pydmclab/dev/echem.py
 pydmclab/dev/entries.py
 pydmclab/dev/grand.py
 pydmclab/dev/reactions.py
 pydmclab/hpc/README.md
 pydmclab/hpc/__init__.py
 pydmclab/hpc/analyze.py
 pydmclab/hpc/launch.py
```

### Comparing `pydmclab-0.0.2/setup.py` & `pydmclab-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 NAME = "pydmclab"
 DESCRIPTION = "Package to facilitate DFT calculations and analysis"
 URL = "https://github.umn.edu/bartel-group/pydmclab"
 EMAIL = "cbartel@umn.edu"
 AUTHOR = "Chris Bartel"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.2"
+VERSION = "1.0.0"
 
 REQUIRED = ["numpy", "pymatgen"]
 EXTRAS = {}
 here = os.path.abspath(os.path.dirname(__file__))
 try:
     with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
         long_description = "\n" + f.read()
```


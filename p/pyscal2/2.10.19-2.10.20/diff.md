# Comparing `tmp/pyscal2-2.10.19.tar.gz` & `tmp/pyscal2-2.10.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscal2-2.10.19.tar", last modified: Fri Apr 28 11:52:55 2023, max compression
+gzip compressed data, was "pyscal2-2.10.20.tar", last modified: Fri Apr 28 23:06:38 2023, max compression
```

## Comparing `pyscal2-2.10.19.tar` & `pyscal2-2.10.20.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:52:55.473199 pyscal2-2.10.19/
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-28 11:52:52.000000 pyscal2-2.10.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-28 11:52:55.473199 pyscal2-2.10.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-28 11:52:52.000000 pyscal2-2.10.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:52:55.465198 pyscal2-2.10.19/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:52:55.469199 pyscal2-2.10.19/lib/voro++/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-28 11:52:52.000000 pyscal2-2.10.19/lib/voro++/voro++.cc
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 11:52:52.000000 pyscal2-2.10.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 11:52:55.473199 pyscal2-2.10.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-28 11:52:52.000000 pyscal2-2.10.19/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:52:55.465198 pyscal2-2.10.19/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:52:55.469199 pyscal2-2.10.19/src/pyscal/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 11:52:52.000000 pyscal2-2.10.19/src/pyscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-04-28 11:52:52.000000 pyscal2-2.10.19/src/pyscal/atom.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18161 2023-04-28 11:52:52.000000 pyscal2-2.10.19/src/pyscal/atom_binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    78087 2023-04-28 11:52:52.000000 pyscal2-2.10.19/src/pyscal/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-04-28 11:52:52.000000 pyscal2-2.10.19/src/pyscal/crystal_structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:52:55.469199 pyscal2-2.10.19/src/pyscal/formats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:52:52.000000 pyscal2-2.10.19/src/pyscal/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-28 11:52:52.000000 pyscal2-2.10.19/src/pyscal/formats/ase.py
--rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-04-28 11:52:52.000000 pyscal2-2.10.19/src/pyscal/formats/lammps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-28 11:52:52.000000 pyscal2-2.10.19/src/pyscal/formats/mdtraj.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-28 11:52:52.000000 pyscal2-2.10.19/src/pyscal/formats/vasp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-28 11:52:52.000000 pyscal2-2.10.19/src/pyscal/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-28 11:52:52.000000 pyscal2-2.10.19/src/pyscal/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    77453 2023-04-28 11:52:52.000000 pyscal2-2.10.19/src/pyscal/system.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-04-28 11:52:52.000000 pyscal2-2.10.19/src/pyscal/system_binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-28 11:52:52.000000 pyscal2-2.10.19/src/pyscal/traj_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-04-28 11:52:52.000000 pyscal2-2.10.19/src/pyscal/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-28 11:52:52.000000 pyscal2-2.10.19/src/pyscal/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:52:55.469199 pyscal2-2.10.19/src/pyscal2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-28 11:52:55.000000 pyscal2-2.10.19/src/pyscal2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-28 11:52:55.000000 pyscal2-2.10.19/src/pyscal2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:52:55.000000 pyscal2-2.10.19/src/pyscal2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:52:55.000000 pyscal2-2.10.19/src/pyscal2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 11:52:55.000000 pyscal2-2.10.19/src/pyscal2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 11:52:55.000000 pyscal2-2.10.19/src/pyscal2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:52:55.473199 pyscal2-2.10.19/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_angular.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_basic_atom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_basic_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_basic_triclinic.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_centrosymmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_chiparams.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_cna.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_crystal_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_cubic_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_disorder.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_formats_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_nucsize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_q10.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_q11.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_q12.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_q2.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_q3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_q4.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_q5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_q6.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_q7.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_q8.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_q9.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_q_atom.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_q_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_qlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_sro.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_traj_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-28 11:52:52.000000 pyscal2-2.10.19/tests/test_voronoi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:06:38.975723 pyscal2-2.10.20/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-28 23:06:35.000000 pyscal2-2.10.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 23:06:35.000000 pyscal2-2.10.20/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-28 23:06:38.975723 pyscal2-2.10.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-28 23:06:35.000000 pyscal2-2.10.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:06:38.963722 pyscal2-2.10.20/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:06:38.967722 pyscal2-2.10.20/lib/voro++/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-28 23:06:35.000000 pyscal2-2.10.20/lib/voro++/voro++.cc
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 23:06:35.000000 pyscal2-2.10.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:06:38.975723 pyscal2-2.10.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-28 23:06:35.000000 pyscal2-2.10.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:06:38.967722 pyscal2-2.10.20/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:06:38.967722 pyscal2-2.10.20/src/pyscal/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 23:06:35.000000 pyscal2-2.10.20/src/pyscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-04-28 23:06:35.000000 pyscal2-2.10.20/src/pyscal/atom.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18161 2023-04-28 23:06:35.000000 pyscal2-2.10.20/src/pyscal/atom_binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    78087 2023-04-28 23:06:35.000000 pyscal2-2.10.20/src/pyscal/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-04-28 23:06:35.000000 pyscal2-2.10.20/src/pyscal/crystal_structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:06:38.967722 pyscal2-2.10.20/src/pyscal/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 23:06:35.000000 pyscal2-2.10.20/src/pyscal/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-28 23:06:35.000000 pyscal2-2.10.20/src/pyscal/formats/ase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-04-28 23:06:35.000000 pyscal2-2.10.20/src/pyscal/formats/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-28 23:06:35.000000 pyscal2-2.10.20/src/pyscal/formats/mdtraj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-28 23:06:35.000000 pyscal2-2.10.20/src/pyscal/formats/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-28 23:06:35.000000 pyscal2-2.10.20/src/pyscal/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-28 23:06:35.000000 pyscal2-2.10.20/src/pyscal/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77453 2023-04-28 23:06:35.000000 pyscal2-2.10.20/src/pyscal/system.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-04-28 23:06:35.000000 pyscal2-2.10.20/src/pyscal/system_binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-28 23:06:35.000000 pyscal2-2.10.20/src/pyscal/traj_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-04-28 23:06:35.000000 pyscal2-2.10.20/src/pyscal/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-28 23:06:35.000000 pyscal2-2.10.20/src/pyscal/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:06:38.971722 pyscal2-2.10.20/src/pyscal2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-28 23:06:38.000000 pyscal2-2.10.20/src/pyscal2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-28 23:06:38.000000 pyscal2-2.10.20/src/pyscal2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:06:38.000000 pyscal2-2.10.20/src/pyscal2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:06:38.000000 pyscal2-2.10.20/src/pyscal2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 23:06:38.000000 pyscal2-2.10.20/src/pyscal2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 23:06:38.000000 pyscal2-2.10.20/src/pyscal2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:06:38.975723 pyscal2-2.10.20/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_angular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_basic_atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_basic_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_basic_triclinic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_centrosymmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_chiparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_cna.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_crystal_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_cubic_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_disorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_formats_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_nucsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_q10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_q11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_q12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_q2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_q3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_q4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_q5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_q6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_q7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_q8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_q9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_q_atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_q_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_qlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_sro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_traj_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-28 23:06:35.000000 pyscal2-2.10.20/tests/test_voronoi.py
```

### Comparing `pyscal2-2.10.19/LICENSE` & `pyscal2-2.10.20/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/setup.py` & `pyscal2-2.10.20/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='pyscal2',
-    version='2.10.19',
+    version='2.10.20',
     author='Sarath Menon',
     author_email='sarath.menon@pyscal.org',
     description='Python library written in C++ for calculation of local atomic structural environment',
     long_description=readme,
     long_description_content_type="text/markdown",
     # tell setuptools to look for any packages under 'src'
     packages=find_packages('src'),
```

### Comparing `pyscal2-2.10.19/src/pyscal/atom.cpp` & `pyscal2-2.10.20/src/pyscal/atom.cpp`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/src/pyscal/atom_binding.cpp` & `pyscal2-2.10.20/src/pyscal/atom_binding.cpp`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/src/pyscal/core.py` & `pyscal2-2.10.20/src/pyscal/core.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/src/pyscal/crystal_structures.py` & `pyscal2-2.10.20/src/pyscal/crystal_structures.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/src/pyscal/formats/ase.py` & `pyscal2-2.10.20/src/pyscal/formats/ase.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/src/pyscal/formats/lammps.py` & `pyscal2-2.10.20/src/pyscal/formats/lammps.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/src/pyscal/formats/mdtraj.py` & `pyscal2-2.10.20/src/pyscal/formats/mdtraj.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/src/pyscal/formats/vasp.py` & `pyscal2-2.10.20/src/pyscal/formats/vasp.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/src/pyscal/misc.py` & `pyscal2-2.10.20/src/pyscal/misc.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/src/pyscal/routines.py` & `pyscal2-2.10.20/src/pyscal/routines.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/src/pyscal/system.cpp` & `pyscal2-2.10.20/src/pyscal/system.cpp`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/src/pyscal/system_binding.cpp` & `pyscal2-2.10.20/src/pyscal/system_binding.cpp`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/src/pyscal/traj_process.py` & `pyscal2-2.10.20/src/pyscal/traj_process.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/src/pyscal/trajectory.py` & `pyscal2-2.10.20/src/pyscal/trajectory.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/src/pyscal/visualization.py` & `pyscal2-2.10.20/src/pyscal/visualization.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/src/pyscal2.egg-info/SOURCES.txt` & `pyscal2-2.10.20/src/pyscal2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 lib/voro++/voro++.cc
 src/pyscal/__init__.py
 src/pyscal/atom.cpp
 src/pyscal/atom_binding.cpp
```

### Comparing `pyscal2-2.10.19/tests/test_adaptive.py` & `pyscal2-2.10.20/tests/test_adaptive.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_basic_atom.py` & `pyscal2-2.10.20/tests/test_basic_atom.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_basic_system.py` & `pyscal2-2.10.20/tests/test_basic_system.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_basic_triclinic.py` & `pyscal2-2.10.20/tests/test_basic_triclinic.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_centrosymmetry.py` & `pyscal2-2.10.20/tests/test_centrosymmetry.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_chiparams.py` & `pyscal2-2.10.20/tests/test_chiparams.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_cna.py` & `pyscal2-2.10.20/tests/test_cna.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_disorder.py` & `pyscal2-2.10.20/tests/test_disorder.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_entropy.py` & `pyscal2-2.10.20/tests/test_entropy.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_file.py` & `pyscal2-2.10.20/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_formats_system.py` & `pyscal2-2.10.20/tests/test_formats_system.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_neighbors.py` & `pyscal2-2.10.20/tests/test_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_nucsize.py` & `pyscal2-2.10.20/tests/test_nucsize.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_q10.py` & `pyscal2-2.10.20/tests/test_q10.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_q12.py` & `pyscal2-2.10.20/tests/test_q12.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_q2.py` & `pyscal2-2.10.20/tests/test_q2.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_q4.py` & `pyscal2-2.10.20/tests/test_q4.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_q6.py` & `pyscal2-2.10.20/tests/test_q6.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_q8.py` & `pyscal2-2.10.20/tests/test_q8.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_q_atom.py` & `pyscal2-2.10.20/tests/test_q_atom.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_q_system.py` & `pyscal2-2.10.20/tests/test_q_system.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_qlist.py` & `pyscal2-2.10.20/tests/test_qlist.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_rdf.py` & `pyscal2-2.10.20/tests/test_rdf.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_sro.py` & `pyscal2-2.10.20/tests/test_sro.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_traj_process.py` & `pyscal2-2.10.20/tests/test_traj_process.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_trajectory.py` & `pyscal2-2.10.20/tests/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `pyscal2-2.10.19/tests/test_volume.py` & `pyscal2-2.10.20/tests/test_volume.py`

 * *Files identical despite different names*


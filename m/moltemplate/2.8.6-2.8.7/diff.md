# Comparing `tmp/moltemplate-2.8.6.tar.gz` & `tmp/moltemplate-2.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/moltemplate-2.8.6.tar", last modified: Thu Jun 28 05:18:36 2018, max compression
+gzip compressed data, was "dist/moltemplate-2.8.7.tar", last modified: Fri Jun 29 01:46:30 2018, max compression
```

## Comparing `moltemplate-2.8.6.tar` & `moltemplate-2.8.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 jewett   (28537) jewett   (28537)        0 2018-06-28 05:18:36.000000 moltemplate-2.8.6/
-drwxrwxr-x   0 jewett   (28537) jewett   (28537)        0 2018-06-28 05:18:36.000000 moltemplate-2.8.6/moltemplate.egg-info/
--rw-rw-r--   0 jewett   (28537) jewett   (28537)       12 2018-06-28 05:18:36.000000 moltemplate-2.8.6/moltemplate.egg-info/top_level.txt
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     1268 2018-06-28 05:18:36.000000 moltemplate-2.8.6/moltemplate.egg-info/entry_points.txt
--rw-rw-r--   0 jewett   (28537) jewett   (28537)        1 2018-06-28 05:18:36.000000 moltemplate-2.8.6/moltemplate.egg-info/zip-safe
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     2001 2018-06-28 05:18:36.000000 moltemplate-2.8.6/moltemplate.egg-info/SOURCES.txt
--rw-rw-r--   0 jewett   (28537) jewett   (28537)        1 2018-06-28 05:18:36.000000 moltemplate-2.8.6/moltemplate.egg-info/dependency_links.txt
--rw-rw-r--   0 jewett   (28537) jewett   (28537)      979 2018-06-28 05:18:36.000000 moltemplate-2.8.6/moltemplate.egg-info/PKG-INFO
-drwxrwxr-x   0 jewett   (28537) jewett   (28537)        0 2018-06-28 05:18:36.000000 moltemplate-2.8.6/moltemplate/
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)   144120 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/lttree_check.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)     6178 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_fix_ttree_assignments.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     1060 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_Bonds.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)   237497 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/ttree.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)    10447 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/lttree_styles.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     2562 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_Dihedrals.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)    16078 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/bonds_by_type.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)      963 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/extract_espresso_atom_types.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)    37089 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_graph_search.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)     5730 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/pdbsort.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)    39725 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/lttree.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)    15992 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/lttree_postprocess.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)     1633 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/remove_duplicates_nbody.py
-drwxrwxr-x   0 jewett   (28537) jewett   (28537)        0 2018-06-28 05:18:36.000000 moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     3203 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/cenJflipIL.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     1732 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/cenIsortJKL.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)      948 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/bonds_nosym.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     3565 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/gaff_imp.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     3451 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/opls_imp.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     1549 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/angles_nosym.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)        0 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/__init__.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     1732 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/cenJsortIKL.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     1375 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/dihedrals_nosym.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     2713 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/cenIflipJK.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     1370 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/impropers_nosym.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     2713 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/cenIswapJK.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     3203 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/cenJswapIL.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)    44034 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/ttree_matrix_stack.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     1224 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/__init__.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)    82052 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/ttree_lex.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)     6680 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/raw2data.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     8850 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/ordereddict.py
-drwxrwxr-x   0 jewett   (28537) jewett   (28537)        0 2018-06-28 05:18:36.000000 moltemplate-2.8.6/moltemplate/scripts/
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)    46860 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/scripts/emoltemplate.sh
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)     4707 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/scripts/cleanup_moltemplate.sh
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)    86918 2018-06-28 05:03:18.000000 moltemplate-2.8.6/moltemplate/scripts/moltemplate.sh
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)     5553 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/ttree_render.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     2962 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/ettree_styles.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)     1467 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/remove_duplicate_atoms.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)    62722 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/dump2data.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)    12657 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/postprocess_coeffs.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)     4790 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/extract_lammps_data.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)    30584 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_by_type.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     3031 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_Impropers.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)    23693 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/ettree.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     2497 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_Angles.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)    17911 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/charge_by_bond.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)     4232 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_reorder_atoms.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)    34054 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/genpoly_lt.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)    22868 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/nbody_by_type_lib.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)   180341 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/ltemplify.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)     6865 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/postprocess_input_script.py
--rwxrwxr-x   0 jewett   (28537) jewett   (28537)     2188 2018-06-27 23:11:10.000000 moltemplate-2.8.6/moltemplate/renumber_DATA_first_column.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)     3316 2018-06-28 05:03:26.000000 moltemplate-2.8.6/setup.py
--rw-rw-r--   0 jewett   (28537) jewett   (28537)      979 2018-06-28 05:18:36.000000 moltemplate-2.8.6/PKG-INFO
--rw-rw-r--   0 jewett   (28537) jewett   (28537)      104 2018-06-28 05:18:36.000000 moltemplate-2.8.6/setup.cfg
+drwxrwxr-x   0 jewett   (28537) jewett   (28537)        0 2018-06-29 01:46:30.000000 moltemplate-2.8.7/
+drwxrwxr-x   0 jewett   (28537) jewett   (28537)        0 2018-06-29 01:46:30.000000 moltemplate-2.8.7/moltemplate.egg-info/
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)       12 2018-06-29 01:46:30.000000 moltemplate-2.8.7/moltemplate.egg-info/top_level.txt
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     1268 2018-06-29 01:46:30.000000 moltemplate-2.8.7/moltemplate.egg-info/entry_points.txt
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)        1 2018-06-29 01:46:30.000000 moltemplate-2.8.7/moltemplate.egg-info/zip-safe
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     2001 2018-06-29 01:46:30.000000 moltemplate-2.8.7/moltemplate.egg-info/SOURCES.txt
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)        1 2018-06-29 01:46:30.000000 moltemplate-2.8.7/moltemplate.egg-info/dependency_links.txt
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)      979 2018-06-29 01:46:30.000000 moltemplate-2.8.7/moltemplate.egg-info/PKG-INFO
+drwxrwxr-x   0 jewett   (28537) jewett   (28537)        0 2018-06-29 01:46:30.000000 moltemplate-2.8.7/moltemplate/
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)   144120 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/lttree_check.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)     6178 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_fix_ttree_assignments.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     1060 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_Bonds.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)   237497 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/ttree.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)    10447 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/lttree_styles.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     2562 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_Dihedrals.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)    16078 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/bonds_by_type.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)      963 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/extract_espresso_atom_types.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)    37089 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_graph_search.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)     5730 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/pdbsort.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)    39725 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/lttree.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)    15992 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/lttree_postprocess.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)     1633 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/remove_duplicates_nbody.py
+drwxrwxr-x   0 jewett   (28537) jewett   (28537)        0 2018-06-29 01:46:30.000000 moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     3203 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/cenJflipIL.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     1732 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/cenIsortJKL.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)      948 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/bonds_nosym.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     3565 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/gaff_imp.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     3451 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/opls_imp.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     1549 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/angles_nosym.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)        0 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/__init__.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     1732 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/cenJsortIKL.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     1375 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/dihedrals_nosym.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     2713 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/cenIflipJK.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     1370 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/impropers_nosym.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     2713 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/cenIswapJK.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     3203 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/cenJswapIL.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)    44034 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/ttree_matrix_stack.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     1224 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/__init__.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)    82052 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/ttree_lex.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)     6680 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/raw2data.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     8850 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/ordereddict.py
+drwxrwxr-x   0 jewett   (28537) jewett   (28537)        0 2018-06-29 01:46:30.000000 moltemplate-2.8.7/moltemplate/scripts/
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)    46860 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/scripts/emoltemplate.sh
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)     4707 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/scripts/cleanup_moltemplate.sh
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)    86918 2018-06-29 01:42:23.000000 moltemplate-2.8.7/moltemplate/scripts/moltemplate.sh
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)     5553 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/ttree_render.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     2962 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/ettree_styles.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)     1467 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/remove_duplicate_atoms.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)    62722 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/dump2data.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)    12657 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/postprocess_coeffs.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)     4790 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/extract_lammps_data.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)    30584 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_by_type.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     3031 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_Impropers.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)    23693 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/ettree.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     2497 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_Angles.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)    17911 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/charge_by_bond.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)     4232 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_reorder_atoms.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)    34054 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/genpoly_lt.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)    22868 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/nbody_by_type_lib.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)   180341 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/ltemplify.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)     6865 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/postprocess_input_script.py
+-rwxrwxr-x   0 jewett   (28537) jewett   (28537)     2188 2018-06-27 23:11:10.000000 moltemplate-2.8.7/moltemplate/renumber_DATA_first_column.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)     3316 2018-06-29 01:42:12.000000 moltemplate-2.8.7/setup.py
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)      979 2018-06-29 01:46:30.000000 moltemplate-2.8.7/PKG-INFO
+-rw-rw-r--   0 jewett   (28537) jewett   (28537)      104 2018-06-29 01:46:30.000000 moltemplate-2.8.7/setup.cfg
```

### Comparing `moltemplate-2.8.6/moltemplate.egg-info/entry_points.txt` & `moltemplate-2.8.7/moltemplate.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate.egg-info/SOURCES.txt` & `moltemplate-2.8.7/moltemplate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate.egg-info/PKG-INFO` & `moltemplate-2.8.7/moltemplate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: moltemplate
-Version: 2.8.6
+Version: 2.8.7
 Summary: A general cross-platform text-based molecule builder for LAMMPS
 Home-page: https://github.com/jewettaij/moltemplate
 Author: Andrew Jewett
 Author-email: jewett.aij@gmail.com
 License: BSD
-Download-URL: https://github.com/jewettaij/moltemplate/archive/v2.8.6.zip
+Download-URL: https://github.com/jewettaij/moltemplate/archive/v2.8.7.zip
 Description: UNKNOWN
 Keywords: simulation,LAMMPS,molecule editor,molecule builder,ESPResSo
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `moltemplate-2.8.6/moltemplate/lttree_check.py` & `moltemplate-2.8.7/moltemplate/lttree_check.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_fix_ttree_assignments.py` & `moltemplate-2.8.7/moltemplate/nbody_fix_ttree_assignments.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_Bonds.py` & `moltemplate-2.8.7/moltemplate/nbody_Bonds.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/ttree.py` & `moltemplate-2.8.7/moltemplate/ttree.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/lttree_styles.py` & `moltemplate-2.8.7/moltemplate/lttree_styles.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_Dihedrals.py` & `moltemplate-2.8.7/moltemplate/nbody_Dihedrals.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/bonds_by_type.py` & `moltemplate-2.8.7/moltemplate/bonds_by_type.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/extract_espresso_atom_types.py` & `moltemplate-2.8.7/moltemplate/extract_espresso_atom_types.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_graph_search.py` & `moltemplate-2.8.7/moltemplate/nbody_graph_search.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/pdbsort.py` & `moltemplate-2.8.7/moltemplate/pdbsort.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/lttree.py` & `moltemplate-2.8.7/moltemplate/lttree.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/lttree_postprocess.py` & `moltemplate-2.8.7/moltemplate/lttree_postprocess.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/remove_duplicates_nbody.py` & `moltemplate-2.8.7/moltemplate/remove_duplicates_nbody.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/cenJflipIL.py` & `moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/cenJflipIL.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/cenIsortJKL.py` & `moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/cenIsortJKL.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/bonds_nosym.py` & `moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/bonds_nosym.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/gaff_imp.py` & `moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/gaff_imp.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/opls_imp.py` & `moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/opls_imp.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/angles_nosym.py` & `moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/angles_nosym.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/cenJsortIKL.py` & `moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/cenJsortIKL.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/dihedrals_nosym.py` & `moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/dihedrals_nosym.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/cenIflipJK.py` & `moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/cenIflipJK.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/impropers_nosym.py` & `moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/impropers_nosym.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/cenIswapJK.py` & `moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/cenIswapJK.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_alt_symmetry/cenJswapIL.py` & `moltemplate-2.8.7/moltemplate/nbody_alt_symmetry/cenJswapIL.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/ttree_matrix_stack.py` & `moltemplate-2.8.7/moltemplate/ttree_matrix_stack.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/__init__.py` & `moltemplate-2.8.7/moltemplate/__init__.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/ttree_lex.py` & `moltemplate-2.8.7/moltemplate/ttree_lex.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/raw2data.py` & `moltemplate-2.8.7/moltemplate/raw2data.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/ordereddict.py` & `moltemplate-2.8.7/moltemplate/ordereddict.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/scripts/emoltemplate.sh` & `moltemplate-2.8.7/moltemplate/scripts/emoltemplate.sh`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/scripts/cleanup_moltemplate.sh` & `moltemplate-2.8.7/moltemplate/scripts/cleanup_moltemplate.sh`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/scripts/moltemplate.sh` & `moltemplate-2.8.7/moltemplate/scripts/moltemplate.sh`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 #         http://www.moltemplate.org
 #         http://www.chem.ucsb.edu/~sheagroup
 # License: 3-clause BSD License  (See LICENSE.txt)
 # Copyright (c) 2012, Regents of the University of California
 # All rights reserved.
 
 G_PROGRAM_NAME="moltemplate.sh"
-G_VERSION="2.8.6"
-G_DATE="2018-6-27"
+G_VERSION="2.8.7"
+G_DATE="2018-6-28"
 
 echo "${G_PROGRAM_NAME} v${G_VERSION} ${G_DATE}" >&2
 echo "" >&2
 
 # Check for python:
 # I prefer python over python3 because python3 requires slightly
 # more memory.  Use regular python (ie 2.7) when available.
```

### Comparing `moltemplate-2.8.6/moltemplate/ttree_render.py` & `moltemplate-2.8.7/moltemplate/ttree_render.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/ettree_styles.py` & `moltemplate-2.8.7/moltemplate/ettree_styles.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/remove_duplicate_atoms.py` & `moltemplate-2.8.7/moltemplate/remove_duplicate_atoms.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/dump2data.py` & `moltemplate-2.8.7/moltemplate/dump2data.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/postprocess_coeffs.py` & `moltemplate-2.8.7/moltemplate/postprocess_coeffs.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/extract_lammps_data.py` & `moltemplate-2.8.7/moltemplate/extract_lammps_data.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_by_type.py` & `moltemplate-2.8.7/moltemplate/nbody_by_type.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_Impropers.py` & `moltemplate-2.8.7/moltemplate/nbody_Impropers.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/ettree.py` & `moltemplate-2.8.7/moltemplate/ettree.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_Angles.py` & `moltemplate-2.8.7/moltemplate/nbody_Angles.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/charge_by_bond.py` & `moltemplate-2.8.7/moltemplate/charge_by_bond.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_reorder_atoms.py` & `moltemplate-2.8.7/moltemplate/nbody_reorder_atoms.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/genpoly_lt.py` & `moltemplate-2.8.7/moltemplate/genpoly_lt.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/nbody_by_type_lib.py` & `moltemplate-2.8.7/moltemplate/nbody_by_type_lib.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/ltemplify.py` & `moltemplate-2.8.7/moltemplate/ltemplify.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/postprocess_input_script.py` & `moltemplate-2.8.7/moltemplate/postprocess_input_script.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/moltemplate/renumber_DATA_first_column.py` & `moltemplate-2.8.7/moltemplate/renumber_DATA_first_column.py`

 * *Files identical despite different names*

### Comparing `moltemplate-2.8.6/setup.py` & `moltemplate-2.8.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
   author='Andrew Jewett',
 
   author_email='jewett.aij@gmail.com',
 
   url='https://github.com/jewettaij/moltemplate',
 
-  download_url='https://github.com/jewettaij/moltemplate/archive/v2.8.6.zip',
+  download_url='https://github.com/jewettaij/moltemplate/archive/v2.8.7.zip',
 
-  version='2.8.6',
+  version='2.8.7',
 
   keywords=['simulation', 'LAMMPS', 'molecule editor', 'molecule builder',
             'ESPResSo'],
             
 
   # BSD 3-Clause License:
   # - http://choosealicense.com/licenses/bsd-3-clause
```

### Comparing `moltemplate-2.8.6/PKG-INFO` & `moltemplate-2.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: moltemplate
-Version: 2.8.6
+Version: 2.8.7
 Summary: A general cross-platform text-based molecule builder for LAMMPS
 Home-page: https://github.com/jewettaij/moltemplate
 Author: Andrew Jewett
 Author-email: jewett.aij@gmail.com
 License: BSD
-Download-URL: https://github.com/jewettaij/moltemplate/archive/v2.8.6.zip
+Download-URL: https://github.com/jewettaij/moltemplate/archive/v2.8.7.zip
 Description: UNKNOWN
 Keywords: simulation,LAMMPS,molecule editor,molecule builder,ESPResSo
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
```


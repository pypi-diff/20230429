# Comparing `tmp/alphafold-colabfold-2.3.4.tar.gz` & `tmp/alphafold-colabfold-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphafold-colabfold-2.3.4.tar", last modified: Sat Feb 18 15:14:13 2023, max compression
+gzip compressed data, was "alphafold-colabfold-2.3.5.tar", last modified: Sat Apr 29 06:11:55 2023, max compression
```

## Comparing `alphafold-colabfold-2.3.4.tar` & `alphafold-colabfold-2.3.5.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:14:13.646900 alphafold-colabfold-2.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-02-18 15:14:13.646900 alphafold-colabfold-2.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34778 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:14:13.634900 alphafold-colabfold-2.3.4/alphafold/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:14:13.634900 alphafold-colabfold-2.3.4/alphafold/common/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/common/confidence.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/common/protein.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/common/protein_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    34972 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/common/residue_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/common/residue_constants_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/common/stereo_chemical_props.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:14:13.638900 alphafold-colabfold-2.3.4/alphafold/data/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/data/feature_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    14174 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/data/mmcif_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/data/msa_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17220 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/data/msa_pairing.py
--rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/data/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/data/pipeline_multimer.py
--rw-r--r--   0 runner    (1001) docker     (123)    40254 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/data/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:14:13.638900 alphafold-colabfold-2.3.4/alphafold/data/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/data/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/data/tools/hhblits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/data/tools/hhsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/data/tools/hmmbuild.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/data/tools/hmmsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/data/tools/jackhmmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/data/tools/kalign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/data/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:14:13.642900 alphafold-colabfold-2.3.4/alphafold/model/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47028 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/all_atom.py
--rw-r--r--   0 runner    (1001) docker     (123)    40135 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/all_atom_multimer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/all_atom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/common_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    26715 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/features.py
--rw-r--r--   0 runner    (1001) docker     (123)    37211 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/folding.py
--rw-r--r--   0 runner    (1001) docker     (123)    42484 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/folding_multimer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:14:13.642900 alphafold-colabfold-2.3.4/alphafold/model/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/geometry/rigid_matrix_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/geometry/rotation_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/geometry/struct_of_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/geometry/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/geometry/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/geometry/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/layer_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/layer_stack_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/lddt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/lddt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    77787 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    40241 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/modules_multimer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/prng.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/prng_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17388 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/quat_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/quat_affine_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/r3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:14:13.642900 alphafold-colabfold-2.3.4/alphafold/model/tf/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21428 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/tf/data_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/tf/input_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/tf/protein_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/tf/protein_features_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/tf/proteins_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/tf/shape_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/tf/shape_helpers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/tf/shape_placeholders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/tf/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:14:13.642900 alphafold-colabfold-2.3.4/alphafold/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/notebooks/notebook_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/notebooks/notebook_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:14:13.646900 alphafold-colabfold-2.3.4/alphafold/relax/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/relax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19061 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/relax/amber_minimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/relax/amber_minimize_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/relax/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/relax/cleanup_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/relax/relax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/relax/relax_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/relax/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/alphafold/relax/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 15:14:13.646900 alphafold-colabfold-2.3.4/alphafold_colabfold.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-02-18 15:14:13.000000 alphafold-colabfold-2.3.4/alphafold_colabfold.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-02-18 15:14:13.000000 alphafold-colabfold-2.3.4/alphafold_colabfold.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-18 15:14:13.000000 alphafold-colabfold-2.3.4/alphafold_colabfold.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-18 15:14:13.000000 alphafold-colabfold-2.3.4/alphafold_colabfold.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-18 15:14:13.000000 alphafold-colabfold-2.3.4/alphafold_colabfold.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-18 15:14:13.646900 alphafold-colabfold-2.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-02-18 15:13:56.000000 alphafold-colabfold-2.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:11:55.880027 alphafold-colabfold-2.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-29 06:11:55.880027 alphafold-colabfold-2.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34778 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:11:55.868027 alphafold-colabfold-2.3.5/alphafold/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:11:55.868027 alphafold-colabfold-2.3.5/alphafold/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/common/confidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/common/protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/common/protein_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34972 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/common/residue_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/common/residue_constants_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/common/stereo_chemical_props.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:11:55.872027 alphafold-colabfold-2.3.5/alphafold/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/data/feature_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14174 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/data/mmcif_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/data/msa_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17220 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/data/msa_pairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/data/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/data/pipeline_multimer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40254 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/data/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:11:55.872027 alphafold-colabfold-2.3.5/alphafold/data/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/data/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/data/tools/hhblits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/data/tools/hhsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/data/tools/hmmbuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/data/tools/hmmsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/data/tools/jackhmmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/data/tools/kalign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/data/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:11:55.876027 alphafold-colabfold-2.3.5/alphafold/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47028 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/all_atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40135 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/all_atom_multimer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/all_atom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/common_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26715 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37211 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42484 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/folding_multimer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:11:55.876027 alphafold-colabfold-2.3.5/alphafold/model/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/geometry/rigid_matrix_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/geometry/rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/geometry/struct_of_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/geometry/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/geometry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/geometry/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/layer_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/layer_stack_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/lddt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/lddt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77787 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40241 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/modules_multimer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/prng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/prng_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17388 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/quat_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/quat_affine_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/r3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:11:55.876027 alphafold-colabfold-2.3.5/alphafold/model/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21428 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/tf/data_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/tf/input_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/tf/protein_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/tf/protein_features_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/tf/proteins_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/tf/shape_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/tf/shape_helpers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/tf/shape_placeholders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/tf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:11:55.876027 alphafold-colabfold-2.3.5/alphafold/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/notebooks/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/notebooks/notebook_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:11:55.876027 alphafold-colabfold-2.3.5/alphafold/relax/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/relax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19039 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/relax/amber_minimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/relax/amber_minimize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/relax/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/relax/cleanup_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/relax/relax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/relax/relax_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/relax/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/alphafold/relax/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:11:55.880027 alphafold-colabfold-2.3.5/alphafold_colabfold.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-29 06:11:55.000000 alphafold-colabfold-2.3.5/alphafold_colabfold.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-29 06:11:55.000000 alphafold-colabfold-2.3.5/alphafold_colabfold.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 06:11:55.000000 alphafold-colabfold-2.3.5/alphafold_colabfold.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-29 06:11:55.000000 alphafold-colabfold-2.3.5/alphafold_colabfold.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 06:11:55.000000 alphafold-colabfold-2.3.5/alphafold_colabfold.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 06:11:55.880027 alphafold-colabfold-2.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-29 06:11:39.000000 alphafold-colabfold-2.3.5/setup.py
```

### Comparing `alphafold-colabfold-2.3.4/LICENSE` & `alphafold-colabfold-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/PKG-INFO` & `alphafold-colabfold-2.3.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphafold-colabfold
-Version: 2.3.4
+Version: 2.3.5
 Summary: An implementation of the inference pipeline of AlphaFold v2.3.1. This is a completely new model that was entered as AlphaFold2 in CASP14 and published in Nature. This package contains patches for colabfold.
 Home-page: https://github.com/sokrypton/alphafold
 Author: DeepMind
 Author-email: alphafold@deepmind.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `alphafold-colabfold-2.3.4/README.md` & `alphafold-colabfold-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/__init__.py` & `alphafold-colabfold-2.3.5/alphafold/__init__.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/common/__init__.py` & `alphafold-colabfold-2.3.5/alphafold/common/__init__.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/common/confidence.py` & `alphafold-colabfold-2.3.5/alphafold/common/confidence.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/common/protein.py` & `alphafold-colabfold-2.3.5/alphafold/common/protein.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/common/protein_test.py` & `alphafold-colabfold-2.3.5/alphafold/common/protein_test.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/common/residue_constants.py` & `alphafold-colabfold-2.3.5/alphafold/common/residue_constants.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/common/residue_constants_test.py` & `alphafold-colabfold-2.3.5/alphafold/common/residue_constants_test.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/common/stereo_chemical_props.txt` & `alphafold-colabfold-2.3.5/alphafold/common/stereo_chemical_props.txt`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/data/__init__.py` & `alphafold-colabfold-2.3.5/alphafold/data/__init__.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/data/feature_processing.py` & `alphafold-colabfold-2.3.5/alphafold/data/feature_processing.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/data/mmcif_parsing.py` & `alphafold-colabfold-2.3.5/alphafold/data/mmcif_parsing.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/data/msa_identifiers.py` & `alphafold-colabfold-2.3.5/alphafold/data/msa_identifiers.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/data/msa_pairing.py` & `alphafold-colabfold-2.3.5/alphafold/data/msa_pairing.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/data/parsers.py` & `alphafold-colabfold-2.3.5/alphafold/data/parsers.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/data/pipeline.py` & `alphafold-colabfold-2.3.5/alphafold/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/data/pipeline_multimer.py` & `alphafold-colabfold-2.3.5/alphafold/data/pipeline_multimer.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/data/templates.py` & `alphafold-colabfold-2.3.5/alphafold/data/templates.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/data/tools/__init__.py` & `alphafold-colabfold-2.3.5/alphafold/data/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/data/tools/hhblits.py` & `alphafold-colabfold-2.3.5/alphafold/data/tools/hhblits.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/data/tools/hhsearch.py` & `alphafold-colabfold-2.3.5/alphafold/data/tools/hhsearch.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/data/tools/hmmbuild.py` & `alphafold-colabfold-2.3.5/alphafold/data/tools/hmmbuild.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/data/tools/hmmsearch.py` & `alphafold-colabfold-2.3.5/alphafold/data/tools/hmmsearch.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/data/tools/jackhmmer.py` & `alphafold-colabfold-2.3.5/alphafold/data/tools/jackhmmer.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/data/tools/kalign.py` & `alphafold-colabfold-2.3.5/alphafold/data/tools/kalign.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/data/tools/utils.py` & `alphafold-colabfold-2.3.5/alphafold/data/tools/utils.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/__init__.py` & `alphafold-colabfold-2.3.5/alphafold/model/__init__.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/all_atom.py` & `alphafold-colabfold-2.3.5/alphafold/model/all_atom.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/all_atom_multimer.py` & `alphafold-colabfold-2.3.5/alphafold/model/all_atom_multimer.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/all_atom_test.py` & `alphafold-colabfold-2.3.5/alphafold/model/all_atom_test.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/common_modules.py` & `alphafold-colabfold-2.3.5/alphafold/model/common_modules.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/config.py` & `alphafold-colabfold-2.3.5/alphafold/model/config.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/data.py` & `alphafold-colabfold-2.3.5/alphafold/model/data.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/features.py` & `alphafold-colabfold-2.3.5/alphafold/model/features.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/folding.py` & `alphafold-colabfold-2.3.5/alphafold/model/folding.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/folding_multimer.py` & `alphafold-colabfold-2.3.5/alphafold/model/folding_multimer.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/geometry/__init__.py` & `alphafold-colabfold-2.3.5/alphafold/model/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/geometry/rigid_matrix_vector.py` & `alphafold-colabfold-2.3.5/alphafold/model/geometry/rigid_matrix_vector.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/geometry/rotation_matrix.py` & `alphafold-colabfold-2.3.5/alphafold/model/geometry/rotation_matrix.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/geometry/struct_of_array.py` & `alphafold-colabfold-2.3.5/alphafold/model/geometry/struct_of_array.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/geometry/test_utils.py` & `alphafold-colabfold-2.3.5/alphafold/model/geometry/test_utils.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/geometry/utils.py` & `alphafold-colabfold-2.3.5/alphafold/model/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/geometry/vector.py` & `alphafold-colabfold-2.3.5/alphafold/model/geometry/vector.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/layer_stack.py` & `alphafold-colabfold-2.3.5/alphafold/model/layer_stack.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/layer_stack_test.py` & `alphafold-colabfold-2.3.5/alphafold/model/layer_stack_test.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/lddt.py` & `alphafold-colabfold-2.3.5/alphafold/model/lddt.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/lddt_test.py` & `alphafold-colabfold-2.3.5/alphafold/model/lddt_test.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/mapping.py` & `alphafold-colabfold-2.3.5/alphafold/model/mapping.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/model.py` & `alphafold-colabfold-2.3.5/alphafold/model/model.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/modules.py` & `alphafold-colabfold-2.3.5/alphafold/model/modules.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/modules_multimer.py` & `alphafold-colabfold-2.3.5/alphafold/model/modules_multimer.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/prng.py` & `alphafold-colabfold-2.3.5/alphafold/model/prng.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/prng_test.py` & `alphafold-colabfold-2.3.5/alphafold/model/prng_test.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/quat_affine.py` & `alphafold-colabfold-2.3.5/alphafold/model/quat_affine.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/quat_affine_test.py` & `alphafold-colabfold-2.3.5/alphafold/model/quat_affine_test.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/r3.py` & `alphafold-colabfold-2.3.5/alphafold/model/r3.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/tf/__init__.py` & `alphafold-colabfold-2.3.5/alphafold/model/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/tf/data_transforms.py` & `alphafold-colabfold-2.3.5/alphafold/model/tf/data_transforms.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/tf/input_pipeline.py` & `alphafold-colabfold-2.3.5/alphafold/model/tf/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/tf/protein_features.py` & `alphafold-colabfold-2.3.5/alphafold/model/tf/protein_features.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/tf/protein_features_test.py` & `alphafold-colabfold-2.3.5/alphafold/model/tf/protein_features_test.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/tf/proteins_dataset.py` & `alphafold-colabfold-2.3.5/alphafold/model/tf/proteins_dataset.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/tf/shape_helpers.py` & `alphafold-colabfold-2.3.5/alphafold/model/tf/shape_helpers.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/tf/shape_helpers_test.py` & `alphafold-colabfold-2.3.5/alphafold/model/tf/shape_helpers_test.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/tf/shape_placeholders.py` & `alphafold-colabfold-2.3.5/alphafold/model/tf/shape_placeholders.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/tf/utils.py` & `alphafold-colabfold-2.3.5/alphafold/model/tf/utils.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/model/utils.py` & `alphafold-colabfold-2.3.5/alphafold/model/utils.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/notebooks/__init__.py` & `alphafold-colabfold-2.3.5/alphafold/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/notebooks/notebook_utils.py` & `alphafold-colabfold-2.3.5/alphafold/notebooks/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/notebooks/notebook_utils_test.py` & `alphafold-colabfold-2.3.5/alphafold/notebooks/notebook_utils_test.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/relax/__init__.py` & `alphafold-colabfold-2.3.5/alphafold/relax/__init__.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/relax/amber_minimize.py` & `alphafold-colabfold-2.3.5/alphafold/relax/amber_minimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 from alphafold.common import residue_constants
 from alphafold.model import folding
 from alphafold.relax import cleanup
 from alphafold.relax import utils
 import ml_collections
 import numpy as np
 import jax
-from simtk import openmm
-from simtk import unit
-from simtk.openmm import app as openmm_app
-from simtk.openmm.app.internal.pdbstructure import PdbStructure
+import openmm
+from openmm import unit
+from openmm import app as openmm_app
+from openmm.app.internal.pdbstructure import PdbStructure
 
 
 ENERGY = unit.kilocalories_per_mole
 LENGTH = unit.angstroms
 
 
 def will_restrain(atom: openmm_app.Atom, rset: str) -> bool:
```

### Comparing `alphafold-colabfold-2.3.4/alphafold/relax/amber_minimize_test.py` & `alphafold-colabfold-2.3.5/alphafold/relax/amber_minimize_test.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/relax/cleanup.py` & `alphafold-colabfold-2.3.5/alphafold/relax/cleanup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 fix_pdb uses a third-party tool. We also support fixing some additional edge
 cases like removing chains of length one (see clean_structure).
 """
 import io
 
 import pdbfixer
-from simtk.openmm import app
-from simtk.openmm.app import element
+from openmm import app
+from openmm.app import element
 
 
 def fix_pdb(pdbfile, alterations_info):
   """Apply pdbfixer to the contents of a PDB file; return a PDB string result.
 
   1) Replaces nonstandard residues.
   2) Removes heterogens (non protein residues) including water.
```

### Comparing `alphafold-colabfold-2.3.4/alphafold/relax/cleanup_test.py` & `alphafold-colabfold-2.3.5/alphafold/relax/cleanup_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Tests for relax.cleanup."""
 import io
 
 from absl.testing import absltest
 from alphafold.relax import cleanup
-from simtk.openmm.app.internal import pdbstructure
+from openmm.app.internal import pdbstructure
 
 
 def _pdb_to_structure(pdb_str):
   handle = io.StringIO(pdb_str)
   return pdbstructure.PdbStructure(handle)
```

### Comparing `alphafold-colabfold-2.3.4/alphafold/relax/relax.py` & `alphafold-colabfold-2.3.5/alphafold/relax/relax.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/relax/relax_test.py` & `alphafold-colabfold-2.3.5/alphafold/relax/relax_test.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/relax/utils.py` & `alphafold-colabfold-2.3.5/alphafold/relax/utils.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold/relax/utils_test.py` & `alphafold-colabfold-2.3.5/alphafold/relax/utils_test.py`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/alphafold_colabfold.egg-info/PKG-INFO` & `alphafold-colabfold-2.3.5/alphafold_colabfold.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphafold-colabfold
-Version: 2.3.4
+Version: 2.3.5
 Summary: An implementation of the inference pipeline of AlphaFold v2.3.1. This is a completely new model that was entered as AlphaFold2 in CASP14 and published in Nature. This package contains patches for colabfold.
 Home-page: https://github.com/sokrypton/alphafold
 Author: DeepMind
 Author-email: alphafold@deepmind.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `alphafold-colabfold-2.3.4/alphafold_colabfold.egg-info/SOURCES.txt` & `alphafold-colabfold-2.3.5/alphafold_colabfold.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphafold-colabfold-2.3.4/setup.py` & `alphafold-colabfold-2.3.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """Install script for setuptools."""
 
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name='alphafold-colabfold',
-    version='2.3.4',
+    version='2.3.5',
     long_description_content_type='text/markdown',
     description='An implementation of the inference pipeline of AlphaFold v2.3.1. '
     'This is a completely new model that was entered as AlphaFold2 in CASP14 '
     'and published in Nature. This package contains patches for colabfold.',
     author='DeepMind',
     author_email='alphafold@deepmind.com',
     license='Apache License, Version 2.0',
```


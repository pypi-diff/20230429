# Comparing `tmp/adcc-0.15.8.tar.gz` & `tmp/adcc-0.15.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adcc-0.15.8.tar", last modified: Tue Apr 27 06:37:58 2021, max compression
+gzip compressed data, was "adcc-0.15.9.tar", last modified: Wed Jun  2 16:21:28 2021, max compression
```

## Comparing `adcc-0.15.8.tar` & `adcc-0.15.9.tar`

### file list

```diff
@@ -1,163 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 06:37:58.908140 adcc-0.15.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-04-27 06:16:59.000000 adcc-0.15.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      152 2021-04-27 06:16:59.000000 adcc-0.15.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4396 2021-04-27 06:37:58.908140 adcc-0.15.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2864 2021-04-27 06:16:59.000000 adcc-0.15.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 06:37:58.896140 adcc-0.15.8/adcc/
--rw-r--r--   0 runner    (1001) docker     (121)    21946 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/AdcMatrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     3263 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/AdcMethod.py
--rw-r--r--   0 runner    (1001) docker     (121)     8172 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/AmplitudeVector.py
--rw-r--r--   0 runner    (1001) docker     (121)    12259 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/DataHfProvider.py
--rw-r--r--   0 runner    (1001) docker     (121)    13554 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/ElectronicTransition.py
--rw-r--r--   0 runner    (1001) docker     (121)     3497 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/Excitation.py
--rw-r--r--   0 runner    (1001) docker     (121)    21736 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/ExcitedStates.py
--rw-r--r--   0 runner    (1001) docker     (121)     3769 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/FormatDominantElements.py
--rw-r--r--   0 runner    (1001) docker     (121)    10232 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/FormatIndex.py
--rw-r--r--   0 runner    (1001) docker     (121)     7902 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/HfCounterData.py
--rw-r--r--   0 runner    (1001) docker     (121)     2754 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/Intermediates.py
--rw-r--r--   0 runner    (1001) docker     (121)    11293 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/LazyMp.py
--rw-r--r--   0 runner    (1001) docker     (121)     7096 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/MoSpaces.py
--rw-r--r--   0 runner    (1001) docker     (121)    15236 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/OneParticleOperator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5376 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/OperatorIntegrals.py
--rw-r--r--   0 runner    (1001) docker     (121)     9116 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/ReferenceState.py
--rw-r--r--   0 runner    (1001) docker     (121)     3573 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/State2States.py
--rw-r--r--   0 runner    (1001) docker     (121)     1634 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/Symmetry.py
--rw-r--r--   0 runner    (1001) docker     (121)     4264 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/Tensor.py
--rw-r--r--   0 runner    (1001) docker     (121)     6157 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 06:37:58.896140 adcc-0.15.8/adcc/adc_pp/
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/adc_pp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19739 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/adc_pp/matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/adc_pp/modified_transition_moments.py
--rw-r--r--   0 runner    (1001) docker     (121)     5838 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/adc_pp/state2state_transition_dm.py
--rw-r--r--   0 runner    (1001) docker     (121)     6218 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/adc_pp/state_diffdm.py
--rw-r--r--   0 runner    (1001) docker     (121)     4736 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/adc_pp/transition_dm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2449 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/adc_pp/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 06:37:58.896140 adcc-0.15.8/adcc/backends/
--rw-r--r--   0 runner    (1001) docker     (121)     5489 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/backends/EriBuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/backends/InvalidReference.py
--rw-r--r--   0 runner    (1001) docker     (121)     6357 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3997 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/backends/molsturm.py
--rw-r--r--   0 runner    (1001) docker     (121)     8677 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/backends/psi4.py
--rw-r--r--   0 runner    (1001) docker     (121)    10888 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/backends/pyscf.py
--rw-r--r--   0 runner    (1001) docker     (121)     8287 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/backends/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)    10488 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/backends/veloxchem.py
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/block.py
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7400 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 06:37:58.896140 adcc-0.15.8/adcc/guess/
--rw-r--r--   0 runner    (1001) docker     (121)     3518 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/guess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7742 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/guess/guess_zero.py
--rw-r--r--   0 runner    (1001) docker     (121)    12727 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/guess/guesses_from_diagonal.py
--rw-r--r--   0 runner    (1001) docker     (121)     7226 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/hdf5io.py
--rw-r--r--   0 runner    (1001) docker     (121)     2702 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/memory_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)     4781 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5607 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/opt_einsum_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 06:37:58.900140 adcc-0.15.8/adcc/solver/
--rw-r--r--   0 runner    (1001) docker     (121)    10689 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/solver/LanczosIterator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2718 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/solver/SolverStateBase.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1832 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/solver/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     6573 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/solver/conjugate_gradient.py
--rw-r--r--   0 runner    (1001) docker     (121)    17437 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/solver/davidson.py
--rw-r--r--   0 runner    (1001) docker     (121)     3985 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/solver/explicit_symmetrisation.py
--rw-r--r--   0 runner    (1001) docker     (121)    13088 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/solver/lanczos.py
--rw-r--r--   0 runner    (1001) docker     (121)     3590 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/solver/orthogonaliser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4532 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/solver/power_method.py
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/solver/preconditioner.py
--rw-r--r--   0 runner    (1001) docker     (121)     8237 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/timings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 06:37:58.900140 adcc-0.15.8/adcc/visualisation/
--rw-r--r--   0 runner    (1001) docker     (121)     1380 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/visualisation/ExcitationSpectrum.py
--rw-r--r--   0 runner    (1001) docker     (121)     6040 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/visualisation/Spectrum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/visualisation/shapefctns.py
--rw-r--r--   0 runner    (1001) docker     (121)    21716 2021-04-27 06:16:59.000000 adcc-0.15.8/adcc/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 06:37:58.896140 adcc-0.15.8/adcc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4396 2021-04-27 06:37:58.000000 adcc-0.15.8/adcc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3990 2021-04-27 06:37:58.000000 adcc-0.15.8/adcc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-27 06:37:58.000000 adcc-0.15.8/adcc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-27 06:20:31.000000 adcc-0.15.8/adcc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      179 2021-04-27 06:37:58.000000 adcc-0.15.8/adcc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-04-27 06:37:58.000000 adcc-0.15.8/adcc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 06:37:58.904140 adcc-0.15.8/libadcc/
--rw-r--r--   0 runner    (1001) docker     (121)     3098 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/AdcMemory.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3787 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/AdcMemory.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/AxisInfo.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1840 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/AxisInfo.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10619 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/HartreeFockSolution_i.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17155 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/MoIndexTranslation.cc
--rw-r--r--   0 runner    (1001) docker     (121)    10278 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/MoIndexTranslation.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 06:37:58.904140 adcc-0.15.8/libadcc/MoSpaces/
--rw-r--r--   0 runner    (1001) docker     (121)     2929 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/MoSpaces/construct_blocks.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/MoSpaces/construct_blocks.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3002 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/MoSpaces/setup_point_group_table.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/MoSpaces/setup_point_group_table.hh
--rw-r--r--   0 runner    (1001) docker     (121)    20300 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/MoSpaces.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7050 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/MoSpaces.hh
--rw-r--r--   0 runner    (1001) docker     (121)    22555 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/ReferenceState.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8729 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/ReferenceState.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14425 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/Symmetry.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7242 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/Symmetry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2058 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/Tensor.cc
--rw-r--r--   0 runner    (1001) docker     (121)    19007 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/Tensor.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 06:37:58.904140 adcc-0.15.8/libadcc/TensorImpl/
--rw-r--r--   0 runner    (1001) docker     (121)    10791 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/TensorImpl/ExpressionTree.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3071 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/TensorImpl/ExpressionTree.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6248 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/TensorImpl/as_bispace.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/TensorImpl/as_bispace.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7310 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/TensorImpl/as_lt_symmetry.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/TensorImpl/as_lt_symmetry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1592 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/TensorImpl/get_block_starts.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1504 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/TensorImpl/get_block_starts.hh
--rw-r--r--   0 runner    (1001) docker     (121)    60702 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/TensorImpl.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8182 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/TensorImpl.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1749 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/ThreadPool.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2170 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/ThreadPool.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1967 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/Timer.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2427 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/Timer.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6696 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/amplitude_vector_enforce_spin_kind.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/amplitude_vector_enforce_spin_kind.hh
--rw-r--r--   0 runner    (1001) docker     (121)      365 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/backend.cc
--rw-r--r--   0 runner    (1001) docker     (121)      421 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/backend.hh
--rw-r--r--   0 runner    (1001) docker     (121)      925 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/config.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/exceptions.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2671 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/fill_pp_doubles_guesses.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1998 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/fill_pp_doubles_guesses.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 06:37:58.904140 adcc-0.15.8/libadcc/guess/
--rw-r--r--   0 runner    (1001) docker     (121)    18276 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/guess/adc_guess_d.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/guess/adc_guess_d.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2423 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/guess/index_group_d.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4838 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/guess/index_group_d.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13676 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/import_eri.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2104 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/import_eri.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13677 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/make_symmetry.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4593 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/make_symmetry.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 06:37:58.908140 adcc-0.15.8/libadcc/pyiface/
--rw-r--r--   0 runner    (1001) docker     (121)     2402 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/pyiface/ExportAdcc.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2706 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/pyiface/export_AdcMemory.cc
--rw-r--r--   0 runner    (1001) docker     (121)    25967 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/pyiface/export_HartreeFockProvider.cc
--rw-r--r--   0 runner    (1001) docker     (121)    11111 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/pyiface/export_MoIndexTranslation.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6067 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/pyiface/export_MoSpaces.cc
--rw-r--r--   0 runner    (1001) docker     (121)     9312 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/pyiface/export_ReferenceState.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7690 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/pyiface/export_Symmetry.cc
--rw-r--r--   0 runner    (1001) docker     (121)    20043 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/pyiface/export_Tensor.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2352 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/pyiface/export_adc_pp.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2098 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/pyiface/export_threading.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2751 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/pyiface/hartree_fock_solution_hack.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2552 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/pyiface/util.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/pyiface/util.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/shape_to_string.cc
--rw-r--r--   0 runner    (1001) docker     (121)      988 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/shape_to_string.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 06:37:58.908140 adcc-0.15.8/libadcc/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     4431 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/tests/HFSolutionMock.hh
--rw-r--r--   0 runner    (1001) docker     (121)    22743 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/tests/MoIndexTranslationTest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    26086 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/tests/MoSpacesTest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    36582 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/tests/TensorTest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    12782 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/tests/TensorTestData.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/tests/TensorTestData.hh
--rw-r--r--   0 runner    (1001) docker     (121)      760 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/tests/main.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/tests/output_tensor.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4194 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/tests/random_tensor.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/tests/random_tensor.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2021-04-27 06:16:59.000000 adcc-0.15.8/libadcc/tests/wrap_libtensor.hh
--rw-r--r--   0 runner    (1001) docker     (121)      686 2021-04-27 06:37:58.908140 adcc-0.15.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)    19417 2021-04-27 06:16:59.000000 adcc-0.15.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 16:21:28.123412 adcc-0.15.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-06-02 16:00:11.000000 adcc-0.15.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2021-06-02 16:00:11.000000 adcc-0.15.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4396 2021-06-02 16:21:28.123412 adcc-0.15.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2864 2021-06-02 16:00:11.000000 adcc-0.15.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 16:21:28.111411 adcc-0.15.9/adcc/
+-rw-r--r--   0 runner    (1001) docker     (121)    25740 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/AdcMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3263 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/AdcMethod.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8283 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/AmplitudeVector.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12259 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/DataHfProvider.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13554 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/ElectronicTransition.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3497 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/Excitation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23288 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/ExcitedStates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3769 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/FormatDominantElements.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10232 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/FormatIndex.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7902 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/HfCounterData.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2754 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/Intermediates.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11293 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/LazyMp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7096 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/MoSpaces.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15236 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/OneParticleOperator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7306 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/OperatorIntegrals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9201 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/ReferenceState.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3573 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/State2States.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1634 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/Symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4264 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/Tensor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6157 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 16:21:28.111411 adcc-0.15.9/adcc/adc_pp/
+-rw-r--r--   0 runner    (1001) docker     (121)     1448 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/adc_pp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1643 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/adc_pp/environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19740 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/adc_pp/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/adc_pp/modified_transition_moments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5838 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/adc_pp/state2state_transition_dm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6218 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/adc_pp/state_diffdm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4736 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/adc_pp/transition_dm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2449 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/adc_pp/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 16:21:28.115411 adcc-0.15.9/adcc/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)     5489 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/backends/EriBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1218 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/backends/InvalidReference.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6357 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3997 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/backends/molsturm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9467 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/backends/psi4.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11712 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/backends/pyscf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8287 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/backends/testing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10782 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/backends/veloxchem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1470 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/block.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1370 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7400 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 16:21:28.115411 adcc-0.15.9/adcc/guess/
+-rw-r--r--   0 runner    (1001) docker     (121)     3518 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/guess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7742 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/guess/guess_zero.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12727 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/guess/guesses_from_diagonal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7226 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/hdf5io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2702 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/memory_pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4781 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5607 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/opt_einsum_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 16:21:28.115411 adcc-0.15.9/adcc/solver/
+-rw-r--r--   0 runner    (1001) docker     (121)    10689 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/solver/LanczosIterator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2718 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/solver/SolverStateBase.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1832 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/solver/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6573 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/solver/conjugate_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17437 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/solver/davidson.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3985 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/solver/explicit_symmetrisation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13088 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/solver/lanczos.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3590 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/solver/orthogonaliser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4532 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/solver/power_method.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3119 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/solver/preconditioner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8237 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/timings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 16:21:28.115411 adcc-0.15.9/adcc/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (121)     1380 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/visualisation/ExcitationSpectrum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6040 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/visualisation/Spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1013 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1163 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/visualisation/shapefctns.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25235 2021-06-02 16:00:11.000000 adcc-0.15.9/adcc/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 16:21:28.111411 adcc-0.15.9/adcc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4396 2021-06-02 16:21:28.000000 adcc-0.15.9/adcc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4017 2021-06-02 16:21:28.000000 adcc-0.15.9/adcc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-02 16:21:28.000000 adcc-0.15.9/adcc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-02 16:03:54.000000 adcc-0.15.9/adcc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2021-06-02 16:21:28.000000 adcc-0.15.9/adcc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-06-02 16:21:28.000000 adcc-0.15.9/adcc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 16:21:28.119412 adcc-0.15.9/libadcc/
+-rw-r--r--   0 runner    (1001) docker     (121)     3098 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/AdcMemory.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3787 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/AdcMemory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/AxisInfo.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1840 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/AxisInfo.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10619 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/HartreeFockSolution_i.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17155 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/MoIndexTranslation.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    10278 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/MoIndexTranslation.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 16:21:28.119412 adcc-0.15.9/libadcc/MoSpaces/
+-rw-r--r--   0 runner    (1001) docker     (121)     2929 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/MoSpaces/construct_blocks.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1508 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/MoSpaces/construct_blocks.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3002 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/MoSpaces/setup_point_group_table.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1241 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/MoSpaces/setup_point_group_table.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    20300 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/MoSpaces.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7050 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/MoSpaces.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    22555 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/ReferenceState.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     8729 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/ReferenceState.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14425 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/Symmetry.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7242 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/Symmetry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2058 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/Tensor.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    19007 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/Tensor.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 16:21:28.119412 adcc-0.15.9/libadcc/TensorImpl/
+-rw-r--r--   0 runner    (1001) docker     (121)    10791 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/TensorImpl/ExpressionTree.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3071 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/TensorImpl/ExpressionTree.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6248 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/TensorImpl/as_bispace.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/TensorImpl/as_bispace.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7310 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/TensorImpl/as_lt_symmetry.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1296 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/TensorImpl/as_lt_symmetry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1592 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/TensorImpl/get_block_starts.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1504 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/TensorImpl/get_block_starts.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    60702 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/TensorImpl.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     8181 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/TensorImpl.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1749 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/ThreadPool.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2170 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/ThreadPool.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1967 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/Timer.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2427 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/Timer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6696 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/amplitude_vector_enforce_spin_kind.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1403 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/amplitude_vector_enforce_spin_kind.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      365 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/backend.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      421 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/backend.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      925 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/config.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1156 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/exceptions.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2671 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/fill_pp_doubles_guesses.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1998 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/fill_pp_doubles_guesses.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 16:21:28.119412 adcc-0.15.9/libadcc/guess/
+-rw-r--r--   0 runner    (1001) docker     (121)    18276 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/guess/adc_guess_d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/guess/adc_guess_d.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2423 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/guess/index_group_d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4838 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/guess/index_group_d.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13676 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/import_eri.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2104 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/import_eri.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13677 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/make_symmetry.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4593 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/make_symmetry.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 16:21:28.123412 adcc-0.15.9/libadcc/pyiface/
+-rw-r--r--   0 runner    (1001) docker     (121)     2402 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/pyiface/ExportAdcc.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2706 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/pyiface/export_AdcMemory.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    25967 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/pyiface/export_HartreeFockProvider.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    11111 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/pyiface/export_MoIndexTranslation.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6067 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/pyiface/export_MoSpaces.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     9312 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/pyiface/export_ReferenceState.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7690 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/pyiface/export_Symmetry.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    20043 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/pyiface/export_Tensor.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2352 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/pyiface/export_adc_pp.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2098 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/pyiface/export_threading.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2751 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/pyiface/hartree_fock_solution_hack.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2552 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/pyiface/util.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/pyiface/util.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/shape_to_string.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      988 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/shape_to_string.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-02 16:21:28.123412 adcc-0.15.9/libadcc/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     4431 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/tests/HFSolutionMock.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    22743 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/tests/MoIndexTranslationTest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    26086 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/tests/MoSpacesTest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    36582 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/tests/TensorTest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    12782 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/tests/TensorTestData.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1502 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/tests/TensorTestData.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      760 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/tests/main.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1159 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/tests/output_tensor.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4194 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/tests/random_tensor.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/tests/random_tensor.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1085 2021-06-02 16:00:11.000000 adcc-0.15.9/libadcc/tests/wrap_libtensor.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      686 2021-06-02 16:21:28.123412 adcc-0.15.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)    19429 2021-06-02 16:00:11.000000 adcc-0.15.9/setup.py
```

### Comparing `adcc-0.15.8/LICENSE` & `adcc-0.15.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/PKG-INFO` & `adcc-0.15.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adcc
-Version: 0.15.8
+Version: 0.15.9
 Summary: adcc:  Seamlessly connect your host program to ADC
 Home-page: https://adc-connect.org
 Author: Michael F. Herbst, Maximilian Scheurer
 Author-email: developers@adc-connect.org
 License: GPL v3
 Project-URL: Source, https://github.com/adc-connect/adcc
 Project-URL: Issues, https://github.com/adc-connect/adcc/issues
```

### Comparing `adcc-0.15.8/README.md` & `adcc-0.15.9/README.md`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/AdcMatrix.py` & `adcc-0.15.9/adcc/AdcMatrix.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,46 @@
 from .adc_pp import matrix as ppmatrix
 from .timings import Timer, timed_member_call
 from .AdcMethod import AdcMethod
 from .Intermediates import Intermediates
 from .AmplitudeVector import AmplitudeVector
 
 
+class AdcExtraTerm:
+    def __init__(self, matrix, blocks):
+        """Initialise an AdcExtraTerm.
+        This class can be used to add customs terms
+        to an existing :py:class:`AdcMatrix`
+
+        Parameters
+        ----------
+        matrix : AdcMatrix
+            The matrix for which the extra term
+            should be created.
+        blocks : dict
+            A dictionary where the key labels the matrix block
+            and the item denotes a callable to construct
+            an :py:class:`AdcBlock`
+        """
+        self.ground_state = matrix.ground_state
+        self.reference_state = matrix.reference_state
+        self.intermediates = matrix.intermediates
+        self.blocks = {}
+        if not isinstance(blocks, dict):
+            raise TypeError("blocks needs to be a dict.")
+        for space in blocks:
+            block_fun = blocks[space]
+            if not callable(block_fun):
+                raise TypeError("Items in additional_blocks must be callable.")
+            block = block_fun(
+                self.reference_state, self.ground_state, self.intermediates
+            )
+            self.blocks[space] = block
+
+
 class AdcMatrixlike:
     """
     Base class marker for all objects like ADC matrices.
     """
     pass
 
 
@@ -46,48 +78,60 @@
         "adc0":  dict(ph_ph=0, ph_pphh=None, pphh_ph=None, pphh_pphh=None),  # noqa: E501
         "adc1":  dict(ph_ph=1, ph_pphh=None, pphh_ph=None, pphh_pphh=None),  # noqa: E501
         "adc2":  dict(ph_ph=2, ph_pphh=1,    pphh_ph=1,    pphh_pphh=0),     # noqa: E501
         "adc2x": dict(ph_ph=2, ph_pphh=1,    pphh_ph=1,    pphh_pphh=1),     # noqa: E501
         "adc3":  dict(ph_ph=3, ph_pphh=2,    pphh_ph=2,    pphh_pphh=1),     # noqa: E501
     }
 
-    def __init__(self, method, hf_or_mp, block_orders=None, intermediates=None):
+    def __init__(self, method, hf_or_mp, block_orders=None, intermediates=None,
+                 diagonal_precomputed=None):
         """
         Initialise an ADC matrix.
 
         Parameters
         ----------
         method : str or AdcMethod
             Method to use.
         hf_or_mp : adcc.ReferenceState or adcc.LazyMp
             HF reference or MP ground state
         block_orders : optional
             The order of perturbation theory to employ for each matrix block.
             If not set, defaults according to the selected ADC method are chosen.
         intermediates : adcc.Intermediates or NoneType
             Allows to pass intermediates to re-use to this class.
+        diagonal_precomputed: adcc.AmplitudeVector
+            Allows to pass a pre-computed diagonal, for internal use only.
         """
         if isinstance(hf_or_mp, (libadcc.ReferenceState,
                                  libadcc.HartreeFockSolution_i)):
             hf_or_mp = LazyMp(hf_or_mp)
         if not isinstance(hf_or_mp, LazyMp):
-            raise TypeError("mp_results is not a valid object. It needs to be "
+            raise TypeError("hf_or_mp is not a valid object. It needs to be "
                             "either a LazyMp, a ReferenceState or a "
                             "HartreeFockSolution_i.")
 
         if not isinstance(method, AdcMethod):
             method = AdcMethod(method)
 
+        if diagonal_precomputed:
+            if not isinstance(diagonal_precomputed, AmplitudeVector):
+                raise TypeError("diagonal_precomputed needs to be"
+                                " an AmplitudeVector.")
+            if diagonal_precomputed.needs_evaluation:
+                raise ValueError("diagonal_precomputed must already"
+                                 " be evaluated.")
+
         self.timer = Timer()
         self.method = method
         self.ground_state = hf_or_mp
         self.reference_state = hf_or_mp.reference_state
         self.mospaces = hf_or_mp.reference_state.mospaces
         self.is_core_valence_separated = method.is_core_valence_separated
         self.ndim = 2
+        self.extra_terms = []
 
         self.intermediates = intermediates
         if self.intermediates is None:
             self.intermediates = Intermediates(self.ground_state)
 
         # Determine orders of PT in the blocks
         if block_orders is None:
@@ -108,27 +152,85 @@
            and block_orders["pphh_pphh"] is None:
             raise ValueError("pphh_pphh cannot be None if ph_pphh isn't.")
         self.block_orders = block_orders
 
         # Build the blocks and diagonals
         with self.timer.record("build"):
             variant = None
-            if method.is_core_valence_separated:
+            if self.is_core_valence_separated:
                 variant = "cvs"
-            self.blocks_ph = {  # TODO Rename to self.block in 0.16.0
+            blocks = {
                 block: ppmatrix.block(self.ground_state, block.split("_"),
                                       order=order, intermediates=self.intermediates,
                                       variant=variant)
-                for block, order in block_orders.items() if order is not None
+                for block, order in self.block_orders.items() if order is not None
             }
-            self.__diagonal = sum(bl.diagonal for bl in self.blocks_ph.values()
-                                  if bl.diagonal)
-            self.__diagonal.evaluate()
+            # TODO Rename to self.block in 0.16.0
+            self.blocks_ph = {bl: blocks[bl].apply for bl in blocks}
+            if diagonal_precomputed:
+                self.__diagonal = diagonal_precomputed
+            else:
+                self.__diagonal = sum(bl.diagonal for bl in blocks.values()
+                                      if bl.diagonal)
+                self.__diagonal.evaluate()
             self.__init_space_data(self.__diagonal)
 
+    def __iadd__(self, other):
+        """In-place addition of an :py:class:`AdcExtraTerm`
+
+        Parameters
+        ----------
+        other : AdcExtraTerm
+            the extra term to be added
+        """
+        if not isinstance(other, AdcExtraTerm):
+            return NotImplemented
+        if not all(k in self.blocks_ph for k in other.blocks):
+            raise ValueError("Can only add to blocks of"
+                             " AdcMatrix that already exist.")
+        for sp in other.blocks:
+            orig_app = self.blocks_ph[sp]
+            other_app = other.blocks[sp].apply
+
+            def patched_apply(ampl, original=orig_app, other=other_app):
+                return sum(app(ampl) for app in (original, other))
+            self.blocks_ph[sp] = patched_apply
+        other_diagonal = sum(bl.diagonal for bl in other.blocks.values()
+                             if bl.diagonal)
+        self.__diagonal = self.__diagonal + other_diagonal
+        self.__diagonal.evaluate()
+        self.extra_terms.append(other)
+        return self
+
+    def __add__(self, other):
+        """Addition of an :py:class:`AdcExtraTerm`, creating
+        a copy of self and adding the term to the new matrix
+
+        Parameters
+        ----------
+        other : AdcExtraTerm
+            the extra term to be added
+
+        Returns
+        -------
+        AdcMatrix
+            a copy of the AdcMatrix with the extra term added
+        """
+        if not isinstance(other, AdcExtraTerm):
+            return NotImplemented
+        ret = AdcMatrix(self.method, self.ground_state,
+                        block_orders=self.block_orders,
+                        intermediates=self.intermediates,
+                        diagonal_precomputed=self.diagonal())
+        ret += other
+        return ret
+
+    def __radd__(self, other):
+        return self.__add__(other)
+
     def __init_space_data(self, diagonal):
         """Update the cached data regarding the spaces of the ADC matrix"""
         self.axis_spaces = {}
         self.axis_lengths = {}
         for block in diagonal.blocks_ph:
             self.axis_spaces[block] = getattr(diagonal, block).subspaces
             self.axis_lengths[block] = np.prod([
@@ -204,24 +306,24 @@
         """
         if not isinstance(tensor, libadcc.Tensor):
             raise TypeError("tensor should be an adcc.Tensor")
 
         with self.timer.record(f"apply/{block}"):
             outblock, inblock = block.split("_")
             ampl = AmplitudeVector(**{inblock: tensor})
-            ret = self.blocks_ph[block].apply(ampl)
+            ret = self.blocks_ph[block](ampl)
             return getattr(ret, outblock)
 
     @timed_member_call()
     def matvec(self, v):
         """
         Compute the matrix-vector product of the ADC matrix
         with an excitation amplitude and return the result.
         """
-        return sum(block.apply(v) for block in self.blocks_ph.values())
+        return sum(block(v) for block in self.blocks_ph.values())
 
     def rmatvec(self, v):
         # ADC matrix is symmetric
         return self.matvec(v)
 
     def compute_matvec(self, ampl):
         """
```

### Comparing `adcc-0.15.8/adcc/AdcMethod.py` & `adcc-0.15.9/adcc/AdcMethod.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/AmplitudeVector.py` & `adcc-0.15.9/adcc/AmplitudeVector.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,18 @@
         return AmplitudeVector(**{k: t.copy() for k, t in self.items()})
 
     def evaluate(self):
         for t in self.values():
             t.evaluate()
         return self
 
+    @property
+    def needs_evaluation(self):
+        return any(t.needs_evaluation for k, t in self.items())
+
     def ones_like(self):
         """Return an empty AmplitudeVector of the same shape and symmetry"""
         return AmplitudeVector(**{k: t.ones_like() for k, t in self.items()})
 
     def empty_like(self):
         """Return an empty AmplitudeVector of the same shape and symmetry"""
         return AmplitudeVector(**{k: t.empty_like() for k, t in self.items()})
```

### Comparing `adcc-0.15.8/adcc/DataHfProvider.py` & `adcc-0.15.9/adcc/DataHfProvider.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/ElectronicTransition.py` & `adcc-0.15.9/adcc/ElectronicTransition.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/Excitation.py` & `adcc-0.15.9/adcc/Excitation.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/ExcitedStates.py` & `adcc-0.15.9/adcc/ExcitedStates.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,40 @@
 from .FormatIndex import (FormatIndexAdcc, FormatIndexBase,
                           FormatIndexHfProvider, FormatIndexHomoLumo)
 from .OneParticleOperator import product_trace
 from .ElectronicTransition import ElectronicTransition
 from .FormatDominantElements import FormatDominantElements
 
 
+class EnergyCorrection:
+    def __init__(self, name, function):
+        """A helper class to represent excitation energy
+        corrections.
+
+        Parameters
+        ----------
+        name : str
+            descriptive name of the energy correction
+        function : callable
+            function that takes a :py:class:`Excitation`
+            as single argument and returns the energy
+            correction as a float
+        """
+        if not isinstance(name, str):
+            raise TypeError("name needs to be a string.")
+        if not callable(function):
+            raise TypeError("function needs to be callable.")
+        self.name = name
+        self.function = function
+
+    def __call__(self, excitation):
+        assert isinstance(excitation, Excitation)
+        return self.function(excitation)
+
+
 class FormatExcitationVector:
     def __init__(self, matrix, tolerance=0.01, index_format=None):
         """
         Set up a formatter class for formatting excitation vectors.
 
         Parameters
         ----------
@@ -123,16 +149,15 @@
             for indices, spins, value in formatted:
                 ret.append(formats[stripped].format(*indices, *spins)
                            + "   " + self.value_format.format(value))
         return "\n".join(ret)
 
 
 class ExcitedStates(ElectronicTransition):
-    def __init__(self, data, method=None, property_method=None,
-                 excitation_energy_corrections={}):
+    def __init__(self, data, method=None, property_method=None):
         """Construct an ExcitedStates class from some data obtained
         from an interative solver or another :class:`ExcitedStates`
         object.
 
         The class provides access to the results from an ADC calculation
         as well as derived properties. Properties are computed lazily
         on the fly as requested by the user.
@@ -149,41 +174,53 @@
             a :class:`solver.EigenSolverStateBase`. Can also be an
             :class:`ExcitedStates` object.
         method : str, optional
             Provide an explicit method parameter if data contains none.
         property_method : str, optional
             Provide an explicit method for property calculations to
             override the automatic selection.
-        excitation_energy_corrections : dict, optional
-            Provide a dictionary of functions to compute corrections for
-            excitation energies, called for each excitation individually
         """
         super().__init__(data, method, property_method)
+        self._excitation_energy_corrections = []
+        # copy energy corrections if possible
+        # and avoids re-computation of the corrections
+        if hasattr(data, "_excitation_energy_corrections"):
+            for eec in data._excitation_energy_corrections:
+                correction_energy = getattr(data, eec.name)
+                setattr(self, eec.name, correction_energy)
+                self._excitation_energy += correction_energy
+                self._excitation_energy_corrections.append(eec)
+
+    def __add_energy_correction(self, correction):
+        assert isinstance(correction, EnergyCorrection)
+        if hasattr(self, correction.name):
+            raise ValueError("ExcitedStates already has a correction"
+                             f" with the name '{correction.name}'")
+        correction_energy = np.array([correction(exci)
+                                      for exci in self.excitations])
+        setattr(self, correction.name, correction_energy)
+        self._excitation_energy += correction_energy
+        self._excitation_energy_corrections.append(correction)
+
+    def __iadd__(self, other):
+        if isinstance(other, EnergyCorrection):
+            self.__add_energy_correction(other)
+        elif isinstance(other, list):
+            for k in other:
+                self += k
+        else:
+            return NotImplemented
+        return self
 
-        if hasattr(data, "excitation_energy_corrections"):
-            merged = data.excitation_energy_corrections.copy()
-            merged.update(excitation_energy_corrections)
-            excitation_energy_corrections = merged
-
-        if hasattr(self.reference_state, "excitation_energy_corrections"):
-            merged = self.reference_state.excitation_energy_corrections.copy()
-            merged.update(excitation_energy_corrections)
-            excitation_energy_corrections = merged
-
-        self.excitation_energy_corrections = excitation_energy_corrections
-        for key in self.excitation_energy_corrections:
-            corr_function = self.excitation_energy_corrections[key]
-            if not callable(corr_function):
-                raise TypeError("Elements in excitation_energy_corrections "
-                                "must be callable.")
-            # call the function for exc. energy correction
-            correction = np.array([corr_function(exci)
-                                   for exci in self.excitations])
-            setattr(self, key, correction)
-            self._excitation_energy += correction
+    def __add__(self, other):
+        if not isinstance(other, (EnergyCorrection, list)):
+            return NotImplemented
+        ret = ExcitedStates(self, self.method, self.property_method)
+        ret += other
+        return ret
 
     @cached_property
     @mark_excitation_property(transform_to_ao=True)
     @timed_member_call(timer="_property_timer")
     def transition_dm(self):
         """List of transition density matrices of all computed states"""
         return [adc_pp.transition_dm(self.property_method, self.ground_state,
@@ -334,14 +371,24 @@
         for i, vec in enumerate(self.excitation_vector):
             fields = {}
             for k, compute in opt.items():
                 fields[k] = compute(i, vec)
             text += body.format(i=i, ene=self.excitation_energy[i],
                                 ev=self.excitation_energy[i] * eV, **fields)
         text += separator + "\n"
+        if len(self._excitation_energy_corrections):
+            head_corr = "|  Excitation energy includes these corrections:"
+            text += head_corr
+            nspace = len(separator) - len(head_corr) - 1
+            text += nspace * " " + "|\n"
+            maxlen = len(separator) - 8
+            for eec in self._excitation_energy_corrections:
+                label = f"|    - {eec.name:{maxlen}.{maxlen}}|\n"
+                text += label
+            text += separator + "\n"
         return text
 
     def _repr_pretty_(self, pp, cycle):
         if cycle:
             pp.text("ExcitedStates(...)")
         else:
             pp.text(self.describe())
@@ -394,15 +441,15 @@
 
     def to_dataframe(self):
         """
         Exports the ExcitedStates object as :class:`pandas.DataFrame`.
         Atomic units are used for all values.
         """
         propkeys = self.excitation_property_keys
-        propkeys.extend(self.excitation_energy_corrections.keys())
+        propkeys.extend([k.name for k in self._excitation_energy_corrections])
         data = {
             "excitation": np.arange(0, self.size, dtype=int),
             "kind": np.tile(self.kind, self.size)
         }
         for key in propkeys:
             try:
                 d = getattr(self, key)
```

### Comparing `adcc-0.15.8/adcc/FormatDominantElements.py` & `adcc-0.15.9/adcc/FormatDominantElements.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/FormatIndex.py` & `adcc-0.15.9/adcc/FormatIndex.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/HfCounterData.py` & `adcc-0.15.9/adcc/HfCounterData.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/Intermediates.py` & `adcc-0.15.9/adcc/Intermediates.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/LazyMp.py` & `adcc-0.15.9/adcc/LazyMp.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/MoSpaces.py` & `adcc-0.15.9/adcc/MoSpaces.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/OneParticleOperator.py` & `adcc-0.15.9/adcc/OneParticleOperator.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/OperatorIntegrals.py` & `adcc-0.15.9/adcc/OperatorIntegrals.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,24 +28,29 @@
 from .OneParticleOperator import OneParticleOperator
 
 import libadcc
 
 
 def transform_operator_ao2mo(tensor_bb, tensor_ff, coefficients,
                              conv_tol=1e-14):
-    """
-    Take a block-diagonal tensor in the atomic orbital basis
+    """Take a block-diagonal tensor in the atomic orbital basis
     and transform it into the molecular orbital basis in the
     convention used by adcc.
 
-    @param tensor_bb  Block-diagonal tensor in the atomic orbital basis
-    @param tensor_ff  Output tensor with the symmetry set-up to contain
-                      the operator in the molecular orbital representation
-    @param coefficients    Function providing coefficient blocks
-    @param conv_tol   SCF convergence tolerance
+    Parameters
+    ----------
+    tensor_bb : Tensor
+        Block-diagonal tensor in the atomic orbital basis
+    tensor_ff : Tensor
+        Output tensor with the symmetry set-up to contain
+        the operator in the molecular orbital representation
+    coefficients : callable
+        Function providing coefficient blocks
+    conv_tol : float, optional
+        SCF convergence tolerance, by default 1e-14
     """
     for blk in tensor_ff.blocks:
         assert len(blk) == 4
         cleft = coefficients(blk[:2] + "b")
         cright = coefficients(blk[2:] + "b")
         temp = cleft @ tensor_bb @ cright.transpose()
 
@@ -89,16 +94,21 @@
         atomic orbital basis from the backend.
         """
         return self.__provider_ao
 
     @cached_property
     def available(self):
         """Which integrals are available in the underlying backend"""
-        return [integral
-                for integral in ("electric_dipole", "magnetic_dipole", "nabla")
+        integrals = (
+            "electric_dipole",
+            "magnetic_dipole",
+            "nabla",
+            "pe_induction_elec"
+        )
+        return [integral for integral in integrals
                 if hasattr(self.provider_ao, integral)]
 
     def import_dipole_like_operator(self, integral, is_symmetric=True):
         if integral not in self.available:
             raise NotImplementedError(f"{integral.replace('_', ' ')} operator "
                                       "not implemented "
                                       f"in {self.provider_ao.backend} backend.")
@@ -133,12 +143,52 @@
     def nabla(self):
         """
         Return the momentum (nabla operator) integrals
         in the molecular orbital basis.
         """
         return self.import_dipole_like_operator("nabla", is_symmetric=False)
 
+    def __import_density_dependent_operator(self, ao_callback, is_symmetric=True):
+        """Returns a function that imports a density-dependent operator.
+        The returned function imports the operator and transforms it to the
+        molecular orbital basis.
+
+        Parameters
+        ----------
+        ao_callback : callable
+            Function that computes the operator in atomic orbitals using
+            a :py:class:`OneParticleOperator` (the density matrix
+            in atomic orbitals) as single argument
+        is_symmetric : bool, optional
+            if the imported operator is symmetric, by default True
+        """
+        def process_operator(dm, callback=ao_callback, is_symmetric=is_symmetric):
+            dm_ao = sum(dm.to_ao_basis())
+            v_ao = callback(dm_ao)
+            v_bb = replicate_ao_block(
+                self.mospaces, v_ao, is_symmetric=is_symmetric
+            )
+            v_ff = OneParticleOperator(self.mospaces, is_symmetric=is_symmetric)
+            transform_operator_ao2mo(
+                v_bb, v_ff, self.__coefficients, self.__conv_tol
+            )
+            return v_ff
+        return process_operator
+
+    @property
+    def pe_induction_elec(self):
+        """
+        Returns a function to obtain the (density-dependent)
+        PE electronic induction operator in the molecular orbital basis
+        """
+        if "pe_induction_elec" not in self.available:
+            raise NotImplementedError("PE electronic induction operator "
+                                      "not implemented "
+                                      f"in {self.provider_ao.backend} backend.")
+        callback = self.provider_ao.pe_induction_elec
+        return self.__import_density_dependent_operator(callback)
+
     @property
     def timer(self):
         ret = Timer()
         ret.attach(self._import_timer, subtree="import")
         return ret
```

### Comparing `adcc-0.15.8/adcc/ReferenceState.py` & `adcc-0.15.9/adcc/ReferenceState.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,16 @@
             super().import_all()
 
         self.operators = OperatorIntegrals(
             hfdata.operator_integral_provider, self._mospaces,
             self.orbital_coefficients, self.conv_tol
         )
 
-        for name in ["excitation_energy_corrections"]:
+        self.environment = None  # no environment attached by default
+        for name in ["excitation_energy_corrections", "environment"]:
             if hasattr(hfdata, name):
                 setattr(self, name, getattr(hfdata, name))
 
     def __getattr__(self, attr):
         from . import block as b
 
         if attr.startswith("f"):
```

### Comparing `adcc-0.15.8/adcc/State2States.py` & `adcc-0.15.9/adcc/State2States.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/Symmetry.py` & `adcc-0.15.9/adcc/Symmetry.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/Tensor.py` & `adcc-0.15.9/adcc/Tensor.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/__init__.py` & `adcc-0.15.9/adcc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
            "Tensor", "DictHfProvider", "DataHfProvider", "OneParticleOperator",
            "guesses_singlet", "guesses_triplet", "guesses_any",
            "guess_symmetries", "guesses_spin_flip", "guess_zero", "LazyMp",
            "adc0", "cis", "adc1", "adc2", "adc2x", "adc3",
            "cvs_adc0", "cvs_adc1", "cvs_adc2", "cvs_adc2x", "cvs_adc3",
            "banner"]
 
-__version__ = "0.15.8"
+__version__ = "0.15.9"
 __license__ = "GPL v3"
 __url__ = "https://adc-connect.org"
 __authors__ = ["Michael F. Herbst", "Maximilian Scheurer"]
 __email__ = "developers@adc-connect.org"
 __contributors__ = []
```

### Comparing `adcc-0.15.8/adcc/adc_pp/__init__.py` & `adcc-0.15.9/adcc/adc_pp/__init__.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/adc_pp/matrix.py` & `adcc-0.15.9/adcc/adc_pp/matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     """
     Gets ground state, potentially intermediates, spaces (ph, pphh and so on)
     and the perturbation theory order for the block,
     variant is "cvs" or sth like that.
 
     It is assumed largely, that CVS is equivalent to mp.has_core_occupied_space,
     while one would probably want in the long run that one can have an "o2" space,
-    but not do CVS
+    but not do CVS.
     """
     if isinstance(variant, str):
         variant = [variant]
     elif variant is None:
         variant = []
     reference_state = ground_state.reference_state
     if intermediates is None:
```

### Comparing `adcc-0.15.8/adcc/adc_pp/modified_transition_moments.py` & `adcc-0.15.9/adcc/adc_pp/modified_transition_moments.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/adc_pp/state2state_transition_dm.py` & `adcc-0.15.9/adcc/adc_pp/state2state_transition_dm.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/adc_pp/state_diffdm.py` & `adcc-0.15.9/adcc/adc_pp/state_diffdm.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/adc_pp/transition_dm.py` & `adcc-0.15.9/adcc/adc_pp/transition_dm.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/adc_pp/util.py` & `adcc-0.15.9/adcc/adc_pp/util.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/backends/EriBuilder.py` & `adcc-0.15.9/adcc/backends/EriBuilder.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/backends/InvalidReference.py` & `adcc-0.15.9/adcc/backends/InvalidReference.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/backends/__init__.py` & `adcc-0.15.9/adcc/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/backends/molsturm.py` & `adcc-0.15.9/adcc/backends/molsturm.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/backends/psi4.py` & `adcc-0.15.9/adcc/backends/psi4.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from libadcc import HartreeFockProvider
 from adcc.misc import cached_property
 
 import psi4
 
 from .EriBuilder import EriBuilder
 from ..exceptions import InvalidReference
+from ..ExcitedStates import EnergyCorrection
 
 
 class Psi4OperatorIntegralProvider:
     def __init__(self, wfn):
         self.wfn = wfn
         self.backend = "psi4"
         self.mints = psi4.core.MintsHelper(self.wfn)
@@ -49,14 +50,24 @@
             for comp in self.mints.ao_angular_momentum()
         ]
 
     @cached_property
     def nabla(self):
         return [-1.0 * np.asarray(comp) for comp in self.mints.ao_nabla()]
 
+    @property
+    def pe_induction_elec(self):
+        if hasattr(self.wfn, "pe_state"):
+            def pe_induction_elec_ao(dm):
+                return self.wfn.pe_state.get_pe_contribution(
+                    psi4.core.Matrix.from_array(dm.to_ndarray()),
+                    elec_only=True
+                )[1]
+            return pe_induction_elec_ao
+
 
 class Psi4EriBuilder(EriBuilder):
     def __init__(self, wfn, n_orbs, n_orbs_alpha, n_alpha, n_beta, restricted):
         self.wfn = wfn
         self.mints = psi4.core.MintsHelper(self.wfn)
         super().__init__(n_orbs, n_orbs_alpha, n_alpha, n_beta, restricted)
 
@@ -93,20 +104,34 @@
         density_psi = psi4.core.Matrix.from_array(dm.to_ndarray())
         e_pe, _ = self.wfn.pe_state.get_pe_contribution(density_psi,
                                                         elec_only=elec_only)
         return e_pe
 
     @property
     def excitation_energy_corrections(self):
-        ret = {}
+        ret = []
+        if self.environment == "pe":
+            ptlr = EnergyCorrection(
+                "pe_ptlr_correction",
+                lambda view: 2.0 * self.pe_energy(view.transition_dm_ao,
+                                                  elec_only=True)
+            )
+            ptss = EnergyCorrection(
+                "pe_ptss_correction",
+                lambda view: self.pe_energy(view.state_diffdm_ao,
+                                            elec_only=True)
+            )
+            ret.extend([ptlr, ptss])
+        return {ec.name: ec for ec in ret}
+
+    @property
+    def environment(self):
+        ret = None
         if hasattr(self.wfn, "pe_state"):
-            ret["pe_ptlr_correction"] = lambda view: \
-                2.0 * self.pe_energy(view.transition_dm_ao, elec_only=True)
-            ret["pe_ptss_correction"] = lambda view: \
-                self.pe_energy(view.state_diffdm_ao, elec_only=True)
+            ret = "pe"
         return ret
 
     def get_backend(self):
         return "psi4"
 
     def get_conv_tol(self):
         conv_tol = psi4.core.get_option("SCF", "E_CONVERGENCE")
@@ -235,15 +260,15 @@
         'scf_type': 'pk',
         'e_convergence': conv_tol,
         'd_convergence': conv_tol_grad,
         'maxiter': max_iter,
         'reference': "RHF",
     })
     if pe_options:
-        psi4.set_options({"pe", "true"})
+        psi4.set_options({"pe": "true"})
         psi4.set_module_options("pe", {"potfile": pe_options["potfile"]})
 
     if multiplicity != 1:
         psi4.set_options({
             'reference': "UHF",
             'maxiter': max_iter + 500,
             'soscf': 'true'
```

### Comparing `adcc-0.15.8/adcc/backends/pyscf.py` & `adcc-0.15.9/adcc/backends/pyscf.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import numpy as np
 
 from libadcc import HartreeFockProvider
 from adcc.misc import cached_property
 
 from .EriBuilder import EriBuilder
 from ..exceptions import InvalidReference
+from ..ExcitedStates import EnergyCorrection
 
 from pyscf import ao2mo, gto, scf, solvent
 
 
 class PyScfOperatorIntegralProvider:
     def __init__(self, scfres):
         self.scfres = scfres
@@ -51,14 +52,24 @@
     @cached_property
     def nabla(self):
         with self.scfres.mol.with_common_orig([0.0, 0.0, 0.0]):
             return list(
                 -1.0 * self.scfres.mol.intor('int1e_ipovlp', comp=3, hermi=2)
             )
 
+    @property
+    def pe_induction_elec(self):
+        if hasattr(self.scfres, "with_solvent"):
+            if isinstance(self.scfres.with_solvent, solvent.pol_embed.PolEmbed):
+                def pe_induction_elec_ao(dm):
+                    return self.scfres.with_solvent._exec_cppe(
+                        dm.to_ndarray(), elec_only=True
+                    )[1]
+                return pe_induction_elec_ao
+
 
 # TODO: refactor ERI builder to be more general
 # IntegralBuilder would be good
 class PyScfEriBuilder(EriBuilder):
     def __init__(self, scfres, n_orbs, n_orbs_alpha, n_alpha, n_beta, restricted):
         self.scfres = scfres
         if restricted:
@@ -112,21 +123,35 @@
     def pe_energy(self, dm, elec_only=True):
         pe_state = self.scfres.with_solvent
         e_pe, _ = pe_state.kernel(dm.to_ndarray(), elec_only=elec_only)
         return e_pe
 
     @property
     def excitation_energy_corrections(self):
-        ret = {}
+        ret = []
+        if self.environment == "pe":
+            ptlr = EnergyCorrection(
+                "pe_ptlr_correction",
+                lambda view: 2.0 * self.pe_energy(view.transition_dm_ao,
+                                                  elec_only=True)
+            )
+            ptss = EnergyCorrection(
+                "pe_ptss_correction",
+                lambda view: self.pe_energy(view.state_diffdm_ao,
+                                            elec_only=True)
+            )
+            ret.extend([ptlr, ptss])
+        return {ec.name: ec for ec in ret}
+
+    @property
+    def environment(self):
+        ret = None
         if hasattr(self.scfres, "with_solvent"):
             if isinstance(self.scfres.with_solvent, solvent.pol_embed.PolEmbed):
-                ret["pe_ptlr_correction"] = lambda view: \
-                    2.0 * self.pe_energy(view.transition_dm_ao, elec_only=True)
-                ret["pe_ptss_correction"] = lambda view: \
-                    self.pe_energy(view.state_diffdm_ao, elec_only=True)
+                ret = "pe"
         return ret
 
     def get_backend(self):
         return "pyscf"
 
     def get_conv_tol(self):
         if self.scfres.conv_tol_grad is None:
@@ -248,15 +273,15 @@
         # Disable commandline argument parsing in pyscf
         parse_arg=False,
         dump_input=False,
         verbose=0,
     )
     if pe_options:
         from pyscf.solvent import PE
-        mf = PE(scf.HF(mol), pe_options["potfile"])
+        mf = PE(scf.HF(mol), pe_options)
     else:
         mf = scf.HF(mol)
     mf.conv_tol = conv_tol
     mf.conv_tol_grad = conv_tol_grad
     mf.max_cycle = max_iter
     # since we want super tight convergence for tests,
     # tweak the options for non-RHF systems
```

### Comparing `adcc-0.15.8/adcc/backends/testing.py` & `adcc-0.15.9/adcc/backends/testing.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/backends/veloxchem.py` & `adcc-0.15.9/adcc/backends/veloxchem.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from libadcc import HartreeFockProvider
 from adcc.misc import cached_property
 
 import veloxchem as vlx
 
 from .EriBuilder import EriBuilder
 from ..exceptions import InvalidReference
+from ..ExcitedStates import EnergyCorrection
 
 from veloxchem.mpitask import MpiTask
 from veloxchem.veloxchemlib import (AngularMomentumIntegralsDriver,
                                     LinearMomentumIntegralsDriver)
 
 
 class VeloxChemOperatorIntegralProvider:
@@ -126,21 +127,28 @@
     def pe_energy(self, dm, elec_only=True):
         e_pe, _ = self.scfdrv.pe_drv.get_pe_contribution(dm.to_ndarray(),
                                                          elec_only=elec_only)
         return e_pe
 
     @property
     def excitation_energy_corrections(self):
-        ret = {}
+        ret = []
         if hasattr(self.scfdrv, "pe_drv"):
-            ret["pe_ptlr_correction"] = lambda view: \
-                2.0 * self.pe_energy(view.transition_dm_ao, elec_only=True)
-            ret["pe_ptss_correction"] = lambda view: \
-                self.pe_energy(view.state_diffdm_ao, elec_only=True)
-        return ret
+            ptlr = EnergyCorrection(
+                "pe_ptlr_correction",
+                lambda view: 2.0 * self.pe_energy(view.transition_dm_ao,
+                                                  elec_only=True)
+            )
+            ptss = EnergyCorrection(
+                "pe_ptss_correction",
+                lambda view: self.pe_energy(view.state_diffdm_ao,
+                                            elec_only=True)
+            )
+            ret.extend([ptlr, ptss])
+        return {ec.name: ec for ec in ret}
 
     def get_backend(self):
         return "veloxchem"
 
     def get_conv_tol(self):
         return self.scfdrv.conv_thresh
```

### Comparing `adcc-0.15.8/adcc/block.py` & `adcc-0.15.9/adcc/block.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/exceptions.py` & `adcc-0.15.9/adcc/exceptions.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/functions.py` & `adcc-0.15.9/adcc/functions.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/guess/__init__.py` & `adcc-0.15.9/adcc/guess/__init__.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/guess/guess_zero.py` & `adcc-0.15.9/adcc/guess/guess_zero.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/guess/guesses_from_diagonal.py` & `adcc-0.15.9/adcc/guess/guesses_from_diagonal.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/hdf5io.py` & `adcc-0.15.9/adcc/hdf5io.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/memory_pool.py` & `adcc-0.15.9/adcc/memory_pool.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/misc.py` & `adcc-0.15.9/adcc/misc.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/opt_einsum_integration.py` & `adcc-0.15.9/adcc/opt_einsum_integration.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/solver/LanczosIterator.py` & `adcc-0.15.9/adcc/solver/LanczosIterator.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/solver/SolverStateBase.py` & `adcc-0.15.9/adcc/solver/SolverStateBase.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/solver/common.py` & `adcc-0.15.9/adcc/solver/common.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/solver/conjugate_gradient.py` & `adcc-0.15.9/adcc/solver/conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/solver/davidson.py` & `adcc-0.15.9/adcc/solver/davidson.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/solver/explicit_symmetrisation.py` & `adcc-0.15.9/adcc/solver/explicit_symmetrisation.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/solver/lanczos.py` & `adcc-0.15.9/adcc/solver/lanczos.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/solver/orthogonaliser.py` & `adcc-0.15.9/adcc/solver/orthogonaliser.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/solver/power_method.py` & `adcc-0.15.9/adcc/solver/power_method.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/solver/preconditioner.py` & `adcc-0.15.9/adcc/solver/preconditioner.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/timings.py` & `adcc-0.15.9/adcc/timings.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/visualisation/ExcitationSpectrum.py` & `adcc-0.15.9/adcc/visualisation/ExcitationSpectrum.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/visualisation/Spectrum.py` & `adcc-0.15.9/adcc/visualisation/Spectrum.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/visualisation/__init__.py` & `adcc-0.15.9/adcc/visualisation/__init__.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/visualisation/shapefctns.py` & `adcc-0.15.9/adcc/visualisation/shapefctns.py`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/adcc/workflow.py` & `adcc-0.15.9/adcc/workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 from libadcc import ReferenceState
 
 from . import solver
 from .guess import (guesses_any, guesses_singlet, guesses_spin_flip,
                     guesses_triplet)
 from .LazyMp import LazyMp
-from .AdcMatrix import AdcMatrix, AdcMatrixlike
+from .AdcMatrix import AdcMatrix, AdcMatrixlike, AdcExtraTerm
 from .AdcMethod import AdcMethod
 from .exceptions import InputError
 from .ExcitedStates import ExcitedStates
 from .ReferenceState import ReferenceState as adcc_ReferenceState
 from .solver.lanczos import lanczos
 from .solver.davidson import jacobi_davidson
 from .solver.explicit_symmetrisation import (IndexSpinSymmetrisation,
@@ -43,15 +43,15 @@
 
 
 def run_adc(data_or_matrix, n_states=None, kind="any", conv_tol=None,
             eigensolver=None, guesses=None, n_guesses=None,
             n_guesses_doubles=None, output=sys.stdout, core_orbitals=None,
             frozen_core=None, frozen_virtual=None, method=None,
             n_singlets=None, n_triplets=None, n_spin_flip=None,
-            **solverargs):
+            environment=None, **solverargs):
     """Run an ADC calculation.
 
     Main entry point to run an ADC calculation. The reference to build the ADC
     calculation upon is supplied using the `data_or_matrix` argument.
     `adcc` is pretty flexible here. Possible options include:
 
         a. Hartree-Fock data from a host program, e.g. a molsturm SCF
@@ -125,14 +125,18 @@
         these see the description in :py:class:`adcc.ReferenceState`.
 
     frozen_virtual : int or list or tuple, optional
         The orbitals to select as frozen virtual orbitals (i.e. inactive
         virtuals for both the MP and ADC methods performed). For ways to define
         these see the description in :py:class:`adcc.ReferenceState`.
 
+    environment : bool or list or dict, optional
+        The keywords to specify how coupling to an environment model,
+        e.g. PE, is treated. For details see :ref:`environment`.
+
     Other parameters
     ----------------
     max_subspace : int, optional
         Maximal subspace size
     max_iter : int, optional
         Maximal number of iterations
 
@@ -187,21 +191,31 @@
     if kind == "spin_flip" and guesses is None:
         spin_change = -1
 
     # Select solver to run
     if eigensolver is None:
         eigensolver = "davidson"
 
+    # Setup environment coupling terms and energy corrections
+    ret = setup_environment(matrix, environment)
+    env_matrix_term, env_energy_corrections = ret
+    # add terms to matrix
+    if env_matrix_term:
+        matrix += env_matrix_term
+
     diagres = diagonalise_adcmatrix(
         matrix, n_states, kind, guesses=guesses, n_guesses=n_guesses,
         n_guesses_doubles=n_guesses_doubles, conv_tol=conv_tol, output=output,
         eigensolver=eigensolver, **solverargs)
     exstates = ExcitedStates(diagres)
     exstates.kind = kind
     exstates.spin_change = spin_change
+
+    # add environment corrections to excited states
+    exstates += env_energy_corrections
     return exstates
 
 
 #
 # Individual steps
 #
 def construct_adcmatrix(data_or_matrix, core_orbitals=None, frozen_core=None,
@@ -491,7 +505,79 @@
     if output is not None:
         print(f"Starting {method_name}{kstr} {solmethod_name} ...",
               file=output)
 
         def inner_callback(state, identifier):
             default_print(state, identifier, output)
         return inner_callback
+
+
+def setup_environment(matrix, environment):
+    """
+    Setup environment matrix terms and/or energy corrections.
+    Internal function called from run_adc.
+    """
+    valid_envs = ["ptss", "ptlr", "linear_response"]
+    hf = matrix.reference_state
+    if hf.environment and environment is None:
+        raise InputError(
+            "Environment found in reference state, but no environment"
+            " configuration specified. Please select from the following"
+            f" schemes: {valid_envs} or set to False."
+        )
+    elif environment and not hf.environment:
+        raise InputError(
+            "Environment specified, but no environment"
+            " was found in reference state."
+        )
+    elif not hf.environment:
+        environment = {}
+
+    convertor = {
+        bool: lambda value: {"ptss": True, "ptlr": True} if value else {},
+        list: lambda value: {k: True for k in value},
+        str: lambda value: {value: True},
+        dict: lambda value: value,
+    }
+    conversion = convertor.get(type(environment), None)
+    if conversion is None:
+        raise TypeError("Cannot convert environment parameter of type"
+                        f"'{type(environment)}' to dict.")
+    environment = conversion(environment)
+
+    if any(env not in valid_envs for env in environment):
+        raise InputError("Invalid key specified for environment."
+                         f" Valid keys are '{valid_envs}'.")
+
+    env_matrix_term = None
+    energy_corrections = []
+
+    forbidden_combinations = [
+        ["ptlr", "linear_response"],
+    ]
+    for fbc in forbidden_combinations:
+        if all(environment.get(k, False) for k in fbc):
+            raise InputError("Combination of environment schemes"
+                             f" '{fbc}' not allowed. Check the"
+                             " adcc documentation for more details.")
+
+    for pt in ["ptss", "ptlr"]:
+        if not environment.get(pt, False):
+            continue
+        hf_corr = hf.excitation_energy_corrections
+        eec_key = f"{hf.environment}_{pt}_correction"
+        if eec_key not in hf_corr:
+            raise ValueError(f"{pt} correction requested, but could not find"
+                             f" the needed function {eec_key} in"
+                             f" reference state from backend {hf.backend}.")
+        energy_corrections.append(hf_corr[eec_key])
+    if environment.get("linear_response", False):
+        from adcc.adc_pp import environment as adcpp_env
+        block_key = f"block_ph_ph_0_{hf.environment}"
+        if not hasattr(adcpp_env, block_key):
+            raise NotImplementedError("Matrix term for linear response coupling"
+                                      f" with solvent {hf.environment}"
+                                      " not implemented.")
+        block_fun = getattr(adcpp_env, block_key)
+        env_matrix_term = AdcExtraTerm(matrix, {'ph_ph': block_fun})
+
+    return env_matrix_term, energy_corrections
```

### Comparing `adcc-0.15.8/adcc.egg-info/PKG-INFO` & `adcc-0.15.9/adcc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adcc
-Version: 0.15.8
+Version: 0.15.9
 Summary: adcc:  Seamlessly connect your host program to ADC
 Home-page: https://adc-connect.org
 Author: Michael F. Herbst, Maximilian Scheurer
 Author-email: developers@adc-connect.org
 License: GPL v3
 Project-URL: Source, https://github.com/adc-connect/adcc
 Project-URL: Issues, https://github.com/adc-connect/adcc/issues
```

### Comparing `adcc-0.15.8/adcc.egg-info/SOURCES.txt` & `adcc-0.15.9/adcc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 adcc.egg-info/PKG-INFO
 adcc.egg-info/SOURCES.txt
 adcc.egg-info/dependency_links.txt
 adcc.egg-info/not-zip-safe
 adcc.egg-info/requires.txt
 adcc.egg-info/top_level.txt
 adcc/adc_pp/__init__.py
+adcc/adc_pp/environment.py
 adcc/adc_pp/matrix.py
 adcc/adc_pp/modified_transition_moments.py
 adcc/adc_pp/state2state_transition_dm.py
 adcc/adc_pp/state_diffdm.py
 adcc/adc_pp/transition_dm.py
 adcc/adc_pp/util.py
 adcc/backends/EriBuilder.py
```

### Comparing `adcc-0.15.8/libadcc/AdcMemory.cc` & `adcc-0.15.9/libadcc/AdcMemory.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/AdcMemory.hh` & `adcc-0.15.9/libadcc/AdcMemory.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/AxisInfo.cc` & `adcc-0.15.9/libadcc/AxisInfo.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/AxisInfo.hh` & `adcc-0.15.9/libadcc/AxisInfo.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/HartreeFockSolution_i.hh` & `adcc-0.15.9/libadcc/HartreeFockSolution_i.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/MoIndexTranslation.cc` & `adcc-0.15.9/libadcc/MoIndexTranslation.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/MoIndexTranslation.hh` & `adcc-0.15.9/libadcc/MoIndexTranslation.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/MoSpaces/construct_blocks.cc` & `adcc-0.15.9/libadcc/MoSpaces/construct_blocks.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/MoSpaces/construct_blocks.hh` & `adcc-0.15.9/libadcc/MoSpaces/construct_blocks.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/MoSpaces/setup_point_group_table.cc` & `adcc-0.15.9/libadcc/MoSpaces/setup_point_group_table.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/MoSpaces/setup_point_group_table.hh` & `adcc-0.15.9/libadcc/MoSpaces/setup_point_group_table.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/MoSpaces.cc` & `adcc-0.15.9/libadcc/MoSpaces.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/MoSpaces.hh` & `adcc-0.15.9/libadcc/MoSpaces.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/ReferenceState.cc` & `adcc-0.15.9/libadcc/ReferenceState.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/ReferenceState.hh` & `adcc-0.15.9/libadcc/ReferenceState.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/Symmetry.cc` & `adcc-0.15.9/libadcc/Symmetry.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/Symmetry.hh` & `adcc-0.15.9/libadcc/Symmetry.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/Tensor.cc` & `adcc-0.15.9/libadcc/Tensor.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/Tensor.hh` & `adcc-0.15.9/libadcc/Tensor.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/TensorImpl/ExpressionTree.cc` & `adcc-0.15.9/libadcc/TensorImpl/ExpressionTree.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/TensorImpl/ExpressionTree.hh` & `adcc-0.15.9/libadcc/TensorImpl/ExpressionTree.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/TensorImpl/as_bispace.cc` & `adcc-0.15.9/libadcc/TensorImpl/as_bispace.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/TensorImpl/as_bispace.hh` & `adcc-0.15.9/libadcc/TensorImpl/as_bispace.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/TensorImpl/as_lt_symmetry.cc` & `adcc-0.15.9/libadcc/TensorImpl/as_lt_symmetry.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/TensorImpl/as_lt_symmetry.hh` & `adcc-0.15.9/libadcc/TensorImpl/as_lt_symmetry.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/TensorImpl/get_block_starts.cc` & `adcc-0.15.9/libadcc/TensorImpl/get_block_starts.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/TensorImpl/get_block_starts.hh` & `adcc-0.15.9/libadcc/TensorImpl/get_block_starts.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/TensorImpl.cc` & `adcc-0.15.9/libadcc/TensorImpl.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/TensorImpl.hh` & `adcc-0.15.9/libadcc/TensorImpl.hh`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         std::function<void(const std::vector<std::pair<size_t, size_t>>&, scalar_type*)>
               generator,
         scalar_type tolerance, bool symmetry_check) override;
   std::string describe_symmetry() const override;
   std::string describe_expression(std::string stage = "unoptimised") const override;
 
   /** Convert object to btensor for use in libtensor functions. */
-  explicit operator libtensor::btensor<N, scalar_type> &() { return *libtensor_ptr(); }
+  explicit operator libtensor::btensor<N, scalar_type>&() { return *libtensor_ptr(); }
 
   /** Return inner btensor object
    *
    * \note This is an advanced function. Use with care, since this can corrupt the
    *       internal state of the Tensor object.
    */
   std::shared_ptr<libtensor::btensor<N, scalar_type>> libtensor_ptr() {
```

### Comparing `adcc-0.15.8/libadcc/ThreadPool.cc` & `adcc-0.15.9/libadcc/ThreadPool.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/ThreadPool.hh` & `adcc-0.15.9/libadcc/ThreadPool.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/Timer.cc` & `adcc-0.15.9/libadcc/Timer.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/Timer.hh` & `adcc-0.15.9/libadcc/Timer.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/amplitude_vector_enforce_spin_kind.cc` & `adcc-0.15.9/libadcc/amplitude_vector_enforce_spin_kind.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/amplitude_vector_enforce_spin_kind.hh` & `adcc-0.15.9/libadcc/amplitude_vector_enforce_spin_kind.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/config.hh` & `adcc-0.15.9/libadcc/config.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/exceptions.hh` & `adcc-0.15.9/libadcc/exceptions.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/fill_pp_doubles_guesses.cc` & `adcc-0.15.9/libadcc/fill_pp_doubles_guesses.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/fill_pp_doubles_guesses.hh` & `adcc-0.15.9/libadcc/fill_pp_doubles_guesses.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/guess/adc_guess_d.cc` & `adcc-0.15.9/libadcc/guess/adc_guess_d.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/guess/adc_guess_d.hh` & `adcc-0.15.9/libadcc/guess/adc_guess_d.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/guess/index_group_d.cc` & `adcc-0.15.9/libadcc/guess/index_group_d.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/guess/index_group_d.hh` & `adcc-0.15.9/libadcc/guess/index_group_d.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/import_eri.cc` & `adcc-0.15.9/libadcc/import_eri.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/import_eri.hh` & `adcc-0.15.9/libadcc/import_eri.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/make_symmetry.cc` & `adcc-0.15.9/libadcc/make_symmetry.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/make_symmetry.hh` & `adcc-0.15.9/libadcc/make_symmetry.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/pyiface/ExportAdcc.cc` & `adcc-0.15.9/libadcc/pyiface/ExportAdcc.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/pyiface/export_AdcMemory.cc` & `adcc-0.15.9/libadcc/pyiface/export_AdcMemory.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/pyiface/export_HartreeFockProvider.cc` & `adcc-0.15.9/libadcc/pyiface/export_HartreeFockProvider.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/pyiface/export_MoIndexTranslation.cc` & `adcc-0.15.9/libadcc/pyiface/export_MoIndexTranslation.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/pyiface/export_MoSpaces.cc` & `adcc-0.15.9/libadcc/pyiface/export_MoSpaces.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/pyiface/export_ReferenceState.cc` & `adcc-0.15.9/libadcc/pyiface/export_ReferenceState.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/pyiface/export_Symmetry.cc` & `adcc-0.15.9/libadcc/pyiface/export_Symmetry.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/pyiface/export_Tensor.cc` & `adcc-0.15.9/libadcc/pyiface/export_Tensor.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/pyiface/export_adc_pp.cc` & `adcc-0.15.9/libadcc/pyiface/export_adc_pp.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/pyiface/export_threading.cc` & `adcc-0.15.9/libadcc/pyiface/export_threading.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/pyiface/hartree_fock_solution_hack.hh` & `adcc-0.15.9/libadcc/pyiface/hartree_fock_solution_hack.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/pyiface/util.cc` & `adcc-0.15.9/libadcc/pyiface/util.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/pyiface/util.hh` & `adcc-0.15.9/libadcc/pyiface/util.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/shape_to_string.cc` & `adcc-0.15.9/libadcc/shape_to_string.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/shape_to_string.hh` & `adcc-0.15.9/libadcc/shape_to_string.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/tests/HFSolutionMock.hh` & `adcc-0.15.9/libadcc/tests/HFSolutionMock.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/tests/MoIndexTranslationTest.cc` & `adcc-0.15.9/libadcc/tests/MoIndexTranslationTest.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/tests/MoSpacesTest.cc` & `adcc-0.15.9/libadcc/tests/MoSpacesTest.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/tests/TensorTest.cc` & `adcc-0.15.9/libadcc/tests/TensorTest.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/tests/TensorTestData.cc` & `adcc-0.15.9/libadcc/tests/TensorTestData.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/tests/TensorTestData.hh` & `adcc-0.15.9/libadcc/tests/TensorTestData.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/tests/main.cc` & `adcc-0.15.9/libadcc/tests/main.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/tests/output_tensor.hh` & `adcc-0.15.9/libadcc/tests/output_tensor.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/tests/random_tensor.cc` & `adcc-0.15.9/libadcc/tests/random_tensor.cc`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/tests/random_tensor.hh` & `adcc-0.15.9/libadcc/tests/random_tensor.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/libadcc/tests/wrap_libtensor.hh` & `adcc-0.15.9/libadcc/tests/wrap_libtensor.hh`

 * *Files identical despite different names*

### Comparing `adcc-0.15.8/setup.cfg` & `adcc-0.15.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.15.8
+current_version = 0.15.9
 commit = True
 tag = True
 
 [bumpversion:file:adcc/__init__.py]
 
 [bumpversion:file:setup.py]
```

### Comparing `adcc-0.15.8/setup.py` & `adcc-0.15.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,15 +456,15 @@
 
 #
 # Main setup code
 #
 def is_conda_build():
     return (
         os.environ.get("CONDA_BUILD", None) == "1"
-        or os.environ.get("CONDA_EXE", None)
+        or os.environ.get("CONDA_EXE", None) is not None
     )
 
 
 def adccsetup(*args, **kwargs):
     """Wrapper around setup, displaying a link to adc-connect.org on any error."""
     if is_conda_build():
         kwargs.pop("install_requires")
@@ -504,15 +504,15 @@
     license="GPL v3",
     url="https://adc-connect.org",
     project_urls={
         "Source": "https://github.com/adc-connect/adcc",
         "Issues": "https://github.com/adc-connect/adcc/issues",
     },
     #
-    version="0.15.8",
+    version="0.15.9",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "License :: Free For Educational Use",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Chemistry",
         "Topic :: Education",
```


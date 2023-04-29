# Comparing `tmp/dlplan-0.2.5.tar.gz` & `tmp/dlplan-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlplan-0.2.5.tar", last modified: Sat Apr 29 10:07:54 2023, max compression
+gzip compressed data, was "dlplan-0.2.6.tar", last modified: Sat Apr 29 13:16:56 2023, max compression
```

## Comparing `dlplan-0.2.5.tar` & `dlplan-0.2.6.tar`

### file list

```diff
@@ -1,414 +1,414 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.119536 dlplan-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-29 10:07:43.000000 dlplan-0.2.5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-04-29 10:07:43.000000 dlplan-0.2.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-29 10:07:43.000000 dlplan-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-29 10:07:54.119536 dlplan-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-29 10:07:43.000000 dlplan-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.047536 dlplan-0.2.5/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.051536 dlplan-0.2.5/api/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-29 10:07:43.000000 dlplan-0.2.5/api/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.055536 dlplan-0.2.5/api/python/src/
--rw-r--r--   0 runner    (1001) docker     (123)    17252 2023-04-29 10:07:43.000000 dlplan-0.2.5/api/python/src/core.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.055536 dlplan-0.2.5/api/python/src/dlplan/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-29 10:07:43.000000 dlplan-0.2.5/api/python/src/dlplan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.055536 dlplan-0.2.5/api/python/src/dlplan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-29 10:07:53.000000 dlplan-0.2.5/api/python/src/dlplan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-04-29 10:07:54.000000 dlplan-0.2.5/api/python/src/dlplan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:07:53.000000 dlplan-0.2.5/api/python/src/dlplan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:07:53.000000 dlplan-0.2.5/api/python/src/dlplan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-29 10:07:53.000000 dlplan-0.2.5/api/python/src/dlplan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-29 10:07:53.000000 dlplan-0.2.5/api/python/src/dlplan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-04-29 10:07:43.000000 dlplan-0.2.5/api/python/src/generator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-29 10:07:43.000000 dlplan-0.2.5/api/python/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-29 10:07:43.000000 dlplan-0.2.5/api/python/src/novelty.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-29 10:07:43.000000 dlplan-0.2.5/api/python/src/policy.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-29 10:07:43.000000 dlplan-0.2.5/api/python/src/state_space.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-29 10:07:43.000000 dlplan-0.2.5/api/python/src/weisfeiler_lehman.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.055536 dlplan-0.2.5/api/python/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:43.000000 dlplan-0.2.5/api/python/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-29 10:07:43.000000 dlplan-0.2.5/api/python/test/test_barman.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-04-29 10:07:43.000000 dlplan-0.2.5/api/python/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-04-29 10:07:43.000000 dlplan-0.2.5/api/python/test/test_generate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.055536 dlplan-0.2.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.055536 dlplan-0.2.5/examples/core/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/core/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.055536 dlplan-0.2.5/examples/core/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/core/__pycache__/tarski.cpython-36.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/core/__pycache__/tarski.cpython-37.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/core/core.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     2438 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/core/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.055536 dlplan-0.2.5/examples/generator/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/generator/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/generator/generator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/generator/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.055536 dlplan-0.2.5/examples/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/policy/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/policy/policy.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     1925 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/policy/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.055536 dlplan-0.2.5/examples/state_space/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/state_space/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.059536 dlplan-0.2.5/examples/state_space/delivery/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/state_space/delivery/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/state_space/delivery/delivery.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/state_space/delivery/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/state_space/delivery/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/state_space/delivery/instance_2_1_0.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-29 10:07:43.000000 dlplan-0.2.5/examples/state_space/delivery/instance_2_2_0.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.059536 dlplan-0.2.5/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-29 10:07:43.000000 dlplan-0.2.5/experiments/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-29 10:07:43.000000 dlplan-0.2.5/experiments/experiment_generator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-29 10:07:43.000000 dlplan-0.2.5/experiments/experiment_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5147 2023-04-29 10:07:43.000000 dlplan-0.2.5/experiments/experiment_runner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2891 2023-04-29 10:07:43.000000 dlplan-0.2.5/experiments/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.047536 dlplan-0.2.5/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.059536 dlplan-0.2.5/include/dlplan/
--rw-r--r--   0 runner    (1001) docker     (123)    25657 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/generator.h
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/novelty.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.063536 dlplan-0.2.5/include/dlplan/phmap/
--rw-r--r--   0 runner    (1001) docker     (123)   166554 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/phmap/btree.h
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/phmap/meminfo.h
--rw-r--r--   0 runner    (1001) docker     (123)   186642 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/phmap/phmap.h
--rw-r--r--   0 runner    (1001) docker     (123)   180847 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/phmap/phmap_base.h
--rw-r--r--   0 runner    (1001) docker     (123)    22491 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/phmap/phmap_bits.h
--rw-r--r--   0 runner    (1001) docker     (123)    28525 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/phmap/phmap_config.h
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/phmap/phmap_dump.h
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/phmap/phmap_fwd_decl.h
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/phmap/phmap_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/policy.h
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/state_space.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.063536 dlplan-0.2.5/include/dlplan/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/utils/cache.h
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/utils/dynamic_bitset.h
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/utils/hashing.h
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/utils/pimpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-29 10:07:43.000000 dlplan-0.2.5/include/dlplan/weisfeiler_lehman.h
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-29 10:07:43.000000 dlplan-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-29 10:07:43.000000 dlplan-0.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 10:07:54.119536 dlplan-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-29 10:07:43.000000 dlplan-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.063536 dlplan-0.2.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.063536 dlplan-0.2.5/src/core/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/atom.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/cache.h
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/constant.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25107 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/core.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/element_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/element_factory.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.063536 dlplan-0.2.5/src/core/elements/
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/boolean.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.067536 dlplan-0.2.5/src/core/elements/booleans/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/booleans/empty.h
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/booleans/inclusion.h
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/booleans/nullary.h
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/concept.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.067536 dlplan-0.2.5/src/core/elements/concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/concepts/all.h
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/concepts/and.h
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/concepts/bot.h
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/concepts/diff.h
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/concepts/equal.h
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/concepts/not.h
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/concepts/one_of.h
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/concepts/or.h
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/concepts/primitive.h
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/concepts/projection.h
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/concepts/some.h
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/concepts/subset.h
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/concepts/top.h
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/element.h
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/numerical.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.067536 dlplan-0.2.5/src/core/elements/numericals/
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/numericals/concept_distance.h
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/numericals/count.h
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/numericals/role_distance.h
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/numericals/sum_concept_distance.h
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/numericals/sum_role_distance.h
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/role.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.071536 dlplan-0.2.5/src/core/elements/roles/
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/roles/and.h
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/roles/compose.h
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/roles/diff.h
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/roles/identity.h
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/roles/inverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/roles/not.h
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/roles/or.h
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/roles/primitive.h
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/roles/restrict.h
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/roles/top.h
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/roles/transitive_closure.h
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/roles/transitive_reflexive_closure.h
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/types.h
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/elements/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/instance_info.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/object.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.071536 dlplan-0.2.5/src/core/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expression_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expression_factory.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.071536 dlplan-0.2.5/src/core/parser/expressions/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/boolean.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.071536 dlplan-0.2.5/src/core/parser/expressions/booleans/
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/booleans/empty.h
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/booleans/inclusion.h
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/booleans/nullary.h
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/concept.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.075536 dlplan-0.2.5/src/core/parser/expressions/concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/concepts/all.h
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/concepts/and.h
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/concepts/bot.h
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/concepts/diff.h
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/concepts/equal.h
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/concepts/not.h
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/concepts/one_of.h
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/concepts/or.h
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/concepts/primitive.h
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/concepts/projection.h
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/concepts/some.h
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/concepts/subset.h
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/concepts/top.h
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/expression.h
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/numerical.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.075536 dlplan-0.2.5/src/core/parser/expressions/numericals/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/numericals/concept_distance.h
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/numericals/count.h
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/numericals/role_distance.h
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/numericals/sum_concept_distance.h
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/numericals/sum_role_distance.h
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/role.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.075536 dlplan-0.2.5/src/core/parser/expressions/roles/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/roles/and.h
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/roles/compose.h
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/roles/diff.h
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/roles/identity.h
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/roles/inverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/roles/not.h
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/roles/or.h
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/roles/primitive.h
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/roles/restrict.h
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/roles/top.h
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/roles/transitive_closure.h
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/expressions/roles/transitive_reflexive_closure.h
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/parser.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/parser.h
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/types.h
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/parser/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/predicate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/state.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/core/vocabulary_info.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.079536 dlplan-0.2.5/src/generator/
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/feature_generator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/feature_generator.h
--rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/generator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/generator_data.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.079536 dlplan-0.2.5/src/generator/rules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.079536 dlplan-0.2.5/src/generator/rules/booleans/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/booleans/empty.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/booleans/empty.h
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/booleans/inclusion.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/booleans/inclusion.h
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/booleans/nullary.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/booleans/nullary.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.083536 dlplan-0.2.5/src/generator/rules/concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/all.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/all.h
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/and.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/and.h
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/bot.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/bot.h
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/diff.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/diff.h
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/equal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/equal.h
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/not.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/not.h
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/one_of.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/one_of.h
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/or.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/or.h
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/primitive.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/primitive.h
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/projection.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/projection.h
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/some.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/some.h
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/subset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/subset.h
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/top.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/concepts/top.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.083536 dlplan-0.2.5/src/generator/rules/numericals/
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/numericals/concept_distance.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/numericals/concept_distance.h
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/numericals/count.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/numericals/count.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.087536 dlplan-0.2.5/src/generator/rules/roles/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/and.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/and.h
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/compose.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/compose.h
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/diff.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/diff.h
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/identity.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/identity.h
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/inverse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/inverse.h
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/not.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/not.h
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/or.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/or.h
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/primitive.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/primitive.h
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/restrict.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/restrict.h
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/top.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/top.h
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/transitive_closure.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/transitive_closure.h
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/transitive_reflexive_closure.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/roles/transitive_reflexive_closure.h
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/generator/rules/rule.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.087536 dlplan-0.2.5/src/novelty/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/novelty/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/novelty/novelty.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/novelty/novelty_base.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/novelty/novelty_table.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/novelty/tuple_graph.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/novelty/tuple_index_generator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/novelty/tuple_node.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.091536 dlplan-0.2.5/src/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/cache.h
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/condition.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/condition.h
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/effect.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/effect.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.091536 dlplan-0.2.5/src/policy/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/parser/expression_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/parser/expression_factory.h
--rw-r--r--   0 runner    (1001) docker     (123)    16349 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/parser/expressions.h
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/parser/parser.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/parser/parser.h
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/parser/types.h
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/parser/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/parser/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/policy.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/policy_builder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/policy_builder.h
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/policy_impl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/policy_minimizer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/reader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/reader.h
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/writer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/policy/writer.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.095536 dlplan-0.2.5/src/state_space/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/state_space/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/state_space/generator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/state_space/generator.h
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/state_space/reader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/state_space/reader.h
--rw-r--r--   0 runner    (1001) docker     (123)    13425 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/state_space/state_space.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.095536 dlplan-0.2.5/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/MurmurHash3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/MurmurHash3.h
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/collections.h
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/command.h
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/countdown_timer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/countdown_timer.h
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/logging.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/math.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/math.h
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/memory.h
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/set_operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/sha-256.c
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/sha-256.h
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/system.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/system.h
--rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/threadpool.h
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/timer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/timer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/utils/tokenizer.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.095536 dlplan-0.2.5/src/weisfeiler_lehman/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/weisfeiler_lehman/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/weisfeiler_lehman/color.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/weisfeiler_lehman/color.h
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-29 10:07:43.000000 dlplan-0.2.5/src/weisfeiler_lehman/weisfeiler_lehman.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.095536 dlplan-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.107536 dlplan-0.2.5/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/b_empty.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/b_inclusion.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/b_nullary.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/c_all.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/c_and.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/c_bot.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/c_diff.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/c_equal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/c_not.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/c_one_of.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/c_or.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/c_primitive.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/c_projection.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/c_some.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/c_subset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/c_top.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/core.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/multi_instance.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/n_concept_distance.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/n_count.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/n_role_distance.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/n_sum_concept_distance.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/n_sum_role_distance.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/r_and.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/r_compose.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/r_diff.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/r_identity.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/r_inverse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/r_not.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/r_or.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/r_primitive.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/r_restrict.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/r_top.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/r_transitive_closure.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/core/r_transitive_reflexive_closure.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.107536 dlplan-0.2.5/tests/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/generator/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.111536 dlplan-0.2.5/tests/generator/delivery/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/generator/delivery/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/generator/delivery/delivery.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/generator/delivery/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/generator/delivery/instance_2_2_0.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/generator/delivery/instance_4_2_29.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.111536 dlplan-0.2.5/tests/novelty/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/novelty/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.111536 dlplan-0.2.5/tests/novelty/gripper/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/novelty/gripper/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/novelty/gripper/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/novelty/gripper/gripper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/novelty/gripper/p-1-0.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/novelty/tuple_index_generator.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.115537 dlplan-0.2.5/tests/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/policy/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/policy/policy_builder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9811 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/policy/policy_minimizer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/policy/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/policy/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.115537 dlplan-0.2.5/tests/state_space/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/state_space/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.115537 dlplan-0.2.5/tests/state_space/gripper/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/state_space/gripper/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/state_space/gripper/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/state_space/gripper/gripper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/state_space/gripper/p-1-0.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:07:54.119536 dlplan-0.2.5/tests/state_space/spanner/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/state_space/spanner/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/state_space/spanner/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/state_space/spanner/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-29 10:07:43.000000 dlplan-0.2.5/tests/state_space/spanner/spanner.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-29 10:07:43.000000 dlplan-0.2.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.509299 dlplan-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-29 13:16:43.000000 dlplan-0.2.6/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-04-29 13:16:43.000000 dlplan-0.2.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-29 13:16:43.000000 dlplan-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-29 13:16:56.509299 dlplan-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-29 13:16:43.000000 dlplan-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.473299 dlplan-0.2.6/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.473299 dlplan-0.2.6/api/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-29 13:16:43.000000 dlplan-0.2.6/api/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.477299 dlplan-0.2.6/api/python/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    17252 2023-04-29 13:16:43.000000 dlplan-0.2.6/api/python/src/core.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.477299 dlplan-0.2.6/api/python/src/dlplan/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-29 13:16:43.000000 dlplan-0.2.6/api/python/src/dlplan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.477299 dlplan-0.2.6/api/python/src/dlplan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-29 13:16:56.000000 dlplan-0.2.6/api/python/src/dlplan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-04-29 13:16:56.000000 dlplan-0.2.6/api/python/src/dlplan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:16:56.000000 dlplan-0.2.6/api/python/src/dlplan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:16:56.000000 dlplan-0.2.6/api/python/src/dlplan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-29 13:16:56.000000 dlplan-0.2.6/api/python/src/dlplan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-29 13:16:56.000000 dlplan-0.2.6/api/python/src/dlplan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-04-29 13:16:43.000000 dlplan-0.2.6/api/python/src/generator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-29 13:16:43.000000 dlplan-0.2.6/api/python/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-29 13:16:43.000000 dlplan-0.2.6/api/python/src/novelty.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-29 13:16:43.000000 dlplan-0.2.6/api/python/src/policy.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-29 13:16:43.000000 dlplan-0.2.6/api/python/src/state_space.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-29 13:16:43.000000 dlplan-0.2.6/api/python/src/weisfeiler_lehman.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.477299 dlplan-0.2.6/api/python/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:43.000000 dlplan-0.2.6/api/python/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-29 13:16:43.000000 dlplan-0.2.6/api/python/test/test_barman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-04-29 13:16:43.000000 dlplan-0.2.6/api/python/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-04-29 13:16:43.000000 dlplan-0.2.6/api/python/test/test_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.477299 dlplan-0.2.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.477299 dlplan-0.2.6/examples/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/core/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.477299 dlplan-0.2.6/examples/core/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/core/__pycache__/tarski.cpython-36.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/core/__pycache__/tarski.cpython-37.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/core/core.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2438 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/core/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.477299 dlplan-0.2.6/examples/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/generator/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/generator/generator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/generator/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.477299 dlplan-0.2.6/examples/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/policy/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/policy/policy.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1925 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/policy/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.477299 dlplan-0.2.6/examples/state_space/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/state_space/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.477299 dlplan-0.2.6/examples/state_space/delivery/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/state_space/delivery/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/state_space/delivery/delivery.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/state_space/delivery/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/state_space/delivery/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/state_space/delivery/instance_2_1_0.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-29 13:16:43.000000 dlplan-0.2.6/examples/state_space/delivery/instance_2_2_0.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.477299 dlplan-0.2.6/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-29 13:16:43.000000 dlplan-0.2.6/experiments/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-29 13:16:43.000000 dlplan-0.2.6/experiments/experiment_generator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-29 13:16:43.000000 dlplan-0.2.6/experiments/experiment_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5147 2023-04-29 13:16:43.000000 dlplan-0.2.6/experiments/experiment_runner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2891 2023-04-29 13:16:43.000000 dlplan-0.2.6/experiments/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.473299 dlplan-0.2.6/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.481299 dlplan-0.2.6/include/dlplan/
+-rw-r--r--   0 runner    (1001) docker     (123)    25657 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/novelty.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.481299 dlplan-0.2.6/include/dlplan/phmap/
+-rw-r--r--   0 runner    (1001) docker     (123)   166554 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/phmap/btree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/phmap/meminfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)   186642 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/phmap/phmap.h
+-rw-r--r--   0 runner    (1001) docker     (123)   180847 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/phmap/phmap_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22491 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/phmap/phmap_bits.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28525 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/phmap/phmap_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/phmap/phmap_dump.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/phmap/phmap_fwd_decl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/phmap/phmap_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/policy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/state_space.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.481299 dlplan-0.2.6/include/dlplan/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/utils/cache.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/utils/dynamic_bitset.h
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/utils/hashing.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/utils/pimpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-29 13:16:43.000000 dlplan-0.2.6/include/dlplan/weisfeiler_lehman.h
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-29 13:16:43.000000 dlplan-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-29 13:16:43.000000 dlplan-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 13:16:56.509299 dlplan-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-29 13:16:43.000000 dlplan-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.481299 dlplan-0.2.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.481299 dlplan-0.2.6/src/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/atom.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/cache.h
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/constant.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25107 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/core.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/element_factory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/element_factory.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.481299 dlplan-0.2.6/src/core/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/boolean.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.485299 dlplan-0.2.6/src/core/elements/booleans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/booleans/empty.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/booleans/inclusion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/booleans/nullary.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/concept.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.485299 dlplan-0.2.6/src/core/elements/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/concepts/all.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/concepts/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/concepts/bot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/concepts/diff.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/concepts/equal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/concepts/not.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/concepts/one_of.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/concepts/or.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/concepts/primitive.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/concepts/projection.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/concepts/some.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/concepts/subset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/concepts/top.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/element.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/numerical.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.485299 dlplan-0.2.6/src/core/elements/numericals/
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/numericals/concept_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/numericals/count.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/numericals/role_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/numericals/sum_concept_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/numericals/sum_role_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/role.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.485299 dlplan-0.2.6/src/core/elements/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/roles/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/roles/compose.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/roles/diff.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/roles/identity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/roles/inverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/roles/not.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/roles/or.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/roles/primitive.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/roles/restrict.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/roles/top.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/roles/transitive_closure.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/roles/transitive_reflexive_closure.h
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/elements/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/instance_info.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/object.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.485299 dlplan-0.2.6/src/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expression_factory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expression_factory.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.485299 dlplan-0.2.6/src/core/parser/expressions/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/boolean.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.489299 dlplan-0.2.6/src/core/parser/expressions/booleans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/booleans/empty.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/booleans/inclusion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/booleans/nullary.h
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/concept.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.489299 dlplan-0.2.6/src/core/parser/expressions/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/concepts/all.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/concepts/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/concepts/bot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/concepts/diff.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/concepts/equal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/concepts/not.h
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/concepts/one_of.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/concepts/or.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/concepts/primitive.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/concepts/projection.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/concepts/some.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/concepts/subset.h
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/concepts/top.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/expression.h
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/numerical.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.489299 dlplan-0.2.6/src/core/parser/expressions/numericals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/numericals/concept_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/numericals/count.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/numericals/role_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/numericals/sum_concept_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/numericals/sum_role_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/role.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.489299 dlplan-0.2.6/src/core/parser/expressions/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/roles/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/roles/compose.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/roles/diff.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/roles/identity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/roles/inverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/roles/not.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/roles/or.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/roles/primitive.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/roles/restrict.h
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/roles/top.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/roles/transitive_closure.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/expressions/roles/transitive_reflexive_closure.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/parser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/parser/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/predicate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/core/vocabulary_info.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.489299 dlplan-0.2.6/src/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/feature_generator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/feature_generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/generator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/generator_data.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.489299 dlplan-0.2.6/src/generator/rules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.493299 dlplan-0.2.6/src/generator/rules/booleans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/booleans/empty.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/booleans/empty.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/booleans/inclusion.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/booleans/inclusion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/booleans/nullary.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/booleans/nullary.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.493299 dlplan-0.2.6/src/generator/rules/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/all.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/all.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/and.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/bot.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/bot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/diff.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/diff.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/equal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/equal.h
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/not.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/not.h
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/one_of.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/one_of.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/or.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/or.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/primitive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/primitive.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/projection.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/projection.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/some.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/some.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/subset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/subset.h
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/top.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/concepts/top.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.493299 dlplan-0.2.6/src/generator/rules/numericals/
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/numericals/concept_distance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/numericals/concept_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/numericals/count.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/numericals/count.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.497299 dlplan-0.2.6/src/generator/rules/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/and.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/compose.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/compose.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/diff.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/diff.h
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/identity.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/identity.h
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/inverse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/inverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/not.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/not.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/or.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/or.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/primitive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/primitive.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/restrict.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/restrict.h
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/top.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/top.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/transitive_closure.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/transitive_closure.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/transitive_reflexive_closure.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/roles/transitive_reflexive_closure.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/generator/rules/rule.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.497299 dlplan-0.2.6/src/novelty/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/novelty/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/novelty/novelty.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/novelty/novelty_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/novelty/novelty_table.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/novelty/tuple_graph.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/novelty/tuple_index_generator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/novelty/tuple_node.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.497299 dlplan-0.2.6/src/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/cache.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/condition.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/condition.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/effect.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/effect.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.501299 dlplan-0.2.6/src/policy/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/parser/expression_factory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/parser/expression_factory.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16349 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/parser/expressions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/parser/parser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/parser/parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/parser/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/parser/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/parser/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/policy.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/policy_builder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/policy_builder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/policy_impl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/policy_minimizer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/reader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/policy/writer.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.501299 dlplan-0.2.6/src/state_space/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/state_space/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/state_space/generator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/state_space/generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/state_space/reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/state_space/reader.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13425 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/state_space/state_space.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.501299 dlplan-0.2.6/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/MurmurHash3.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/MurmurHash3.h
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/collections.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/command.h
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/countdown_timer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/countdown_timer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/math.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/math.h
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/memory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/set_operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/sha-256.c
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/sha-256.h
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/system.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/system.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/threadpool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/timer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/timer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/utils/tokenizer.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.501299 dlplan-0.2.6/src/weisfeiler_lehman/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/weisfeiler_lehman/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/weisfeiler_lehman/color.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/weisfeiler_lehman/color.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-29 13:16:43.000000 dlplan-0.2.6/src/weisfeiler_lehman/weisfeiler_lehman.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.501299 dlplan-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.505299 dlplan-0.2.6/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/b_empty.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/b_inclusion.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/b_nullary.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/c_all.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/c_and.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/c_bot.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/c_diff.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/c_equal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/c_not.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/c_one_of.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/c_or.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/c_primitive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/c_projection.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/c_some.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/c_subset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/c_top.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/core.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/multi_instance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/n_concept_distance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/n_count.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/n_role_distance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/n_sum_concept_distance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/n_sum_role_distance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/r_and.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/r_compose.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/r_diff.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/r_identity.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/r_inverse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/r_not.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/r_or.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/r_primitive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/r_restrict.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/r_top.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/r_transitive_closure.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/core/r_transitive_reflexive_closure.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.505299 dlplan-0.2.6/tests/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/generator/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.505299 dlplan-0.2.6/tests/generator/delivery/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/generator/delivery/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/generator/delivery/delivery.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/generator/delivery/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/generator/delivery/instance_2_2_0.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/generator/delivery/instance_4_2_29.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.505299 dlplan-0.2.6/tests/novelty/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/novelty/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.505299 dlplan-0.2.6/tests/novelty/gripper/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/novelty/gripper/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/novelty/gripper/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/novelty/gripper/gripper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/novelty/gripper/p-1-0.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/novelty/tuple_index_generator.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.505299 dlplan-0.2.6/tests/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/policy/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/policy/policy_builder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9811 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/policy/policy_minimizer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/policy/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/policy/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.509299 dlplan-0.2.6/tests/state_space/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/state_space/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.509299 dlplan-0.2.6/tests/state_space/gripper/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/state_space/gripper/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/state_space/gripper/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/state_space/gripper/gripper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/state_space/gripper/p-1-0.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:16:56.509299 dlplan-0.2.6/tests/state_space/spanner/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/state_space/spanner/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/state_space/spanner/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/state_space/spanner/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-29 13:16:43.000000 dlplan-0.2.6/tests/state_space/spanner/spanner.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-29 13:16:43.000000 dlplan-0.2.6/tox.ini
```

### Comparing `dlplan-0.2.5/CMakeLists.txt` & `dlplan-0.2.6/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/LICENSE.md` & `dlplan-0.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/README.md` & `dlplan-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/api/python/CMakeLists.txt` & `dlplan-0.2.6/api/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/api/python/src/core.cpp` & `dlplan-0.2.6/api/python/src/core.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/api/python/src/dlplan.egg-info/SOURCES.txt` & `dlplan-0.2.6/api/python/src/dlplan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/api/python/src/generator.cpp` & `dlplan-0.2.6/api/python/src/generator.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/api/python/src/main.cpp` & `dlplan-0.2.6/api/python/src/main.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/api/python/src/novelty.cpp` & `dlplan-0.2.6/api/python/src/novelty.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/api/python/src/policy.cpp` & `dlplan-0.2.6/api/python/src/policy.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/api/python/src/state_space.cpp` & `dlplan-0.2.6/api/python/src/state_space.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/api/python/src/weisfeiler_lehman.cpp` & `dlplan-0.2.6/api/python/src/weisfeiler_lehman.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/api/python/test/test_barman.py` & `dlplan-0.2.6/api/python/test/test_barman.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/api/python/test/test_core.py` & `dlplan-0.2.6/api/python/test/test_core.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/api/python/test/test_generate.py` & `dlplan-0.2.6/api/python/test/test_generate.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/examples/core/__pycache__/tarski.cpython-36.pyc` & `dlplan-0.2.6/examples/core/__pycache__/tarski.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/examples/core/__pycache__/tarski.cpython-37.pyc` & `dlplan-0.2.6/examples/core/__pycache__/tarski.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/examples/core/core.cpp` & `dlplan-0.2.6/examples/core/core.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/examples/core/core.py` & `dlplan-0.2.6/examples/core/core.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/examples/generator/generator.cpp` & `dlplan-0.2.6/examples/generator/generator.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/examples/generator/generator.py` & `dlplan-0.2.6/examples/generator/generator.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/examples/policy/policy.cpp` & `dlplan-0.2.6/examples/policy/policy.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/examples/policy/policy.py` & `dlplan-0.2.6/examples/policy/policy.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/examples/state_space/delivery/CMakeLists.txt` & `dlplan-0.2.6/examples/state_space/delivery/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/examples/state_space/delivery/delivery.cpp` & `dlplan-0.2.6/examples/state_space/delivery/delivery.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/examples/state_space/delivery/delivery.py` & `dlplan-0.2.6/examples/state_space/delivery/delivery.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/examples/state_space/delivery/domain.pddl` & `dlplan-0.2.6/examples/state_space/delivery/domain.pddl`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/examples/state_space/delivery/instance_2_1_0.pddl` & `dlplan-0.2.6/examples/state_space/delivery/instance_2_1_0.pddl`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/examples/state_space/delivery/instance_2_2_0.pddl` & `dlplan-0.2.6/examples/state_space/delivery/instance_2_2_0.pddl`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/experiments/experiment_generator.cpp` & `dlplan-0.2.6/experiments/experiment_generator.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/experiments/experiment_parser.py` & `dlplan-0.2.6/experiments/experiment_parser.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/experiments/experiment_runner.py` & `dlplan-0.2.6/experiments/experiment_runner.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/experiments/main.py` & `dlplan-0.2.6/experiments/main.py`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/include/dlplan/core.h` & `dlplan-0.2.6/include/dlplan/core.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/include/dlplan/generator.h` & `dlplan-0.2.6/include/dlplan/generator.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/include/dlplan/novelty.h` & `dlplan-0.2.6/include/dlplan/novelty.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/include/dlplan/phmap/btree.h` & `dlplan-0.2.6/include/dlplan/phmap/btree.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/include/dlplan/phmap/meminfo.h` & `dlplan-0.2.6/include/dlplan/phmap/meminfo.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/include/dlplan/phmap/phmap.h` & `dlplan-0.2.6/include/dlplan/phmap/phmap.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/include/dlplan/phmap/phmap_base.h` & `dlplan-0.2.6/include/dlplan/phmap/phmap_base.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/include/dlplan/phmap/phmap_bits.h` & `dlplan-0.2.6/include/dlplan/phmap/phmap_bits.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/include/dlplan/phmap/phmap_config.h` & `dlplan-0.2.6/include/dlplan/phmap/phmap_config.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/include/dlplan/phmap/phmap_dump.h` & `dlplan-0.2.6/include/dlplan/phmap/phmap_dump.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/include/dlplan/phmap/phmap_fwd_decl.h` & `dlplan-0.2.6/include/dlplan/phmap/phmap_fwd_decl.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/include/dlplan/phmap/phmap_utils.h` & `dlplan-0.2.6/include/dlplan/phmap/phmap_utils.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/include/dlplan/policy.h` & `dlplan-0.2.6/include/dlplan/policy.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/include/dlplan/state_space.h` & `dlplan-0.2.6/include/dlplan/state_space.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/include/dlplan/utils/cache.h` & `dlplan-0.2.6/include/dlplan/utils/cache.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/include/dlplan/utils/dynamic_bitset.h` & `dlplan-0.2.6/include/dlplan/utils/dynamic_bitset.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/include/dlplan/utils/pimpl.h` & `dlplan-0.2.6/include/dlplan/utils/pimpl.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/include/dlplan/weisfeiler_lehman.h` & `dlplan-0.2.6/include/dlplan/weisfeiler_lehman.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/setup.py` & `dlplan-0.2.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 import subprocess
 from pathlib import Path
 
 from setuptools import setup, Extension, find_packages
 from setuptools.command.build_ext import build_ext
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 HERE = Path(__file__).resolve().parent
 
 
 # A CMakeExtension needs a sourcedir instead of a file list.
 # The name must be the _single_ output extension from the CMake build.
 # If you need multiple extensions, see scikit-build.
 class CMakeExtension(Extension):
@@ -58,15 +58,15 @@
     name="dlplan",
     version=__version__,
     author="Dominik Drexler, Jendrik Seipp and Guillem Francès",
     author_email="dominik.drexler@liu.se",
     url="https://github.com/rleap-project/dlplan",
     description="A library for using description logics features in planning",
     long_description="",
-    install_requires=["pybind11==2.10.4", "pybind11-global==2.10.4", "state_space_generator==0.1.4", "cmake>=3.16.3"],
+    install_requires=["pybind11==2.10.4", "pybind11-global==2.10.4", "state_space_generator==0.1.5", "cmake>=3.16.3"],
     packages=['dlplan'],
     package_dir={"": "api/python/src"},
     ext_modules=[CMakeExtension("_dlplan")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     extras_require={
         'test': [
```

### Comparing `dlplan-0.2.5/src/core/CMakeLists.txt` & `dlplan-0.2.6/src/core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/atom.cpp` & `dlplan-0.2.6/src/core/atom.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/cache.h` & `dlplan-0.2.6/src/core/cache.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/constant.cpp` & `dlplan-0.2.6/src/core/constant.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/core.cpp` & `dlplan-0.2.6/src/core/core.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/element_factory.cpp` & `dlplan-0.2.6/src/core/element_factory.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/element_factory.h` & `dlplan-0.2.6/src/core/element_factory.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/boolean.h` & `dlplan-0.2.6/src/core/elements/boolean.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/booleans/empty.h` & `dlplan-0.2.6/src/core/elements/booleans/empty.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/booleans/inclusion.h` & `dlplan-0.2.6/src/core/elements/booleans/inclusion.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/booleans/nullary.h` & `dlplan-0.2.6/src/core/elements/booleans/nullary.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/concept.h` & `dlplan-0.2.6/src/core/elements/concept.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/concepts/all.h` & `dlplan-0.2.6/src/core/elements/concepts/all.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/concepts/and.h` & `dlplan-0.2.6/src/core/elements/concepts/and.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/concepts/bot.h` & `dlplan-0.2.6/src/core/elements/concepts/bot.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/concepts/diff.h` & `dlplan-0.2.6/src/core/elements/concepts/diff.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/concepts/equal.h` & `dlplan-0.2.6/src/core/elements/concepts/equal.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/concepts/not.h` & `dlplan-0.2.6/src/core/elements/concepts/not.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/concepts/one_of.h` & `dlplan-0.2.6/src/core/elements/concepts/one_of.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/concepts/or.h` & `dlplan-0.2.6/src/core/elements/concepts/or.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/concepts/primitive.h` & `dlplan-0.2.6/src/core/elements/concepts/primitive.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/concepts/projection.h` & `dlplan-0.2.6/src/core/elements/concepts/projection.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/concepts/some.h` & `dlplan-0.2.6/src/core/elements/concepts/some.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/concepts/subset.h` & `dlplan-0.2.6/src/core/elements/concepts/subset.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/concepts/top.h` & `dlplan-0.2.6/src/core/elements/concepts/top.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/element.h` & `dlplan-0.2.6/src/core/elements/element.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/numerical.h` & `dlplan-0.2.6/src/core/elements/numerical.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/numericals/concept_distance.h` & `dlplan-0.2.6/src/core/elements/numericals/concept_distance.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/numericals/count.h` & `dlplan-0.2.6/src/core/elements/numericals/count.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/numericals/role_distance.h` & `dlplan-0.2.6/src/core/elements/numericals/role_distance.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/numericals/sum_concept_distance.h` & `dlplan-0.2.6/src/core/elements/numericals/sum_concept_distance.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/numericals/sum_role_distance.h` & `dlplan-0.2.6/src/core/elements/numericals/sum_role_distance.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/role.h` & `dlplan-0.2.6/src/core/elements/role.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/roles/and.h` & `dlplan-0.2.6/src/core/elements/roles/and.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/roles/compose.h` & `dlplan-0.2.6/src/core/elements/roles/compose.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/roles/diff.h` & `dlplan-0.2.6/src/core/elements/roles/diff.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/roles/identity.h` & `dlplan-0.2.6/src/core/elements/roles/identity.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/roles/inverse.h` & `dlplan-0.2.6/src/core/elements/roles/inverse.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/roles/not.h` & `dlplan-0.2.6/src/core/elements/roles/not.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/roles/or.h` & `dlplan-0.2.6/src/core/elements/roles/or.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/roles/primitive.h` & `dlplan-0.2.6/src/core/elements/roles/primitive.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/roles/restrict.h` & `dlplan-0.2.6/src/core/elements/roles/restrict.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/roles/top.h` & `dlplan-0.2.6/src/core/elements/roles/top.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/roles/transitive_closure.h` & `dlplan-0.2.6/src/core/elements/roles/transitive_closure.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/roles/transitive_reflexive_closure.h` & `dlplan-0.2.6/src/core/elements/roles/transitive_reflexive_closure.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/utils.cpp` & `dlplan-0.2.6/src/core/elements/utils.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/elements/utils.h` & `dlplan-0.2.6/src/core/elements/utils.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/instance_info.cpp` & `dlplan-0.2.6/src/core/instance_info.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/object.cpp` & `dlplan-0.2.6/src/core/object.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expression_factory.cpp` & `dlplan-0.2.6/src/core/parser/expression_factory.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/boolean.h` & `dlplan-0.2.6/src/core/parser/expressions/boolean.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/booleans/empty.h` & `dlplan-0.2.6/src/core/parser/expressions/booleans/empty.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/booleans/inclusion.h` & `dlplan-0.2.6/src/core/parser/expressions/booleans/inclusion.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/booleans/nullary.h` & `dlplan-0.2.6/src/core/parser/expressions/booleans/nullary.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/concept.h` & `dlplan-0.2.6/src/core/parser/expressions/concept.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/concepts/all.h` & `dlplan-0.2.6/src/core/parser/expressions/concepts/all.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/concepts/and.h` & `dlplan-0.2.6/src/core/parser/expressions/concepts/and.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/concepts/bot.h` & `dlplan-0.2.6/src/core/parser/expressions/concepts/bot.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/concepts/diff.h` & `dlplan-0.2.6/src/core/parser/expressions/concepts/diff.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/concepts/equal.h` & `dlplan-0.2.6/src/core/parser/expressions/concepts/equal.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/concepts/not.h` & `dlplan-0.2.6/src/core/parser/expressions/concepts/not.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/concepts/one_of.h` & `dlplan-0.2.6/src/core/parser/expressions/concepts/one_of.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/concepts/or.h` & `dlplan-0.2.6/src/core/parser/expressions/concepts/or.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/concepts/primitive.h` & `dlplan-0.2.6/src/core/parser/expressions/concepts/primitive.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/concepts/projection.h` & `dlplan-0.2.6/src/core/parser/expressions/concepts/projection.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/concepts/some.h` & `dlplan-0.2.6/src/core/parser/expressions/concepts/some.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/concepts/subset.h` & `dlplan-0.2.6/src/core/parser/expressions/concepts/subset.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/concepts/top.h` & `dlplan-0.2.6/src/core/parser/expressions/concepts/top.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/expression.h` & `dlplan-0.2.6/src/core/parser/expressions/expression.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/numerical.h` & `dlplan-0.2.6/src/core/parser/expressions/numerical.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/numericals/concept_distance.h` & `dlplan-0.2.6/src/core/parser/expressions/numericals/concept_distance.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/numericals/count.h` & `dlplan-0.2.6/src/core/parser/expressions/numericals/count.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/numericals/role_distance.h` & `dlplan-0.2.6/src/core/parser/expressions/numericals/role_distance.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/numericals/sum_concept_distance.h` & `dlplan-0.2.6/src/core/parser/expressions/numericals/sum_concept_distance.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/numericals/sum_role_distance.h` & `dlplan-0.2.6/src/core/parser/expressions/numericals/sum_role_distance.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/role.h` & `dlplan-0.2.6/src/core/parser/expressions/role.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/roles/and.h` & `dlplan-0.2.6/src/core/parser/expressions/roles/and.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/roles/compose.h` & `dlplan-0.2.6/src/core/parser/expressions/roles/compose.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/roles/diff.h` & `dlplan-0.2.6/src/core/parser/expressions/roles/diff.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/roles/identity.h` & `dlplan-0.2.6/src/core/parser/expressions/roles/identity.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/roles/inverse.h` & `dlplan-0.2.6/src/core/parser/expressions/roles/inverse.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/roles/not.h` & `dlplan-0.2.6/src/core/parser/expressions/roles/not.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/roles/or.h` & `dlplan-0.2.6/src/core/parser/expressions/roles/or.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/roles/primitive.h` & `dlplan-0.2.6/src/core/parser/expressions/roles/primitive.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/roles/restrict.h` & `dlplan-0.2.6/src/core/parser/expressions/roles/restrict.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/roles/top.h` & `dlplan-0.2.6/src/core/parser/expressions/roles/top.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/roles/transitive_closure.h` & `dlplan-0.2.6/src/core/parser/expressions/roles/transitive_closure.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/expressions/roles/transitive_reflexive_closure.h` & `dlplan-0.2.6/src/core/parser/expressions/roles/transitive_reflexive_closure.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/parser.cpp` & `dlplan-0.2.6/src/core/parser/parser.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/parser.h` & `dlplan-0.2.6/src/core/parser/parser.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/parser/utils.h` & `dlplan-0.2.6/src/core/parser/utils.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/predicate.cpp` & `dlplan-0.2.6/src/core/predicate.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/state.cpp` & `dlplan-0.2.6/src/core/state.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/core/vocabulary_info.cpp` & `dlplan-0.2.6/src/core/vocabulary_info.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/CMakeLists.txt` & `dlplan-0.2.6/src/generator/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/feature_generator.cpp` & `dlplan-0.2.6/src/generator/feature_generator.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/feature_generator.h` & `dlplan-0.2.6/src/generator/feature_generator.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/generator.cpp` & `dlplan-0.2.6/src/generator/generator.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/generator_data.h` & `dlplan-0.2.6/src/generator/generator_data.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/booleans/empty.cpp` & `dlplan-0.2.6/src/generator/rules/booleans/empty.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/booleans/inclusion.cpp` & `dlplan-0.2.6/src/generator/rules/booleans/inclusion.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/booleans/nullary.cpp` & `dlplan-0.2.6/src/generator/rules/booleans/nullary.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/concepts/all.cpp` & `dlplan-0.2.6/src/generator/rules/concepts/all.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/concepts/and.cpp` & `dlplan-0.2.6/src/generator/rules/concepts/and.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/concepts/bot.cpp` & `dlplan-0.2.6/src/generator/rules/concepts/bot.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/concepts/diff.cpp` & `dlplan-0.2.6/src/generator/rules/concepts/diff.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/concepts/equal.cpp` & `dlplan-0.2.6/src/generator/rules/concepts/equal.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/concepts/not.cpp` & `dlplan-0.2.6/src/generator/rules/concepts/not.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/concepts/one_of.cpp` & `dlplan-0.2.6/src/generator/rules/concepts/one_of.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/concepts/or.cpp` & `dlplan-0.2.6/src/generator/rules/concepts/or.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/concepts/primitive.cpp` & `dlplan-0.2.6/src/generator/rules/concepts/primitive.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/concepts/projection.cpp` & `dlplan-0.2.6/src/generator/rules/concepts/projection.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/concepts/some.cpp` & `dlplan-0.2.6/src/generator/rules/concepts/some.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/concepts/subset.cpp` & `dlplan-0.2.6/src/generator/rules/concepts/subset.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/concepts/top.cpp` & `dlplan-0.2.6/src/generator/rules/concepts/top.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/numericals/concept_distance.cpp` & `dlplan-0.2.6/src/generator/rules/numericals/concept_distance.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/numericals/count.cpp` & `dlplan-0.2.6/src/generator/rules/numericals/count.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/roles/and.cpp` & `dlplan-0.2.6/src/generator/rules/roles/and.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/roles/compose.cpp` & `dlplan-0.2.6/src/generator/rules/roles/compose.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/roles/diff.cpp` & `dlplan-0.2.6/src/generator/rules/roles/diff.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/roles/identity.cpp` & `dlplan-0.2.6/src/generator/rules/roles/identity.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/roles/inverse.cpp` & `dlplan-0.2.6/src/generator/rules/roles/inverse.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/roles/not.cpp` & `dlplan-0.2.6/src/generator/rules/roles/not.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/roles/or.cpp` & `dlplan-0.2.6/src/generator/rules/roles/or.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/roles/primitive.cpp` & `dlplan-0.2.6/src/generator/rules/roles/primitive.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/roles/restrict.cpp` & `dlplan-0.2.6/src/generator/rules/roles/restrict.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/roles/top.cpp` & `dlplan-0.2.6/src/generator/rules/roles/top.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/roles/transitive_closure.cpp` & `dlplan-0.2.6/src/generator/rules/roles/transitive_closure.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/roles/transitive_reflexive_closure.cpp` & `dlplan-0.2.6/src/generator/rules/roles/transitive_reflexive_closure.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/generator/rules/rule.h` & `dlplan-0.2.6/src/generator/rules/rule.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/novelty/CMakeLists.txt` & `dlplan-0.2.6/src/novelty/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/novelty/novelty_base.cpp` & `dlplan-0.2.6/src/novelty/novelty_base.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/novelty/novelty_table.cpp` & `dlplan-0.2.6/src/novelty/novelty_table.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/novelty/tuple_graph.cpp` & `dlplan-0.2.6/src/novelty/tuple_graph.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/novelty/tuple_index_generator.cpp` & `dlplan-0.2.6/src/novelty/tuple_index_generator.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/novelty/tuple_node.cpp` & `dlplan-0.2.6/src/novelty/tuple_node.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/policy/CMakeLists.txt` & `dlplan-0.2.6/src/policy/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/policy/cache.h` & `dlplan-0.2.6/src/policy/cache.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/policy/condition.cpp` & `dlplan-0.2.6/src/policy/condition.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/policy/condition.h` & `dlplan-0.2.6/src/policy/condition.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/policy/effect.cpp` & `dlplan-0.2.6/src/policy/effect.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/policy/effect.h` & `dlplan-0.2.6/src/policy/effect.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/policy/parser/expression_factory.cpp` & `dlplan-0.2.6/src/policy/parser/expression_factory.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/policy/parser/expression_factory.h` & `dlplan-0.2.6/src/policy/parser/expression_factory.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/policy/parser/expressions.h` & `dlplan-0.2.6/src/policy/parser/expressions.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/policy/parser/parser.cpp` & `dlplan-0.2.6/src/policy/parser/parser.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/policy/parser/parser.h` & `dlplan-0.2.6/src/policy/parser/parser.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/policy/policy.cpp` & `dlplan-0.2.6/src/policy/policy.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/policy/policy_builder.cpp` & `dlplan-0.2.6/src/policy/policy_builder.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/policy/policy_builder.h` & `dlplan-0.2.6/src/policy/policy_builder.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/policy/policy_impl.cpp` & `dlplan-0.2.6/src/policy/policy_impl.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/policy/policy_minimizer.cpp` & `dlplan-0.2.6/src/policy/policy_minimizer.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/policy/rule.cpp` & `dlplan-0.2.6/src/policy/rule.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/state_space/CMakeLists.txt` & `dlplan-0.2.6/src/state_space/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/state_space/generator.cpp` & `dlplan-0.2.6/src/state_space/generator.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/state_space/reader.cpp` & `dlplan-0.2.6/src/state_space/reader.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/state_space/state_space.cpp` & `dlplan-0.2.6/src/state_space/state_space.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/utils/MurmurHash3.cpp` & `dlplan-0.2.6/src/utils/MurmurHash3.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/utils/MurmurHash3.h` & `dlplan-0.2.6/src/utils/MurmurHash3.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/utils/collections.h` & `dlplan-0.2.6/src/utils/collections.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/utils/command.h` & `dlplan-0.2.6/src/utils/command.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/utils/countdown_timer.cpp` & `dlplan-0.2.6/src/utils/countdown_timer.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/utils/logging.h` & `dlplan-0.2.6/src/utils/logging.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/utils/set_operators.h` & `dlplan-0.2.6/src/utils/set_operators.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/utils/sha-256.c` & `dlplan-0.2.6/src/utils/sha-256.c`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/utils/system.cpp` & `dlplan-0.2.6/src/utils/system.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/utils/threadpool.h` & `dlplan-0.2.6/src/utils/threadpool.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/utils/timer.cpp` & `dlplan-0.2.6/src/utils/timer.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/utils/timer.h` & `dlplan-0.2.6/src/utils/timer.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/utils/tokenizer.h` & `dlplan-0.2.6/src/utils/tokenizer.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/weisfeiler_lehman/CMakeLists.txt` & `dlplan-0.2.6/src/weisfeiler_lehman/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/weisfeiler_lehman/color.h` & `dlplan-0.2.6/src/weisfeiler_lehman/color.h`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/src/weisfeiler_lehman/weisfeiler_lehman.cpp` & `dlplan-0.2.6/src/weisfeiler_lehman/weisfeiler_lehman.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/CMakeLists.txt` & `dlplan-0.2.6/tests/core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/b_empty.cpp` & `dlplan-0.2.6/tests/core/b_empty.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/b_inclusion.cpp` & `dlplan-0.2.6/tests/core/b_inclusion.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/b_nullary.cpp` & `dlplan-0.2.6/tests/core/b_nullary.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/c_all.cpp` & `dlplan-0.2.6/tests/core/c_all.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/c_and.cpp` & `dlplan-0.2.6/tests/core/c_and.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/c_bot.cpp` & `dlplan-0.2.6/tests/core/c_bot.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/c_diff.cpp` & `dlplan-0.2.6/tests/core/c_diff.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/c_equal.cpp` & `dlplan-0.2.6/tests/core/c_equal.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/c_not.cpp` & `dlplan-0.2.6/tests/core/c_not.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/c_one_of.cpp` & `dlplan-0.2.6/tests/core/c_one_of.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/c_or.cpp` & `dlplan-0.2.6/tests/core/c_or.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/c_primitive.cpp` & `dlplan-0.2.6/tests/core/c_primitive.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/c_projection.cpp` & `dlplan-0.2.6/tests/core/c_projection.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/c_some.cpp` & `dlplan-0.2.6/tests/core/c_some.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/c_subset.cpp` & `dlplan-0.2.6/tests/core/c_subset.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/c_top.cpp` & `dlplan-0.2.6/tests/core/c_top.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/core.cpp` & `dlplan-0.2.6/tests/core/core.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/multi_instance.cpp` & `dlplan-0.2.6/tests/core/multi_instance.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/n_concept_distance.cpp` & `dlplan-0.2.6/tests/core/n_concept_distance.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/n_count.cpp` & `dlplan-0.2.6/tests/core/n_count.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/n_role_distance.cpp` & `dlplan-0.2.6/tests/core/n_role_distance.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/n_sum_concept_distance.cpp` & `dlplan-0.2.6/tests/core/n_sum_concept_distance.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/n_sum_role_distance.cpp` & `dlplan-0.2.6/tests/core/n_sum_role_distance.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/r_and.cpp` & `dlplan-0.2.6/tests/core/r_and.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/r_compose.cpp` & `dlplan-0.2.6/tests/core/r_compose.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/r_diff.cpp` & `dlplan-0.2.6/tests/core/r_diff.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/r_identity.cpp` & `dlplan-0.2.6/tests/core/r_identity.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/r_inverse.cpp` & `dlplan-0.2.6/tests/core/r_inverse.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/r_not.cpp` & `dlplan-0.2.6/tests/core/r_not.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/r_or.cpp` & `dlplan-0.2.6/tests/core/r_or.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/r_primitive.cpp` & `dlplan-0.2.6/tests/core/r_primitive.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/r_restrict.cpp` & `dlplan-0.2.6/tests/core/r_restrict.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/r_top.cpp` & `dlplan-0.2.6/tests/core/r_top.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/r_transitive_closure.cpp` & `dlplan-0.2.6/tests/core/r_transitive_closure.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/core/r_transitive_reflexive_closure.cpp` & `dlplan-0.2.6/tests/core/r_transitive_reflexive_closure.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/generator/delivery/CMakeLists.txt` & `dlplan-0.2.6/tests/generator/delivery/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/generator/delivery/delivery.cpp` & `dlplan-0.2.6/tests/generator/delivery/delivery.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/generator/delivery/domain.pddl` & `dlplan-0.2.6/tests/generator/delivery/domain.pddl`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/generator/delivery/instance_2_2_0.pddl` & `dlplan-0.2.6/tests/generator/delivery/instance_2_2_0.pddl`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/generator/delivery/instance_4_2_29.pddl` & `dlplan-0.2.6/tests/generator/delivery/instance_4_2_29.pddl`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/novelty/gripper/CMakeLists.txt` & `dlplan-0.2.6/tests/novelty/gripper/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/novelty/gripper/domain.pddl` & `dlplan-0.2.6/tests/novelty/gripper/domain.pddl`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/novelty/gripper/gripper.cpp` & `dlplan-0.2.6/tests/novelty/gripper/gripper.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/novelty/tuple_index_generator.cpp` & `dlplan-0.2.6/tests/novelty/tuple_index_generator.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/policy/policy_builder.cpp` & `dlplan-0.2.6/tests/policy/policy_builder.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/policy/policy_minimizer.cpp` & `dlplan-0.2.6/tests/policy/policy_minimizer.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/policy/utils.cpp` & `dlplan-0.2.6/tests/policy/utils.cpp`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/state_space/gripper/CMakeLists.txt` & `dlplan-0.2.6/tests/state_space/gripper/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/state_space/gripper/domain.pddl` & `dlplan-0.2.6/tests/state_space/gripper/domain.pddl`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/state_space/spanner/CMakeLists.txt` & `dlplan-0.2.6/tests/state_space/spanner/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dlplan-0.2.5/tests/state_space/spanner/domain.pddl` & `dlplan-0.2.6/tests/state_space/spanner/domain.pddl`

 * *Files identical despite different names*


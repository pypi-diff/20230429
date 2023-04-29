# Comparing `tmp/gerrychain-0.2.8.tar.gz` & `tmp/gerrychain-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gerrychain-0.2.8.tar", last modified: Wed Feb 27 17:44:53 2019, max compression
+gzip compressed data, was "dist\gerrychain-0.2.9.tar", last modified: Wed Apr 17 16:35:01 2019, max compression
```

## Comparing `gerrychain-0.2.8.tar` & `gerrychain-0.2.9.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-27 17:44:53.000000 gerrychain-0.2.8/
--rw-r--r--   0 root         (0) root         (0)       53 2019-02-27 17:44:24.000000 gerrychain-0.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3665 2019-02-27 17:44:53.000000 gerrychain-0.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2535 2019-02-27 17:44:24.000000 gerrychain-0.2.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-27 17:44:53.000000 gerrychain-0.2.8/gerrychain/
--rw-r--r--   0 root         (0) root         (0)      243 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/__init__.py
--rw-r--r--   0 root         (0) root         (0)      498 2019-02-27 17:44:53.000000 gerrychain-0.2.8/gerrychain/_version.py
--rw-r--r--   0 root         (0) root         (0)      544 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/accept.py
--rw-r--r--   0 root         (0) root         (0)     3044 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/chain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-27 17:44:53.000000 gerrychain-0.2.8/gerrychain/constraints/
--rw-r--r--   0 root         (0) root         (0)     3066 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/constraints/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4632 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/constraints/bounds.py
--rw-r--r--   0 root         (0) root         (0)      779 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/constraints/compactness.py
--rw-r--r--   0 root         (0) root         (0)     6911 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/constraints/contiguity.py
--rw-r--r--   0 root         (0) root         (0)     4943 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/constraints/validity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-27 17:44:53.000000 gerrychain-0.2.8/gerrychain/graph/
--rw-r--r--   0 root         (0) root         (0)       65 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2736 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/graph/adjacency.py
--rw-r--r--   0 root         (0) root         (0)     1783 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/graph/geo.py
--rw-r--r--   0 root         (0) root         (0)    11199 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)     5785 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/grid.py
--rw-r--r--   0 root         (0) root         (0)     1007 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/metagraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-27 17:44:53.000000 gerrychain-0.2.8/gerrychain/partition/
--rw-r--r--   0 root         (0) root         (0)      125 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/partition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3912 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/partition/assignment.py
--rw-r--r--   0 root         (0) root         (0)      827 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/partition/geographic.py
--rw-r--r--   0 root         (0) root         (0)     8193 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/partition/partition.py
--rw-r--r--   0 root         (0) root         (0)      521 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/partition/subgraphs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-27 17:44:53.000000 gerrychain-0.2.8/gerrychain/proposals/
--rw-r--r--   0 root         (0) root         (0)       59 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/proposals/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2196 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/proposals/proposals.py
--rw-r--r--   0 root         (0) root         (0)     1664 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/proposals/tree_proposals.py
--rw-r--r--   0 root         (0) root         (0)       97 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/random.py
--rw-r--r--   0 root         (0) root         (0)     4597 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/scores.py
--rw-r--r--   0 root         (0) root         (0)     4854 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/tree.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-27 17:44:53.000000 gerrychain-0.2.8/gerrychain/updaters/
--rw-r--r--   0 root         (0) root         (0)      788 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/updaters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3234 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/updaters/compactness.py
--rw-r--r--   0 root         (0) root         (0)     2271 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/updaters/county_splits.py
--rw-r--r--   0 root         (0) root         (0)     1899 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/updaters/cut_edges.py
--rw-r--r--   0 root         (0) root         (0)     8571 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/updaters/election.py
--rw-r--r--   0 root         (0) root         (0)     5002 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/updaters/flows.py
--rw-r--r--   0 root         (0) root         (0)     4469 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/updaters/tally.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-27 17:44:53.000000 gerrychain-0.2.8/gerrychain/vendor/
--rw-r--r--   0 root         (0) root         (0)        0 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/vendor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-27 17:44:53.000000 gerrychain-0.2.8/gerrychain/vendor/utm/
--rw-r--r--   0 root         (0) root         (0)      173 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/vendor/utm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8697 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/vendor/utm/conversion.py
--rw-r--r--   0 root         (0) root         (0)       44 2019-02-27 17:44:24.000000 gerrychain-0.2.8/gerrychain/vendor/utm/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-27 17:44:53.000000 gerrychain-0.2.8/gerrychain.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3665 2019-02-27 17:44:53.000000 gerrychain-0.2.8/gerrychain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1337 2019-02-27 17:44:53.000000 gerrychain-0.2.8/gerrychain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-02-27 17:44:53.000000 gerrychain-0.2.8/gerrychain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2019-02-27 17:44:53.000000 gerrychain-0.2.8/gerrychain.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2019-02-27 17:44:53.000000 gerrychain-0.2.8/gerrychain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      711 2019-02-27 17:44:53.000000 gerrychain-0.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1091 2019-02-27 17:44:24.000000 gerrychain-0.2.8/setup.py
--rw-r--r--   0 root         (0) root         (0)    68611 2019-02-27 17:44:24.000000 gerrychain-0.2.8/versioneer.py
+drwxrwxrwx   0        0        0        0 2019-04-17 16:35:01.000000 gerrychain-0.2.9/
+-rw-rw-rw-   0        0        0     5695 2019-04-17 16:35:01.000000 gerrychain-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4147 2019-04-17 16:28:42.000000 gerrychain-0.2.9/README.rst
+drwxrwxrwx   0        0        0        0 2019-04-17 16:35:01.000000 gerrychain-0.2.9/gerrychain/
+-rw-rw-rw-   0        0        0      251 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/__init__.py
+-rw-rw-rw-   0        0        0      519 2019-04-17 16:35:01.000000 gerrychain-0.2.9/gerrychain/_version.py
+-rw-rw-rw-   0        0        0      565 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/accept.py
+-rw-rw-rw-   0        0        0     3077 2019-04-10 18:42:19.000000 gerrychain-0.2.9/gerrychain/chain.py
+drwxrwxrwx   0        0        0        0 2019-04-17 16:35:01.000000 gerrychain-0.2.9/gerrychain/constraints/
+-rw-rw-rw-   0        0        0     3118 2019-03-26 13:53:09.000000 gerrychain-0.2.9/gerrychain/constraints/__init__.py
+-rw-rw-rw-   0        0        0     4787 2019-03-26 13:53:09.000000 gerrychain-0.2.9/gerrychain/constraints/bounds.py
+-rw-rw-rw-   0        0        0      808 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/constraints/compactness.py
+-rw-rw-rw-   0        0        0     7138 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/constraints/contiguity.py
+-rw-rw-rw-   0        0        0     5080 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/constraints/validity.py
+drwxrwxrwx   0        0        0        0 2019-04-17 16:35:01.000000 gerrychain-0.2.9/gerrychain/graph/
+-rw-rw-rw-   0        0        0       68 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/graph/__init__.py
+-rw-rw-rw-   0        0        0     2831 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/graph/adjacency.py
+-rw-rw-rw-   0        0        0     1839 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/graph/geo.py
+-rw-rw-rw-   0        0        0    11671 2019-04-10 18:31:02.000000 gerrychain-0.2.9/gerrychain/graph/graph.py
+-rw-rw-rw-   0        0        0     5963 2019-04-17 16:25:32.000000 gerrychain-0.2.9/gerrychain/grid.py
+-rw-rw-rw-   0        0        0     1040 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/metagraph.py
+drwxrwxrwx   0        0        0        0 2019-04-17 16:35:01.000000 gerrychain-0.2.9/gerrychain/metrics/
+-rw-rw-rw-   0        0        0       65 2019-04-17 16:25:32.000000 gerrychain-0.2.9/gerrychain/metrics/__init__.py
+-rw-rw-rw-   0        0        0      389 2019-04-17 16:25:32.000000 gerrychain-0.2.9/gerrychain/metrics/compactness.py
+-rw-rw-rw-   0        0        0     4707 2019-04-17 16:25:32.000000 gerrychain-0.2.9/gerrychain/metrics/partisan.py
+drwxrwxrwx   0        0        0        0 2019-04-17 16:35:01.000000 gerrychain-0.2.9/gerrychain/partition/
+-rw-rw-rw-   0        0        0      129 2019-04-17 15:01:23.000000 gerrychain-0.2.9/gerrychain/partition/__init__.py
+-rw-rw-rw-   0        0        0     4896 2019-04-10 18:35:09.000000 gerrychain-0.2.9/gerrychain/partition/assignment.py
+-rw-rw-rw-   0        0        0      854 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/partition/geographic.py
+-rw-rw-rw-   0        0        0     8553 2019-04-17 15:01:23.000000 gerrychain-0.2.9/gerrychain/partition/partition.py
+-rw-rw-rw-   0        0        0      539 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/partition/subgraphs.py
+drwxrwxrwx   0        0        0        0 2019-04-17 16:35:01.000000 gerrychain-0.2.9/gerrychain/proposals/
+-rw-rw-rw-   0        0        0       61 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/proposals/__init__.py
+-rw-rw-rw-   0        0        0     2270 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/proposals/proposals.py
+-rw-rw-rw-   0        0        0     1713 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/proposals/tree_proposals.py
+-rw-rw-rw-   0        0        0      102 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/random.py
+-rw-rw-rw-   0        0        0     5417 2019-03-13 19:42:24.000000 gerrychain-0.2.9/gerrychain/tree.py
+drwxrwxrwx   0        0        0        0 2019-04-17 16:35:01.000000 gerrychain-0.2.9/gerrychain/updaters/
+-rw-rw-rw-   0        0        0      758 2019-04-17 16:25:32.000000 gerrychain-0.2.9/gerrychain/updaters/__init__.py
+-rw-rw-rw-   0        0        0     3057 2019-04-17 16:25:32.000000 gerrychain-0.2.9/gerrychain/updaters/compactness.py
+-rw-rw-rw-   0        0        0     2342 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/updaters/county_splits.py
+-rw-rw-rw-   0        0        0     1963 2019-04-10 18:30:13.000000 gerrychain-0.2.9/gerrychain/updaters/cut_edges.py
+-rw-rw-rw-   0        0        0     8815 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/updaters/election.py
+-rw-rw-rw-   0        0        0     5146 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/updaters/flows.py
+-rw-rw-rw-   0        0        0     4597 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/updaters/tally.py
+drwxrwxrwx   0        0        0        0 2019-04-17 16:35:01.000000 gerrychain-0.2.9/gerrychain/vendor/
+-rw-rw-rw-   0        0        0        0 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2019-04-17 16:35:01.000000 gerrychain-0.2.9/gerrychain/vendor/utm/
+-rw-rw-rw-   0        0        0      181 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/vendor/utm/__init__.py
+-rw-rw-rw-   0        0        0     9017 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/vendor/utm/conversion.py
+-rw-rw-rw-   0        0        0       46 2019-03-08 15:04:44.000000 gerrychain-0.2.9/gerrychain/vendor/utm/error.py
+drwxrwxrwx   0        0        0        0 2019-04-17 16:35:01.000000 gerrychain-0.2.9/gerrychain.egg-info/
+-rw-rw-rw-   0        0        0     5695 2019-04-17 16:35:01.000000 gerrychain-0.2.9/gerrychain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1386 2019-04-17 16:35:01.000000 gerrychain-0.2.9/gerrychain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2019-04-17 16:35:01.000000 gerrychain-0.2.9/gerrychain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2019-04-17 16:35:01.000000 gerrychain-0.2.9/gerrychain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2019-04-17 16:35:01.000000 gerrychain-0.2.9/gerrychain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      879 2019-04-17 16:35:01.000000 gerrychain-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1129 2019-04-17 16:33:50.000000 gerrychain-0.2.9/setup.py
```

### Comparing `gerrychain-0.2.8/gerrychain/accept.py` & `gerrychain-0.2.9/gerrychain/accept.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from .random import random
-
-
-def always_accept(partition):
-    return True
-
-
-def cut_edge_accept(partition):
-    """Always accepts the flip if the number of cut_edges increases.
-    Otherwise, uses the Metropolis criterion to decide.
-
-    :param partition: The current partition to accept a flip from.
-    :return: True if accepted, False to remain in place
-
-    """
-    bound = 1
-
-    if partition.parent is not None:
-        bound = min(1, len(partition.parent["cut_edges"]) / len(partition["cut_edges"]))
-
-    return random.random() < bound
+from .random import random
+
+
+def always_accept(partition):
+    return True
+
+
+def cut_edge_accept(partition):
+    """Always accepts the flip if the number of cut_edges increases.
+    Otherwise, uses the Metropolis criterion to decide.
+
+    :param partition: The current partition to accept a flip from.
+    :return: True if accepted, False to remain in place
+
+    """
+    bound = 1
+
+    if partition.parent is not None:
+        bound = min(1, len(partition.parent["cut_edges"]) / len(partition["cut_edges"]))
+
+    return random.random() < bound
```

### Comparing `gerrychain-0.2.8/gerrychain/constraints/__init__.py` & `gerrychain-0.2.9/gerrychain/constraints/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-"""
-The :mod:`gerrychain.constraints` module provides a collection of constraint
-functions and helper classes for the validation step in GerryChain.
-
-=============================== ===============================================
-Helper classes
-===============================================================================
-``Validator``                    Collection of constraints
-``Bounds``                       Bounds on numeric constraints
-``UpperBounds``                  Upper bounds on numeric constraints
-``LowerBounds``                  Lower bounds on numeric constraints
-``SelfConfiguringUpperBound``    Automatic upper bounds on numeric constraints
-``SelfConfiguringLowerBound``    Automatic lower bounds on numeric constraints
-``WithinPercentRangeOfBounds``   Percentage bounds for numeric constraints
-===============================================================================
-
-|
-
-================================================== ==============================================
-Binary constraint functions
-=================================================================================================
-``no_worse_L1_reciprocal_polsby_popper``            Lower bounded L1-reciprocal Polsby-Popper
-``no_worse_L_minus_1_reciprocal_polsby_popper``     Lower bounded L(-1)-reciprocal Polsby-Popper
-``contiguous``                                      Districts are contiguous (with NetworkX methods)
-``contiguous_bf``                                   Districts are contiguous (with a breadth-first search)
-``single_flip_contiguous``                          Districts are contiguous (optimized for ``propose_random_flip`` proposal)
-``no_vanishing_districts``                          No districts may be completely consumed
-================================================== ==============================================
-
-Each new step proposed to the chain is passed off to the "validator" functions
-here to determine whether or not the step is valid. If it is invalid (breaks
-contiguity, for instance), then the step is immediately rejected.
-
-A validator should take in a :class:`~gerrychain.partition.Partition` instance,
-and should return whether or not the instance is valid according to their
-rules. Many top-level functions following this signature in this module are
-examples of this.
-
-"""
-
-from .bounds import (LowerBound, SelfConfiguringLowerBound,
-                     SelfConfiguringUpperBound, UpperBound,
-                     WithinPercentRangeOfBounds)
-from .compactness import (L1_polsby_popper, L1_reciprocal_polsby_popper,
-                          L2_polsby_popper, L_minus_1_polsby_popper,
-                          no_worse_L1_reciprocal_polsby_popper,
-                          no_worse_L_minus_1_polsby_popper)
-from .contiguity import (contiguous, contiguous_bfs, no_more_discontiguous,
-                         single_flip_contiguous)
-from .validity import (Validator, districts_within_tolerance,
-                       no_vanishing_districts, refuse_new_splits,
-                       within_percent_of_ideal_population)
+"""
+The :mod:`gerrychain.constraints` module provides a collection of constraint
+functions and helper classes for the validation step in GerryChain.
+
+=============================== ===============================================
+Helper classes
+===============================================================================
+``Validator``                    Collection of constraints
+``Bounds``                       Bounds on numeric constraints
+``UpperBounds``                  Upper bounds on numeric constraints
+``LowerBounds``                  Lower bounds on numeric constraints
+``SelfConfiguringUpperBound``    Automatic upper bounds on numeric constraints
+``SelfConfiguringLowerBound``    Automatic lower bounds on numeric constraints
+``WithinPercentRangeOfBounds``   Percentage bounds for numeric constraints
+===============================================================================
+
+|
+
+================================================== ==============================================
+Binary constraint functions
+=================================================================================================
+``no_worse_L1_reciprocal_polsby_popper``            Lower bounded L1-reciprocal Polsby-Popper
+``no_worse_L_minus_1_reciprocal_polsby_popper``     Lower bounded L(-1)-reciprocal Polsby-Popper
+``contiguous``                                      Districts are contiguous (with NetworkX methods)
+``contiguous_bf``                                   Districts are contiguous (with a breadth-first search)
+``single_flip_contiguous``                          Districts are contiguous (optimized for ``propose_random_flip`` proposal)
+``no_vanishing_districts``                          No districts may be completely consumed
+================================================== ==============================================
+
+Each new step proposed to the chain is passed off to the "validator" functions
+here to determine whether or not the step is valid. If it is invalid (breaks
+contiguity, for instance), then the step is immediately rejected.
+
+A validator should take in a :class:`~gerrychain.partition.Partition` instance,
+and should return whether or not the instance is valid according to their
+rules. Many top-level functions following this signature in this module are
+examples of this.
+
+"""
+
+from .bounds import (LowerBound, SelfConfiguringLowerBound,
+                     SelfConfiguringUpperBound, UpperBound,
+                     WithinPercentRangeOfBounds)
+from .compactness import (L1_polsby_popper, L1_reciprocal_polsby_popper,
+                          L2_polsby_popper, L_minus_1_polsby_popper,
+                          no_worse_L1_reciprocal_polsby_popper,
+                          no_worse_L_minus_1_polsby_popper)
+from .contiguity import (contiguous, contiguous_bfs, no_more_discontiguous,
+                         single_flip_contiguous)
+from .validity import (Validator, districts_within_tolerance,
+                       no_vanishing_districts, refuse_new_splits,
+                       within_percent_of_ideal_population)
```

### Comparing `gerrychain-0.2.8/gerrychain/constraints/compactness.py` & `gerrychain-0.2.9/gerrychain/constraints/compactness.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-
-import math
-
-from .bounds import SelfConfiguringLowerBound, SelfConfiguringUpperBound
-
-
-def L1_reciprocal_polsby_popper(partition):
-    return sum(1 / value for value in partition["polsby_popper"].values())
-
-
-def L1_polsby_popper(partition):
-    return sum(value for value in partition["polsby_popper"].values())
-
-
-def L2_polsby_popper(partition):
-    return math.sqrt(sum(value ** 2 for value in partition["polsby_popper"].values()))
-
-
-def L_minus_1_polsby_popper(partition):
-    return len(partition.parts) / sum(
-        1 / value for value in partition["polsby_popper"].values()
-    )
-
-
-no_worse_L_minus_1_polsby_popper = SelfConfiguringLowerBound(L_minus_1_polsby_popper)
-
-no_worse_L1_reciprocal_polsby_popper = SelfConfiguringUpperBound(
-    L1_reciprocal_polsby_popper
-)
+
+import math
+
+from .bounds import SelfConfiguringLowerBound, SelfConfiguringUpperBound
+
+
+def L1_reciprocal_polsby_popper(partition):
+    return sum(1 / value for value in partition["polsby_popper"].values())
+
+
+def L1_polsby_popper(partition):
+    return sum(value for value in partition["polsby_popper"].values())
+
+
+def L2_polsby_popper(partition):
+    return math.sqrt(sum(value ** 2 for value in partition["polsby_popper"].values()))
+
+
+def L_minus_1_polsby_popper(partition):
+    return len(partition.parts) / sum(
+        1 / value for value in partition["polsby_popper"].values()
+    )
+
+
+no_worse_L_minus_1_polsby_popper = SelfConfiguringLowerBound(L_minus_1_polsby_popper)
+
+no_worse_L1_reciprocal_polsby_popper = SelfConfiguringUpperBound(
+    L1_reciprocal_polsby_popper
+)
```

### Comparing `gerrychain-0.2.8/gerrychain/constraints/contiguity.py` & `gerrychain-0.2.9/gerrychain/constraints/contiguity.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,227 +1,227 @@
-from heapq import heappop, heappush
-from itertools import count
-
-import networkx as nx
-
-from ..random import random
-from .bounds import SelfConfiguringLowerBound
-
-
-def are_reachable(G, source, avoid, targets):
-    """Check that source can reach targets while avoiding given edges.
-    This function is a modified form of NetworkX's ``_dijkstra_multisource()``.
-
-    :param G: NetworkX graph.
-    :param source: Starting node.
-    :param weight: Function with (u, v, data) input that returns that edges weight.
-    :param targets: Nodes required to find.
-    :return:
-        A mapping from node to shortest distance to that node from one
-        of the source nodes.
-    :rtype: dict
-    """
-    G_succ = G._succ if G.is_directed() else G._adj
-
-    push = heappush
-    pop = heappop
-    dist = {}  # dictionary of final distances
-    seen = {}
-    # fringe is heapq with 3-tuples (distance,c,node)
-    # use the count c to avoid comparing nodes (may not be able to)
-    c = count()
-    fringe = []
-
-    seen[source] = 0
-    push(fringe, (0, next(c), source))
-
-    while not all(t in seen for t in targets) and fringe:
-        (d, _, v) = pop(fringe)
-        if v in dist:
-            continue  # already searched this node.
-        dist[v] = d
-        for u, e in G_succ[v].items():
-            if avoid(v, u, e):
-                continue
-
-            vu_dist = dist[v] + 1
-            if u not in seen or vu_dist < seen[u]:
-                seen[u] = vu_dist
-                push(fringe, (vu_dist, next(c), u))
-
-    return all(t in seen for t in targets)
-
-
-def single_flip_contiguous(partition):
-    """Check if swapping the given node from its old assignment disconnects the
-    old assignment class.
-
-    :param partition: The proposed next :class:`~gerrychain.partition.Partition`
-
-    :return: whether the partition is contiguous
-    :rtype: bool
-
-    We assume that `removed_node` belonged to an assignment class that formed a
-    connected subgraph. To see if its removal left the subgraph connected, we
-    check that the neighbors of the removed node are still connected through
-    the changed graph.
-
-    """
-    parent = partition.parent
-    flips = partition.flips
-    if not flips or not parent:
-        return contiguous(partition)
-
-    graph = partition.graph
-    assignment = partition.assignment
-
-    def partition_edge_avoid(start_node, end_node, edge_attrs):
-        """Compute the district edge weight, which is 1 if the nodes have the same
-        assignment, and infinity otherwise.
-        """
-        if assignment[start_node] != assignment[end_node]:
-            # Fun fact: networkx actually refuses to take edges with None
-            # weight.
-            return True
-
-        return False
-
-    for changed_node in flips:
-        old_assignment = partition.parent.assignment[changed_node]
-
-        old_neighbors = [
-            node
-            for node in graph.neighbors(changed_node)
-            if assignment[node] == old_assignment
-        ]
-
-        if not old_neighbors:
-            # Under our assumptions, if there are no old neighbors, then the
-            # old_assignment district has vanished. It is trivially connected.
-
-            # However, we actually don't want any districts to disappear because
-            # it ends up breaking a lot of our other updaters. So we consider
-            # the empty district to be disconnected.
-            return False
-
-        start_neighbor = random.choice(old_neighbors)
-
-        connected = are_reachable(
-            graph, start_neighbor, partition_edge_avoid, old_neighbors
-        )
-
-        if not connected:
-            return False
-
-    # All neighbors of all changed nodes are connected, so the new graph is
-    # connected.
-    return True
-
-
-def affected_parts(partition):
-    """Returns the set of IDs of all parts that gained or lost a node during the last
-    flip.
-    """
-    flips = partition.flips
-    parent = partition.parent
-
-    if flips is None:
-        return partition.parts
-
-    affected = set()
-    for node, part in flips.items():
-        affected.add(part)
-        affected.add(parent.assignment[node])
-
-    return affected
-
-
-def contiguous(partition):
-    """Check if the parts of a partition are connected using :func:`networkx.is_connected`.
-
-    :param partition: The proposed next :class:`~gerrychain.partition.Partition`
-
-    :return: whether the partition is contiguous
-    :rtype: bool
-    """
-    return all(
-        nx.is_connected(partition.subgraphs[part]) for part in affected_parts(partition)
-    )
-
-
-def contiguous_bfs(partition):
-    """Checks that a given partition's parts are connected as graphs using a simple
-    breadth-first search.
-
-    :param partition: Instance of Partition
-    :return: Whether the parts of this partition are connected
-    :rtype: bool
-    """
-    parts_to_check = affected_parts(partition)
-
-    # Generates a subgraph for each district and perform a BFS on it
-    # to check connectedness.
-    for part in parts_to_check:
-        adj = nx.to_dict_of_lists(partition.subgraphs[part])
-        if _bfs(adj) is False:
-            return False
-
-    return True
-
-
-def number_of_contiguous_parts(partition):
-    """Return the number of non-connected assignment subgraphs.
-
-    :param partition: Instance of Partition; contains connected components.
-    :return: number of contiguous districts
-    :rtype: int
-    """
-    parts = partition.assignment.parts
-    return sum(1 for part in parts if nx.is_connected(partition.subgraphs[part]))
-
-
-def contiguous_components(partition):
-    """Return then connected components of each of the subgraphs of the parts
-    of the partition.
-
-    :param partition: Instance of Partition; contains connected components.
-    :return: dictionary mapping each part ID to a list holding the connected
-        subgraphs of that part of the partition
-    :rtype: dict
-    """
-    return {
-        part: [subgraph.subgraph(nodes) for nodes in nx.connected_components(subgraph)]
-        for part, subgraph in partition.subgraphs.items()
-    }
-
-
-no_more_discontiguous = SelfConfiguringLowerBound(number_of_contiguous_parts)
-
-
-def _bfs(graph):
-    """Performs a breadth-first search on the provided graph and returns true or
-    false depending on whether the graph is connected.
-
-    :param graph: Dict-of-lists; an adjacency matrix.
-    :return: is this graph connected?
-    :rtype: bool
-    """
-    q = [next(iter(graph))]
-    visited = set()
-    total_vertices = len(graph)
-
-    # Check if the district has a single vertex. If it does, then simply return
-    # `True`, as it's trivially connected.
-    if total_vertices <= 1:
-        return True
-
-    # bfs!
-    while len(q) > 0:
-        current = q.pop(0)
-        neighbors = graph[current]
-
-        for neighbor in neighbors:
-            if neighbor not in visited:
-                visited.add(neighbor)
-                q += [neighbor]
-
-    return total_vertices == len(visited)
+from heapq import heappop, heappush
+from itertools import count
+
+import networkx as nx
+
+from ..random import random
+from .bounds import SelfConfiguringLowerBound
+
+
+def are_reachable(G, source, avoid, targets):
+    """Check that source can reach targets while avoiding given edges.
+    This function is a modified form of NetworkX's ``_dijkstra_multisource()``.
+
+    :param G: NetworkX graph.
+    :param source: Starting node.
+    :param weight: Function with (u, v, data) input that returns that edges weight.
+    :param targets: Nodes required to find.
+    :return:
+        A mapping from node to shortest distance to that node from one
+        of the source nodes.
+    :rtype: dict
+    """
+    G_succ = G._succ if G.is_directed() else G._adj
+
+    push = heappush
+    pop = heappop
+    dist = {}  # dictionary of final distances
+    seen = {}
+    # fringe is heapq with 3-tuples (distance,c,node)
+    # use the count c to avoid comparing nodes (may not be able to)
+    c = count()
+    fringe = []
+
+    seen[source] = 0
+    push(fringe, (0, next(c), source))
+
+    while not all(t in seen for t in targets) and fringe:
+        (d, _, v) = pop(fringe)
+        if v in dist:
+            continue  # already searched this node.
+        dist[v] = d
+        for u, e in G_succ[v].items():
+            if avoid(v, u, e):
+                continue
+
+            vu_dist = dist[v] + 1
+            if u not in seen or vu_dist < seen[u]:
+                seen[u] = vu_dist
+                push(fringe, (vu_dist, next(c), u))
+
+    return all(t in seen for t in targets)
+
+
+def single_flip_contiguous(partition):
+    """Check if swapping the given node from its old assignment disconnects the
+    old assignment class.
+
+    :param partition: The proposed next :class:`~gerrychain.partition.Partition`
+
+    :return: whether the partition is contiguous
+    :rtype: bool
+
+    We assume that `removed_node` belonged to an assignment class that formed a
+    connected subgraph. To see if its removal left the subgraph connected, we
+    check that the neighbors of the removed node are still connected through
+    the changed graph.
+
+    """
+    parent = partition.parent
+    flips = partition.flips
+    if not flips or not parent:
+        return contiguous(partition)
+
+    graph = partition.graph
+    assignment = partition.assignment
+
+    def partition_edge_avoid(start_node, end_node, edge_attrs):
+        """Compute the district edge weight, which is 1 if the nodes have the same
+        assignment, and infinity otherwise.
+        """
+        if assignment[start_node] != assignment[end_node]:
+            # Fun fact: networkx actually refuses to take edges with None
+            # weight.
+            return True
+
+        return False
+
+    for changed_node in flips:
+        old_assignment = partition.parent.assignment[changed_node]
+
+        old_neighbors = [
+            node
+            for node in graph.neighbors(changed_node)
+            if assignment[node] == old_assignment
+        ]
+
+        if not old_neighbors:
+            # Under our assumptions, if there are no old neighbors, then the
+            # old_assignment district has vanished. It is trivially connected.
+
+            # However, we actually don't want any districts to disappear because
+            # it ends up breaking a lot of our other updaters. So we consider
+            # the empty district to be disconnected.
+            return False
+
+        start_neighbor = random.choice(old_neighbors)
+
+        connected = are_reachable(
+            graph, start_neighbor, partition_edge_avoid, old_neighbors
+        )
+
+        if not connected:
+            return False
+
+    # All neighbors of all changed nodes are connected, so the new graph is
+    # connected.
+    return True
+
+
+def affected_parts(partition):
+    """Returns the set of IDs of all parts that gained or lost a node during the last
+    flip.
+    """
+    flips = partition.flips
+    parent = partition.parent
+
+    if flips is None:
+        return partition.parts
+
+    affected = set()
+    for node, part in flips.items():
+        affected.add(part)
+        affected.add(parent.assignment[node])
+
+    return affected
+
+
+def contiguous(partition):
+    """Check if the parts of a partition are connected using :func:`networkx.is_connected`.
+
+    :param partition: The proposed next :class:`~gerrychain.partition.Partition`
+
+    :return: whether the partition is contiguous
+    :rtype: bool
+    """
+    return all(
+        nx.is_connected(partition.subgraphs[part]) for part in affected_parts(partition)
+    )
+
+
+def contiguous_bfs(partition):
+    """Checks that a given partition's parts are connected as graphs using a simple
+    breadth-first search.
+
+    :param partition: Instance of Partition
+    :return: Whether the parts of this partition are connected
+    :rtype: bool
+    """
+    parts_to_check = affected_parts(partition)
+
+    # Generates a subgraph for each district and perform a BFS on it
+    # to check connectedness.
+    for part in parts_to_check:
+        adj = nx.to_dict_of_lists(partition.subgraphs[part])
+        if _bfs(adj) is False:
+            return False
+
+    return True
+
+
+def number_of_contiguous_parts(partition):
+    """Return the number of non-connected assignment subgraphs.
+
+    :param partition: Instance of Partition; contains connected components.
+    :return: number of contiguous districts
+    :rtype: int
+    """
+    parts = partition.assignment.parts
+    return sum(1 for part in parts if nx.is_connected(partition.subgraphs[part]))
+
+
+def contiguous_components(partition):
+    """Return then connected components of each of the subgraphs of the parts
+    of the partition.
+
+    :param partition: Instance of Partition; contains connected components.
+    :return: dictionary mapping each part ID to a list holding the connected
+        subgraphs of that part of the partition
+    :rtype: dict
+    """
+    return {
+        part: [subgraph.subgraph(nodes) for nodes in nx.connected_components(subgraph)]
+        for part, subgraph in partition.subgraphs.items()
+    }
+
+
+no_more_discontiguous = SelfConfiguringLowerBound(number_of_contiguous_parts)
+
+
+def _bfs(graph):
+    """Performs a breadth-first search on the provided graph and returns true or
+    false depending on whether the graph is connected.
+
+    :param graph: Dict-of-lists; an adjacency matrix.
+    :return: is this graph connected?
+    :rtype: bool
+    """
+    q = [next(iter(graph))]
+    visited = set()
+    total_vertices = len(graph)
+
+    # Check if the district has a single vertex. If it does, then simply return
+    # `True`, as it's trivially connected.
+    if total_vertices <= 1:
+        return True
+
+    # bfs!
+    while len(q) > 0:
+        current = q.pop(0)
+        neighbors = graph[current]
+
+        for neighbor in neighbors:
+            if neighbor not in visited:
+                visited.add(neighbor)
+                q += [neighbor]
+
+    return total_vertices == len(visited)
```

### Comparing `gerrychain-0.2.8/gerrychain/constraints/validity.py` & `gerrychain-0.2.9/gerrychain/constraints/validity.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-from ..updaters import CountySplit
-from .bounds import Bounds
-
-
-class Validator:
-    """A single callable for checking that a partition passes a collection of
-    constraints. Intended to be passed as the ``is_valid`` parameter when
-    instantiating :class:`~gerrychain.MarkovChain`.
-
-    This class is meant to be called as a function after instantiation; its
-    return is ``True`` if all validators pass, and ``False`` if any one fails.
-
-    Example usage::
-
-        is_valid = Validator([constraint1, constraint2, constraint3])
-        chain = MarkovChain(proposal, is_valid, accept, initial_state, total_steps)
-    """
-
-    def __init__(self, constraints):
-        """
-        :param constraints: List of validator functions that will check partitions.
-        """
-        self.constraints = constraints
-
-    def __call__(self, partition):
-        """Determine if the given partition is valid.
-
-        :param partition: :class:`Partition` class to check.
-
-        """
-        # check each constraint function and fail when a constraint test fails
-        for constraint in self.constraints:
-            is_valid = constraint(partition)
-            if is_valid is False:
-                return False
-            elif is_valid is True:
-                pass
-            else:
-                raise TypeError(
-                    "Constraint {} returned a non-boolean.".format(repr(constraint))
-                )
-
-        # all constraints are satisfied
-        return True
-
-
-def within_percent_of_ideal_population(
-    initial_partition, percent=0.01, pop_key="population"
-):
-    """Require that all districts are within a certain percent of "ideal" (i.e.,
-    uniform) population.
-
-    Ideal population is defined as "total population / number of districts."
-
-    :param initial_partition: Starting partition from which to compute district information.
-    :param percent: (optional) Allowed percentage deviation. Default is 1%.
-    :param pop_key: (optional) The name of the population
-        :class:`Tally <gerrychain.updaters.Tally>`. Default is ``"population"``.
-    :return: A :class:`.Bounds` constraint on the population attribute identified
-        by ``pop_key``.
-    """
-
-    def population(partition):
-        return partition[pop_key].values()
-
-    number_of_districts = len(initial_partition[pop_key].keys())
-    total_population = sum(initial_partition[pop_key].values())
-    ideal_population = total_population / number_of_districts
-    bounds = ((1 - percent) * ideal_population, (1 + percent) * ideal_population)
-
-    return Bounds(population, bounds=bounds)
-
-
-def deviation_from_ideal(partition, attribute="population"):
-    """Computes the deviation of the given ``attribute`` from exact equality
-    among parts of the partition. Usually ``attribute`` is the population, and
-    this function is used to compute how far a districting plan is from exact population
-    equality.
-
-    By "deviation" we mean ``(actual_value - ideal)/ideal`` (not the absolute value).
-
-    :param partition: A partition.
-    :param attribute: (optional) The :class:`Tally <gerrychain.updaters.Tally>` to
-        compute deviation for. Default is ``"population"``.
-    :return: dictionary from parts to their deviation
-    """
-    number_of_districts = len(partition[attribute].keys())
-    total = sum(partition[attribute].values())
-    ideal = total / number_of_districts
-
-    return {
-        part: (value - ideal) / ideal for part, value in partition[attribute].items()
-    }
-
-
-def districts_within_tolerance(partition, attribute_name="population", percentage=0.1):
-    """Check if all districts are within a certain percentage of the "smallest"
-    district, as defined by the given attribute.
-
-    :param partition: partition class instance
-    :param attrName: string that is the name of an updater in partition
-    :param percentage: what percent difference is allowed
-    :return: whether the districts are within specified tolerance
-    :rtype: bool
-    """
-    if percentage >= 1:
-        percentage *= 0.01
-
-    values = partition[attribute_name].values()
-    max_difference = max(values) - min(values)
-
-    within_tolerance = max_difference <= percentage * min(values)
-    return within_tolerance
-
-
-def refuse_new_splits(partition_county_field):
-    """Refuse all proposals that split a county that was previous unsplit.
-
-    :param partition_county_field: Name of field for county information generated by
-        :func:`.county_splits`.
-    """
-
-    def _refuse_new_splits(partition):
-        for county_info in partition[partition_county_field].values():
-            if county_info.split == CountySplit.NEW_SPLIT:
-                return False
-
-        return True
-
-    return _refuse_new_splits
-
-
-def no_vanishing_districts(partition):
-    """Require that no districts be completely consumed."""
-    if not partition.parent:
-        return True
-    return all(len(part) > 0 for part in partition.assignment.parts.values())
+from ..updaters import CountySplit
+from .bounds import Bounds
+
+
+class Validator:
+    """A single callable for checking that a partition passes a collection of
+    constraints. Intended to be passed as the ``is_valid`` parameter when
+    instantiating :class:`~gerrychain.MarkovChain`.
+
+    This class is meant to be called as a function after instantiation; its
+    return is ``True`` if all validators pass, and ``False`` if any one fails.
+
+    Example usage::
+
+        is_valid = Validator([constraint1, constraint2, constraint3])
+        chain = MarkovChain(proposal, is_valid, accept, initial_state, total_steps)
+    """
+
+    def __init__(self, constraints):
+        """
+        :param constraints: List of validator functions that will check partitions.
+        """
+        self.constraints = constraints
+
+    def __call__(self, partition):
+        """Determine if the given partition is valid.
+
+        :param partition: :class:`Partition` class to check.
+
+        """
+        # check each constraint function and fail when a constraint test fails
+        for constraint in self.constraints:
+            is_valid = constraint(partition)
+            if is_valid is False:
+                return False
+            elif is_valid is True:
+                pass
+            else:
+                raise TypeError(
+                    "Constraint {} returned a non-boolean.".format(repr(constraint))
+                )
+
+        # all constraints are satisfied
+        return True
+
+
+def within_percent_of_ideal_population(
+    initial_partition, percent=0.01, pop_key="population"
+):
+    """Require that all districts are within a certain percent of "ideal" (i.e.,
+    uniform) population.
+
+    Ideal population is defined as "total population / number of districts."
+
+    :param initial_partition: Starting partition from which to compute district information.
+    :param percent: (optional) Allowed percentage deviation. Default is 1%.
+    :param pop_key: (optional) The name of the population
+        :class:`Tally <gerrychain.updaters.Tally>`. Default is ``"population"``.
+    :return: A :class:`.Bounds` constraint on the population attribute identified
+        by ``pop_key``.
+    """
+
+    def population(partition):
+        return partition[pop_key].values()
+
+    number_of_districts = len(initial_partition[pop_key].keys())
+    total_population = sum(initial_partition[pop_key].values())
+    ideal_population = total_population / number_of_districts
+    bounds = ((1 - percent) * ideal_population, (1 + percent) * ideal_population)
+
+    return Bounds(population, bounds=bounds)
+
+
+def deviation_from_ideal(partition, attribute="population"):
+    """Computes the deviation of the given ``attribute`` from exact equality
+    among parts of the partition. Usually ``attribute`` is the population, and
+    this function is used to compute how far a districting plan is from exact population
+    equality.
+
+    By "deviation" we mean ``(actual_value - ideal)/ideal`` (not the absolute value).
+
+    :param partition: A partition.
+    :param attribute: (optional) The :class:`Tally <gerrychain.updaters.Tally>` to
+        compute deviation for. Default is ``"population"``.
+    :return: dictionary from parts to their deviation
+    """
+    number_of_districts = len(partition[attribute].keys())
+    total = sum(partition[attribute].values())
+    ideal = total / number_of_districts
+
+    return {
+        part: (value - ideal) / ideal for part, value in partition[attribute].items()
+    }
+
+
+def districts_within_tolerance(partition, attribute_name="population", percentage=0.1):
+    """Check if all districts are within a certain percentage of the "smallest"
+    district, as defined by the given attribute.
+
+    :param partition: partition class instance
+    :param attrName: string that is the name of an updater in partition
+    :param percentage: what percent difference is allowed
+    :return: whether the districts are within specified tolerance
+    :rtype: bool
+    """
+    if percentage >= 1:
+        percentage *= 0.01
+
+    values = partition[attribute_name].values()
+    max_difference = max(values) - min(values)
+
+    within_tolerance = max_difference <= percentage * min(values)
+    return within_tolerance
+
+
+def refuse_new_splits(partition_county_field):
+    """Refuse all proposals that split a county that was previous unsplit.
+
+    :param partition_county_field: Name of field for county information generated by
+        :func:`.county_splits`.
+    """
+
+    def _refuse_new_splits(partition):
+        for county_info in partition[partition_county_field].values():
+            if county_info.split == CountySplit.NEW_SPLIT:
+                return False
+
+        return True
+
+    return _refuse_new_splits
+
+
+def no_vanishing_districts(partition):
+    """Require that no districts be completely consumed."""
+    if not partition.parent:
+        return True
+    return all(len(part) > 0 for part in partition.assignment.parts.values())
```

### Comparing `gerrychain-0.2.8/gerrychain/graph/geo.py` & `gerrychain-0.2.9/gerrychain/graph/geo.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from collections import Counter
-from shapely.validation import explain_validity
-from gerrychain.vendor.utm import from_latlon
-
-
-def utm_of_point(point):
-    return from_latlon(point.y, point.x)[2]
-
-
-def identify_utm_zone(df):
-    wgs_df = df.to_crs("+proj=longlat +ellps=WGS84 +datum=WGS84 +no_defs")
-    utm_counts = Counter(utm_of_point(point) for point in wgs_df["geometry"].centroid)
-    # most_common returns a list of tuples, and we want the 0,0th entry
-    most_common = utm_counts.most_common(1)[0][0]
-    return most_common
-
-
-def invalid_geometries(df):
-    """Given a GeoDataFrame, returns a list of row indices
-    with invalid geometries.
-
-    :param df: :class:`geopandas.GeoDataFrame`
-    :rtype: list of int
-    """
-    invalid = []
-    for idx, row in df.iterrows():
-        validity = explain_validity(row.geometry)
-        if validity != "Valid Geometry":
-            invalid.append(idx)
-    return invalid
-
-
-def reprojected(df):
-    """Returns a copy of `df`, projected into the coordinate reference system of a suitable
-        `Universal Transverse Mercator`_ zone.
-    :param df: :class:`geopandas.GeoDataFrame`
-    :rtype: :class:`geopandas.GeoDataFrame`
-
-    .. _`Universal Transverse Mercator`: https://en.wikipedia.org/wiki/UTM_coordinate_system
-    """
-    utm = identify_utm_zone(df)
-    return df.to_crs(
-        "+proj=utm +zone={utm} +ellps=WGS84 +datum=WGS84 +units=m +no_defs".format(
-            utm=utm
-        )
-    )
-
-
-class GeometryError(Exception):
-    """
-    Wrapper error class for projection failures.
-    Changing a map's projection may create invalid geometries, which may
-    or may not be repairable using the `.buffer(0)`_ trick.
-
-    .. _`.buffer(0)`: https://shapely.readthedocs.io/en/stable/manual.html#constructive-methods
-    """
+from collections import Counter
+from shapely.validation import explain_validity
+from gerrychain.vendor.utm import from_latlon
+
+
+def utm_of_point(point):
+    return from_latlon(point.y, point.x)[2]
+
+
+def identify_utm_zone(df):
+    wgs_df = df.to_crs("+proj=longlat +ellps=WGS84 +datum=WGS84 +no_defs")
+    utm_counts = Counter(utm_of_point(point) for point in wgs_df["geometry"].centroid)
+    # most_common returns a list of tuples, and we want the 0,0th entry
+    most_common = utm_counts.most_common(1)[0][0]
+    return most_common
+
+
+def invalid_geometries(df):
+    """Given a GeoDataFrame, returns a list of row indices
+    with invalid geometries.
+
+    :param df: :class:`geopandas.GeoDataFrame`
+    :rtype: list of int
+    """
+    invalid = []
+    for idx, row in df.iterrows():
+        validity = explain_validity(row.geometry)
+        if validity != "Valid Geometry":
+            invalid.append(idx)
+    return invalid
+
+
+def reprojected(df):
+    """Returns a copy of `df`, projected into the coordinate reference system of a suitable
+        `Universal Transverse Mercator`_ zone.
+    :param df: :class:`geopandas.GeoDataFrame`
+    :rtype: :class:`geopandas.GeoDataFrame`
+
+    .. _`Universal Transverse Mercator`: https://en.wikipedia.org/wiki/UTM_coordinate_system
+    """
+    utm = identify_utm_zone(df)
+    return df.to_crs(
+        "+proj=utm +zone={utm} +ellps=WGS84 +datum=WGS84 +units=m +no_defs".format(
+            utm=utm
+        )
+    )
+
+
+class GeometryError(Exception):
+    """
+    Wrapper error class for projection failures.
+    Changing a map's projection may create invalid geometries, which may
+    or may not be repairable using the `.buffer(0)`_ trick.
+
+    .. _`.buffer(0)`: https://shapely.readthedocs.io/en/stable/manual.html#constructive-methods
+    """
```

### Comparing `gerrychain-0.2.8/gerrychain/graph/graph.py` & `gerrychain-0.2.9/gerrychain/graph/graph.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,284 +1,289 @@
-import json
-import warnings
-
-import geopandas as gp
-import networkx
-from networkx.readwrite import json_graph
-from shapely.ops import unary_union
-from shapely.prepared import prep
-
-from .adjacency import neighbors
-from .geo import GeometryError, invalid_geometries, reprojected
-
-
-class Graph(networkx.Graph):
-    """Represents a graph to be partitioned. It is based on :class:`networkx.Graph`.
-
-    We have added some classmethods to help construct graphs from shapefiles, and
-    to save and load graphs as JSON files.
-    """
-
-    @classmethod
-    def from_json(cls, json_file):
-        """Load a graph from a JSON file in the NetworkX json_graph format.
-        :param json_file: Path to JSON file.
-        :return: Graph
-        """
-        with open(json_file) as f:
-            data = json.load(f)
-        g = json_graph.adjacency_graph(data)
-        graph = cls(g)
-        graph.issue_warnings()
-        return graph
-
-    def to_json(self, json_file, *, include_geometries_as_geojson=False):
-        """Save a graph to a JSON file in the NetworkX json_graph format.
-        :param json_file: Path to target JSON file.
-        :param bool include_geometry_as_geojson: (optional) Whether to include any
-            :mod:`shapely` geometry objects encountered in the graph's node attributes
-            as GeoJSON. The default (``False``) behavior is to remove all geometry
-            objects because they are not serializable. Including the GeoJSON will result
-            in a much larger JSON file.
-        """
-        data = json_graph.adjacency_data(self)
-
-        if include_geometries_as_geojson:
-            convert_geometries_to_geojson(data)
-        else:
-            remove_geometries(data)
-
-        with open(json_file, "w") as f:
-            json.dump(data, f)
-
-    @classmethod
-    def from_file(
-        cls,
-        filename,
-        adjacency="rook",
-        cols_to_add=None,
-        reproject=True,
-        ignore_errors=False,
-    ):
-        """Create a :class:`Graph` from a shapefile (or GeoPackage, or GeoJSON, or
-        any other library that :mod:`geopandas` can read. See :meth:`from_geodataframe`
-        for more details.
-
-        :param cols_to_add: (optional) The names of the columns that you want to
-            add to the graph as node attributes. By default, all columns are added.
-        """
-        df = gp.read_file(filename)
-        graph = cls.from_geodataframe(df, adjacency, reproject)
-        graph.add_data(df, columns=cols_to_add)
-        return graph
-
-    @classmethod
-    def from_geodataframe(
-        cls, dataframe, adjacency="rook", reproject=True, ignore_errors=False
-    ):
-        """Creates the adjacency :class:`Graph` of geometries described by `dataframe`.
-        The areas of the polygons are included as node attributes (with key `area`).
-        The shared perimeter of neighboring polygons are included as edge attributes
-        (with key `shared_perim`).
-        Nodes corresponding to polygons on the boundary of the union of all the geometries
-        (e.g., the state, if your dataframe describes VTDs) have a `boundary_node` attribute
-        (set to `True`) and a `boundary_perim` attribute with the length of this "exterior"
-        boundary.
-
-        By default, areas and lengths are computed in a UTM projection suitable for the
-        geometries. This prevents the bizarro area and perimeter values that show up when
-        you accidentally do computations in Longitude-Latitude coordinates. If the user
-        specifies `reproject=False`, then the areas and lengths will be computed in the
-        GeoDataFrame's current coordinate reference system. This option is for users who
-        have a preferred CRS they would like to use.
-
-        :param dataframe: :class:`geopandas.GeoDataFrame`
-        :param adjacency: (optional) The adjacency type to use ("rook" or "queen").
-            Default is "rook".
-        :param reproject: (optional) Whether to reproject to a UTM projection before
-            creating the graph. Default is ``True``.
-        :param ignore_errors: (optional) Whether to ignore all invalid geometries and
-            attept to create the graph anyway. Default is ``False``.
-        :return: The adjacency graph of the geometries from `dataframe`.
-        :rtype: :class:`Graph`
-        """
-        # Validate geometries before reprojection
-        invalid = invalid_geometries(dataframe)
-        if invalid and not ignore_errors:
-            raise GeometryError(
-                "Invalid geometries at rows {} before "
-                "reprojection. Consider repairing the affected geometries with "
-                "`.buffer(0)`, or pass `ignore_errors=True` to attempt to create "
-                "the graph anyways.".format(invalid)
-            )
-
-        # Project the dataframe to an appropriate UTM projection unless
-        # explicitly told not to.
-        if reproject:
-            df = reprojected(dataframe)
-            invalid_reproj = invalid_geometries(df)
-            if invalid_reproj and not ignore_errors:
-                raise GeometryError(
-                    "Invalid geometries at rows {} after "
-                    "reprojection. Consider reloading the GeoDataFrame with "
-                    "`reproject=False` or repairing the affected geometries "
-                    "with `.buffer(0)`.".format(invalid_reproj)
-                )
-        else:
-            df = dataframe
-
-        # Generate dict of dicts of dicts with shared perimeters according
-        # to the requested adjacency rule
-        adjacencies = neighbors(df, adjacency)
-        graph = cls(adjacencies)
-
-        graph.issue_warnings()
-
-        # Add "exterior" perimeters to the boundary nodes
-        add_boundary_perimeters(graph, df.geometry)
-
-        # Add area data to the nodes
-        areas = df.geometry.area.to_dict()
-        networkx.set_node_attributes(graph, name="area", values=areas)
-
-        return graph
-
-    def add_data(self, df, columns=None):
-        """Add columns of a DataFrame to a graph as node attributes using
-        by matching the DataFrame's index to node ids.
-
-        :param df: Dataframe containing given columns.
-        :param columns: (optional) List of dataframe column names to add.
-        """
-
-        if columns is None:
-            columns = df.columns
-
-        check_dataframe(df[columns])
-
-        column_dictionaries = df.to_dict("index")
-        networkx.set_node_attributes(self, column_dictionaries)
-
-    def join(self, dataframe, columns=None, left_index=None, right_index=None):
-        """Add data from a dataframe to the graph, matching nodes to rows when
-        the node's `left_index` attribute equals the row's `right_index` value.
-
-        :param dataframe: DataFrame.
-        :columns: (optional) The columns whose data you wish to add to the graph.
-            If not provided, all columns are added.
-        :left_index: (optional) The node attribute used to match nodes to rows.
-            If not provided, node IDs are used.
-        :right_index: (optional) The DataFrame column name to use to match rows
-            to nodes. If not provided, the DataFrame's index is used.
-        """
-        if right_index is not None:
-            df = dataframe.set_index(right_index)
-        else:
-            df = dataframe
-
-        if columns is not None:
-            df = df[columns]
-
-        check_dataframe(df)
-
-        column_dictionaries = df.to_dict()
-
-        if left_index is not None:
-            ids_to_index = networkx.get_node_attributes(self, left_index)
-        else:
-            # When the left_index is node ID, the matching is just
-            # a redundant {node: node} dictionary
-            ids_to_index = dict(zip(self.nodes, self.nodes))
-
-        node_attributes = {
-            node_id: {
-                column: values[index] for column, values in column_dictionaries.items()
-            }
-            for node_id, index in ids_to_index.items()
-        }
-
-        networkx.set_node_attributes(self, node_attributes)
-
-    @property
-    def islands(self):
-        """The set of degree-0 nodes."""
-        return set(node for node in self if self.degree[node] == 0)
-
-    def warn_for_islands(self):
-        """Issue a warning if the graph has any islands (degree-0 nodes)."""
-        islands = self.islands
-        if len(self.islands) > 0:
-            warnings.warn(
-                "Found islands (degree-0 nodes). Indices of islands: {}".format(islands)
-            )
-
-    def issue_warnings(self):
-        """Issue warnings if the graph has any red flags (right now, only islands)."""
-        self.warn_for_islands()
-
-
-def add_boundary_perimeters(graph, geometries):
-    """Add shared perimeter between nodes and the total geometry boundary.
-
-    :param graph: NetworkX graph
-    :param df: Geodataframe containing geometry information.
-    :return: The updated graph.
-    """
-    prepared_boundary = prep(unary_union(geometries).boundary)
-
-    boundary_nodes = geometries.boundary.apply(prepared_boundary.intersects)
-
-    for node in graph:
-        graph.nodes[node]["boundary_node"] = bool(boundary_nodes[node])
-        if boundary_nodes[node]:
-            total_perimeter = geometries[node].boundary.length
-            shared_perimeter = sum(
-                neighbor_data["shared_perim"] for neighbor_data in graph[node].values()
-            )
-            boundary_perimeter = total_perimeter - shared_perimeter
-            graph.nodes[node]["boundary_perim"] = boundary_perimeter
-
-
-def check_dataframe(df):
-    for column in df.columns:
-        if sum(df[column].isna()) > 0:
-            warnings.warn("NA values found in column {}!".format(column))
-
-
-def remove_geometries(data):
-    """Remove geometry attributes from NetworkX adjacency data object,
-    because they are not serializable. Mutates the ``data`` object.
-
-    Does nothing if no geometry attributes are found.
-
-    :param data: an adjacency data object (returned by
-        :func:`networkx.readwrite.json_graph.adjacency_data`)
-    """
-    for node in data["nodes"]:
-        bad_keys = []
-        for key in node:
-            # having a ``__geo_interface__``` property identifies the object
-            # as being a ``shapely`` geometry object
-            if hasattr(node[key], "__geo_interface__"):
-                bad_keys.append(key)
-        for key in bad_keys:
-            del node[key]
-
-
-def convert_geometries_to_geojson(data):
-    """Convert geometry attributes in a NetworkX adjacency data object
-    to GeoJSON, so that they can be serialized. Mutates the ``data`` object.
-
-    Does nothing if no geometry attributes are found.
-
-    :param data: an adjacency data object (returned by
-        :func:`networkx.readwrite.json_graph.adjacency_data`)
-    """
-    for node in data["nodes"]:
-        for key in node:
-            # having a ``__geo_interface__``` property identifies the object
-            # as being a ``shapely`` geometry object
-            if hasattr(node[key], "__geo_interface__"):
-                # The ``__geo_interface__`` property is essentially GeoJSON.
-                # This is what :func:`geopandas.GeoSeries.to_json` uses under
-                # the hood.
-                node[key] = node[key].__geo_interface__
+import json
+import warnings
+
+import geopandas as gp
+import networkx
+from networkx.readwrite import json_graph
+from shapely.ops import unary_union
+from shapely.prepared import prep
+
+from .adjacency import neighbors
+from .geo import GeometryError, invalid_geometries, reprojected
+
+
+class Graph(networkx.Graph):
+    """Represents a graph to be partitioned. It is based on :class:`networkx.Graph`.
+
+    We have added some classmethods to help construct graphs from shapefiles, and
+    to save and load graphs as JSON files.
+    """
+
+    def __repr__(self):
+        return "<Graph [{} nodes, {} edges]>".format(len(self.nodes), len(self.edges))
+
+    @classmethod
+    def from_json(cls, json_file):
+        """Load a graph from a JSON file in the NetworkX json_graph format.
+        :param json_file: Path to JSON file.
+        :return: Graph
+        """
+        with open(json_file) as f:
+            data = json.load(f)
+        g = json_graph.adjacency_graph(data)
+        graph = cls(g)
+        graph.issue_warnings()
+        return graph
+
+    def to_json(self, json_file, *, include_geometries_as_geojson=False):
+        """Save a graph to a JSON file in the NetworkX json_graph format.
+        :param json_file: Path to target JSON file.
+        :param bool include_geometry_as_geojson: (optional) Whether to include any
+            :mod:`shapely` geometry objects encountered in the graph's node attributes
+            as GeoJSON. The default (``False``) behavior is to remove all geometry
+            objects because they are not serializable. Including the GeoJSON will result
+            in a much larger JSON file.
+        """
+        data = json_graph.adjacency_data(self)
+
+        if include_geometries_as_geojson:
+            convert_geometries_to_geojson(data)
+        else:
+            remove_geometries(data)
+
+        with open(json_file, "w") as f:
+            json.dump(data, f)
+
+    @classmethod
+    def from_file(
+        cls,
+        filename,
+        adjacency="rook",
+        cols_to_add=None,
+        reproject=True,
+        ignore_errors=False,
+    ):
+        """Create a :class:`Graph` from a shapefile (or GeoPackage, or GeoJSON, or
+        any other library that :mod:`geopandas` can read. See :meth:`from_geodataframe`
+        for more details.
+
+        :param cols_to_add: (optional) The names of the columns that you want to
+            add to the graph as node attributes. By default, all columns are added.
+        """
+        df = gp.read_file(filename)
+        graph = cls.from_geodataframe(
+            df, adjacency=adjacency, reproject=reproject, ignore_errors=ignore_errors
+        )
+        graph.add_data(df, columns=cols_to_add)
+        return graph
+
+    @classmethod
+    def from_geodataframe(
+        cls, dataframe, adjacency="rook", reproject=True, ignore_errors=False
+    ):
+        """Creates the adjacency :class:`Graph` of geometries described by `dataframe`.
+        The areas of the polygons are included as node attributes (with key `area`).
+        The shared perimeter of neighboring polygons are included as edge attributes
+        (with key `shared_perim`).
+        Nodes corresponding to polygons on the boundary of the union of all the geometries
+        (e.g., the state, if your dataframe describes VTDs) have a `boundary_node` attribute
+        (set to `True`) and a `boundary_perim` attribute with the length of this "exterior"
+        boundary.
+
+        By default, areas and lengths are computed in a UTM projection suitable for the
+        geometries. This prevents the bizarro area and perimeter values that show up when
+        you accidentally do computations in Longitude-Latitude coordinates. If the user
+        specifies `reproject=False`, then the areas and lengths will be computed in the
+        GeoDataFrame's current coordinate reference system. This option is for users who
+        have a preferred CRS they would like to use.
+
+        :param dataframe: :class:`geopandas.GeoDataFrame`
+        :param adjacency: (optional) The adjacency type to use ("rook" or "queen").
+            Default is "rook".
+        :param reproject: (optional) Whether to reproject to a UTM projection before
+            creating the graph. Default is ``True``.
+        :param ignore_errors: (optional) Whether to ignore all invalid geometries and
+            attept to create the graph anyway. Default is ``False``.
+        :return: The adjacency graph of the geometries from `dataframe`.
+        :rtype: :class:`Graph`
+        """
+        # Validate geometries before reprojection
+        invalid = invalid_geometries(dataframe)
+        if invalid and not ignore_errors:
+            raise GeometryError(
+                "Invalid geometries at rows {} before "
+                "reprojection. Consider repairing the affected geometries with "
+                "`.buffer(0)`, or pass `ignore_errors=True` to attempt to create "
+                "the graph anyways.".format(invalid)
+            )
+
+        # Project the dataframe to an appropriate UTM projection unless
+        # explicitly told not to.
+        if reproject:
+            df = reprojected(dataframe)
+            invalid_reproj = invalid_geometries(df)
+            if invalid_reproj and not ignore_errors:
+                raise GeometryError(
+                    "Invalid geometries at rows {} after "
+                    "reprojection. Consider reloading the GeoDataFrame with "
+                    "`reproject=False` or repairing the affected geometries "
+                    "with `.buffer(0)`.".format(invalid_reproj)
+                )
+        else:
+            df = dataframe
+
+        # Generate dict of dicts of dicts with shared perimeters according
+        # to the requested adjacency rule
+        adjacencies = neighbors(df, adjacency)
+        graph = cls(adjacencies)
+
+        graph.issue_warnings()
+
+        # Add "exterior" perimeters to the boundary nodes
+        add_boundary_perimeters(graph, df.geometry)
+
+        # Add area data to the nodes
+        areas = df.geometry.area.to_dict()
+        networkx.set_node_attributes(graph, name="area", values=areas)
+
+        return graph
+
+    def add_data(self, df, columns=None):
+        """Add columns of a DataFrame to a graph as node attributes using
+        by matching the DataFrame's index to node ids.
+
+        :param df: Dataframe containing given columns.
+        :param columns: (optional) List of dataframe column names to add.
+        """
+
+        if columns is None:
+            columns = df.columns
+
+        check_dataframe(df[columns])
+
+        column_dictionaries = df.to_dict("index")
+        networkx.set_node_attributes(self, column_dictionaries)
+
+    def join(self, dataframe, columns=None, left_index=None, right_index=None):
+        """Add data from a dataframe to the graph, matching nodes to rows when
+        the node's `left_index` attribute equals the row's `right_index` value.
+
+        :param dataframe: DataFrame.
+        :columns: (optional) The columns whose data you wish to add to the graph.
+            If not provided, all columns are added.
+        :left_index: (optional) The node attribute used to match nodes to rows.
+            If not provided, node IDs are used.
+        :right_index: (optional) The DataFrame column name to use to match rows
+            to nodes. If not provided, the DataFrame's index is used.
+        """
+        if right_index is not None:
+            df = dataframe.set_index(right_index)
+        else:
+            df = dataframe
+
+        if columns is not None:
+            df = df[columns]
+
+        check_dataframe(df)
+
+        column_dictionaries = df.to_dict()
+
+        if left_index is not None:
+            ids_to_index = networkx.get_node_attributes(self, left_index)
+        else:
+            # When the left_index is node ID, the matching is just
+            # a redundant {node: node} dictionary
+            ids_to_index = dict(zip(self.nodes, self.nodes))
+
+        node_attributes = {
+            node_id: {
+                column: values[index] for column, values in column_dictionaries.items()
+            }
+            for node_id, index in ids_to_index.items()
+        }
+
+        networkx.set_node_attributes(self, node_attributes)
+
+    @property
+    def islands(self):
+        """The set of degree-0 nodes."""
+        return set(node for node in self if self.degree[node] == 0)
+
+    def warn_for_islands(self):
+        """Issue a warning if the graph has any islands (degree-0 nodes)."""
+        islands = self.islands
+        if len(self.islands) > 0:
+            warnings.warn(
+                "Found islands (degree-0 nodes). Indices of islands: {}".format(islands)
+            )
+
+    def issue_warnings(self):
+        """Issue warnings if the graph has any red flags (right now, only islands)."""
+        self.warn_for_islands()
+
+
+def add_boundary_perimeters(graph, geometries):
+    """Add shared perimeter between nodes and the total geometry boundary.
+
+    :param graph: NetworkX graph
+    :param df: Geodataframe containing geometry information.
+    :return: The updated graph.
+    """
+    prepared_boundary = prep(unary_union(geometries).boundary)
+
+    boundary_nodes = geometries.boundary.apply(prepared_boundary.intersects)
+
+    for node in graph:
+        graph.nodes[node]["boundary_node"] = bool(boundary_nodes[node])
+        if boundary_nodes[node]:
+            total_perimeter = geometries[node].boundary.length
+            shared_perimeter = sum(
+                neighbor_data["shared_perim"] for neighbor_data in graph[node].values()
+            )
+            boundary_perimeter = total_perimeter - shared_perimeter
+            graph.nodes[node]["boundary_perim"] = boundary_perimeter
+
+
+def check_dataframe(df):
+    for column in df.columns:
+        if sum(df[column].isna()) > 0:
+            warnings.warn("NA values found in column {}!".format(column))
+
+
+def remove_geometries(data):
+    """Remove geometry attributes from NetworkX adjacency data object,
+    because they are not serializable. Mutates the ``data`` object.
+
+    Does nothing if no geometry attributes are found.
+
+    :param data: an adjacency data object (returned by
+        :func:`networkx.readwrite.json_graph.adjacency_data`)
+    """
+    for node in data["nodes"]:
+        bad_keys = []
+        for key in node:
+            # having a ``__geo_interface__``` property identifies the object
+            # as being a ``shapely`` geometry object
+            if hasattr(node[key], "__geo_interface__"):
+                bad_keys.append(key)
+        for key in bad_keys:
+            del node[key]
+
+
+def convert_geometries_to_geojson(data):
+    """Convert geometry attributes in a NetworkX adjacency data object
+    to GeoJSON, so that they can be serialized. Mutates the ``data`` object.
+
+    Does nothing if no geometry attributes are found.
+
+    :param data: an adjacency data object (returned by
+        :func:`networkx.readwrite.json_graph.adjacency_data`)
+    """
+    for node in data["nodes"]:
+        for key in node:
+            # having a ``__geo_interface__``` property identifies the object
+            # as being a ``shapely`` geometry object
+            if hasattr(node[key], "__geo_interface__"):
+                # The ``__geo_interface__`` property is essentially GeoJSON.
+                # This is what :func:`geopandas.GeoSeries.to_json` uses under
+                # the hood.
+                node[key] = node[key].__geo_interface__
```

### Comparing `gerrychain-0.2.8/gerrychain/grid.py` & `gerrychain-0.2.9/gerrychain/grid.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,176 +1,183 @@
-import math
-
-import networkx
-
-from gerrychain.partition import Partition
-from gerrychain.updaters import (Tally, boundary_nodes, cut_edges,
-                                 cut_edges_by_part, exterior_boundaries,
-                                 interior_boundaries, perimeter, polsby_popper)
-
-
-class Grid(Partition):
-    """
-    The :class:`Grid` class represents a grid partitioned into districts.
-    It is useful for running little experiments with GerryChain without needing to do
-    any data processing or cleaning to get started.
-
-    Example usage::
-
-        grid = Grid((10,10))
-
-    The nodes of ``grid.graph`` are labelled by tuples ``(i,j)``, for ``0 <= i <= 10``
-    and ``0 <= j <= 10``. Each node has an ``area`` of 1 and each edge has ``shared_perim`` 1.
-    """
-
-    default_updaters = {
-        "cut_edges": cut_edges,
-        "population": Tally("population"),
-        "perimeter": perimeter,
-        "exterior_boundaries": exterior_boundaries,
-        "interior_boundaries": interior_boundaries,
-        "boundary_nodes": boundary_nodes,
-        "area": Tally("area", alias="area"),
-        "polsby_popper": polsby_popper,
-        "cut_edges_by_part": cut_edges_by_part,
-    }
-
-    def __init__(
-        self,
-        dimensions=None,
-        with_diagonals=False,
-        assignment=None,
-        updaters=None,
-        parent=None,
-        flips=None,
-    ):
-        """
-        :param dimensions: tuple (m,n) of the desired dimensions of the grid.
-        :param with_diagonals: (optional, defaults to False) whether to include diagonals
-            as edges of the graph (i.e., whether to use 'queen' adjacency rather than
-            'rook' adjacency).
-        :param assignment: (optional) dict matching nodes to their districts. If not
-            provided, partitions the grid into 4 quarters of roughly equal size.
-        :param updaters: (optional) dict matching names of attributes of the Partition
-            to functions that compute their values. If not provided, the Grid
-            configures the cut_edges updater for convenience.
-        """
-        if dimensions:
-            self.dimensions = dimensions
-            graph = create_grid_graph(dimensions, with_diagonals)
-
-            if not assignment:
-                thresholds = tuple(math.floor(n / 2) for n in self.dimensions)
-                assignment = {
-                    node: color_quadrants(node, thresholds) for node in graph.nodes
-                }
-
-            if not updaters:
-                updaters = dict()
-            updaters.update(self.default_updaters)
-
-            super().__init__(graph, assignment, updaters)
-        elif parent:
-            self.dimensions = parent.dimensions
-            super().__init__(parent=parent, flips=flips)
-        else:
-            raise Exception("Not a good way to create a Partition")
-
-    def __str__(self):
-        rows = self.as_list_of_lists()
-        return "\n".join(["".join([str(x) for x in row]) for row in rows]) + "\n"
-
-    def __repr__(self):
-        dims = "x".join(str(d) for d in self.dimensions)
-        number_of_parts = len(self.parts)
-        s = "s" if number_of_parts > 1 else ""
-        return "{} Grid\nPartitioned into {} part{}".format(dims, number_of_parts, s)
-
-    def as_list_of_lists(self):
-        """
-        Returns the grid as a list of lists (like a matrix), where the (i,j)th
-        entry is the assigned district of the node in position (i,j) on the
-        grid.
-        """
-        m, n = self.dimensions
-        return [[self.assignment[(i, j)] for i in range(m)] for j in range(n)]
-
-
-def create_grid_graph(dimensions, with_diagonals):
-    if len(dimensions) != 2:
-        raise ValueError("Expected two dimensions.")
-    m, n = dimensions
-    graph = networkx.generators.lattice.grid_2d_graph(m, n)
-
-    networkx.set_edge_attributes(graph, 1, "shared_perim")
-
-    if with_diagonals:
-        nw_to_se = [
-            ((i, j), (i + 1, j + 1)) for i in range(m - 1) for j in range(n - 1)
-        ]
-        sw_to_ne = [
-            ((i, j + 1), (i + 1, j)) for i in range(m - 1) for j in range(n - 1)
-        ]
-        diagonal_edges = nw_to_se + sw_to_ne
-        graph.add_edges_from(diagonal_edges)
-        for edge in diagonal_edges:
-            graph.edges[edge]["shared_perim"] = 0
-
-    networkx.set_node_attributes(graph, 1, "population")
-    networkx.set_node_attributes(graph, 1, "area")
-
-    tag_boundary_nodes(graph, dimensions)
-
-    return graph
-
-
-def give_constant_attribute(graph, attribute, value):
-    for node in graph.nodes:
-        graph.nodes[node][attribute] = value
-
-
-def tag_boundary_nodes(graph, dimensions):
-    m, n = dimensions
-    for node in graph.nodes:
-        if node[0] in [0, m - 1] or node[1] in [0, n - 1]:
-            graph.nodes[node]["boundary_node"] = True
-            graph.nodes[node]["boundary_perim"] = get_boundary_perim(node, dimensions)
-        else:
-            graph.nodes[node]["boundary_node"] = False
-
-
-def get_boundary_perim(node, dimensions):
-    m, n = dimensions
-    if node in [(0, 0), (m - 1, 0), (0, n - 1), (m - 1, n - 1)]:
-        return 2
-    elif node[0] in [0, m - 1] or node[1] in [0, n - 1]:
-        return 1
-    else:
-        return 0
-
-
-def color_half(node, threshold=5):
-    x = node[0]
-    return 0 if x <= threshold else 1
-
-
-def color_quadrants(node, thresholds):
-    x, y = node
-    x_color = 0 if x < thresholds[0] else 1
-    y_color = 0 if y < thresholds[1] else 2
-    return x_color + y_color
-
-
-def grid_size(parition):
-    """ This is a hardcoded population function
-    for the grid class"""
-
-    L = parition.as_list_of_lists()
-    permit = [3, 4, 5]
-
-    sizes = [0, 0, 0, 0]
-
-    for i in range(len(L)):
-        for j in range(len(L[0])):
-            sizes[L[i][j]] += 1
-
-    return all(x in permit for x in sizes)
+import math
+
+import networkx
+
+from gerrychain.partition import Partition
+from gerrychain.updaters import (
+    Tally,
+    boundary_nodes,
+    cut_edges,
+    cut_edges_by_part,
+    exterior_boundaries,
+    interior_boundaries,
+    perimeter,
+)
+from gerrychain.metrics import polsby_popper
+
+
+class Grid(Partition):
+    """
+    The :class:`Grid` class represents a grid partitioned into districts.
+    It is useful for running little experiments with GerryChain without needing to do
+    any data processing or cleaning to get started.
+
+    Example usage::
+
+        grid = Grid((10,10))
+
+    The nodes of ``grid.graph`` are labelled by tuples ``(i,j)``, for ``0 <= i <= 10``
+    and ``0 <= j <= 10``. Each node has an ``area`` of 1 and each edge has ``shared_perim`` 1.
+    """
+
+    default_updaters = {
+        "cut_edges": cut_edges,
+        "population": Tally("population"),
+        "perimeter": perimeter,
+        "exterior_boundaries": exterior_boundaries,
+        "interior_boundaries": interior_boundaries,
+        "boundary_nodes": boundary_nodes,
+        "area": Tally("area", alias="area"),
+        "polsby_popper": polsby_popper,
+        "cut_edges_by_part": cut_edges_by_part,
+    }
+
+    def __init__(
+        self,
+        dimensions=None,
+        with_diagonals=False,
+        assignment=None,
+        updaters=None,
+        parent=None,
+        flips=None,
+    ):
+        """
+        :param dimensions: tuple (m,n) of the desired dimensions of the grid.
+        :param with_diagonals: (optional, defaults to False) whether to include diagonals
+            as edges of the graph (i.e., whether to use 'queen' adjacency rather than
+            'rook' adjacency).
+        :param assignment: (optional) dict matching nodes to their districts. If not
+            provided, partitions the grid into 4 quarters of roughly equal size.
+        :param updaters: (optional) dict matching names of attributes of the Partition
+            to functions that compute their values. If not provided, the Grid
+            configures the cut_edges updater for convenience.
+        """
+        if dimensions:
+            self.dimensions = dimensions
+            graph = create_grid_graph(dimensions, with_diagonals)
+
+            if not assignment:
+                thresholds = tuple(math.floor(n / 2) for n in self.dimensions)
+                assignment = {
+                    node: color_quadrants(node, thresholds) for node in graph.nodes
+                }
+
+            if not updaters:
+                updaters = dict()
+            updaters.update(self.default_updaters)
+
+            super().__init__(graph, assignment, updaters)
+        elif parent:
+            self.dimensions = parent.dimensions
+            super().__init__(parent=parent, flips=flips)
+        else:
+            raise Exception("Not a good way to create a Partition")
+
+    def __str__(self):
+        rows = self.as_list_of_lists()
+        return "\n".join(["".join([str(x) for x in row]) for row in rows]) + "\n"
+
+    def __repr__(self):
+        dims = "x".join(str(d) for d in self.dimensions)
+        number_of_parts = len(self.parts)
+        s = "s" if number_of_parts > 1 else ""
+        return "{} Grid\nPartitioned into {} part{}".format(dims, number_of_parts, s)
+
+    def as_list_of_lists(self):
+        """
+        Returns the grid as a list of lists (like a matrix), where the (i,j)th
+        entry is the assigned district of the node in position (i,j) on the
+        grid.
+        """
+        m, n = self.dimensions
+        return [[self.assignment[(i, j)] for i in range(m)] for j in range(n)]
+
+
+def create_grid_graph(dimensions, with_diagonals):
+    if len(dimensions) != 2:
+        raise ValueError("Expected two dimensions.")
+    m, n = dimensions
+    graph = networkx.generators.lattice.grid_2d_graph(m, n)
+
+    networkx.set_edge_attributes(graph, 1, "shared_perim")
+
+    if with_diagonals:
+        nw_to_se = [
+            ((i, j), (i + 1, j + 1)) for i in range(m - 1) for j in range(n - 1)
+        ]
+        sw_to_ne = [
+            ((i, j + 1), (i + 1, j)) for i in range(m - 1) for j in range(n - 1)
+        ]
+        diagonal_edges = nw_to_se + sw_to_ne
+        graph.add_edges_from(diagonal_edges)
+        for edge in diagonal_edges:
+            graph.edges[edge]["shared_perim"] = 0
+
+    networkx.set_node_attributes(graph, 1, "population")
+    networkx.set_node_attributes(graph, 1, "area")
+
+    tag_boundary_nodes(graph, dimensions)
+
+    return graph
+
+
+def give_constant_attribute(graph, attribute, value):
+    for node in graph.nodes:
+        graph.nodes[node][attribute] = value
+
+
+def tag_boundary_nodes(graph, dimensions):
+    m, n = dimensions
+    for node in graph.nodes:
+        if node[0] in [0, m - 1] or node[1] in [0, n - 1]:
+            graph.nodes[node]["boundary_node"] = True
+            graph.nodes[node]["boundary_perim"] = get_boundary_perim(node, dimensions)
+        else:
+            graph.nodes[node]["boundary_node"] = False
+
+
+def get_boundary_perim(node, dimensions):
+    m, n = dimensions
+    if node in [(0, 0), (m - 1, 0), (0, n - 1), (m - 1, n - 1)]:
+        return 2
+    elif node[0] in [0, m - 1] or node[1] in [0, n - 1]:
+        return 1
+    else:
+        return 0
+
+
+def color_half(node, threshold=5):
+    x = node[0]
+    return 0 if x <= threshold else 1
+
+
+def color_quadrants(node, thresholds):
+    x, y = node
+    x_color = 0 if x < thresholds[0] else 1
+    y_color = 0 if y < thresholds[1] else 2
+    return x_color + y_color
+
+
+def grid_size(parition):
+    """ This is a hardcoded population function
+    for the grid class"""
+
+    L = parition.as_list_of_lists()
+    permit = [3, 4, 5]
+
+    sizes = [0, 0, 0, 0]
+
+    for i in range(len(L)):
+        for j in range(len(L[0])):
+            sizes[L[i][j]] += 1
+
+    return all(x in permit for x in sizes)
```

### Comparing `gerrychain-0.2.8/gerrychain/partition/partition.py` & `gerrychain-0.2.9/gerrychain/partition/partition.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,214 +1,217 @@
-import json
-
-import geopandas
-
-from ..graph import Graph
-from ..updaters import compute_edge_flows, flows_from_changes
-from .assignment import get_assignment
-from .subgraphs import SubgraphView
-
-
-class Partition:
-    """
-    Partition represents a partition of the nodes of the graph. It will perform
-    the first layer of computations at each step in the Markov chain - basic
-    aggregations and calculations that we want to optimize.
-    """
-
-    default_updaters = {}
-
-    def __init__(
-        self, graph=None, assignment=None, updaters=None, parent=None, flips=None
-    ):
-        """
-        :param graph: Underlying graph; a NetworkX object.
-        :param assignment: Dictionary assigning nodes to districts. If None,
-            initialized to assign all nodes to district 0.
-        :param updaters: Dictionary of functions to track data about the partition.
-            The keys are stored as attributes on the partition class,
-            which the functions compute.
-        """
-        if parent is None:
-            self._first_time(graph, assignment, updaters)
-        else:
-            self._from_parent(parent, flips)
-
-        self._cache = dict()
-        self.subgraphs = SubgraphView(self.graph, self.parts)
-
-    def _first_time(self, graph, assignment, updaters):
-        self.graph = graph
-
-        self.assignment = get_assignment(assignment, graph)
-
-        if updaters is None:
-            updaters = dict()
-        self.updaters = self.default_updaters.copy()
-        self.updaters.update(updaters)
-
-        self.parent = None
-        self.flips = None
-        self.flows = None
-        self.edge_flows = None
-
-    def _from_parent(self, parent, flips):
-        self.parent = parent
-        self.flips = flips
-
-        self.assignment = parent.assignment.copy()
-        self.assignment.update(flips)
-
-        self.graph = parent.graph
-        self.updaters = parent.updaters
-
-        self.flows = flows_from_changes(parent.assignment, flips)
-        self.edge_flows = compute_edge_flows(self)
-
-    def __repr__(self):
-        number_of_parts = len(self)
-        s = "s" if number_of_parts > 1 else ""
-        return "Partition of a graph into {} part{}".format(number_of_parts, s)
-
-    def __len__(self):
-        return len(self.parts)
-
-    def flip(self, flips):
-        """Returns the new partition obtained by performing the given `flips`
-        on this partition.
-
-        :param flips: dictionary assigning nodes of the graph to their new districts
-        :return: the new :class:`Partition`
-        :rtype: Partition
-        """
-        return self.__class__(parent=self, flips=flips)
-
-    def crosses_parts(self, edge):
-        """Answers the question "Does this edge cross from one part of the
-        partition to another?
-
-        :param edge: tuple of node IDs
-        :rtype: bool
-        """
-        return self.assignment[edge[0]] != self.assignment[edge[1]]
-
-    def __getitem__(self, key):
-        """Allows accessing the values of updaters computed for this
-        Partition instance.
-
-        :param key: Property to access.
-        """
-        if key not in self._cache:
-            self._cache[key] = self.updaters[key](self)
-        return self._cache[key]
-
-    def __getattr__(self, key):
-        return self[key]
-
-    @property
-    def parts(self):
-        return self.assignment.parts
-
-    def plot(self, geometries, **kwargs):
-        """Plot the partition, using the provided geometries.
-
-        :param geometries: A :class:`geopandas.GeoDataFrame` or :class:`geopandas.GeoSeries`
-            holding the geometries to use for plotting. Its :class:`~pandas.Index` should match
-            the node labels of the partition's underlying :class:`~gerrychain.Graph`.
-        :param **kwargs: Additional arguments to pass to :meth:`geopandas.GeoDataFrame.plot`
-            to adjust the plot.
-        """
-        if set(geometries.index) != set(self.graph.nodes):
-            raise TypeError(
-                "The provided geometries do not match the nodes of the graph."
-            )
-        assignment_series = self.assignment.to_series()
-        if isinstance(geometries, geopandas.GeoDataFrame):
-            geometries = geometries.geometry
-        df = geopandas.GeoDataFrame(
-            {"assignment": assignment_series}, geometry=geometries
-        )
-        return df.plot(column="assignment", **kwargs)
-
-    @classmethod
-    def from_json(cls, graph_path, assignment, updaters=None):
-        """Creates a :class:`Partition` from a json file containing a
-        serialized NetworkX `adjacency_data` object. Files of this
-        kind for each state are available in the @gerrymandr/vtd-adjacency-graphs
-        GitHub repository.
-
-        :param graph_path: String filename for the json file
-        :param assignment: String key for the node attribute giving a district
-            assignment, or a dictionary mapping node IDs to district IDs.
-        :param updaters: (optional) Dictionary of updater functions to
-            attach to the partition, in addition to the default_updaters of `cls`.
-        """
-        graph = Graph.from_json(graph_path)
-
-        return cls(graph, assignment, updaters)
-
-    def to_json(
-        self, json_path, *, save_assignment_as=None, include_geometries_as_geojson=False
-    ):
-        """Save the partition to a JSON file in the NetworkX json_graph format.
-
-        :param json_file: Path to target JSON file.
-        :param str save_assignment_as: (optional) The string to use as a node attribute
-            key holding the current assignment. By default, does not save the
-            assignment as an attribute.
-        :param bool include_geometries_as_geojson: (optional) Whether to include any
-            :mod:`shapely` geometry objects encountered in the graph's node attributes
-            as GeoJSON. The default (``False``) behavior is to remove all geometry
-            objects because they are not serializable. Including the GeoJSON will result
-            in a much larger JSON file.
-        """
-        graph = Graph(self.graph)
-
-        if save_assignment_as is not None:
-            for node in graph.nodes:
-                graph.nodes[node][save_assignment_as] = self.assignment[node]
-
-        graph.to_json(
-            json_path, include_geometries_as_geojson=include_geometries_as_geojson
-        )
-
-    @classmethod
-    def from_file(cls, filename, assignment, updaters=None, columns=None):
-        """Create a :class:`Partition` from an ESRI Shapefile, a GeoPackage,
-        a GeoJSON file, or any other file that the `fiona` library can handle.
-        """
-        graph = Graph.from_file(filename, cols_to_add=columns)
-        return cls(graph, assignment, updaters)
-
-    @classmethod
-    def from_districtr_file(cls, graph, districtr_file, updaters=None):
-        """Create a Partition from a districting plan created with `Districtr`_,
-        a free and open-source web app created by MGGG for drawing districts.
-
-        The provided ``graph`` should be created from the same shapefile as the
-        Districtr module used to draw the districting plan. These shapefiles may
-        be found in a repository in the `mggg-states`_ GitHub organization, or by
-        request from MGGG.
-
-        .. _`Districtr`: https://mggg.org/Districtr
-        .. _`mggg-states`: https://github.com/mggg-states
-
-        :param graph: :class:`~gerrychain.Graph`
-        :param districtr_file: the path to the ``.json`` file exported from Districtr
-        :param updaters: dictionary of updaters
-        """
-        with open(districtr_file) as f:
-            districtr_plan = json.load(f)
-
-        id_column_key = districtr_plan["idColumn"]["key"]
-        districtr_assignment = districtr_plan["assignment"]
-        try:
-            node_to_id = {node: str(graph.nodes[node][id_column_key]) for node in graph}
-        except KeyError:
-            raise TypeError(
-                "The provided graph is missing the {} column, which is "
-                "needed to match the Districtr assignment to the nodes of the graph."
-            )
-
-        assignment = {node: districtr_assignment[node_to_id[node]] for node in graph}
-
-        return cls(graph, assignment, updaters)
+import json
+
+import geopandas
+
+from ..graph import Graph
+from ..updaters import compute_edge_flows, flows_from_changes
+from .assignment import get_assignment
+from .subgraphs import SubgraphView
+
+
+class Partition:
+    """
+    Partition represents a partition of the nodes of the graph. It will perform
+    the first layer of computations at each step in the Markov chain - basic
+    aggregations and calculations that we want to optimize.
+    """
+
+    default_updaters = {}
+
+    def __init__(
+        self, graph=None, assignment=None, updaters=None, parent=None, flips=None
+    ):
+        """
+        :param graph: Underlying graph; a NetworkX object.
+        :param assignment: Dictionary assigning nodes to districts. If None,
+            initialized to assign all nodes to district 0.
+        :param updaters: Dictionary of functions to track data about the partition.
+            The keys are stored as attributes on the partition class,
+            which the functions compute.
+        """
+        if parent is None:
+            self._first_time(graph, assignment, updaters)
+        else:
+            self._from_parent(parent, flips)
+
+        self._cache = dict()
+        self.subgraphs = SubgraphView(self.graph, self.parts)
+
+    def _first_time(self, graph, assignment, updaters):
+        self.graph = graph
+
+        self.assignment = get_assignment(assignment, graph)
+
+        if set(self.assignment) != set(graph):
+            raise KeyError("The graph's node labels do not match the Assignment's keys")
+
+        if updaters is None:
+            updaters = dict()
+        self.updaters = self.default_updaters.copy()
+        self.updaters.update(updaters)
+
+        self.parent = None
+        self.flips = None
+        self.flows = None
+        self.edge_flows = None
+
+    def _from_parent(self, parent, flips):
+        self.parent = parent
+        self.flips = flips
+
+        self.assignment = parent.assignment.copy()
+        self.assignment.update(flips)
+
+        self.graph = parent.graph
+        self.updaters = parent.updaters
+
+        self.flows = flows_from_changes(parent.assignment, flips)
+        self.edge_flows = compute_edge_flows(self)
+
+    def __repr__(self):
+        number_of_parts = len(self)
+        s = "s" if number_of_parts > 1 else ""
+        return "<{} [{} part{}]>".format(self.__class__.__name__, number_of_parts, s)
+
+    def __len__(self):
+        return len(self.parts)
+
+    def flip(self, flips):
+        """Returns the new partition obtained by performing the given `flips`
+        on this partition.
+
+        :param flips: dictionary assigning nodes of the graph to their new districts
+        :return: the new :class:`Partition`
+        :rtype: Partition
+        """
+        return self.__class__(parent=self, flips=flips)
+
+    def crosses_parts(self, edge):
+        """Answers the question "Does this edge cross from one part of the
+        partition to another?
+
+        :param edge: tuple of node IDs
+        :rtype: bool
+        """
+        return self.assignment[edge[0]] != self.assignment[edge[1]]
+
+    def __getitem__(self, key):
+        """Allows accessing the values of updaters computed for this
+        Partition instance.
+
+        :param key: Property to access.
+        """
+        if key not in self._cache:
+            self._cache[key] = self.updaters[key](self)
+        return self._cache[key]
+
+    def __getattr__(self, key):
+        return self[key]
+
+    @property
+    def parts(self):
+        return self.assignment.parts
+
+    def plot(self, geometries, **kwargs):
+        """Plot the partition, using the provided geometries.
+
+        :param geometries: A :class:`geopandas.GeoDataFrame` or :class:`geopandas.GeoSeries`
+            holding the geometries to use for plotting. Its :class:`~pandas.Index` should match
+            the node labels of the partition's underlying :class:`~gerrychain.Graph`.
+        :param **kwargs: Additional arguments to pass to :meth:`geopandas.GeoDataFrame.plot`
+            to adjust the plot.
+        """
+        if set(geometries.index) != set(self.graph.nodes):
+            raise TypeError(
+                "The provided geometries do not match the nodes of the graph."
+            )
+        assignment_series = self.assignment.to_series()
+        if isinstance(geometries, geopandas.GeoDataFrame):
+            geometries = geometries.geometry
+        df = geopandas.GeoDataFrame(
+            {"assignment": assignment_series}, geometry=geometries
+        )
+        return df.plot(column="assignment", **kwargs)
+
+    @classmethod
+    def from_json(cls, graph_path, assignment, updaters=None):
+        """Creates a :class:`Partition` from a json file containing a
+        serialized NetworkX `adjacency_data` object. Files of this
+        kind for each state are available in the @gerrymandr/vtd-adjacency-graphs
+        GitHub repository.
+
+        :param graph_path: String filename for the json file
+        :param assignment: String key for the node attribute giving a district
+            assignment, or a dictionary mapping node IDs to district IDs.
+        :param updaters: (optional) Dictionary of updater functions to
+            attach to the partition, in addition to the default_updaters of `cls`.
+        """
+        graph = Graph.from_json(graph_path)
+
+        return cls(graph, assignment, updaters)
+
+    def to_json(
+        self, json_path, *, save_assignment_as=None, include_geometries_as_geojson=False
+    ):
+        """Save the partition to a JSON file in the NetworkX json_graph format.
+
+        :param json_file: Path to target JSON file.
+        :param str save_assignment_as: (optional) The string to use as a node attribute
+            key holding the current assignment. By default, does not save the
+            assignment as an attribute.
+        :param bool include_geometries_as_geojson: (optional) Whether to include any
+            :mod:`shapely` geometry objects encountered in the graph's node attributes
+            as GeoJSON. The default (``False``) behavior is to remove all geometry
+            objects because they are not serializable. Including the GeoJSON will result
+            in a much larger JSON file.
+        """
+        graph = Graph(self.graph)
+
+        if save_assignment_as is not None:
+            for node in graph.nodes:
+                graph.nodes[node][save_assignment_as] = self.assignment[node]
+
+        graph.to_json(
+            json_path, include_geometries_as_geojson=include_geometries_as_geojson
+        )
+
+    @classmethod
+    def from_file(cls, filename, assignment, updaters=None, columns=None):
+        """Create a :class:`Partition` from an ESRI Shapefile, a GeoPackage,
+        a GeoJSON file, or any other file that the `fiona` library can handle.
+        """
+        graph = Graph.from_file(filename, cols_to_add=columns)
+        return cls(graph, assignment, updaters)
+
+    @classmethod
+    def from_districtr_file(cls, graph, districtr_file, updaters=None):
+        """Create a Partition from a districting plan created with `Districtr`_,
+        a free and open-source web app created by MGGG for drawing districts.
+
+        The provided ``graph`` should be created from the same shapefile as the
+        Districtr module used to draw the districting plan. These shapefiles may
+        be found in a repository in the `mggg-states`_ GitHub organization, or by
+        request from MGGG.
+
+        .. _`Districtr`: https://mggg.org/Districtr
+        .. _`mggg-states`: https://github.com/mggg-states
+
+        :param graph: :class:`~gerrychain.Graph`
+        :param districtr_file: the path to the ``.json`` file exported from Districtr
+        :param updaters: dictionary of updaters
+        """
+        with open(districtr_file) as f:
+            districtr_plan = json.load(f)
+
+        id_column_key = districtr_plan["idColumn"]["key"]
+        districtr_assignment = districtr_plan["assignment"]
+        try:
+            node_to_id = {node: str(graph.nodes[node][id_column_key]) for node in graph}
+        except KeyError:
+            raise TypeError(
+                "The provided graph is missing the {} column, which is "
+                "needed to match the Districtr assignment to the nodes of the graph."
+            )
+
+        assignment = {node: districtr_assignment[node_to_id[node]] for node in graph}
+
+        return cls(graph, assignment, updaters)
```

### Comparing `gerrychain-0.2.8/gerrychain/partition/subgraphs.py` & `gerrychain-0.2.9/gerrychain/partition/subgraphs.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-class SubgraphView:
-    def __init__(self, graph, parts):
-        self.graph = graph
-        self.parts = parts
-        self.subgraphs_cache = {}
-
-    def __getitem__(self, part):
-        if part not in self.subgraphs_cache:
-            self.subgraphs_cache[part] = self.graph.subgraph(self.parts[part])
-        return self.subgraphs_cache[part]
-
-    def __iter__(self):
-        for part in self.parts:
-            yield self[part]
-
-    def items(self):
-        for part in self.parts:
-            yield part, self[part]
+class SubgraphView:
+    def __init__(self, graph, parts):
+        self.graph = graph
+        self.parts = parts
+        self.subgraphs_cache = {}
+
+    def __getitem__(self, part):
+        if part not in self.subgraphs_cache:
+            self.subgraphs_cache[part] = self.graph.subgraph(self.parts[part])
+        return self.subgraphs_cache[part]
+
+    def __iter__(self):
+        for part in self.parts:
+            yield self[part]
+
+    def items(self):
+        for part in self.parts:
+            yield part, self[part]
```

### Comparing `gerrychain-0.2.8/gerrychain/proposals/proposals.py` & `gerrychain-0.2.9/gerrychain/proposals/proposals.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-from ..random import random
-
-
-def propose_any_node_flip(partition):
-    """Flip a random node (not necessarily on the boundary) to a random part
-    """
-
-    node = random.choice(tuple(partition.graph))
-    newpart = random.choice(tuple(partition.parts))
-
-    return partition.flip({node: newpart})
-
-
-def propose_flip_every_district(partition):
-    """Proposes a random boundary flip for each district in the partition.
-
-    :param partition: The current partition to propose a flip from.
-    :return: a proposed next `~gerrychain.Partition`
-    """
-    flips = dict()
-
-    for dist_edges in partition["cut_edges_by_part"].values():
-        edge = random.choice(tuple(dist_edges))
-
-        index = random.choice((0, 1))
-        flipped_node, other_node = edge[index], edge[1 - index]
-        flip = {flipped_node: partition.assignment[other_node]}
-
-        flips.update(flip)
-
-    return partition.flip(flips)
-
-
-def propose_chunk_flip(partition):
-    """Chooses a random boundary node and proposes to flip it and all of its neighbors
-
-    :param partition: The current partition to propose a flip from.
-    :return: a proposed next `~gerrychain.Partition`
-    """
-    flips = dict()
-
-    edge = random.choice(tuple(partition["cut_edges"]))
-    index = random.choice((0, 1))
-
-    flipped_node = edge[index]
-
-    valid_flips = [
-        nbr
-        for nbr in partition.graph.neighbors(flipped_node)
-        if partition.assignment[nbr] != partition.assignment[flipped_node]
-    ]
-
-    for flipped_neighbor in valid_flips:
-        flips.update({flipped_neighbor: partition.assignment[flipped_node]})
-
-    return partition.flip(flips)
-
-
-def propose_random_flip(partition):
-    """Proposes a random boundary flip from the partition.
-
-    :param partition: The current partition to propose a flip from.
-    :return: a proposed next `~gerrychain.Partition`
-    """
-    if len(partition["cut_edges"]) == 0:
-        return partition
-    edge = random.choice(tuple(partition["cut_edges"]))
-    index = random.choice((0, 1))
-    flipped_node, other_node = edge[index], edge[1 - index]
-    flip = {flipped_node: partition.assignment[other_node]}
-    return partition.flip(flip)
-
-
-flip = propose_random_flip
+from ..random import random
+
+
+def propose_any_node_flip(partition):
+    """Flip a random node (not necessarily on the boundary) to a random part
+    """
+
+    node = random.choice(tuple(partition.graph))
+    newpart = random.choice(tuple(partition.parts))
+
+    return partition.flip({node: newpart})
+
+
+def propose_flip_every_district(partition):
+    """Proposes a random boundary flip for each district in the partition.
+
+    :param partition: The current partition to propose a flip from.
+    :return: a proposed next `~gerrychain.Partition`
+    """
+    flips = dict()
+
+    for dist_edges in partition["cut_edges_by_part"].values():
+        edge = random.choice(tuple(dist_edges))
+
+        index = random.choice((0, 1))
+        flipped_node, other_node = edge[index], edge[1 - index]
+        flip = {flipped_node: partition.assignment[other_node]}
+
+        flips.update(flip)
+
+    return partition.flip(flips)
+
+
+def propose_chunk_flip(partition):
+    """Chooses a random boundary node and proposes to flip it and all of its neighbors
+
+    :param partition: The current partition to propose a flip from.
+    :return: a proposed next `~gerrychain.Partition`
+    """
+    flips = dict()
+
+    edge = random.choice(tuple(partition["cut_edges"]))
+    index = random.choice((0, 1))
+
+    flipped_node = edge[index]
+
+    valid_flips = [
+        nbr
+        for nbr in partition.graph.neighbors(flipped_node)
+        if partition.assignment[nbr] != partition.assignment[flipped_node]
+    ]
+
+    for flipped_neighbor in valid_flips:
+        flips.update({flipped_neighbor: partition.assignment[flipped_node]})
+
+    return partition.flip(flips)
+
+
+def propose_random_flip(partition):
+    """Proposes a random boundary flip from the partition.
+
+    :param partition: The current partition to propose a flip from.
+    :return: a proposed next `~gerrychain.Partition`
+    """
+    if len(partition["cut_edges"]) == 0:
+        return partition
+    edge = random.choice(tuple(partition["cut_edges"]))
+    index = random.choice((0, 1))
+    flipped_node, other_node = edge[index], edge[1 - index]
+    flip = {flipped_node: partition.assignment[other_node]}
+    return partition.flip(flip)
+
+
+flip = propose_random_flip
```

### Comparing `gerrychain-0.2.8/gerrychain/scores.py` & `gerrychain-0.2.9/gerrychain/metrics/partisan.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-import numpy
-
-
-def mean_median(election_results):
-    """
-    Computes the Mean-Median score for the given ElectionResults.
-    A positive value indicates an advantage for the first party listed
-    in the Election's parties_to_columns dictionary.
-    """
-    first_party = election_results.election.parties[0]
-    data = election_results.percents(first_party)
-
-    return numpy.median(data) - numpy.mean(data)
-
-
-def mean_thirdian(election_results):
-    """
-    Computes the Mean-Median score for the given ElectionResults.
-    A positive value indicates an advantage for the first party listed
-    in the Election's parties_to_columns dictionary.
-
-    The motivation for this score is that the minority party in many
-    states struggles to win even a third of the seats.
-    """
-    first_party = election_results.election.parties[0]
-    data = election_results.percents(first_party)
-
-    thirdian_index = round(len(data) / 3)
-    thirdian = sorted(data)[thirdian_index]
-
-    return thirdian - numpy.mean(data)
-
-
-def efficiency_gap(results):
-    """
-    Computes the efficiency gap for the given ElectionResults.
-    A positive value indicates an advantage for the first party listed
-    in the Election's parties_to_columns dictionary.
-    """
-    party1, party2 = [results.counts(party) for party in results.election.parties]
-    wasted_votes_by_part = map(wasted_votes, party1, party2)
-    total_votes = results.total_votes()
-    numerator = sum(waste2 - waste1 for waste1, waste2 in wasted_votes_by_part)
-    return numerator / total_votes
-
-
-def wasted_votes(party1_votes, party2_votes):
-    """
-    Computes the wasted votes for each party in the given race.
-    :party1_votes: the number of votes party1 received in the race
-    :party2_votes: the number of votes party2 received in the race
-    """
-    total_votes = party1_votes + party2_votes
-    if party1_votes > party2_votes:
-        party1_waste = party1_votes - total_votes / 2
-        party2_waste = party2_votes
-    else:
-        party2_waste = party2_votes - total_votes / 2
-        party1_waste = party1_votes
-    return party1_waste, party2_waste
-
-
-def partisan_bias(election_results):
-    """
-    Computes the partisan bias for the given ElectionResults.
-    The partisan bias is defined as the number of districts with above-mean
-    vote share by the first party divided by the total number of districts,
-    minus 1/2.
-    """
-    first_party = election_results.election.parties[0]
-    party_shares = numpy.array(election_results.percents(first_party))
-    mean_share = numpy.mean(party_shares)
-    above_mean_districts = len(party_shares[party_shares > mean_share])
-    return (above_mean_districts / len(party_shares)) - 0.5
-
-
-def partisan_gini(election_results):
-    """
-    Computes the partisan Gini score for the given ElectionResults.
-    The partisan Gini score is defined as the area between the seats-votes
-    curve and its reflection about (.5, .5).
-    """
-    # For two parties, the Gini score is symmetric--it does not vary by party.
-    party = election_results.election.parties[0]
-
-    # To find seats as a function of votes, we assume uniform partisan swing.
-    # That is, if the statewide popular vote share for a party swings by some
-    # delta, the vote share for that party swings by that delta in each
-    # district.
-    # We calculate the necessary delta to shift the district with the highest
-    # vote share for the party to a vote share of 0.5. This delta, subtracted
-    # from the original popular vote share, gives the minimum popular vote
-    # share that yields 1 seat to the party.
-    # We repeat this process for the district with the second-highest vote
-    # share, which gives the minimum popular vote share yielding 2 seats,
-    # and so on.
-    overall_result = election_results.percent(party)
-    race_results = sorted(election_results.percents(party), reverse=True)
-    seats_votes = [overall_result - r + 0.5 for r in race_results]
-
-    # Apply reflection of seats-votes curve about (.5, .5)
-    reflected_sv = reversed([1 - s for s in seats_votes])
-    # Calculate the unscaled, unsigned area between the seats-votes curve
-    # and its reflection. For each possible number of seats attained, we find
-    # the area of a rectangle of unit height, with a width determined by the
-    # horizontal distance between the curves at that number of seats.
-    unscaled_area = sum(abs(s - r) for s, r in zip(seats_votes, reflected_sv))
-    # We divide by area by the number of seats to obtain a partisan Gini score
-    # between 0 and 1.
-    return unscaled_area / len(race_results)
+import numpy
+
+
+def mean_median(election_results):
+    """
+    Computes the Mean-Median score for the given ElectionResults.
+    A positive value indicates an advantage for the first party listed
+    in the Election's parties_to_columns dictionary.
+    """
+    first_party = election_results.election.parties[0]
+    data = election_results.percents(first_party)
+
+    return numpy.median(data) - numpy.mean(data)
+
+
+def mean_thirdian(election_results):
+    """
+    Computes the Mean-Median score for the given ElectionResults.
+    A positive value indicates an advantage for the first party listed
+    in the Election's parties_to_columns dictionary.
+
+    The motivation for this score is that the minority party in many
+    states struggles to win even a third of the seats.
+    """
+    first_party = election_results.election.parties[0]
+    data = election_results.percents(first_party)
+
+    thirdian_index = round(len(data) / 3)
+    thirdian = sorted(data)[thirdian_index]
+
+    return thirdian - numpy.mean(data)
+
+
+def efficiency_gap(results):
+    """
+    Computes the efficiency gap for the given ElectionResults.
+    A positive value indicates an advantage for the first party listed
+    in the Election's parties_to_columns dictionary.
+    """
+    party1, party2 = [results.counts(party) for party in results.election.parties]
+    wasted_votes_by_part = map(wasted_votes, party1, party2)
+    total_votes = results.total_votes()
+    numerator = sum(waste2 - waste1 for waste1, waste2 in wasted_votes_by_part)
+    return numerator / total_votes
+
+
+def wasted_votes(party1_votes, party2_votes):
+    """
+    Computes the wasted votes for each party in the given race.
+    :party1_votes: the number of votes party1 received in the race
+    :party2_votes: the number of votes party2 received in the race
+    """
+    total_votes = party1_votes + party2_votes
+    if party1_votes > party2_votes:
+        party1_waste = party1_votes - total_votes / 2
+        party2_waste = party2_votes
+    else:
+        party2_waste = party2_votes - total_votes / 2
+        party1_waste = party1_votes
+    return party1_waste, party2_waste
+
+
+def partisan_bias(election_results):
+    """
+    Computes the partisan bias for the given ElectionResults.
+    The partisan bias is defined as the number of districts with above-mean
+    vote share by the first party divided by the total number of districts,
+    minus 1/2.
+    """
+    first_party = election_results.election.parties[0]
+    party_shares = numpy.array(election_results.percents(first_party))
+    mean_share = numpy.mean(party_shares)
+    above_mean_districts = len(party_shares[party_shares > mean_share])
+    return (above_mean_districts / len(party_shares)) - 0.5
+
+
+def partisan_gini(election_results):
+    """
+    Computes the partisan Gini score for the given ElectionResults.
+    The partisan Gini score is defined as the area between the seats-votes
+    curve and its reflection about (.5, .5).
+    """
+    # For two parties, the Gini score is symmetric--it does not vary by party.
+    party = election_results.election.parties[0]
+
+    # To find seats as a function of votes, we assume uniform partisan swing.
+    # That is, if the statewide popular vote share for a party swings by some
+    # delta, the vote share for that party swings by that delta in each
+    # district.
+    # We calculate the necessary delta to shift the district with the highest
+    # vote share for the party to a vote share of 0.5. This delta, subtracted
+    # from the original popular vote share, gives the minimum popular vote
+    # share that yields 1 seat to the party.
+    # We repeat this process for the district with the second-highest vote
+    # share, which gives the minimum popular vote share yielding 2 seats,
+    # and so on.
+    overall_result = election_results.percent(party)
+    race_results = sorted(election_results.percents(party), reverse=True)
+    seats_votes = [overall_result - r + 0.5 for r in race_results]
+
+    # Apply reflection of seats-votes curve about (.5, .5)
+    reflected_sv = reversed([1 - s for s in seats_votes])
+    # Calculate the unscaled, unsigned area between the seats-votes curve
+    # and its reflection. For each possible number of seats attained, we find
+    # the area of a rectangle of unit height, with a width determined by the
+    # horizontal distance between the curves at that number of seats.
+    unscaled_area = sum(abs(s - r) for s, r in zip(seats_votes, reflected_sv))
+    # We divide by area by the number of seats to obtain a partisan Gini score
+    # between 0 and 1.
+    return unscaled_area / len(race_results)
```

### Comparing `gerrychain-0.2.8/gerrychain/tree.py` & `gerrychain-0.2.9/gerrychain/tree.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,132 +1,145 @@
-import networkx as nx
-from networkx.algorithms import tree
-
-from .random import random
-
-
-def predecessors(h, root):
-    return {a: b for a, b in nx.bfs_predecessors(h, root)}
-
-
-def random_spanning_tree(graph, pop_col):
-    for edge in graph.edges:
-        graph.edges[edge]["weight"] = random.random()
-
-    edges = tree.maximum_spanning_edges(graph, algorithm="kruskal", data=False)
-    spanning_tree = nx.Graph(edges)
-    for node in graph:
-        spanning_tree.nodes[node][pop_col] = graph.nodes[node][pop_col]
-    return spanning_tree
-
-
-def bipartition_tree(
-    graph,
-    pop_col,
-    pop_target,
-    epsilon,
-    node_repeats,
-    restarts=0,
-    spanning_tree=None,
-    choice=random.choice,
-):
-    """This function finds a balanced 2 partition of a graph by drawing a
-    spanning tree and finding an edge to cut that leaves at most an epsilon
-    imbalance between the populations of the parts. If a root fails, new roots
-    are tried until node_repeats in which case a new tree is drawn.
-
-    Builds up a connected subgraph with a connected complement whose population
-    is ``epsilon * pop_target`` away from ``pop_target``.
-
-    Returns a subset of nodes of ``graph`` (whose induced subgraph is connected).
-    The other part of the partition is the complement of this subset.
-
-    :param graph: The graph to partition
-    :param pop_col: The node attribute holding the population of each node
-    :param pop_target: The target population for the returned subset of nodes
-    :param epsilon: The allowable deviation from  ``pop_target`` (as a percentage of
-        ``pop_target``) for the subgraph's population
-    :param node_repeats: A parameter for the algorithm: how many different choices
-        of root to use before drawing a new spanning tree.
-    :param restarts: Number of iterations (used when the algorithm chooses a new root)
-    :param spanning_tree: The spanning tree for the algorithm to use (used when the
-        algorithm chooses a new root and for testing)
-    :param choice: :func:`random.choice`. Can be substituted for testing.
-    """
-
-    if spanning_tree is None:
-        spanning_tree = random_spanning_tree(graph, pop_col)
-
-    h = spanning_tree.copy()
-
-    # this used to be greater than 2 but failed on small grids:(
-    root = choice([x for x in spanning_tree.nodes if spanning_tree.degree(x) > 1])
-
-    # BFS predecessors for iteratively contracting leaves
-    pred = predecessors(h, root)
-
-    # As we contract leaves, we keep track of which nodes merged together in
-    # this dictionary:
-    subsets = {x: {x} for x in graph}
-
-    while len(h) > 1:
-        leaves = [x for x in h if h.degree(x) == 1 and x != root]
-
-        for leaf in leaves:
-            if abs(h.nodes[leaf][pop_col] - pop_target) < epsilon * pop_target:
-                return subsets[leaf]
-            # Contract the leaf:
-            parent = pred[leaf]
-            h.nodes[parent][pop_col] += h.nodes[leaf][pop_col]
-            subsets[parent] |= subsets[leaf]
-            h.remove_node(leaf)
-
-    if restarts < node_repeats:
-        # Try again with new root, same tree
-        return bipartition_tree(
-            graph,
-            pop_col,
-            pop_target,
-            epsilon,
-            node_repeats,
-            restarts + 1,
-            spanning_tree,
-        )
-    else:
-        # If restarts == node_repeats, start over completely with a new tree
-        return bipartition_tree(graph, pop_col, pop_target, epsilon, node_repeats)
-
-
-def recursive_tree_part(graph, parts, pop_target, pop_col, epsilon, node_repeats=None):
-    """Uses :func:`~gerrychain.tree_methods.bipartition_tree` recursively to partition a tree into
-    ``len(parts)`` parts of population ``pop_target`` (within ``epsilon``). Can be used to
-    generate initial seed plans or to implement ReCom-like "merge walk" proposals.
-
-    :param graph: The graph
-    :param parts: Iterable of part labels (like ``[0,1,2]`` or ``range(4)``
-    :param pop_target: Target population for each part of the partition
-    :param pop_col: Node attribute key holding population data
-    :param epsilon: How far (as a percentage of ``pop_target``) from ``pop_target`` the parts
-        of the partition can be
-    :param node_repeats: Parameter for :func:`~gerrychain.tree_methods.bipartition_tree` to use.
-    :return: New assignments for the nodes of ``graph``.
-    :rtype: dict
-    """
-    flips = {}
-    remaining_nodes = set(graph.nodes)
-
-    for part in parts[:-1]:
-        nodes = bipartition_tree(
-            graph.subgraph(remaining_nodes), pop_col, pop_target, epsilon, node_repeats
-        )
-
-        for node in nodes:
-            flips[node] = part
-        # update pop_target?
-
-        remaining_nodes -= nodes
-
-    # All of the remaining nodes go in the last part
-    for node in remaining_nodes:
-        flips[node] = parts[-1]
-
-    return flips
+import networkx as nx
+from networkx.algorithms import tree
+
+from .random import random
+
+
+def predecessors(h, root):
+    return {a: b for a, b in nx.bfs_predecessors(h, root)}
+
+
+def random_spanning_tree(graph):
+    for edge in graph.edges:
+        graph.edges[edge]["weight"] = random.random()
+
+    spanning_tree = tree.maximum_spanning_tree(
+        graph, algorithm="kruskal", weight="weight"
+    )
+    return spanning_tree
+
+
+class PopulatedGraph(nx.Graph):
+    def __init__(self, graph, populations, ideal_pop, epsilon):
+        super().__init__(graph)
+        self.subsets = {node: {node} for node in self}
+        self.population = {node: populations[node] for node in self}
+        self.ideal_pop = ideal_pop
+        self.epsilon = epsilon
+
+    def contract_node(self, node, parent):
+        self.population[parent] += self.population[node]
+        self.subsets[parent] |= self.subsets[node]
+        self.remove_node(node)
+
+    def has_ideal_population(self, node):
+        return (
+            abs(self.population[node] - self.ideal_pop) < self.epsilon * self.ideal_pop
+        )
+
+
+def contract_leaves_until_balanced_or_none(h, choice=random.choice):
+    # this used to be greater than 2 but failed on small grids:(
+    root = choice([x for x in h.nodes if h.degree(x) > 1])
+    # BFS predecessors for iteratively contracting leaves
+    pred = predecessors(h, root)
+
+    # As we contract leaves, we keep track of which nodes merged together in
+    # this dictionary:
+    while len(h) > 1:
+        leaves = [x for x in h if h.degree(x) == 1 and x != root]
+
+        for leaf in leaves:
+            if h.has_ideal_population(leaf):
+                return h.subsets[leaf]
+            # Contract the leaf:
+            parent = pred[leaf]
+            h.contract_node(leaf, parent)
+    return None
+
+
+def bipartition_tree(
+    graph,
+    pop_col,
+    pop_target,
+    epsilon,
+    node_repeats,
+    spanning_tree=None,
+    choice=random.choice,
+):
+    """This function finds a balanced 2 partition of a graph by drawing a
+    spanning tree and finding an edge to cut that leaves at most an epsilon
+    imbalance between the populations of the parts. If a root fails, new roots
+    are tried until node_repeats in which case a new tree is drawn.
+
+    Builds up a connected subgraph with a connected complement whose population
+    is ``epsilon * pop_target`` away from ``pop_target``.
+
+    Returns a subset of nodes of ``graph`` (whose induced subgraph is connected).
+    The other part of the partition is the complement of this subset.
+
+    :param graph: The graph to partition
+    :param pop_col: The node attribute holding the population of each node
+    :param pop_target: The target population for the returned subset of nodes
+    :param epsilon: The allowable deviation from  ``pop_target`` (as a percentage of
+        ``pop_target``) for the subgraph's population
+    :param node_repeats: A parameter for the algorithm: how many different choices
+        of root to use before drawing a new spanning tree.
+    :param spanning_tree: The spanning tree for the algorithm to use (used when the
+        algorithm chooses a new root and for testing)
+    :param choice: :func:`random.choice`. Can be substituted for testing.
+    """
+    populations = {node: graph.nodes[node][pop_col] for node in graph}
+
+    balanced_subtree = None
+    if spanning_tree is None:
+        spanning_tree = random_spanning_tree(graph)
+    restarts = 0
+    while balanced_subtree is None:
+        if restarts == node_repeats:
+            spanning_tree = random_spanning_tree(graph)
+            restarts = 0
+        h = PopulatedGraph(spanning_tree.copy(), populations, pop_target, epsilon)
+        balanced_subtree = contract_leaves_until_balanced_or_none(h, choice=choice)
+        restarts += 1
+
+    return balanced_subtree
+
+
+def recursive_tree_part(graph, parts, pop_target, pop_col, epsilon, node_repeats=None):
+    """Uses :func:`~gerrychain.tree_methods.bipartition_tree` recursively to partition a tree into
+    ``len(parts)`` parts of population ``pop_target`` (within ``epsilon``). Can be used to
+    generate initial seed plans or to implement ReCom-like "merge walk" proposals.
+
+    :param graph: The graph
+    :param parts: Iterable of part labels (like ``[0,1,2]`` or ``range(4)``
+    :param pop_target: Target population for each part of the partition
+    :param pop_col: Node attribute key holding population data
+    :param epsilon: How far (as a percentage of ``pop_target``) from ``pop_target`` the parts
+        of the partition can be
+    :param node_repeats: Parameter for :func:`~gerrychain.tree_methods.bipartition_tree` to use.
+    :return: New assignments for the nodes of ``graph``.
+    :rtype: dict
+    """
+    flips = {}
+    remaining_nodes = set(graph.nodes)
+
+    for part in parts[:-1]:
+        nodes = bipartition_tree(
+            graph.subgraph(remaining_nodes),
+            pop_col=pop_col,
+            pop_target=pop_target,
+            epsilon=epsilon,
+            node_repeats=node_repeats,
+        )
+
+        for node in nodes:
+            flips[node] = part
+        # update pop_target?
+
+        remaining_nodes -= nodes
+
+    # All of the remaining nodes go in the last part
+    for node in remaining_nodes:
+        flips[node] = parts[-1]
+
+    return flips
```

### Comparing `gerrychain-0.2.8/gerrychain/updaters/__init__.py` & `gerrychain-0.2.9/gerrychain/updaters/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-from .compactness import (boundary_nodes, exterior_boundaries,
-                          exterior_boundaries_as_a_set, flips,
-                          interior_boundaries, perimeter, polsby_popper)
-from .county_splits import CountySplit, county_splits
-from .cut_edges import cut_edges, cut_edges_by_part
-from .election import Election
-from .flows import compute_edge_flows, flows_from_changes
-from .tally import DataTally, Tally
-
-__all__ = [
-    "flows_from_changes",
-    "polsby_popper",
-    "county_splits",
-    "cut_edges",
-    "cut_edges_by_part",
-    "Tally",
-    "DataTally",
-    "boundary_nodes",
-    "flips",
-    "perimeter",
-    "exterior_boundaries",
-    "interior_boundaries",
-    "exterior_boundaries_as_a_set",
-    "CountySplit",
-    "compute_edge_flows",
-    "Election",
-]
+from .compactness import (
+    boundary_nodes,
+    exterior_boundaries,
+    exterior_boundaries_as_a_set,
+    flips,
+    interior_boundaries,
+    perimeter,
+)
+from .county_splits import CountySplit, county_splits
+from .cut_edges import cut_edges, cut_edges_by_part
+from .election import Election
+from .flows import compute_edge_flows, flows_from_changes
+from .tally import DataTally, Tally
+
+__all__ = [
+    "flows_from_changes",
+    "county_splits",
+    "cut_edges",
+    "cut_edges_by_part",
+    "Tally",
+    "DataTally",
+    "boundary_nodes",
+    "flips",
+    "perimeter",
+    "exterior_boundaries",
+    "interior_boundaries",
+    "exterior_boundaries_as_a_set",
+    "CountySplit",
+    "compute_edge_flows",
+    "Election",
+]
```

### Comparing `gerrychain-0.2.8/gerrychain/updaters/compactness.py` & `gerrychain-0.2.9/gerrychain/updaters/compactness.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,88 +1,91 @@
-import collections
-import math
-
-from .flows import on_flow
-from .cut_edges import on_edge_flow
-
-
-def compute_polsby_popper(area, perimeter):
-    try:
-        return 4 * math.pi * area / perimeter**2
-    except ZeroDivisionError:
-        return math.nan
-
-
-def polsby_popper(partition):
-    return {part: compute_polsby_popper(partition['area'][part], partition['perimeter'][part])
-            for part in partition.parts}
-
-
-def boundary_nodes(partition, alias='boundary_nodes'):
-    if partition.parent:
-        return partition.parent[alias]
-    return {node for node in partition.graph.nodes if partition.graph.nodes[node]['boundary_node']}
-
-
-def initialize_exterior_boundaries_as_a_set(partition):
-    part_boundaries = collections.defaultdict(set)
-    for node in partition['boundary_nodes']:
-        part_boundaries[partition.assignment[node]].add(node)
-    return part_boundaries
-
-
-@on_flow(initialize_exterior_boundaries_as_a_set, alias='exterior_boundaries_as_a_set')
-def exterior_boundaries_as_a_set(partition, previous, inflow, outflow):
-    graph_boundary = partition['boundary_nodes']
-    return (previous | (inflow & graph_boundary)) - outflow
-
-
-def initialize_exterior_boundaries(partition):
-    graph_boundary = partition['boundary_nodes']
-    boundaries = collections.defaultdict(lambda: 0)
-    for node in graph_boundary:
-        part = partition.assignment[node]
-        boundaries[part] += partition.graph.nodes[node]['boundary_perim']
-    return boundaries
-
-
-@on_flow(initialize_exterior_boundaries, alias='exterior_boundaries')
-def exterior_boundaries(partition, previous, inflow, outflow):
-    graph_boundary = partition['boundary_nodes']
-    added_perimeter = sum(partition.graph.nodes[node]['boundary_perim']
-                          for node in inflow & graph_boundary)
-    removed_perimeter = sum(partition.graph.nodes[node]['boundary_perim']
-                            for node in outflow & graph_boundary)
-    return previous + added_perimeter - removed_perimeter
-
-
-def initialize_interior_boundaries(partition):
-    return {part: sum(partition.graph.edges[edge]['shared_perim']
-                      for edge in partition['cut_edges_by_part'][part])
-            for part in partition.parts}
-
-
-@on_edge_flow(initialize_interior_boundaries, alias='interior_boundaries')
-def interior_boundaries(partition, previous, new_edges, old_edges):
-    added_perimeter = sum(partition.graph.edges[edge]['shared_perim'] for edge in new_edges)
-    removed_perimeter = sum(partition.graph.edges[edge]['shared_perim'] for edge in old_edges)
-    return previous + added_perimeter - removed_perimeter
-
-
-def flips(partition):
-    return partition.flips
-
-
-def perimeter_of_part(partition, part):
-    """
-    Totals up the perimeter of the part in the partition.
-    Requires that 'boundary_perim' be a node attribute, 'shared_perim' be an edge
-    attribute, 'cut_edges' be an updater, and 'exterior_boundaries' be an updater.
-    """
-    exterior_perimeter = partition['exterior_boundaries'][part]
-    interior_perimeter = partition['interior_boundaries'][part]
-
-    return exterior_perimeter + interior_perimeter
-
-
-def perimeter(partition):
-    return {part: perimeter_of_part(partition, part) for part in partition.parts}
+import collections
+
+from .flows import on_flow
+from .cut_edges import on_edge_flow
+
+
+def boundary_nodes(partition, alias="boundary_nodes"):
+    if partition.parent:
+        return partition.parent[alias]
+    return {
+        node
+        for node in partition.graph.nodes
+        if partition.graph.nodes[node]["boundary_node"]
+    }
+
+
+def initialize_exterior_boundaries_as_a_set(partition):
+    part_boundaries = collections.defaultdict(set)
+    for node in partition["boundary_nodes"]:
+        part_boundaries[partition.assignment[node]].add(node)
+    return part_boundaries
+
+
+@on_flow(initialize_exterior_boundaries_as_a_set, alias="exterior_boundaries_as_a_set")
+def exterior_boundaries_as_a_set(partition, previous, inflow, outflow):
+    graph_boundary = partition["boundary_nodes"]
+    return (previous | (inflow & graph_boundary)) - outflow
+
+
+def initialize_exterior_boundaries(partition):
+    graph_boundary = partition["boundary_nodes"]
+    boundaries = collections.defaultdict(lambda: 0)
+    for node in graph_boundary:
+        part = partition.assignment[node]
+        boundaries[part] += partition.graph.nodes[node]["boundary_perim"]
+    return boundaries
+
+
+@on_flow(initialize_exterior_boundaries, alias="exterior_boundaries")
+def exterior_boundaries(partition, previous, inflow, outflow):
+    graph_boundary = partition["boundary_nodes"]
+    added_perimeter = sum(
+        partition.graph.nodes[node]["boundary_perim"]
+        for node in inflow & graph_boundary
+    )
+    removed_perimeter = sum(
+        partition.graph.nodes[node]["boundary_perim"]
+        for node in outflow & graph_boundary
+    )
+    return previous + added_perimeter - removed_perimeter
+
+
+def initialize_interior_boundaries(partition):
+    return {
+        part: sum(
+            partition.graph.edges[edge]["shared_perim"]
+            for edge in partition["cut_edges_by_part"][part]
+        )
+        for part in partition.parts
+    }
+
+
+@on_edge_flow(initialize_interior_boundaries, alias="interior_boundaries")
+def interior_boundaries(partition, previous, new_edges, old_edges):
+    added_perimeter = sum(
+        partition.graph.edges[edge]["shared_perim"] for edge in new_edges
+    )
+    removed_perimeter = sum(
+        partition.graph.edges[edge]["shared_perim"] for edge in old_edges
+    )
+    return previous + added_perimeter - removed_perimeter
+
+
+def flips(partition):
+    return partition.flips
+
+
+def perimeter_of_part(partition, part):
+    """
+    Totals up the perimeter of the part in the partition.
+    Requires that 'boundary_perim' be a node attribute, 'shared_perim' be an edge
+    attribute, 'cut_edges' be an updater, and 'exterior_boundaries' be an updater.
+    """
+    exterior_perimeter = partition["exterior_boundaries"][part]
+    interior_perimeter = partition["interior_boundaries"][part]
+
+    return exterior_perimeter + interior_perimeter
+
+
+def perimeter(partition):
+    return {part: perimeter_of_part(partition, part) for part in partition.parts}
```

### Comparing `gerrychain-0.2.8/gerrychain/updaters/cut_edges.py` & `gerrychain-0.2.9/gerrychain/updaters/cut_edges.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import collections
-
-from .flows import on_edge_flow
-
-
-def put_edges_into_parts(edges, assignment):
-    by_part = collections.defaultdict(set)
-    for edge in edges:
-        # add edge to the sets corresponding to the parts it touches
-        by_part[assignment[edge[0]]].add(edge)
-        by_part[assignment[edge[1]]].add(edge)
-    return by_part
-
-
-def new_cuts(partition):
-    """The edges that were not cut, but now are"""
-    return {
-        tuple(sorted((node, neighbor)))
-        for node in partition.flips
-        for neighbor in partition.graph.neighbors(node)
-        if partition.crosses_parts((node, neighbor))
-    }
-
-
-def obsolete_cuts(partition):
-    """The edges that were cut, but now are not"""
-    return {
-        tuple(sorted((node, neighbor)))
-        for node in partition.flips
-        for neighbor in partition.graph.neighbors(node)
-        if partition.parent.crosses_parts((node, neighbor))
-        and not partition.crosses_parts((node, neighbor))
-    }
-
-
-def initialize_cut_edges(partition):
-    edges = {
-        tuple(sorted(edge))
-        for edge in partition.graph.edges
-        if partition.crosses_parts(edge)
-    }
-    return put_edges_into_parts(edges, partition.assignment)
-
-
-@on_edge_flow(initialize_cut_edges, alias="cut_edges_by_part")
-def cut_edges_by_part(partition, previous, new_edges, old_edges):
-    return (previous | new_edges) - old_edges
-
-
-def cut_edges(partition):
-    parent = partition.parent
-
-    if not parent:
-        return {
-            tuple(sorted(edge))
-            for edge in partition.graph.edges
-            if partition.crosses_parts(edge)
-        }
-    # Edges that weren't cut, but now are cut
-    # We sort the tuples to make sure we don't accidentally end
-    # up with both (4,5) and (5,4) (for example) in it
-    new, obsolete = new_cuts(partition), obsolete_cuts(partition)
-
-    return (parent["cut_edges"] | new) - obsolete
+import collections
+
+from .flows import on_edge_flow
+
+
+def put_edges_into_parts(edges, assignment):
+    by_part = collections.defaultdict(set)
+    for edge in edges:
+        # add edge to the sets corresponding to the parts it touches
+        by_part[assignment[edge[0]]].add(edge)
+        by_part[assignment[edge[1]]].add(edge)
+    return by_part
+
+
+def new_cuts(partition):
+    """The edges that were not cut, but now are"""
+    return {
+        tuple(sorted((node, neighbor)))
+        for node in partition.flips
+        for neighbor in partition.graph.neighbors(node)
+        if partition.crosses_parts((node, neighbor))
+    }
+
+
+def obsolete_cuts(partition):
+    """The edges that were cut, but now are not"""
+    return {
+        tuple(sorted((node, neighbor)))
+        for node in partition.flips
+        for neighbor in partition.graph.neighbors(node)
+        if partition.parent.crosses_parts((node, neighbor))
+        and not partition.crosses_parts((node, neighbor))
+    }
+
+
+def initialize_cut_edges(partition):
+    edges = {
+        tuple(sorted(edge))
+        for edge in partition.graph.edges
+        if partition.crosses_parts(edge)
+    }
+    return put_edges_into_parts(edges, partition.assignment)
+
+
+@on_edge_flow(initialize_cut_edges, alias="cut_edges_by_part")
+def cut_edges_by_part(partition, previous, new_edges, old_edges):
+    return (previous | new_edges) - old_edges
+
+
+def cut_edges(partition):
+    parent = partition.parent
+
+    if not parent:
+        return {
+            tuple(sorted(edge))
+            for edge in partition.graph.edges
+            if partition.crosses_parts(edge)
+        }
+    # Edges that weren't cut, but now are cut
+    # We sort the tuples to make sure we don't accidentally end
+    # up with both (4,5) and (5,4) (for example) in it
+    new, obsolete = new_cuts(partition), obsolete_cuts(partition)
+
+    return (parent["cut_edges"] | new) - obsolete
```

### Comparing `gerrychain-0.2.8/gerrychain/updaters/election.py` & `gerrychain-0.2.9/gerrychain/updaters/election.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,244 +1,244 @@
-import math
-
-from gerrychain.updaters.tally import DataTally
-
-
-class Election:
-    """Represents the data of one election, with races conducted in each part of
-    the partition.
-
-    As we vary the districting plan, we can use the same node-level vote totals
-    to tabulate hypothetical elections. To do this manually with tallies, we would
-    have to maintain tallies for each party, as well as the total number of votes,
-    and then compute the electoral results and percentages from scratch every time.
-    To make this simpler, this class provides an :class:`ElectionUpdater` to manage
-    these tallies. The updater returns an :class:`ElectionResults` class giving
-    a convenient view of the election results, with methods like
-    :meth:`~ElectionResults.wins` or :meth:`~ElectionResults.percent` for common queries
-    the user might make on election results.
-
-    Example usage::
-
-        # Assuming your nodes have attributes "2008_D", "2008_R"
-        # with (for example) 2008 senate election vote totals
-        election = Election(
-            "2008 Senate",
-            {"Democratic": "2008_D", "Republican": "2008_R"},
-            alias="2008_Sen"
-        )
-
-        # Assuming you already have a graph and assignment:
-        partition = Partition(
-            graph,
-            assignment,
-            updaters={"2008_Sen": election}
-        )
-
-        # The updater returns an ElectionResults instance, which
-        # we can use (for example) to see how many seats a given
-        # party would win in this partition using this election's
-        # vote distribution:
-        partition["2008_Sen"].wins("Republican")
-
-    """
-
-    def __init__(self, name, parties_to_columns, alias=None):
-        """
-        :param name: The name of the election. (e.g. "2008 Presidential")
-        :param parties_to_columns: A dictionary matching party names to their
-            data columns, either as actual columns (list-like, indexed by nodes)
-            or as string keys for the node attributes that hold the party's
-            vote totals. Or, a list of strings which will serve as both
-            the party names and the node attribute keys.
-        :param alias: (optional) Alias that the election is registered under
-            in the Partition's dictionary of updaters.
-        """
-        self.name = name
-
-        if alias is None:
-            alias = name
-        self.alias = alias
-
-        if isinstance(parties_to_columns, dict):
-            self.parties = list(parties_to_columns.keys())
-            self.columns = list(parties_to_columns.values())
-            self.parties_to_columns = parties_to_columns
-        elif isinstance(parties_to_columns, list):
-            self.parties = parties_to_columns
-            self.columns = parties_to_columns
-            self.parties_to_columns = dict(zip(self.parties, self.columns))
-        else:
-            raise TypeError("Election expects parties_to_columns to be a dict or list")
-
-        self.tallies = {
-            party: DataTally(self.parties_to_columns[party], party)
-            for party in self.parties
-        }
-
-        self.updater = ElectionUpdater(self)
-
-    def __str__(self):
-        return "Election '{}' with vote totals for parties {} from columns {}.".format(
-            self.name, str(self.parties), str(self.columns)
-        )
-
-    def __repr__(self):
-        return "Election(parties={}, columns={}, alias={})".format(
-            str(self.parties), str(self.columns), str(self.alias)
-        )
-
-    def __call__(self, *args, **kwargs):
-        return self.updater(*args, **kwargs)
-
-
-class ElectionUpdater:
-    """
-    The updater for computing the election results in each part of the partition after
-    each step in the Markov chain. The actual results are returned to the user as
-    an :class:`ElectionResults` instance.
-    """
-
-    def __init__(self, election):
-        self.election = election
-
-    def __call__(self, partition):
-        previous_totals_for_party = self.get_previous_values(partition)
-        parties = self.election.parties
-        tallies = self.election.tallies
-
-        counts = {
-            party: tallies[party](partition, previous=previous_totals_for_party[party])
-            for party in parties
-        }
-
-        return ElectionResults(self.election, counts, races=partition.parts)
-
-    def get_previous_values(self, partition):
-        parent = partition.parent
-        if parent is None:
-            previous_totals_for_party = {party: None for party in self.election.parties}
-        else:
-            previous_totals_for_party = partition.parent[
-                self.election.alias
-            ].totals_for_party
-        return previous_totals_for_party
-
-
-def get_percents(counts, totals):
-    return {
-        part: counts[part] / totals[part] if totals[part] > 0 else math.nan
-        for part in totals
-    }
-
-
-class ElectionResults:
-    """
-    Represents the results of an election. Provides helpful methods to answer
-    common questions you might have about an election (Who won? How many seats?, etc.).
-    """
-
-    def __init__(self, election, counts, races):
-        self.election = election
-        self.totals_for_party = counts
-        self.races = races
-
-        self.totals = {
-            race: sum(counts[party][race] for party in self.election.parties)
-            for race in self.races
-        }
-
-        self.percents_for_party = {
-            party: get_percents(counts[party], self.totals)
-            for party in election.parties
-        }
-
-    def __str__(self):
-        results_by_part = "\n".join(
-            format_part_results(self.percents_for_party, part) for part in self.totals
-        )
-        return "Election Results for {name}\n{results}".format(
-            name=self.election.name, results=results_by_part
-        )
-
-    def seats(self, party):
-        """
-        Returns the number of races that ``party`` won.
-        """
-        return sum(self.won(party, race) for race in self.races)
-
-    def wins(self, party):
-        """
-        An alias for :meth:`seats`.
-        """
-        return self.seats(party)
-
-    def percent(self, party, race=None):
-        """
-        Returns the percentage of the vote that ``party`` received in a given race
-        (part of the partition). If ``race`` is omitted, returns the overall vote
-        share of ``party``.
-
-        :param party: Party ID.
-        :param race: ID of the part of the partition whose votes we want to tally.
-        """
-        if race is not None:
-            return self.percents_for_party[party][race]
-        return sum(self.votes(party)) / sum(self.totals[race] for race in self.races)
-
-    def percents(self, party):
-        """
-        :param party: The party
-        :return: The tuple of the percentage of votes that ``party`` received
-            in each part of the partition
-        """
-        return tuple(self.percents_for_party[party][race] for race in self.races)
-
-    def count(self, party, race=None):
-        """
-        Returns the total number of votes that ``party`` received in a given race
-        (part of the partition). If ``race`` is omitted, returns the overall vote
-        total of ``party``.
-
-        :param party: Party ID.
-        :param race: ID of the part of the partition whose votes we want to tally.
-        """
-        if race is not None:
-            return self.totals_for_party[party][race]
-        return sum(self.totals_for_party[party][race] for race in self.races)
-
-    def counts(self, party):
-        """
-        :param party: Party ID
-        :return: tuple of the total votes cast for ``party`` in each part of
-            the partition
-        """
-        return tuple(self.totals_for_party[party][race] for race in self.races)
-
-    def votes(self, party):
-        """
-        An alias for :meth:`counts`.
-        """
-        return self.counts(party)
-
-    def won(self, party, race):
-        """
-        Answers "Did ``party`` win the race in part ``race``?" with ``True`` or ``False``.
-        """
-        return all(
-            self.totals_for_party[party][race] >= self.totals_for_party[opponent][race]
-            for opponent in self.election.parties
-        )
-
-    def total_votes(self):
-        return sum(self.totals.values())
-
-
-def format_part_results(percents_for_party, part):
-    heading = "{part}:\n".format(part=str(part))
-    body = "\n".join(
-        "  {party}: {percent}".format(
-            party=str(party), percent=round(percents_for_party[party][part], 4)
-        )
-        for party in percents_for_party
-    )
-    return heading + body
+import math
+
+from gerrychain.updaters.tally import DataTally
+
+
+class Election:
+    """Represents the data of one election, with races conducted in each part of
+    the partition.
+
+    As we vary the districting plan, we can use the same node-level vote totals
+    to tabulate hypothetical elections. To do this manually with tallies, we would
+    have to maintain tallies for each party, as well as the total number of votes,
+    and then compute the electoral results and percentages from scratch every time.
+    To make this simpler, this class provides an :class:`ElectionUpdater` to manage
+    these tallies. The updater returns an :class:`ElectionResults` class giving
+    a convenient view of the election results, with methods like
+    :meth:`~ElectionResults.wins` or :meth:`~ElectionResults.percent` for common queries
+    the user might make on election results.
+
+    Example usage::
+
+        # Assuming your nodes have attributes "2008_D", "2008_R"
+        # with (for example) 2008 senate election vote totals
+        election = Election(
+            "2008 Senate",
+            {"Democratic": "2008_D", "Republican": "2008_R"},
+            alias="2008_Sen"
+        )
+
+        # Assuming you already have a graph and assignment:
+        partition = Partition(
+            graph,
+            assignment,
+            updaters={"2008_Sen": election}
+        )
+
+        # The updater returns an ElectionResults instance, which
+        # we can use (for example) to see how many seats a given
+        # party would win in this partition using this election's
+        # vote distribution:
+        partition["2008_Sen"].wins("Republican")
+
+    """
+
+    def __init__(self, name, parties_to_columns, alias=None):
+        """
+        :param name: The name of the election. (e.g. "2008 Presidential")
+        :param parties_to_columns: A dictionary matching party names to their
+            data columns, either as actual columns (list-like, indexed by nodes)
+            or as string keys for the node attributes that hold the party's
+            vote totals. Or, a list of strings which will serve as both
+            the party names and the node attribute keys.
+        :param alias: (optional) Alias that the election is registered under
+            in the Partition's dictionary of updaters.
+        """
+        self.name = name
+
+        if alias is None:
+            alias = name
+        self.alias = alias
+
+        if isinstance(parties_to_columns, dict):
+            self.parties = list(parties_to_columns.keys())
+            self.columns = list(parties_to_columns.values())
+            self.parties_to_columns = parties_to_columns
+        elif isinstance(parties_to_columns, list):
+            self.parties = parties_to_columns
+            self.columns = parties_to_columns
+            self.parties_to_columns = dict(zip(self.parties, self.columns))
+        else:
+            raise TypeError("Election expects parties_to_columns to be a dict or list")
+
+        self.tallies = {
+            party: DataTally(self.parties_to_columns[party], party)
+            for party in self.parties
+        }
+
+        self.updater = ElectionUpdater(self)
+
+    def __str__(self):
+        return "Election '{}' with vote totals for parties {} from columns {}.".format(
+            self.name, str(self.parties), str(self.columns)
+        )
+
+    def __repr__(self):
+        return "Election(parties={}, columns={}, alias={})".format(
+            str(self.parties), str(self.columns), str(self.alias)
+        )
+
+    def __call__(self, *args, **kwargs):
+        return self.updater(*args, **kwargs)
+
+
+class ElectionUpdater:
+    """
+    The updater for computing the election results in each part of the partition after
+    each step in the Markov chain. The actual results are returned to the user as
+    an :class:`ElectionResults` instance.
+    """
+
+    def __init__(self, election):
+        self.election = election
+
+    def __call__(self, partition):
+        previous_totals_for_party = self.get_previous_values(partition)
+        parties = self.election.parties
+        tallies = self.election.tallies
+
+        counts = {
+            party: tallies[party](partition, previous=previous_totals_for_party[party])
+            for party in parties
+        }
+
+        return ElectionResults(self.election, counts, races=partition.parts)
+
+    def get_previous_values(self, partition):
+        parent = partition.parent
+        if parent is None:
+            previous_totals_for_party = {party: None for party in self.election.parties}
+        else:
+            previous_totals_for_party = partition.parent[
+                self.election.alias
+            ].totals_for_party
+        return previous_totals_for_party
+
+
+def get_percents(counts, totals):
+    return {
+        part: counts[part] / totals[part] if totals[part] > 0 else math.nan
+        for part in totals
+    }
+
+
+class ElectionResults:
+    """
+    Represents the results of an election. Provides helpful methods to answer
+    common questions you might have about an election (Who won? How many seats?, etc.).
+    """
+
+    def __init__(self, election, counts, races):
+        self.election = election
+        self.totals_for_party = counts
+        self.races = races
+
+        self.totals = {
+            race: sum(counts[party][race] for party in self.election.parties)
+            for race in self.races
+        }
+
+        self.percents_for_party = {
+            party: get_percents(counts[party], self.totals)
+            for party in election.parties
+        }
+
+    def __str__(self):
+        results_by_part = "\n".join(
+            format_part_results(self.percents_for_party, part) for part in self.totals
+        )
+        return "Election Results for {name}\n{results}".format(
+            name=self.election.name, results=results_by_part
+        )
+
+    def seats(self, party):
+        """
+        Returns the number of races that ``party`` won.
+        """
+        return sum(self.won(party, race) for race in self.races)
+
+    def wins(self, party):
+        """
+        An alias for :meth:`seats`.
+        """
+        return self.seats(party)
+
+    def percent(self, party, race=None):
+        """
+        Returns the percentage of the vote that ``party`` received in a given race
+        (part of the partition). If ``race`` is omitted, returns the overall vote
+        share of ``party``.
+
+        :param party: Party ID.
+        :param race: ID of the part of the partition whose votes we want to tally.
+        """
+        if race is not None:
+            return self.percents_for_party[party][race]
+        return sum(self.votes(party)) / sum(self.totals[race] for race in self.races)
+
+    def percents(self, party):
+        """
+        :param party: The party
+        :return: The tuple of the percentage of votes that ``party`` received
+            in each part of the partition
+        """
+        return tuple(self.percents_for_party[party][race] for race in self.races)
+
+    def count(self, party, race=None):
+        """
+        Returns the total number of votes that ``party`` received in a given race
+        (part of the partition). If ``race`` is omitted, returns the overall vote
+        total of ``party``.
+
+        :param party: Party ID.
+        :param race: ID of the part of the partition whose votes we want to tally.
+        """
+        if race is not None:
+            return self.totals_for_party[party][race]
+        return sum(self.totals_for_party[party][race] for race in self.races)
+
+    def counts(self, party):
+        """
+        :param party: Party ID
+        :return: tuple of the total votes cast for ``party`` in each part of
+            the partition
+        """
+        return tuple(self.totals_for_party[party][race] for race in self.races)
+
+    def votes(self, party):
+        """
+        An alias for :meth:`counts`.
+        """
+        return self.counts(party)
+
+    def won(self, party, race):
+        """
+        Answers "Did ``party`` win the race in part ``race``?" with ``True`` or ``False``.
+        """
+        return all(
+            self.totals_for_party[party][race] >= self.totals_for_party[opponent][race]
+            for opponent in self.election.parties
+        )
+
+    def total_votes(self):
+        return sum(self.totals.values())
+
+
+def format_part_results(percents_for_party, part):
+    heading = "{part}:\n".format(part=str(part))
+    body = "\n".join(
+        "  {party}: {percent}".format(
+            party=str(party), percent=round(percents_for_party[party][part], 4)
+        )
+        for party in percents_for_party
+    )
+    return heading + body
```

### Comparing `gerrychain-0.2.8/gerrychain/updaters/flows.py` & `gerrychain-0.2.9/gerrychain/updaters/flows.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-import collections
-import functools
-
-
-def create_flow():
-    return {'in': set(), 'out': set()}
-
-
-def flows_from_changes(old_assignment, flips):
-    flows = collections.defaultdict(create_flow)
-    for node, target in flips.items():
-        source = old_assignment[node]
-        if source != target:
-            flows[target]['in'].add(node)
-            flows[source]['out'].add(node)
-    return flows
-
-
-def on_flow(initializer, alias):
-    """
-    Use this decorator to create an updater that responds to flows of nodes
-    between parts of the partition.
-
-    Decorate a function that takes:
-    - The partition
-    - The previous value of the updater on a fixed part P_i
-    - The new nodes that are just joining P_i at this step
-    - The old nodes that are just leaving P_i at this step
-    and returns:
-    - The new value of the updater for the fixed part P_i.
-
-    This will create an updater whose values are dictionaries of the
-    form `{part: <value of the given function on the part>}`.
-
-    The initializer, by contrast, should take the entire partition and
-    return the entire `{part: <value>}` dictionary.
-
-    Example:
-
-    .. code-block:: python
-
-        @on_flow(initializer, alias='my_updater')
-        def my_updater(partition, previous, new_nodes, old_nodes):
-            # return new value for the part
-    """
-    def decorator(function):
-        @functools.wraps(function)
-        def wrapped(partition, previous=None):
-            if partition.parent is None:
-                return initializer(partition)
-
-            if previous is None:
-                previous = partition.parent[alias]
-
-            new_values = previous.copy()
-
-            for part, flow in partition.flows.items():
-                new_values[part] = function(partition, previous[part], flow['in'], flow['out'])
-
-            return new_values
-        return wrapped
-    return decorator
-
-
-def compute_edge_flows(partition):
-    edge_flows = collections.defaultdict(create_flow)
-    assignment = partition.assignment
-    old_assignment = partition.parent.assignment
-    for node in partition.flips:
-        for neighbor in partition.graph.neighbors(node):
-            edge = tuple(sorted((node, neighbor)))
-
-            old_source = old_assignment[node]
-            old_target = old_assignment[neighbor]
-
-            new_source = assignment[node]
-            new_target = assignment[neighbor]
-
-            cut = new_source != new_target
-            was_cut = old_source != old_target
-
-            if not cut and was_cut:
-                edge_flows[old_target]['out'].add(edge)
-                edge_flows[old_source]['out'].add(edge)
-            elif cut and not was_cut:
-                edge_flows[new_target]['in'].add(edge)
-                edge_flows[new_source]['in'].add(edge)
-            elif cut and was_cut:
-                # If an edge was cut and still is cut, we need to make sure the
-                # edge is listed under the correct parts.
-                no_longer_incident_parts = {old_target, old_source} - \
-                                            {new_target, new_source}
-                for part in no_longer_incident_parts:
-                    edge_flows[part]['out'].add(edge)
-
-                newly_incident_parts = {new_target, new_source} - {old_target, old_source}
-                for part in newly_incident_parts:
-                    edge_flows[part]['in'].add(edge)
-    return edge_flows
-
-
-def on_edge_flow(initializer, alias):
-    """
-    Use this decorator to create an updater that responds to flows of cut
-    edges between parts of the partition.
-
-    Decorate a function that takes:
-    - The partition
-    - The previous value of the updater for a fixed part P_i
-    - The new cut edges that are just joining P_i at this step
-    - The old cut edges that are just leaving P_i at this step
-    and returns:
-    - The new value of the updater for the fixed part P_i.
-
-    This will create an updater whose values are dictionaries of the
-    form `{part: <value of the given function on the part>}`.
-
-    The initializer, by contrast, should take the entire partition and
-    return the entire `{part: <value>}` dictionary.
-
-    Example:
-
-    .. code-block:: python
-
-        @on_edge_flow(initializer, alias='my_updater')
-        def my_updater(partition, previous, new_edges, old_edges):
-            # return new value of the part
-    """
-    def decorator(f):
-        @functools.wraps(f)
-        def wrapper(partition):
-            if not partition.parent:
-                return initializer(partition)
-            edge_flows = partition.edge_flows
-            previous = partition.parent[alias]
-
-            new_values = previous.copy()
-            for part in partition.edge_flows:
-                new_values[part] = f(partition, previous[part],
-                                     new_edges=edge_flows[part]['in'],
-                                     old_edges=edge_flows[part]['out'])
-            return new_values
-        return wrapper
-    return decorator
+import collections
+import functools
+
+
+def create_flow():
+    return {'in': set(), 'out': set()}
+
+
+def flows_from_changes(old_assignment, flips):
+    flows = collections.defaultdict(create_flow)
+    for node, target in flips.items():
+        source = old_assignment[node]
+        if source != target:
+            flows[target]['in'].add(node)
+            flows[source]['out'].add(node)
+    return flows
+
+
+def on_flow(initializer, alias):
+    """
+    Use this decorator to create an updater that responds to flows of nodes
+    between parts of the partition.
+
+    Decorate a function that takes:
+    - The partition
+    - The previous value of the updater on a fixed part P_i
+    - The new nodes that are just joining P_i at this step
+    - The old nodes that are just leaving P_i at this step
+    and returns:
+    - The new value of the updater for the fixed part P_i.
+
+    This will create an updater whose values are dictionaries of the
+    form `{part: <value of the given function on the part>}`.
+
+    The initializer, by contrast, should take the entire partition and
+    return the entire `{part: <value>}` dictionary.
+
+    Example:
+
+    .. code-block:: python
+
+        @on_flow(initializer, alias='my_updater')
+        def my_updater(partition, previous, new_nodes, old_nodes):
+            # return new value for the part
+    """
+    def decorator(function):
+        @functools.wraps(function)
+        def wrapped(partition, previous=None):
+            if partition.parent is None:
+                return initializer(partition)
+
+            if previous is None:
+                previous = partition.parent[alias]
+
+            new_values = previous.copy()
+
+            for part, flow in partition.flows.items():
+                new_values[part] = function(partition, previous[part], flow['in'], flow['out'])
+
+            return new_values
+        return wrapped
+    return decorator
+
+
+def compute_edge_flows(partition):
+    edge_flows = collections.defaultdict(create_flow)
+    assignment = partition.assignment
+    old_assignment = partition.parent.assignment
+    for node in partition.flips:
+        for neighbor in partition.graph.neighbors(node):
+            edge = tuple(sorted((node, neighbor)))
+
+            old_source = old_assignment[node]
+            old_target = old_assignment[neighbor]
+
+            new_source = assignment[node]
+            new_target = assignment[neighbor]
+
+            cut = new_source != new_target
+            was_cut = old_source != old_target
+
+            if not cut and was_cut:
+                edge_flows[old_target]['out'].add(edge)
+                edge_flows[old_source]['out'].add(edge)
+            elif cut and not was_cut:
+                edge_flows[new_target]['in'].add(edge)
+                edge_flows[new_source]['in'].add(edge)
+            elif cut and was_cut:
+                # If an edge was cut and still is cut, we need to make sure the
+                # edge is listed under the correct parts.
+                no_longer_incident_parts = {old_target, old_source} - \
+                                            {new_target, new_source}
+                for part in no_longer_incident_parts:
+                    edge_flows[part]['out'].add(edge)
+
+                newly_incident_parts = {new_target, new_source} - {old_target, old_source}
+                for part in newly_incident_parts:
+                    edge_flows[part]['in'].add(edge)
+    return edge_flows
+
+
+def on_edge_flow(initializer, alias):
+    """
+    Use this decorator to create an updater that responds to flows of cut
+    edges between parts of the partition.
+
+    Decorate a function that takes:
+    - The partition
+    - The previous value of the updater for a fixed part P_i
+    - The new cut edges that are just joining P_i at this step
+    - The old cut edges that are just leaving P_i at this step
+    and returns:
+    - The new value of the updater for the fixed part P_i.
+
+    This will create an updater whose values are dictionaries of the
+    form `{part: <value of the given function on the part>}`.
+
+    The initializer, by contrast, should take the entire partition and
+    return the entire `{part: <value>}` dictionary.
+
+    Example:
+
+    .. code-block:: python
+
+        @on_edge_flow(initializer, alias='my_updater')
+        def my_updater(partition, previous, new_edges, old_edges):
+            # return new value of the part
+    """
+    def decorator(f):
+        @functools.wraps(f)
+        def wrapper(partition):
+            if not partition.parent:
+                return initializer(partition)
+            edge_flows = partition.edge_flows
+            previous = partition.parent[alias]
+
+            new_values = previous.copy()
+            for part in partition.edge_flows:
+                new_values[part] = f(partition, previous[part],
+                                     new_edges=edge_flows[part]['in'],
+                                     old_edges=edge_flows[part]['out'])
+            return new_values
+        return wrapper
+    return decorator
```

### Comparing `gerrychain-0.2.8/gerrychain/vendor/utm/conversion.py` & `gerrychain-0.2.9/gerrychain/vendor/utm/conversion.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,320 +1,320 @@
-from .error import OutOfRangeError
-
-# For most use cases in this module, numpy is indistinguishable
-# from math, except it also works on numpy arrays
-try:
-    import numpy as mathlib
-
-    use_numpy = True
-except ImportError:
-    import math as mathlib
-
-    use_numpy = False
-
-__all__ = ["to_latlon", "from_latlon"]
-
-K0 = 0.9996
-
-E = 0.00669438
-E2 = E * E
-E3 = E2 * E
-E_P2 = E / (1.0 - E)
-
-SQRT_E = mathlib.sqrt(1 - E)
-_E = (1 - SQRT_E) / (1 + SQRT_E)
-_E2 = _E * _E
-_E3 = _E2 * _E
-_E4 = _E3 * _E
-_E5 = _E4 * _E
-
-M1 = 1 - E / 4 - 3 * E2 / 64 - 5 * E3 / 256
-M2 = 3 * E / 8 + 3 * E2 / 32 + 45 * E3 / 1024
-M3 = 15 * E2 / 256 + 45 * E3 / 1024
-M4 = 35 * E3 / 3072
-
-P2 = 3. / 2 * _E - 27. / 32 * _E3 + 269. / 512 * _E5
-P3 = 21. / 16 * _E2 - 55. / 32 * _E4
-P4 = 151. / 96 * _E3 - 417. / 128 * _E5
-P5 = 1097. / 512 * _E4
-
-R = 6378137
-
-ZONE_LETTERS = "CDEFGHJKLMNPQRSTUVWXX"
-
-
-def in_bounds(x, lower, upper, upper_strict=False):
-    if upper_strict and use_numpy:
-        return lower <= mathlib.min(x) and mathlib.max(x) < upper
-    elif upper_strict and not use_numpy:
-        return lower <= x < upper
-    elif use_numpy:
-        return lower <= mathlib.min(x) and mathlib.max(x) <= upper
-    return lower <= x <= upper
-
-
-def check_valid_zone(zone_number, zone_letter):
-    if not 1 <= zone_number <= 60:
-        raise OutOfRangeError("zone number out of range (must be between 1 and 60)")
-
-    if zone_letter:
-        zone_letter = zone_letter.upper()
-
-        if not "C" <= zone_letter <= "X" or zone_letter in ["I", "O"]:
-            raise OutOfRangeError("zone letter out of range (must be between C and X)")
-
-
-def mixed_signs(x):
-    return use_numpy and mathlib.min(x) < 0 and mathlib.max(x) >= 0
-
-
-def negative(x):
-    if use_numpy:
-        return mathlib.max(x) < 0
-    return x < 0
-
-
-def to_latlon(
-    easting, northing, zone_number, zone_letter=None, northern=None, strict=True
-):
-    """This function convert an UTM coordinate into Latitude and Longitude
-
-        Parameters
-        ----------
-        easting: int
-            Easting value of UTM coordinate
-
-        northing: int
-            Northing value of UTM coordinate
-
-        zone number: int
-            Zone Number is represented with global map numbers of an UTM Zone
-            Numbers Map. More information see utmzones [1]_
-
-        zone_letter: str
-            Zone Letter can be represented as string values. Where UTM Zone
-            Designators can be accessed in [1]_
-
-        northern: bool
-            You can set True or False to set this parameter. Default is None
-
-
-       .. _[1]: http://www.jaworski.ca/utmzones.htm
-
-    """
-    if not zone_letter and northern is None:
-        raise ValueError("either zone_letter or northern needs to be set")
-
-    elif zone_letter and northern is not None:
-        raise ValueError("set either zone_letter or northern, but not both")
-
-    if strict:
-        if not in_bounds(easting, 100000, 1000000, upper_strict=True):
-            raise OutOfRangeError(
-                "easting out of range (must be between 100.000 m and 999.999 m)"
-            )
-        if not in_bounds(northing, 0, 10000000):
-            raise OutOfRangeError(
-                "northing out of range (must be between 0 m and 10.000.000 m)"
-            )
-
-    check_valid_zone(zone_number, zone_letter)
-
-    if zone_letter:
-        zone_letter = zone_letter.upper()
-        northern = zone_letter >= "N"
-
-    x = easting - 500000
-    y = northing
-
-    if not northern:
-        y -= 10000000
-
-    m = y / K0
-    mu = m / (R * M1)
-
-    p_rad = (
-        mu +
-        P2 * mathlib.sin(2 * mu) +
-        P3 * mathlib.sin(4 * mu) +
-        P4 * mathlib.sin(6 * mu) +
-        P5 * mathlib.sin(8 * mu)
-    )
-
-    p_sin = mathlib.sin(p_rad)
-    p_sin2 = p_sin * p_sin
-
-    p_cos = mathlib.cos(p_rad)
-
-    p_tan = p_sin / p_cos
-    p_tan2 = p_tan * p_tan
-    p_tan4 = p_tan2 * p_tan2
-
-    ep_sin = 1 - E * p_sin2
-    ep_sin_sqrt = mathlib.sqrt(1 - E * p_sin2)
-
-    n = R / ep_sin_sqrt
-    r = (1 - E) / ep_sin
-
-    c = _E * p_cos ** 2
-    c2 = c * c
-
-    d = x / (n * K0)
-    d2 = d * d
-    d3 = d2 * d
-    d4 = d3 * d
-    d5 = d4 * d
-    d6 = d5 * d
-
-    latitude = (
-        p_rad -
-        (p_tan / r) *
-        (d2 / 2 - d4 / 24 * (5 + 3 * p_tan2 + 10 * c - 4 * c2 - 9 * E_P2)) +
-        d6 / 720 * (61 + 90 * p_tan2 + 298 * c + 45 * p_tan4 - 252 * E_P2 - 3 * c2)
-    )
-
-    longitude = (
-        d -
-        d3 / 6 * (1 + 2 * p_tan2 + c) +
-        d5 / 120 * (5 - 2 * c + 28 * p_tan2 - 3 * c2 + 8 * E_P2 + 24 * p_tan4)
-    ) / p_cos
-
-    return (
-        mathlib.degrees(latitude),
-        mathlib.degrees(longitude) + zone_number_to_central_longitude(zone_number),
-    )
-
-
-def from_latlon(latitude, longitude, force_zone_number=None, force_zone_letter=None):
-    """This function convert Latitude and Longitude to UTM coordinate
-
-        Parameters
-        ----------
-        latitude: float
-            Latitude between 80 deg S and 84 deg N, e.g. (-80.0 to 84.0)
-
-        longitude: float
-            Longitude between 180 deg W and 180 deg E, e.g. (-180.0 to 180.0).
-
-        force_zone number: int
-            Zone Number is represented with global map numbers of an UTM Zone
-            Numbers Map. You may force conversion including one UTM Zone Number.
-            More information see utmzones [1]_
-
-       .. _[1]: http://www.jaworski.ca/utmzones.htm
-    """
-    if not in_bounds(latitude, -80.0, 84.0):
-        raise OutOfRangeError(
-            "latitude out of range (must be between 80 deg S and 84 deg N)"
-        )
-    if not in_bounds(longitude, -180.0, 180.0):
-        raise OutOfRangeError(
-            "longitude out of range (must be between 180 deg W and 180 deg E)"
-        )
-    if force_zone_number is not None:
-        check_valid_zone(force_zone_number, force_zone_letter)
-
-    lat_rad = mathlib.radians(latitude)
-    lat_sin = mathlib.sin(lat_rad)
-    lat_cos = mathlib.cos(lat_rad)
-
-    lat_tan = lat_sin / lat_cos
-    lat_tan2 = lat_tan * lat_tan
-    lat_tan4 = lat_tan2 * lat_tan2
-
-    if force_zone_number is None:
-        zone_number = latlon_to_zone_number(latitude, longitude)
-    else:
-        zone_number = force_zone_number
-
-    if force_zone_letter is None:
-        zone_letter = latitude_to_zone_letter(latitude)
-    else:
-        zone_letter = force_zone_letter
-
-    lon_rad = mathlib.radians(longitude)
-    central_lon = zone_number_to_central_longitude(zone_number)
-    central_lon_rad = mathlib.radians(central_lon)
-
-    n = R / mathlib.sqrt(1 - E * lat_sin ** 2)
-    c = E_P2 * lat_cos ** 2
-
-    a = lat_cos * (lon_rad - central_lon_rad)
-    a2 = a * a
-    a3 = a2 * a
-    a4 = a3 * a
-    a5 = a4 * a
-    a6 = a5 * a
-
-    m = R * (
-        M1 * lat_rad -
-        M2 * mathlib.sin(2 * lat_rad) +
-        M3 * mathlib.sin(4 * lat_rad) -
-        M4 * mathlib.sin(6 * lat_rad)
-    )
-
-    easting = (
-        K0 *
-        n *
-        (
-            a +
-            a3 / 6 * (1 - lat_tan2 + c) +
-            a5 / 120 * (5 - 18 * lat_tan2 + lat_tan4 + 72 * c - 58 * E_P2)
-        ) + 500000
-    )
-
-    northing = K0 * (
-        m +
-        n *
-        lat_tan * (
-            a2 / 2 + a4 / 24 * (5 - lat_tan2 + 9 * c + 4 * c ** 2) +
-            a6 / 720 * (61 - 58 * lat_tan2 + lat_tan4 + 600 * c - 330 * E_P2)
-        )
-    )
-
-    if mixed_signs(latitude):
-        raise ValueError("latitudes must all have the same sign")
-    elif negative(latitude):
-        northing += 10000000
-
-    return easting, northing, zone_number, zone_letter
-
-
-def latitude_to_zone_letter(latitude):
-    # If the input is a numpy array, just use the first element
-    # User responsibility to make sure that all points are in one zone
-    if use_numpy and isinstance(latitude, mathlib.ndarray):
-        latitude = latitude.flat[0]
-
-    if -80 <= latitude <= 84:
-        return ZONE_LETTERS[int(latitude + 80) >> 3]
-    else:
-        return None
-
-
-def latlon_to_zone_number(latitude, longitude):
-    # If the input is a numpy array, just use the first element
-    # User responsibility to make sure that all points are in one zone
-    if use_numpy:
-        if isinstance(latitude, mathlib.ndarray):
-            latitude = latitude.flat[0]
-        if isinstance(longitude, mathlib.ndarray):
-            longitude = longitude.flat[0]
-
-    if 56 <= latitude < 64 and 3 <= longitude < 12:
-        return 32
-
-    if 72 <= latitude <= 84 and longitude >= 0:
-        if longitude < 9:
-            return 31
-        elif longitude < 21:
-            return 33
-        elif longitude < 33:
-            return 35
-        elif longitude < 42:
-            return 37
-
-    return int((longitude + 180) / 6) + 1
-
-
-def zone_number_to_central_longitude(zone_number):
-    return (zone_number - 1) * 6 - 180 + 3
+from .error import OutOfRangeError
+
+# For most use cases in this module, numpy is indistinguishable
+# from math, except it also works on numpy arrays
+try:
+    import numpy as mathlib
+
+    use_numpy = True
+except ImportError:
+    import math as mathlib
+
+    use_numpy = False
+
+__all__ = ["to_latlon", "from_latlon"]
+
+K0 = 0.9996
+
+E = 0.00669438
+E2 = E * E
+E3 = E2 * E
+E_P2 = E / (1.0 - E)
+
+SQRT_E = mathlib.sqrt(1 - E)
+_E = (1 - SQRT_E) / (1 + SQRT_E)
+_E2 = _E * _E
+_E3 = _E2 * _E
+_E4 = _E3 * _E
+_E5 = _E4 * _E
+
+M1 = 1 - E / 4 - 3 * E2 / 64 - 5 * E3 / 256
+M2 = 3 * E / 8 + 3 * E2 / 32 + 45 * E3 / 1024
+M3 = 15 * E2 / 256 + 45 * E3 / 1024
+M4 = 35 * E3 / 3072
+
+P2 = 3. / 2 * _E - 27. / 32 * _E3 + 269. / 512 * _E5
+P3 = 21. / 16 * _E2 - 55. / 32 * _E4
+P4 = 151. / 96 * _E3 - 417. / 128 * _E5
+P5 = 1097. / 512 * _E4
+
+R = 6378137
+
+ZONE_LETTERS = "CDEFGHJKLMNPQRSTUVWXX"
+
+
+def in_bounds(x, lower, upper, upper_strict=False):
+    if upper_strict and use_numpy:
+        return lower <= mathlib.min(x) and mathlib.max(x) < upper
+    elif upper_strict and not use_numpy:
+        return lower <= x < upper
+    elif use_numpy:
+        return lower <= mathlib.min(x) and mathlib.max(x) <= upper
+    return lower <= x <= upper
+
+
+def check_valid_zone(zone_number, zone_letter):
+    if not 1 <= zone_number <= 60:
+        raise OutOfRangeError("zone number out of range (must be between 1 and 60)")
+
+    if zone_letter:
+        zone_letter = zone_letter.upper()
+
+        if not "C" <= zone_letter <= "X" or zone_letter in ["I", "O"]:
+            raise OutOfRangeError("zone letter out of range (must be between C and X)")
+
+
+def mixed_signs(x):
+    return use_numpy and mathlib.min(x) < 0 and mathlib.max(x) >= 0
+
+
+def negative(x):
+    if use_numpy:
+        return mathlib.max(x) < 0
+    return x < 0
+
+
+def to_latlon(
+    easting, northing, zone_number, zone_letter=None, northern=None, strict=True
+):
+    """This function convert an UTM coordinate into Latitude and Longitude
+
+        Parameters
+        ----------
+        easting: int
+            Easting value of UTM coordinate
+
+        northing: int
+            Northing value of UTM coordinate
+
+        zone number: int
+            Zone Number is represented with global map numbers of an UTM Zone
+            Numbers Map. More information see utmzones [1]_
+
+        zone_letter: str
+            Zone Letter can be represented as string values. Where UTM Zone
+            Designators can be accessed in [1]_
+
+        northern: bool
+            You can set True or False to set this parameter. Default is None
+
+
+       .. _[1]: http://www.jaworski.ca/utmzones.htm
+
+    """
+    if not zone_letter and northern is None:
+        raise ValueError("either zone_letter or northern needs to be set")
+
+    elif zone_letter and northern is not None:
+        raise ValueError("set either zone_letter or northern, but not both")
+
+    if strict:
+        if not in_bounds(easting, 100000, 1000000, upper_strict=True):
+            raise OutOfRangeError(
+                "easting out of range (must be between 100.000 m and 999.999 m)"
+            )
+        if not in_bounds(northing, 0, 10000000):
+            raise OutOfRangeError(
+                "northing out of range (must be between 0 m and 10.000.000 m)"
+            )
+
+    check_valid_zone(zone_number, zone_letter)
+
+    if zone_letter:
+        zone_letter = zone_letter.upper()
+        northern = zone_letter >= "N"
+
+    x = easting - 500000
+    y = northing
+
+    if not northern:
+        y -= 10000000
+
+    m = y / K0
+    mu = m / (R * M1)
+
+    p_rad = (
+        mu +
+        P2 * mathlib.sin(2 * mu) +
+        P3 * mathlib.sin(4 * mu) +
+        P4 * mathlib.sin(6 * mu) +
+        P5 * mathlib.sin(8 * mu)
+    )
+
+    p_sin = mathlib.sin(p_rad)
+    p_sin2 = p_sin * p_sin
+
+    p_cos = mathlib.cos(p_rad)
+
+    p_tan = p_sin / p_cos
+    p_tan2 = p_tan * p_tan
+    p_tan4 = p_tan2 * p_tan2
+
+    ep_sin = 1 - E * p_sin2
+    ep_sin_sqrt = mathlib.sqrt(1 - E * p_sin2)
+
+    n = R / ep_sin_sqrt
+    r = (1 - E) / ep_sin
+
+    c = _E * p_cos ** 2
+    c2 = c * c
+
+    d = x / (n * K0)
+    d2 = d * d
+    d3 = d2 * d
+    d4 = d3 * d
+    d5 = d4 * d
+    d6 = d5 * d
+
+    latitude = (
+        p_rad -
+        (p_tan / r) *
+        (d2 / 2 - d4 / 24 * (5 + 3 * p_tan2 + 10 * c - 4 * c2 - 9 * E_P2)) +
+        d6 / 720 * (61 + 90 * p_tan2 + 298 * c + 45 * p_tan4 - 252 * E_P2 - 3 * c2)
+    )
+
+    longitude = (
+        d -
+        d3 / 6 * (1 + 2 * p_tan2 + c) +
+        d5 / 120 * (5 - 2 * c + 28 * p_tan2 - 3 * c2 + 8 * E_P2 + 24 * p_tan4)
+    ) / p_cos
+
+    return (
+        mathlib.degrees(latitude),
+        mathlib.degrees(longitude) + zone_number_to_central_longitude(zone_number),
+    )
+
+
+def from_latlon(latitude, longitude, force_zone_number=None, force_zone_letter=None):
+    """This function convert Latitude and Longitude to UTM coordinate
+
+        Parameters
+        ----------
+        latitude: float
+            Latitude between 80 deg S and 84 deg N, e.g. (-80.0 to 84.0)
+
+        longitude: float
+            Longitude between 180 deg W and 180 deg E, e.g. (-180.0 to 180.0).
+
+        force_zone number: int
+            Zone Number is represented with global map numbers of an UTM Zone
+            Numbers Map. You may force conversion including one UTM Zone Number.
+            More information see utmzones [1]_
+
+       .. _[1]: http://www.jaworski.ca/utmzones.htm
+    """
+    if not in_bounds(latitude, -80.0, 84.0):
+        raise OutOfRangeError(
+            "latitude out of range (must be between 80 deg S and 84 deg N)"
+        )
+    if not in_bounds(longitude, -180.0, 180.0):
+        raise OutOfRangeError(
+            "longitude out of range (must be between 180 deg W and 180 deg E)"
+        )
+    if force_zone_number is not None:
+        check_valid_zone(force_zone_number, force_zone_letter)
+
+    lat_rad = mathlib.radians(latitude)
+    lat_sin = mathlib.sin(lat_rad)
+    lat_cos = mathlib.cos(lat_rad)
+
+    lat_tan = lat_sin / lat_cos
+    lat_tan2 = lat_tan * lat_tan
+    lat_tan4 = lat_tan2 * lat_tan2
+
+    if force_zone_number is None:
+        zone_number = latlon_to_zone_number(latitude, longitude)
+    else:
+        zone_number = force_zone_number
+
+    if force_zone_letter is None:
+        zone_letter = latitude_to_zone_letter(latitude)
+    else:
+        zone_letter = force_zone_letter
+
+    lon_rad = mathlib.radians(longitude)
+    central_lon = zone_number_to_central_longitude(zone_number)
+    central_lon_rad = mathlib.radians(central_lon)
+
+    n = R / mathlib.sqrt(1 - E * lat_sin ** 2)
+    c = E_P2 * lat_cos ** 2
+
+    a = lat_cos * (lon_rad - central_lon_rad)
+    a2 = a * a
+    a3 = a2 * a
+    a4 = a3 * a
+    a5 = a4 * a
+    a6 = a5 * a
+
+    m = R * (
+        M1 * lat_rad -
+        M2 * mathlib.sin(2 * lat_rad) +
+        M3 * mathlib.sin(4 * lat_rad) -
+        M4 * mathlib.sin(6 * lat_rad)
+    )
+
+    easting = (
+        K0 *
+        n *
+        (
+            a +
+            a3 / 6 * (1 - lat_tan2 + c) +
+            a5 / 120 * (5 - 18 * lat_tan2 + lat_tan4 + 72 * c - 58 * E_P2)
+        ) + 500000
+    )
+
+    northing = K0 * (
+        m +
+        n *
+        lat_tan * (
+            a2 / 2 + a4 / 24 * (5 - lat_tan2 + 9 * c + 4 * c ** 2) +
+            a6 / 720 * (61 - 58 * lat_tan2 + lat_tan4 + 600 * c - 330 * E_P2)
+        )
+    )
+
+    if mixed_signs(latitude):
+        raise ValueError("latitudes must all have the same sign")
+    elif negative(latitude):
+        northing += 10000000
+
+    return easting, northing, zone_number, zone_letter
+
+
+def latitude_to_zone_letter(latitude):
+    # If the input is a numpy array, just use the first element
+    # User responsibility to make sure that all points are in one zone
+    if use_numpy and isinstance(latitude, mathlib.ndarray):
+        latitude = latitude.flat[0]
+
+    if -80 <= latitude <= 84:
+        return ZONE_LETTERS[int(latitude + 80) >> 3]
+    else:
+        return None
+
+
+def latlon_to_zone_number(latitude, longitude):
+    # If the input is a numpy array, just use the first element
+    # User responsibility to make sure that all points are in one zone
+    if use_numpy:
+        if isinstance(latitude, mathlib.ndarray):
+            latitude = latitude.flat[0]
+        if isinstance(longitude, mathlib.ndarray):
+            longitude = longitude.flat[0]
+
+    if 56 <= latitude < 64 and 3 <= longitude < 12:
+        return 32
+
+    if 72 <= latitude <= 84 and longitude >= 0:
+        if longitude < 9:
+            return 31
+        elif longitude < 21:
+            return 33
+        elif longitude < 33:
+            return 35
+        elif longitude < 42:
+            return 37
+
+    return int((longitude + 180) / 6) + 1
+
+
+def zone_number_to_central_longitude(zone_number):
+    return (zone_number - 1) * 6 - 180 + 3
```

### Comparing `gerrychain-0.2.8/gerrychain.egg-info/SOURCES.txt` & `gerrychain-0.2.9/gerrychain.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-MANIFEST.in
 README.rst
 setup.cfg
 setup.py
-versioneer.py
 gerrychain/__init__.py
 gerrychain/_version.py
 gerrychain/accept.py
 gerrychain/chain.py
 gerrychain/grid.py
 gerrychain/metagraph.py
 gerrychain/random.py
-gerrychain/scores.py
 gerrychain/tree.py
 gerrychain.egg-info/PKG-INFO
 gerrychain.egg-info/SOURCES.txt
 gerrychain.egg-info/dependency_links.txt
 gerrychain.egg-info/requires.txt
 gerrychain.egg-info/top_level.txt
 gerrychain/constraints/__init__.py
@@ -22,14 +19,17 @@
 gerrychain/constraints/compactness.py
 gerrychain/constraints/contiguity.py
 gerrychain/constraints/validity.py
 gerrychain/graph/__init__.py
 gerrychain/graph/adjacency.py
 gerrychain/graph/geo.py
 gerrychain/graph/graph.py
+gerrychain/metrics/__init__.py
+gerrychain/metrics/compactness.py
+gerrychain/metrics/partisan.py
 gerrychain/partition/__init__.py
 gerrychain/partition/assignment.py
 gerrychain/partition/geographic.py
 gerrychain/partition/partition.py
 gerrychain/partition/subgraphs.py
 gerrychain/proposals/__init__.py
 gerrychain/proposals/proposals.py
```

### Comparing `gerrychain-0.2.8/setup.py` & `gerrychain-0.2.9/setup.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from setuptools import find_packages, setup
-
-import versioneer
-
-with open("./README.rst") as f:
-    long_description = f.read()
-
-requirements = [
-    # package requirements go here
-    "pandas",
-    "networkx",
-    "geopandas",
-    "shapely",
-    "matplotlib",
-]
-
-setup(
-    name="gerrychain",
-    description="Use Markov chain Monte Carlo to analyze districting plans and gerrymanders",
-    author="Metric Geometry and Gerrymandering Group",
-    author_email="gerrymandr@gmail.com",
-    maintainer="Max Hully",
-    maintainer_email="max@mggg.org",
-    long_description=long_description,
-    long_description_content_type="text/x-rst",
-    url="https://github.com/mggg/GerryChain",
-    packages=find_packages(exclude=("tests",)),
-    version=versioneer.get_version(),
-    cmdclass=versioneer.get_cmdclass(),
-    install_requires=requirements,
-    keywords="GerryChain",
-    classifiers=[
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Operating System :: OS Independent",
-        "License :: OSI Approved :: BSD License",
-    ],
-)
+from setuptools import find_packages, setup
+
+import versioneer
+
+with open("./README.rst") as f:
+    long_description = f.read()
+
+requirements = [
+    # package requirements go here
+    "pandas",
+    "networkx",
+    "geopandas",
+    "shapely",
+    "matplotlib",
+]
+
+setup(
+    name="gerrychain",
+    description="Use Markov chain Monte Carlo to analyze districting plans and gerrymanders",
+    author="Metric Geometry and Gerrymandering Group",
+    author_email="gerrymandr@gmail.com",
+    maintainer="Max Hully",
+    maintainer_email="max@mggg.org",
+    long_description=long_description,
+    long_description_content_type="text/x-rst",
+    url="https://github.com/mggg/GerryChain",
+    packages=find_packages(exclude=("tests",)),
+    version=versioneer.get_version(),
+    cmdclass=versioneer.get_cmdclass(),
+    install_requires=requirements,
+    keywords="GerryChain",
+    classifiers=[
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Operating System :: OS Independent",
+        "License :: OSI Approved :: BSD License",
+    ],
+)
```


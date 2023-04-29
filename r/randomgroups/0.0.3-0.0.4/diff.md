# Comparing `tmp/randomgroups-0.0.3.tar.gz` & `tmp/randomgroups-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randomgroups-0.0.3.tar", last modified: Wed Apr  5 08:21:16 2023, max compression
+gzip compressed data, was "randomgroups-0.0.4.tar", last modified: Sat Apr 29 09:58:12 2023, max compression
```

## Comparing `randomgroups-0.0.3.tar` & `randomgroups-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:21:16.476614 randomgroups-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:21:16.468614 randomgroups-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:21:16.472614 randomgroups-0.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-05 08:21:04.000000 randomgroups-0.0.3/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-05 08:21:04.000000 randomgroups-0.0.3/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-05 08:21:04.000000 randomgroups-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:21:16.472614 randomgroups-0.0.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-05 08:21:04.000000 randomgroups-0.0.3/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:21:16.472614 randomgroups-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-05 08:21:04.000000 randomgroups-0.0.3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-05 08:21:04.000000 randomgroups-0.0.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-05 08:21:04.000000 randomgroups-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-05 08:21:04.000000 randomgroups-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-05 08:21:04.000000 randomgroups-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-05 08:21:16.476614 randomgroups-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-05 08:21:04.000000 randomgroups-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-05 08:21:04.000000 randomgroups-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-05 08:21:16.476614 randomgroups-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-05 08:21:04.000000 randomgroups-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:21:16.472614 randomgroups-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:21:16.472614 randomgroups-0.0.3/src/randomgroups/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:21:04.000000 randomgroups-0.0.3/src/randomgroups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-05 08:21:16.000000 randomgroups-0.0.3/src/randomgroups/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-05 08:21:04.000000 randomgroups-0.0.3/src/randomgroups/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-04-05 08:21:04.000000 randomgroups-0.0.3/src/randomgroups/create_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-04-05 08:21:04.000000 randomgroups-0.0.3/src/randomgroups/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:21:16.476614 randomgroups-0.0.3/src/randomgroups.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-05 08:21:16.000000 randomgroups-0.0.3/src/randomgroups.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-05 08:21:16.000000 randomgroups-0.0.3/src/randomgroups.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 08:21:16.000000 randomgroups-0.0.3/src/randomgroups.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 08:21:16.000000 randomgroups-0.0.3/src/randomgroups.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-05 08:21:16.000000 randomgroups-0.0.3/src/randomgroups.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-05 08:21:16.000000 randomgroups-0.0.3/src/randomgroups.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:58:12.063377 randomgroups-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:58:12.059377 randomgroups-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:58:12.063377 randomgroups-0.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-29 09:58:01.000000 randomgroups-0.0.4/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-29 09:58:01.000000 randomgroups-0.0.4/.github/ISSUE_TEMPLATE/enhancement.md
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-29 09:58:01.000000 randomgroups-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:58:12.063377 randomgroups-0.0.4/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-29 09:58:01.000000 randomgroups-0.0.4/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:58:12.063377 randomgroups-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-29 09:58:01.000000 randomgroups-0.0.4/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-29 09:58:01.000000 randomgroups-0.0.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-29 09:58:01.000000 randomgroups-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-29 09:58:01.000000 randomgroups-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-29 09:58:01.000000 randomgroups-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-04-29 09:58:12.063377 randomgroups-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-29 09:58:01.000000 randomgroups-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-29 09:58:01.000000 randomgroups-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-29 09:58:12.063377 randomgroups-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-29 09:58:01.000000 randomgroups-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:58:12.059377 randomgroups-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:58:12.063377 randomgroups-0.0.4/src/randomgroups/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 09:58:01.000000 randomgroups-0.0.4/src/randomgroups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-29 09:58:12.000000 randomgroups-0.0.4/src/randomgroups/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-04-29 09:58:01.000000 randomgroups-0.0.4/src/randomgroups/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-04-29 09:58:01.000000 randomgroups-0.0.4/src/randomgroups/create_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-04-29 09:58:01.000000 randomgroups-0.0.4/src/randomgroups/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:58:12.063377 randomgroups-0.0.4/src/randomgroups.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-04-29 09:58:12.000000 randomgroups-0.0.4/src/randomgroups.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-29 09:58:12.000000 randomgroups-0.0.4/src/randomgroups.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 09:58:12.000000 randomgroups-0.0.4/src/randomgroups.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 09:58:11.000000 randomgroups-0.0.4/src/randomgroups.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-29 09:58:12.000000 randomgroups-0.0.4/src/randomgroups.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 09:58:12.000000 randomgroups-0.0.4/src/randomgroups.egg-info/top_level.txt
```

### Comparing `randomgroups-0.0.3/.github/ISSUE_TEMPLATE/bug-report.md` & `randomgroups-0.0.4/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `randomgroups-0.0.3/.github/ISSUE_TEMPLATE/enhancement.md` & `randomgroups-0.0.4/.github/ISSUE_TEMPLATE/enhancement.md`

 * *Files identical despite different names*

### Comparing `randomgroups-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md` & `randomgroups-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `randomgroups-0.0.3/.github/workflows/main.yml` & `randomgroups-0.0.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `randomgroups-0.0.3/.github/workflows/publish-to-pypi.yml` & `randomgroups-0.0.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `randomgroups-0.0.3/.gitignore` & `randomgroups-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `randomgroups-0.0.3/LICENSE` & `randomgroups-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `randomgroups-0.0.3/MANIFEST.in` & `randomgroups-0.0.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `randomgroups-0.0.3/PKG-INFO` & `randomgroups-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: randomgroups
-Version: 0.0.3
+Version: 0.0.4
 Summary: Algorithm to create recurring random groups
 Home-page: https://github.com/timmens/random-grouping
 Author: Tim Mensinger
 Author-email: mensingertim@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
@@ -22,15 +22,15 @@
 [![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![image](https://codecov.io/gh/timmens/random-grouping/branch/main/graph/badge.svg)](https://codecov.io/gh/timmens/random-grouping)
 [![image](https://results.pre-commit.ci/badge/github/timmens/random-grouping/main.svg)](https://github.com/timmens/randomg-grouping/actions?query=branch%3Amain)
 
 # Introduction
 
 This package exports a single function called `create_matching` which can be used to
-create matchings for reccuring meetings from a varying but overlapping set of members.
+create matchings for recurring meetings from a varying but overlapping set of members.
 In particular, the internal algorithm makes sure that matchings at different meetings
 are mixed.
 
 # Installation
 
 The package can be installed via pip. To do so, type the following commands in your
 favorite terminal emulator:
@@ -73,32 +73,35 @@
 named matchings for the current meeting, and second, `matchings_history.csv` which
 contains information on matchings. The latter file needs to be saved since it will be
 used in subsequent function calls. Example files are given here:
 [matching.txt](https://github.com/timmens/random-grouping/blob/main/tests/data/matching.txt),
 [matchings_history.csv](https://github.com/timmens/random-grouping/blob/main/tests/data/matchings_history.csv).
 
 *Remark:* If the files `names.csv` is a Google sheet which is updated on a regular basis
-it can be sensible not to donwload the file but to provide a link to the sheet directly.
+it can be sensible not to download the file but to provide a link to the sheet directly.
 In the case with Google sheets this is easily done by opening the Google sheet and then
 publishing the document in the file options. This creates a link to a downloadable csv
 file which updates when the Google sheet is updated. This URL can then be passed to
 `names_path`.
 
 **Subsequent Usage:**
 
 Once the file `matchings_history.csv` has been created one can further pass the path of
 this file to the function call via `matchings_history_path=...`. The previous matchings
 will then influence new group formations.
 
 **Assortative Matching:**
 
-The 'status' column in the names csv-file allows one to distuingish between 'student'
-and 'faculty'. One can then use the 'wants_mixing' column to specify whether an
-individual wants to be mixed with people from another group. This is not absolute. A
-float parameter ("faculty_multiplier") can be specified in a dictionary an passed to the
-main function via the argument "matching_params". If this parameter is very high it will
-be less likely that faculty that does not want to mix is mixed.
+The 'status' column in the names csv-file allows one to distinguish between different
+statuses like 'student' or 'faculty'. One can then use the 'wants_mixing' column to
+specify whether an individual wants to be mixed with people from another group. This is
+not absolute. A float parameter ("mixing_multiplier") can be specified. If this
+parameter is very high it will be less likely that people with a different status and
+which do not want to mix are mixed. In fact, a negative value will make it more likely
+that people with a different status are mixed. Multiple status columns can be used,
+e.g., "status", "status2", etc. and a dict of mixing multipliers can be passed to get
+different mixing multipliers for different status columns.
 
 # Contributing
 
 If you want to contribute to this repository feel free to open a pull request or submit
 an issue. You can also simply contact me, see [here](https://github.com/timmens).
```

### Comparing `randomgroups-0.0.3/README.md` & `randomgroups-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![image](https://codecov.io/gh/timmens/random-grouping/branch/main/graph/badge.svg)](https://codecov.io/gh/timmens/random-grouping)
 [![image](https://results.pre-commit.ci/badge/github/timmens/random-grouping/main.svg)](https://github.com/timmens/randomg-grouping/actions?query=branch%3Amain)
 
 # Introduction
 
 This package exports a single function called `create_matching` which can be used to
-create matchings for reccuring meetings from a varying but overlapping set of members.
+create matchings for recurring meetings from a varying but overlapping set of members.
 In particular, the internal algorithm makes sure that matchings at different meetings
 are mixed.
 
 # Installation
 
 The package can be installed via pip. To do so, type the following commands in your
 favorite terminal emulator:
@@ -55,32 +55,35 @@
 named matchings for the current meeting, and second, `matchings_history.csv` which
 contains information on matchings. The latter file needs to be saved since it will be
 used in subsequent function calls. Example files are given here:
 [matching.txt](https://github.com/timmens/random-grouping/blob/main/tests/data/matching.txt),
 [matchings_history.csv](https://github.com/timmens/random-grouping/blob/main/tests/data/matchings_history.csv).
 
 *Remark:* If the files `names.csv` is a Google sheet which is updated on a regular basis
-it can be sensible not to donwload the file but to provide a link to the sheet directly.
+it can be sensible not to download the file but to provide a link to the sheet directly.
 In the case with Google sheets this is easily done by opening the Google sheet and then
 publishing the document in the file options. This creates a link to a downloadable csv
 file which updates when the Google sheet is updated. This URL can then be passed to
 `names_path`.
 
 **Subsequent Usage:**
 
 Once the file `matchings_history.csv` has been created one can further pass the path of
 this file to the function call via `matchings_history_path=...`. The previous matchings
 will then influence new group formations.
 
 **Assortative Matching:**
 
-The 'status' column in the names csv-file allows one to distuingish between 'student'
-and 'faculty'. One can then use the 'wants_mixing' column to specify whether an
-individual wants to be mixed with people from another group. This is not absolute. A
-float parameter ("faculty_multiplier") can be specified in a dictionary an passed to the
-main function via the argument "matching_params". If this parameter is very high it will
-be less likely that faculty that does not want to mix is mixed.
+The 'status' column in the names csv-file allows one to distinguish between different
+statuses like 'student' or 'faculty'. One can then use the 'wants_mixing' column to
+specify whether an individual wants to be mixed with people from another group. This is
+not absolute. A float parameter ("mixing_multiplier") can be specified. If this
+parameter is very high it will be less likely that people with a different status and
+which do not want to mix are mixed. In fact, a negative value will make it more likely
+that people with a different status are mixed. Multiple status columns can be used,
+e.g., "status", "status2", etc. and a dict of mixing multipliers can be passed to get
+different mixing multipliers for different status columns.
 
 # Contributing
 
 If you want to contribute to this repository feel free to open a pull request or submit
 an issue. You can also simply contact me, see [here](https://github.com/timmens).
```

### Comparing `randomgroups-0.0.3/pyproject.toml` & `randomgroups-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `randomgroups-0.0.3/setup.cfg` & `randomgroups-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `randomgroups-0.0.3/src/randomgroups/algorithm.py` & `randomgroups-0.0.4/src/randomgroups/algorithm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 from itertools import combinations
-from typing import List, Union
+from typing import List, Union, Dict
 
 import numpy as np
 import pandas as pd
 
 
 def find_optimal_matching(
     candidates: List[List[pd.DataFrame]],
     matchings_history: pd.DataFrame,
     penalty_func: callable,
-    faculty_multiplier: float,
+    mixing_multiplier: Dict[str, float],
     assortative_matching: bool,
 ) -> List[pd.DataFrame]:
     """Find best matching from list of candidates.
 
     Args:
         candidates (list): List of matching candidates.
         matchings_history (pd.DataFrame): Square df containing group information. Index
             and column is given by the 'id' column in src/data/names.csv.
         penalty_func (callable): Penalty function, defaults to np.exp. Is applied to
             punish large values in matchings_history.
-        faculty_multiplier (float): Multiplier determining how much faculty members
-            want to stay in the same group.
+        mixing_multiplier (Dict[str, float]): Multiplier determining how many members
+            of different status want to stay in the same group. Positive values favor
+            assortative matchings, negative values favor mixed matchings.
+            Can only be used if assortative_matching is True.
         assortative_matching (bool): Whether to use assortative matching.
 
     Returns:
         List[pd.DataFrame]: Matching that minimizes the criterion.
 
     """
     criterion_values = []
     for matching in candidates:
         updated_history = update_matchings_history(matchings_history, matching)
         score = _compute_history_score(updated_history, penalty_func)
         if assortative_matching:
-            score += _compute_assortativity_score(matching, faculty_multiplier)
+            score += _compute_assortativity_score(matching, mixing_multiplier)
         criterion_values.append(score)
 
     optimal_matching = candidates[np.argmin(criterion_values)]
     return optimal_matching
 
 
 def _compute_history_score(
@@ -64,37 +66,43 @@
     counts = np.bincount(tril)
 
     score = np.sum(counts * penalty_func(np.arange(len(counts))))
     return score
 
 
 def _compute_assortativity_score(
-    matching: List[pd.DataFrame], faculty_multiplier: float
+    matching: List[pd.DataFrame], mixing_multiplier: Dict[str, float]
 ) -> float:
     """Compute assortativity score.
 
     Scores the matching by the fact whether the members of each group want an
     assortative or mixed group.
 
     Args:
         matching (list): Matching.
-        faculty_multiplier (float): Multiplier determining how much faculty members
-            want to stay in the same group.
+        mixing_multiplier (Dict[str, float]): Multiplier determining how many members
+            of different status want to stay in the same group. Positive values favor
+            assortative matchings, negative values favor mixed matchings.
 
     Returns:
         float: The corresponding score.
 
     """
+    # check if group has more than one status
+    statuses_columns = [col for col in matching[0].columns if "status" in col]
+
     score = 0.0
     for group in matching:
-        if len(group.status.unique()) > 1:
-            wants_assortative = 1 - group.wants_mixing
-            wants_assortative.loc[group.status == "faculty"] *= faculty_multiplier
-            score += wants_assortative.mean()
-
+        for status in statuses_columns:
+            unique_status = group[status].dropna().unique()
+            n_unique_status = len(unique_status)
+            if n_unique_status > 1:
+                wants_assortative = 1 - group.wants_mixing
+                wants_assortative *= mixing_multiplier[status] * n_unique_status
+                score += wants_assortative.mean()
     return score
 
 
 def update_matchings_history(
     matchings_history: pd.DataFrame, matching: List[pd.DataFrame]
 ) -> pd.DataFrame:
     """Update grouping matrix using matching.
```

### Comparing `randomgroups-0.0.3/src/randomgroups/create_matching.py` & `randomgroups-0.0.4/src/randomgroups/create_matching.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import numpy as np
 import pandas as pd
 from pathlib import Path
-from typing import Union, Optional
+from typing import Union, Optional, Dict
 
 from randomgroups.algorithm import draw_candidate_matchings
 from randomgroups.algorithm import find_optimal_matching
 from randomgroups.algorithm import update_matchings_history
 from randomgroups.algorithm import update_min_size_using_n_groups
 from randomgroups.algorithm import get_number_of_excluded_participants
 from randomgroups.io import format_matching_as_str
 from randomgroups.io import read_names
 from randomgroups.io import read_or_create_matchings_history
 from randomgroups.io import write_matching
 from randomgroups.io import write_matchings_history
 
 
 def create_matching(
-    names_path: Union[str, Path] = None,
-    matchings_history_path: Union[str, Path] = None,
-    output_path: Union[str, Path] = None,
+    names_path: Union[str, Path],
+    matchings_history_path: Optional[Union[str, Path]] = None,
+    output_path: Optional[Union[str, Path]] = None,
     min_size: int = 2,
     n_groups: Optional[int] = None,
     max_size: Optional[int] = None,
     penalty_func: callable = np.exp,
-    faculty_multiplier: float = 3.0,
+    mixing_multiplier: Union[float, Dict[str, float]] = 3.0,
     assortative_matching: bool = False,
     n_draws: int = 1_000,
     seed: int = 12345,
     return_results: bool = False,
     overwrite: bool = False,
 ):
     """Create matching.
@@ -40,16 +40,19 @@
         n_groups (int or None): Number of groups to create.
             If None, min_size is used to determine the number of groups.
         max_size (int or None): Setting a maximal group size can lead to participants
             being excluded (the participants with the most matchings in history file).
             If None, no maximum size is enforced.
         penalty_func (callable): Penalty function, defaults to np.exp. Is applied to
             punish large values in matchings_history.
-        faculty_multiplier (float): Multiplier determining how much faculty members
-            want to stay in the same group.
+        mixing_multiplier (float, Dict[str, float]): Multiplier determining how many
+            members of different status want to stay in the same group. Positive values
+            favor assortative matchings, negative values favor mixed matchings. Can be
+            a dict with statuses as keys and can only be used if
+            assortative_matching is True.
         assortative_matching (bool): Whether to use assortative matching.
         n_draws (int): Number of candidate groups to try during loss minimization.
         seed (int): Seed from which to start the seed generator.
         return_results (bool): Indicates whether the results should be returned.
         overwrite (bool): Whether to overwrite output files.
 
     Returns:
@@ -66,15 +69,17 @@
     if output_path is None and return_results is False:
         raise ValueError(
             "No output path is given and return_results is set to False. Please either "
             "pass a valid output path or set return_results to True."
         )
 
     names_path = Path(names_path)
-    matchings_history_path = Path(matchings_history_path)
+    matchings_history_path = (
+        None if matchings_history_path is None else Path(matchings_history_path)
+    )
     output_path = None if output_path is None else Path(output_path)
 
     test_penalties = penalty_func(np.array([1, 2]))
     if not isinstance(test_penalties, np.ndarray) or len(test_penalties) != 2:
         raise ValueError(
             "penalty_func must return a numpy array of the same length as the input "
             "array."
@@ -95,19 +100,39 @@
     all_participants = all_participants.convert_dtypes()
 
     if not all_participants.index.is_unique:
         raise ValueError("id column in names table is not unique.")
     if len(all_participants) < min_size:
         raise ValueError("There are less participants than 'min_size'.")
 
-    if "status" not in names.columns and assortative_matching:
-        raise ValueError(
-            "Assortative matching is requested but 'status' column is not present in "
-            "names table."
-        )
+    if assortative_matching:
+        # check if group has at least one or more statuses
+        statuses_columns = [col for col in names.columns if "status" in col]
+        if len(statuses_columns) == 0:
+            raise ValueError(
+                "Assortative matching is requested but 'status' column is not "
+                "present in names table."
+            )
+
+        # check if mixing_multiplier is valid
+        if isinstance(mixing_multiplier, (float, int)):
+            mixing_multiplier = {
+                status: mixing_multiplier for status in statuses_columns
+            }
+        elif set(mixing_multiplier.keys()) != set(statuses_columns):
+            raise ValueError(
+                "'mixing_multiplier' must be a float or a dict with keys "
+                "equal to the statuses."
+            )
+
+        # check if wants_mixing column is specified
+        # if not, assume that no-one wants mixing
+        # (otherwise one should set assortative_matching=False)
+        if "wants_mixing" not in all_participants.columns:
+            all_participants["wants_mixing"] = 0
 
     matchings_history = read_or_create_matchings_history(
         names=names,
         path=matchings_history_path,
     )
     matchings_history = _add_new_individuals(
         matchings_history=matchings_history,
@@ -141,15 +166,15 @@
                 n_groups=n_groups,
                 n_participants=len(all_participants) - n_to_exclude,
             )
     else:
         n_to_exclude = 0
 
     # ==================================================================================
-    # Exclude participants if neccessary
+    # Exclude participants if necessary
     # ==================================================================================
 
     participants = _exclude_participants_with_most_matchings(
         all_participants,
         matchings_history=matchings_history,
         n_to_exclude=n_to_exclude,
     )
@@ -169,15 +194,15 @@
         rng=rng,
     )
 
     optimal_matching = find_optimal_matching(
         candidates=list_of_matchings,
         matchings_history=matchings_history,
         penalty_func=penalty_func,
-        faculty_multiplier=faculty_multiplier,
+        mixing_multiplier=mixing_multiplier,
         assortative_matching=assortative_matching,
     )
 
     # ==================================================================================
     # Prepare results
     # ==================================================================================
```

### Comparing `randomgroups-0.0.3/src/randomgroups/io.py` & `randomgroups-0.0.4/src/randomgroups/io.py`

 * *Files identical despite different names*

### Comparing `randomgroups-0.0.3/src/randomgroups.egg-info/PKG-INFO` & `randomgroups-0.0.4/src/randomgroups.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: randomgroups
-Version: 0.0.3
+Version: 0.0.4
 Summary: Algorithm to create recurring random groups
 Home-page: https://github.com/timmens/random-grouping
 Author: Tim Mensinger
 Author-email: mensingertim@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
@@ -22,15 +22,15 @@
 [![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![image](https://codecov.io/gh/timmens/random-grouping/branch/main/graph/badge.svg)](https://codecov.io/gh/timmens/random-grouping)
 [![image](https://results.pre-commit.ci/badge/github/timmens/random-grouping/main.svg)](https://github.com/timmens/randomg-grouping/actions?query=branch%3Amain)
 
 # Introduction
 
 This package exports a single function called `create_matching` which can be used to
-create matchings for reccuring meetings from a varying but overlapping set of members.
+create matchings for recurring meetings from a varying but overlapping set of members.
 In particular, the internal algorithm makes sure that matchings at different meetings
 are mixed.
 
 # Installation
 
 The package can be installed via pip. To do so, type the following commands in your
 favorite terminal emulator:
@@ -73,32 +73,35 @@
 named matchings for the current meeting, and second, `matchings_history.csv` which
 contains information on matchings. The latter file needs to be saved since it will be
 used in subsequent function calls. Example files are given here:
 [matching.txt](https://github.com/timmens/random-grouping/blob/main/tests/data/matching.txt),
 [matchings_history.csv](https://github.com/timmens/random-grouping/blob/main/tests/data/matchings_history.csv).
 
 *Remark:* If the files `names.csv` is a Google sheet which is updated on a regular basis
-it can be sensible not to donwload the file but to provide a link to the sheet directly.
+it can be sensible not to download the file but to provide a link to the sheet directly.
 In the case with Google sheets this is easily done by opening the Google sheet and then
 publishing the document in the file options. This creates a link to a downloadable csv
 file which updates when the Google sheet is updated. This URL can then be passed to
 `names_path`.
 
 **Subsequent Usage:**
 
 Once the file `matchings_history.csv` has been created one can further pass the path of
 this file to the function call via `matchings_history_path=...`. The previous matchings
 will then influence new group formations.
 
 **Assortative Matching:**
 
-The 'status' column in the names csv-file allows one to distuingish between 'student'
-and 'faculty'. One can then use the 'wants_mixing' column to specify whether an
-individual wants to be mixed with people from another group. This is not absolute. A
-float parameter ("faculty_multiplier") can be specified in a dictionary an passed to the
-main function via the argument "matching_params". If this parameter is very high it will
-be less likely that faculty that does not want to mix is mixed.
+The 'status' column in the names csv-file allows one to distinguish between different
+statuses like 'student' or 'faculty'. One can then use the 'wants_mixing' column to
+specify whether an individual wants to be mixed with people from another group. This is
+not absolute. A float parameter ("mixing_multiplier") can be specified. If this
+parameter is very high it will be less likely that people with a different status and
+which do not want to mix are mixed. In fact, a negative value will make it more likely
+that people with a different status are mixed. Multiple status columns can be used,
+e.g., "status", "status2", etc. and a dict of mixing multipliers can be passed to get
+different mixing multipliers for different status columns.
 
 # Contributing
 
 If you want to contribute to this repository feel free to open a pull request or submit
 an issue. You can also simply contact me, see [here](https://github.com/timmens).
```

### Comparing `randomgroups-0.0.3/src/randomgroups.egg-info/SOURCES.txt` & `randomgroups-0.0.4/src/randomgroups.egg-info/SOURCES.txt`

 * *Files identical despite different names*


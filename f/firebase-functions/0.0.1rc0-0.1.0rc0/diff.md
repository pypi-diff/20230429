# Comparing `tmp/firebase_functions-0.0.1rc0.tar.gz` & `tmp/firebase_functions-0.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firebase_functions-0.0.1rc0.tar", last modified: Thu Apr 27 00:24:32 2023, max compression
+gzip compressed data, was "firebase_functions-0.1.0rc0.tar", last modified: Fri Apr 28 23:59:43 2023, max compression
```

## Comparing `firebase_functions-0.0.1rc0.tar` & `firebase_functions-0.1.0rc0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:24:32.686358 firebase_functions-0.0.1rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-27 00:24:32.686358 firebase_functions-0.0.1rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 00:24:32.686358 firebase_functions-0.0.1rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:24:32.674358 firebase_functions-0.0.1rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:24:32.682357 firebase_functions-0.0.1rc0/src/firebase_functions/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:24:32.682357 firebase_functions-0.0.1rc0/src/firebase_functions/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/alerts/app_distribution_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/alerts/billing_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/alerts/crashlytics_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/alerts/performance_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/alerts_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/db_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/eventarc_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/firestore_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/https_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/identity_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    37728 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:24:32.686358 firebase_functions-0.0.1rc0/src/firebase_functions/private/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/private/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/private/_alerts_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/private/_identity_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/private/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/private/path_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/private/serving.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/private/token_verifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/private/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/pubsub_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/remote_config_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/scheduler_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/storage_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/tasks_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/src/firebase_functions/test_lab_fn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:24:32.682357 firebase_functions-0.0.1rc0/src/firebase_functions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-27 00:24:32.000000 firebase_functions-0.0.1rc0/src/firebase_functions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-27 00:24:32.000000 firebase_functions-0.0.1rc0/src/firebase_functions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 00:24:32.000000 firebase_functions-0.0.1rc0/src/firebase_functions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-27 00:24:32.000000 firebase_functions-0.0.1rc0/src/firebase_functions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-27 00:24:32.000000 firebase_functions-0.0.1rc0/src/firebase_functions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:24:32.686358 firebase_functions-0.0.1rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/tests/test_eventarc_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     9827 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/tests/test_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/tests/test_path_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/tests/test_pubsub_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/tests/test_remote_config_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/tests/test_scheduler_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/tests/test_tasks_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/tests/test_test_lab_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-27 00:23:44.000000 firebase_functions-0.0.1rc0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:59:43.483568 firebase_functions-0.1.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-28 23:59:43.483568 firebase_functions-0.1.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:59:43.483568 firebase_functions-0.1.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:59:43.475568 firebase_functions-0.1.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:59:43.479568 firebase_functions-0.1.0rc0/src/firebase_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:59:43.479568 firebase_functions-0.1.0rc0/src/firebase_functions/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/alerts/app_distribution_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/alerts/billing_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/alerts/crashlytics_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/alerts/performance_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/alerts_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/db_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/eventarc_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/firestore_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/https_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/identity_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37728 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:59:43.479568 firebase_functions-0.1.0rc0/src/firebase_functions/private/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/private/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/private/_alerts_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/private/_identity_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/private/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/private/path_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/private/serving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/private/token_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/private/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/pubsub_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/remote_config_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/scheduler_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/storage_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/tasks_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/test_lab_fn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:59:43.479568 firebase_functions-0.1.0rc0/src/firebase_functions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-28 23:59:43.000000 firebase_functions-0.1.0rc0/src/firebase_functions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-28 23:59:43.000000 firebase_functions-0.1.0rc0/src/firebase_functions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:59:43.000000 firebase_functions-0.1.0rc0/src/firebase_functions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-28 23:59:43.000000 firebase_functions-0.1.0rc0/src/firebase_functions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 23:59:43.000000 firebase_functions-0.1.0rc0/src/firebase_functions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:59:43.479568 firebase_functions-0.1.0rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_eventarc_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9827 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_path_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_pubsub_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_remote_config_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_scheduler_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_tasks_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_test_lab_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_util.py
```

### Comparing `firebase_functions-0.0.1rc0/LICENSE` & `firebase_functions-0.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/PKG-INFO` & `firebase_functions-0.1.0rc0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebase_functions
-Version: 0.0.1rc0
+Version: 0.1.0rc0
 Summary: Firebase Functions Python SDK
 Home-page: https://github.com/firebase/firebase-functions-python
 Author: Firebase Team
 License: Apache License 2.0
 Keywords: firebase,functions,google,cloud
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `firebase_functions-0.0.1rc0/README.md` & `firebase_functions-0.1.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/setup.py` & `firebase_functions-0.1.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/__init__.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Firebase Functions for Python.
 """
 
-__version__ = "0.0.1rc0"
+__version__ = "0.1.0rc0"
```

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/alerts/__init__.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/alerts/app_distribution_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/alerts/app_distribution_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/alerts/billing_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/alerts/billing_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/alerts/crashlytics_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/alerts/crashlytics_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/alerts/performance_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/alerts/performance_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/alerts_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/alerts_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/core.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/core.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/db_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/db_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/eventarc_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/eventarc_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/firestore_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/firestore_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import google.events.cloud.firestore as _firestore
 import google.cloud.firestore_v1 as _firestore_v1
 import firebase_functions.private.util as _util
 import firebase_functions.private.path_pattern as _path_pattern
 import firebase_functions.core as _core
 import cloudevents.http as _ce
 
+from firebase_admin import initialize_app, get_app, _apps, _DEFAULT_APP_NAME
 from google.cloud._helpers import _datetime_to_pb_timestamp
 from google.cloud.firestore_v1 import _helpers as _firestore_helpers
 
 from google.cloud.firestore_v1 import DocumentSnapshot, DocumentReference
 from firebase_functions.options import FirestoreOptions
 from firebase_functions.core import Change
 
@@ -111,15 +112,19 @@
     event_document = event_attributes["document"]
     event_database = event_attributes["database"]
     event_time = _dt.datetime.strptime(
         event_attributes["time"],
         "%Y-%m-%dT%H:%M:%S.%f%z",
     )
 
-    firestore_client = _firestore_v1.Client(database=event_database)
+    if _DEFAULT_APP_NAME not in _apps:
+        initialize_app()
+    app = get_app()
+    firestore_client = _firestore_v1.Client(project=app.project_id,
+                                            database=event_database)
     firestore_ref: DocumentReference = firestore_client.document(event_document)
     value_snapshot: DocumentSnapshot | None = None
     old_value_snapshot: DocumentSnapshot | None = None
 
     if firestore_event_data.value:
         document_dict = _firestore_helpers.decode_dict(
             firestore_event_data.value.fields, firestore_client)
```

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/https_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/https_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/identity_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/identity_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/options.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/options.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/params.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/params.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/private/__init__.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/private/__init__.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/private/_alerts_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/private/_alerts_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/private/_identity_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/private/_identity_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/private/manifest.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/private/manifest.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/private/path_pattern.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/private/path_pattern.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/private/serving.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/private/serving.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/private/token_verifier.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/private/token_verifier.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/private/util.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/private/util.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/pubsub_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/pubsub_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/remote_config_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/remote_config_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/scheduler_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/scheduler_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/storage_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/storage_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/tasks_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/tasks_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions/test_lab_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/test_lab_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions.egg-info/PKG-INFO` & `firebase_functions-0.1.0rc0/src/firebase_functions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebase-functions
-Version: 0.0.1rc0
+Version: 0.1.0rc0
 Summary: Firebase Functions Python SDK
 Home-page: https://github.com/firebase/firebase-functions-python
 Author: Firebase Team
 License: Apache License 2.0
 Keywords: firebase,functions,google,cloud
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `firebase_functions-0.0.1rc0/src/firebase_functions.egg-info/SOURCES.txt` & `firebase_functions-0.1.0rc0/src/firebase_functions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/tests/test_eventarc_fn.py` & `firebase_functions-0.1.0rc0/tests/test_eventarc_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/tests/test_manifest.py` & `firebase_functions-0.1.0rc0/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/tests/test_options.py` & `firebase_functions-0.1.0rc0/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/tests/test_params.py` & `firebase_functions-0.1.0rc0/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/tests/test_path_pattern.py` & `firebase_functions-0.1.0rc0/tests/test_path_pattern.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/tests/test_pubsub_fn.py` & `firebase_functions-0.1.0rc0/tests/test_pubsub_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/tests/test_remote_config_fn.py` & `firebase_functions-0.1.0rc0/tests/test_remote_config_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/tests/test_scheduler_fn.py` & `firebase_functions-0.1.0rc0/tests/test_scheduler_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/tests/test_tasks_fn.py` & `firebase_functions-0.1.0rc0/tests/test_tasks_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/tests/test_test_lab_fn.py` & `firebase_functions-0.1.0rc0/tests/test_test_lab_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.0.1rc0/tests/test_util.py` & `firebase_functions-0.1.0rc0/tests/test_util.py`

 * *Files identical despite different names*


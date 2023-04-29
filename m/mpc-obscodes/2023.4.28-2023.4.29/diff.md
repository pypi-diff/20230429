# Comparing `tmp/mpc_obscodes-2023.4.28.tar.gz` & `tmp/mpc_obscodes-2023.4.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpc_obscodes-2023.4.28.tar", last modified: Fri Apr 28 01:16:48 2023, max compression
+gzip compressed data, was "mpc_obscodes-2023.4.29.tar", last modified: Sat Apr 29 02:26:52 2023, max compression
```

## Comparing `mpc_obscodes-2023.4.28.tar` & `mpc_obscodes-2023.4.29.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:16:48.204168 mpc_obscodes-2023.4.28/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 01:16:31.000000 mpc_obscodes-2023.4.28/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-28 01:16:48.204168 mpc_obscodes-2023.4.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-28 01:16:31.000000 mpc_obscodes-2023.4.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:16:48.204168 mpc_obscodes-2023.4.28/mpc_obscodes/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-28 01:16:31.000000 mpc_obscodes-2023.4.28/mpc_obscodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-28 01:16:31.000000 mpc_obscodes-2023.4.28/mpc_obscodes/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-28 01:16:31.000000 mpc_obscodes-2023.4.28/mpc_obscodes/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)   245177 2023-04-28 01:16:36.000000 mpc_obscodes-2023.4.28/mpc_obscodes/obscodes_extended.json
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 01:16:36.000000 mpc_obscodes-2023.4.28/mpc_obscodes/obscodes_extended.md5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:16:48.204168 mpc_obscodes-2023.4.28/mpc_obscodes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 01:16:31.000000 mpc_obscodes-2023.4.28/mpc_obscodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-28 01:16:31.000000 mpc_obscodes-2023.4.28/mpc_obscodes/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-28 01:16:31.000000 mpc_obscodes-2023.4.28/mpc_obscodes/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-28 01:16:31.000000 mpc_obscodes-2023.4.28/mpc_obscodes/tests/test_mpc_obscodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:16:48.204168 mpc_obscodes-2023.4.28/mpc_obscodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-28 01:16:48.000000 mpc_obscodes-2023.4.28/mpc_obscodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-28 01:16:48.000000 mpc_obscodes-2023.4.28/mpc_obscodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 01:16:48.000000 mpc_obscodes-2023.4.28/mpc_obscodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 01:16:48.000000 mpc_obscodes-2023.4.28/mpc_obscodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 01:16:48.000000 mpc_obscodes-2023.4.28/mpc_obscodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-28 01:16:36.000000 mpc_obscodes-2023.4.28/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 01:16:48.204168 mpc_obscodes-2023.4.28/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:26:52.489684 mpc_obscodes-2023.4.29/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-29 02:26:37.000000 mpc_obscodes-2023.4.29/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-29 02:26:52.489684 mpc_obscodes-2023.4.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-29 02:26:37.000000 mpc_obscodes-2023.4.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:26:52.489684 mpc_obscodes-2023.4.29/mpc_obscodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-29 02:26:37.000000 mpc_obscodes-2023.4.29/mpc_obscodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-29 02:26:37.000000 mpc_obscodes-2023.4.29/mpc_obscodes/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-29 02:26:37.000000 mpc_obscodes-2023.4.29/mpc_obscodes/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)   245280 2023-04-29 02:26:40.000000 mpc_obscodes-2023.4.29/mpc_obscodes/obscodes_extended.json
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-29 02:26:40.000000 mpc_obscodes-2023.4.29/mpc_obscodes/obscodes_extended.md5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:26:52.489684 mpc_obscodes-2023.4.29/mpc_obscodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 02:26:37.000000 mpc_obscodes-2023.4.29/mpc_obscodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-29 02:26:37.000000 mpc_obscodes-2023.4.29/mpc_obscodes/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-29 02:26:37.000000 mpc_obscodes-2023.4.29/mpc_obscodes/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-29 02:26:37.000000 mpc_obscodes-2023.4.29/mpc_obscodes/tests/test_mpc_obscodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:26:52.489684 mpc_obscodes-2023.4.29/mpc_obscodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-29 02:26:52.000000 mpc_obscodes-2023.4.29/mpc_obscodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-29 02:26:52.000000 mpc_obscodes-2023.4.29/mpc_obscodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 02:26:52.000000 mpc_obscodes-2023.4.29/mpc_obscodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 02:26:52.000000 mpc_obscodes-2023.4.29/mpc_obscodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 02:26:52.000000 mpc_obscodes-2023.4.29/mpc_obscodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-29 02:26:40.000000 mpc_obscodes-2023.4.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 02:26:52.489684 mpc_obscodes-2023.4.29/setup.cfg
```

### Comparing `mpc_obscodes-2023.4.28/PKG-INFO` & `mpc_obscodes-2023.4.29/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc_obscodes
-Version: 2023.4.28
+Version: 2023.4.29
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # Minor Planet Center Observatory Codes
@@ -15,15 +15,15 @@
 [![Build, Test, & Publish](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test_publish.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test_publish.yml)  
 
 This package ships the Minor Planet Center's [file](https://minorplanetcenter.net/Extended_Files/obscodes_extended.json.gz) of observatory codes and their geodetic coordinates.
 
 This is not an official MPC package. It is an automatically generated mirror of the file so that it is
 installable via `pip`.
 
-Every night at around 1 AM UTC, the MPC observatory code file is downloaded and compared (via md5 checksum) to the current version of this package. If the checksums are different, a new package will be published.
+Every night at around 2:15 AM UTC, the MPC observatory code file is downloaded and compared (via md5 checksum) to the current version of this package. If the checksums are different, a new package will be published.
 
 ## Installation
 
 The latest version of the file can be install via pip:  
 `pip install mpc-obscodes`
 
 ## Usage
```

### Comparing `mpc_obscodes-2023.4.28/README.md` & `mpc_obscodes-2023.4.29/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![Build, Test, & Publish](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test_publish.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test_publish.yml)  
 
 This package ships the Minor Planet Center's [file](https://minorplanetcenter.net/Extended_Files/obscodes_extended.json.gz) of observatory codes and their geodetic coordinates.
 
 This is not an official MPC package. It is an automatically generated mirror of the file so that it is
 installable via `pip`.
 
-Every night at around 1 AM UTC, the MPC observatory code file is downloaded and compared (via md5 checksum) to the current version of this package. If the checksums are different, a new package will be published.
+Every night at around 2:15 AM UTC, the MPC observatory code file is downloaded and compared (via md5 checksum) to the current version of this package. If the checksums are different, a new package will be published.
 
 ## Installation
 
 The latest version of the file can be install via pip:  
 `pip install mpc-obscodes`
 
 ## Usage
```

### Comparing `mpc_obscodes-2023.4.28/mpc_obscodes/compare.py` & `mpc_obscodes-2023.4.29/mpc_obscodes/compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.28/mpc_obscodes/fetch.py` & `mpc_obscodes-2023.4.29/mpc_obscodes/fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.28/mpc_obscodes/obscodes_extended.json` & `mpc_obscodes-2023.4.29/mpc_obscodes/obscodes_extended.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995884773662551%*

 * *Differences: {"'M53'": "OrderedDict([('Longitude', 10.28219), ('cos', 0.585977), ('sin', 0.807623), ('Name', "*

 * *          "'CAS Observatory, Preetz')])"}*

```diff
@@ -12073,14 +12073,20 @@
     },
     "M52": {
         "Longitude": 8.5785,
         "Name": "Sassari",
         "cos": 0.758941,
         "sin": 0.649052
     },
+    "M53": {
+        "Longitude": 10.28219,
+        "Name": "CAS Observatory, Preetz",
+        "cos": 0.585977,
+        "sin": 0.807623
+    },
     "M90": {
         "Longitude": 65.4286,
         "Name": "Chervishevo",
         "cos": 0.54672,
         "sin": 0.83452
     },
     "N27": {
```

### Comparing `mpc_obscodes-2023.4.28/mpc_obscodes/tests/test_compare.py` & `mpc_obscodes-2023.4.29/mpc_obscodes/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.28/mpc_obscodes/tests/test_fetch.py` & `mpc_obscodes-2023.4.29/mpc_obscodes/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.28/mpc_obscodes/tests/test_mpc_obscodes.py` & `mpc_obscodes-2023.4.29/mpc_obscodes/tests/test_mpc_obscodes.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.28/mpc_obscodes.egg-info/PKG-INFO` & `mpc_obscodes-2023.4.29/mpc_obscodes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc-obscodes
-Version: 2023.4.28
+Version: 2023.4.29
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # Minor Planet Center Observatory Codes
@@ -15,15 +15,15 @@
 [![Build, Test, & Publish](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test_publish.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/mpc_obscodes/actions/workflows/build_test_publish.yml)  
 
 This package ships the Minor Planet Center's [file](https://minorplanetcenter.net/Extended_Files/obscodes_extended.json.gz) of observatory codes and their geodetic coordinates.
 
 This is not an official MPC package. It is an automatically generated mirror of the file so that it is
 installable via `pip`.
 
-Every night at around 1 AM UTC, the MPC observatory code file is downloaded and compared (via md5 checksum) to the current version of this package. If the checksums are different, a new package will be published.
+Every night at around 2:15 AM UTC, the MPC observatory code file is downloaded and compared (via md5 checksum) to the current version of this package. If the checksums are different, a new package will be published.
 
 ## Installation
 
 The latest version of the file can be install via pip:  
 `pip install mpc-obscodes`
 
 ## Usage
```

### Comparing `mpc_obscodes-2023.4.28/pyproject.toml` & `mpc_obscodes-2023.4.29/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires =  ["setuptools>=45", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpc_obscodes"
-version = "2023.04.28"
+version = "2023.04.29"
 authors = [
     {name = "B612 Asteroid Institute", email = "info@b612foundation.org"},
 ]
 description = "Minor Planet Center Observatory Codes"
 readme = "README.md"
 requires-python = ">=3.7"
```


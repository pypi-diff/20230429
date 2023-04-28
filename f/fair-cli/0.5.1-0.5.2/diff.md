# Comparing `tmp/fair_cli-0.5.1.tar.gz` & `tmp/fair_cli-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_cli-0.5.1.tar", max compression
+gzip compressed data, was "fair_cli-0.5.2.tar", max compression
```

## Comparing `fair_cli-0.5.1.tar` & `fair_cli-0.5.2.tar`

### file list

```diff
@@ -1,38 +1,37 @@
--rw-r--r--   0        0        0     1888 2023-02-09 14:07:59.333304 fair_cli-0.5.1/CHANGELOG.md
--rw-r--r--   0        0        0     1397 2023-02-09 14:07:59.333304 fair_cli-0.5.1/CITATION.cff
--rw-r--r--   0        0        0     2027 2023-02-09 11:58:00.275447 fair_cli-0.5.1/fair/__init__.py
--rw-r--r--   0        0        0    20683 2023-02-09 14:07:59.343297 fair_cli-0.5.1/fair/cli.py
--rw-r--r--   0        0        0     9462 2023-02-09 14:07:59.344297 fair_cli-0.5.1/fair/common.py
--rw-r--r--   0        0        0    28995 2023-02-09 14:07:59.346295 fair_cli-0.5.1/fair/configuration/__init__.py
--rw-r--r--   0        0        0     3443 2023-02-09 14:07:59.347295 fair_cli-0.5.1/fair/configuration/validation.py
--rw-r--r--   0        0        0     5555 2023-02-09 14:07:59.348293 fair_cli-0.5.1/fair/exceptions.py
--rw-r--r--   0        0        0    10127 2023-02-09 14:07:59.349293 fair_cli-0.5.1/fair/files.txt
--rw-r--r--   0        0        0     4785 2023-02-09 14:07:59.349293 fair_cli-0.5.1/fair/history.py
--rw-r--r--   0        0        0     4139 2023-02-09 14:07:59.350292 fair_cli-0.5.1/fair/identifiers.py
--rw-r--r--   0        0        0     2383 2023-02-09 14:07:59.351291 fair_cli-0.5.1/fair/logging.py
--rw-r--r--   0        0        0     8423 2023-02-09 14:07:59.352290 fair_cli-0.5.1/fair/register.py
--rw-r--r--   0        0        0      168 2023-02-09 14:07:59.352290 fair_cli-0.5.1/fair/registry/__init__.py
--rw-r--r--   0        0        0     1285 2023-02-09 11:58:00.286440 fair_cli-0.5.1/fair/registry/file_formats.json
--rw-r--r--   0        0        0      126 2023-02-09 11:58:00.287439 fair_cli-0.5.1/fair/registry/file_types.py
--rw-r--r--   0        0        0    15642 2023-02-09 14:07:59.353290 fair_cli-0.5.1/fair/registry/requests.py
--rw-r--r--   0        0        0    15251 2023-02-09 14:08:03.921654 fair_cli-0.5.1/fair/registry/server.py
--rw-r--r--   0        0        0    23360 2023-02-09 14:07:59.355290 fair_cli-0.5.1/fair/registry/storage.py
--rw-r--r--   0        0        0    15401 2023-02-09 14:07:59.357288 fair_cli-0.5.1/fair/registry/sync.py
--rw-r--r--   0        0        0     4936 2023-02-09 14:07:59.357288 fair_cli-0.5.1/fair/registry/versioning.py
--rw-r--r--   0        0        0     2396 2023-02-09 14:07:59.358287 fair_cli-0.5.1/fair/run.py
--rw-r--r--   0        0        0    41645 2023-02-09 14:07:59.360286 fair_cli-0.5.1/fair/session.py
--rw-r--r--   0        0        0    15660 2023-02-09 14:07:59.361299 fair_cli-0.5.1/fair/staging.py
--rw-r--r--   0        0        0      515 2023-02-09 11:58:00.294435 fair_cli-0.5.1/fair/templates/__init__.py
--rw-r--r--   0        0        0      301 2023-02-09 11:58:00.295432 fair_cli-0.5.1/fair/templates/config.jinja
--rw-r--r--   0        0        0      139 2023-02-09 11:58:00.296432 fair_cli-0.5.1/fair/templates/hist.jinja
--rw-r--r--   0        0        0     3284 2023-02-09 14:07:59.362285 fair_cli-0.5.1/fair/testing.py
--rw-r--r--   0        0        0    55154 2023-02-09 14:07:59.364293 fair_cli-0.5.1/fair/user_config/__init__.py
--rw-r--r--   0        0        0     5023 2023-02-09 14:07:59.365283 fair_cli-0.5.1/fair/user_config/globbing.py
--rw-r--r--   0        0        0     9510 2023-02-09 14:07:59.365283 fair_cli-0.5.1/fair/user_config/validation.py
--rw-r--r--   0        0        0     5168 2023-02-09 14:07:59.366283 fair_cli-0.5.1/fair/utilities.py
--rw-r--r--   0        0        0     1511 2023-02-09 14:07:59.367282 fair_cli-0.5.1/fair/virtualenv.py
--rw-r--r--   0        0        0     1339 2023-02-09 11:58:00.264453 fair_cli-0.5.1/LICENSE
--rw-r--r--   0        0        0     2463 2023-02-09 14:08:03.923652 fair_cli-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    11631 2023-02-09 14:07:59.334303 fair_cli-0.5.1/README.md
--rw-r--r--   0        0        0    12890 1970-01-01 00:00:00.000000 fair_cli-0.5.1/setup.py
--rw-r--r--   0        0        0    13363 1970-01-01 00:00:00.000000 fair_cli-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1888 2023-04-27 13:19:09.272183 fair_cli-0.5.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1397 2023-04-27 13:19:09.272183 fair_cli-0.5.2/CITATION.cff
+-rw-r--r--   0        0        0     2027 2023-04-27 10:42:03.123818 fair_cli-0.5.2/fair/__init__.py
+-rw-r--r--   0        0        0    20683 2023-04-28 23:41:25.182481 fair_cli-0.5.2/fair/cli.py
+-rw-r--r--   0        0        0     9462 2023-04-27 13:19:09.276183 fair_cli-0.5.2/fair/common.py
+-rw-r--r--   0        0        0    28995 2023-04-28 23:41:25.182481 fair_cli-0.5.2/fair/configuration/__init__.py
+-rw-r--r--   0        0        0     3443 2023-04-27 13:19:09.277182 fair_cli-0.5.2/fair/configuration/validation.py
+-rw-r--r--   0        0        0     5555 2023-04-27 13:19:09.277182 fair_cli-0.5.2/fair/exceptions.py
+-rw-r--r--   0        0        0    10127 2023-04-27 13:19:09.278183 fair_cli-0.5.2/fair/files.txt
+-rw-r--r--   0        0        0     4785 2023-04-27 13:19:09.278183 fair_cli-0.5.2/fair/history.py
+-rw-r--r--   0        0        0     4139 2023-04-28 23:41:30.085525 fair_cli-0.5.2/fair/identifiers.py
+-rw-r--r--   0        0        0     2383 2023-04-27 13:19:09.279183 fair_cli-0.5.2/fair/logging.py
+-rw-r--r--   0        0        0     8423 2023-04-27 13:19:09.279183 fair_cli-0.5.2/fair/register.py
+-rw-r--r--   0        0        0      168 2023-04-27 13:19:09.280182 fair_cli-0.5.2/fair/registry/__init__.py
+-rw-r--r--   0        0        0     1285 2023-04-27 10:42:03.127817 fair_cli-0.5.2/fair/registry/file_formats.json
+-rw-r--r--   0        0        0      126 2023-04-27 10:42:03.127817 fair_cli-0.5.2/fair/registry/file_types.py
+-rw-r--r--   0        0        0    15642 2023-04-28 23:41:25.183481 fair_cli-0.5.2/fair/registry/requests.py
+-rw-r--r--   0        0        0    15251 2023-04-28 23:41:25.183481 fair_cli-0.5.2/fair/registry/server.py
+-rw-r--r--   0        0        0    23360 2023-04-28 23:41:25.184481 fair_cli-0.5.2/fair/registry/storage.py
+-rw-r--r--   0        0        0    15401 2023-04-28 23:41:25.184481 fair_cli-0.5.2/fair/registry/sync.py
+-rw-r--r--   0        0        0     4936 2023-04-27 13:19:09.281183 fair_cli-0.5.2/fair/registry/versioning.py
+-rw-r--r--   0        0        0     2396 2023-04-27 13:19:09.282183 fair_cli-0.5.2/fair/run.py
+-rw-r--r--   0        0        0    41645 2023-04-28 23:41:25.185481 fair_cli-0.5.2/fair/session.py
+-rw-r--r--   0        0        0    15660 2023-04-28 23:41:25.185481 fair_cli-0.5.2/fair/staging.py
+-rw-r--r--   0        0        0      515 2023-04-27 10:42:03.130817 fair_cli-0.5.2/fair/templates/__init__.py
+-rw-r--r--   0        0        0      301 2023-04-27 10:42:03.131817 fair_cli-0.5.2/fair/templates/config.jinja
+-rw-r--r--   0        0        0      139 2023-04-27 10:42:03.131817 fair_cli-0.5.2/fair/templates/hist.jinja
+-rw-r--r--   0        0        0     3284 2023-04-27 13:19:09.283182 fair_cli-0.5.2/fair/testing.py
+-rw-r--r--   0        0        0    55154 2023-04-27 13:19:09.284183 fair_cli-0.5.2/fair/user_config/__init__.py
+-rw-r--r--   0        0        0     5023 2023-04-27 13:19:09.284183 fair_cli-0.5.2/fair/user_config/globbing.py
+-rw-r--r--   0        0        0     9510 2023-04-27 13:19:09.285183 fair_cli-0.5.2/fair/user_config/validation.py
+-rw-r--r--   0        0        0     5168 2023-04-28 23:41:25.186481 fair_cli-0.5.2/fair/utilities.py
+-rw-r--r--   0        0        0     1511 2023-04-27 13:19:09.285183 fair_cli-0.5.2/fair/virtualenv.py
+-rw-r--r--   0        0        0     1339 2023-04-27 10:42:03.118817 fair_cli-0.5.2/LICENSE
+-rw-r--r--   0        0        0     2463 2023-04-28 23:41:30.085525 fair_cli-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0    11631 2023-04-27 13:19:09.272183 fair_cli-0.5.2/README.md
+-rw-r--r--   0        0        0    13363 1970-01-01 00:00:00.000000 fair_cli-0.5.2/PKG-INFO
```

### Comparing `fair_cli-0.5.1/CHANGELOG.md` & `fair_cli-0.5.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/CITATION.cff` & `fair_cli-0.5.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/__init__.py` & `fair_cli-0.5.2/fair/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/cli.py` & `fair_cli-0.5.2/fair/cli.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/common.py` & `fair_cli-0.5.2/fair/common.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/configuration/__init__.py` & `fair_cli-0.5.2/fair/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/configuration/validation.py` & `fair_cli-0.5.2/fair/configuration/validation.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/exceptions.py` & `fair_cli-0.5.2/fair/exceptions.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/files.txt` & `fair_cli-0.5.2/fair/files.txt`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/history.py` & `fair_cli-0.5.2/fair/history.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/identifiers.py` & `fair_cli-0.5.2/fair/identifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 ID_URIS = {
     "orcid": "https://orcid.org/",
     "ror": "https://ror.org/",
 }
 
 QUERY_URLS = {
-    "orcid": "https://pub.orcid.org/v2.0/",
+    "orcid": "https://pub.orcid.org/v3.0/",
     "ror": "https://api.ror.org/organizations?query=",
 }
 
 
 def check_orcid(orcid: str) -> typing.Dict:
     """Checks if valid ORCID using ORCID public api
```

### Comparing `fair_cli-0.5.1/fair/logging.py` & `fair_cli-0.5.2/fair/logging.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/register.py` & `fair_cli-0.5.2/fair/register.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/registry/file_formats.json` & `fair_cli-0.5.2/fair/registry/file_formats.json`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/registry/requests.py` & `fair_cli-0.5.2/fair/registry/requests.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/registry/server.py` & `fair_cli-0.5.2/fair/registry/server.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/registry/storage.py` & `fair_cli-0.5.2/fair/registry/storage.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/registry/sync.py` & `fair_cli-0.5.2/fair/registry/sync.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/registry/versioning.py` & `fair_cli-0.5.2/fair/registry/versioning.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/run.py` & `fair_cli-0.5.2/fair/run.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/session.py` & `fair_cli-0.5.2/fair/session.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/staging.py` & `fair_cli-0.5.2/fair/staging.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/templates/__init__.py` & `fair_cli-0.5.2/fair/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/testing.py` & `fair_cli-0.5.2/fair/testing.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/user_config/__init__.py` & `fair_cli-0.5.2/fair/user_config/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/user_config/globbing.py` & `fair_cli-0.5.2/fair/user_config/globbing.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/user_config/validation.py` & `fair_cli-0.5.2/fair/user_config/validation.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/utilities.py` & `fair_cli-0.5.2/fair/utilities.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/fair/virtualenv.py` & `fair_cli-0.5.2/fair/virtualenv.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/LICENSE` & `fair_cli-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/pyproject.toml` & `fair_cli-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   "Environment :: Console",
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS",
   "Operating System :: OS Independent",
 ]
 description = "Synchronization interface for the SCRC FAIR Data Pipeline registry"
 name = "fair-cli"
-version = "0.5.1"
+version = "0.5.2"
 
 homepage = "https://www.fairdatapipeline.org/"
 
 repository = "https://github.com/FAIRDataPipeline/FAIR-CLI"
 
 documentation = "https://www.fairdatapipeline.org/docs/interface/fdp/"
```

### Comparing `fair_cli-0.5.1/README.md` & `fair_cli-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.1/PKG-INFO` & `fair_cli-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair-cli
-Version: 0.5.1
+Version: 0.5.2
 Summary: Synchronization interface for the SCRC FAIR Data Pipeline registry
 Home-page: https://www.fairdatapipeline.org/
 License: BSD-2-Clause
 Keywords: FAIR Data Pipeline,FAIR,Data Management,Provenance
 Author: Richard Reeve
 Author-email: richard.reeve@glasgow.ac.uk
 Requires-Python: >=3.8.0,<4.0.0
```


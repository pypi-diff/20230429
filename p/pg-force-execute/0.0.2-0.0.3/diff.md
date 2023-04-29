# Comparing `tmp/pg_force_execute-0.0.2.tar.gz` & `tmp/pg_force_execute-0.0.3.tar.gz`

## Comparing `pg_force_execute-0.0.2.tar` & `pg_force_execute-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 pg_force_execute-0.0.2/pg_force_execute.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pg_force_execute-0.0.2/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_force_execute-0.0.2/LICENSE
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 pg_force_execute-0.0.2/README.md
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 pg_force_execute-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 pg_force_execute-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 pg_force_execute-0.0.3/pg_force_execute.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pg_force_execute-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_force_execute-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 pg_force_execute-0.0.3/README.md
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 pg_force_execute-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 pg_force_execute-0.0.3/PKG-INFO
```

### Comparing `pg_force_execute-0.0.2/.gitignore` & `pg_force_execute-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_force_execute-0.0.2/LICENSE` & `pg_force_execute-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_force_execute-0.0.2/README.md` & `pg_force_execute-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pg_force_execute-0.0.2/pyproject.toml` & `pg_force_execute-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-force-execute"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Department for International Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "Utility function to run a PostgreSQL query with SQLAlchemy, terminating any queries that block it"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pg_force_execute-0.0.2/PKG-INFO` & `pg_force_execute-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-force-execute
-Version: 0.0.2
+Version: 0.0.3
 Summary: Utility function to run a PostgreSQL query with SQLAlchemy, terminating any queries that block it
 Project-URL: Source, https://github.com/uktrade/pg-force-execute
 Author-email: Department for International Trade <sre@digital.trade.gov.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```


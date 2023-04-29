# Comparing `tmp/mausy5043_common-1.4.3.tar.gz` & `tmp/mausy5043_common-1.4.4.tar.gz`

## Comparing `mausy5043_common-1.4.3.tar` & `mausy5043_common-1.4.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mausy5043_common-1.4.3/.editorconfig
--rw-r--r--   0        0        0    20770 2020-02-02 00:00:00.000000 mausy5043_common-1.4.3/.pylintrc
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 mausy5043_common-1.4.3/BUILDING.md
--rwxr-xr-x   0        0        0     2210 2020-02-02 00:00:00.000000 mausy5043_common-1.4.3/build
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 mausy5043_common-1.4.3/requirements.txt
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 mausy5043_common-1.4.3/tox.ini
--rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 mausy5043_common-1.4.3/src/mausy5043_common/__init__.py
--rwxr-xr-x   0        0        0      951 2020-02-02 00:00:00.000000 mausy5043_common-1.4.3/src/mausy5043_common/funfile.py
--rwxr-xr-x   0        0        0     1396 2020-02-02 00:00:00.000000 mausy5043_common-1.4.3/src/mausy5043_common/funmeteo.py
--rwxr-xr-x   0        0        0      683 2020-02-02 00:00:00.000000 mausy5043_common-1.4.3/src/mausy5043_common/libsignals.py
--rwxr-xr-x   0        0        0     8944 2020-02-02 00:00:00.000000 mausy5043_common-1.4.3/src/mausy5043_common/libsqlite3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mausy5043_common-1.4.3/tests/.placeholder
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 mausy5043_common-1.4.3/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mausy5043_common-1.4.3/LICENSE
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 mausy5043_common-1.4.3/README.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 mausy5043_common-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 mausy5043_common-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mausy5043_common-1.4.4/.editorconfig
+-rw-r--r--   0        0        0    20770 2020-02-02 00:00:00.000000 mausy5043_common-1.4.4/.pylintrc
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 mausy5043_common-1.4.4/BUILDING.md
+-rwxr-xr-x   0        0        0     2210 2020-02-02 00:00:00.000000 mausy5043_common-1.4.4/build
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 mausy5043_common-1.4.4/requirements.txt
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 mausy5043_common-1.4.4/tox.ini
+-rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 mausy5043_common-1.4.4/src/mausy5043_common/__init__.py
+-rwxr-xr-x   0        0        0      951 2020-02-02 00:00:00.000000 mausy5043_common-1.4.4/src/mausy5043_common/funfile.py
+-rwxr-xr-x   0        0        0     1396 2020-02-02 00:00:00.000000 mausy5043_common-1.4.4/src/mausy5043_common/funmeteo.py
+-rwxr-xr-x   0        0        0      683 2020-02-02 00:00:00.000000 mausy5043_common-1.4.4/src/mausy5043_common/libsignals.py
+-rwxr-xr-x   0        0        0     8944 2020-02-02 00:00:00.000000 mausy5043_common-1.4.4/src/mausy5043_common/libsqlite3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mausy5043_common-1.4.4/tests/.placeholder
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 mausy5043_common-1.4.4/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mausy5043_common-1.4.4/LICENSE
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 mausy5043_common-1.4.4/README.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 mausy5043_common-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 mausy5043_common-1.4.4/PKG-INFO
```

### Comparing `mausy5043_common-1.4.3/.pylintrc` & `mausy5043_common-1.4.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.3/BUILDING.md` & `mausy5043_common-1.4.4/BUILDING.md`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.3/build` & `mausy5043_common-1.4.4/build`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.3/tox.ini` & `mausy5043_common-1.4.4/tox.ini`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.3/src/mausy5043_common/funfile.py` & `mausy5043_common-1.4.4/src/mausy5043_common/funfile.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.3/src/mausy5043_common/funmeteo.py` & `mausy5043_common-1.4.4/src/mausy5043_common/funmeteo.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.3/src/mausy5043_common/libsignals.py` & `mausy5043_common-1.4.4/src/mausy5043_common/libsignals.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.3/src/mausy5043_common/libsqlite3.py` & `mausy5043_common-1.4.4/src/mausy5043_common/libsqlite3.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             cursor.close()
             consql.commit()
             consql.close()
             mf.syslog_trace(
                 f"Attached to SQLite3 server: {versql}", syslog.LOG_INFO, self.debug
             )
             mf.syslog_trace(
-                f"Using DB file             : {self.database}@{self.table}",
+                f"Using DB file             : {self.table}@{self.database}",
                 syslog.LOG_INFO,
                 self.debug,
             )
         except s3.Error as her:
             mf.syslog_trace(
                 f"Unexpected SQLite3 error of type {type(her).__name__} during test.",
                 syslog.LOG_CRIT,
```

### Comparing `mausy5043_common-1.4.3/.gitignore` & `mausy5043_common-1.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.3/LICENSE` & `mausy5043_common-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.3/README.md` & `mausy5043_common-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.4.3/pyproject.toml` & `mausy5043_common-1.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mausy5043-common"
 description = "Common python functions"
-version = "1.4.3"
+version = "1.4.4"
 dependencies = [
     "numpy",
     "pandas",
 ]
 authors = [
   { name="Mausy5043" },
 ]
```

### Comparing `mausy5043_common-1.4.3/PKG-INFO` & `mausy5043_common-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mausy5043-common
-Version: 1.4.3
+Version: 1.4.4
 Summary: Common python functions
 Project-URL: Homepage, https://github.com/Mausy5043/mausy5043-common
 Project-URL: Bug Tracker, https://github.com/Mausy5043/mausy5043-common/issues
 Author: Mausy5043
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```


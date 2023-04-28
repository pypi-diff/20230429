# Comparing `tmp/bdew_datetimes-0.3.8.tar.gz` & `tmp/bdew_datetimes-0.3.9.tar.gz`

## Comparing `bdew_datetimes-0.3.8.tar` & `bdew_datetimes-0.3.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/README.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/requirements.in
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/requirements.txt
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/tox.ini
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/.github/dependabot.yml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/.github/workflows/black.yml
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/.github/workflows/linters.yml
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/.github/workflows/release.yml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/src/_bdew_datetimes_version.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/src/bdew_datetimes/__init__.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/src/bdew_datetimes/calendar.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/src/bdew_datetimes/german_strom_and_gas_tag.py
--rw-r--r--   0        0        0     8447 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/src/bdew_datetimes/periods.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/src/bdew_datetimes/py.typed
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/LICENSE
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     6613 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/README.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/requirements.in
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/requirements.txt
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/tox.ini
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/.github/dependabot.yml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/.github/workflows/black.yml
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/.github/workflows/linters.yml
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/.github/workflows/release.yml
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/src/_bdew_datetimes_version.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/src/bdew_datetimes/__init__.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/src/bdew_datetimes/calendar.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/src/bdew_datetimes/german_strom_and_gas_tag.py
+-rw-r--r--   0        0        0     8447 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/src/bdew_datetimes/periods.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/src/bdew_datetimes/py.typed
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/LICENSE
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     6613 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.9/PKG-INFO
```

### Comparing `bdew_datetimes-0.3.8/README.md` & `bdew_datetimes-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.8/tox.ini` & `bdew_datetimes-0.3.9/tox.ini`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.8/.github/dependabot.yml` & `bdew_datetimes-0.3.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.8/.github/workflows/linters.yml` & `bdew_datetimes-0.3.9/.github/workflows/linters.yml`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.8/.github/workflows/packaging_test.yml` & `bdew_datetimes-0.3.9/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.8/.github/workflows/release.yml` & `bdew_datetimes-0.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.8/.github/workflows/unittests.yml` & `bdew_datetimes-0.3.9/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.8/src/bdew_datetimes/calendar.py` & `bdew_datetimes-0.3.9/src/bdew_datetimes/calendar.py`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.8/src/bdew_datetimes/german_strom_and_gas_tag.py` & `bdew_datetimes-0.3.9/src/bdew_datetimes/german_strom_and_gas_tag.py`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.8/src/bdew_datetimes/periods.py` & `bdew_datetimes-0.3.9/src/bdew_datetimes/periods.py`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.8/.gitignore` & `bdew_datetimes-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.8/LICENSE` & `bdew_datetimes-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.8/pyproject.toml` & `bdew_datetimes-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.8/PKG-INFO` & `bdew_datetimes-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdew_datetimes
-Version: 0.3.8
+Version: 0.3.9
 Summary: Generate and work with holidays of the BDEW-Calendar for power and gas in Germany
 Project-URL: Changelog, https://github.com/mj0nez/bdew-datetimes/releases
 Project-URL: Homepage, https://github.com/mj0nez/bdew-datetimes/
 Author: Konstantin Klein
 Author-email: Marcel Johannesmann <mj0nez@fn.de>
 License: MIT
 License-File: LICENSE
```


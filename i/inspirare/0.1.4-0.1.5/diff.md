# Comparing `tmp/inspirare-0.1.4.tar.gz` & `tmp/inspirare-0.1.5.tar.gz`

## Comparing `inspirare-0.1.4.tar` & `inspirare-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 inspirare-0.1.4/src/inspirare/__init__.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 inspirare-0.1.4/src/inspirare/array.py
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 inspirare-0.1.4/src/inspirare/json.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 inspirare-0.1.4/src/inspirare/pattern.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 inspirare-0.1.4/src/inspirare/random.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 inspirare-0.1.4/src/inspirare/system.py
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 inspirare-0.1.4/src/inspirare/time.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 inspirare-0.1.4/LICENSE
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 inspirare-0.1.4/README.md
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 inspirare-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 inspirare-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 inspirare-0.1.5/src/inspirare/__init__.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 inspirare-0.1.5/src/inspirare/array.py
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 inspirare-0.1.5/src/inspirare/json.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 inspirare-0.1.5/src/inspirare/pattern.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 inspirare-0.1.5/src/inspirare/random.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 inspirare-0.1.5/src/inspirare/system.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 inspirare-0.1.5/src/inspirare/time.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 inspirare-0.1.5/LICENSE
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 inspirare-0.1.5/README.md
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 inspirare-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 inspirare-0.1.5/PKG-INFO
```

### Comparing `inspirare-0.1.4/src/inspirare/__init__.py` & `inspirare-0.1.5/src/inspirare/__init__.py`

 * *Files identical despite different names*

### Comparing `inspirare-0.1.4/src/inspirare/array.py` & `inspirare-0.1.5/src/inspirare/array.py`

 * *Files identical despite different names*

### Comparing `inspirare-0.1.4/src/inspirare/json.py` & `inspirare-0.1.5/src/inspirare/json.py`

 * *Files identical despite different names*

### Comparing `inspirare-0.1.4/src/inspirare/pattern.py` & `inspirare-0.1.5/src/inspirare/pattern.py`

 * *Files identical despite different names*

### Comparing `inspirare-0.1.4/src/inspirare/system.py` & `inspirare-0.1.5/src/inspirare/system.py`

 * *Files identical despite different names*

### Comparing `inspirare-0.1.4/src/inspirare/time.py` & `inspirare-0.1.5/src/inspirare/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import arrow 
 
 
+def get_n_days_ago(n):
+    now = arrow.now()
+    return now.shift(days=-(n-1)).date()
+
+    
 def get_timestamp_by_date(date_):
     """日期转时间戳"""
     return arrow.get(date_).timestamp
 
 
 def get_timestamp():
     """获取当前时间戳"""
```

### Comparing `inspirare-0.1.4/LICENSE` & `inspirare-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `inspirare-0.1.4/pyproject.toml` & `inspirare-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "inspirare"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "library of my handy tools"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `inspirare-0.1.4/PKG-INFO` & `inspirare-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspirare
-Version: 0.1.4
+Version: 0.1.5
 Summary: library of my handy tools
 Project-URL: Homepage, https://github.com/inspirare6/inspirare
 Project-URL: Bug Tracker, https://github.com/inspirare6/inspirare/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


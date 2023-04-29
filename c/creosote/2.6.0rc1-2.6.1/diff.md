# Comparing `tmp/creosote-2.6.0rc1-py3-none-any.whl.zip` & `tmp/creosote-2.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 14152 bytes, number of entries: 12
--rw-r--r--  2.0 unx       25 b- defN 20-Feb-02 00:00 creosote/__about__.py
+Zip file size: 14112 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 creosote/__about__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 creosote/__init__.py
 -rw-r--r--  2.0 unx     6597 b- defN 20-Feb-02 00:00 creosote/cli.py
 -rw-r--r--  2.0 unx     1109 b- defN 20-Feb-02 00:00 creosote/formatters.py
 -rw-r--r--  2.0 unx      523 b- defN 20-Feb-02 00:00 creosote/models.py
 -rw-r--r--  2.0 unx     8558 b- defN 20-Feb-02 00:00 creosote/parsers.py
 -rw-r--r--  2.0 unx     9413 b- defN 20-Feb-02 00:00 creosote/resolvers.py
-?rw-r--r--  2.0 unx    13016 b- defN 20-Feb-02 00:00 creosote-2.6.0rc1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 creosote-2.6.0rc1.dist-info/WHEEL
-?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 creosote-2.6.0rc1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1072 b- defN 20-Feb-02 00:00 creosote-2.6.0rc1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      948 b- defN 20-Feb-02 00:00 creosote-2.6.0rc1.dist-info/RECORD
-12 files, 41395 bytes uncompressed, 12564 bytes compressed:  69.6%
+?rw-r--r--  2.0 unx    13013 b- defN 20-Feb-02 00:00 creosote-2.6.1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 creosote-2.6.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 creosote-2.6.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1072 b- defN 20-Feb-02 00:00 creosote-2.6.1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      933 b- defN 20-Feb-02 00:00 creosote-2.6.1.dist-info/RECORD
+12 files, 41374 bytes uncompressed, 12554 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: creosote/parsers.py
 Comment: 
 
 Filename: creosote/resolvers.py
 Comment: 
 
-Filename: creosote-2.6.0rc1.dist-info/METADATA
+Filename: creosote-2.6.1.dist-info/METADATA
 Comment: 
 
-Filename: creosote-2.6.0rc1.dist-info/WHEEL
+Filename: creosote-2.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: creosote-2.6.0rc1.dist-info/entry_points.txt
+Filename: creosote-2.6.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: creosote-2.6.0rc1.dist-info/licenses/LICENSE
+Filename: creosote-2.6.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: creosote-2.6.0rc1.dist-info/RECORD
+Filename: creosote-2.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## creosote/__about__.py

```diff
@@ -1 +1 @@
-__version__ = "2.6.0rc1"
+__version__ = "2.6.1"
```

## Comparing `creosote-2.6.0rc1.dist-info/METADATA` & `creosote-2.6.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creosote
-Version: 2.6.0rc1
+Version: 2.6.1
 Summary: Identify unused dependencies and avoid a bloated virtual environment.
 Project-URL: Source, https://github.com/fredrikaverpil/creosote
 Project-URL: Tracker, https://github.com/fredrikaverpil/creosote/issues
 Author-email: Fredrik Averpil <fredrik.averpil@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: dotty-dict<1.4,>=1.3.1
-Requires-Dist: loguru<0.7,>=0.6.0
+Requires-Dist: loguru<0.8,>=0.6.0
 Requires-Dist: pip-requirements-parser<33.1,>=32.0.1
 Requires-Dist: toml<0.11,>=0.10.2
 Provides-Extra: dev
 Requires-Dist: creosote[lint,test,types]; extra == 'dev'
 Provides-Extra: lint
 Requires-Dist: black; extra == 'lint'
 Requires-Dist: ruff; extra == 'lint'
```

## Comparing `creosote-2.6.0rc1.dist-info/licenses/LICENSE` & `creosote-2.6.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*


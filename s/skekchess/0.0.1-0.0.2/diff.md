# Comparing `tmp/skekchess-0.0.1.tar.gz` & `tmp/skekchess-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skekchess-0.0.1.tar", last modified: Sat Apr 29 15:55:26 2023, max compression
+gzip compressed data, was "skekchess-0.0.2.tar", last modified: Sat Apr 29 16:17:32 2023, max compression
```

## Comparing `skekchess-0.0.1.tar` & `skekchess-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 15:55:26.713775 skekchess-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-04-29 15:50:28.000000 skekchess-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      537 2023-04-29 15:55:26.711933 skekchess-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-04-29 15:52:35.000000 skekchess-0.0.1/README.md
--rw-rw-rw-   0        0        0      453 2023-04-29 15:53:42.000000 skekchess-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 15:55:26.713775 skekchess-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-29 15:55:26.685417 skekchess-0.0.1/src/
--rw-rw-rw-   0        0        0        0 2023-04-28 09:36:12.000000 skekchess-0.0.1/src/__init__.py
--rw-rw-rw-   0        0        0     5680 2023-04-29 08:22:40.000000 skekchess-0.0.1/src/board.py
--rw-rw-rw-   0        0        0    14895 2023-04-29 08:04:53.000000 skekchess-0.0.1/src/chessman.py
--rw-rw-rw-   0        0        0     3390 2023-04-28 09:36:10.000000 skekchess-0.0.1/src/enums.py
--rw-rw-rw-   0        0        0     4424 2023-04-29 08:07:45.000000 skekchess-0.0.1/src/skek_chess.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:55:26.709889 skekchess-0.0.1/src/skekchess.egg-info/
--rw-rw-rw-   0        0        0      537 2023-04-29 15:55:26.000000 skekchess-0.0.1/src/skekchess.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-04-29 15:55:26.000000 skekchess-0.0.1/src/skekchess.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 15:55:26.000000 skekchess-0.0.1/src/skekchess.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-29 15:55:26.000000 skekchess-0.0.1/src/skekchess.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 16:17:32.927236 skekchess-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2023-04-29 15:50:28.000000 skekchess-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      537 2023-04-29 16:17:32.926439 skekchess-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2023-04-29 15:52:35.000000 skekchess-0.0.2/README.md
+-rw-rw-rw-   0        0        0      453 2023-04-29 16:17:09.000000 skekchess-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 16:17:32.927236 skekchess-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 16:17:32.864574 skekchess-0.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-04-28 09:36:12.000000 skekchess-0.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:17:32.908924 skekchess-0.0.2/src/skekchess/
+-rw-rw-rw-   0        0        0     5680 2023-04-29 08:22:40.000000 skekchess-0.0.2/src/skekchess/board.py
+-rw-rw-rw-   0        0        0    14895 2023-04-29 08:04:53.000000 skekchess-0.0.2/src/skekchess/chessman.py
+-rw-rw-rw-   0        0        0     3390 2023-04-28 09:36:10.000000 skekchess-0.0.2/src/skekchess/enums.py
+-rw-rw-rw-   0        0        0     4424 2023-04-29 08:07:45.000000 skekchess-0.0.2/src/skekchess/skek_chess.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:17:32.924476 skekchess-0.0.2/src/skekchess.egg-info/
+-rw-rw-rw-   0        0        0      537 2023-04-29 16:17:32.000000 skekchess-0.0.2/src/skekchess.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-04-29 16:17:32.000000 skekchess-0.0.2/src/skekchess.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 16:17:32.000000 skekchess-0.0.2/src/skekchess.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-29 16:17:32.000000 skekchess-0.0.2/src/skekchess.egg-info/top_level.txt
```

### Comparing `skekchess-0.0.1/LICENSE` & `skekchess-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skekchess-0.0.1/PKG-INFO` & `skekchess-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skekchess
-Version: 0.0.1
+Version: 0.0.2
 Summary: Chess but for my own use.
 Author-email: Skekdog <skekdog@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `skekchess-0.0.1/src/board.py` & `skekchess-0.0.2/src/skekchess/board.py`

 * *Files identical despite different names*

### Comparing `skekchess-0.0.1/src/chessman.py` & `skekchess-0.0.2/src/skekchess/chessman.py`

 * *Files identical despite different names*

### Comparing `skekchess-0.0.1/src/enums.py` & `skekchess-0.0.2/src/skekchess/enums.py`

 * *Files identical despite different names*

### Comparing `skekchess-0.0.1/src/skek_chess.py` & `skekchess-0.0.2/src/skekchess/skek_chess.py`

 * *Files identical despite different names*

### Comparing `skekchess-0.0.1/src/skekchess.egg-info/PKG-INFO` & `skekchess-0.0.2/src/skekchess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skekchess
-Version: 0.0.1
+Version: 0.0.2
 Summary: Chess but for my own use.
 Author-email: Skekdog <skekdog@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```


# Comparing `tmp/xcpcio_board_spider-0.0.3.tar.gz` & `tmp/xcpcio_board_spider-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcpcio_board_spider-0.0.3.tar", max compression
+gzip compressed data, was "xcpcio_board_spider-0.0.4.tar", max compression
```

## Comparing `xcpcio_board_spider-0.0.3.tar` & `xcpcio_board_spider-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2023-04-29 17:18:32.055767 xcpcio_board_spider-0.0.3/LICENSE
--rw-r--r--   0        0        0      538 2023-04-29 17:18:32.055767 xcpcio_board_spider-0.0.3/README.md
--rw-r--r--   0        0        0      977 2023-04-29 17:18:32.059767 xcpcio_board_spider-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-29 17:18:32.059767 xcpcio_board_spider-0.0.3/xcpcio_board_spider/__init__.py
--rw-r--r--   0        0        0     1851 2023-04-29 17:18:32.059767 xcpcio_board_spider-0.0.3/xcpcio_board_spider/utils.py
--rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 xcpcio_board_spider-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-29 17:21:52.609006 xcpcio_board_spider-0.0.4/LICENSE
+-rw-r--r--   0        0        0      538 2023-04-29 17:21:52.609006 xcpcio_board_spider-0.0.4/README.md
+-rw-r--r--   0        0        0      977 2023-04-29 17:21:52.613006 xcpcio_board_spider-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-29 17:21:52.613006 xcpcio_board_spider-0.0.4/xcpcio_board_spider/__init__.py
+-rw-r--r--   0        0        0     1851 2023-04-29 17:21:52.613006 xcpcio_board_spider-0.0.4/xcpcio_board_spider/utils.py
+-rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 xcpcio_board_spider-0.0.4/PKG-INFO
```

### Comparing `xcpcio_board_spider-0.0.3/LICENSE` & `xcpcio_board_spider-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.3/README.md` & `xcpcio_board_spider-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.3/pyproject.toml` & `xcpcio_board_spider-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcpcio-board-spider"
-version = "0.0.3"
+version = "0.0.4"
 description = "XCPCIO Board Spider"
 authors = ["Dup4 <lyuzhi.pan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `xcpcio_board_spider-0.0.3/xcpcio_board_spider/utils.py` & `xcpcio_board_spider-0.0.4/xcpcio_board_spider/utils.py`

 * *Files identical despite different names*

### Comparing `xcpcio_board_spider-0.0.3/PKG-INFO` & `xcpcio_board_spider-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcpcio-board-spider
-Version: 0.0.3
+Version: 0.0.4
 Summary: XCPCIO Board Spider
 License: MIT
 Author: Dup4
 Author-email: lyuzhi.pan@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


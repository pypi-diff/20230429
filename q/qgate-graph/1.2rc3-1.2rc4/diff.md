# Comparing `tmp/qgate_graph-1.2rc3.tar.gz` & `tmp/qgate_graph-1.2rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgate_graph-1.2rc3.tar", last modified: Sat Apr 29 10:06:55 2023, max compression
+gzip compressed data, was "qgate_graph-1.2rc4.tar", last modified: Sat Apr 29 10:09:11 2023, max compression
```

## Comparing `qgate_graph-1.2rc3.tar` & `qgate_graph-1.2rc4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 10:06:55.161824 qgate_graph-1.2rc3/
--rw-rw-rw-   0        0        0      392 2023-04-29 10:06:55.161824 qgate_graph-1.2rc3/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-04-27 20:17:36.000000 qgate_graph-1.2rc3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 10:06:55.102575 qgate_graph-1.2rc3/qgate_graph/
--rw-rw-rw-   0        0        0       40 2023-04-29 09:53:53.000000 qgate_graph-1.2rc3/qgate_graph/__init__.py
--rw-rw-rw-   0        0        0      913 2023-04-27 20:17:36.000000 qgate_graph-1.2rc3/qgate_graph/constant.py
--rw-rw-rw-   0        0        0     8695 2023-04-29 09:32:27.000000 qgate_graph-1.2rc3/qgate_graph/graph.py
--rw-rw-rw-   0        0        0      218 2023-04-29 09:57:08.000000 qgate_graph-1.2rc3/qgate_graph/version.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:06:55.153725 qgate_graph-1.2rc3/qgate_graph.egg-info/
--rw-rw-rw-   0        0        0      392 2023-04-29 10:06:54.000000 qgate_graph-1.2rc3/qgate_graph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-04-29 10:06:54.000000 qgate_graph-1.2rc3/qgate_graph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 10:06:54.000000 qgate_graph-1.2rc3/qgate_graph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-29 10:06:54.000000 qgate_graph-1.2rc3/qgate_graph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 10:06:54.000000 qgate_graph-1.2rc3/qgate_graph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 10:06:55.161824 qgate_graph-1.2rc3/setup.cfg
--rw-rw-rw-   0        0        0     1071 2023-04-29 09:54:54.000000 qgate_graph-1.2rc3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:09:11.395226 qgate_graph-1.2rc4/
+-rw-rw-rw-   0        0        0      392 2023-04-29 10:09:11.395226 qgate_graph-1.2rc4/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-04-27 20:17:36.000000 qgate_graph-1.2rc4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 10:09:11.346701 qgate_graph-1.2rc4/qgate_graph/
+-rw-rw-rw-   0        0        0       40 2023-04-29 09:53:53.000000 qgate_graph-1.2rc4/qgate_graph/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-04-27 20:17:36.000000 qgate_graph-1.2rc4/qgate_graph/constant.py
+-rw-rw-rw-   0        0        0     8695 2023-04-29 09:32:27.000000 qgate_graph-1.2rc4/qgate_graph/graph.py
+-rw-rw-rw-   0        0        0      217 2023-04-29 10:08:43.000000 qgate_graph-1.2rc4/qgate_graph/version.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:09:11.378921 qgate_graph-1.2rc4/qgate_graph.egg-info/
+-rw-rw-rw-   0        0        0      392 2023-04-29 10:09:11.000000 qgate_graph-1.2rc4/qgate_graph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-29 10:09:11.000000 qgate_graph-1.2rc4/qgate_graph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 10:09:11.000000 qgate_graph-1.2rc4/qgate_graph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-29 10:09:11.000000 qgate_graph-1.2rc4/qgate_graph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 10:09:11.000000 qgate_graph-1.2rc4/qgate_graph.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 10:09:11.395226 qgate_graph-1.2rc4/setup.cfg
+-rw-rw-rw-   0        0        0     1071 2023-04-29 09:54:54.000000 qgate_graph-1.2rc4/setup.py
```

### Comparing `qgate_graph-1.2rc3/qgate_graph/constant.py` & `qgate_graph-1.2rc4/qgate_graph/constant.py`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.2rc3/qgate_graph/graph.py` & `qgate_graph-1.2rc4/qgate_graph/graph.py`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.2rc3/setup.py` & `qgate_graph-1.2rc4/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/d2py-0.3.7.tar.gz` & `tmp/d2py-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d2py-0.3.7.tar", last modified: Tue Mar 14 11:19:19 2023, max compression
+gzip compressed data, was "d2py-0.3.8.tar", last modified: Sat Apr 29 06:20:39 2023, max compression
```

## Comparing `d2py-0.3.7.tar` & `d2py-0.3.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2023-01-11 11:03:09.486667 d2py-0.3.7/LICENSE
--rw-r--r--   0        0        0     2103 2023-01-11 11:03:09.486667 d2py-0.3.7/README.md
--rw-r--r--   0        0        0     1366 2023-03-11 05:31:14.723945 d2py-0.3.7/pyproject.toml
--rw-r--r--   0        0        0       46 2023-03-14 11:18:47.512331 d2py-0.3.7/src/d2py/__init__.py
--rw-r--r--   0        0        0        0 2023-01-11 11:03:09.506667 d2py-0.3.7/src/d2py/abc/__init__.py
--rw-r--r--   0        0        0     2036 2023-01-11 11:03:09.506667 d2py-0.3.7/src/d2py/abc/draft/runner.py
--rw-r--r--   0        0        0        0 2023-01-11 11:03:09.506667 d2py-0.3.7/src/d2py/abc/profile.py
--rw-r--r--   0        0        0     1857 2023-01-11 11:03:09.506667 d2py-0.3.7/src/d2py/abc/trace_code.py
--rw-r--r--   0        0        0     2591 2023-01-11 11:03:09.510668 d2py-0.3.7/src/d2py/abc/validate.py
--rw-r--r--   0        0        0       35 2023-01-11 11:03:09.510668 d2py-0.3.7/src/d2py/algebra/__init__.py
--rw-r--r--   0        0        0       36 2023-01-11 11:03:09.510668 d2py-0.3.7/src/d2py/analysis/__init__.py
--rw-r--r--   0        0        0       38 2023-01-11 11:03:09.510668 d2py-0.3.7/src/d2py/analysis/numbers.py
--rw-r--r--   0        0        0      590 2023-01-14 05:19:51.736610 d2py-0.3.7/src/d2py/download/__init__.py
--rw-r--r--   0        0        0       64 2023-03-14 10:59:06.935018 d2py-0.3.7/src/d2py/quantum/__init__.py
--rw-r--r--   0        0        0       22 2023-03-14 10:59:53.852198 d2py-0.3.7/src/d2py/quantum/graph/__init__.py
--rw-r--r--   0        0        0      213 2023-03-14 11:17:12.813585 d2py-0.3.7/src/d2py/quantum/graph/tree.py
--rw-r--r--   0        0        0     1415 2023-03-11 05:53:42.880146 d2py-0.3.7/src/d2py/timeitx.py
--rw-r--r--   0        0        0      865 2023-01-11 11:03:09.510668 d2py-0.3.7/src/d2py/tools/write/__init__.py
--rw-r--r--   0        0        0     2294 2023-01-11 11:03:09.510668 d2py-0.3.7/src/d2py/tools/write/_docs.py
--rw-r--r--   0        0        0     1656 2023-01-11 11:03:09.510668 d2py-0.3.7/src/d2py/tools/write/doc.py
--rw-r--r--   0        0        0      205 2023-01-11 11:03:09.510668 d2py-0.3.7/src/d2py/tools/write/release.py
--rw-r--r--   0        0        0       17 2023-01-11 11:03:09.510668 d2py-0.3.7/src/d2py/utils/__init__.py
--rw-r--r--   0        0        0      178 2023-01-14 05:52:34.779543 d2py-0.3.7/src/d2py/utils/file.py
--rw-r--r--   0        0        0     1120 2023-01-11 11:03:09.510668 d2py-0.3.7/src/d2py/utils/unzip.py
--rw-r--r--   0        0        0     3855 1970-01-01 00:00:00.000000 d2py-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-11 11:03:09.486667 d2py-0.3.8/LICENSE
+-rw-r--r--   0        0        0     2103 2023-01-11 11:03:09.486667 d2py-0.3.8/README.md
+-rw-r--r--   0        0        0     1365 2023-04-29 06:19:58.117404 d2py-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-04-29 06:20:10.997708 d2py-0.3.8/src/d2py/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-11 11:03:09.506667 d2py-0.3.8/src/d2py/abc/__init__.py
+-rw-r--r--   0        0        0     2036 2023-01-11 11:03:09.506667 d2py-0.3.8/src/d2py/abc/draft/runner.py
+-rw-r--r--   0        0        0        0 2023-01-11 11:03:09.506667 d2py-0.3.8/src/d2py/abc/profile.py
+-rw-r--r--   0        0        0     1857 2023-01-11 11:03:09.506667 d2py-0.3.8/src/d2py/abc/trace_code.py
+-rw-r--r--   0        0        0     2591 2023-01-11 11:03:09.510668 d2py-0.3.8/src/d2py/abc/validate.py
+-rw-r--r--   0        0        0       35 2023-01-11 11:03:09.510668 d2py-0.3.8/src/d2py/algebra/__init__.py
+-rw-r--r--   0        0        0       36 2023-01-11 11:03:09.510668 d2py-0.3.8/src/d2py/analysis/__init__.py
+-rw-r--r--   0        0        0       38 2023-01-11 11:03:09.510668 d2py-0.3.8/src/d2py/analysis/numbers.py
+-rw-r--r--   0        0        0      590 2023-01-14 05:19:51.736610 d2py-0.3.8/src/d2py/download/__init__.py
+-rw-r--r--   0        0        0       64 2023-03-14 10:59:06.935018 d2py-0.3.8/src/d2py/quantum/__init__.py
+-rw-r--r--   0        0        0       22 2023-03-14 10:59:53.852198 d2py-0.3.8/src/d2py/quantum/graph/__init__.py
+-rw-r--r--   0        0        0      213 2023-03-14 11:17:12.813585 d2py-0.3.8/src/d2py/quantum/graph/tree.py
+-rw-r--r--   0        0        0     1415 2023-03-11 05:53:42.880146 d2py-0.3.8/src/d2py/timeitx.py
+-rw-r--r--   0        0        0      865 2023-01-11 11:03:09.510668 d2py-0.3.8/src/d2py/tools/write/__init__.py
+-rw-r--r--   0        0        0     2294 2023-01-11 11:03:09.510668 d2py-0.3.8/src/d2py/tools/write/_docs.py
+-rw-r--r--   0        0        0     1656 2023-01-11 11:03:09.510668 d2py-0.3.8/src/d2py/tools/write/doc.py
+-rw-r--r--   0        0        0      205 2023-01-11 11:03:09.510668 d2py-0.3.8/src/d2py/tools/write/release.py
+-rw-r--r--   0        0        0       17 2023-01-11 11:03:09.510668 d2py-0.3.8/src/d2py/utils/__init__.py
+-rw-r--r--   0        0        0      178 2023-01-14 05:52:34.779543 d2py-0.3.8/src/d2py/utils/file.py
+-rw-r--r--   0        0        0     1120 2023-01-11 11:03:09.510668 d2py-0.3.8/src/d2py/utils/unzip.py
+-rw-r--r--   0        0        0     3854 1970-01-01 00:00:00.000000 d2py-0.3.8/PKG-INFO
```

### Comparing `d2py-0.3.7/LICENSE` & `d2py-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `d2py-0.3.7/README.md` & `d2py-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `d2py-0.3.7/pyproject.toml` & `d2py-0.3.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 authors = [{name = "xinetzone", email = "735613050@qq.com"}]
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 dynamic = ["version", "description"]
 license = {file = "LICENSE"}
 name = "d2py"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 
 dependencies = [
   "invoke",
   "pdm",
   "PyGithub[integrations]",
   "bytecode",
   "numpy"
```

### Comparing `d2py-0.3.7/src/d2py/abc/draft/runner.py` & `d2py-0.3.8/src/d2py/abc/draft/runner.py`

 * *Files identical despite different names*

### Comparing `d2py-0.3.7/src/d2py/abc/trace_code.py` & `d2py-0.3.8/src/d2py/abc/trace_code.py`

 * *Files identical despite different names*

### Comparing `d2py-0.3.7/src/d2py/abc/validate.py` & `d2py-0.3.8/src/d2py/abc/validate.py`

 * *Files identical despite different names*

### Comparing `d2py-0.3.7/src/d2py/download/__init__.py` & `d2py-0.3.8/src/d2py/download/__init__.py`

 * *Files identical despite different names*

### Comparing `d2py-0.3.7/src/d2py/timeitx.py` & `d2py-0.3.8/src/d2py/timeitx.py`

 * *Files identical despite different names*

### Comparing `d2py-0.3.7/src/d2py/tools/write/__init__.py` & `d2py-0.3.8/src/d2py/tools/write/__init__.py`

 * *Files identical despite different names*

### Comparing `d2py-0.3.7/src/d2py/tools/write/_docs.py` & `d2py-0.3.8/src/d2py/tools/write/_docs.py`

 * *Files identical despite different names*

### Comparing `d2py-0.3.7/src/d2py/tools/write/doc.py` & `d2py-0.3.8/src/d2py/tools/write/doc.py`

 * *Files identical despite different names*

### Comparing `d2py-0.3.7/src/d2py/utils/unzip.py` & `d2py-0.3.8/src/d2py/utils/unzip.py`

 * *Files identical despite different names*

### Comparing `d2py-0.3.7/PKG-INFO` & `d2py-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: d2py
-Version: 0.3.7
+Version: 0.3.8
 Summary: Dive into Python.
 Author-email: xinetzone <735613050@qq.com>
 Maintainer-email: xinetzone <735613050@qq.com>
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: invoke
 Requires-Dist: pdm
 Requires-Dist: PyGithub[integrations]
 Requires-Dist: bytecode
 Requires-Dist: numpy
```


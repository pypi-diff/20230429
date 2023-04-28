# Comparing `tmp/CalSciPy-0.2.2.tar.gz` & `tmp/CalSciPy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CalSciPy-0.2.2.tar", last modified: Fri Apr 28 15:08:19 2023, max compression
+gzip compressed data, was "CalSciPy-0.2.3.tar", last modified: Fri Apr 28 22:03:12 2023, max compression
```

## Comparing `CalSciPy-0.2.2.tar` & `CalSciPy-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 15:08:19.358989 CalSciPy-0.2.2/
--rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     4998 2023-04-28 15:08:19.357988 CalSciPy-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2840 2023-04-03 15:47:56.000000 CalSciPy-0.2.2/README.md
--rw-rw-rw-   0        0        0     2330 2023-04-28 15:07:52.000000 CalSciPy-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 15:08:19.358989 CalSciPy-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 15:08:19.311988 CalSciPy-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 15:08:19.332989 CalSciPy-0.2.2/src/CalSciPy/
--rw-rw-rw-   0        0        0      388 2023-04-03 13:04:29.000000 CalSciPy-0.2.2/src/CalSciPy/__init__.py
--rw-rw-rw-   0        0        0    11403 2023-04-05 15:38:36.000000 CalSciPy-0.2.2/src/CalSciPy/bruker.py
--rw-rw-rw-   0        0        0     3028 2023-04-07 16:45:41.000000 CalSciPy-0.2.2/src/CalSciPy/coloring.py
--rw-rw-rw-   0        0        0     2237 2023-04-03 13:04:29.000000 CalSciPy-0.2.2/src/CalSciPy/event_processing.py
--rw-rw-rw-   0        0        0     2388 2023-04-28 15:05:04.000000 CalSciPy-0.2.2/src/CalSciPy/image_processing.py
--rw-rw-rw-   0        0        0     9653 2023-04-26 15:19:07.000000 CalSciPy-0.2.2/src/CalSciPy/io_tools.py
--rw-rw-rw-   0        0        0     6019 2023-04-28 15:07:33.000000 CalSciPy-0.2.2/src/CalSciPy/misc.py
--rw-rw-rw-   0        0        0     3444 2023-03-29 17:06:08.000000 CalSciPy-0.2.2/src/CalSciPy/reorganization.py
--rw-rw-rw-   0        0        0     4770 2023-03-29 21:13:37.000000 CalSciPy-0.2.2/src/CalSciPy/trace_processing.py
--rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.2.2/src/CalSciPy/version.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:08:19.340989 CalSciPy-0.2.2/src/CalSciPy.egg-info/
--rw-rw-rw-   0        0        0     4998 2023-04-28 15:08:19.000000 CalSciPy-0.2.2/src/CalSciPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      701 2023-04-28 15:08:19.000000 CalSciPy-0.2.2/src/CalSciPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 15:08:19.000000 CalSciPy-0.2.2/src/CalSciPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      365 2023-04-28 15:08:19.000000 CalSciPy-0.2.2/src/CalSciPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-28 15:08:19.000000 CalSciPy-0.2.2/src/CalSciPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.2.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:08:19.355989 CalSciPy-0.2.2/tests/
--rw-rw-rw-   0        0        0     1933 2023-04-03 13:04:29.000000 CalSciPy-0.2.2/tests/test_a_install.py
--rw-rw-rw-   0        0        0     3074 2023-04-05 17:07:30.000000 CalSciPy-0.2.2/tests/test_bruker.py
--rw-rw-rw-   0        0        0      887 2023-04-07 16:44:54.000000 CalSciPy-0.2.2/tests/test_coloring.py
--rw-rw-rw-   0        0        0     1218 2023-04-03 15:39:20.000000 CalSciPy-0.2.2/tests/test_event_processing.py
--rw-rw-rw-   0        0        0    12735 2023-04-05 16:39:27.000000 CalSciPy-0.2.2/tests/test_io_tools.py
--rw-rw-rw-   0        0        0     2373 2023-04-05 15:55:20.000000 CalSciPy-0.2.2/tests/test_misc.py
--rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.2.2/tests/test_reorganization.py
--rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.2.2/tests/test_trace_processing.py
+drwxrwxrwx   0        0        0        0 2023-04-28 22:03:12.598456 CalSciPy-0.2.3/
+-rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     4998 2023-04-28 22:03:12.597450 CalSciPy-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2840 2023-04-03 15:47:56.000000 CalSciPy-0.2.3/README.md
+-rw-rw-rw-   0        0        0     2330 2023-04-28 22:02:45.000000 CalSciPy-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 22:03:12.598456 CalSciPy-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 22:03:12.549425 CalSciPy-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 22:03:12.570453 CalSciPy-0.2.3/src/CalSciPy/
+-rw-rw-rw-   0        0        0      388 2023-04-03 13:04:29.000000 CalSciPy-0.2.3/src/CalSciPy/__init__.py
+-rw-rw-rw-   0        0        0    11403 2023-04-05 15:38:36.000000 CalSciPy-0.2.3/src/CalSciPy/bruker.py
+-rw-rw-rw-   0        0        0     3028 2023-04-07 16:45:41.000000 CalSciPy-0.2.3/src/CalSciPy/coloring.py
+-rw-rw-rw-   0        0        0     2237 2023-04-03 13:04:29.000000 CalSciPy-0.2.3/src/CalSciPy/event_processing.py
+-rw-rw-rw-   0        0        0     4621 2023-04-28 22:02:25.000000 CalSciPy-0.2.3/src/CalSciPy/image_processing.py
+-rw-rw-rw-   0        0        0     9653 2023-04-26 15:19:07.000000 CalSciPy-0.2.3/src/CalSciPy/io_tools.py
+-rw-rw-rw-   0        0        0     5917 2023-04-28 16:24:44.000000 CalSciPy-0.2.3/src/CalSciPy/misc.py
+-rw-rw-rw-   0        0        0     3444 2023-03-29 17:06:08.000000 CalSciPy-0.2.3/src/CalSciPy/reorganization.py
+-rw-rw-rw-   0        0        0     4770 2023-03-29 21:13:37.000000 CalSciPy-0.2.3/src/CalSciPy/trace_processing.py
+-rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.2.3/src/CalSciPy/version.py
+drwxrwxrwx   0        0        0        0 2023-04-28 22:03:12.579450 CalSciPy-0.2.3/src/CalSciPy.egg-info/
+-rw-rw-rw-   0        0        0     4998 2023-04-28 22:03:12.000000 CalSciPy-0.2.3/src/CalSciPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      701 2023-04-28 22:03:12.000000 CalSciPy-0.2.3/src/CalSciPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 22:03:12.000000 CalSciPy-0.2.3/src/CalSciPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      365 2023-04-28 22:03:12.000000 CalSciPy-0.2.3/src/CalSciPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-28 22:03:12.000000 CalSciPy-0.2.3/src/CalSciPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.2.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 22:03:12.595449 CalSciPy-0.2.3/tests/
+-rw-rw-rw-   0        0        0     1933 2023-04-03 13:04:29.000000 CalSciPy-0.2.3/tests/test_a_install.py
+-rw-rw-rw-   0        0        0     3074 2023-04-05 17:07:30.000000 CalSciPy-0.2.3/tests/test_bruker.py
+-rw-rw-rw-   0        0        0      887 2023-04-07 16:44:54.000000 CalSciPy-0.2.3/tests/test_coloring.py
+-rw-rw-rw-   0        0        0     1218 2023-04-03 15:39:20.000000 CalSciPy-0.2.3/tests/test_event_processing.py
+-rw-rw-rw-   0        0        0    12735 2023-04-05 16:39:27.000000 CalSciPy-0.2.3/tests/test_io_tools.py
+-rw-rw-rw-   0        0        0     2373 2023-04-05 15:55:20.000000 CalSciPy-0.2.3/tests/test_misc.py
+-rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.2.3/tests/test_reorganization.py
+-rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.2.3/tests/test_trace_processing.py
```

### Comparing `CalSciPy-0.2.2/LICENSE` & `CalSciPy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.2/PKG-INFO` & `CalSciPy-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.2.2
+Version: 0.2.3
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
```

### Comparing `CalSciPy-0.2.2/README.md` & `CalSciPy-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.2/pyproject.toml` & `CalSciPy-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CalSciPy"
-version = "0.2.2"
+version = "0.2.3"
 description = "A collection"
 readme = "README.md"
 requires-python = ">=3.7, <4"
 license = {file = "LICENSE"}
 keywords = ["CalSciPy", "Calcium Imaging"]
 authors = [
   {name = "Darik A. O'Neil"}
```

### Comparing `CalSciPy-0.2.2/src/CalSciPy/bruker.py` & `CalSciPy-0.2.3/src/CalSciPy/bruker.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.2/src/CalSciPy/coloring.py` & `CalSciPy-0.2.3/src/CalSciPy/coloring.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.2/src/CalSciPy/event_processing.py` & `CalSciPy-0.2.3/src/CalSciPy/event_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.2/src/CalSciPy/io_tools.py` & `CalSciPy-0.2.3/src/CalSciPy/io_tools.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.2/src/CalSciPy/misc.py` & `CalSciPy-0.2.3/src/CalSciPy/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,18 +118,18 @@
     :param cupy_function: any cupy function that accepts numpy arrays
     :type cupy_function: Callable
     :return: wrapped function
     :rtype: Callable
     """
     @wraps(cupy_function)
     def decorator(*args, **kwargs) -> Callable:
-        for arg in args:
-            if isinstance(arg, np.ndarray):
-                arg = cupy.asarray(arg, dtype=arg.dtype)  # Not here that I am not ensuring matched to the arrays
-                # memory order. I simply am not sure how...
+        args = list(args)
+        if isinstance(args[0], np.ndarray):
+            args[0] = cupy.asarray(args[0])
+        args = tuple(args)
         return cupy_function(*args, **kwargs).get()
     return decorator
 
 
 class PatternMatching:
     def __init__(self, value: Any, comparison_expressions: Iterable[Any]):
         """
```

### Comparing `CalSciPy-0.2.2/src/CalSciPy/reorganization.py` & `CalSciPy-0.2.3/src/CalSciPy/reorganization.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.2/src/CalSciPy/trace_processing.py` & `CalSciPy-0.2.3/src/CalSciPy/trace_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.2/src/CalSciPy.egg-info/PKG-INFO` & `CalSciPy-0.2.3/src/CalSciPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.2.2
+Version: 0.2.3
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
```

### Comparing `CalSciPy-0.2.2/src/CalSciPy.egg-info/SOURCES.txt` & `CalSciPy-0.2.3/src/CalSciPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.2/tests/test_a_install.py` & `CalSciPy-0.2.3/tests/test_a_install.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.2/tests/test_bruker.py` & `CalSciPy-0.2.3/tests/test_bruker.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.2/tests/test_coloring.py` & `CalSciPy-0.2.3/tests/test_coloring.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.2/tests/test_event_processing.py` & `CalSciPy-0.2.3/tests/test_event_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.2/tests/test_io_tools.py` & `CalSciPy-0.2.3/tests/test_io_tools.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.2/tests/test_misc.py` & `CalSciPy-0.2.3/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.2/tests/test_reorganization.py` & `CalSciPy-0.2.3/tests/test_reorganization.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.2/tests/test_trace_processing.py` & `CalSciPy-0.2.3/tests/test_trace_processing.py`

 * *Files identical despite different names*


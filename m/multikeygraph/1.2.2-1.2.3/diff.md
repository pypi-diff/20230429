# Comparing `tmp/multikeygraph-1.2.2.tar.gz` & `tmp/multikeygraph-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multikeygraph-1.2.2.tar", last modified: Sun Aug 14 17:10:50 2022, max compression
+gzip compressed data, was "multikeygraph-1.2.3.tar", last modified: Sat Apr 29 12:32:11 2023, max compression
```

## Comparing `multikeygraph-1.2.2.tar` & `multikeygraph-1.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2022-08-14 17:10:50.257998 multikeygraph-1.2.2/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1127 2021-04-19 22:55:53.000000 multikeygraph-1.2.2/LICENSE
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1863 2022-08-14 17:10:50.257998 multikeygraph-1.2.2/PKG-INFO
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1406 2021-04-19 22:55:53.000000 multikeygraph-1.2.2/README.md
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2022-08-14 17:10:50.256998 multikeygraph-1.2.2/multikeygraph/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)    11204 2022-08-14 17:08:40.000000 multikeygraph-1.2.2/multikeygraph/__init__.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     6683 2022-04-14 23:31:45.000000 multikeygraph-1.2.2/multikeygraph/main.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2022-08-14 17:10:50.257998 multikeygraph-1.2.2/multikeygraph.egg-info/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1863 2022-08-14 17:10:50.000000 multikeygraph-1.2.2/multikeygraph.egg-info/PKG-INFO
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      262 2022-08-14 17:10:50.000000 multikeygraph-1.2.2/multikeygraph.egg-info/SOURCES.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        1 2022-08-14 17:10:50.000000 multikeygraph-1.2.2/multikeygraph.egg-info/dependency_links.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)       61 2022-08-14 17:10:50.000000 multikeygraph-1.2.2/multikeygraph.egg-info/entry_points.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)       14 2022-08-14 17:10:50.000000 multikeygraph-1.2.2/multikeygraph.egg-info/top_level.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2022-08-14 17:10:50.257998 multikeygraph-1.2.2/setup.cfg
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      822 2022-08-14 17:10:37.000000 multikeygraph-1.2.2/setup.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-29 12:32:11.451243 multikeygraph-1.2.3/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1127 2021-04-19 22:55:53.000000 multikeygraph-1.2.3/LICENSE
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1826 2023-04-29 12:32:11.451243 multikeygraph-1.2.3/PKG-INFO
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1406 2021-04-19 22:55:53.000000 multikeygraph-1.2.3/README.md
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-29 12:32:11.450244 multikeygraph-1.2.3/multikeygraph/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)    11271 2023-04-19 13:48:57.000000 multikeygraph-1.2.3/multikeygraph/__init__.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     6683 2022-04-14 23:31:45.000000 multikeygraph-1.2.3/multikeygraph/main.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-29 12:32:11.451243 multikeygraph-1.2.3/multikeygraph.egg-info/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1826 2023-04-29 12:32:11.000000 multikeygraph-1.2.3/multikeygraph.egg-info/PKG-INFO
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      262 2023-04-29 12:32:11.000000 multikeygraph-1.2.3/multikeygraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        1 2023-04-29 12:32:11.000000 multikeygraph-1.2.3/multikeygraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)       60 2023-04-29 12:32:11.000000 multikeygraph-1.2.3/multikeygraph.egg-info/entry_points.txt
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)       14 2023-04-29 12:32:11.000000 multikeygraph-1.2.3/multikeygraph.egg-info/top_level.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-04-29 12:32:11.452243 multikeygraph-1.2.3/setup.cfg
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      822 2023-04-19 13:50:28.000000 multikeygraph-1.2.3/setup.py
```

### Comparing `multikeygraph-1.2.2/LICENSE` & `multikeygraph-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multikeygraph-1.2.2/PKG-INFO` & `multikeygraph-1.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: multikeygraph
-Version: 1.2.2
+Version: 1.2.3
 Summary: Plot multiple keys on multiple graphs in a pyfsdb/FSDB file.
 Home-page: https://github.com/gawseed/multikeygraph
 Author: Wes Hardaker
 Author-email: opensource@hardakers.net
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # About
@@ -58,9 +56,7 @@
 Wes Hardaker @ USC/ISI
 
 # See also
 
 The FSDB website and manual page for the original perl module: 
 
 https://www.isi.edu/~johnh/SOFTWARE/FSDB/
-
-
```

### Comparing `multikeygraph-1.2.2/README.md` & `multikeygraph-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `multikeygraph-1.2.2/multikeygraph/__init__.py` & `multikeygraph-1.2.3/multikeygraph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/python3
 
 # ick, remote during packaging:
 from pyfsdb import Fsdb
 import matplotlib
 import matplotlib.lines
+import datetime
 
 plt = None
 dates = None
 
 
 class MultiKeyGraph(object):
 
@@ -154,15 +155,15 @@
                 if label in legend_map:
                     label = legend_map[label]
 
                 # convert the xaxis data to time data for better label printing
                 if no_dates:
                     xdata = col_data[column][key]['x']
                 else:
-                    xdata = dates.epoch2num(col_data[column][key]['x'])
+                    xdata = [datetime.datetime.utcfromtimestamp(x) for x in col_data[column][key]['x']]
                     formatter = dates.DateFormatter("%Y/%m/%d\n%H:%M")
                     axs[n].xaxis.set_major_formatter(formatter)
 
                 if use_dots:
                     marker = '.'
                 else:
                     marker = markers[m % len(markers)]
@@ -181,15 +182,15 @@
                 if len(col_data[column][key]['y']) > 0:
                     miny = min(miny, min(col_data[column][key]['y']))
                     maxy = max(maxy, max(col_data[column][key]['y']))
 
             if time_markers:
                 for marker in time_markers:
                     if not no_dates:
-                        marker = dates.epoch2num(marker)
+                        marker = datetime.datetime.utcfromtimestamp(marker)
                     axs[n].plot([marker, marker],
                                 [miny, maxy],
                                 alpha=.4, color='black')
 
             # if there was anything to actually plot... add the legend
             if n == 0:
                 if (len(col_data[column]) <= 10 and not no_legend) or \
```

### Comparing `multikeygraph-1.2.2/multikeygraph/main.py` & `multikeygraph-1.2.3/multikeygraph/main.py`

 * *Files identical despite different names*

### Comparing `multikeygraph-1.2.2/multikeygraph.egg-info/PKG-INFO` & `multikeygraph-1.2.3/multikeygraph.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: multikeygraph
-Version: 1.2.2
+Version: 1.2.3
 Summary: Plot multiple keys on multiple graphs in a pyfsdb/FSDB file.
 Home-page: https://github.com/gawseed/multikeygraph
 Author: Wes Hardaker
 Author-email: opensource@hardakers.net
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # About
@@ -58,9 +56,7 @@
 Wes Hardaker @ USC/ISI
 
 # See also
 
 The FSDB website and manual page for the original perl module: 
 
 https://www.isi.edu/~johnh/SOFTWARE/FSDB/
-
-
```

### Comparing `multikeygraph-1.2.2/setup.py` & `multikeygraph-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="multikeygraph",
-    version="1.2.2",
+    version="1.2.3",
     author="Wes Hardaker",
     author_email="opensource@hardakers.net",
     description="Plot multiple keys on multiple graphs in a pyfsdb/FSDB file.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gawseed/multikeygraph",
     packages=setuptools.find_packages(),
```


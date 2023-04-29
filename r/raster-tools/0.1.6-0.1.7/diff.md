# Comparing `tmp/raster-tools-0.1.6.tar.gz` & `tmp/raster-tools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster-tools-0.1.6.tar", last modified: Sat Apr 22 00:03:06 2023, max compression
+gzip compressed data, was "raster-tools-0.1.7.tar", last modified: Sat Apr 29 02:05:15 2023, max compression
```

## Comparing `raster-tools-0.1.6.tar` & `raster-tools-0.1.7.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-22 00:03:06.702038 raster-tools-0.1.6/
--rw-------   0 fred      (1000) fred      (1000)    35149 2022-08-26 20:44:14.000000 raster-tools-0.1.6/LICENSE
--rw-r--r--   0 fred      (1000) fred      (1000)      316 2022-08-26 20:44:14.000000 raster-tools-0.1.6/MANIFEST.in
--rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-04-22 00:03:06.702038 raster-tools-0.1.6/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)     1198 2023-04-11 21:45:35.000000 raster-tools-0.1.6/README.md
--rw-r--r--   0 fred      (1000) fred      (1000)      273 2022-08-26 20:44:14.000000 raster-tools-0.1.6/pyproject.toml
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-22 00:03:06.698038 raster-tools-0.1.6/raster_tools/
--rw-rw-r--   0 fred      (1000) fred      (1000)      934 2023-01-25 21:30:15.000000 raster-tools-0.1.6/raster_tools/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)      383 2023-01-28 03:26:22.000000 raster-tools-0.1.6/raster_tools/_compat.py
--rw-rw-r--   0 fred      (1000) fred      (1000)       22 2023-04-22 00:02:29.000000 raster-tools-0.1.6/raster_tools/_version.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     7664 2023-01-04 22:54:45.000000 raster-tools-0.1.6/raster_tools/batch.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     6536 2023-02-01 01:11:45.000000 raster-tools-0.1.6/raster_tools/clipping.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     9647 2023-03-29 17:25:11.000000 raster-tools-0.1.6/raster_tools/creation.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1286 2022-11-29 01:39:49.000000 raster-tools-0.1.6/raster_tools/dask_utils.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-22 00:03:06.698038 raster-tools-0.1.6/raster_tools/distance/
--rw-r--r--   0 fred      (1000) fred      (1000)      427 2022-08-26 20:44:16.000000 raster-tools-0.1.6/raster_tools/distance/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     6777 2022-10-21 23:01:50.000000 raster-tools-0.1.6/raster_tools/distance/_heap.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    26495 2023-01-04 22:54:45.000000 raster-tools-0.1.6/raster_tools/distance/cost_distance.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    34940 2023-04-13 22:25:41.000000 raster-tools-0.1.6/raster_tools/distance/proximity.py
--rw-r--r--   0 fred      (1000) fred      (1000)     3240 2022-12-09 03:28:15.000000 raster-tools-0.1.6/raster_tools/dtypes.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    21032 2023-04-21 22:57:28.000000 raster-tools-0.1.6/raster_tools/focal.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    35299 2023-04-22 00:02:50.000000 raster-tools-0.1.6/raster_tools/general.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     7149 2023-01-04 22:54:45.000000 raster-tools-0.1.6/raster_tools/io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    12275 2023-02-15 02:21:21.000000 raster-tools-0.1.6/raster_tools/line_stats.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2123 2022-10-22 00:44:28.000000 raster-tools-0.1.6/raster_tools/masking.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    47679 2023-04-22 00:02:50.000000 raster-tools-0.1.6/raster_tools/raster.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4076 2022-10-21 23:01:50.000000 raster-tools-0.1.6/raster_tools/stat_common.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    17964 2023-03-31 23:07:40.000000 raster-tools-0.1.6/raster_tools/surface.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3170 2023-04-18 19:26:49.000000 raster-tools-0.1.6/raster_tools/utils.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    30306 2023-04-22 00:02:50.000000 raster-tools-0.1.6/raster_tools/vector.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    20196 2023-04-06 21:19:23.000000 raster-tools-0.1.6/raster_tools/zonal.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-22 00:03:06.698038 raster-tools-0.1.6/raster_tools.egg-info/
--rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-04-22 00:03:06.000000 raster-tools-0.1.6/raster_tools.egg-info/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)     1774 2023-04-22 00:03:06.000000 raster-tools-0.1.6/raster_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)        1 2023-04-22 00:03:06.000000 raster-tools-0.1.6/raster_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-04-22 00:03:06.000000 raster-tools-0.1.6/raster_tools.egg-info/requires.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       13 2023-04-22 00:03:06.000000 raster-tools-0.1.6/raster_tools.egg-info/top_level.txt
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-22 00:03:06.698038 raster-tools-0.1.6/requirements/
--rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-01-25 21:30:15.000000 raster-tools-0.1.6/requirements/default.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       38 2023-04-22 00:03:06.702038 raster-tools-0.1.6/setup.cfg
--rw-rw-r--   0 fred      (1000) fred      (1000)     1526 2023-01-31 00:50:40.000000 raster-tools-0.1.6/setup.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-22 00:03:06.702038 raster-tools-0.1.6/tests/
--rw-rw-r--   0 fred      (1000) fred      (1000)     4072 2023-01-04 22:54:46.000000 raster-tools-0.1.6/tests/test_clipping.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     7404 2023-01-04 22:54:46.000000 raster-tools-0.1.6/tests/test_distance.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1297 2022-08-26 20:44:16.000000 raster-tools-0.1.6/tests/test_distance__heap.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     8212 2023-04-14 00:09:55.000000 raster-tools-0.1.6/tests/test_distance_proximity.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    20233 2023-03-03 21:13:40.000000 raster-tools-0.1.6/tests/test_focal.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    24340 2023-04-21 20:48:50.000000 raster-tools-0.1.6/tests/test_general.py
--rw-r--r--   0 fred      (1000) fred      (1000)     7288 2023-01-28 03:48:27.000000 raster-tools-0.1.6/tests/test_line_stats.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    56488 2023-04-22 00:02:50.000000 raster-tools-0.1.6/tests/test_raster.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4124 2022-08-26 20:44:16.000000 raster-tools-0.1.6/tests/test_stat_common.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5157 2023-02-15 02:21:21.000000 raster-tools-0.1.6/tests/test_surface.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    10830 2023-01-25 02:09:19.000000 raster-tools-0.1.6/tests/test_vector.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     6903 2023-04-06 20:45:48.000000 raster-tools-0.1.6/tests/test_zonal.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-29 02:05:15.422075 raster-tools-0.1.7/
+-rw-------   0 fred      (1000) fred      (1000)    35149 2022-08-26 20:44:14.000000 raster-tools-0.1.7/LICENSE
+-rw-r--r--   0 fred      (1000) fred      (1000)      316 2022-08-26 20:44:14.000000 raster-tools-0.1.7/MANIFEST.in
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-04-29 02:05:15.422075 raster-tools-0.1.7/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1198 2023-04-11 21:45:35.000000 raster-tools-0.1.7/README.md
+-rw-r--r--   0 fred      (1000) fred      (1000)      273 2022-08-26 20:44:14.000000 raster-tools-0.1.7/pyproject.toml
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-29 02:05:15.418075 raster-tools-0.1.7/raster_tools/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      934 2023-01-25 21:30:15.000000 raster-tools-0.1.7/raster_tools/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)      383 2023-01-28 03:26:22.000000 raster-tools-0.1.7/raster_tools/_compat.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)       22 2023-04-29 02:04:16.000000 raster-tools-0.1.7/raster_tools/_version.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     7664 2023-01-04 22:54:45.000000 raster-tools-0.1.7/raster_tools/batch.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     6536 2023-02-01 01:11:45.000000 raster-tools-0.1.7/raster_tools/clipping.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    11725 2023-04-29 01:59:00.000000 raster-tools-0.1.7/raster_tools/creation.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1286 2022-11-29 01:39:49.000000 raster-tools-0.1.7/raster_tools/dask_utils.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-29 02:05:15.418075 raster-tools-0.1.7/raster_tools/distance/
+-rw-r--r--   0 fred      (1000) fred      (1000)      427 2022-08-26 20:44:16.000000 raster-tools-0.1.7/raster_tools/distance/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6777 2022-10-21 23:01:50.000000 raster-tools-0.1.7/raster_tools/distance/_heap.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    26495 2023-01-04 22:54:45.000000 raster-tools-0.1.7/raster_tools/distance/cost_distance.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    34940 2023-04-13 22:25:41.000000 raster-tools-0.1.7/raster_tools/distance/proximity.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     3240 2022-12-09 03:28:15.000000 raster-tools-0.1.7/raster_tools/dtypes.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    21032 2023-04-21 22:57:28.000000 raster-tools-0.1.7/raster_tools/focal.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    43049 2023-04-29 01:59:10.000000 raster-tools-0.1.7/raster_tools/general.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     7149 2023-01-04 22:54:45.000000 raster-tools-0.1.7/raster_tools/io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    12275 2023-02-15 02:21:21.000000 raster-tools-0.1.7/raster_tools/line_stats.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     2123 2022-10-22 00:44:28.000000 raster-tools-0.1.7/raster_tools/masking.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    49497 2023-04-29 02:04:35.000000 raster-tools-0.1.7/raster_tools/raster.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4076 2022-10-21 23:01:50.000000 raster-tools-0.1.7/raster_tools/stat_common.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    17964 2023-03-31 23:07:40.000000 raster-tools-0.1.7/raster_tools/surface.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3170 2023-04-26 23:51:30.000000 raster-tools-0.1.7/raster_tools/utils.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    32323 2023-04-29 02:04:35.000000 raster-tools-0.1.7/raster_tools/vector.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    20962 2023-04-29 01:59:10.000000 raster-tools-0.1.7/raster_tools/zonal.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-29 02:05:15.422075 raster-tools-0.1.7/raster_tools.egg-info/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-04-29 02:05:15.000000 raster-tools-0.1.7/raster_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1797 2023-04-29 02:05:15.000000 raster-tools-0.1.7/raster_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)        1 2023-04-29 02:05:15.000000 raster-tools-0.1.7/raster_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-04-29 02:05:15.000000 raster-tools-0.1.7/raster_tools.egg-info/requires.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)       13 2023-04-29 02:05:15.000000 raster-tools-0.1.7/raster_tools.egg-info/top_level.txt
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-29 02:05:15.422075 raster-tools-0.1.7/requirements/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-01-25 21:30:15.000000 raster-tools-0.1.7/requirements/default.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)       38 2023-04-29 02:05:15.422075 raster-tools-0.1.7/setup.cfg
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1526 2023-01-31 00:50:40.000000 raster-tools-0.1.7/setup.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-29 02:05:15.422075 raster-tools-0.1.7/tests/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4072 2023-01-04 22:54:46.000000 raster-tools-0.1.7/tests/test_clipping.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4827 2023-04-29 01:59:00.000000 raster-tools-0.1.7/tests/test_creation.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     7404 2023-01-04 22:54:46.000000 raster-tools-0.1.7/tests/test_distance.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1297 2022-08-26 20:44:16.000000 raster-tools-0.1.7/tests/test_distance__heap.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     8212 2023-04-14 00:09:55.000000 raster-tools-0.1.7/tests/test_distance_proximity.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    20233 2023-03-03 21:13:40.000000 raster-tools-0.1.7/tests/test_focal.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    29890 2023-04-29 01:59:10.000000 raster-tools-0.1.7/tests/test_general.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7288 2023-01-28 03:48:27.000000 raster-tools-0.1.7/tests/test_line_stats.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    56751 2023-04-29 02:04:35.000000 raster-tools-0.1.7/tests/test_raster.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4124 2022-08-26 20:44:16.000000 raster-tools-0.1.7/tests/test_stat_common.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5157 2023-02-15 02:21:21.000000 raster-tools-0.1.7/tests/test_surface.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    10830 2023-01-25 02:09:19.000000 raster-tools-0.1.7/tests/test_vector.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     6903 2023-04-06 20:45:48.000000 raster-tools-0.1.7/tests/test_zonal.py
```

### Comparing `raster-tools-0.1.6/LICENSE` & `raster-tools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/PKG-INFO` & `raster-tools-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster-tools
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tools for processing geospatial data
 Home-page: https://github.com/UM-RMRS/raster_tools
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/UM-RMRS/raster_tools/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `raster-tools-0.1.6/README.md` & `raster-tools-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/raster_tools/__init__.py` & `raster-tools-0.1.7/raster_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/raster_tools/batch.py` & `raster-tools-0.1.7/raster_tools/batch.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/raster_tools/clipping.py` & `raster-tools-0.1.7/raster_tools/clipping.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/raster_tools/creation.py` & `raster-tools-0.1.7/raster_tools/creation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections.abc import Sequence
 
 import dask.array as da
 import numpy as np
 import xarray as xr
 
 from raster_tools.dtypes import is_int, is_scalar
+from raster_tools.masking import get_default_null_value
 from raster_tools.raster import Raster, get_raster
 from raster_tools.utils import make_raster_ds
 
 __all__ = [
     "constant_raster",
     "empty_like",
     "full_like",
@@ -24,21 +25,51 @@
         "n",
         "normal",
         "p",
         "poisson",
         "u",
         "uniform",
         "w",
-        "webull",
+        "weibull",
     )
 )
 
 
+def _copy_mask(template, out_bands):
+    if out_bands == template.nbands:
+        return template.xmask.copy()
+    mask = template.get_bands(1).xmask
+    mask = xr.concat([mask] * out_bands, "band")
+    mask["band"] = np.arange(out_bands) + 1
+    return mask
+
+
+def _build_result(template, xdata, nbands, copy_mask, copy_nv):
+    if template._masked and copy_mask:
+        xmask = _copy_mask(template, nbands)
+        nv = (
+            template.null_value
+            if copy_nv
+            else get_default_null_value(xdata.dtype)
+        )
+        xdata = xdata.rio.write_nodata(nv)
+    else:
+        xmask = xr.zeros_like(xdata, dtype=bool)
+    ds = make_raster_ds(xdata, xmask)
+    if template.crs is not None:
+        ds = ds.rio.write_crs(template.crs)
+    return Raster(ds, _fast_path=True).burn_mask()
+
+
 def random_raster(
-    raster_template, distribution="normal", bands=1, params=(1, 0.5)
+    raster_template,
+    distribution="normal",
+    bands=1,
+    params=(1, 0.5),
+    copy_mask=False,
 ):
     """Creates a Raster of random values based on the desired distribution.
 
     This function uses dask.array.random to generate data. The default is a
     normal distribution with mean of 1 and standard deviation of 0.5.
 
     Parameters
@@ -66,14 +97,18 @@
     bands : int, optional
         Number of bands needed desired. Default is 1.
     params : list of scalars, optional
         Additional parameters for generating the distribution. For example
         `distribution='normal'` and `params=(1, 0.5)` would result in a normal
         distribution with mean of 1 and standard deviation of 0.5. Default is
         ``(1, 0.5)``.
+    copy_mask : bool
+        If `True`, the template raster's mask is copied to the result raster.
+        If `bands` differs from `raster_template`, the first band's mask is
+        copied `bands` times.
 
     Returns
     -------
     Raster
         The resulting raster of random values pulled from the distribution.
 
     """
@@ -133,31 +168,32 @@
         ndata = da.random.random(size=shape, chunks=chunks)
     # TODO: add more distributions
 
     cband = np.arange(bands) + 1
     xdata = xr.DataArray(
         ndata, coords=(cband, rst.y, rst.x), dims=("band", "y", "x")
     )
-    if rst.crs is not None:
-        xdata = xdata.rio.write_crs(rst.crs)
-    xmask = xr.zeros_like(xdata, dtype=bool)
-    return Raster(make_raster_ds(xdata, xmask), _fast_path=True)
+    return _build_result(rst, xdata, bands, copy_mask, False)
 
 
-def empty_like(raster_template, bands=1, dtype=None):
+def empty_like(raster_template, bands=1, dtype=None, copy_mask=False):
     """Create a Raster filled with uninitialized data like a template raster.
 
     Parameters
     ----------
     raster_template : Raster, str
         Template raster used to define rows, columns, crs, resolution, etc
     bands : int, optional
         Number of bands desired for output. Default is 1.
     dtype : data-type, optional
         Overrides the result dtype.
+    copy_mask : bool
+        If `True`, the template raster's mask is copied to the result raster.
+        If `bands` differs from `raster_template`, the first band's mask is
+        copied `bands` times.
 
     Returns
     -------
     Raster
         The resulting raster of uninitialized data.
 
     """
@@ -184,33 +220,35 @@
     chunks = ((1,) * bands,) + rst.data.chunks[1:]
     ndata = da.empty(shape, chunks=chunks, dtype=dtype)
     xdata = xr.DataArray(
         ndata,
         coords=(np.arange(bands) + 1, rst.y, rst.x),
         dims=("band", "y", "x"),
     )
-    if rst.crs is not None:
-        xdata = xdata.rio.write_crs(rst.crs)
-    xmask = xr.zeros_like(xdata, dtype=bool)
-    return Raster(make_raster_ds(xdata, xmask), _fast_path=True)
+    copy_null = dtype is None or np.dtype(dtype) == rst.dtype
+    return _build_result(rst, xdata, bands, copy_mask, copy_null)
 
 
-def full_like(raster_template, value, bands=1, dtype=None):
+def full_like(raster_template, value, bands=1, dtype=None, copy_mask=False):
     """Create a Raster filled with a constant value like a template raster.
 
     Parameters
     ----------
     raster_template : Raster, str
         Template raster used to define rows, columns, crs, resolution, etc
     value : scalar
         Value to fill result with.
     bands : int, optional
         Number of bands desired for output. Default is 1.
     dtype : data-type, optional
         Overrides the result dtype.
+    copy_mask : bool
+        If `True`, the template raster's mask is copied to the result raster.
+        If `bands` differs from `raster_template`, the first band's mask is
+        copied `bands` times.
 
     Returns
     -------
     Raster
         The resulting raster of constant values.
 
     """
@@ -244,76 +282,90 @@
     chunks = ((1,) * bands,) + rst.data.chunks[1:]
     ndata = da.full(shape, value, chunks=chunks, dtype=dtype)
     xdata = xr.DataArray(
         ndata,
         coords=(np.arange(bands) + 1, rst.y, rst.x),
         dims=("band", "y", "x"),
     )
-    if rst.crs is not None:
-        xdata = xdata.rio.write_crs(rst.crs)
-    xmask = xr.zeros_like(xdata, dtype=bool)
-    return Raster(make_raster_ds(xdata, xmask), _fast_path=True)
+    copy_null = dtype is None or np.dtype(dtype) == rst.dtype
+    return _build_result(rst, xdata, bands, copy_mask, copy_null)
 
 
-def constant_raster(raster_template, value=1, bands=1):
+def constant_raster(raster_template, value=1, bands=1, copy_mask=False):
     """Create a Raster filled with a constant value like a template raster.
 
     This is a convenience function that wraps :func:`full_like`.
 
     Parameters
     ----------
     raster_template : Raster, str
         Template raster used to define rows, columns, crs, resolution, etc
     value : scalar, optional
         Value to fill result with. Default is 1.
     bands : int, optional
         Number of bands desired for output. Default is 1.
+    copy_mask : bool
+        If `True`, the template raster's mask is copied to the result raster.
+        If `bands` differs from `raster_template`, the first band's mask is
+        copied `bands` times.
 
     Returns
     -------
     Raster
         The resulting raster of constant values.
 
     """
-    return full_like(raster_template, value, bands=bands)
+    return full_like(raster_template, value, bands=bands, copy_mask=copy_mask)
 
 
-def zeros_like(raster_template, bands=1, dtype=None):
+def zeros_like(raster_template, bands=1, dtype=None, copy_mask=False):
     """Create a Raster filled with zeros like a template raster.
 
     Parameters
     ----------
     raster_template : Raster, str
         Template raster used to define rows, columns, crs, resolution, etc
     bands : int, optional
         Number of bands desired for output. Default is 1.
     dtype : data-type, optional
         Overrides the result dtype.
+    copy_mask : bool
+        If `True`, the template raster's mask is copied to the result raster.
+        If `bands` differs from `raster_template`, the first band's mask is
+        copied `bands` times.
 
     Returns
     -------
     Raster
         The resulting raster of zreos.
 
     """
-    return full_like(raster_template, 0, bands=bands, dtype=dtype)
+    return full_like(
+        raster_template, 0, bands=bands, dtype=dtype, copy_mask=copy_mask
+    )
 
 
-def ones_like(raster_template, bands=1, dtype=None):
+def ones_like(raster_template, bands=1, dtype=None, copy_mask=False):
     """Create a Raster filled with ones like a template raster.
 
     Parameters
     ----------
     raster_template : Raster, str
         Template raster used to define rows, columns, crs, resolution, etc
     bands : int, optional
         Number of bands desired for output. Default is 1.
     dtype : data-type, optional
         Overrides the result dtype.
+    copy_mask : bool
+        If `True`, the template raster's mask is copied to the result raster.
+        If `bands` differs from `raster_template`, the first band's mask is
+        copied `bands` times.
 
     Returns
     -------
     Raster
         The resulting raster of ones.
 
     """
-    return full_like(raster_template, 1, bands=bands, dtype=dtype)
+    return full_like(
+        raster_template, 1, bands=bands, dtype=dtype, copy_mask=copy_mask
+    )
```

### Comparing `raster-tools-0.1.6/raster_tools/dask_utils.py` & `raster-tools-0.1.7/raster_tools/dask_utils.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/raster_tools/distance/_heap.py` & `raster-tools-0.1.7/raster_tools/distance/_heap.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/raster_tools/distance/cost_distance.py` & `raster-tools-0.1.7/raster_tools/distance/cost_distance.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/raster_tools/distance/proximity.py` & `raster-tools-0.1.7/raster_tools/distance/proximity.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/raster_tools/dtypes.py` & `raster-tools-0.1.7/raster_tools/dtypes.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/raster_tools/focal.py` & `raster-tools-0.1.7/raster_tools/focal.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/raster_tools/general.py` & `raster-tools-0.1.7/raster_tools/general.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import re
 from collections.abc import Iterable, Sequence
 from functools import partial
 
 import dask.array as da
 import numba as nb
 import numpy as np
+import pandas as pd
 import xarray as xr
 from dask_image import ndmeasure as ndm
 from scipy.ndimage import (
     binary_dilation,
     binary_erosion,
     grey_dilation,
     grey_erosion,
@@ -57,20 +58,22 @@
     nanasm_jit,
     nanentropy_jit,
     nanmode_jit,
 )
 from raster_tools.utils import make_raster_ds
 
 __all__ = [
+    "ModelPredictAdaptor",
     "aggregate",
     "band_concat",
     "dilate",
     "erode",
     "local_stats",
-    "predict_model",
+    "model_predict_vector",
+    "model_predict_raster",
     "reclassify",
     "regions",
     "remap_range",
 ]
 
 # TODO: mosaic
 
@@ -152,19 +155,19 @@
     if raster._masked:
         # Set null values to 0 to skip them in the labeling phase
         data = da.where(raster._ds.mask.data, 0, data)
 
     for bnd in range(data.shape[0]):
         dout[bnd] = _create_labels(data[bnd], wd, unique_values)
 
+    nv = reconcile_nullvalue_with_dtype(raster.null_value, rs_out.dtype)
     if raster._masked:
-        nv = reconcile_nullvalue_with_dtype(raster.null_value, rs_out.dtype)
         dout = da.where(raster._ds.mask.data, nv, dout)
     rs_out._ds.raster.data = dout
-    return rs_out
+    return rs_out.set_null_value(nv)
 
 
 @nb.jit(nopython=True, nogil=True, parallel=True)
 def _coarsen_chunk(x, axis, func, out_dtype, check_nan):
     dims = sorted(set(range(len(x.shape))) - set(axis))
     shape = (x.shape[dims[0]], x.shape[dims[1]], x.shape[dims[2]])
     out = np.empty(shape, out_dtype)
@@ -327,46 +330,271 @@
     else:
         ds_out["mask"] = xr.zeros_like(rs.get_bands(1).xmask)
     if rs.crs is not None:
         ds_out = ds_out.rio.write_crs(rs.crs)
     return Raster(ds_out, _fast_path=True)
 
 
-def predict_model(raster, model):
+class ModelPredictAdaptor:
     """
-    Predict cell estimates from a model using raster band values as predictors.
+    An adaptor class that allows models without a `predict` method to be used
+    with :func:`model_predict_raster` and :func:`model_predict_vector`.
 
-    Predictor bands correspond to the order of the predictor variables within
-    the model. Outputs are raster surfaces with bands cell values depending on
-    the type of model.
+    Examples
+    --------
+    For a model function:
+
+    >>> def my_model_func(x):
+    ...     return np.sin(x) + np.cos(x)
+    >>> model = ModelPredictAdaptor(my_model_func)
+    >>> result_raster = rts.general.model_predict_raster(
+    ...         predictors, model, n_outputs=predictors.nbands
+    ... )
+
+    For a model function lacking a `predict` method:
+
+    >>> class MyModel:
+    ...     # ...
+    ...     def transform(x):
+    ...         # ...
+    ...         return result
+    >>> model = ModelPredictAdaptor(MyModel(), "transform")
+    >>> result_raster = rts.general.model_predict_raster(predictors, model)
+
+    """
+
+    def __init__(self, model, method=None):
+        """
+        Constructs an adaptor.
+
+        Parameters
+        ----------
+        model : callable, object
+            The model function or object. The `method` parameter determines
+            how this object is handled.
+        method : None, str, callable, optional
+            Determines how input data is provided to `model`. If ``None``,
+            `model` is called with the data as the argument, e.g. `model(x)`.
+            If a string, the adaptor passes input data to the method on `model`
+            with the same name, e.g. for `method="my_func"`,
+            `model.my_func(x)` is called.
+
+        """
+        if method is None:
+
+            def func(x):
+                return model(x)
+
+            self.method = func
+        elif isinstance(method, str):
+            if not hasattr(model, method):
+                raise AttributeError(
+                    f"The given model object has no attribute '{method}'"
+                )
+
+            def func(x):
+                return getattr(model, method)(x)
+
+            self.method = func
+        else:
+            raise ValueError(
+                "Could not understand the method argument. method must be "
+                "None or a string."
+            )
+
+    def predict(self, x):
+        """Pass the input data to the wrapped model and produce the results"""
+        return self.method(x)
+
+
+def _pred_raster(xarr, model, nbands):
+    b, y, x = xarr.shape
+    vl_arr = np.moveaxis(xarr, 0, -1).reshape(y * x, b)
+    pred = model.predict(np.nan_to_num(vl_arr))
+    if pred.ndim == 1:
+        pred = np.expand_dims(pred, 1)
+    return np.moveaxis(pred, -1, 0).reshape(nbands, y, x)
 
-    The function uses the `model` class' predict method to estimate a new
-    raster surface.
+
+def model_predict_raster(raster, model, n_outputs=1):
+    """
+    Generate a new raster using the provided model to predict new values.
+
+    The raster's values are used as the predictor inputs for `model`. Each band
+    in the input raster is used as a separate input variable. Outputs are
+    raster surfaces where each band corresponds to a variable output by
+    `model`.
+
+    The `model` argument must provide a `predict` method. If the desired model
+    does not provide a `predict` function, :class:`ModelPredictAdaptor` can be
+    used to wrap it and make it compatible with this function.
 
     Parameters
     ----------
-    raster : Raster or path str
-        Raster of predictor variables where the bands correspond to variables
-        in the model (one band for each variable in the model).
     model : object
-        The model used to estimate new values. Must have a `predict` method
-        that takes an `xarray.DataArray` object. The provided DataArray will
-        have null cells marked with ``NaN``.
+        The model used to estimate new values. It must have a `predict` method
+        that takes an array-like object of shape `(N, M)`, where `N` is the
+        number of samples and `M` is the number of features/predictor
+        variables. The `predict` method should return an `(N, [n_outputs])`
+        shape result. If only one variable is resurned, then the `n_outputs`
+        dimension is optional.
+    n_outputs : int, optional
+        The number of output variables from the model. Each output variable
+        produced by the model is converted to a band in the output raster. The
+        default is ``1``.
 
     Returns
     -------
     Raster
-        The resulting raster of estmated values.
+        The resulting raster of estimated values. Each band corresponds to an
+        output variable produced by `model`.
 
     """
-    rs = get_raster(raster, null_to_nan=True)
-    xarr = rs.xdata
-    xarrout = model.predict(xarr)
+    in_raster = get_raster(raster, null_to_nan=True)
+    n_outputs = int(n_outputs)
+    if n_outputs < 1:
+        raise ValueError("n_outputs must be greater than 0")
+    in_chunks = in_raster.xdata.chunksizes
+    nbands = in_raster.nbands
+
+    data = in_raster.data.rechunk(chunks=(nbands, "auto", "auto"))
+    interim_chunks = data.chunks
+
+    data = data.map_blocks(
+        _pred_raster,
+        model=model,
+        nbands=n_outputs,
+        chunks=(n_outputs, interim_chunks[1], interim_chunks[2]),
+        meta=np.array((), dtype=F64),
+        dtype=F64,
+    ).rechunk((1, in_chunks["y"], in_chunks["x"]))
+    xdata = xr.DataArray(
+        data,
+        coords={
+            "band": np.arange(n_outputs) + 1,
+            "y": in_raster.y,
+            "x": in_raster.x,
+        },
+    )
+    if in_raster._masked:
+        xmask = in_raster.xmask.any(dim="band", keepdims=True)
+        if n_outputs > 1:
+            xmask = xr.concat([xmask] * n_outputs, "band")
+        xdata = xdata.rio.write_nodata(get_default_null_value(xdata.dtype))
+    else:
+        xmask = xr.zeros_like(xdata, dtype=bool)
+    ds = make_raster_ds(xdata, xmask)
+    if in_raster.crs is not None:
+        ds = ds.rio.write_crs(in_raster.crs)
+    return Raster(ds, _fast_path=True).burn_mask()
+
+
+def _pred_df(df, model, columns, n_outputs, prefix):
+    X = df[columns].values
+    valid_mask = ~np.isnan(X).any(axis=1)
+
+    y = model.predict(X[valid_mask])
+    if y.ndim == 1:
+        y = np.expand_dims(y, 1)
+    pred = np.empty((len(df), n_outputs), dtype=F64)
+    pred[valid_mask] = y
+    pred[~valid_mask] = np.nan
+
+    dic = {}
+    if pred.shape[1] > 1:
+        for i in range(pred.shape[1]):
+            dic[f"{prefix}{i + 1}"] = pred[:, i]
+    else:
+        dic[f"{prefix}{1}"] = pred.squeeze()
+    df2 = pd.DataFrame(dic, index=df.index)
+    return pd.concat([df, df2], axis=1)
+
+
+def model_predict_vector(
+    features, model, fields, n_outputs=1, out_prefix="pred_"
+):
+    """Predict new columns using a model.
+
+    `features`' values are used as predictors for the model to produce new
+    predictions. The resulting predictions are used to create a new vector with
+    the results appended as new columns.
+
+    The `model` argument must provide a `predict` method. If the desired model
+    does not provide a `predict` function, :class:`ModelPredictAdaptor` can be
+    used to wrap it and make it compatible with this function. information.
+
+    Parameters
+    ----------
+    features : vector or path str
+        Vector with attribute columns.
+    model : object
+        The model used to estimate new values. It must have a `predict` method
+        that takes an array-like object of shape `(N, M)`, where `N` is the
+        number of samples and `M` is the number of features/predictor
+        variables. The `predict` method should return an `(N, [n_outputs])`
+        shape result. If only one variable is resurned, then the `n_outputs`
+        dimension is optional.
+    fields : list of str
+        The names of columns used in the model
+    n_outputs : int, optional
+        The number of output variables from the model. Each output variable
+        produced by the model is converted to a band in the output raster. The
+        default is ``1``.
+    out_prefix : str, optional
+        The prefix to use when naming the resulting column(s). The prefix will
+        be combined with the 1-based number of the output variable. The Default
+        is `"pred_"`.
 
-    return Raster(xarrout)
+    Returns
+    -------
+    Vector
+        The resulting vector with estimated values appended as a columns
+        (pred_1, pred_2, pred_3 ...).
+
+    """
+    from raster_tools.vector import get_vector
+
+    vc = get_vector(features).copy()
+    df = vc._geo
+    fields = list(fields)
+    for field in fields:
+        if field not in df:
+            raise KeyError(f"Invalid field name: '{field}'")
+    n_outputs = int(n_outputs)
+    if n_outputs < 1:
+        raise ValueError("n_outputs must be greater than 0")
+    if not isinstance(out_prefix, str):
+        raise TypeError("out_prefix must be a string")
+    for i in range(n_outputs):
+        i += 1
+        c = f"{out_prefix}{i}"
+        if c in df:
+            raise KeyError(
+                "out_prefix produced a column name that is already present in "
+                "the feature: '{c}'."
+            )
+
+    meta = df._meta.copy()
+    new_meta_cols = pd.DataFrame(
+        {
+            f"{out_prefix}{i + 1}": np.array([], dtype=F64)
+            for i in range(n_outputs)
+        }
+    )
+    meta = pd.concat([df._meta, new_meta_cols], axis=1)
+    print(meta.dtypes)
+    vc._geo = df.map_partitions(
+        _pred_df,
+        model=model,
+        columns=fields,
+        n_outputs=n_outputs,
+        prefix=out_prefix,
+        meta=meta,
+    )
+    return vc
 
 
 @nb.jit(nopython=True, nogil=True)
 def _local_chunk(x, func, out):
     dshape = x.shape
     rws = dshape[1]
     clms = dshape[2]
@@ -934,15 +1162,14 @@
         xcondition = xcondition > 0
 
     out_xrs = xr.where(xcondition, xtrue, xfalse)
     if masked and not scalar_and_nan:
         xtrue_mask, xfalse_mask = [
             r.xmask
             if isinstance(r, Raster)
-            # else condition.xmask
             else xr.DataArray(
                 create_null_mask(condition.xdata, None),
                 dims=condition.xdata.dims,
                 coords=condition.xdata.coords,
             )
             for r in args
         ]
```

### Comparing `raster-tools-0.1.6/raster_tools/io.py` & `raster-tools-0.1.7/raster_tools/io.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/raster_tools/line_stats.py` & `raster-tools-0.1.7/raster_tools/line_stats.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/raster_tools/masking.py` & `raster-tools-0.1.7/raster_tools/masking.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/raster_tools/raster.py` & `raster-tools-0.1.7/raster_tools/raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -679,14 +679,21 @@
         The shape will always be of the form ``(B, Y, X)`` where ``B`` is the
         band dimension, ``Y`` is the y dimension, and ``X`` is the x dimension.
 
         """
         return self._ds.raster.shape
 
     @property
+    def size(self):
+        """
+        The number of grid cells across all bands.
+        """
+        return self.data.size
+
+    @property
     def nbands(self):
         """The number of bands."""
         return self._ds.band.size
 
     @property
     def crs(self):
         """The raster's CRS.
@@ -1163,14 +1170,52 @@
 
         """
         # local import to avoid circular import
         from raster_tools.general import remap_range
 
         return remap_range(self, mapping, inclusivity=inclusivity)
 
+    def model_predict(self, model, n_outputs=1):
+        """
+        Generate a new raster using the provided model to predict new values.
+
+        The raster's values are used as the predictor inputs for `model`.
+        Each band in the input raster is used as a separate input variable.
+        Outputs are raster surfaces where each band corresponds to a variable
+        output by `model`.
+
+        The `model` argument must provide a `predict` method. If the desired
+        model does not provide a `predict` function,
+        :class:`ModelPredictAdaptor` can be used to wrap it and make it
+        compatible with this function.
+
+        Parameters
+        ----------
+        model : object
+            The model used to estimate new values. It must have a `predict`
+            method that takes an array-like object of shape `(N, M)`, where `N`
+            is the number of samples and `M` is the number of
+            features/predictor variables. The `predict` method should return an
+            `(N, [n_outputs])` shape result. If only one variable is resurned,
+            then the `n_outputs` dimension is optional.
+        n_outputs : int, optional
+            The number of output variables from the model. Each output variable
+            produced by the model is converted to a band in output raster. The
+            default is ``1``.
+
+        Returns
+        -------
+        Raster
+            The resulting raster of estimated values. Each band corresponds to
+            an output variable produced by the `model`.
+        """
+        from raster_tools.general import model_predict_raster
+
+        return model_predict_raster(self, model, n_outputs)
+
     def reclassify(self, remapping, unmapped_to_null=False):
         """Reclassify raster values based on a mapping.
 
         The raster must have an integer type.
 
         Parameters
         ----------
@@ -1369,15 +1414,15 @@
             )
             ds = make_raster_ds(xdata_quad, xmask_quad)
             if self.crs is not None:
                 ds = ds.rio.write_crs(self.crs)
             results.append(Raster(ds, _fast_path=True))
         return RasterQuadrantsResult(*results)
 
-    def chunk_geometries(self):
+    def get_chunk_geometries(self):
         _, ychunks, xchunks = self.data.chunks
         i = 0
         j = 0
         chunk_boxes = []
         rows = []
         cols = []
         for row, yc in enumerate(ychunks):
```

### Comparing `raster-tools-0.1.6/raster_tools/stat_common.py` & `raster-tools-0.1.7/raster_tools/stat_common.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/raster_tools/surface.py` & `raster-tools-0.1.7/raster_tools/surface.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/raster_tools/utils.py` & `raster-tools-0.1.7/raster_tools/utils.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/raster_tools/vector.py` & `raster-tools-0.1.7/raster_tools/vector.py`

 * *Files 4% similar despite different names*

```diff
@@ -963,7 +963,52 @@
         Vector
             Returns a new vector pointing to the saved location.
 
         """
         (geo,) = dask.compute(self._geo)
         geo.to_file(path, **fiona_kwargs)
         return open_vectors(path)
+
+    def model_predict(self, model, fields, n_outputs=1, out_prefix="pred_"):
+        """Predict new columns using a model.
+
+        `layer`'s values are used as predictors for the model to produce new
+        predictions. The resulting predictions are used to create a new vector
+        with the results appended as new columns.
+
+        The `model` argument must provide a `predict` method. If the desired
+        model does not provide a `predict` function,
+        :class:`ModelPredictAdaptor` can be used to wrap it and make it
+        compatible with this function. information.
+
+        Parameters
+        ----------
+        layer : vector or path str
+            Vector with attribute columns.
+        model : object
+            The model used to estimate new values. It must have a `predict`
+            method that takes an array-like object of shape `(N, M)`, where `N`
+            is the number of samples and `M` is the number of
+            features/predictor variables. The `predict` method should return an
+            `(N, [n_outputs])` shape result. If only one variable is resurned,
+            then the `n_outputs` dimension is optional.
+        fields : list of str
+            The names of columns used in the model
+        n_outputs : int, optional
+            The number of output variables from the model. Each output variable
+            produced by the model is converted to a band in the output raster.
+            The default is ``1``.
+        out_prefix : str, optional
+            The prefix to use when naming the resulting column(s). The prefix
+            will be combined with the 1-based number of the output variable.
+            The Default is `"pred_"`.
+
+        Returns
+        -------
+        Vector
+            The resulting vector with estimated values appended as a columns
+            (pred_1, pred_2, pred_3 ...).
+
+        """
+        from raster_tools.general import model_predict_vector
+
+        return model_predict_vector(self, model, fields, n_outputs, out_prefix)
```

### Comparing `raster-tools-0.1.6/raster_tools/zonal.py` & `raster-tools-0.1.7/raster_tools/zonal.py`

 * *Files 2% similar despite different names*

```diff
@@ -513,15 +513,15 @@
         exmask[valid_mask] = mask.vindex[i, r[valid_mask], c[valid_mask]]
         extracted[exmask] = np.nan
         out[i + 1]["extracted"] = extracted
     return out
 
 
 def extract_points_eager(
-    points, raster, column_name="extracted", skip_validation=True
+    points, raster, column_name="extracted", skip_validation=True, axis=0
 ):
     """Extract the raster cell values using point features
 
     Note
     ----
     This function is partially eager. The x and y values for the target points
     are computed. The result is still a lazy dask DataFrame.
@@ -541,23 +541,31 @@
     column_name : str, optional
         The column name to use for the extracted data points. Default is
         `"extracted"`.
     skip_validation : bool, optional
         If `True`, the input `points` is not validated to make sure that all
         features are points. This prevents partially computing the data.
         Default is `True`.
+    axis : int, optional
+        If 0 band column and values will be appended to a dataframe. Otherwise
+        band values will be append to the columns named after the prefix and
+        band of a dataframe
 
     Returns
     -------
     dask.dataframe.DataFrame
-        The columns are "band" and `column_name. These are the band data was
-        pulled from and the extracted value, respectively. NaN values in the
-        extracted column are where there was missing data in the raster or
-        the point was outside the raster's domain.
-
+        The columns names depend on the value of axis and are based on the
+        "band" and `column_name variable. If axis = 0, the output band column
+        within the dataframe identifies the band the value was extracted from.
+        The values within the column named after the column name variable are
+        the extracted values from the given band. Otherwise, the column names
+        within the dataframe are appended to the column_name prefix and provide
+        the extracted values. NaN values in the extracted column are where
+        there was missing data in the raster or the point was outside the
+        raster's domain.
     """
     points = get_vector(points)
     raster = get_raster(raster)
 
     if not len(column_name):
         raise ValueError("column_name must not be empty")
     if (
@@ -575,24 +583,29 @@
     r, c = raster.index(*dask.compute(x, y))
     nb, nr, nc = raster.shape
     valid = (r >= 0) & (r < nr) & (c >= 0) & (c < nc)
     n = len(valid)
     dfs = []
     for i in range(nb):
         bnd = i + 1
-        index = _create_dask_range_index(n * i, n * bnd)
-        df = (
-            da.full(n, bnd, dtype=np.min_scalar_type(nb + 1))
-            .to_dask_dataframe(index=index)
-            .to_frame("band")
-        )
         extracted = da.full(n, np.nan, dtype=F64)
         extracted[valid] = raster.data.vindex[i, r[valid], c[valid]]
         # Mask out missing points within the valid zones
         exmask = da.zeros(n, dtype=bool)
         exmask[valid] = raster.mask.vindex[i, r[valid], c[valid]]
         extracted[exmask] = np.nan
-        df[column_name] = extracted.to_dask_dataframe(index=index)
+        if axis == 0:
+            index = _create_dask_range_index(n * i, n * bnd)
+            df = (
+                da.full(n, bnd, dtype=np.min_scalar_type(nb + 1))
+                .to_dask_dataframe(index=index)
+                .to_frame("band")
+            )
+            df[column_name] = extracted.to_dask_dataframe(index=index)
+        else:
+            df = extracted.to_dask_dataframe(
+                columns=column_name + "_" + str(bnd)
+            )
         assert df.known_divisions
         dfs.append(df)
-    df = dd.concat(dfs)
+    df = dd.concat(dfs, axis=axis)
     return df
```

### Comparing `raster-tools-0.1.6/raster_tools.egg-info/PKG-INFO` & `raster-tools-0.1.7/raster_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster-tools
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tools for processing geospatial data
 Home-page: https://github.com/UM-RMRS/raster_tools
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/UM-RMRS/raster_tools/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `raster-tools-0.1.6/raster_tools.egg-info/SOURCES.txt` & `raster-tools-0.1.7/raster_tools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 raster_tools.egg-info/top_level.txt
 raster_tools/distance/__init__.py
 raster_tools/distance/_heap.py
 raster_tools/distance/cost_distance.py
 raster_tools/distance/proximity.py
 requirements/default.txt
 tests/test_clipping.py
+tests/test_creation.py
 tests/test_distance.py
 tests/test_distance__heap.py
 tests/test_distance_proximity.py
 tests/test_focal.py
 tests/test_general.py
 tests/test_line_stats.py
 tests/test_raster.py
```

### Comparing `raster-tools-0.1.6/setup.py` & `raster-tools-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/tests/test_clipping.py` & `raster-tools-0.1.7/tests/test_clipping.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/tests/test_distance.py` & `raster-tools-0.1.7/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/tests/test_distance__heap.py` & `raster-tools-0.1.7/tests/test_distance__heap.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/tests/test_distance_proximity.py` & `raster-tools-0.1.7/tests/test_distance_proximity.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/tests/test_focal.py` & `raster-tools-0.1.7/tests/test_focal.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/tests/test_general.py` & `raster-tools-0.1.7/tests/test_general.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,21 @@
+# isort: off
+# TODO(pygeos): remove this once shapely is the default backend for geopandas.
+# Force raster_tools._compat to be loaded before geopandas when running tests
+import raster_tools  # noqa: F401
+
+# isort: on
+
 import unittest
 from functools import partial
 
 import dask.array as da
+import dask_geopandas as dgpd
 import numpy as np
+import pandas as pd
 import pytest
 import xarray as xr
 from scipy.ndimage import (
     binary_dilation,
     binary_erosion,
     grey_dilation,
     grey_erosion,
@@ -20,15 +29,21 @@
     nan_unique_count_jit,
     nanargmax_jit,
     nanargmin_jit,
     nanasm_jit,
     nanentropy_jit,
     nanmode_jit,
 )
-from tests.utils import arange_nd, assert_valid_raster
+from raster_tools.vector import Vector
+from tests.utils import (
+    arange_nd,
+    arange_raster,
+    assert_rasters_similar,
+    assert_valid_raster,
+)
 
 stat_funcs = {
     "max": partial(np.nanmax, axis=0),
     "mean": partial(np.nanmean, axis=0),
     "median": partial(np.nanmedian, axis=0),
     "min": partial(np.nanmin, axis=0),
     "prod": partial(np.nanprod, axis=0),
@@ -273,14 +288,182 @@
 )
 def test_aggregate_errors(window, stat, error_type):
     rs = Raster("tests/data/raster/elevation.tif")
     with pytest.raises(error_type):
         general.aggregate(rs, window, stat)
 
 
+def mock_model_function(x):
+    return x @ np.array([1] * x.shape[-1])
+
+
+class MockModelClass:
+    def __init__(self, func):
+        self.func = func
+
+    def apply(self, x):
+        return self.func(x)
+
+
+class ModelAdaptor:
+    def __init__(self, func):
+        self.func = func
+
+    def predict(self, x):
+        return self.func(x)
+
+
+@pytest.mark.parametrize(
+    "raster,model,nout",
+    [
+        (
+            arange_raster((3, 4, 4)),
+            ModelAdaptor(lambda x: np.sum(x, axis=-1, keepdims=True)),
+            1,
+        ),
+        (
+            arange_raster((3, 4, 4)).set_null_value(0).set_crs("5070"),
+            ModelAdaptor(lambda x: np.sum(x, axis=-1, keepdims=True)),
+            1,
+        ),
+        (
+            arange_raster((3, 4, 4), dtype="int8"),
+            ModelAdaptor(np.sin),
+            3,
+        ),
+        (
+            arange_raster((2, 4, 4)).chunk((1, 2, 2)),
+            ModelAdaptor(lambda x: np.concatenate([x, x], axis=1)),
+            4,
+        ),
+        # Params to test ModelPredictAdaptor
+        (
+            arange_raster((3, 4, 4)).chunk((1, 2, 2)),
+            general.ModelPredictAdaptor(mock_model_function),
+            1,
+        ),
+        (
+            arange_raster((3, 4, 4)),
+            general.ModelPredictAdaptor(
+                MockModelClass(mock_model_function), "apply"
+            ),
+            1,
+        ),
+    ],
+)
+def test_model_predict_raster(raster, model, nout):
+    data = np.nan_to_num(raster.data.compute())
+    mask = raster.mask.any(axis=0).compute()
+    test_input = np.zeros((1, raster.nbands), dtype=data.dtype)
+    r = model.predict(test_input)
+    assert r.size == nout
+    assert r.shape == (1, nout) or r.shape == (nout,)
+    truth = np.empty((nout, *raster.shape[1:]), dtype=r.dtype)
+    for i in range(data.shape[1]):
+        for j in range(data.shape[2]):
+            truth[:, i, j] = model.predict(data[:, i, j][None])
+    if raster._masked:
+        truth[:, mask] = get_default_null_value(F64)
+
+    for result in [
+        general.model_predict_raster(raster, model, nout),
+        raster.model_predict(model, nout),
+    ]:
+        assert_valid_raster(result)
+        assert_rasters_similar(
+            raster, result, check_chunks=True, check_nbands=False
+        )
+        assert result.nbands == nout
+        assert np.allclose(result, truth)
+        assert result.dtype == F64
+        if raster._masked:
+            assert result.null_value == get_default_null_value(F64)
+        assert np.allclose(result.mask, np.stack(mask, axis=0))
+
+
+@pytest.mark.parametrize(
+    "features,model,columns,nout,prefix",
+    [
+        (
+            dgpd.read_file("tests/data/vector/pods.shp", chunksize=20),
+            ModelAdaptor(lambda x: np.sum(x, axis=-1, keepdims=True)),
+            ["Shape_Leng", "Shape_Area"],
+            1,
+            "pred_",
+        ),
+        (
+            dgpd.read_file("tests/data/vector/pods.shp", chunksize=20).where(
+                dgpd.read_file(
+                    "tests/data/vector/pods.shp", chunksize=20
+                ).Shape_Leng
+                > 7e4,
+                np.nan,
+            ),
+            ModelAdaptor(lambda x: np.sum(x, axis=-1, keepdims=True)),
+            ["Shape_Leng", "Shape_Area"],
+            1,
+            "result",
+        ),
+        (
+            dgpd.read_file("tests/data/vector/pods.shp", chunksize=20),
+            ModelAdaptor(np.sin),
+            ["Shape_Leng", "POD_Acres", "Shape_Area"],
+            3,
+            "pred_",
+        ),
+        (
+            dgpd.read_file("tests/data/vector/pods.shp", chunksize=20),
+            ModelAdaptor(lambda x: np.concatenate([x, x], axis=1)),
+            ["Shape_Leng", "Shape_Area"],
+            4,
+            "others",
+        ),
+        # Params to test ModelPredictAdaptor
+        (
+            dgpd.read_file("tests/data/vector/pods.shp", chunksize=20),
+            general.ModelPredictAdaptor(mock_model_function),
+            ["Shape_Leng", "Shape_Area"],
+            1,
+            "p",
+        ),
+        (
+            dgpd.read_file("tests/data/vector/pods.shp", chunksize=20),
+            general.ModelPredictAdaptor(
+                MockModelClass(mock_model_function), "apply"
+            ),
+            ["Shape_Leng", "Shape_Area"],
+            1,
+            "p",
+        ),
+    ],
+)
+def test_model_predict_vector(features, model, columns, nout, prefix):
+    df = features.compute()
+    new_columns = [f"{prefix}{i + 1}" for i in range(nout)]
+    data = df[columns].values
+    valid = ~np.isnan(data).any(axis=1)
+    truth = np.full((len(df), nout), np.nan, dtype=F64)
+    r = model.predict(data[valid])
+    if r.ndim == 1:
+        r = r[:, None]
+    truth[valid] = r
+    new_df = pd.DataFrame({c: t for c, t in zip(new_columns, truth.T)})
+    truth_df = pd.concat([df, new_df], axis=1)
+
+    for result in [
+        general.model_predict_vector(features, model, columns, nout, prefix),
+        Vector(features).model_predict(model, columns, nout, prefix),
+    ]:
+        assert isinstance(result, Vector)
+        for c in new_columns:
+            assert c in result._geo
+        rdf = result._geo.compute()
+        assert truth_df.equals(rdf)
+
+
 @pytest.mark.parametrize("chunk", [False, True])
 @pytest.mark.parametrize("null_value", [-99, 100, np.nan])
 @pytest.mark.parametrize(
     "size", [2, 3, 4, 5, (3, 1), (1, 4), (2, 3), (3, 3), (3, 5), (4, 6)]
 )
 @pytest.mark.parametrize("name", ["erode", "dilate"])
 def test_erode_dilate(name, size, null_value, chunk):
```

### Comparing `raster-tools-0.1.6/tests/test_line_stats.py` & `raster-tools-0.1.7/tests/test_line_stats.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/tests/test_raster.py` & `raster-tools-0.1.7/tests/test_raster.py`

 * *Files 1% similar despite different names*

```diff
@@ -520,14 +520,27 @@
     raster = Raster(path)
     xdata = riox.open_rasterio(path)
     assert hasattr(raster, "shape")
     assert isinstance(raster.shape, tuple)
     assert raster.shape == xdata.shape
 
 
+@pytest.mark.parametrize(
+    "raster",
+    [
+        band_concat(["tests/data/raster/elevation_small.tif"] * 3),
+        arange_raster((4, 20, 25)),
+    ],
+)
+def test_property_size(raster):
+    data = raster.data.compute()
+
+    assert raster.size == data.size
+
+
 def test_property_crs():
     path = "tests/data/raster/elevation_clipped_small.tif"
     raster = Raster(path)
     xdata = riox.open_rasterio(path)
     assert hasattr(raster, "crs")
     assert isinstance(raster.crs, rio.crs.CRS)
     assert raster.crs == xdata.rio.crs
```

### Comparing `raster-tools-0.1.6/tests/test_stat_common.py` & `raster-tools-0.1.7/tests/test_stat_common.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/tests/test_surface.py` & `raster-tools-0.1.7/tests/test_surface.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/tests/test_vector.py` & `raster-tools-0.1.7/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.6/tests/test_zonal.py` & `raster-tools-0.1.7/tests/test_zonal.py`

 * *Files identical despite different names*


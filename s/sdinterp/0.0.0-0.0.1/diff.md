# Comparing `tmp/sdinterp-0.0.0.tar.gz` & `tmp/sdinterp-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdinterp-0.0.0.tar", last modified: Sat Apr 29 15:22:26 2023, max compression
+gzip compressed data, was "sdinterp-0.0.1.tar", last modified: Sat Apr 29 15:36:50 2023, max compression
```

## Comparing `sdinterp-0.0.0.tar` & `sdinterp-0.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 alv.popov   (503) staff       (20)        0 2023-04-29 15:22:26.680002 sdinterp-0.0.0/
--rw-r--r--   0 alv.popov   (503) staff       (20)     1073 2023-04-29 14:56:01.000000 sdinterp-0.0.0/LICENSE
--rw-r--r--   0 alv.popov   (503) staff       (20)     2041 2023-04-29 15:22:26.678625 sdinterp-0.0.0/PKG-INFO
--rw-r--r--   0 alv.popov   (503) staff       (20)     1549 2023-04-29 14:56:01.000000 sdinterp-0.0.0/README.md
--rw-r--r--   0 alv.popov   (503) staff       (20)      719 2023-04-29 15:22:07.000000 sdinterp-0.0.0/pyproject.toml
--rw-r--r--   0 alv.popov   (503) staff       (20)       38 2023-04-29 15:22:26.680680 sdinterp-0.0.0/setup.cfg
-drwxr-xr-x   0 alv.popov   (503) staff       (20)        0 2023-04-29 15:22:26.622341 sdinterp-0.0.0/src/
-drwxr-xr-x   0 alv.popov   (503) staff       (20)        0 2023-04-29 15:22:26.628785 sdinterp-0.0.0/src/sdi/
--rw-r--r--   0 alv.popov   (503) staff       (20)        0 2023-04-29 14:56:01.000000 sdinterp-0.0.0/src/sdi/__init__.py
-drwxr-xr-x   0 alv.popov   (503) staff       (20)        0 2023-04-29 15:22:26.636977 sdinterp-0.0.0/src/sdi/interpolation/
--rw-r--r--   0 alv.popov   (503) staff       (20)       98 2023-04-29 14:56:01.000000 sdinterp-0.0.0/src/sdi/interpolation/__init__.py
--rw-r--r--   0 alv.popov   (503) staff       (20)     1837 2023-04-29 14:56:01.000000 sdinterp-0.0.0/src/sdi/interpolation/idw.py
-drwxr-xr-x   0 alv.popov   (503) staff       (20)        0 2023-04-29 15:22:26.641909 sdinterp-0.0.0/src/sdi/interpolation/kriging/
--rw-r--r--   0 alv.popov   (503) staff       (20)       91 2023-04-29 14:56:01.000000 sdinterp-0.0.0/src/sdi/interpolation/kriging/__init__.py
--rw-r--r--   0 alv.popov   (503) staff       (20)      770 2023-04-29 14:56:01.000000 sdinterp-0.0.0/src/sdi/interpolation/kriging/ordinary.py
--rw-r--r--   0 alv.popov   (503) staff       (20)      751 2023-04-29 14:56:01.000000 sdinterp-0.0.0/src/sdi/interpolation/kriging/simple.py
--rw-r--r--   0 alv.popov   (503) staff       (20)      979 2023-04-29 14:56:01.000000 sdinterp-0.0.0/src/sdi/interpolation/kriging/universal.py
--rw-r--r--   0 alv.popov   (503) staff       (20)      529 2023-04-29 14:56:01.000000 sdinterp-0.0.0/src/sdi/interpolation/linear.py
--rw-r--r--   0 alv.popov   (503) staff       (20)      546 2023-04-29 14:56:01.000000 sdinterp-0.0.0/src/sdi/interpolation/nearest.py
--rw-r--r--   0 alv.popov   (503) staff       (20)     2173 2023-04-29 14:56:01.000000 sdinterp-0.0.0/src/sdi/interpolation/rbf.py
--rw-r--r--   0 alv.popov   (503) staff       (20)      526 2023-04-29 14:56:01.000000 sdinterp-0.0.0/src/sdi/interpolator.py
-drwxr-xr-x   0 alv.popov   (503) staff       (20)        0 2023-04-29 15:22:26.649232 sdinterp-0.0.0/src/sdi/variogram/
--rw-r--r--   0 alv.popov   (503) staff       (20)       87 2023-04-29 14:56:01.000000 sdinterp-0.0.0/src/sdi/variogram/__init__.py
--rw-r--r--   0 alv.popov   (503) staff       (20)      665 2023-04-29 14:56:01.000000 sdinterp-0.0.0/src/sdi/variogram/empirical.py
--rw-r--r--   0 alv.popov   (503) staff       (20)     1855 2023-04-29 14:56:01.000000 sdinterp-0.0.0/src/sdi/variogram/models.py
-drwxr-xr-x   0 alv.popov   (503) staff       (20)        0 2023-04-29 15:22:26.669113 sdinterp-0.0.0/src/sdinterp.egg-info/
--rw-r--r--   0 alv.popov   (503) staff       (20)     2041 2023-04-29 15:22:26.000000 sdinterp-0.0.0/src/sdinterp.egg-info/PKG-INFO
--rw-r--r--   0 alv.popov   (503) staff       (20)      746 2023-04-29 15:22:26.000000 sdinterp-0.0.0/src/sdinterp.egg-info/SOURCES.txt
--rw-r--r--   0 alv.popov   (503) staff       (20)        1 2023-04-29 15:22:26.000000 sdinterp-0.0.0/src/sdinterp.egg-info/dependency_links.txt
--rw-r--r--   0 alv.popov   (503) staff       (20)       43 2023-04-29 15:22:26.000000 sdinterp-0.0.0/src/sdinterp.egg-info/requires.txt
--rw-r--r--   0 alv.popov   (503) staff       (20)        4 2023-04-29 15:22:26.000000 sdinterp-0.0.0/src/sdinterp.egg-info/top_level.txt
-drwxr-xr-x   0 alv.popov   (503) staff       (20)        0 2023-04-29 15:22:26.677025 sdinterp-0.0.0/test/
--rw-r--r--   0 alv.popov   (503) staff       (20)     2303 2023-04-29 14:56:01.000000 sdinterp-0.0.0/test/test_kriging.py
--rw-r--r--   0 alv.popov   (503) staff       (20)     2231 2023-04-29 14:56:01.000000 sdinterp-0.0.0/test/test_simple_interpolation.py
--rw-r--r--   0 alv.popov   (503) staff       (20)     1817 2023-04-29 14:56:01.000000 sdinterp-0.0.0/test/test_variogram.py
+drwxr-xr-x   0 alv.popov   (503) staff       (20)        0 2023-04-29 15:36:50.532768 sdinterp-0.0.1/
+-rw-r--r--   0 alv.popov   (503) staff       (20)     1073 2023-04-29 15:33:52.000000 sdinterp-0.0.1/LICENSE
+-rw-r--r--   0 alv.popov   (503) staff       (20)     2056 2023-04-29 15:36:50.531606 sdinterp-0.0.1/PKG-INFO
+-rw-r--r--   0 alv.popov   (503) staff       (20)     1559 2023-04-29 15:33:52.000000 sdinterp-0.0.1/README.md
+-rw-r--r--   0 alv.popov   (503) staff       (20)      724 2023-04-29 15:33:52.000000 sdinterp-0.0.1/pyproject.toml
+-rw-r--r--   0 alv.popov   (503) staff       (20)       38 2023-04-29 15:36:50.533347 sdinterp-0.0.1/setup.cfg
+drwxr-xr-x   0 alv.popov   (503) staff       (20)        0 2023-04-29 15:36:50.490084 sdinterp-0.0.1/src/
+drwxr-xr-x   0 alv.popov   (503) staff       (20)        0 2023-04-29 15:36:50.495721 sdinterp-0.0.1/src/sdinterp/
+-rw-r--r--   0 alv.popov   (503) staff       (20)        0 2023-04-29 15:33:52.000000 sdinterp-0.0.1/src/sdinterp/__init__.py
+drwxr-xr-x   0 alv.popov   (503) staff       (20)        0 2023-04-29 15:36:50.512400 sdinterp-0.0.1/src/sdinterp/interpolation/
+-rw-r--r--   0 alv.popov   (503) staff       (20)       98 2023-04-29 15:33:52.000000 sdinterp-0.0.1/src/sdinterp/interpolation/__init__.py
+-rw-r--r--   0 alv.popov   (503) staff       (20)     1842 2023-04-29 15:33:52.000000 sdinterp-0.0.1/src/sdinterp/interpolation/idw.py
+drwxr-xr-x   0 alv.popov   (503) staff       (20)        0 2023-04-29 15:36:50.518757 sdinterp-0.0.1/src/sdinterp/interpolation/kriging/
+-rw-r--r--   0 alv.popov   (503) staff       (20)       91 2023-04-29 15:33:52.000000 sdinterp-0.0.1/src/sdinterp/interpolation/kriging/__init__.py
+-rw-r--r--   0 alv.popov   (503) staff       (20)      775 2023-04-29 15:33:52.000000 sdinterp-0.0.1/src/sdinterp/interpolation/kriging/ordinary.py
+-rw-r--r--   0 alv.popov   (503) staff       (20)      756 2023-04-29 15:33:52.000000 sdinterp-0.0.1/src/sdinterp/interpolation/kriging/simple.py
+-rw-r--r--   0 alv.popov   (503) staff       (20)      984 2023-04-29 15:33:52.000000 sdinterp-0.0.1/src/sdinterp/interpolation/kriging/universal.py
+-rw-r--r--   0 alv.popov   (503) staff       (20)      534 2023-04-29 15:33:52.000000 sdinterp-0.0.1/src/sdinterp/interpolation/linear.py
+-rw-r--r--   0 alv.popov   (503) staff       (20)      551 2023-04-29 15:33:52.000000 sdinterp-0.0.1/src/sdinterp/interpolation/nearest.py
+-rw-r--r--   0 alv.popov   (503) staff       (20)     2178 2023-04-29 15:33:52.000000 sdinterp-0.0.1/src/sdinterp/interpolation/rbf.py
+-rw-r--r--   0 alv.popov   (503) staff       (20)      526 2023-04-29 15:33:52.000000 sdinterp-0.0.1/src/sdinterp/interpolator.py
+drwxr-xr-x   0 alv.popov   (503) staff       (20)        0 2023-04-29 15:36:50.523946 sdinterp-0.0.1/src/sdinterp/variogram/
+-rw-r--r--   0 alv.popov   (503) staff       (20)       87 2023-04-29 15:33:52.000000 sdinterp-0.0.1/src/sdinterp/variogram/__init__.py
+-rw-r--r--   0 alv.popov   (503) staff       (20)      665 2023-04-29 15:33:52.000000 sdinterp-0.0.1/src/sdinterp/variogram/empirical.py
+-rw-r--r--   0 alv.popov   (503) staff       (20)     1855 2023-04-29 15:33:52.000000 sdinterp-0.0.1/src/sdinterp/variogram/models.py
+drwxr-xr-x   0 alv.popov   (503) staff       (20)        0 2023-04-29 15:36:50.505703 sdinterp-0.0.1/src/sdinterp.egg-info/
+-rw-r--r--   0 alv.popov   (503) staff       (20)     2056 2023-04-29 15:36:50.000000 sdinterp-0.0.1/src/sdinterp.egg-info/PKG-INFO
+-rw-r--r--   0 alv.popov   (503) staff       (20)      816 2023-04-29 15:36:50.000000 sdinterp-0.0.1/src/sdinterp.egg-info/SOURCES.txt
+-rw-r--r--   0 alv.popov   (503) staff       (20)        1 2023-04-29 15:36:50.000000 sdinterp-0.0.1/src/sdinterp.egg-info/dependency_links.txt
+-rw-r--r--   0 alv.popov   (503) staff       (20)       43 2023-04-29 15:36:50.000000 sdinterp-0.0.1/src/sdinterp.egg-info/requires.txt
+-rw-r--r--   0 alv.popov   (503) staff       (20)        9 2023-04-29 15:36:50.000000 sdinterp-0.0.1/src/sdinterp.egg-info/top_level.txt
+drwxr-xr-x   0 alv.popov   (503) staff       (20)        0 2023-04-29 15:36:50.530027 sdinterp-0.0.1/test/
+-rw-r--r--   0 alv.popov   (503) staff       (20)     2313 2023-04-29 15:33:52.000000 sdinterp-0.0.1/test/test_kriging.py
+-rw-r--r--   0 alv.popov   (503) staff       (20)     2236 2023-04-29 15:33:52.000000 sdinterp-0.0.1/test/test_simple_interpolation.py
+-rw-r--r--   0 alv.popov   (503) staff       (20)     1822 2023-04-29 15:33:52.000000 sdinterp-0.0.1/test/test_variogram.py
```

### Comparing `sdinterp-0.0.0/LICENSE` & `sdinterp-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sdinterp-0.0.0/PKG-INFO` & `sdinterp-0.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sdinterp
-Version: 0.0.0
+Version: 0.0.1
 Summary: A package providing single interface to different interpolation methods
 Author-email: Aleksandr Popov <popov.aleksandr.v01@gmail.com>
 License: MIT
-Project-URL: Homepage, https://github.com/rytuo/sdi
+Project-URL: Homepage, https://github.com/rytuo/sdinterp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,16 +18,16 @@
 
 ## Example
 
 Regular usage of ordinary kriging method
 
 ```python
 import numpy as np
-from sdi.variogram import calc_empirical, get_cov_model, fit_cov_model
-from sdi.interpolation.kriging import Ordinary
+from sdinterp.variogram import calc_empirical, get_cov_model, fit_cov_model
+from sdinterp.interpolation.kriging import Ordinary
 
 # prepare data
 n = 100
 points = np.random.random((n, 2))
 target = np.random.random((n,))
 
 # get empirical variogram and fit model to it
```

### Comparing `sdinterp-0.0.0/README.md` & `sdinterp-0.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 ## Example
 
 Regular usage of ordinary kriging method
 
 ```python
 import numpy as np
-from sdi.variogram import calc_empirical, get_cov_model, fit_cov_model
-from sdi.interpolation.kriging import Ordinary
+from sdinterp.variogram import calc_empirical, get_cov_model, fit_cov_model
+from sdinterp.interpolation.kriging import Ordinary
 
 # prepare data
 n = 100
 points = np.random.random((n, 2))
 target = np.random.random((n,))
 
 # get empirical variogram and fit model to it
```

### Comparing `sdinterp-0.0.0/pyproject.toml` & `sdinterp-0.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sdinterp"
-version = "0.0.0"
+version = "0.0.1"
 authors = [
     { name = "Aleksandr Popov", email = "popov.aleksandr.v01@gmail.com" },
 ]
 description = "A package providing single interface to different interpolation methods"
 readme = "README.md"
 license = {text = "MIT"}
 requires-python = ">=3.9"
@@ -20,11 +20,11 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/rytuo/sdi"
+"Homepage" = "https://github.com/rytuo/sdinterp"
 
 [tool.setuptools]
 license-files = ["LICENSE"]
```

### Comparing `sdinterp-0.0.0/src/sdi/interpolation/idw.py` & `sdinterp-0.0.1/src/sdinterp/interpolation/idw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from scipy.spatial import KDTree
 
-from sdi.interpolator import Interpolator
+from sdinterp.interpolator import Interpolator
 
 
 class Idw(Interpolator):
     """
     Inverse distance weighting with modified Shepard's method.
     See https://en.wikipedia.org/wiki/Inverse_distance_weighting
```

### Comparing `sdinterp-0.0.0/src/sdi/interpolation/kriging/ordinary.py` & `sdinterp-0.0.1/src/sdinterp/interpolation/kriging/ordinary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import gstools as gs
 import numpy as np
 
-from sdi.interpolator import Interpolator
+from sdinterp.interpolator import Interpolator
 
 
 class Ordinary(Interpolator):
     """
     Ordinary kriging.
     Ordinary kriging is used to interpolate data and estimate a proper mean.
     See `gstools.krige.methods.Ordinary`
```

### Comparing `sdinterp-0.0.0/src/sdi/interpolation/kriging/simple.py` & `sdinterp-0.0.1/src/sdinterp/interpolation/kriging/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import gstools as gs
 import numpy as np
 
-from sdi.interpolator import Interpolator
+from sdinterp.interpolator import Interpolator
 
 
 class Simple(Interpolator):
     """
     Simple kriging.
     Simple kriging is used to interpolate data with a given mean.
     See `gstools.krige.methods.Simple`
```

### Comparing `sdinterp-0.0.0/src/sdi/interpolation/kriging/universal.py` & `sdinterp-0.0.1/src/sdinterp/interpolation/kriging/universal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import gstools as gs
 import numpy as np
 
-from sdi.interpolator import Interpolator
+from sdinterp.interpolator import Interpolator
 
 
 class Universal(Interpolator):
     """
     Universal kriging.
     Universal kriging is used to interpolate given data with a variable mean, that is determined by a functional drift.
     See `gstools.krige.methods.Universal`
```

### Comparing `sdinterp-0.0.0/src/sdi/interpolation/linear.py` & `sdinterp-0.0.1/src/sdinterp/interpolation/linear.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from scipy.interpolate import LinearNDInterpolator
 
-from sdi.interpolator import Interpolator
+from sdinterp.interpolator import Interpolator
 
 
 class Linear(Interpolator):
     """
     Linear interpolation.
     See `scipy.interpolate.interpnd.LinearNDInterpolator`
```

### Comparing `sdinterp-0.0.0/src/sdi/interpolation/nearest.py` & `sdinterp-0.0.1/src/sdinterp/interpolation/nearest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from scipy.interpolate import NearestNDInterpolator
 
-from sdi.interpolator import Interpolator
+from sdinterp.interpolator import Interpolator
 
 
 class Nearest(Interpolator):
     """
     Nearest-neighbor interpolation.
     See `scipy.interpolate._ndgriddata.NearestNDInterpolator`
```

### Comparing `sdinterp-0.0.0/src/sdi/interpolation/rbf.py` & `sdinterp-0.0.1/src/sdinterp/interpolation/rbf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from scipy.interpolate import RBFInterpolator
 
-from sdi.interpolator import Interpolator
+from sdinterp.interpolator import Interpolator
 
 
 class Rbf(Interpolator):
     """
     Radial basis function interpolation.
     See `scipy.interpolate._rbfinterp.RBFInterpolator`
```

### Comparing `sdinterp-0.0.0/src/sdi/interpolator.py` & `sdinterp-0.0.1/src/sdinterp/interpolator.py`

 * *Files identical despite different names*

### Comparing `sdinterp-0.0.0/src/sdi/variogram/empirical.py` & `sdinterp-0.0.1/src/sdinterp/variogram/empirical.py`

 * *Files identical despite different names*

### Comparing `sdinterp-0.0.0/src/sdi/variogram/models.py` & `sdinterp-0.0.1/src/sdinterp/variogram/models.py`

 * *Files identical despite different names*

### Comparing `sdinterp-0.0.0/src/sdinterp.egg-info/PKG-INFO` & `sdinterp-0.0.1/src/sdinterp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sdinterp
-Version: 0.0.0
+Version: 0.0.1
 Summary: A package providing single interface to different interpolation methods
 Author-email: Aleksandr Popov <popov.aleksandr.v01@gmail.com>
 License: MIT
-Project-URL: Homepage, https://github.com/rytuo/sdi
+Project-URL: Homepage, https://github.com/rytuo/sdinterp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,16 +18,16 @@
 
 ## Example
 
 Regular usage of ordinary kriging method
 
 ```python
 import numpy as np
-from sdi.variogram import calc_empirical, get_cov_model, fit_cov_model
-from sdi.interpolation.kriging import Ordinary
+from sdinterp.variogram import calc_empirical, get_cov_model, fit_cov_model
+from sdinterp.interpolation.kriging import Ordinary
 
 # prepare data
 n = 100
 points = np.random.random((n, 2))
 target = np.random.random((n,))
 
 # get empirical variogram and fit model to it
```

### Comparing `sdinterp-0.0.0/src/sdinterp.egg-info/SOURCES.txt` & `sdinterp-0.0.1/src/sdinterp.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 LICENSE
 README.md
 pyproject.toml
-src/sdi/__init__.py
-src/sdi/interpolator.py
-src/sdi/interpolation/__init__.py
-src/sdi/interpolation/idw.py
-src/sdi/interpolation/linear.py
-src/sdi/interpolation/nearest.py
-src/sdi/interpolation/rbf.py
-src/sdi/interpolation/kriging/__init__.py
-src/sdi/interpolation/kriging/ordinary.py
-src/sdi/interpolation/kriging/simple.py
-src/sdi/interpolation/kriging/universal.py
-src/sdi/variogram/__init__.py
-src/sdi/variogram/empirical.py
-src/sdi/variogram/models.py
+src/sdinterp/__init__.py
+src/sdinterp/interpolator.py
 src/sdinterp.egg-info/PKG-INFO
 src/sdinterp.egg-info/SOURCES.txt
 src/sdinterp.egg-info/dependency_links.txt
 src/sdinterp.egg-info/requires.txt
 src/sdinterp.egg-info/top_level.txt
+src/sdinterp/interpolation/__init__.py
+src/sdinterp/interpolation/idw.py
+src/sdinterp/interpolation/linear.py
+src/sdinterp/interpolation/nearest.py
+src/sdinterp/interpolation/rbf.py
+src/sdinterp/interpolation/kriging/__init__.py
+src/sdinterp/interpolation/kriging/ordinary.py
+src/sdinterp/interpolation/kriging/simple.py
+src/sdinterp/interpolation/kriging/universal.py
+src/sdinterp/variogram/__init__.py
+src/sdinterp/variogram/empirical.py
+src/sdinterp/variogram/models.py
 test/test_kriging.py
 test/test_simple_interpolation.py
 test/test_variogram.py
```

### Comparing `sdinterp-0.0.0/test/test_kriging.py` & `sdinterp-0.0.1/test/test_kriging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
-from sdi.interpolation.kriging import Simple, Ordinary, Universal
+from sdinterp.interpolation.kriging import Simple, Ordinary, Universal
 
-from sdi.variogram import calc_empirical, get_cov_model, fit_cov_model
+from sdinterp.variogram import calc_empirical, get_cov_model, fit_cov_model
 
 
 def test_simple_kriging():
     x, y = np.meshgrid(np.linspace(-100, 100, 10), np.linspace(-100, 100, 10), indexing='ij')
     x, y = x.flatten(), y.flatten()
     points = np.stack((x, y), axis=1)
     target = np.linspace(-100, 0, len(points))
```

### Comparing `sdinterp-0.0.0/test/test_simple_interpolation.py` & `sdinterp-0.0.1/test/test_simple_interpolation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from sdi.interpolation import Idw, Linear, Nearest, Rbf
+from sdinterp.interpolation import Idw, Linear, Nearest, Rbf
 
 
 def test_idw():
     x, y = np.meshgrid(np.linspace(-100, 100, 100), np.linspace(-100, 100, 100), indexing='ij')
     x, y = x.flatten(), y.flatten()
     points = np.stack((x, y), axis=1)
     target = np.linspace(-100, 0, len(points))
```

### Comparing `sdinterp-0.0.0/test/test_variogram.py` & `sdinterp-0.0.1/test/test_variogram.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import pytest
 
-from sdi.variogram import calc_empirical, get_cov_model, fit_cov_model
+from sdinterp.variogram import calc_empirical, get_cov_model, fit_cov_model
 
 
 def test_calc_empirical():
     points = np.linspace((-100, -100), (100, 100), 100)
     target = np.linspace(-100, 100, 100)
     bin_edges, gamma = calc_empirical(points, target)
     assert np.all(np.isclose(0, bin_edges - np.asarray([
```


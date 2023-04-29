# Comparing `tmp/svg.path-6.2.tar.gz` & `tmp/svg.path-6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svg.path-6.2.tar", last modified: Fri Jun 17 12:22:18 2022, max compression
+gzip compressed data, was "svg.path-6.3.tar", last modified: Sat Apr 29 16:04:01 2023, max compression
```

## Comparing `svg.path-6.2.tar` & `svg.path-6.3.tar`

### file list

```diff
@@ -1,32 +1,23 @@
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2022-06-17 12:22:18.888301 svg.path-6.2/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6267 2022-06-17 12:22:18.000000 svg.path-6.2/CHANGES.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      864 2022-06-17 12:22:18.000000 svg.path-6.2/CONTRIBUTORS.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1087 2022-06-17 12:22:18.000000 svg.path-6.2/LICENSE.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       58 2022-06-17 12:22:18.000000 svg.path-6.2/MANIFEST.in
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    16330 2022-06-17 12:22:18.888301 svg.path-6.2/PKG-INFO
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4938 2022-06-17 12:22:18.000000 svg.path-6.2/README.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1191 2022-06-17 12:22:18.888301 svg.path-6.2/setup.cfg
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       38 2022-06-17 12:22:18.000000 svg.path-6.2/setup.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2022-06-17 12:22:18.884292 svg.path-6.2/src/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2022-06-17 12:22:18.884292 svg.path-6.2/src/svg/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       65 2022-06-17 12:22:18.000000 svg.path-6.2/src/svg/__init__.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2022-06-17 12:22:18.884292 svg.path-6.2/src/svg/path/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      226 2022-06-17 12:22:18.000000 svg.path-6.2/src/svg/path/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     9147 2022-06-17 12:22:18.000000 svg.path-6.2/src/svg/path/parser.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    21958 2022-06-17 12:22:18.000000 svg.path-6.2/src/svg/path/path.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2022-06-17 12:22:18.888301 svg.path-6.2/src/svg/path/tests/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        0 2022-06-17 12:22:18.000000 svg.path-6.2/src/svg/path/tests/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       83 2022-06-17 12:22:18.000000 svg.path-6.2/src/svg/path/tests/test_doc.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1111 2022-06-17 12:22:18.000000 svg.path-6.2/src/svg/path/tests/test_generation.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    12166 2022-06-17 12:22:18.000000 svg.path-6.2/src/svg/path/tests/test_image.png
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4491 2022-06-17 12:22:18.000000 svg.path-6.2/src/svg/path/tests/test_image.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    23257 2022-06-17 12:22:18.000000 svg.path-6.2/src/svg/path/tests/test_parsing.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    34745 2022-06-17 12:22:18.000000 svg.path-6.2/src/svg/path/tests/test_paths.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2492 2022-06-17 12:22:18.000000 svg.path-6.2/src/svg/path/tests/test_tokenizer.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2022-06-17 12:22:18.884292 svg.path-6.2/src/svg.path.egg-info/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    16330 2022-06-17 12:22:18.000000 svg.path-6.2/src/svg.path.egg-info/PKG-INFO
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      653 2022-06-17 12:22:18.000000 svg.path-6.2/src/svg.path.egg-info/SOURCES.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2022-06-17 12:22:18.000000 svg.path-6.2/src/svg.path.egg-info/dependency_links.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       33 2022-06-17 12:22:18.000000 svg.path-6.2/src/svg.path.egg-info/requires.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        4 2022-06-17 12:22:18.000000 svg.path-6.2/src/svg.path.egg-info/top_level.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2022-06-17 12:22:18.000000 svg.path-6.2/src/svg.path.egg-info/zip-safe
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-29 16:04:01.585635 svg.path-6.3/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6568 2023-04-29 16:04:01.000000 svg.path-6.3/CHANGES.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      933 2023-04-29 16:04:01.000000 svg.path-6.3/CONTRIBUTORS.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1087 2023-04-29 16:04:01.000000 svg.path-6.3/LICENSE.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       73 2023-04-29 16:04:01.000000 svg.path-6.3/MANIFEST.in
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    13420 2023-04-29 16:04:01.585635 svg.path-6.3/PKG-INFO
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4938 2023-04-29 16:04:01.000000 svg.path-6.3/README.rst
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1243 2023-04-29 16:04:01.585635 svg.path-6.3/setup.cfg
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       38 2023-04-29 16:04:01.000000 svg.path-6.3/setup.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-29 16:04:01.581635 svg.path-6.3/src/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-29 16:04:01.581635 svg.path-6.3/src/svg/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       65 2023-04-29 16:04:01.000000 svg.path-6.3/src/svg/__init__.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-29 16:04:01.581635 svg.path-6.3/src/svg/path/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      226 2023-04-29 16:04:01.000000 svg.path-6.3/src/svg/path/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     9147 2023-04-29 16:04:01.000000 svg.path-6.3/src/svg/path/parser.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    29085 2023-04-29 16:04:01.000000 svg.path-6.3/src/svg/path/path.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-29 16:04:01.581635 svg.path-6.3/src/svg.path.egg-info/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    13420 2023-04-29 16:04:01.000000 svg.path-6.3/src/svg.path.egg-info/PKG-INFO
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      381 2023-04-29 16:04:01.000000 svg.path-6.3/src/svg.path.egg-info/SOURCES.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-04-29 16:04:01.000000 svg.path-6.3/src/svg.path.egg-info/dependency_links.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       95 2023-04-29 16:04:01.000000 svg.path-6.3/src/svg.path.egg-info/requires.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        4 2023-04-29 16:04:01.000000 svg.path-6.3/src/svg.path.egg-info/top_level.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-04-29 16:04:01.000000 svg.path-6.3/src/svg.path.egg-info/zip-safe
```

### Comparing `svg.path-6.2/CHANGES.txt` & `svg.path-6.3/CHANGES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 Changelog
 =========
 
 
+6.3 (2023-04-29)
+----------------
+
+- Fixed serialization of 'H'/'h' command.
+
+- New boundingbox() methods allow you to get the boundingbox() for paths.[twjang]
+
+- Tests are now outside the source directory, which is common practice now.
+
+- Drops Python 3.6 and 3.7, adds support for 3.10 and 3.11.
+
+
 6.2 (2022-06-17)
 ----------------
 
 - Allow numbers with decimal point but no decimals, because other parsers do.
 
-- Re-enabled the README.rst doctest, which got lost when switching to pytest
+- Re-enabled the README.rst doctest, which got lost when switching to pytest.
 
 
 6.1 (2022-06-09)
 ----------------
 
 - Not all path segments preserved the relative setting. [Lucas-C]
```

### Comparing `svg.path-6.2/CONTRIBUTORS.txt` & `svg.path-6.3/CONTRIBUTORS.txt`

 * *Files 9% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 Michiel Schallig suggested calculating length by recursive straight-line
 approximations, which enables you to choose between accuracy or speed.
 Steve Schwarz added an error argument to make that choice an argument.
 
 ClayJarCom speeded up `point()` calculations for paths.
 
 Thanks also to bug fixers Martin R, abcjjy, Daniel Stender, MTician,
-blokhin, Karthikeyan, jaraco and martinleopold.
+blokhin, Karthikeyan, jaraco, martinleopold and twjang.
 
 Thanks to tatarize for help with investigating issues, and coming with
 much feedback and ideas.
 
 Samuel Carlsson [vidstige] provided the `tangent()` functions.
 
 Lucas Simon discovered and fixed that not all path segments preserved
 the relative setting when parsing.
+
+Taewoong Jang [twjang] implemented boundingbox functions. 
+
```

### Comparing `svg.path-6.2/LICENSE.txt` & `svg.path-6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `svg.path-6.2/README.rst` & `svg.path-6.3/README.rst`

 * *Files identical despite different names*

### Comparing `svg.path-6.2/setup.cfg` & `svg.path-6.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 [metadata]
 name = svg.path
-version = 6.2
+version = 6.3
 description = SVG path objects and parser
 long_description = file: README.rst, CONTRIBUTORS.txt, CHANGES.txt
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Multimedia :: Graphics
 keywords = svg, path, maths
 author = Lennart Regebro
 author_email = regebro@gmail.com
 url = https://github.com/regebro/svg.path
 license = MIT
 
 [options]
+python_requires = >=3.8
 zip_safe = True
 include_package_data = True
 packages = find:
 package_dir = 
 	= src
-test_suite = svg.path.tests
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
 	Pillow
+	black
+	flake8
+	pyroma
+	check-manifest
+	zest.releaser[recommended]
 
 [flake8]
 max-line-length = 120
 
 [bdist_wheel]
 universal = 1
 
 [tool:pytest]
 testpaths = 
-	src/svg/path/tests
+	tests
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `svg.path-6.2/src/svg/path/parser.py` & `svg.path-6.3/src/svg/path/parser.py`

 * *Files identical despite different names*

### Comparing `svg.path-6.2/src/svg/path/path.py` & `svg.path-6.3/src/svg/path/path.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,79 @@
 from math import sqrt, cos, sin, acos, degrees, radians, log, pi
 from bisect import bisect
 from abc import ABC, abstractmethod
+import math
 
 try:
     from collections.abc import MutableSequence
 except ImportError:
     from collections import MutableSequence
 
 # This file contains classes for the different types of SVG path segments as
 # well as a Path object that contains a sequence of path segments.
 
 MIN_DEPTH = 5
 ERROR = 1e-12
 
 
+def _find_solutions_for_bezier(c2, c1, c0):
+    """Find solutions of c2 * t^2 + c1 * t + c0 = 0 where t in [0, 1]"""
+    soln = []
+    if c2 == 0:
+        if c1 != 0:
+            soln.append(-c0 / c1)
+    else:
+        det = c1**2 - 4 * c2 * c0
+        if det >= 0:
+            soln.append((-c1 + math.pow(det, 0.5)) / 2.0 / c2)
+            soln.append((-c1 - math.pow(det, 0.5)) / 2.0 / c2)
+    return [s for s in soln if 0.0 <= s and s <= 1.0]
+
+
+def _find_solutions_for_arc(a, b, c, d):
+    """Find solution for a sin(x) + b cos(x) = 0 where x = c + d * t and t in [0, 1]"""
+    if a == 0:
+        # when n \in Z
+        # pi / 2 + pi * n = c + d * t
+        # --> n = d / pi * t - (1/2 - c/pi)
+        # --> t = (pi / 2 - c + pi * n) / d
+        n_ranges = [-0.5 + c / math.pi, d / math.pi - 0.5 + c / math.pi]
+        n_range_start = math.floor(min(n_ranges))
+        n_range_end = math.ceil(max(n_ranges))
+        t_list = [
+            (math.pi / 2 - c + math.pi * n) / d
+            for n in range(n_range_start, n_range_end + 1)
+        ]
+    elif b == 0:
+        # when n \in Z
+        # pi * n = c + d * t
+        # --> n = d / pi * t + c / pi
+        # --> t = (- c + pi * n) / d
+        n_ranges = [c / math.pi, d / math.pi + c / math.pi]
+        n_range_start = math.floor(min(n_ranges))
+        n_range_end = math.ceil(max(n_ranges))
+        t_list = [(-c + math.pi * n) / d for n in range(n_range_start, n_range_end + 1)]
+    else:
+        # when n \in Z
+        # arct = tan^-1 (- b / a)  and
+        # arct + pi * n = c + d * t
+        # --> n = (c - arct + d * t) / pi
+        # --> t = (arct - c + pi * n) / d
+        arct = math.atan(-b / a)
+        n_ranges = [(c - arct) / math.pi, d / math.pi + (c - arct) / math.pi]
+        n_range_start = math.floor(min(n_ranges))
+        n_range_end = math.ceil(max(n_ranges))
+        t_list = [
+            (arct - c + math.pi * n) / d for n in range(n_range_start, n_range_end + 1)
+        ]
+
+    t_list = [t for t in t_list if 0.0 <= t and t <= 1.0]
+    return t_list
+
+
 def segment_length(curve, start, end, start_point, end_point, error, min_depth, depth):
     """Recursively approximates the length by straight lines"""
     mid = (start + end) / 2
     mid_point = curve.point(mid)
     length = abs(end_point - start_point)
     first_half = abs(mid_point - start_point)
     second_half = abs(end_point - mid_point)
@@ -53,14 +109,18 @@
         """Returns the length of a path.
 
         The CubicBezier and Arc lengths are non-exact and iterative and you can select to
         either do the calculations until a maximum error has been achieved, or a minimum
         number of iterations.
         """
 
+    @abstractmethod
+    def boundingbox(self):
+        """Returns the bounding box of a path in the format of [left, top, right, bottom]"""
+
 
 class NonLinear(PathSegment):
     """A line that is not straight
 
     The base of Arc, QuadraticBezier and CubicBezier
     """
 
@@ -114,29 +174,36 @@
         y = self.end.imag
         if self.relative:
             x -= previous.end.real
             y -= previous.end.imag
 
         if self.horizontal and self.is_horizontal_from(previous):
             cmd = "h" if self.relative else "H"
-            return f"{cmd} {x:G},{y:G}"
+            return f"{cmd} {x:G}"
 
         if self.vertical and self.is_vertical_from(previous):
             cmd = "v" if self.relative else "V"
             return f"{cmd} {y:G}"
 
         cmd = "l" if self.relative else "L"
         return f"{cmd} {x:G},{y:G}"
 
     def is_vertical_from(self, previous):
         return self.start == previous.end and self.start.real == self.end.real
 
     def is_horizontal_from(self, previous):
         return self.start == previous.end and self.start.imag == self.end.imag
 
+    def boundingbox(self):
+        x_min = min(self.start.real, self.end.real)
+        x_max = max(self.start.real, self.end.real)
+        y_min = min(self.start.imag, self.end.imag)
+        y_max = max(self.start.imag, self.end.imag)
+        return [x_min, y_min, x_max, y_max]
+
 
 class CubicBezier(NonLinear):
     def __init__(self, start, control1, control2, end, relative=False, smooth=False):
         self.start = start
         self.control1 = control1
         self.control2 = control2
         self.end = end
@@ -217,14 +284,49 @@
 
     def length(self, error=ERROR, min_depth=MIN_DEPTH):
         """Calculate the length of the path up to a certain position"""
         start_point = self.point(0)
         end_point = self.point(1)
         return segment_length(self, 0, 1, start_point, end_point, error, min_depth, 0)
 
+    def boundingbox(self):
+        """Calculate the bounding box of a cubic Bezier curve.
+
+        A cubic Bezier curve and its derivative are given as follows.
+
+        P(t)  = (1-t)^3 P0 + 3 t (1-t)^2 P1 + 3 t^2 (1-t) P2 + t^3 P_3
+        P'(t) = 3(1-t)^2 (P1-P0) + 6(1-t)t (P2-P1) + 3 t^2 (P3 - P2)
+        """
+        g0 = self.control1 - self.start
+        g1 = self.control2 - self.control1
+        g2 = self.end - self.control2
+
+        c0 = 3 * g0
+        c1 = -6 * g0 + 6 * g1
+        c2 = 3 * g0 - 6 * g1 + 3 * g2
+
+        x_c0, x_c1, x_c2 = [c.real for c in [c0, c1, c2]]
+        y_c0, y_c1, y_c2 = [c.imag for c in [c0, c1, c2]]
+
+        x_cand = [0, 1] + _find_solutions_for_bezier(x_c2, x_c1, x_c0)
+        y_cand = [0, 1] + _find_solutions_for_bezier(y_c2, y_c1, y_c0)
+
+        x_coords = []
+        y_coords = []
+        for t in x_cand:
+            p = self.point(t)
+            x_coords.append(p.real)
+        for t in y_cand:
+            p = self.point(t)
+            y_coords.append(p.imag)
+
+        x_min, x_max = min(x_coords), max(x_coords)
+        y_min, y_max = min(y_coords), max(y_coords)
+        return [x_min, y_min, x_max, y_max]
+
 
 class QuadraticBezier(NonLinear):
     def __init__(self, start, control, end, relative=False, smooth=False):
         self.start = start
         self.end = end
         self.control = control
         self.relative = relative
@@ -322,14 +424,47 @@
                 k = abs(b) / abs(a)
                 if k >= 2:
                     s = abs(b) - abs(a)
                 else:
                     s = abs(a) * (k**2 / 2 - k + 1)
         return s
 
+    def boundingbox(self):
+        """Calculate the bounding box of a quadratic Bezier curve.
+
+        A quadratic Bezier curve and its derivative are given as follows.
+
+        P(t)  = (1-t)^2 P0 + 2 t (1-t)^2 P1 + t^2 P2
+        P'(t) = 2(1-t) (P1-P0) + 2t (P2-P1)
+        """
+        g0 = self.control - self.start
+        g1 = self.end - self.control
+
+        c0 = 2 * g0
+        c1 = -2 * g0 + 2 * g1
+
+        x_c0, x_c1 = [c.real for c in [c0, c1]]
+        y_c0, y_c1 = [c.imag for c in [c0, c1]]
+
+        x_cand = [0, 1] + _find_solutions_for_bezier(0, x_c1, x_c0)
+        y_cand = [0, 1] + _find_solutions_for_bezier(0, y_c1, y_c0)
+
+        x_coords = []
+        y_coords = []
+        for t in x_cand:
+            p = self.point(t)
+            x_coords.append(p.real)
+        for t in y_cand:
+            p = self.point(t)
+            y_coords.append(p.imag)
+
+        x_min, x_max = min(x_coords), max(x_coords)
+        y_min, y_max = min(y_coords), max(y_coords)
+        return [x_min, y_min, x_max, y_max]
+
 
 class Arc(NonLinear):
     def __init__(self, start, radius, rotation, arc, sweep, end, relative=False):
         """radius is complex, rotation is in degrees,
         large and sweep are 1 or 0 (True/False also work)"""
 
         self.start = start
@@ -511,14 +646,61 @@
             radius = self.radius.real * self.radius_scale
             return abs(radius * self.delta * pi / 180)
 
         start_point = self.point(0)
         end_point = self.point(1)
         return segment_length(self, 0, 1, start_point, end_point, error, min_depth, 0)
 
+    def boundingbox(self):
+        """Calculate the bounding box of an arc
+
+        To calculate the extremums of the arc coordinates, we solve
+
+        x'(angle) = - cosr * radius.real * sin(angle)
+                    - sinr * radius.imag * cos(angle) = 0
+
+        y'(angle) = - sinr * radius.real * sin(angle)
+                    + cosr * radius.imag * cos(angle) = 0
+
+        and
+            angle = radians(self.theta + (self.delta * pos))
+        where pos ranges from 0 to 1
+        """
+
+        # angle = radians(self.theta + (self.delta * pos))
+        cosr = cos(radians(self.rotation))
+        sinr = sin(radians(self.rotation))
+        radius = self.radius * self.radius_scale
+
+        x_a = -cosr * radius.real
+        x_b = -sinr * radius.imag
+        x_c = radians(self.theta)
+        x_d = radians(self.delta)
+
+        y_a = -sinr * radius.real
+        y_b = +cosr * radius.imag
+        y_c = radians(self.theta)
+        y_d = radians(self.delta)
+
+        x_pos = [0, 1.0] + _find_solutions_for_arc(x_a, x_b, x_c, x_d)
+        y_pos = [0, 1.0] + _find_solutions_for_arc(y_a, y_b, y_c, y_d)
+
+        x_coords = []
+        y_coords = []
+        for pos in x_pos:
+            p = self.point(pos)
+            x_coords.append(p.real)
+        for pos in y_pos:
+            p = self.point(pos)
+            y_coords.append(p.imag)
+
+        x_min, x_max = min(x_coords), max(x_coords)
+        y_min, y_max = min(y_coords), max(y_coords)
+        return [x_min, y_min, x_max, y_max]
+
 
 class Move:
     """Represents move commands. Does nothing, but is there to handle
     paths that consist of only move commands, which is valid, but pointless.
     """
 
     def __init__(self, to, relative=False):
@@ -554,14 +736,21 @@
 
     def tangent(self, pos):
         return 0
 
     def length(self, error=ERROR, min_depth=MIN_DEPTH):
         return 0
 
+    def boundingbox(self):
+        x_min = min(self.start.real, self.end.real)
+        x_max = max(self.start.real, self.end.real)
+        y_min = min(self.start.imag, self.end.imag)
+        y_max = max(self.start.imag, self.end.imag)
+        return [x_min, y_min, x_max, y_max]
+
 
 class Close(Linear):
     """Represents the closepath command"""
 
     def __eq__(self, other):
         if not isinstance(other, Close):
             return NotImplemented
@@ -569,14 +758,21 @@
 
     def __repr__(self):
         return f"Close(start={self.start}, end={self.end})"
 
     def _d(self, previous):
         return "z" if self.relative else "Z"
 
+    def boundingbox(self):
+        x_min = min(self.start.real, self.end.real)
+        x_max = max(self.start.real, self.end.real)
+        y_min = min(self.start.imag, self.end.imag)
+        y_max = max(self.start.imag, self.end.imag)
+        return [x_min, y_min, x_max, y_max]
+
 
 class Path(MutableSequence):
     """A Path is a sequence of path segments"""
 
     def __init__(self, *segments):
         self._segments = list(segments)
         self._length = None
@@ -607,15 +803,14 @@
     def __len__(self):
         return len(self._segments)
 
     def __repr__(self):
         return "Path(%s)" % (", ".join(repr(x) for x in self._segments))
 
     def __eq__(self, other):
-
         if not isinstance(other, Path):
             return NotImplemented
         if len(self) != len(other):
             return False
         for s, o in zip(self._segments, other._segments):
             if not s == o:
                 return False
@@ -684,7 +879,22 @@
         previous_segment = None
 
         for segment in self:
             parts.append(segment._d(previous_segment))
             previous_segment = segment
 
         return " ".join(parts)
+
+    def boundingbox(self):
+        x_coords = []
+        y_coords = []
+
+        for e in self:
+            x_min, y_min, x_max, y_max = e.boundingbox()
+            x_coords.append(x_min)
+            x_coords.append(x_max)
+            y_coords.append(y_min)
+            y_coords.append(y_max)
+
+        x_min, x_max = min(x_coords), max(x_coords)
+        y_min, y_max = min(y_coords), max(y_coords)
+        return [x_min, y_min, x_max, y_max]
```


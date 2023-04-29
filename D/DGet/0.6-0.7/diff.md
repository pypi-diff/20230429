# Comparing `tmp/DGet-0.6.tar.gz` & `tmp/DGet-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DGet-0.6.tar", last modified: Thu Apr 27 05:31:05 2023, max compression
+gzip compressed data, was "DGet-0.7.tar", last modified: Sat Apr 29 03:33:47 2023, max compression
```

## Comparing `DGet-0.6.tar` & `DGet-0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:31:05.559666 DGet-0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:31:05.559666 DGet-0.6/DGet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-27 05:31:05.000000 DGet-0.6/DGet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-27 05:31:05.000000 DGet-0.6/DGet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 05:31:05.000000 DGet-0.6/DGet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 05:31:05.000000 DGet-0.6/DGet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-27 05:31:05.000000 DGet-0.6/DGet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 05:31:05.000000 DGet-0.6/DGet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 05:30:55.000000 DGet-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-27 05:31:05.559666 DGet-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-27 05:30:55.000000 DGet-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:31:05.559666 DGet-0.6/dget/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 05:30:55.000000 DGet-0.6/dget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-27 05:30:55.000000 DGet-0.6/dget/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-27 05:30:55.000000 DGet-0.6/dget/adduct.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-27 05:30:55.000000 DGet-0.6/dget/convolve.py
--rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-04-27 05:30:55.000000 DGet-0.6/dget/dget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-27 05:30:55.000000 DGet-0.6/dget/formula.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 05:31:05.559666 DGet-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-27 05:30:55.000000 DGet-0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:31:05.559666 DGet-0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-27 05:30:55.000000 DGet-0.6/tests/test_adduct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-27 05:30:55.000000 DGet-0.6/tests/test_dget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-27 05:30:55.000000 DGet-0.6/tests/test_formula.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:33:47.149280 DGet-0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:33:47.145280 DGet-0.7/DGet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-29 03:33:47.000000 DGet-0.7/DGet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-29 03:33:47.000000 DGet-0.7/DGet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 03:33:47.000000 DGet-0.7/DGet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-29 03:33:47.000000 DGet-0.7/DGet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-29 03:33:47.000000 DGet-0.7/DGet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 03:33:47.000000 DGet-0.7/DGet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-29 03:33:36.000000 DGet-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-29 03:33:47.149280 DGet-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-29 03:33:36.000000 DGet-0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:33:47.149280 DGet-0.7/dget/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-29 03:33:36.000000 DGet-0.7/dget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-29 03:33:36.000000 DGet-0.7/dget/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-29 03:33:36.000000 DGet-0.7/dget/adduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-29 03:33:36.000000 DGet-0.7/dget/convolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-04-29 03:33:36.000000 DGet-0.7/dget/dget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-29 03:33:36.000000 DGet-0.7/dget/formula.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 03:33:47.149280 DGet-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-29 03:33:36.000000 DGet-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:33:47.149280 DGet-0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-29 03:33:36.000000 DGet-0.7/tests/test_adduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-29 03:33:36.000000 DGet-0.7/tests/test_dget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-29 03:33:36.000000 DGet-0.7/tests/test_formula.py
```

### Comparing `DGet-0.6/LICENSE` & `DGet-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `DGet-0.6/dget/__main__.py` & `DGet-0.7/dget/__main__.py`

 * *Files identical despite different names*

### Comparing `DGet-0.6/dget/adduct.py` & `DGet-0.7/dget/adduct.py`

 * *Files identical despite different names*

### Comparing `DGet-0.6/dget/convolve.py` & `DGet-0.7/dget/convolve.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     Deconvolution is performed in frequency domain.
 
     Args:
         x: array
         psf: point spread function
         mode: if same, return same size as `x` {'valid', 'same'}
 
+    Returns:
+        recovered data
+        remainder
+
     Notes:
         Based on https://rosettacode.org/wiki/Deconvolution/1D
     """
 
     def shift_bit_length(x: int) -> int:
         return 1 << (x - 1).bit_length()
```

### Comparing `DGet-0.6/dget/dget.py` & `DGet-0.7/dget/dget.py`

 * *Files 3% similar despite different names*

```diff
@@ -182,32 +182,14 @@
         return f"DGet({self.adduct!r})"
 
     def _read_tofdata(
         self, path: str | Path, **kwargs
     ) -> Tuple[np.ndarray, np.ndarray]:
         """Internal helper to read mass spectra data.
 
-        kwargs are forwarded to ``numpy.loadtxt``.
-Formula          : C12H[2H]8N
-Adduct           : [M-H]-
-M/Z              : 175.12371326162
-Adduct M/Z       : 174.11643680929907
-%D               : 93.66 %
-
-Deuteration Ratio Spectra
-D0               :  0.15 %
-D1               :  0.18 %
-D2               :  0.20 %
-D3               :  0.26 %
-D4               :  0.39 %
-D5               :  1.41 %
-D6               :  6.05 %
-D7               : 27.79 %
-D8               : 63.56 %
-
         Args:
             path: path to file
 
         Returns:
             masses
             signals
         """
@@ -339,29 +321,29 @@
         masses = [i.mz for i in self.spectrum.values()]
         ax.stem(
             masses,
             scale_spectra(x, y, masses, self.psf),
             markerfmt=" ",
             basefmt=" ",
             linefmt="blue",
-            label=f"{self.adduct.formula.formula} Spectra",
+            label="Adduct Spectra",
         )
         ax.set_title(f"{self.adduct.base.formula} {self.adduct.adduct}")
-        ax.set_xlabel("Mass")
+        ax.set_xlabel("M/Z")
         ax.set_ylabel("Signal")
-        ax.legend()
+        ax.legend(loc="best", bbox_to_anchor=(0.0, 0.6, 1.0, 0.4))
 
     def print_results(self) -> None:
         """Print results to stdout."""
         pd = self.deuteration  # ensure calculated
 
         print(f"Formula          : {self.adduct.base.formula}")
         print(f"Adduct           : {self.adduct.adduct}")
-        print(f"M/Z              : {self.adduct.base.isotope.mz}")
-        print(f"Adduct M/Z       : {self.formula.isotope.mz}")
+        print(f"M/Z              : {self.adduct.base.isotope.mz:.4f}")
+        print(f"Adduct M/Z       : {self.formula.isotope.mz:.4f}")
         print(f"%Deuteration     : {pd * 100.0:.2f} %")
         print()
         print("Deuteration Ratio Spectra")
         for i, p in enumerate(self.deuteration_probabilites):
             print(f"D{i:<2}              : {p * 100.0:5.2f} %")
 
     def spectra(self, **kwargs) -> Generator[Spectrum, None, None]:
```

### Comparing `DGet-0.6/dget/formula.py` & `DGet-0.7/dget/formula.py`

 * *Files identical despite different names*

### Comparing `DGet-0.6/setup.py` & `DGet-0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 from setuptools import setup
 
-with open("README.md") as fp:
+with open("README.rst") as fp:
     long_description = fp.read()
 
 with Path("dget", "__init__.py").open() as fp:
     version = None
     for line in fp:
         if line.startswith("__version__"):
             version = line.split("=")[1].strip().strip('"')
@@ -14,15 +14,15 @@
         raise ValueError("Could not read version from __init__.py")
 
 setup(
     name="DGet",
     version=version,
     description="Calculates compound deuteration from ToF-MS data.",
     long_description=long_description,
-    long_description_content_type="text/markdown",
+    long_description_content_type="text/x-rst",
     packages=["dget"],
     license="GPL3",
     author="djdt",
     url="https://github.com/djdt/dget",
     project_urls={
         "Documentation": "https://dget.readthedocs.io",
         "Source": "https://github.com/djdt/dget",
```

### Comparing `DGet-0.6/tests/test_adduct.py` & `DGet-0.7/tests/test_adduct.py`

 * *Files identical despite different names*

### Comparing `DGet-0.6/tests/test_dget.py` & `DGet-0.7/tests/test_dget.py`

 * *Files identical despite different names*

### Comparing `DGet-0.6/tests/test_formula.py` & `DGet-0.7/tests/test_formula.py`

 * *Files identical despite different names*


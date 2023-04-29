# Comparing `tmp/bhv-0.2.4.tar.gz` & `tmp/bhv-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.2.4.tar", last modified: Sun Apr 23 18:45:46 2023, max compression
+gzip compressed data, was "bhv-0.2.5.tar", last modified: Sat Apr 29 19:08:25 2023, max compression
```

## Comparing `bhv-0.2.4.tar` & `bhv-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-23 18:45:46.086419 bhv-0.2.4/
--rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.2.4/LICENSE
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-04-23 18:45:46.086419 bhv-0.2.4/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3142 2023-04-23 18:45:24.000000 bhv-0.2.4/README.md
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-23 18:45:46.086419 bhv-0.2.4/bhv/
--rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-11 14:49:00.000000 bhv-0.2.4/bhv/__init__.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11929 2023-04-21 10:02:48.000000 bhv-0.2.4/bhv/abstract.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1635 2023-04-11 14:49:00.000000 bhv-0.2.4/bhv/embedding.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11175 2023-04-18 17:00:07.000000 bhv-0.2.4/bhv/np.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     8193 2023-04-18 19:16:09.000000 bhv-0.2.4/bhv/pytorch.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2022 2023-04-17 15:03:13.000000 bhv-0.2.4/bhv/shared.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    13150 2023-04-23 16:54:25.000000 bhv-0.2.4/bhv/symbolic.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      633 2023-04-23 18:40:01.000000 bhv-0.2.4/bhv/visualization.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-23 18:45:46.086419 bhv-0.2.4/bhv.egg-info/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-04-23 18:45:46.000000 bhv-0.2.4/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)      285 2023-04-23 18:45:46.000000 bhv-0.2.4/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-04-23 18:45:46.000000 bhv-0.2.4/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       73 2023-04-23 18:45:46.000000 bhv-0.2.4/bhv.egg-info/requires.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-04-23 18:45:46.000000 bhv-0.2.4/bhv.egg-info/top_level.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-04-23 18:45:46.086419 bhv-0.2.4/setup.cfg
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1331 2023-04-23 18:17:55.000000 bhv-0.2.4/setup.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-29 19:08:25.402615 bhv-0.2.5/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.2.5/LICENSE
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-04-29 19:08:25.402615 bhv-0.2.5/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3202 2023-04-29 09:52:26.000000 bhv-0.2.5/README.md
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-29 19:08:25.402615 bhv-0.2.5/bhv/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.2.5/bhv/__init__.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11962 2023-04-28 20:37:06.000000 bhv-0.2.5/bhv/abstract.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1635 2023-04-11 14:49:00.000000 bhv-0.2.5/bhv/embedding.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11175 2023-04-18 17:00:07.000000 bhv-0.2.5/bhv/np.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-04-24 21:41:56.000000 bhv-0.2.5/bhv/poibin.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.2.5/bhv/positions.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     8193 2023-04-18 19:16:09.000000 bhv-0.2.5/bhv/pytorch.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2356 2023-04-28 22:56:24.000000 bhv-0.2.5/bhv/shared.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1152 2023-04-24 02:20:49.000000 bhv-0.2.5/bhv/slice.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    21307 2023-04-29 09:47:12.000000 bhv-0.2.5/bhv/symbolic.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3325 2023-04-28 20:51:52.000000 bhv-0.2.5/bhv/vanilla.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      782 2023-04-28 16:55:18.000000 bhv-0.2.5/bhv/visualization.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-29 19:08:25.402615 bhv-0.2.5/bhv.egg-info/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-04-29 19:08:25.000000 bhv-0.2.5/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      344 2023-04-29 19:08:25.000000 bhv-0.2.5/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-04-29 19:08:25.000000 bhv-0.2.5/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       73 2023-04-29 19:08:25.000000 bhv-0.2.5/bhv.egg-info/requires.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-04-29 19:08:25.000000 bhv-0.2.5/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-04-29 19:08:25.402615 bhv-0.2.5/setup.cfg
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1331 2023-04-29 19:07:56.000000 bhv-0.2.5/setup.py
```

### Comparing `bhv-0.2.4/LICENSE` & `bhv-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bhv-0.2.4/PKG-INFO` & `bhv-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.2.4
+Version: 0.2.5
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bhv-0.2.4/README.md` & `bhv-0.2.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 # Python Boolean Hyper-Vectors
 
 WIP repository for research into vector symbolic architectures like Multiply-Add-Permute and Binary Spatter Codes.
+Can be used dependency-free.
 
 ## Contains
-The fundamental research includes finding algebras with interesting properties on top of large boolean vectors. To this extend the library has [laws used for testing](tests/laws.py) and an expansive [set of operators](bhv/abstract.py) including:
+The fundamental research includes finding algebras with interesting properties on top of large boolean vectors. To this extent the library has [laws used for testing](tests/laws.py) and an expansive [set of operators](bhv/abstract.py) including:
 - Multiple types of random vector generation
 - Random and indexed select between vectors
 - Ability to slightly modify a vector, for example by flipping a fraction of its bits
 - Permutation, roll, and swapping with multiple interfaces
 - Hashing and encoding
 - Majority with multiple implementation
 - AND, OR, and XOR operators
 - Hamming, jaccard, cosine, and bit-error-rate "metrics"
 - A system for relatedness, unrelatedness, and standard deviations apart
 - zscore and pvalue
 
 Additionally, provided are
-- A symbolic implementation with plotting and pretty printing
+- A symbolic implementation with analysis, plotting and pretty printing
 - Efficient bit-packed representation
 - Three redundant implementations on NumPy for performance and correctness
 - A minimal abstraction for permutations with caching and composition
 - Very basic embeddings for other datatypes (more to come)
 - Graph visualization of distances in hyperdimensional space ([see example](examples/viz_distances.py)).
+- Boolean expression and network synthesis
 
 ## Installation
 `pip install bhv`
 
-If you only want to work with the symbolic implementation, you're good to go with `from bhv.symbolic import Var, SymbolicBHV`.
+If you only want to work with plain Python, you're good to go with `from bhv.vanilla VanillaBHV as BHV`.
 
 Else you'll need
 `pip install numpy` or `pip install torch` with respectively `from bhv.np import NumPyPacked64BHV as BHV` or `from bhv.np import TorchBoolBHV as BHV`. 
 
 ## Getting started
 One way to start is with going over [Kanerva's initial paper](http://ww.robertdick.org/iesr/papers/kanerva09jan.pdf) together with the library.
 For that, multiple resources are provided:
```

### Comparing `bhv-0.2.4/bhv/abstract.py` & `bhv-0.2.5/bhv/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,17 +325,15 @@
         return cls._majority3(g, cls._majority3(c, mdef, cls._majority3(a, b, mdef)), cls._majority3(f, mabc, cls._majority3(d, e, mabc)))
 
     ZERO: Self
     ONE: Self
     HALF: Self
 
 
-class MemoizedPermutation:
-    _permutations: 'dict[int | tuple[int, ...], Self]'
-
+class Permutation:
     @classmethod
     def nrandom(cls, n) -> list[Self]:
         return [cls.random() for _ in range(n)]
 
     @classmethod
     def random(cls) -> Self:
         raise NotImplementedError()
@@ -351,14 +349,18 @@
         for _ in range(power - 1):
             permutation = permutation*permutation
         return permutation
 
     def __call__(self, hv: 'AbstractBHV') -> 'AbstractBHV':
         raise NotImplementedError()
 
+
+class MemoizedPermutation(Permutation):
+    _permutations: 'dict[int | tuple[int, ...], Self]'
+
     @classmethod
     def _get_singular(cls, permutation_id: int) -> Self:
         if permutation_id in cls._permutations:
             return cls._permutations[permutation_id]
         elif -permutation_id in cls._permutations:
             inv_permutation = cls._permutations[-permutation_id]
             permutation = ~inv_permutation
```

### Comparing `bhv-0.2.4/bhv/embedding.py` & `bhv-0.2.5/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.4/bhv/np.py` & `bhv-0.2.5/bhv/np.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.4/bhv/pytorch.py` & `bhv-0.2.5/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.4/bhv/shared.py` & `bhv-0.2.5/bhv/shared.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,8 +52,31 @@
     :param version: Increase this number if you want to unconditionally break all hashcodes
     :return: The 24 character base64 (with - and _) string hash
     """
     h = stable_hash(d)
     padded = h.rjust(18, version.to_bytes(1, "little"))
     base64 = binascii.b2a_base64(padded, newline=False)
     url_safe = base64.translate(_urlsafe_encode_translation)
-    return url_safe.decode()
+    return url_safe.decode()
+
+
+def nbs(i, w):
+    k = 1
+    for _ in range(w):
+        yield i ^ k
+        k <<= 1
+
+
+def binw(i, w):
+    return bin(i)[2:].rjust(w, '0')
+
+
+def to_bitmask(s):
+    return [x == '1' for x in s]
+
+
+def bin_bitmask(m):
+    return ''.join("01"[x] for x in m)
+
+
+def bitconfigs(n):
+    return [to_bitmask(binw(i, n)) for i in range(2**n)]
```

### Comparing `bhv-0.2.4/bhv/visualization.py` & `bhv-0.2.5/bhv/visualization.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from .abstract import AbstractBHV
 
 
 class DistanceGraph:
-    def __init__(self, d: 'dict[str, AbstractBHV]'):
-        self.hvs = list(d.values())
-        self.labels = list(d.keys())
+    @classmethod
+    def from_scope(cls, local_dict):
+        return cls(*zip(*[(v, k) for k, v in local_dict.items() if isinstance(v, AbstractBHV)]))
+
+    def __init__(self, hvs: 'list[AbstractBHV]', labels: 'list[str]'):
+        self.hvs = hvs
+        self.labels = labels
         self.adj = [[round(min(v.std_apart(w, invert=True), v.std_apart(w))) if not v.unrelated(w) else 0
                      for v in self.hvs]
                     for w in self.hvs]
 
     def graphviz(self):
         for i, (r, l) in enumerate(zip(self.adj, self.labels)):
             print(f"{i} [label=\"{l}\"];")
```

### Comparing `bhv-0.2.4/bhv.egg-info/PKG-INFO` & `bhv-0.2.5/bhv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.2.4
+Version: 0.2.5
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bhv-0.2.4/setup.py` & `bhv-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.4'
+VERSION = '0.2.5'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 setup(
     name="bhv",
     version=VERSION,
     author="Adam Vandervorst",
```


# Comparing `tmp/tamp-1.0.1.tar.gz` & `tmp/tamp-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tamp-1.0.1.tar", max compression
+gzip compressed data, was "tamp-1.0.2.tar", max compression
```

## Comparing `tamp-1.0.1.tar` & `tamp-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-04-28 19:23:23.715803 tamp-1.0.1/LICENSE
--rw-r--r--   0        0        0    14323 2023-04-28 19:23:23.715803 tamp-1.0.1/README.rst
--rw-r--r--   0        0        0     4998 2023-04-28 19:23:46.532631 tamp-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2497 2023-04-28 19:23:46.536632 tamp-1.0.1/tamp/__init__.py
--rw-r--r--   0        0        0     1523 2023-04-28 19:23:23.719803 tamp-1.0.1/tamp/__init__.pyi
--rw-r--r--   0        0        0       57 2023-04-28 19:23:23.719803 tamp-1.0.1/tamp/__main__.py
--rw-r--r--   0        0        0        0 2023-04-28 19:23:23.719803 tamp-1.0.1/tamp/cli/__init__.py
--rw-r--r--   0        0        0     2665 2023-04-28 19:23:23.719803 tamp-1.0.1/tamp/cli/main.py
--rw-r--r--   0        0        0     8237 2023-04-28 19:23:23.719803 tamp-1.0.1/tamp/compressor.py
--rw-r--r--   0        0        0     7136 2023-04-28 19:23:23.719803 tamp-1.0.1/tamp/compressor_viper.py
--rw-r--r--   0        0        0     6530 2023-04-28 19:23:23.719803 tamp-1.0.1/tamp/decompressor.py
--rw-r--r--   0        0        0     9951 2023-04-28 19:23:23.719803 tamp-1.0.1/tamp/decompressor_viper.py
--rw-r--r--   0        0        0        0 2023-04-28 19:23:23.719803 tamp-1.0.1/tamp/py.typed
--rw-r--r--   0        0        0    14942 1970-01-01 00:00:00.000000 tamp-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-29 16:23:57.808892 tamp-1.0.2/LICENSE
+-rw-r--r--   0        0        0    14325 2023-04-29 16:23:57.808892 tamp-1.0.2/README.rst
+-rw-r--r--   0        0        0     4891 2023-04-29 16:24:20.810662 tamp-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2497 2023-04-29 16:24:20.810662 tamp-1.0.2/tamp/__init__.py
+-rw-r--r--   0        0        0     1619 2023-04-29 16:23:57.812893 tamp-1.0.2/tamp/__init__.pyi
+-rw-r--r--   0        0        0       57 2023-04-29 16:23:57.812893 tamp-1.0.2/tamp/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-29 16:23:57.812893 tamp-1.0.2/tamp/cli/__init__.py
+-rw-r--r--   0        0        0     2665 2023-04-29 16:23:57.812893 tamp-1.0.2/tamp/cli/main.py
+-rw-r--r--   0        0        0     8237 2023-04-29 16:23:57.812893 tamp-1.0.2/tamp/compressor.py
+-rw-r--r--   0        0        0     7136 2023-04-29 16:23:57.812893 tamp-1.0.2/tamp/compressor_viper.py
+-rw-r--r--   0        0        0     6530 2023-04-29 16:23:57.812893 tamp-1.0.2/tamp/decompressor.py
+-rw-r--r--   0        0        0     9951 2023-04-29 16:23:57.812893 tamp-1.0.2/tamp/decompressor_viper.py
+-rw-r--r--   0        0        0        0 2023-04-29 16:23:57.812893 tamp-1.0.2/tamp/py.typed
+-rw-r--r--   0        0        0    14944 1970-01-01 00:00:00.000000 tamp-1.0.2/PKG-INFO
```

### Comparing `tamp-1.0.1/LICENSE` & `tamp-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tamp-1.0.1/README.rst` & `tamp-1.0.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
 Tamp usually out-performs heatshrink, and is generally very competitive with zlib.
 While trying to be an apples-to-apples comparison, zlib still uses significantly more
 memory during both compression and decompression (see next section). Tamp accomplishes
 competitive performance while using around 10x less memory.
 
 Memory Usage
 ^^^^^^^^^^^^
-The following table shows approximately how much memory each algorithm uses with a window size of 1KB (10 bit).
+The following table shows approximately how much memory each algorithm uses during compression and decompression.
 
 +---------------+-------------------+------------------------------+-------------------+
 | Action        | tamp              | zlib                         | heatshrink        |
 +===============+===================+==============================+===================+
 | Compression   | (1 << windowBits) | (1 << (windowBits+2)) + 7 KB | (1 << windowBits) |
 +---------------+-------------------+------------------------------+-------------------+
 | Decompression | (1 << windowBits) | (1 << windowBits) + 7 KB     | (1 << windowBits) |
```

### Comparing `tamp-1.0.1/pyproject.toml` & `tamp-1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,58 +5,51 @@
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs = "git"
 style = "semver"
 
 [tool.poetry]
 name = "tamp"
-version = "1.0.1"  # Do not change, let poetry-dynamic-versioning handle it.
+version = "1.0.2"  # Do not change, let poetry-dynamic-versioning handle it.
 homepage = "https://github.com/BrianPugh/tamp"
 repository = "https://github.com/BrianPugh/tamp"
 license = "Apache-2.0"
 description = ""
 authors = ["Brian Pugh"]
 readme = "README.rst"
 packages = [{include = "tamp"}]
 
 [tool.poetry.scripts]
 tamp = "tamp.cli.main:run_app"
 
 [tool.poetry.dependencies]
 # Be as loose as possible if writing a library.
 python = "^3.8"
-typer = "^0.6.0"
+typer = ">=0.6.0, <1.0.0"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "~4.5.0"
 sphinx_rtd_theme = "~1.0.0"
 gitpython = "^3.1.31"
-sphinx-copybutton = "^0.5.2"
+sphinx-copybutton = ">=0.5.2, <1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 coverage = {extras = ["toml"], version = "^5.1"}
 poetry-dynamic-versioning = ">=0.16.0, <1.0.0"
 pre_commit = "^2.16.0"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 pytest-mock = "^3.7.0"
 black = "^23.1.0"
 belay = ">=0.19.2, <1.0.0"
 tqdm = "^4.65.0"
 matplotlib = "^3.7.1"
-ipdb = "^0.13.13"
+ipdb = ">=0.13.13, <1.0.0"
 mpremote = "^1.20.0"
 
-[tool.poetry.group.debug]
-optional = true
-
-[tool.poetry.group.debug.dependencies]
-ipdb = ">=0.13.9, <1.0.0"
-line_profiler = "^3.5.1"
-
 [tool.belay]
 name = "tamp"
 
 [tool.belay.group.dev]
 optional = true
 
 [tool.belay.group.dev.dependencies]
```

### Comparing `tamp-1.0.1/tamp/__init__.py` & `tamp-1.0.2/tamp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Don't manually change, let poetry-dynamic-versioning-plugin handle it.
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 
 class ExcessBitsError(Exception):
     """Provided data has more bits than expected ``literal`` bits."""
 
 
 def bit_size(value):
```

### Comparing `tamp-1.0.1/tamp/__init__.pyi` & `tamp-1.0.2/tamp/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from pathlib import Path
 from typing import Literal, Optional, Union, overload
 
 from .compressor import Compressor as Compressor
 from .compressor import TextCompressor as TextCompressor
+from .compressor import compress as compress
 from .decompressor import Decompressor as Decompressor
 from .decompressor import TextDecompressor as TextDecompressor
+from .decompressor import decompress as decompress
 
 __version__: str
 
 PathLike = Union[Path, str]
 
 OpenTextModeWriting = Literal["w", "wt", "tw"]
 OpenTextModeReading = Literal["r", "rt", "tr"]
```

### Comparing `tamp-1.0.1/tamp/cli/main.py` & `tamp-1.0.2/tamp/cli/main.py`

 * *Files identical despite different names*

### Comparing `tamp-1.0.1/tamp/compressor.py` & `tamp-1.0.2/tamp/compressor.py`

 * *Files identical despite different names*

### Comparing `tamp-1.0.1/tamp/compressor_viper.py` & `tamp-1.0.2/tamp/compressor_viper.py`

 * *Files identical despite different names*

### Comparing `tamp-1.0.1/tamp/decompressor.py` & `tamp-1.0.2/tamp/decompressor.py`

 * *Files identical despite different names*

### Comparing `tamp-1.0.1/tamp/decompressor_viper.py` & `tamp-1.0.2/tamp/decompressor_viper.py`

 * *Files identical despite different names*

### Comparing `tamp-1.0.1/PKG-INFO` & `tamp-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: tamp
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 Home-page: https://github.com/BrianPugh/tamp
 License: Apache-2.0
 Author: Brian Pugh
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: typer (>=0.6.0,<0.7.0)
+Requires-Dist: typer (>=0.6.0,<1.0.0)
 Project-URL: Repository, https://github.com/BrianPugh/tamp
 Description-Content-Type: text/x-rst
 
 .. image:: https://raw.githubusercontent.com/BrianPugh/tamp/main/assets/logo_300w.png
    :alt: tamp logo
    :width: 300
    :align: center
@@ -246,15 +246,15 @@
 Tamp usually out-performs heatshrink, and is generally very competitive with zlib.
 While trying to be an apples-to-apples comparison, zlib still uses significantly more
 memory during both compression and decompression (see next section). Tamp accomplishes
 competitive performance while using around 10x less memory.
 
 Memory Usage
 ^^^^^^^^^^^^
-The following table shows approximately how much memory each algorithm uses with a window size of 1KB (10 bit).
+The following table shows approximately how much memory each algorithm uses during compression and decompression.
 
 +---------------+-------------------+------------------------------+-------------------+
 | Action        | tamp              | zlib                         | heatshrink        |
 +===============+===================+==============================+===================+
 | Compression   | (1 << windowBits) | (1 << (windowBits+2)) + 7 KB | (1 << windowBits) |
 +---------------+-------------------+------------------------------+-------------------+
 | Decompression | (1 << windowBits) | (1 << windowBits) + 7 KB     | (1 << windowBits) |
```


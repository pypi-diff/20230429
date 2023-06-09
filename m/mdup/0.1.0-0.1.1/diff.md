# Comparing `tmp/mdup-0.1.0.tar.gz` & `tmp/mdup-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdup-0.1.0.tar", max compression
+gzip compressed data, was "mdup-0.1.1.tar", max compression
```

## Comparing `mdup-0.1.0.tar` & `mdup-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-04-28 20:21:54.847432 mdup-0.1.0/LICENSE
--rw-r--r--   0        0        0     1730 2023-04-29 07:37:57.616300 mdup-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-28 20:23:45.221191 mdup-0.1.0/mdup/__init__.py
--rw-r--r--   0        0        0     3632 2023-04-29 06:36:35.552520 mdup-0.1.0/mdup/mdup.py
--rw-r--r--   0        0        0      780 2023-04-28 23:49:20.739506 mdup-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2163 1970-01-01 00:00:00.000000 mdup-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-28 20:21:54.847432 mdup-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1786 2023-04-29 08:00:35.717833 mdup-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 20:23:45.221191 mdup-0.1.1/mdup/__init__.py
+-rw-r--r--   0        0        0     3632 2023-04-29 06:36:35.552520 mdup-0.1.1/mdup/mdup.py
+-rw-r--r--   0        0        0      863 2023-04-29 08:20:20.738532 mdup-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2363 1970-01-01 00:00:00.000000 mdup-0.1.1/PKG-INFO
```

### Comparing `mdup-0.1.0/LICENSE` & `mdup-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mdup-0.1.0/README.md` & `mdup-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 
 [![Build](https://github.com/alexandru-dinu/mdup/actions/workflows/main.yml/badge.svg)](https://github.com/alexandru-dinu/mdup/actions/workflows/main.yml)
 
 Keep markdown files up-to-date by injecting code or script output between special blocks.
 
 There are no external dependencies, i.e. apart from Python stdlib.
 
+## Install
+
+```
+pip install mdup
+```
+
 ## How does it work?
 
 The blocks are defined using HTML comments.
 Specifically, the **begin** block is of the form:
 
     <!-- MDUP:BEG ({CMD}:{CONTENTS}) -->
 
@@ -18,15 +24,15 @@
 - `RUN`: to execute the script from `{CONTENTS}` and inject its stdout in the block
 
 **NOTES**
 - For `SRC` and `RUN` commands, the `{CONTENTS}` must be a path, relative to the md file.
 - The blocks must be defined as the sole contents of the line, i.e. matching `^` and `$` anchors.
 
 ## Usage
-<!-- MDUP:BEG (RUN:./help.sh) -->
+<!-- MDUP:BEG (RUN:./scripts/help.sh) -->
 ```
 usage: mdup [-h] -i INPUT [-o OUTPUT]
 
 options:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         Input file.
@@ -38,13 +44,13 @@
 Running `mdup -i <input.md> -o <output.md>` will replace the contents between each block
 with the appropriate action as defined above. This means that you can keep files up-to-date by simply rerunning `mdup`.
 
 Omitting the `-o` option will edit the file in-place.
 
 For example, the cmdline usage block above is automatically generated by defining:
 
-    <!-- MDUP:BEG (RUN:./help.sh) -->
+    <!-- MDUP:BEG (RUN:./scripts/help.sh) -->
     <!-- MDUP:END -->
 
-then running `mdup -i README.md`
+then running `mdup -i README.md`.
 
-[^1]: Inspired by [DavidWells/markdown-magic](https://github.com/DavidWells/markdown-magic).
+[^1]: Inspired by [DavidWells/markdown-magic](https://github.com/DavidWells/markdown-magic).
```

### Comparing `mdup-0.1.0/mdup/mdup.py` & `mdup-0.1.1/mdup/mdup.py`

 * *Files identical despite different names*

### Comparing `mdup-0.1.0/pyproject.toml` & `mdup-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "mdup"
-version = "0.1.0"
+version = "0.1.1"
+homepage = "https://github.com/alexandru-dinu/mdup"
 description = "Keep markdown files up-to-date."
 authors = ["Alexandru Dinu <alex.dinu07@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "mdup"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
-
+python = ">=3.8"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.263"
 autoflake = "^2.1.1"
 isort = "^5.12.0"
 black = "^23.3.0"
 mypy = "^1.2.0"
@@ -30,10 +30,13 @@
     "B", # flake8-bugbear
     "SIM", # flake8-simplify
 ]
 ignore = [
     "E501",  # line too long, handled by black
 ]
 
+[tool.isort]
+profile = "black"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mdup-0.1.0/PKG-INFO` & `mdup-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 Metadata-Version: 2.1
 Name: mdup
-Version: 0.1.0
+Version: 0.1.1
 Summary: Keep markdown files up-to-date.
+Home-page: https://github.com/alexandru-dinu/mdup
 License: MIT
 Author: Alexandru Dinu
 Author-email: alex.dinu07@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # `mdup`
 
 [![Build](https://github.com/alexandru-dinu/mdup/actions/workflows/main.yml/badge.svg)](https://github.com/alexandru-dinu/mdup/actions/workflows/main.yml)
 
 Keep markdown files up-to-date by injecting code or script output between special blocks.
 
 There are no external dependencies, i.e. apart from Python stdlib.
 
+## Install
+
+```
+pip install mdup
+```
+
 ## How does it work?
 
 The blocks are defined using HTML comments.
 Specifically, the **begin** block is of the form:
 
     <!-- MDUP:BEG ({CMD}:{CONTENTS}) -->
 
@@ -32,15 +41,15 @@
 - `RUN`: to execute the script from `{CONTENTS}` and inject its stdout in the block
 
 **NOTES**
 - For `SRC` and `RUN` commands, the `{CONTENTS}` must be a path, relative to the md file.
 - The blocks must be defined as the sole contents of the line, i.e. matching `^` and `$` anchors.
 
 ## Usage
-<!-- MDUP:BEG (RUN:./help.sh) -->
+<!-- MDUP:BEG (RUN:./scripts/help.sh) -->
 ```
 usage: mdup [-h] -i INPUT [-o OUTPUT]
 
 options:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         Input file.
@@ -52,13 +61,14 @@
 Running `mdup -i <input.md> -o <output.md>` will replace the contents between each block
 with the appropriate action as defined above. This means that you can keep files up-to-date by simply rerunning `mdup`.
 
 Omitting the `-o` option will edit the file in-place.
 
 For example, the cmdline usage block above is automatically generated by defining:
 
-    <!-- MDUP:BEG (RUN:./help.sh) -->
+    <!-- MDUP:BEG (RUN:./scripts/help.sh) -->
     <!-- MDUP:END -->
 
-then running `mdup -i README.md`
+then running `mdup -i README.md`.
 
 [^1]: Inspired by [DavidWells/markdown-magic](https://github.com/DavidWells/markdown-magic).
+
```


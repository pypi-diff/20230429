# Comparing `tmp/lammps-manylinux-2-28-2022.6.23.3.1.tar.gz` & `tmp/lammps-manylinux-2-28-2022.6.23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lammps-manylinux-2-28-2022.6.23.3.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "lammps-manylinux-2-28-2022.6.23.4.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `lammps-manylinux-2-28-2022.6.23.3.1.tar` & `lammps-manylinux-2-28-2022.6.23.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      382 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.3.1/.github/workflows/build.yml
--rw-r--r--   0        0        0     2435 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.3.1/.github/workflows/wheel.yml
--rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.3.1/CMakeLists.txt
--rw-r--r--   0        0        0    18059 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.3.1/LICENSE
--rw-r--r--   0        0        0      168 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.3.1/README.md
--rw-r--r--   0        0        0      524 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.3.1/lammps/__init__.py
--rw-r--r--   0        0        0      925 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.3.1/lammps/executable.py
--rw-r--r--   0        0        0     2231 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.3.1/pyproject.toml
--rw-r--r--   0        0        0       27 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.3.1/tests/test_import.py
--rw-r--r--   0        0        0    21497 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.3.1/PKG-INFO
+-rw-r--r--   0        0        0      382 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.4.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2435 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.4.0/.github/workflows/wheel.yml
+-rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.4.0/CMakeLists.txt
+-rw-r--r--   0        0        0    18059 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.4.0/LICENSE
+-rw-r--r--   0        0        0      168 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.4.0/README.md
+-rw-r--r--   0        0        0      524 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.4.0/lammps/__init__.py
+-rw-r--r--   0        0        0      925 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.4.0/lammps/executable.py
+-rw-r--r--   0        0        0     2231 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.4.0/pyproject.toml
+-rw-r--r--   0        0        0       27 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.4.0/tests/test_import.py
+-rw-r--r--   0        0        0    21497 2022-11-09 12:37:21.000000 lammps-manylinux-2-28-2022.6.23.4.0/PKG-INFO
```

### Comparing `lammps-manylinux-2-28-2022.6.23.3.1/.github/workflows/wheel.yml` & `lammps-manylinux-2-28-2022.6.23.4.0/.github/workflows/wheel.yml`

 * *Files identical despite different names*

### Comparing `lammps-manylinux-2-28-2022.6.23.3.1/CMakeLists.txt` & `lammps-manylinux-2-28-2022.6.23.4.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `lammps-manylinux-2-28-2022.6.23.3.1/LICENSE` & `lammps-manylinux-2-28-2022.6.23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lammps-manylinux-2-28-2022.6.23.3.1/lammps/__init__.py` & `lammps-manylinux-2-28-2022.6.23.4.0/lammps/__init__.py`

 * *Files identical despite different names*

### Comparing `lammps-manylinux-2-28-2022.6.23.3.1/lammps/executable.py` & `lammps-manylinux-2-28-2022.6.23.4.0/lammps/executable.py`

 * *Files identical despite different names*

### Comparing `lammps-manylinux-2-28-2022.6.23.3.1/pyproject.toml` & `lammps-manylinux-2-28-2022.6.23.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["scikit-build-core>=0.1.4"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "lammps_manylinux_2_28"
-version = "2022.6.23.3.1"
+version = "2022.6.23.4.0"
 description = "unoffical LAMMPS Molecular Dynamics Python package"
 authors = [
   {name = "The LAMMPS Developers", email = "developers@lammps.org"},
   {name = "Jinzhe Zeng", email = "jinzhe.zeng@rutgers.edu"},
 ]
 license = {file = "LICENSE"}
 classifiers = [
@@ -33,15 +33,15 @@
 [project.scripts]
 lmp = "lammps.executable:lmp"
 
 [tool.scikit-build]
 wheel.install-dir = "lammps"
 wheel.py-api = "py2.py3"
 cmake.args = [
-    "-D LAMMPS_VERSION=8160bfb589fad2c27e4af350e1c8981c4f901b23",
+    "-D LAMMPS_VERSION=93fc33a5504ff56186c266926490d32d3ed2b700",
     "-D LAMMPS_EXCEPTIONS=ON",
     "-D BUILD_SHARED_LIBS=ON",
 ]
 
 [tool.cibuildwheel]
 build = ["cp311-*"]
 skip = ["*-win32", "*-manylinux_i686", "*-musllinux*"]
```

### Comparing `lammps-manylinux-2-28-2022.6.23.3.1/PKG-INFO` & `lammps-manylinux-2-28-2022.6.23.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lammps-manylinux-2-28
-Version: 2022.6.23.3.1
+Version: 2022.6.23.4.0
 Summary: unoffical LAMMPS Molecular Dynamics Python package
 Keywords: lammps
 Author-Email: The LAMMPS Developers <developers@lammps.org>, Jinzhe Zeng <jinzhe.zeng@rutgers.edu>
 License: GNU GENERAL PUBLIC LICENSE
         
         Version 2, June 1991
```


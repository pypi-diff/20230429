# Comparing `tmp/pyift-0.0.6.tar.gz` & `tmp/pyift-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyift-0.0.6.tar", last modified: Wed Nov 10 05:26:02 2021, max compression
+gzip compressed data, was "pyift-0.1.0.tar", last modified: Sat Apr 29 05:22:14 2023, max compression
```

## Comparing `pyift-0.0.6.tar` & `pyift-0.1.0.tar`

### file list

```diff
@@ -1,63 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 05:26:02.838008 pyift-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-11-10 05:25:48.000000 pyift-0.0.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 05:26:02.830008 pyift-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 05:26:02.830008 pyift-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2126 2021-11-10 05:25:48.000000 pyift-0.0.6/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      715 2021-11-10 05:25:48.000000 pyift-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      257 2021-11-10 05:25:48.000000 pyift-0.0.6/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 05:26:02.834009 pyift-0.0.6/.travis/
--rwxr-xr-x   0 runner    (1001) docker     (121)      150 2021-11-10 05:25:48.000000 pyift-0.0.6/.travis/install.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)       45 2021-11-10 05:25:48.000000 pyift-0.0.6/.travis/test.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2021-11-10 05:25:48.000000 pyift-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       60 2021-11-10 05:25:48.000000 pyift-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1949 2021-11-10 05:26:02.838008 pyift-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2021-11-10 05:25:48.000000 pyift-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-11-10 05:25:48.000000 pyift-0.0.6/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 05:26:02.834009 pyift-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2021-11-10 05:25:48.000000 pyift-0.0.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      799 2021-11-10 05:25:48.000000 pyift-0.0.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-11-10 05:25:48.000000 pyift-0.0.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 05:26:02.834009 pyift-0.0.6/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2021-11-10 05:25:48.000000 pyift-0.0.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      280 2021-11-10 05:25:48.000000 pyift-0.0.6/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       95 2021-11-10 05:25:48.000000 pyift-0.0.6/docs/source/livewire.rst
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-11-10 05:25:48.000000 pyift-0.0.6/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)      287 2021-11-10 05:25:48.000000 pyift-0.0.6/docs/source/shortestpath.rst
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-11-10 05:26:02.838008 pyift-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2959 2021-11-10 05:25:48.000000 pyift-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 05:26:02.830008 pyift-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 05:26:02.834009 pyift-0.0.6/src/libift/
--rw-r--r--   0 runner    (1001) docker     (121)     5059 2021-11-10 05:25:48.000000 pyift-0.0.6/src/libift/adjacency.c
--rw-r--r--   0 runner    (1001) docker     (121)      776 2021-11-10 05:25:48.000000 pyift-0.0.6/src/libift/adjacency.h
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 05:25:48.000000 pyift-0.0.6/src/libift/core.c
--rw-r--r--   0 runner    (1001) docker     (121)      893 2021-11-10 05:25:48.000000 pyift-0.0.6/src/libift/core.h
--rw-r--r--   0 runner    (1001) docker     (121)     4916 2021-11-10 05:25:48.000000 pyift-0.0.6/src/libift/heap.c
--rw-r--r--   0 runner    (1001) docker     (121)      984 2021-11-10 05:25:48.000000 pyift-0.0.6/src/libift/heap.h
--rw-r--r--   0 runner    (1001) docker     (121)      936 2021-11-10 05:25:48.000000 pyift-0.0.6/src/libift/set.c
--rw-r--r--   0 runner    (1001) docker     (121)      356 2021-11-10 05:25:48.000000 pyift-0.0.6/src/libift/set.h
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2021-11-10 05:25:48.000000 pyift-0.0.6/src/libift/sort.c
--rw-r--r--   0 runner    (1001) docker     (121)      280 2021-11-10 05:25:48.000000 pyift-0.0.6/src/libift/sort.h
--rw-r--r--   0 runner    (1001) docker     (121)     2118 2021-11-10 05:25:48.000000 pyift-0.0.6/src/libift/tags
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 05:26:02.834009 pyift-0.0.6/src/pyift/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-11-10 05:25:48.000000 pyift-0.0.6/src/pyift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-11-10 05:26:02.000000 pyift-0.0.6/src/pyift/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     8592 2021-11-10 05:25:48.000000 pyift-0.0.6/src/pyift/livewire.py
--rw-r--r--   0 runner    (1001) docker     (121)    16575 2021-11-10 05:25:48.000000 pyift-0.0.6/src/pyift/shortestpath.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 05:26:02.834009 pyift-0.0.6/src/pyift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1949 2021-11-10 05:26:02.000000 pyift-0.0.6/src/pyift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2021-11-10 05:26:02.000000 pyift-0.0.6/src/pyift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-10 05:26:02.000000 pyift-0.0.6/src/pyift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-11-10 05:26:02.000000 pyift-0.0.6/src/pyift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-11-10 05:26:02.000000 pyift-0.0.6/src/pyift.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 05:26:02.834009 pyift-0.0.6/src/pyift_c_ext/
--rw-r--r--   0 runner    (1001) docker     (121)     5844 2021-11-10 05:25:48.000000 pyift-0.0.6/src/pyift_c_ext/_livewire.c
--rw-r--r--   0 runner    (1001) docker     (121)      656 2021-11-10 05:25:48.000000 pyift-0.0.6/src/pyift_c_ext/_livewire.h
--rw-r--r--   0 runner    (1001) docker     (121)     5890 2021-11-10 05:25:48.000000 pyift-0.0.6/src/pyift_c_ext/_pyift.c
--rw-r--r--   0 runner    (1001) docker     (121)    39029 2021-11-10 05:25:48.000000 pyift-0.0.6/src/pyift_c_ext/_shortestpath.c
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2021-11-10 05:25:48.000000 pyift-0.0.6/src/pyift_c_ext/_shortestpath.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 05:26:02.834009 pyift-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 05:25:48.000000 pyift-0.0.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 05:26:02.838008 pyift-0.0.6/tests/pyift/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 05:25:48.000000 pyift-0.0.6/tests/pyift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2021-11-10 05:25:48.000000 pyift-0.0.6/tests/pyift/test_livewire.py
--rw-r--r--   0 runner    (1001) docker     (121)    11881 2021-11-10 05:25:48.000000 pyift-0.0.6/tests/pyift/test_shortestpath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:22:14.488214 pyift-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-29 05:22:01.000000 pyift-0.1.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:22:14.480214 pyift-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:22:14.484214 pyift-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-29 05:22:01.000000 pyift-0.1.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-29 05:22:01.000000 pyift-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-29 05:22:01.000000 pyift-0.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-29 05:22:01.000000 pyift-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-29 05:22:01.000000 pyift-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-29 05:22:14.488214 pyift-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-29 05:22:01.000000 pyift-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-29 05:22:01.000000 pyift-0.1.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:22:14.484214 pyift-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-29 05:22:01.000000 pyift-0.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-29 05:22:01.000000 pyift-0.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-29 05:22:01.000000 pyift-0.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:22:14.484214 pyift-0.1.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-29 05:22:01.000000 pyift-0.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-29 05:22:01.000000 pyift-0.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-29 05:22:01.000000 pyift-0.1.0/docs/source/livewire.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 05:22:01.000000 pyift-0.1.0/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-29 05:22:01.000000 pyift-0.1.0/docs/source/shortestpath.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-29 05:22:14.488214 pyift-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-29 05:22:01.000000 pyift-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:22:14.484214 pyift-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:22:14.488214 pyift-0.1.0/src/libift/
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-29 05:22:01.000000 pyift-0.1.0/src/libift/adjacency.c
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-29 05:22:01.000000 pyift-0.1.0/src/libift/adjacency.h
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 05:22:01.000000 pyift-0.1.0/src/libift/core.c
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-29 05:22:01.000000 pyift-0.1.0/src/libift/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-04-29 05:22:01.000000 pyift-0.1.0/src/libift/heap.c
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-29 05:22:01.000000 pyift-0.1.0/src/libift/heap.h
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-29 05:22:01.000000 pyift-0.1.0/src/libift/set.c
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-29 05:22:01.000000 pyift-0.1.0/src/libift/set.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-29 05:22:01.000000 pyift-0.1.0/src/libift/sort.c
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-29 05:22:01.000000 pyift-0.1.0/src/libift/sort.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-29 05:22:01.000000 pyift-0.1.0/src/libift/tags
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:22:14.488214 pyift-0.1.0/src/pyift/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-29 05:22:01.000000 pyift-0.1.0/src/pyift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-29 05:22:14.000000 pyift-0.1.0/src/pyift/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-04-29 05:22:01.000000 pyift-0.1.0/src/pyift/livewire.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-04-29 05:22:01.000000 pyift-0.1.0/src/pyift/shortestpath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:22:14.488214 pyift-0.1.0/src/pyift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-29 05:22:14.000000 pyift-0.1.0/src/pyift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-29 05:22:14.000000 pyift-0.1.0/src/pyift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 05:22:14.000000 pyift-0.1.0/src/pyift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 05:22:14.000000 pyift-0.1.0/src/pyift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 05:22:14.000000 pyift-0.1.0/src/pyift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:22:14.488214 pyift-0.1.0/src/pyift_c_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-04-29 05:22:01.000000 pyift-0.1.0/src/pyift_c_ext/_livewire.c
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-29 05:22:01.000000 pyift-0.1.0/src/pyift_c_ext/_livewire.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-04-29 05:22:01.000000 pyift-0.1.0/src/pyift_c_ext/_pyift.c
+-rw-r--r--   0 runner    (1001) docker     (123)    39029 2023-04-29 05:22:01.000000 pyift-0.1.0/src/pyift_c_ext/_shortestpath.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-29 05:22:01.000000 pyift-0.1.0/src/pyift_c_ext/_shortestpath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:22:14.488214 pyift-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 05:22:01.000000 pyift-0.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:22:14.488214 pyift-0.1.0/tests/pyift/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 05:22:01.000000 pyift-0.1.0/tests/pyift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-29 05:22:01.000000 pyift-0.1.0/tests/pyift/test_livewire.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-04-29 05:22:01.000000 pyift-0.1.0/tests/pyift/test_shortestpath.py
```

### Comparing `pyift-0.0.6/.github/workflows/test_and_deploy.yml` & `pyift-0.1.0/.github/workflows/test_and_deploy.yml`

 * *Files 6% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 
 jobs:
   test:
     name: ${{ matrix.platform }} py${{ matrix.python-version }}
     runs-on: ${{ matrix.platform }}
     strategy:
       matrix:
-        platform: [ubuntu-latest, macos-latest]
-        python-version: [3.7, 3.8, 3.9]
+        platform: [ubuntu-latest, macos-latest]  # windows-latest
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - uses: actions/checkout@v2
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install setuptools codecov pytest-cov flake8
-          python setup.py install
+          pip install .
 
       - name: Lint code
         run: python -m flake8 src tests setup.py
 
       - name: Test and coverage
         run: python -m pytest --cov && codecov
         env:
@@ -67,8 +67,8 @@
       - name: Build and publish
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.TWINE_API_KEY }}
         run: |
           git tag
           python setup.py sdist
-          twine upload dist/*
+          twine upload dist/*
```

### Comparing `pyift-0.0.6/.gitignore` & `pyift-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/LICENSE` & `pyift-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/PKG-INFO` & `pyift-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: pyift
-Version: 0.0.6
+Version: 0.1.0
 Summary: Python Image Foresting Transform Library
 Home-page: https://github.com/pyift/pyift
 Author: Jordao Bragantini
 Author-email: jordao.bragantini+pyift@gmail.com
 License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyIFT
 
-[![Build Status](https://api.travis-ci.org/PyIFT/pyift.svg?branch=master)](https://travis-ci.com/github/PyIFT/pyift)
+[![PyPI](https://img.shields.io/pypi/v/pyift?color=green)](https://pypi.org/project/pyift)
+[![Python Version](https://img.shields.io/pypi/pyversions/pyift.svg?color=green)](https://python.org)
+[![tests](https://github.com/PyIFT/pyift/workflows/tests/badge.svg)](https://github.com/PyIFT/pyift/actions)
 [![codecov](https://codecov.io/gh/PyIFT/pyift/branch/master/graph/badge.svg)](https://codecov.io/gh/PyIFT/pyift)
 [![Documentation Status](https://readthedocs.org/projects/pyift/badge/?version=latest)](https://pyift.readthedocs.io/en/latest)
 
 ## Python Image Foresting Transform Library
 
 PyIFT is a Python wrapper of a fork of the [LIDS](http://lids.ic.unicamp.br/) C library.
 
@@ -53,9 +59,7 @@
   volume={26},
   number={1},
   pages={19--29},
   year={2004},
   publisher={IEEE}
 }
 ```
-
-
```

### Comparing `pyift-0.0.6/README.md` & `pyift-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # PyIFT
 
-[![Build Status](https://api.travis-ci.org/PyIFT/pyift.svg?branch=master)](https://travis-ci.com/github/PyIFT/pyift)
+[![PyPI](https://img.shields.io/pypi/v/pyift?color=green)](https://pypi.org/project/pyift)
+[![Python Version](https://img.shields.io/pypi/pyversions/pyift.svg?color=green)](https://python.org)
+[![tests](https://github.com/PyIFT/pyift/workflows/tests/badge.svg)](https://github.com/PyIFT/pyift/actions)
 [![codecov](https://codecov.io/gh/PyIFT/pyift/branch/master/graph/badge.svg)](https://codecov.io/gh/PyIFT/pyift)
 [![Documentation Status](https://readthedocs.org/projects/pyift/badge/?version=latest)](https://pyift.readthedocs.io/en/latest)
 
 ## Python Image Foresting Transform Library
 
 PyIFT is a Python wrapper of a fork of the [LIDS](http://lids.ic.unicamp.br/) C library.
```

### Comparing `pyift-0.0.6/docs/Makefile` & `pyift-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/docs/make.bat` & `pyift-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/docs/source/conf.py` & `pyift-0.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/src/libift/adjacency.c` & `pyift-0.1.0/src/libift/adjacency.c`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/src/libift/adjacency.h` & `pyift-0.1.0/src/libift/adjacency.h`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/src/libift/core.h` & `pyift-0.1.0/src/libift/core.h`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/src/libift/heap.c` & `pyift-0.1.0/src/libift/heap.c`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/src/libift/heap.h` & `pyift-0.1.0/src/libift/heap.h`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/src/libift/set.c` & `pyift-0.1.0/src/libift/set.c`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/src/libift/sort.c` & `pyift-0.1.0/src/libift/sort.c`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/src/libift/tags` & `pyift-0.1.0/src/libift/tags`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/src/pyift/livewire.py` & `pyift-0.1.0/src/pyift/livewire.py`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/src/pyift/shortestpath.py` & `pyift-0.1.0/src/pyift/shortestpath.py`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/src/pyift.egg-info/PKG-INFO` & `pyift-0.1.0/src/pyift.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: pyift
-Version: 0.0.6
+Version: 0.1.0
 Summary: Python Image Foresting Transform Library
 Home-page: https://github.com/pyift/pyift
 Author: Jordao Bragantini
 Author-email: jordao.bragantini+pyift@gmail.com
 License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyIFT
 
-[![Build Status](https://api.travis-ci.org/PyIFT/pyift.svg?branch=master)](https://travis-ci.com/github/PyIFT/pyift)
+[![PyPI](https://img.shields.io/pypi/v/pyift?color=green)](https://pypi.org/project/pyift)
+[![Python Version](https://img.shields.io/pypi/pyversions/pyift.svg?color=green)](https://python.org)
+[![tests](https://github.com/PyIFT/pyift/workflows/tests/badge.svg)](https://github.com/PyIFT/pyift/actions)
 [![codecov](https://codecov.io/gh/PyIFT/pyift/branch/master/graph/badge.svg)](https://codecov.io/gh/PyIFT/pyift)
 [![Documentation Status](https://readthedocs.org/projects/pyift/badge/?version=latest)](https://pyift.readthedocs.io/en/latest)
 
 ## Python Image Foresting Transform Library
 
 PyIFT is a Python wrapper of a fork of the [LIDS](http://lids.ic.unicamp.br/) C library.
 
@@ -53,9 +59,7 @@
   volume={26},
   number={1},
   pages={19--29},
   year={2004},
   publisher={IEEE}
 }
 ```
-
-
```

### Comparing `pyift-0.0.6/src/pyift.egg-info/SOURCES.txt` & `pyift-0.1.0/src/pyift.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 LICENSE
 MANIFEST.in
 README.md
 codecov.yml
 setup.cfg
 setup.py
 .github/workflows/test_and_deploy.yml
-.travis/install.sh
-.travis/test.sh
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
 docs/source/conf.py
 docs/source/index.rst
 docs/source/livewire.rst
 docs/source/readme.rst
```

### Comparing `pyift-0.0.6/src/pyift_c_ext/_livewire.c` & `pyift-0.1.0/src/pyift_c_ext/_livewire.c`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/src/pyift_c_ext/_livewire.h` & `pyift-0.1.0/src/pyift_c_ext/_livewire.h`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/src/pyift_c_ext/_pyift.c` & `pyift-0.1.0/src/pyift_c_ext/_pyift.c`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/src/pyift_c_ext/_shortestpath.c` & `pyift-0.1.0/src/pyift_c_ext/_shortestpath.c`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/src/pyift_c_ext/_shortestpath.h` & `pyift-0.1.0/src/pyift_c_ext/_shortestpath.h`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/tests/pyift/test_livewire.py` & `pyift-0.1.0/tests/pyift/test_livewire.py`

 * *Files identical despite different names*

### Comparing `pyift-0.0.6/tests/pyift/test_shortestpath.py` & `pyift-0.1.0/tests/pyift/test_shortestpath.py`

 * *Files identical despite different names*


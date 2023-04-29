# Comparing `tmp/tinyshap-0.0.1.tar.gz` & `tmp/tinyshap-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyshap-0.0.1.tar", last modified: Mon Apr 24 17:47:20 2023, max compression
+gzip compressed data, was "C:\Users\user\Documents\tinyshap\dist\.tmp-jo1bxdz_\tinyshap-0.0.3.tar", last modified: Sat Apr 29 17:29:45 2023, max compression
```

## Comparing `tinyshap-0.0.1.tar` & `tinyshap-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 17:47:20.580622 tinyshap-0.0.1/
--rw-rw-rw-   0        0        0     1086 2023-04-09 14:34:23.000000 tinyshap-0.0.1/LICENCE
--rw-rw-rw-   0        0        0      835 2023-04-24 17:47:20.578626 tinyshap-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-09 14:34:58.000000 tinyshap-0.0.1/README.md
--rw-rw-rw-   0        0        0     1076 2023-04-24 17:46:55.000000 tinyshap-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 17:47:20.580622 tinyshap-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 17:47:20.574627 tinyshap-0.0.1/tinyshap.egg-info/
--rw-rw-rw-   0        0        0      835 2023-04-24 17:47:20.000000 tinyshap-0.0.1/tinyshap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-04-24 17:47:20.000000 tinyshap-0.0.1/tinyshap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 17:47:20.000000 tinyshap-0.0.1/tinyshap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-24 17:47:20.000000 tinyshap-0.0.1/tinyshap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 17:47:20.000000 tinyshap-0.0.1/tinyshap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 17:29:45.984774 tinyshap-0.0.3/
+-rw-rw-rw-   0        0        0     1089 2023-04-29 16:41:09.000000 tinyshap-0.0.3/LICENCE
+-rw-rw-rw-   0        0        0     1995 2023-04-29 17:29:45.983767 tinyshap-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1094 2023-04-29 17:08:30.000000 tinyshap-0.0.3/README.md
+-rw-rw-rw-   0        0        0     1166 2023-04-29 17:29:05.000000 tinyshap-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 17:29:45.985769 tinyshap-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 17:29:45.980770 tinyshap-0.0.3/tinyshap.egg-info/
+-rw-rw-rw-   0        0        0     1995 2023-04-29 17:29:45.000000 tinyshap-0.0.3/tinyshap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-04-29 17:29:45.000000 tinyshap-0.0.3/tinyshap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 17:29:45.000000 tinyshap-0.0.3/tinyshap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-29 17:29:45.000000 tinyshap-0.0.3/tinyshap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-29 17:29:45.000000 tinyshap-0.0.3/tinyshap.egg-info/top_level.txt
```

### Comparing `tinyshap-0.0.1/LICENCE` & `tinyshap-0.0.3/LICENCE`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-The MIT License (MIT) Copyright (c) 2020 Andrej Karpathy
+The MIT License (MIT) Copyright (c) 2023 Theodore Tsitsimis
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```


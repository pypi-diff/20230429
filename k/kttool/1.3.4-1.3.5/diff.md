# Comparing `tmp/kttool-1.3.4.tar.gz` & `tmp/kttool-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kttool-1.3.4.tar", last modified: Sun Jan  8 15:02:14 2023, max compression
+gzip compressed data, was "dist/kttool-1.3.5.tar", last modified: Sat Apr 29 07:00:27 2023, max compression
```

## Comparing `kttool-1.3.4.tar` & `kttool-1.3.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 heiseish  (1000) heiseish  (1000)        0 2023-01-08 15:02:14.000000 kttool-1.3.4/
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     1065 2022-12-25 11:12:17.000000 kttool-1.3.4/LICENSE
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     3487 2023-01-08 15:02:14.000000 kttool-1.3.4/PKG-INFO
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     2916 2023-01-05 12:53:08.000000 kttool-1.3.4/README.md
--rwxrwxr-x   0 heiseish  (1000) heiseish  (1000)      491 2022-12-25 10:41:51.000000 kttool-1.3.4/kt
-drwxrwxr-x   0 heiseish  (1000) heiseish  (1000)        0 2023-01-08 15:02:14.000000 kttool-1.3.4/kttool/
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)        5 2023-01-08 15:01:47.000000 kttool-1.3.4/kttool/VERSION
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)        0 2022-12-25 11:14:21.000000 kttool-1.3.4/kttool/__init__.py
-drwxrwxr-x   0 heiseish  (1000) heiseish  (1000)        0 2023-01-08 15:02:14.000000 kttool-1.3.4/kttool/actions/
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)        0 2022-12-25 11:14:21.000000 kttool-1.3.4/kttool/actions/__init__.py
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     6238 2023-01-05 12:52:48.000000 kttool-1.3.4/kttool/actions/config.py
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     6325 2023-01-05 12:52:48.000000 kttool-1.3.4/kttool/actions/gen.py
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      901 2022-12-25 11:14:21.000000 kttool-1.3.4/kttool/actions/open.py
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     8568 2023-01-05 12:53:08.000000 kttool-1.3.4/kttool/actions/submit.py
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     3354 2023-01-05 12:52:48.000000 kttool-1.3.4/kttool/actions/surprise.py
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     6511 2023-01-05 12:52:48.000000 kttool-1.3.4/kttool/actions/test.py
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     1173 2023-01-05 12:52:48.000000 kttool-1.3.4/kttool/actions/update.py
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      337 2022-12-25 14:02:38.000000 kttool-1.3.4/kttool/actions/version.py
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     9093 2023-01-08 15:01:44.000000 kttool-1.3.4/kttool/base.py
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      507 2022-12-25 11:14:21.000000 kttool-1.3.4/kttool/context.py
-drwxrwxr-x   0 heiseish  (1000) heiseish  (1000)        0 2023-01-08 15:02:14.000000 kttool-1.3.4/kttool/default_templates/
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)       65 2022-12-07 06:21:56.000000 kttool-1.3.4/kttool/default_templates/template.c
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      138 2022-12-07 06:21:56.000000 kttool-1.3.4/kttool/default_templates/template.cc
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      138 2022-12-07 06:21:56.000000 kttool-1.3.4/kttool/default_templates/template.cpp
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)       66 2022-12-07 06:21:56.000000 kttool-1.3.4/kttool/default_templates/template.go
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      108 2022-12-07 06:21:56.000000 kttool-1.3.4/kttool/default_templates/template.java
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)       21 2022-12-07 06:21:56.000000 kttool-1.3.4/kttool/default_templates/template.js
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)       72 2022-12-25 11:14:21.000000 kttool-1.3.4/kttool/default_templates/template.py
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     5874 2023-01-05 12:53:08.000000 kttool-1.3.4/kttool/default_templates/template.rs
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     1162 2022-12-25 11:14:21.000000 kttool-1.3.4/kttool/logger.py
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     1556 2022-12-25 11:14:21.000000 kttool-1.3.4/kttool/parser.py
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     3781 2022-12-25 11:14:21.000000 kttool-1.3.4/kttool/utils.py
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      111 2022-12-25 11:14:21.000000 kttool-1.3.4/kttool/version.py
-drwxrwxr-x   0 heiseish  (1000) heiseish  (1000)        0 2023-01-08 15:02:14.000000 kttool-1.3.4/kttool.egg-info/
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     3487 2023-01-08 15:02:14.000000 kttool-1.3.4/kttool.egg-info/PKG-INFO
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      851 2023-01-08 15:02:14.000000 kttool-1.3.4/kttool.egg-info/SOURCES.txt
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)        1 2023-01-08 15:02:14.000000 kttool-1.3.4/kttool.egg-info/dependency_links.txt
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      109 2023-01-08 15:02:14.000000 kttool-1.3.4/kttool.egg-info/requires.txt
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)        7 2023-01-08 15:02:14.000000 kttool-1.3.4/kttool.egg-info/top_level.txt
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      108 2022-12-25 05:49:15.000000 kttool-1.3.4/requirements.txt
--rw-rw-r--   0 heiseish  (1000) heiseish  (1000)       38 2023-01-08 15:02:14.000000 kttool-1.3.4/setup.cfg
--rwxrwxr-x   0 heiseish  (1000) heiseish  (1000)     1403 2022-12-25 04:46:47.000000 kttool-1.3.4/setup.py
+drwxrwxr-x   0 heiseish  (1000) heiseish  (1000)        0 2023-04-29 07:00:27.000000 kttool-1.3.5/
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     1065 2022-12-25 11:12:17.000000 kttool-1.3.5/LICENSE
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     3487 2023-04-29 07:00:27.000000 kttool-1.3.5/PKG-INFO
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     2916 2023-01-05 12:53:08.000000 kttool-1.3.5/README.md
+-rwxrwxr-x   0 heiseish  (1000) heiseish  (1000)      491 2022-12-25 10:41:51.000000 kttool-1.3.5/kt
+drwxrwxr-x   0 heiseish  (1000) heiseish  (1000)        0 2023-04-29 07:00:27.000000 kttool-1.3.5/kttool/
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)        5 2023-04-29 06:59:28.000000 kttool-1.3.5/kttool/VERSION
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)        0 2022-12-25 11:14:21.000000 kttool-1.3.5/kttool/__init__.py
+drwxrwxr-x   0 heiseish  (1000) heiseish  (1000)        0 2023-04-29 07:00:27.000000 kttool-1.3.5/kttool/actions/
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)        0 2022-12-25 11:14:21.000000 kttool-1.3.5/kttool/actions/__init__.py
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     6238 2023-01-05 12:52:48.000000 kttool-1.3.5/kttool/actions/config.py
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     6325 2023-01-05 12:52:48.000000 kttool-1.3.5/kttool/actions/gen.py
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      901 2022-12-25 11:14:21.000000 kttool-1.3.5/kttool/actions/open.py
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     8568 2023-01-05 12:53:08.000000 kttool-1.3.5/kttool/actions/submit.py
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     3354 2023-01-05 12:52:48.000000 kttool-1.3.5/kttool/actions/surprise.py
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     6724 2023-04-29 06:59:48.000000 kttool-1.3.5/kttool/actions/test.py
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     1173 2023-01-05 12:52:48.000000 kttool-1.3.5/kttool/actions/update.py
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      337 2022-12-25 14:02:38.000000 kttool-1.3.5/kttool/actions/version.py
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     9093 2023-01-08 15:01:44.000000 kttool-1.3.5/kttool/base.py
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      507 2022-12-25 11:14:21.000000 kttool-1.3.5/kttool/context.py
+drwxrwxr-x   0 heiseish  (1000) heiseish  (1000)        0 2023-04-29 07:00:27.000000 kttool-1.3.5/kttool/default_templates/
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)       65 2022-12-07 06:21:56.000000 kttool-1.3.5/kttool/default_templates/template.c
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      138 2022-12-07 06:21:56.000000 kttool-1.3.5/kttool/default_templates/template.cc
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      138 2022-12-07 06:21:56.000000 kttool-1.3.5/kttool/default_templates/template.cpp
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)       66 2022-12-07 06:21:56.000000 kttool-1.3.5/kttool/default_templates/template.go
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      108 2022-12-07 06:21:56.000000 kttool-1.3.5/kttool/default_templates/template.java
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)       21 2022-12-07 06:21:56.000000 kttool-1.3.5/kttool/default_templates/template.js
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)       72 2022-12-25 11:14:21.000000 kttool-1.3.5/kttool/default_templates/template.py
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     5874 2023-01-05 12:53:08.000000 kttool-1.3.5/kttool/default_templates/template.rs
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     1162 2022-12-25 11:14:21.000000 kttool-1.3.5/kttool/logger.py
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     1556 2022-12-25 11:14:21.000000 kttool-1.3.5/kttool/parser.py
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     3781 2022-12-25 11:14:21.000000 kttool-1.3.5/kttool/utils.py
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      111 2022-12-25 11:14:21.000000 kttool-1.3.5/kttool/version.py
+drwxrwxr-x   0 heiseish  (1000) heiseish  (1000)        0 2023-04-29 07:00:27.000000 kttool-1.3.5/kttool.egg-info/
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)     3487 2023-04-29 07:00:27.000000 kttool-1.3.5/kttool.egg-info/PKG-INFO
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      851 2023-04-29 07:00:27.000000 kttool-1.3.5/kttool.egg-info/SOURCES.txt
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)        1 2023-04-29 07:00:27.000000 kttool-1.3.5/kttool.egg-info/dependency_links.txt
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      109 2023-04-29 07:00:27.000000 kttool-1.3.5/kttool.egg-info/requires.txt
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)        7 2023-04-29 07:00:27.000000 kttool-1.3.5/kttool.egg-info/top_level.txt
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)      108 2022-12-25 05:49:15.000000 kttool-1.3.5/requirements.txt
+-rw-rw-r--   0 heiseish  (1000) heiseish  (1000)       38 2023-04-29 07:00:27.000000 kttool-1.3.5/setup.cfg
+-rwxrwxr-x   0 heiseish  (1000) heiseish  (1000)     1403 2022-12-25 04:46:47.000000 kttool-1.3.5/setup.py
```

### Comparing `kttool-1.3.4/LICENSE` & `kttool-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kttool-1.3.4/PKG-INFO` & `kttool-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kttool
-Version: 1.3.4
+Version: 1.3.5
 Summary: Kattis command line tool
 Home-page: https://github.com/heiseish/kt
 Author: Dao Truong Giang
 Author-email: dtrnggiang@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `kttool-1.3.4/README.md` & `kttool-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `kttool-1.3.4/kttool/actions/config.py` & `kttool-1.3.5/kttool/actions/config.py`

 * *Files identical despite different names*

### Comparing `kttool-1.3.4/kttool/actions/gen.py` & `kttool-1.3.5/kttool/actions/gen.py`

 * *Files identical despite different names*

### Comparing `kttool-1.3.4/kttool/actions/open.py` & `kttool-1.3.5/kttool/actions/open.py`

 * *Files identical despite different names*

### Comparing `kttool-1.3.4/kttool/actions/submit.py` & `kttool-1.3.5/kttool/actions/submit.py`

 * *Files identical despite different names*

### Comparing `kttool-1.3.4/kttool/actions/surprise.py` & `kttool-1.3.5/kttool/actions/surprise.py`

 * *Files identical despite different names*

### Comparing `kttool-1.3.4/kttool/actions/test.py` & `kttool-1.3.5/kttool/actions/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,25 +131,31 @@
             if x.is_file() and x.stem.startswith('ans')
         ]
         usable_samples: List[Sample] = []
 
         in_pattern = re.compile("in(\d+).txt")
         ans_pattern = re.compile("ans(\d+).txt")
         for input_file in input_files:
-            idx = int(in_pattern.search(input_file.name).group(1))
-            for output_file in output_files:
-                if idx == int(ans_pattern.search(output_file.name).group(1)):
-                    usable_samples.append(
-                        Sample(
-                            index=idx,
-                            input_file=Path(input_file).absolute(),
-                            output_file=Path(output_file).absolute()
+            try:
+                idx = int(in_pattern.search(input_file.name).group(1))
+                for output_file in output_files:
+                    if idx == int(
+                        ans_pattern.search(output_file.name).group(1)
+                    ):
+                        usable_samples.append(
+                            Sample(
+                                index=idx,
+                                input_file=Path(input_file).absolute(),
+                                output_file=Path(output_file).absolute()
+                            )
                         )
-                    )
-                    break
+                        break
+            except:
+                ...
+        log(f'{color_green(len(usable_samples))} samples found.')
         # run test from ascending number of file index
         return sorted(usable_samples, key=lambda x: x.index)
 
     def _act(self) -> None:
         """ Run the executable file against sample input and output files present in the folder
         The sample files will only be recognized if the conditions hold:
         - Naming style should be in{idx}.txt and ans{txt}.txt
```

### Comparing `kttool-1.3.4/kttool/actions/update.py` & `kttool-1.3.5/kttool/actions/update.py`

 * *Files identical despite different names*

### Comparing `kttool-1.3.4/kttool/base.py` & `kttool-1.3.5/kttool/base.py`

 * *Files identical despite different names*

### Comparing `kttool-1.3.4/kttool/default_templates/template.rs` & `kttool-1.3.5/kttool/default_templates/template.rs`

 * *Files identical despite different names*

### Comparing `kttool-1.3.4/kttool/logger.py` & `kttool-1.3.5/kttool/logger.py`

 * *Files identical despite different names*

### Comparing `kttool-1.3.4/kttool/parser.py` & `kttool-1.3.5/kttool/parser.py`

 * *Files identical despite different names*

### Comparing `kttool-1.3.4/kttool/utils.py` & `kttool-1.3.5/kttool/utils.py`

 * *Files identical despite different names*

### Comparing `kttool-1.3.4/kttool.egg-info/PKG-INFO` & `kttool-1.3.5/kttool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kttool
-Version: 1.3.4
+Version: 1.3.5
 Summary: Kattis command line tool
 Home-page: https://github.com/heiseish/kt
 Author: Dao Truong Giang
 Author-email: dtrnggiang@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `kttool-1.3.4/kttool.egg-info/SOURCES.txt` & `kttool-1.3.5/kttool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kttool-1.3.4/setup.py` & `kttool-1.3.5/setup.py`

 * *Files identical despite different names*


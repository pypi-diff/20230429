# Comparing `tmp/hhcm_forest-1.1.7.tar.gz` & `tmp/hhcm_forest-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhcm_forest-1.1.7.tar", last modified: Thu Apr 20 15:03:30 2023, max compression
+gzip compressed data, was "hhcm_forest-1.1.8.tar", last modified: Sat Apr 29 18:30:09 2023, max compression
```

## Comparing `hhcm_forest-1.1.7.tar` & `hhcm_forest-1.1.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:03:30.569134 hhcm_forest-1.1.7/
--rw-rw-r--   0 root         (0) root         (0)     1073 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      134 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4760 2023-04-20 15:03:30.569134 hhcm_forest-1.1.7/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4238 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/README.md
--rw-rw-r--   0 root         (0) root         (0)      111 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)      787 2023-04-20 15:03:30.569134 hhcm_forest-1.1.7/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      237 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:03:30.565133 hhcm_forest-1.1.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:03:30.565133 hhcm_forest-1.1.7/src/forest/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       54 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:03:30.565133 hhcm_forest-1.1.7/src/forest/cmake_tools/
--rw-rw-r--   0 root         (0) root         (0)     1649 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/cmake_tools/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1838 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/cmake_tools/_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:03:30.565133 hhcm_forest-1.1.7/src/forest/cmake_tools/template/
--rw-rw-r--   0 root         (0) root         (0)      101 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/cmake_tools/template/find_package.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:03:30.569134 hhcm_forest-1.1.7/src/forest/common/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/common/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8418 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/common/build_handler.py
--rw-rw-r--   0 root         (0) root         (0)      419 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/common/config_handler.py
--rw-rw-r--   0 root         (0) root         (0)     4994 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/common/eval_handler.py
--rw-rw-r--   0 root         (0) root         (0)     7930 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/common/fetch_handler.py
--rw-rw-r--   0 root         (0) root         (0)      206 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/common/forest_dirs.py
--rw-rw-r--   0 root         (0) root         (0)     8100 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/common/install.py
--rw-rw-r--   0 root         (0) root         (0)     3124 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/common/package.py
--rw-rw-r--   0 root         (0) root         (0)     3921 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/common/parser.py
--rw-rw-r--   0 root         (0) root         (0)      923 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/common/print_utils.py
--rw-rw-r--   0 root         (0) root         (0)     4293 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/common/proc_utils.py
--rw-rw-r--   0 root         (0) root         (0)     5000 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/common/recipe.py
--rw-rw-r--   0 root         (0) root         (0)      683 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/common/setup.bash
--rw-rw-r--   0 root         (0) root         (0)     1842 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/common/sudo_refresh.py
--rw-rw-r--   0 root         (0) root         (0)       45 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/forest.bash
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:03:30.569134 hhcm_forest-1.1.7/src/forest/git_tools/
--rw-rw-r--   0 root         (0) root         (0)     2398 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/git_tools/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/git_tools/_impl.py
--rwxrwxr-x   0 root         (0) root         (0)     9830 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/src/forest/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:03:30.569134 hhcm_forest-1.1.7/src/hhcm_forest.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4760 2023-04-20 15:03:30.000000 hhcm_forest-1.1.7/src/hhcm_forest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2023-04-20 15:03:30.000000 hhcm_forest-1.1.7/src/hhcm_forest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 15:03:30.000000 hhcm_forest-1.1.7/src/hhcm_forest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-20 15:03:30.000000 hhcm_forest-1.1.7/src/hhcm_forest.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-20 15:03:30.000000 hhcm_forest-1.1.7/src/hhcm_forest.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-20 15:03:30.000000 hhcm_forest-1.1.7/src/hhcm_forest.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:03:30.569134 hhcm_forest-1.1.7/test/
--rw-rw-r--   0 root         (0) root         (0)      703 2023-04-20 15:01:25.000000 hhcm_forest-1.1.7/test/test_run_bash_tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:30:09.077353 hhcm_forest-1.1.8/
+-rw-rw-r--   0 root         (0) root         (0)     1073 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      134 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4760 2023-04-29 18:30:09.077353 hhcm_forest-1.1.8/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4238 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/README.md
+-rw-rw-r--   0 root         (0) root         (0)      111 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)      787 2023-04-29 18:30:09.081354 hhcm_forest-1.1.8/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      237 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:30:09.073353 hhcm_forest-1.1.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:30:09.077353 hhcm_forest-1.1.8/src/forest/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       54 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:30:09.077353 hhcm_forest-1.1.8/src/forest/cmake_tools/
+-rw-rw-r--   0 root         (0) root         (0)     1649 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/cmake_tools/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1959 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/cmake_tools/_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:30:09.077353 hhcm_forest-1.1.8/src/forest/cmake_tools/template/
+-rw-rw-r--   0 root         (0) root         (0)      101 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/cmake_tools/template/find_package.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:30:09.077353 hhcm_forest-1.1.8/src/forest/common/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8418 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/build_handler.py
+-rw-rw-r--   0 root         (0) root         (0)      419 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/config_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     4994 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/eval_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     7930 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/fetch_handler.py
+-rw-rw-r--   0 root         (0) root         (0)      206 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/forest_dirs.py
+-rw-rw-r--   0 root         (0) root         (0)     8048 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/install.py
+-rw-rw-r--   0 root         (0) root         (0)     3124 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/package.py
+-rw-rw-r--   0 root         (0) root         (0)     3921 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/parser.py
+-rw-rw-r--   0 root         (0) root         (0)      923 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/print_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4102 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/proc_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     5000 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/recipe.py
+-rw-rw-r--   0 root         (0) root         (0)      683 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/setup.bash
+-rw-rw-r--   0 root         (0) root         (0)     1842 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/sudo_refresh.py
+-rw-rw-r--   0 root         (0) root         (0)       45 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/forest.bash
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:30:09.077353 hhcm_forest-1.1.8/src/forest/git_tools/
+-rw-rw-r--   0 root         (0) root         (0)     2328 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/git_tools/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/git_tools/_impl.py
+-rwxrwxr-x   0 root         (0) root         (0)     9831 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:30:09.077353 hhcm_forest-1.1.8/src/hhcm_forest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4760 2023-04-29 18:30:08.000000 hhcm_forest-1.1.8/src/hhcm_forest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-04-29 18:30:09.000000 hhcm_forest-1.1.8/src/hhcm_forest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 18:30:08.000000 hhcm_forest-1.1.8/src/hhcm_forest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-29 18:30:08.000000 hhcm_forest-1.1.8/src/hhcm_forest.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-29 18:30:08.000000 hhcm_forest-1.1.8/src/hhcm_forest.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-29 18:30:09.000000 hhcm_forest-1.1.8/src/hhcm_forest.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:30:09.077353 hhcm_forest-1.1.8/test/
+-rw-rw-r--   0 root         (0) root         (0)      703 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/test/test_run_bash_tests.py
```

### Comparing `hhcm_forest-1.1.7/LICENSE` & `hhcm_forest-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.7/PKG-INFO` & `hhcm_forest-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhcm_forest
-Version: 1.1.7
+Version: 1.1.8
 Summary: A minimalistic tool to automate source code cloning and building
 Home-page: https://none
 Author: Arturo Laurenzi
 Author-email: arturo.laurenzi@iit.it
 License: UNKNOWN
 Project-URL: Bug Tracker, https://none
 Platform: UNKNOWN
```

### Comparing `hhcm_forest-1.1.7/README.md` & `hhcm_forest-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.7/setup.cfg` & `hhcm_forest-1.1.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hhcm_forest
-version = 1.1.7
+version = 1.1.8
 author = Arturo Laurenzi
 author_email = arturo.laurenzi@iit.it
 description = A minimalistic tool to automate source code cloning and building
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://none
 project_urls =
```

### Comparing `hhcm_forest-1.1.7/src/forest/cmake_tools/__init__.py` & `hhcm_forest-1.1.8/src/forest/cmake_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.7/src/forest/cmake_tools/_impl.py` & `hhcm_forest-1.1.8/src/forest/cmake_tools/_impl.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,24 +27,25 @@
         args = list()
 
     return _call_cmake([self.srcdir] + args + default_args, cwd=self.builddir)
     
 
 def _build(self, target, jobs):
 
-    return _call_cmake(['--build', self.builddir, '--target', target, '--', '-j', jobs])
+    return _call_cmake(['--build', self.builddir, '--target', target, '--', '-j', jobs], print_progress=True)
 
 
-def _call_cmake(args, cwd='.', print_on_error=True):
+def _call_cmake(args, cwd='.', print_on_error=True, print_progress=False):
 
     args_str = list(map(str, args))
+    update_regrex_pattern = make_regrex_pattern if print_progress else None
     return proc_utils.call_process(args=[cmake_command] + args_str,
                                    cwd=cwd, 
                                    print_on_error=print_on_error,
-                                   update_regrex_pattern=make_regrex_pattern)
+                                   update_regrex_pattern=update_regrex_pattern)
 
 
 def _find_package(pkg_name: str):
         
     with TemporaryDirectory(prefix="foresttmp-") as tmpdir:
 
         # dir of current file
```

### Comparing `hhcm_forest-1.1.7/src/forest/common/build_handler.py` & `hhcm_forest-1.1.8/src/forest/common/build_handler.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.7/src/forest/common/eval_handler.py` & `hhcm_forest-1.1.8/src/forest/common/eval_handler.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.7/src/forest/common/fetch_handler.py` & `hhcm_forest-1.1.8/src/forest/common/fetch_handler.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.7/src/forest/common/install.py` & `hhcm_forest-1.1.8/src/forest/common/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,14 @@
             if not _remove_fname(pkg.name, fname, installdir, verbose):
                 error = True
 
     if not error:
         pprint('uninstalled successfully')
         return True
 
-    pprint('errors occurred during uninstallation')
     return False
 
 
 def _remove_fname(pkg: str, fname: str, installdir:str, verbose: bool):
 
     # custom print
     pprint = ProgressReporter.get_print_fn(pkg)
```

### Comparing `hhcm_forest-1.1.7/src/forest/common/package.py` & `hhcm_forest-1.1.8/src/forest/common/package.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.7/src/forest/common/parser.py` & `hhcm_forest-1.1.8/src/forest/common/parser.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.7/src/forest/common/print_utils.py` & `hhcm_forest-1.1.8/src/forest/common/print_utils.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.7/src/forest/common/proc_utils.py` & `hhcm_forest-1.1.8/src/forest/common/proc_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import subprocess
 import sys
-import getpass
-import re
 import typing
 import progressbar
+import os
 
 from forest.common import print_utils
 from forest.common.parser import update_progress_bar
+from forest.common.forest_dirs import rootdir
 
 call_process_verbose = False
 
 
 def call_process(args: typing.List[str] = None, 
                  cwd='.', 
                  input=None,
                  verbose=False,
                  print_on_error=True, 
                  shell: bool=False,
                  timeout=None,
-                 update_regrex_pattern=None,
-                 stderr_to_stdout=False
+                 update_regrex_pattern=None
                  ) -> bool:    
     
     # convert args to string
     args = list(map(str, args))    
     
     if verbose or call_process_verbose:
         if shell:
@@ -49,30 +48,36 @@
 
         print(f'returned {proc.returncode}')
 
         return proc.returncode == 0         
 
     try:
         #  # universal_newlines=True equivalent to text=True (backward compatibility)
-        #  see https://docs.python.org/3/library/subprocess.html#subprocess.Popen:~:text=Used%20Arguments.-,The%20universal_newlines%20argument%20is%20equivalent%20to%20text%20and%20is%20provided%20for%20backwards%20compatibility.%20By%20default%2C%20file%20objects%20are%20opened%20in%20binary%20mode.,-New%20in%20version
-        stderr = subprocess.STDOUT if stderr_to_stdout else subprocess.PIPE
         pr = subprocess.Popen(args=popen_args,
                                 stdout=subprocess.PIPE,
-                                stderr=stderr, 
+                                stderr=subprocess.STDOUT, 
                                 cwd=cwd, 
                                 shell=shell, 
                                 executable=executable,
                                 universal_newlines=True)
         
+        lines = []
         if update_regrex_pattern is not None:
-            _progress_bar(pr, update_regrex_pattern)
+            lines = _progress_bar(pr, update_regrex_pattern)
             
         if pr.wait(timeout=timeout) != 0:
-            if print_on_error:
-                print(pr.stderr.read(), file=sys.stderr)  
+            if lines:
+                print_utils.log_file.writelines(lines)
+            else:
+                print_utils.log_file.write(pr.stdout.read())
+            
+            if print_on_error and not verbose:
+                print_utils.log_file.seek(0)  # go to the beginning of the file
+                print(print_utils.log_file.read(), file=sys.stderr)
+
             return False
         
         return True
 
     #todo: fix subprocess.CalledProcessError not working with subprocess.Popen
     except subprocess.CalledProcessError as e:
         # on error, print output (includes stderr)
@@ -83,30 +88,26 @@
             
         return False
 
 def _progress_bar(process, regrex_pattern):
     pbar = progressbar.ProgressBar(maxval=100, \
     widgets=[progressbar.Bar('=', '[', ']'), ' ', progressbar.Percentage()])
     pbar.start()
-    
+    lines = []
+
     while True:
         line = process.stdout.readline()
+        lines.append(line)
 
         if not line:
             pbar.finish()
-            break
+            return lines
             
         update_progress_bar(line, pbar=pbar, regrex_pattern=regrex_pattern)
 
-def _no_progress_bar(process):
-    while True:
-            line = process.stdout.readline()
-
-            if not line:
-                break
 
 def get_output(args, cwd='.', input=None, verbose=False, print_on_error=True, shell=False):
 
     if verbose or call_process_verbose:
         if shell:
             print(f'calling shell with command "{args}"')
         else:
```

### Comparing `hhcm_forest-1.1.7/src/forest/common/recipe.py` & `hhcm_forest-1.1.8/src/forest/common/recipe.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.7/src/forest/common/setup.bash` & `hhcm_forest-1.1.8/src/forest/common/setup.bash`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.7/src/forest/common/sudo_refresh.py` & `hhcm_forest-1.1.8/src/forest/common/sudo_refresh.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.7/src/forest/git_tools/__init__.py` & `hhcm_forest-1.1.8/src/forest/git_tools/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,16 +51,15 @@
         cmd.extend([addr, self.srcdir])
 
         # clone, and delete the source folder on failure
         # (either exception or git returns != 0) 
         try:
             # Progress status is reported on the standard error stream
             clone_ok = proc_utils.call_process(args=cmd, 
-                                               update_regrex_pattern=git_regrex_pattern,
-                                               stderr_to_stdout=True)
+                                               update_regrex_pattern=git_regrex_pattern)
             
             # checkout to requested branch/tag/commit
             if tag is not None:
                 clone_ok = clone_ok and self.checkout(tag=tag)
             
             if not clone_ok:
                 self.rm()
```

### Comparing `hhcm_forest-1.1.7/src/forest/main.py` & `hhcm_forest-1.1.8/src/forest/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     # verbose mode will show output of any called process
     if args.verbose:
         from forest.common import proc_utils
         proc_utils.call_process_verbose = True
 
     if not args.verbose:
         from forest.common import print_utils
-        print_utils.log_file = open(args.log_file, 'w')
+        print_utils.log_file = open(args.log_file, 'w+')
 
     # sudo handling 
     if args.command == grow_cmd and args.pwd is not None:
         sudo_refresher = sudo_refresh.SudoRefresher(pwd=args.pwd)
 
     # print available packages
     if args.list:
```

### Comparing `hhcm_forest-1.1.7/src/hhcm_forest.egg-info/PKG-INFO` & `hhcm_forest-1.1.8/src/hhcm_forest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhcm-forest
-Version: 1.1.7
+Version: 1.1.8
 Summary: A minimalistic tool to automate source code cloning and building
 Home-page: https://none
 Author: Arturo Laurenzi
 Author-email: arturo.laurenzi@iit.it
 License: UNKNOWN
 Project-URL: Bug Tracker, https://none
 Platform: UNKNOWN
```

### Comparing `hhcm_forest-1.1.7/src/hhcm_forest.egg-info/SOURCES.txt` & `hhcm_forest-1.1.8/src/hhcm_forest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.7/test/test_run_bash_tests.py` & `hhcm_forest-1.1.8/test/test_run_bash_tests.py`

 * *Files identical despite different names*


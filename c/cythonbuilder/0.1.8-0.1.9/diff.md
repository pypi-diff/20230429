# Comparing `tmp/cythonbuilder-0.1.8.tar.gz` & `tmp/cythonbuilder-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cythonbuilder-0.1.8.tar", last modified: Mon May 16 14:03:44 2022, max compression
+gzip compressed data, was "cythonbuilder-0.1.9.tar", last modified: Mon May 16 14:22:13 2022, max compression
```

## Comparing `cythonbuilder-0.1.8.tar` & `cythonbuilder-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-05-16 14:03:44.087987 cythonbuilder-0.1.8/
--rw-rw-rw-   0        0        0     5785 2022-05-16 14:03:44.087987 cythonbuilder-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     4934 2022-05-13 13:50:21.000000 cythonbuilder-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2022-05-16 14:03:44.040910 cythonbuilder-0.1.8/cythonbuilder/
--rw-rw-rw-   0        0        0      436 2022-05-16 14:03:42.000000 cythonbuilder-0.1.8/cythonbuilder/__init__.py
--rw-rw-rw-   0        0        0      149 2022-05-13 13:52:21.000000 cythonbuilder-0.1.8/cythonbuilder/__main__.py
--rw-rw-rw-   0        0        0      220 2022-05-09 13:04:16.000000 cythonbuilder-0.1.8/cythonbuilder/appsettings.py
--rw-rw-rw-   0        0        0    10215 2022-05-16 09:31:08.000000 cythonbuilder-0.1.8/cythonbuilder/cli.py
--rw-rw-rw-   0        0        0     6822 2022-05-10 07:24:48.000000 cythonbuilder-0.1.8/cythonbuilder/cython_builder.py
--rw-rw-rw-   0        0        0      210 2022-05-10 08:37:15.000000 cythonbuilder-0.1.8/cythonbuilder/definitions.py
--rw-rw-rw-   0        0        0     5496 2022-05-09 18:12:22.000000 cythonbuilder-0.1.8/cythonbuilder/helpers.py
--rw-rw-rw-   0        0        0     7267 2022-05-09 18:19:14.000000 cythonbuilder-0.1.8/cythonbuilder/logs.py
--rw-rw-rw-   0        0        0     7495 2022-05-13 13:45:03.000000 cythonbuilder-0.1.8/cythonbuilder/pyigenerator.py
--rw-rw-rw-   0        0        0      844 2022-05-09 18:19:30.000000 cythonbuilder-0.1.8/cythonbuilder/services.py
-drwxrwxrwx   0        0        0        0 2022-05-16 14:03:44.085910 cythonbuilder-0.1.8/cythonbuilder.egg-info/
--rw-rw-rw-   0        0        0     5785 2022-05-16 14:03:43.000000 cythonbuilder-0.1.8/cythonbuilder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2022-05-16 14:03:43.000000 cythonbuilder-0.1.8/cythonbuilder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-16 14:03:43.000000 cythonbuilder-0.1.8/cythonbuilder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2022-05-16 14:03:43.000000 cythonbuilder-0.1.8/cythonbuilder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2022-05-16 14:03:43.000000 cythonbuilder-0.1.8/cythonbuilder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-05-16 14:03:43.000000 cythonbuilder-0.1.8/cythonbuilder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1100 2022-05-09 13:21:49.000000 cythonbuilder-0.1.8/license.txt
--rw-rw-rw-   0        0        0       86 2022-05-16 14:03:44.088992 cythonbuilder-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     2069 2022-05-16 14:03:42.000000 cythonbuilder-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-16 14:03:44.086910 cythonbuilder-0.1.8/test/
--rw-rw-rw-   0        0        0      650 2022-05-09 12:22:23.000000 cythonbuilder-0.1.8/test/test_functions.py
+drwxrwxrwx   0        0        0        0 2022-05-16 14:22:13.257881 cythonbuilder-0.1.9/
+-rw-rw-rw-   0        0        0     5785 2022-05-16 14:22:13.257881 cythonbuilder-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4934 2022-05-13 13:50:21.000000 cythonbuilder-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2022-05-16 14:22:13.240881 cythonbuilder-0.1.9/cythonbuilder/
+-rw-rw-rw-   0        0        0      436 2022-05-16 14:22:12.000000 cythonbuilder-0.1.9/cythonbuilder/__init__.py
+-rw-rw-rw-   0        0        0      149 2022-05-13 13:52:21.000000 cythonbuilder-0.1.9/cythonbuilder/__main__.py
+-rw-rw-rw-   0        0        0      220 2022-05-09 13:04:16.000000 cythonbuilder-0.1.9/cythonbuilder/appsettings.py
+-rw-rw-rw-   0        0        0    10215 2022-05-16 09:31:08.000000 cythonbuilder-0.1.9/cythonbuilder/cli.py
+-rw-rw-rw-   0        0        0     6822 2022-05-10 07:24:48.000000 cythonbuilder-0.1.9/cythonbuilder/cython_builder.py
+-rw-rw-rw-   0        0        0      210 2022-05-10 08:37:15.000000 cythonbuilder-0.1.9/cythonbuilder/definitions.py
+-rw-rw-rw-   0        0        0     5496 2022-05-09 18:12:22.000000 cythonbuilder-0.1.9/cythonbuilder/helpers.py
+-rw-rw-rw-   0        0        0     7267 2022-05-09 18:19:14.000000 cythonbuilder-0.1.9/cythonbuilder/logs.py
+-rw-rw-rw-   0        0        0     7716 2022-05-16 14:21:50.000000 cythonbuilder-0.1.9/cythonbuilder/pyigenerator.py
+-rw-rw-rw-   0        0        0      844 2022-05-09 18:19:30.000000 cythonbuilder-0.1.9/cythonbuilder/services.py
+drwxrwxrwx   0        0        0        0 2022-05-16 14:22:13.250881 cythonbuilder-0.1.9/cythonbuilder.egg-info/
+-rw-rw-rw-   0        0        0     5785 2022-05-16 14:22:12.000000 cythonbuilder-0.1.9/cythonbuilder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2022-05-16 14:22:13.000000 cythonbuilder-0.1.9/cythonbuilder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-16 14:22:12.000000 cythonbuilder-0.1.9/cythonbuilder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2022-05-16 14:22:12.000000 cythonbuilder-0.1.9/cythonbuilder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2022-05-16 14:22:13.000000 cythonbuilder-0.1.9/cythonbuilder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2022-05-16 14:22:13.000000 cythonbuilder-0.1.9/cythonbuilder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1100 2022-05-09 13:21:49.000000 cythonbuilder-0.1.9/license.txt
+-rw-rw-rw-   0        0        0       86 2022-05-16 14:22:13.258882 cythonbuilder-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2069 2022-05-16 14:22:12.000000 cythonbuilder-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-16 14:22:13.251882 cythonbuilder-0.1.9/test/
+-rw-rw-rw-   0        0        0      650 2022-05-09 12:22:23.000000 cythonbuilder-0.1.9/test/test_functions.py
```

### Comparing `cythonbuilder-0.1.8/PKG-INFO` & `cythonbuilder-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cythonbuilder
-Version: 0.1.8
+Version: 0.1.9
 Summary: CythonBuilder; automated compiling and packaging of Cython code
 Home-page: https://github.com/mike-huls/cythonbuilder
 Author: Mike Huls
 Author-email: mikehuls42@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/mike-huls/cythonbuilder/
 Project-URL: Bug Tracker, https://github.com/mike-huls/cythonbuilder/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cythonbuilder Version: 0.1.8 Summary:
+Metadata-Version: 2.1 Name: cythonbuilder Version: 0.1.9 Summary:
 CythonBuilder; automated compiling and packaging of Cython code Home-page:
 https://github.com/mike-huls/cythonbuilder Author: Mike Huls Author-email:
 mikehuls42@gmail.com License: MIT Project-URL: Source, https://github.com/mike-
 huls/cythonbuilder/ Project-URL: Bug Tracker, https://github.com/mike-huls/
 cythonbuilder/issues Project-URL: Documentation, https://github.com/mike-huls/
 cythonbuilder/blob/main/README.md/ Keywords:
 pypi,Cython,setup,packaging,compilation Platform: UNKNOWN Classifier:
```

### Comparing `cythonbuilder-0.1.8/README.md` & `cythonbuilder-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cythonbuilder-0.1.8/cythonbuilder/cli.py` & `cythonbuilder-0.1.9/cythonbuilder/cli.py`

 * *Files identical despite different names*

### Comparing `cythonbuilder-0.1.8/cythonbuilder/cython_builder.py` & `cythonbuilder-0.1.9/cythonbuilder/cython_builder.py`

 * *Files identical despite different names*

### Comparing `cythonbuilder-0.1.8/cythonbuilder/helpers.py` & `cythonbuilder-0.1.9/cythonbuilder/helpers.py`

 * *Files identical despite different names*

### Comparing `cythonbuilder-0.1.8/cythonbuilder/logs.py` & `cythonbuilder-0.1.9/cythonbuilder/logs.py`

 * *Files identical despite different names*

### Comparing `cythonbuilder-0.1.8/cythonbuilder/pyigenerator.py` & `cythonbuilder-0.1.9/cythonbuilder/pyigenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,19 @@
         # for line in py_lines:
         #     print(line+'\n')
         #     pyi_out.write(line)
 
 
 def line_is_import(line:str) -> bool:
     """ """
-    return line.split(" ")[0] in ['import', 'cimport']
+    line = line.strip()
+    word_array = line.split(" ")
+    first_word_is_import = word_array[0] in ['import', 'cimport']
+    line_contains_from_import = word_array[0] == 'from' and 'import' in word_array
+    return any([first_word_is_import, line_contains_from_import])
 def line_is_class(line:str) -> bool:
     """ """
     return line[-1] == ":" and "class" in line.split(" ")
 
 def line_is_function(line:str) -> bool:
     """ """
     line = line.strip(' ')
```

### Comparing `cythonbuilder-0.1.8/cythonbuilder/services.py` & `cythonbuilder-0.1.9/cythonbuilder/services.py`

 * *Files identical despite different names*

### Comparing `cythonbuilder-0.1.8/cythonbuilder.egg-info/PKG-INFO` & `cythonbuilder-0.1.9/cythonbuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cythonbuilder
-Version: 0.1.8
+Version: 0.1.9
 Summary: CythonBuilder; automated compiling and packaging of Cython code
 Home-page: https://github.com/mike-huls/cythonbuilder
 Author: Mike Huls
 Author-email: mikehuls42@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/mike-huls/cythonbuilder/
 Project-URL: Bug Tracker, https://github.com/mike-huls/cythonbuilder/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cythonbuilder Version: 0.1.8 Summary:
+Metadata-Version: 2.1 Name: cythonbuilder Version: 0.1.9 Summary:
 CythonBuilder; automated compiling and packaging of Cython code Home-page:
 https://github.com/mike-huls/cythonbuilder Author: Mike Huls Author-email:
 mikehuls42@gmail.com License: MIT Project-URL: Source, https://github.com/mike-
 huls/cythonbuilder/ Project-URL: Bug Tracker, https://github.com/mike-huls/
 cythonbuilder/issues Project-URL: Documentation, https://github.com/mike-huls/
 cythonbuilder/blob/main/README.md/ Keywords:
 pypi,Cython,setup,packaging,compilation Platform: UNKNOWN Classifier:
```

### Comparing `cythonbuilder-0.1.8/cythonbuilder.egg-info/SOURCES.txt` & `cythonbuilder-0.1.9/cythonbuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cythonbuilder-0.1.8/license.txt` & `cythonbuilder-0.1.9/license.txt`

 * *Files identical despite different names*

### Comparing `cythonbuilder-0.1.8/setup.py` & `cythonbuilder-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 __package_name__ = "cythonbuilder"
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 __author__ = 'Mike Huls'
 __license__ = "MIT"
 __maintainer__ = "Mike Huls"
 __email__ = "mikehuls42@gmail.com"
 __status__ = "Development"
 __description__ = "CythonBuilder; automated compiling and packaging of Cython code"
 __project_url__ = "https://github.com/mike-huls/cythonbuilder"
```

### Comparing `cythonbuilder-0.1.8/test/test_functions.py` & `cythonbuilder-0.1.9/test/test_functions.py`

 * *Files identical despite different names*


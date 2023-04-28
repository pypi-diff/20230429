# Comparing `tmp/unisci-1.3.0.tar.gz` & `tmp/unisci-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unisci-1.3.0.tar", last modified: Fri Apr 28 21:34:02 2023, max compression
+gzip compressed data, was "unisci-1.3.1.tar", last modified: Fri Apr 28 21:59:01 2023, max compression
```

## Comparing `unisci-1.3.0.tar` & `unisci-1.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-28 21:34:02.316713 unisci-1.3.0/
--rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.3.0/LICENSE
--rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-27 04:25:20.000000 unisci-1.3.0/MANIFEST.in
--rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-04-28 21:34:02.316425 unisci-1.3.0/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)     1286 2023-04-28 05:01:19.000000 unisci-1.3.0/README.md
--rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-04-28 21:34:02.316790 unisci-1.3.0/setup.cfg
--rw-r--r--   0 vivaan     (501) staff       (20)      679 2023-04-28 21:30:28.000000 unisci-1.3.0/setup.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-28 21:34:02.309845 unisci-1.3.0/unisci/
--rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-04-28 21:30:06.000000 unisci-1.3.0/unisci/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.3.0/unisci/constants.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1508 2023-04-26 14:57:12.000000 unisci-1.3.0/unisci/conversion_factors.py
--rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.3.0/unisci/error.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-28 21:34:02.312321 unisci-1.3.0/unisci/formulas/
--rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.3.0/unisci/formulas/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)    11279 2023-04-28 21:29:37.000000 unisci-1.3.0/unisci/formulas/chemistry.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1840 2023-04-26 16:06:26.000000 unisci-1.3.0/unisci/metric.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-28 21:34:02.315571 unisci-1.3.0/unisci/periodic/
--rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.3.0/unisci/periodic/periodic-table-lookup.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-04-21 14:47:26.000000 unisci-1.3.0/unisci/periodic/periodic-table-numbers.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.3.0/unisci/periodic/periodic-table-symbols.json
--rw-r--r--   0 vivaan     (501) staff       (20)    38863 2023-04-28 04:22:19.000000 unisci-1.3.0/unisci/types.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-28 21:34:02.311838 unisci-1.3.0/unisci.egg-info/
--rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-04-28 21:34:02.000000 unisci-1.3.0/unisci.egg-info/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)      492 2023-04-28 21:34:02.000000 unisci-1.3.0/unisci.egg-info/SOURCES.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-04-28 21:34:02.000000 unisci-1.3.0/unisci.egg-info/dependency_links.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       30 2023-04-28 21:34:02.000000 unisci-1.3.0/unisci.egg-info/requires.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-04-28 21:34:02.000000 unisci-1.3.0/unisci.egg-info/top_level.txt
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-28 21:59:01.175364 unisci-1.3.1/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.3.1/LICENSE
+-rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-27 04:25:20.000000 unisci-1.3.1/MANIFEST.in
+-rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-04-28 21:59:01.175078 unisci-1.3.1/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)     1286 2023-04-28 05:01:19.000000 unisci-1.3.1/README.md
+-rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-04-28 21:59:01.175444 unisci-1.3.1/setup.cfg
+-rw-r--r--   0 vivaan     (501) staff       (20)      679 2023-04-28 21:56:03.000000 unisci-1.3.1/setup.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-28 21:59:01.170941 unisci-1.3.1/unisci/
+-rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-04-28 21:56:09.000000 unisci-1.3.1/unisci/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.3.1/unisci/constants.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1508 2023-04-26 14:57:12.000000 unisci-1.3.1/unisci/conversion_factors.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.3.1/unisci/error.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-28 21:59:01.173588 unisci-1.3.1/unisci/formulas/
+-rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.3.1/unisci/formulas/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)    11414 2023-04-28 21:53:09.000000 unisci-1.3.1/unisci/formulas/chemistry.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1840 2023-04-26 16:06:26.000000 unisci-1.3.1/unisci/metric.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-28 21:59:01.174741 unisci-1.3.1/unisci/periodic/
+-rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.3.1/unisci/periodic/periodic-table-lookup.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-04-21 14:47:26.000000 unisci-1.3.1/unisci/periodic/periodic-table-numbers.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.3.1/unisci/periodic/periodic-table-symbols.json
+-rw-r--r--   0 vivaan     (501) staff       (20)    38863 2023-04-28 04:22:19.000000 unisci-1.3.1/unisci/types.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-28 21:59:01.173092 unisci-1.3.1/unisci.egg-info/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-04-28 21:59:01.000000 unisci-1.3.1/unisci.egg-info/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)      492 2023-04-28 21:59:01.000000 unisci-1.3.1/unisci.egg-info/SOURCES.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-04-28 21:59:01.000000 unisci-1.3.1/unisci.egg-info/dependency_links.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       30 2023-04-28 21:59:01.000000 unisci-1.3.1/unisci.egg-info/requires.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-04-28 21:59:01.000000 unisci-1.3.1/unisci.egg-info/top_level.txt
```

### Comparing `unisci-1.3.0/LICENSE` & `unisci-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unisci-1.3.0/PKG-INFO` & `unisci-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.3.0
+Version: 1.3.1
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://unisci.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `unisci-1.3.0/README.md` & `unisci-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `unisci-1.3.0/setup.py` & `unisci-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.readlines()
 
 setup(
     name='unisci',
-    version='1.3.0',
+    version='1.3.1',
     author='Vivaan Singhvi',
     author_email='singhvi.vivaan@gmail.com',
     description='Units Conversions, and Science Package',
     long_description=description,
     long_description_content_type="text/markdown",
     license='MIT',
     packages=find_packages(),
```

### Comparing `unisci-1.3.0/unisci/conversion_factors.py` & `unisci-1.3.1/unisci/conversion_factors.py`

 * *Files identical despite different names*

### Comparing `unisci-1.3.0/unisci/error.py` & `unisci-1.3.1/unisci/error.py`

 * *Files identical despite different names*

### Comparing `unisci-1.3.0/unisci/formulas/chemistry.py` & `unisci-1.3.1/unisci/formulas/chemistry.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,16 @@
     Arguments: A molecule to find the molar mass of. Enter subscripts as normal numbers. Exclude coefficients or charges. Parentheses are supported.
 
     Raises: UnsupportedError for a wrongly formatted molecule.
 
     Returns: The molar mass as a Quantity in g/mol.
     """
 
+    molecule += " "     # for indexing another time
+
     # store sum
     total_mass = Quantity(0, {'g': 1, 'mol': -1})
 
     # empty vars
     parens = []
     temp_inside_paren = ""
     temp_paren_num = ""
@@ -311,14 +313,16 @@
 
             # keep adding to the number   
             if c.isnumeric():
                 temp_paren_num += c
 
             # if not part of the number go back a character and add number to the paren numbers
             else:
+                if temp_paren_num == "":
+                    temp_paren_num = "1"
                 paren_numbers.append(int(temp_paren_num))   # adds integer version to mulitply by thing
                 temp_paren_num = ""                         # resets variables
                 find_num = False
                 i -= 1                                      # moves incrementor back
 
         # adds to molecules inside the parentheses
         elif paren_level > 0:
```

### Comparing `unisci-1.3.0/unisci/metric.py` & `unisci-1.3.1/unisci/metric.py`

 * *Files identical despite different names*

### Comparing `unisci-1.3.0/unisci/periodic/periodic-table-lookup.json` & `unisci-1.3.1/unisci/periodic/periodic-table-lookup.json`

 * *Files identical despite different names*

### Comparing `unisci-1.3.0/unisci/periodic/periodic-table-numbers.json` & `unisci-1.3.1/unisci/periodic/periodic-table-numbers.json`

 * *Files identical despite different names*

### Comparing `unisci-1.3.0/unisci/periodic/periodic-table-symbols.json` & `unisci-1.3.1/unisci/periodic/periodic-table-symbols.json`

 * *Files identical despite different names*

### Comparing `unisci-1.3.0/unisci/types.py` & `unisci-1.3.1/unisci/types.py`

 * *Files identical despite different names*

### Comparing `unisci-1.3.0/unisci.egg-info/PKG-INFO` & `unisci-1.3.1/unisci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.3.0
+Version: 1.3.1
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://unisci.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```


# Comparing `tmp/VDBforGenAI-0.1.tar.gz` & `tmp/VDBforGenAI-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VDBforGenAI-0.1.tar", last modified: Sat Apr 29 11:19:21 2023, max compression
+gzip compressed data, was "VDBforGenAI-0.2.tar", last modified: Sat Apr 29 11:31:30 2023, max compression
```

## Comparing `VDBforGenAI-0.1.tar` & `VDBforGenAI-0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 11:19:21.896342 VDBforGenAI-0.1/
--rw-rw-rw-   0        0        0     1091 2023-04-19 17:28:40.000000 VDBforGenAI-0.1/LICENSE
--rw-rw-rw-   0        0        0     3530 2023-04-29 11:19:21.895345 VDBforGenAI-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3022 2023-04-22 19:03:13.000000 VDBforGenAI-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 11:19:21.870411 VDBforGenAI-0.1/VDBforGenAI/
-drwxrwxrwx   0        0        0        0 2023-04-29 11:19:21.888363 VDBforGenAI-0.1/VDBforGenAI/Utilities/
--rw-rw-rw-   0        0        0     1103 2023-04-22 19:09:41.000000 VDBforGenAI-0.1/VDBforGenAI/Utilities/Loading.py
--rw-rw-rw-   0        0        0     1189 2023-04-25 00:13:24.000000 VDBforGenAI-0.1/VDBforGenAI/Utilities/StringUtilities.py
--rw-rw-rw-   0        0        0        0 2023-04-22 19:05:05.000000 VDBforGenAI-0.1/VDBforGenAI/Utilities/__init__.py
--rw-rw-rw-   0        0        0    18354 2023-04-29 11:15:16.000000 VDBforGenAI-0.1/VDBforGenAI/VectorDatabase.py
-drwxrwxrwx   0        0        0        0 2023-04-29 11:19:21.894347 VDBforGenAI-0.1/VDBforGenAI/VectorisationAndIndexCreation/
--rw-rw-rw-   0        0        0     2685 2023-04-25 00:40:09.000000 VDBforGenAI-0.1/VDBforGenAI/VectorisationAndIndexCreation/SearchFunctions.py
--rw-rw-rw-   0        0        0        0 2023-04-19 17:31:55.000000 VDBforGenAI-0.1/VDBforGenAI/VectorisationAndIndexCreation/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-24 23:14:42.000000 VDBforGenAI-0.1/VDBforGenAI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 11:19:21.881381 VDBforGenAI-0.1/VDBforGenAI.egg-info/
--rw-rw-rw-   0        0        0     3530 2023-04-29 11:19:21.000000 VDBforGenAI-0.1/VDBforGenAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-04-29 11:19:21.000000 VDBforGenAI-0.1/VDBforGenAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 11:19:21.000000 VDBforGenAI-0.1/VDBforGenAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-29 11:19:21.000000 VDBforGenAI-0.1/VDBforGenAI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 11:19:21.000000 VDBforGenAI-0.1/VDBforGenAI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 11:19:21.896342 VDBforGenAI-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1658 2023-04-24 23:20:52.000000 VDBforGenAI-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:31:30.949611 VDBforGenAI-0.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-19 17:28:40.000000 VDBforGenAI-0.2/LICENSE
+-rw-rw-rw-   0        0        0     3554 2023-04-29 11:31:30.948614 VDBforGenAI-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3022 2023-04-22 19:03:13.000000 VDBforGenAI-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 11:31:30.925565 VDBforGenAI-0.2/VDBforGenAI/
+drwxrwxrwx   0        0        0        0 2023-04-29 11:31:30.946618 VDBforGenAI-0.2/VDBforGenAI/Utilities/
+-rw-rw-rw-   0        0        0     1103 2023-04-22 19:09:41.000000 VDBforGenAI-0.2/VDBforGenAI/Utilities/Loading.py
+-rw-rw-rw-   0        0        0     1189 2023-04-25 00:13:24.000000 VDBforGenAI-0.2/VDBforGenAI/Utilities/StringUtilities.py
+-rw-rw-rw-   0        0        0        0 2023-04-22 19:05:05.000000 VDBforGenAI-0.2/VDBforGenAI/Utilities/__init__.py
+-rw-rw-rw-   0        0        0    18354 2023-04-29 11:15:16.000000 VDBforGenAI-0.2/VDBforGenAI/VectorDatabase.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:31:30.948614 VDBforGenAI-0.2/VDBforGenAI/VectorisationAndIndexCreation/
+-rw-rw-rw-   0        0        0     2685 2023-04-25 00:40:09.000000 VDBforGenAI-0.2/VDBforGenAI/VectorisationAndIndexCreation/SearchFunctions.py
+-rw-rw-rw-   0        0        0        0 2023-04-19 17:31:55.000000 VDBforGenAI-0.2/VDBforGenAI/VectorisationAndIndexCreation/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 23:14:42.000000 VDBforGenAI-0.2/VDBforGenAI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:31:30.944628 VDBforGenAI-0.2/VDBforGenAI.egg-info/
+-rw-rw-rw-   0        0        0     3554 2023-04-29 11:31:30.000000 VDBforGenAI-0.2/VDBforGenAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-04-29 11:31:30.000000 VDBforGenAI-0.2/VDBforGenAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 11:31:30.000000 VDBforGenAI-0.2/VDBforGenAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-29 11:31:30.000000 VDBforGenAI-0.2/VDBforGenAI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 11:31:30.000000 VDBforGenAI-0.2/VDBforGenAI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 11:31:30.949611 VDBforGenAI-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-04-29 11:28:12.000000 VDBforGenAI-0.2/setup.py
```

### Comparing `VDBforGenAI-0.1/LICENSE` & `VDBforGenAI-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `VDBforGenAI-0.1/PKG-INFO` & `VDBforGenAI-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: VDBforGenAI
-Version: 0.1
-Summary: A package for generating and querying Vector Databases for Genomic Data using AI
+Version: 0.2
+Summary: A simple package for generating and querying Vector Databases for Generative AI as well any other reason
 Home-page: https://github.com/JakubJDolezal/VDBforGenAI
 Author: Jakub Dolezal
 Author-email: jakubdolezal93@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `VDBforGenAI-0.1/README.md` & `VDBforGenAI-0.2/README.md`

 * *Files identical despite different names*

### Comparing `VDBforGenAI-0.1/VDBforGenAI/Utilities/Loading.py` & `VDBforGenAI-0.2/VDBforGenAI/Utilities/Loading.py`

 * *Files identical despite different names*

### Comparing `VDBforGenAI-0.1/VDBforGenAI/Utilities/StringUtilities.py` & `VDBforGenAI-0.2/VDBforGenAI/Utilities/StringUtilities.py`

 * *Files identical despite different names*

### Comparing `VDBforGenAI-0.1/VDBforGenAI/VectorDatabase.py` & `VDBforGenAI-0.2/VDBforGenAI/VectorDatabase.py`

 * *Files identical despite different names*

### Comparing `VDBforGenAI-0.1/VDBforGenAI/VectorisationAndIndexCreation/SearchFunctions.py` & `VDBforGenAI-0.2/VDBforGenAI/VectorisationAndIndexCreation/SearchFunctions.py`

 * *Files identical despite different names*

### Comparing `VDBforGenAI-0.1/VDBforGenAI.egg-info/PKG-INFO` & `VDBforGenAI-0.2/VDBforGenAI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: VDBforGenAI
-Version: 0.1
-Summary: A package for generating and querying Vector Databases for Genomic Data using AI
+Version: 0.2
+Summary: A simple package for generating and querying Vector Databases for Generative AI as well any other reason
 Home-page: https://github.com/JakubJDolezal/VDBforGenAI
 Author: Jakub Dolezal
 Author-email: jakubdolezal93@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `VDBforGenAI-0.1/setup.py` & `VDBforGenAI-0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 setup(
 	# Name of the package 
 	name='VDBforGenAI',
 	# Packages to include into the distribution 
 	packages=find_packages('.'),
 	# Start with a small number and increase it with 
 	# every change you make https://semver.org 
-	version='0.1',
+	version='0.2',
 	# Chose a license from here: https: // 
 	# help.github.com / articles / licensing - a - 
 	# repository. For example: MIT 
 	license='',
 	# Short description of your library 
-	description='A package for generating and querying Vector Databases for Genomic Data using AI',
+	description='A simple package for generating and querying Vector Databases for Generative AI as well any other reason',
 	# Long description of your library 
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	# Your name 
 	author='Jakub Dolezal',
 	# Your email 
 	author_email='jakubdolezal93@gmail.com',
```


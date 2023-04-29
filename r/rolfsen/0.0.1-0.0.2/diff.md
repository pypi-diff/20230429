# Comparing `tmp/rolfsen-0.0.1.tar.gz` & `tmp/rolfsen-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rolfsen-0.0.1.tar", last modified: Sat Apr 29 05:00:16 2023, max compression
+gzip compressed data, was "rolfsen-0.0.2.tar", last modified: Sat Apr 29 08:12:59 2023, max compression
```

## Comparing `rolfsen-0.0.1.tar` & `rolfsen-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 james.rolfsen   (502) staff       (20)        0 2023-04-29 05:00:16.882909 rolfsen-0.0.1/
--rw-r--r--   0 james.rolfsen   (502) staff       (20)      571 2023-04-29 05:00:16.882717 rolfsen-0.0.1/PKG-INFO
-drwxr-xr-x   0 james.rolfsen   (502) staff       (20)        0 2023-04-29 05:00:16.881715 rolfsen-0.0.1/rolfsen/
--rw-rw-r--   0 james.rolfsen   (502) staff       (20)      118 2023-04-29 00:25:57.000000 rolfsen-0.0.1/rolfsen/__init__.py
-drwxr-xr-x   0 james.rolfsen   (502) staff       (20)        0 2023-04-29 05:00:16.882524 rolfsen-0.0.1/rolfsen.egg-info/
--rw-r--r--   0 james.rolfsen   (502) staff       (20)      571 2023-04-29 05:00:16.000000 rolfsen-0.0.1/rolfsen.egg-info/PKG-INFO
--rw-r--r--   0 james.rolfsen   (502) staff       (20)      152 2023-04-29 05:00:16.000000 rolfsen-0.0.1/rolfsen.egg-info/SOURCES.txt
--rw-r--r--   0 james.rolfsen   (502) staff       (20)        1 2023-04-29 05:00:16.000000 rolfsen-0.0.1/rolfsen.egg-info/dependency_links.txt
--rw-r--r--   0 james.rolfsen   (502) staff       (20)        8 2023-04-29 05:00:16.000000 rolfsen-0.0.1/rolfsen.egg-info/top_level.txt
--rw-r--r--   0 james.rolfsen   (502) staff       (20)       38 2023-04-29 05:00:16.882970 rolfsen-0.0.1/setup.cfg
--rw-rw-r--   0 james.rolfsen   (502) staff       (20)      817 2023-04-29 04:56:12.000000 rolfsen-0.0.1/setup.py
+drwxr-xr-x   0 james.rolfsen   (502) staff       (20)        0 2023-04-29 08:12:59.881664 rolfsen-0.0.2/
+-rw-r--r--   0 james.rolfsen   (502) staff       (20)      571 2023-04-29 08:12:59.881458 rolfsen-0.0.2/PKG-INFO
+drwxr-xr-x   0 james.rolfsen   (502) staff       (20)        0 2023-04-29 08:12:59.880467 rolfsen-0.0.2/rolfsen/
+-rw-rw-r--   0 james.rolfsen   (502) staff       (20)      118 2023-04-29 00:25:57.000000 rolfsen-0.0.2/rolfsen/__init__.py
+drwxr-xr-x   0 james.rolfsen   (502) staff       (20)        0 2023-04-29 08:12:59.881250 rolfsen-0.0.2/rolfsen.egg-info/
+-rw-r--r--   0 james.rolfsen   (502) staff       (20)      571 2023-04-29 08:12:59.000000 rolfsen-0.0.2/rolfsen.egg-info/PKG-INFO
+-rw-r--r--   0 james.rolfsen   (502) staff       (20)      152 2023-04-29 08:12:59.000000 rolfsen-0.0.2/rolfsen.egg-info/SOURCES.txt
+-rw-r--r--   0 james.rolfsen   (502) staff       (20)        1 2023-04-29 08:12:59.000000 rolfsen-0.0.2/rolfsen.egg-info/dependency_links.txt
+-rw-r--r--   0 james.rolfsen   (502) staff       (20)        8 2023-04-29 08:12:59.000000 rolfsen-0.0.2/rolfsen.egg-info/top_level.txt
+-rw-r--r--   0 james.rolfsen   (502) staff       (20)       38 2023-04-29 08:12:59.881716 rolfsen-0.0.2/setup.cfg
+-rw-rw-r--   0 james.rolfsen   (502) staff       (20)      845 2023-04-29 08:12:25.000000 rolfsen-0.0.2/setup.py
```

### Comparing `rolfsen-0.0.1/PKG-INFO` & `rolfsen-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rolfsen
-Version: 0.0.1
+Version: 0.0.2
 Summary: A really simple module to introduce everyone to James.
 Home-page: https://www.linkedin.com/in/jamesrolfsen/
 Author: James Rolfsen
 Author-email: james.rolfsen@think.dev
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rolfsen-0.0.1/rolfsen.egg-info/PKG-INFO` & `rolfsen-0.0.2/rolfsen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rolfsen
-Version: 0.0.1
+Version: 0.0.2
 Summary: A really simple module to introduce everyone to James.
 Home-page: https://www.linkedin.com/in/jamesrolfsen/
 Author: James Rolfsen
 Author-email: james.rolfsen@think.dev
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rolfsen-0.0.1/setup.py` & `rolfsen-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='rolfsen',
-    version='0.0.1',
+    version='0.0.2',
     description='A really simple module to introduce everyone to James.',
     author='James Rolfsen',
     author_email='james.rolfsen@think.dev',
     url='https://www.linkedin.com/in/jamesrolfsen/', 
-    packages=find_packages(),
+    #packages=find_packages(),
+    packages=['rolfsen'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```


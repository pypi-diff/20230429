# Comparing `tmp/pymailers-1.0.5.tar.gz` & `tmp/pymailers-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymailers-1.0.5.tar", last modified: Sat Apr 29 11:09:50 2023, max compression
+gzip compressed data, was "pymailers-1.1.5.tar", last modified: Sat Apr 29 14:12:08 2023, max compression
```

## Comparing `pymailers-1.0.5.tar` & `pymailers-1.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 root         (0) permagrp2  (9997)        0 2023-04-29 11:09:50.436000 pymailers-1.0.5/
--rw-rw----   0 root         (0) permagrp2  (9997)     2229 2023-04-29 11:09:50.420000 pymailers-1.0.5/PKG-INFO
--rw-rw----   0 root         (0) permagrp2  (9997)     1107 2023-04-29 10:37:28.000000 pymailers-1.0.5/README.md
-drwxrwx---   0 root         (0) permagrp2  (9997)        0 2023-04-29 11:09:50.292000 pymailers-1.0.5/pymailers/
--rw-rw----   0 root         (0) permagrp2  (9997)     1146 2023-04-29 11:03:12.000000 pymailers-1.0.5/pymailers/PyMailer.py
--rw-rw----   0 root         (0) permagrp2  (9997)        0 2023-04-29 10:37:28.000000 pymailers-1.0.5/pymailers/__init__.py
-drwxrwx---   0 root         (0) permagrp2  (9997)        0 2023-04-29 11:09:50.400000 pymailers-1.0.5/pymailers.egg-info/
--rw-rw----   0 root         (0) permagrp2  (9997)     2229 2023-04-29 11:09:48.000000 pymailers-1.0.5/pymailers.egg-info/PKG-INFO
--rw-rw----   0 root         (0) permagrp2  (9997)      194 2023-04-29 11:09:49.000000 pymailers-1.0.5/pymailers.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) permagrp2  (9997)        1 2023-04-29 11:09:49.000000 pymailers-1.0.5/pymailers.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) permagrp2  (9997)       10 2023-04-29 11:09:49.000000 pymailers-1.0.5/pymailers.egg-info/top_level.txt
--rw-rw----   0 root         (0) permagrp2  (9997)       38 2023-04-29 11:09:50.436000 pymailers-1.0.5/setup.cfg
--rw-rw----   0 root         (0) permagrp2  (9997)     1034 2023-04-29 11:08:45.000000 pymailers-1.0.5/setup.py
+drwxrwx---   0 root         (0) permagrp2  (9997)        0 2023-04-29 14:12:08.260001 pymailers-1.1.5/
+-rw-rw----   0 root         (0) permagrp2  (9997)     2229 2023-04-29 14:12:08.244001 pymailers-1.1.5/PKG-INFO
+-rw-rw----   0 root         (0) permagrp2  (9997)     1107 2023-04-29 13:19:31.000000 pymailers-1.1.5/README.md
+drwxrwx---   0 root         (0) permagrp2  (9997)        0 2023-04-29 14:12:08.108000 pymailers-1.1.5/pymailers/
+-rw-rw----   0 root         (0) permagrp2  (9997)     1749 2023-04-29 14:06:03.000000 pymailers-1.1.5/pymailers/PyMailer.py
+-rw-rw----   0 root         (0) permagrp2  (9997)        0 2023-04-29 13:19:31.000000 pymailers-1.1.5/pymailers/__init__.py
+drwxrwx---   0 root         (0) permagrp2  (9997)        0 2023-04-29 14:12:08.224001 pymailers-1.1.5/pymailers.egg-info/
+-rw-rw----   0 root         (0) permagrp2  (9997)     2229 2023-04-29 14:12:07.000000 pymailers-1.1.5/pymailers.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) permagrp2  (9997)      194 2023-04-29 14:12:07.000000 pymailers-1.1.5/pymailers.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) permagrp2  (9997)        1 2023-04-29 14:12:07.000000 pymailers-1.1.5/pymailers.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) permagrp2  (9997)       10 2023-04-29 14:12:07.000000 pymailers-1.1.5/pymailers.egg-info/top_level.txt
+-rw-rw----   0 root         (0) permagrp2  (9997)       38 2023-04-29 14:12:08.260001 pymailers-1.1.5/setup.cfg
+-rw-rw----   0 root         (0) permagrp2  (9997)     1034 2023-04-29 14:07:57.000000 pymailers-1.1.5/setup.py
```

### Comparing `pymailers-1.0.5/PKG-INFO` & `pymailers-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymailers
-Version: 1.0.5
+Version: 1.1.5
 Summary: The classic email sending library for Python.
 Home-page: https://github.com/rioagungpurnomo/pymailers
 Author: Rio Agung Purnomo
 Author-email: rioagungpurnomo.ak@gmail.com
 License: UNKNOWN
 Description: # PyMailers
         The classic email sending library for Python.
```

### Comparing `pymailers-1.0.5/README.md` & `pymailers-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pymailers-1.0.5/pymailers.egg-info/PKG-INFO` & `pymailers-1.1.5/pymailers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymailers
-Version: 1.0.5
+Version: 1.1.5
 Summary: The classic email sending library for Python.
 Home-page: https://github.com/rioagungpurnomo/pymailers
 Author: Rio Agung Purnomo
 Author-email: rioagungpurnomo.ak@gmail.com
 License: UNKNOWN
 Description: # PyMailers
         The classic email sending library for Python.
```

### Comparing `pymailers-1.0.5/setup.py` & `pymailers-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pymailers',
-    version='1.0.5',
+    version='1.1.5',
     description='The classic email sending library for Python.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Rio Agung Purnomo',
     author_email='rioagungpurnomo.ak@gmail.com',
     url='https://github.com/rioagungpurnomo/pymailers',
     packages=['pymailers'],
```


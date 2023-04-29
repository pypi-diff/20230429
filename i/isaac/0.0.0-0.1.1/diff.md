# Comparing `tmp/isaac-0.0.0.tar.gz` & `tmp/isaac-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isaac-0.0.0.tar", last modified: Fri Apr 22 14:36:33 2022, max compression
+gzip compressed data, was "isaac-0.1.1.tar", last modified: Sat Apr 29 09:05:08 2023, max compression
```

## Comparing `isaac-0.0.0.tar` & `isaac-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxr-xr-x   0 felixpetersen   (501) staff       (20)        0 2022-04-22 14:36:33.245225 isaac-0.0.0/
--rw-r--r--   0 felixpetersen   (501) staff       (20)      781 2022-04-22 14:36:33.244944 isaac-0.0.0/PKG-INFO
--rw-r--r--   0 felixpetersen   (501) staff       (20)        8 2022-04-22 14:35:53.000000 isaac-0.0.0/README.md
-drwxr-xr-x   0 felixpetersen   (501) staff       (20)        0 2022-04-22 14:36:33.244420 isaac-0.0.0/isaac.egg-info/
--rw-r--r--   0 felixpetersen   (501) staff       (20)      781 2022-04-22 14:36:32.000000 isaac-0.0.0/isaac.egg-info/PKG-INFO
--rw-r--r--   0 felixpetersen   (501) staff       (20)      162 2022-04-22 14:36:33.000000 isaac-0.0.0/isaac.egg-info/SOURCES.txt
--rw-r--r--   0 felixpetersen   (501) staff       (20)        1 2022-04-22 14:36:32.000000 isaac-0.0.0/isaac.egg-info/dependency_links.txt
--rw-r--r--   0 felixpetersen   (501) staff       (20)       19 2022-04-22 14:36:33.000000 isaac-0.0.0/isaac.egg-info/requires.txt
--rw-r--r--   0 felixpetersen   (501) staff       (20)        1 2022-04-22 14:36:33.000000 isaac-0.0.0/isaac.egg-info/top_level.txt
--rw-r--r--   0 felixpetersen   (501) staff       (20)       38 2022-04-22 14:36:33.245294 isaac-0.0.0/setup.cfg
--rw-r--r--   0 felixpetersen   (501) staff       (20)     1246 2022-04-22 14:35:53.000000 isaac-0.0.0/setup.py
+drwxr-xr-x   0 felixpetersen   (501) staff       (20)        0 2023-04-29 09:05:08.333316 isaac-0.1.1/
+-rw-r--r--   0 felixpetersen   (501) staff       (20)     1070 2023-04-29 08:54:03.000000 isaac-0.1.1/LICENSE
+-rw-r--r--   0 felixpetersen   (501) staff       (20)     3502 2023-04-29 09:05:08.333165 isaac-0.1.1/PKG-INFO
+-rw-r--r--   0 felixpetersen   (501) staff       (20)     2667 2023-04-29 08:54:03.000000 isaac-0.1.1/README.md
+drwxr-xr-x   0 felixpetersen   (501) staff       (20)        0 2023-04-29 09:05:08.332081 isaac-0.1.1/isaac/
+-rw-r--r--   0 felixpetersen   (501) staff       (20)      149 2023-04-29 08:54:03.000000 isaac-0.1.1/isaac/__init__.py
+-rw-r--r--   0 felixpetersen   (501) staff       (20)     4741 2023-04-29 08:54:03.000000 isaac-0.1.1/isaac/isaac.py
+drwxr-xr-x   0 felixpetersen   (501) staff       (20)        0 2023-04-29 09:05:08.332927 isaac-0.1.1/isaac.egg-info/
+-rw-r--r--   0 felixpetersen   (501) staff       (20)     3502 2023-04-29 09:05:08.000000 isaac-0.1.1/isaac.egg-info/PKG-INFO
+-rw-r--r--   0 felixpetersen   (501) staff       (20)      203 2023-04-29 09:05:08.000000 isaac-0.1.1/isaac.egg-info/SOURCES.txt
+-rw-r--r--   0 felixpetersen   (501) staff       (20)        1 2023-04-29 09:05:08.000000 isaac-0.1.1/isaac.egg-info/dependency_links.txt
+-rw-r--r--   0 felixpetersen   (501) staff       (20)       19 2023-04-29 09:05:08.000000 isaac-0.1.1/isaac.egg-info/requires.txt
+-rw-r--r--   0 felixpetersen   (501) staff       (20)        6 2023-04-29 09:05:08.000000 isaac-0.1.1/isaac.egg-info/top_level.txt
+-rw-r--r--   0 felixpetersen   (501) staff       (20)       38 2023-04-29 09:05:08.333378 isaac-0.1.1/setup.cfg
+-rw-r--r--   0 felixpetersen   (501) staff       (20)     1333 2023-04-29 09:03:49.000000 isaac-0.1.1/setup.py
```

### Comparing `isaac-0.0.0/setup.py` & `isaac-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
+isaac
 Copyright (c) Felix Petersen.
-
 This source code is licensed under the MIT license found in the LICENSE file.
 """
 
 __author__ = "Felix Petersen"
 __email__ = "ads0399@felix-petersen.de"
 
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='isaac',
-    version='v0.0.0',
-    description='isaac',
+    version='0.1.1',
+    description='ISAAC Newton - a method for accelerating neural network training.',
     author='Felix Petersen',
     author_email=__email__,
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Felix-Petersen/isaac',
     classifiers=[
         'Programming Language :: Python :: 3',
@@ -29,15 +29,15 @@
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     license='MIT License',
-    package_dir={},
-    packages=[],
+    package_dir={'isaac': 'isaac'},
+    packages=['isaac'],
     python_requires='>=3.6',
     install_requires=[
         'numpy',
         'torch>=1.9.0'
     ]
 )
```


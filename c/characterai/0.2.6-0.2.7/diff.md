# Comparing `tmp/characterai-0.2.6.tar.gz` & `tmp/characterai-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "characterai-0.2.6.tar", last modified: Sat Apr 29 18:36:41 2023, max compression
+gzip compressed data, was "characterai-0.2.7.tar", last modified: Sat Apr 29 20:07:49 2023, max compression
```

## Comparing `characterai-0.2.6.tar` & `characterai-0.2.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:36:41.687003 characterai-0.2.6/
--rw-r--r--   0 root         (0) root         (0)     1082 2023-04-29 18:28:44.000000 characterai-0.2.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1834 2023-04-29 18:36:41.687003 characterai-0.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1525 2023-04-29 18:28:44.000000 characterai-0.2.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:36:41.687003 characterai-0.2.6/characterai/
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-29 18:28:44.000000 characterai-0.2.6/characterai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9356 2023-04-29 18:32:10.000000 characterai-0.2.6/characterai/characterai.py
--rw-r--r--   0 root         (0) root         (0)      126 2023-04-29 18:28:44.000000 characterai-0.2.6/characterai/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:36:41.687003 characterai-0.2.6/characterai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1834 2023-04-29 18:36:41.000000 characterai-0.2.6/characterai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      273 2023-04-29 18:36:41.000000 characterai-0.2.6/characterai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 18:36:41.000000 characterai-0.2.6/characterai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-29 18:36:41.000000 characterai-0.2.6/characterai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-29 18:36:41.000000 characterai-0.2.6/characterai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 18:36:41.687003 characterai-0.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      631 2023-04-29 18:36:32.000000 characterai-0.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 20:07:49.769737 characterai-0.2.7/
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-04-29 18:28:44.000000 characterai-0.2.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-04-29 20:07:49.769737 characterai-0.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-04-29 18:28:44.000000 characterai-0.2.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 20:07:49.769737 characterai-0.2.7/characterai/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-29 18:28:44.000000 characterai-0.2.7/characterai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9356 2023-04-29 18:32:10.000000 characterai-0.2.7/characterai/characterai.py
+-rw-r--r--   0 root         (0) root         (0)      126 2023-04-29 18:28:44.000000 characterai-0.2.7/characterai/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 20:07:49.769737 characterai-0.2.7/characterai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-04-29 20:07:49.000000 characterai-0.2.7/characterai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      273 2023-04-29 20:07:49.000000 characterai-0.2.7/characterai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 20:07:49.000000 characterai-0.2.7/characterai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-29 20:07:49.000000 characterai-0.2.7/characterai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-29 20:07:49.000000 characterai-0.2.7/characterai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 20:07:49.769737 characterai-0.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      602 2023-04-29 20:06:40.000000 characterai-0.2.7/setup.py
```

### Comparing `characterai-0.2.6/LICENSE` & `characterai-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `characterai-0.2.6/PKG-INFO` & `characterai-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: characterai
-Version: 0.2.6
+Version: 0.2.7
 Summary: An unofficial API for character.ai for Python
 Home-page: https://github.com/kramcat/CharacterAI
 Author: kramcat
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `characterai-0.2.6/README.md` & `characterai-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `characterai-0.2.6/characterai/characterai.py` & `characterai-0.2.7/characterai/characterai.py`

 * *Files identical despite different names*

### Comparing `characterai-0.2.6/characterai.egg-info/PKG-INFO` & `characterai-0.2.7/characterai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: characterai
-Version: 0.2.6
+Version: 0.2.7
 Summary: An unofficial API for character.ai for Python
 Home-page: https://github.com/kramcat/CharacterAI
 Author: kramcat
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `characterai-0.2.6/setup.py` & `characterai-0.2.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 with open('README.md') as readme:
     long_description = readme.read()
 
 setup(
     name='characterai',
-    version='0.2.6',
+    version='0.2.7',
     author='kramcat',
     description='An unofficial API for character.ai for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kramcat/CharacterAI',
     packages=['characterai'],
-    install_requires=open('requirements.txt').read().strip().split('\n'),
+    install_requires=['playwright==1.32.1'],
     classifiers=[
         'Programming Language :: Python :: 3.9',
         'License :: OSI Approved :: MIT License',
     ],
 )
```


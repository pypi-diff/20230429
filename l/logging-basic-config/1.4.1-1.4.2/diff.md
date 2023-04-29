# Comparing `tmp/logging_basic_config-1.4.1.tar.gz` & `tmp/logging_basic_config-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/logging_basic_config-1.4.1.tar", last modified: Fri Apr 21 21:38:14 2023, max compression
+gzip compressed data, was "dist/logging_basic_config-1.4.2.tar", last modified: Fri Apr 28 17:25:08 2023, max compression
```

## Comparing `logging_basic_config-1.4.1.tar` & `logging_basic_config-1.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 msantino  (1000) msantino  (1000)        0 2023-04-21 21:38:14.000000 logging_basic_config-1.4.1/
--rw-r--r--   0 msantino  (1000) msantino  (1000)     1073 2023-04-20 20:50:29.000000 logging_basic_config-1.4.1/LICENSE
--rw-rw-r--   0 msantino  (1000) msantino  (1000)      997 2023-04-21 21:38:14.000000 logging_basic_config-1.4.1/PKG-INFO
--rw-r--r--   0 msantino  (1000) msantino  (1000)      536 2023-04-20 21:02:37.000000 logging_basic_config-1.4.1/README.md
-drwxrwxr-x   0 msantino  (1000) msantino  (1000)        0 2023-04-21 21:38:14.000000 logging_basic_config-1.4.1/logging_basic_config/
--rw-r--r--   0 msantino  (1000) msantino  (1000)       26 2023-04-20 20:55:50.000000 logging_basic_config-1.4.1/logging_basic_config/__init__.py
--rw-r--r--   0 msantino  (1000) msantino  (1000)     1273 2023-04-21 21:37:05.000000 logging_basic_config-1.4.1/logging_basic_config/config.py
-drwxrwxr-x   0 msantino  (1000) msantino  (1000)        0 2023-04-21 21:38:14.000000 logging_basic_config-1.4.1/logging_basic_config.egg-info/
--rw-rw-r--   0 msantino  (1000) msantino  (1000)      997 2023-04-21 21:38:14.000000 logging_basic_config-1.4.1/logging_basic_config.egg-info/PKG-INFO
--rw-rw-r--   0 msantino  (1000) msantino  (1000)      309 2023-04-21 21:38:14.000000 logging_basic_config-1.4.1/logging_basic_config.egg-info/SOURCES.txt
--rw-rw-r--   0 msantino  (1000) msantino  (1000)        1 2023-04-21 21:38:14.000000 logging_basic_config-1.4.1/logging_basic_config.egg-info/dependency_links.txt
--rw-rw-r--   0 msantino  (1000) msantino  (1000)        1 2023-04-21 21:38:14.000000 logging_basic_config-1.4.1/logging_basic_config.egg-info/not-zip-safe
--rw-rw-r--   0 msantino  (1000) msantino  (1000)       21 2023-04-21 21:38:14.000000 logging_basic_config-1.4.1/logging_basic_config.egg-info/top_level.txt
--rw-rw-r--   0 msantino  (1000) msantino  (1000)       38 2023-04-21 21:38:14.000000 logging_basic_config-1.4.1/setup.cfg
--rw-r--r--   0 msantino  (1000) msantino  (1000)      893 2023-04-21 21:37:39.000000 logging_basic_config-1.4.1/setup.py
+drwxrwxr-x   0 msantino  (1000) msantino  (1000)        0 2023-04-28 17:25:08.000000 logging_basic_config-1.4.2/
+-rw-r--r--   0 msantino  (1000) msantino  (1000)     1073 2023-04-20 20:50:29.000000 logging_basic_config-1.4.2/LICENSE
+-rw-rw-r--   0 msantino  (1000) msantino  (1000)      997 2023-04-28 17:25:08.000000 logging_basic_config-1.4.2/PKG-INFO
+-rw-r--r--   0 msantino  (1000) msantino  (1000)      536 2023-04-20 21:02:37.000000 logging_basic_config-1.4.2/README.md
+drwxrwxr-x   0 msantino  (1000) msantino  (1000)        0 2023-04-28 17:25:08.000000 logging_basic_config-1.4.2/logging_basic_config/
+-rw-r--r--   0 msantino  (1000) msantino  (1000)       26 2023-04-20 20:55:50.000000 logging_basic_config-1.4.2/logging_basic_config/__init__.py
+-rw-r--r--   0 msantino  (1000) msantino  (1000)     1270 2023-04-28 17:24:12.000000 logging_basic_config-1.4.2/logging_basic_config/config.py
+drwxrwxr-x   0 msantino  (1000) msantino  (1000)        0 2023-04-28 17:25:08.000000 logging_basic_config-1.4.2/logging_basic_config.egg-info/
+-rw-rw-r--   0 msantino  (1000) msantino  (1000)      997 2023-04-28 17:25:08.000000 logging_basic_config-1.4.2/logging_basic_config.egg-info/PKG-INFO
+-rw-rw-r--   0 msantino  (1000) msantino  (1000)      309 2023-04-28 17:25:08.000000 logging_basic_config-1.4.2/logging_basic_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 msantino  (1000) msantino  (1000)        1 2023-04-28 17:25:08.000000 logging_basic_config-1.4.2/logging_basic_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 msantino  (1000) msantino  (1000)        1 2023-04-28 17:25:08.000000 logging_basic_config-1.4.2/logging_basic_config.egg-info/not-zip-safe
+-rw-rw-r--   0 msantino  (1000) msantino  (1000)       21 2023-04-28 17:25:08.000000 logging_basic_config-1.4.2/logging_basic_config.egg-info/top_level.txt
+-rw-rw-r--   0 msantino  (1000) msantino  (1000)       38 2023-04-28 17:25:08.000000 logging_basic_config-1.4.2/setup.cfg
+-rw-r--r--   0 msantino  (1000) msantino  (1000)      893 2023-04-28 17:24:33.000000 logging_basic_config-1.4.2/setup.py
```

### Comparing `logging_basic_config-1.4.1/LICENSE` & `logging_basic_config-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `logging_basic_config-1.4.1/PKG-INFO` & `logging_basic_config-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logging_basic_config
-Version: 1.4.1
+Version: 1.4.2
 Summary: Basic logging configurations to easily use in many projects
 Home-page: https://github.com/msantino/logging-basic-config
 Author: Marcelo Santino
 Author-email: marcelo@santino.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `logging_basic_config-1.4.1/README.md` & `logging_basic_config-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `logging_basic_config-1.4.1/logging_basic_config/config.py` & `logging_basic_config-1.4.2/logging_basic_config/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from os import getenv
 import sys
 
 
 def config(
         logging_level : str = "INFO",
         libs_to_silence : list = None,
-        env_var_force_timestamp : list = None
+        env_var_hide_timestamp : list = None
     ):
     
     # Set higher level for external libs logging
     if libs_to_silence is None:
         libs_to_silence = [
             'botocore',
             'boto3',
@@ -22,18 +22,18 @@
         ]
     for lib in libs_to_silence:
             logging.getLogger(lib).setLevel(logging.ERROR)
 
     LOGGING_LEVEL = getenv('LOGGING_LEVEL', logging_level)
 
     # Local execution shows time. Remote executions logging has it's own timestamp adding
-    if env_var_force_timestamp is not None and getenv(env_var_force_timestamp, None) is not None:
-        log_format = '%(asctime)s - %(levelname)s - %(filename)s[%(lineno)s] %(message)s'
-    else:
+    if env_var_hide_timestamp is not None and getenv(env_var_hide_timestamp, None) is not None:
         log_format = '%(levelname)s - %(filename)s[%(lineno)s] %(message)s'
+    else:
+        log_format = '%(asctime)s - %(levelname)s - %(filename)s[%(lineno)s] %(message)s'
 
     logger = logging.getLogger()
     for h in logger.handlers:
         logger.removeHandler(h)
     handler = logging.StreamHandler(sys.stdout)
     handler.setFormatter(logging.Formatter(log_format))
     logger.addHandler(handler)
```

### Comparing `logging_basic_config-1.4.1/logging_basic_config.egg-info/PKG-INFO` & `logging_basic_config-1.4.2/logging_basic_config.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logging-basic-config
-Version: 1.4.1
+Version: 1.4.2
 Summary: Basic logging configurations to easily use in many projects
 Home-page: https://github.com/msantino/logging-basic-config
 Author: Marcelo Santino
 Author-email: marcelo@santino.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `logging_basic_config-1.4.1/setup.py` & `logging_basic_config-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 MYDIR = path.abspath(path.dirname(__file__))
 
 cmdclass = {}
 ext_modules = []
 
 setup(
     name='logging_basic_config',  
-    version='1.4.1',
+    version='1.4.2',
     author="Marcelo Santino",
     author_email="marcelo@santino.dev",
     description="Basic logging configurations to easily use in many projects",
     url='https://github.com/msantino/logging-basic-config',
     long_description=io.open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['tests']),
```


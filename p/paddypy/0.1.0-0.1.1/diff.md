# Comparing `tmp/paddypy-0.1.0.tar.gz` & `tmp/paddypy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddypy-0.1.0.tar", last modified: Fri Apr 21 08:32:52 2023, max compression
+gzip compressed data, was "paddypy-0.1.1.tar", last modified: Sat Apr 29 10:23:18 2023, max compression
```

## Comparing `paddypy-0.1.0.tar` & `paddypy-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 08:32:52.235098 paddypy-0.1.0/
--rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1795 2023-04-21 08:32:52.234597 paddypy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 08:32:52.218596 paddypy-0.1.0/paddypy/
--rw-rw-rw-   0        0        0      102 2023-04-17 12:26:22.000000 paddypy-0.1.0/paddypy/__init__.py
--rw-rw-rw-   0        0        0     5772 2023-04-17 12:26:22.000000 paddypy-0.1.0/paddypy/access.py
--rw-rw-rw-   0        0        0     2847 2023-04-21 08:31:43.000000 paddypy-0.1.0/paddypy/log.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:32:52.233599 paddypy-0.1.0/paddypy.egg-info/
--rw-rw-rw-   0        0        0     1795 2023-04-21 08:32:51.000000 paddypy-0.1.0/paddypy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-04-21 08:32:52.000000 paddypy-0.1.0/paddypy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 08:32:51.000000 paddypy-0.1.0/paddypy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-04-21 08:32:51.000000 paddypy-0.1.0/paddypy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-21 08:32:51.000000 paddypy-0.1.0/paddypy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 08:32:52.235098 paddypy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1449 2023-04-21 08:32:10.000000 paddypy-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:23:18.171106 paddypy-0.1.1/
+-rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1795 2023-04-29 10:23:18.170606 paddypy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 10:23:18.158605 paddypy-0.1.1/paddypy/
+-rw-rw-rw-   0        0        0      102 2023-04-17 12:26:22.000000 paddypy-0.1.1/paddypy/__init__.py
+-rw-rw-rw-   0        0        0     5772 2023-04-17 12:26:22.000000 paddypy-0.1.1/paddypy/access.py
+-rw-rw-rw-   0        0        0     3341 2023-04-29 10:17:29.000000 paddypy-0.1.1/paddypy/log.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:23:18.169606 paddypy-0.1.1/paddypy.egg-info/
+-rw-rw-rw-   0        0        0     1795 2023-04-29 10:23:17.000000 paddypy-0.1.1/paddypy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-04-29 10:23:18.000000 paddypy-0.1.1/paddypy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 10:23:17.000000 paddypy-0.1.1/paddypy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-04-29 10:23:17.000000 paddypy-0.1.1/paddypy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-29 10:23:17.000000 paddypy-0.1.1/paddypy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 10:23:18.171106 paddypy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1480 2023-04-29 10:22:54.000000 paddypy-0.1.1/setup.py
```

### Comparing `paddypy-0.1.0/LICENSE` & `paddypy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paddypy-0.1.0/PKG-INFO` & `paddypy-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.1.0/README.md` & `paddypy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `paddypy-0.1.0/paddypy/access.py` & `paddypy-0.1.1/paddypy/access.py`

 * *Files identical despite different names*

### Comparing `paddypy-0.1.0/paddypy/log.py` & `paddypy-0.1.1/paddypy/log.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 
 from functools import wraps
 import time
 import logging
 import datetime
+from opencensus.ext.azure.log_exporter import AzureLogHandler
 from . import access
 
 class CloudLogger():
-    def __init__(self, app_logger_name, module_name, logger_level=10):
+    def __init__(self, app_logger_name, module_name, applicationinsights_key=None, logger_level=10):
         self.LOGGER_LEVEL = logger_level
-        self.logger = self._get_logger(app_logger_name=app_logger_name, module_name=module_name)
+        self.logger = self._get_logger(app_logger_name=app_logger_name, module_name=module_name, applicationinsights_key=applicationinsights_key, logger_level=self.LOGGER_LEVEL)
 
         
-    def _get_logger(self, app_logger_name, module_name):
+    def _get_logger(self, app_logger_name, module_name, applicationinsights_key, logger_level):
         FMT = "[{levelname:^9}] {name}: {message}"
         FORMATS = {
             logging.DEBUG: FMT,
             logging.INFO: "\33[36m{fmt}\33[0m".format(fmt=FMT),
             logging.WARNING: "\33[33m{fmt}\33[0m".format(fmt=FMT),
             logging.ERROR: "\33[31m{fmt}\33[0m".format(fmt=FMT),
             logging.CRITICAL: "\33[1m\33[31m{fmt}\33[0m".format(fmt=FMT)
@@ -30,19 +31,24 @@
                 return formatter.format(record)
 
         
 
         handler = logging.StreamHandler()
         handler.setFormatter(CustomFormatter())
         logging.basicConfig(
-            level=self.LOGGER_LEVEL,
+            level=logger_level,
             handlers=[handler]
         )
 
         logger = logging.getLogger(app_logger_name).getChild(module_name)
+        # Add the AzureLogHandler for Application Insights
+        if applicationinsights_key:
+            azure_handler = AzureLogHandler(connection_string=str(applicationinsights_key))
+            azure_handler.setLevel(logger_level)
+            logger.addHandler(azure_handler)
         return logger
 
 
     def timeit(self, func):
         @wraps(func)
         def timeit_wrapper(*args, **kwargs):
             start_time = time.perf_counter()
```

### Comparing `paddypy-0.1.0/paddypy.egg-info/PKG-INFO` & `paddypy-0.1.1/paddypy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.1.0/setup.py` & `paddypy-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Collection of helpfull extensions'
 LONG_DESCRIPTION = 'Collection of helpfull extensions'
 
 # Setting up
 setup(
     name="paddypy",
     version=VERSION,
     author="Patrik",
     author_email="<patrikhartl@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['azure-appconfiguration>=1.1.0', 'texttable>=1.4.4', 'azure-identity>=1.5.0', 'azure-keyvault-secrets>=4.1.0'],
+    install_requires=['azure-appconfiguration>=1.1.1', 'texttable>=1.4.4', 'azure-identity>=1.5.0', 'azure-keyvault-secrets>=4.1.0', 'opencensus-ext-azure>=1.1.9'],
     keywords=['python', 'appconfiguration', 'azure'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```


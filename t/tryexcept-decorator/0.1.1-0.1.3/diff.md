# Comparing `tmp/tryexcept-decorator-0.1.1.tar.gz` & `tmp/tryexcept-decorator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tryexcept-decorator-0.1.1.tar", last modified: Sat Apr  8 12:48:38 2023, max compression
+gzip compressed data, was "tryexcept-decorator-0.1.3.tar", last modified: Sat Apr 29 07:17:05 2023, max compression
```

## Comparing `tryexcept-decorator-0.1.1.tar` & `tryexcept-decorator-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 12:48:38.232127 tryexcept-decorator-0.1.1/
--rw-rw-rw-   0        0        0     1094 2023-04-07 12:59:02.000000 tryexcept-decorator-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      448 2023-04-08 12:48:38.228157 tryexcept-decorator-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3266 2023-04-07 12:59:02.000000 tryexcept-decorator-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-08 12:48:38.235109 tryexcept-decorator-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      574 2023-04-08 12:48:27.000000 tryexcept-decorator-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 12:48:38.196367 tryexcept-decorator-0.1.1/tryexcept_decorator.egg-info/
--rw-rw-rw-   0        0        0      448 2023-04-08 12:48:37.000000 tryexcept-decorator-0.1.1/tryexcept_decorator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-04-08 12:48:37.000000 tryexcept-decorator-0.1.1/tryexcept_decorator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 12:48:37.000000 tryexcept-decorator-0.1.1/tryexcept_decorator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 12:48:37.000000 tryexcept-decorator-0.1.1/tryexcept_decorator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 07:17:05.705843 tryexcept-decorator-0.1.3/
+-rw-rw-rw-   0        0        0     1094 2023-04-07 12:59:02.000000 tryexcept-decorator-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      448 2023-04-29 07:17:05.704844 tryexcept-decorator-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2822 2023-04-27 15:12:18.000000 tryexcept-decorator-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-29 07:17:05.706844 tryexcept-decorator-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      574 2023-04-27 15:11:36.000000 tryexcept-decorator-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 07:17:05.700843 tryexcept-decorator-0.1.3/tryexcept_decorator.egg-info/
+-rw-rw-rw-   0        0        0      448 2023-04-29 07:17:05.000000 tryexcept-decorator-0.1.3/tryexcept_decorator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-04-29 07:17:05.000000 tryexcept-decorator-0.1.3/tryexcept_decorator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 07:17:05.000000 tryexcept-decorator-0.1.3/tryexcept_decorator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 07:17:05.000000 tryexcept-decorator-0.1.3/tryexcept_decorator.egg-info/top_level.txt
```

### Comparing `tryexcept-decorator-0.1.1/LICENSE` & `tryexcept-decorator-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tryexcept-decorator-0.1.1/setup.py` & `tryexcept-decorator-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tryexcept-decorator',
-    version='0.1.1',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[],
     author='Davide Di Grande',
     author_email='davidedigrande.dev@gmail.com',
     description='See README',
     url='https://github.com/davidedigrande/exception_handler_decorator',
     classifiers=[
```

